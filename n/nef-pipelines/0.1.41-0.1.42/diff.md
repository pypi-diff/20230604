# Comparing `tmp/nef_pipelines-0.1.41.tar.gz` & `tmp/nef_pipelines-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.41.tar", last modified: Sun May 21 14:33:58 2023, max compression
+gzip compressed data, was "nef_pipelines-0.1.42.tar", last modified: Sun Jun  4 15:55:22 2023, max compression
```

## Comparing `nef_pipelines-0.1.41.tar` & `nef_pipelines-0.1.42.tar`

### file list

```diff
@@ -1,384 +1,396 @@
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.517225 nef_pipelines-0.1.41/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.194884 nef_pipelines-0.1.41/.github/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.346278 nef_pipelines-0.1.41/.github/workflows/
--rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.41/.github/workflows/ci.yml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.371524 nef_pipelines-0.1.41/.idea/
--rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.41/.idea/.gitignore
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.41/.idea/.name
--rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.41/.idea/NFC.iml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.378198 nef_pipelines-0.1.41/.idea/inspectionProfiles/
--rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.41/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.41/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.41/.idea/modules.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.41/.idea/vcs.xml
--rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.41/.pre-commit-config.yaml
--rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.41/.readthedocs.yml
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.41/AUTHORS.md
--rw-r--r--   0 garythompson   (501) staff       (20)     3747 2023-05-21 14:33:32.000000 nef_pipelines-0.1.41/CHANGELOG.md
--rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.41/CONTRIBUTING.md
--rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.41/LICENSE.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-21 14:33:58.517928 nef_pipelines-0.1.41/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.41/README.md
--rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.41/TODO.md
--rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.41/pyproject.toml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.420488 nef_pipelines-0.1.41/references/
--rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.41/references/Nmr Experiment Nomenclature v2.docx
--rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.41/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
--rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.41/release_to_pypi.sh
--rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.41/requirements.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-05-21 14:33:58.520813 nef_pipelines-0.1.41/setup.cfg
--rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.41/setup.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.196515 nef_pipelines-0.1.41/src/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.437581 nef_pipelines-0.1.41/src/nef_pipelines/
--rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.41/src/nef_pipelines/VERSION
--rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.483392 nef_pipelines-0.1.41/src/nef_pipelines/data/
--rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.522436 nef_pipelines-0.1.41/src/nef_pipelines/lib/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    18119 2023-05-07 11:12:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15083 2023-05-21 10:50:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    21187 2023-04-30 15:31:02.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/spectra_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4191 2023-05-21 10:59:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10234 2023-04-26 19:21:33.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.526259 nef_pipelines-0.1.41/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/translation_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garythompson   (501) staff       (20)    23798 2023-05-20 12:39:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5335 2023-05-20 12:46:21.000000 nef_pipelines-0.1.41/src/nef_pipelines/main.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.526744 nef_pipelines-0.1.41/src/nef_pipelines/nef_app/
--rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.541052 nef_pipelines-0.1.41/src/nef_pipelines/tests/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.551539 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/__init__.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.560572 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_list.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.561663 nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.565697 nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.567189 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.569703 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     3610 2023-05-06 20:59:13.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_import_peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.570775 nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.587194 nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.599153 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.601611 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_delete.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1884 2023-05-16 09:49:59.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_list.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_rename.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_tabulate.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.619120 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.622078 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.633915 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.721788 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.750362 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.801095 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.804024 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.837308 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.839184 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.855641 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.857177 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifts/test_make_peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.862181 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.912707 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.945053 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      241 2023-04-26 21:06:34.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4311 2023-05-21 12:09:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2322 2023-05-16 09:41:29.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_sparky_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.980425 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/empty.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/header.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/test_agv.neff
--rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_header.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_nef_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     7641 2023-04-24 20:39:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_test.py
--rw-r--r--   0 garythompson   (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_util.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.982508 nef_pipelines-0.1.41/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.023205 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.028630 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_data/basic.seq
--rw-r--r--   0 garythompson   (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     3392 2023-05-21 11:56:45.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_import_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1551 2023-05-21 14:27:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_import_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8984 2023-05-21 14:27:42.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.043376 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.114938 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.130156 nef_pipelines-0.1.41/src/nef_pipelines/tools/
--rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.164161 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.169319 nef_pipelines-0.1.41/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.184455 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7414 2023-05-16 09:49:59.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.186767 nef_pipelines-0.1.41/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/res_assign.py_unused
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.207948 nef_pipelines-0.1.41/src/nef_pipelines/tools/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7145 2023-05-16 20:28:28.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/shifts/make_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.210415 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.211088 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.213451 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.217845 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/
--rw-r--r--   0 garythompson   (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.219645 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15433 2023-05-21 12:09:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/importers/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.221960 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.244582 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.249655 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-04-24 20:34:49.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.252169 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)      892 2023-05-21 10:50:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.264103 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.267115 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11657 2023-04-24 20:38:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.300090 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.308412 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3498 2023-04-24 20:38:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3151 2023-04-24 20:36:47.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)    20224 2023-04-24 21:17:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.315992 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.351483 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.361872 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2330 2023-04-24 20:38:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5787 2023-04-24 20:38:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.365683 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.369587 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    10943 2023-05-07 09:41:03.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.371699 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.391469 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pdbx/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.395773 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.399364 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.401394 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.403816 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6339 2023-04-24 20:32:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.408395 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.437163 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15804 2023-05-04 07:46:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.446559 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    16181 2023-05-21 12:09:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6463 2023-05-20 13:08:43.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8328 2023-05-15 12:35:13.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/sparky_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.449738 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.451599 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.454990 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/
--rw-r--r--   0 garythompson   (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.478916 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)     2925 2023-05-21 12:09:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2852 2023-05-21 11:00:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1899 2023-05-21 14:30:07.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)    22539 2023-05-21 14:29:12.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.485417 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.489902 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.515026 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.455047 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)    14639 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.41/tox.ini
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.364850 nef_pipelines-0.1.42/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.107114 nef_pipelines-0.1.42/.github/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.221578 nef_pipelines-0.1.42/.github/workflows/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.42/.github/workflows/ci.yml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.242321 nef_pipelines-0.1.42/.idea/
+-rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.42/.idea/.gitignore
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.42/.idea/.name
+-rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.42/.idea/NFC.iml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.248021 nef_pipelines-0.1.42/.idea/inspectionProfiles/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.42/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.42/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.42/.idea/modules.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.42/.idea/vcs.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.42/.pre-commit-config.yaml
+-rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.42/.readthedocs.yml
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.42/AUTHORS.md
+-rw-r--r--   0 garythompson   (501) staff       (20)     3974 2023-06-04 15:54:43.000000 nef_pipelines-0.1.42/CHANGELOG.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.42/CONTRIBUTING.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.42/LICENSE.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-06-04 15:55:22.365936 nef_pipelines-0.1.42/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.42/README.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      807 2023-05-21 15:23:42.000000 nef_pipelines-0.1.42/TODO.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.42/pyproject.toml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.272098 nef_pipelines-0.1.42/references/
+-rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.42/references/Nmr Experiment Nomenclature v2.docx
+-rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.42/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
+-rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.42/release_to_pypi.sh
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.42/requirements.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-06-04 15:55:22.370751 nef_pipelines-0.1.42/setup.cfg
+-rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.42/setup.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.108391 nef_pipelines-0.1.42/src/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.297602 nef_pipelines-0.1.42/src/nef_pipelines/
+-rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.42/src/nef_pipelines/VERSION
+-rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.351028 nef_pipelines-0.1.42/src/nef_pipelines/data/
+-rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.414313 nef_pipelines-0.1.42/src/nef_pipelines/lib/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    18119 2023-05-07 11:12:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15025 2023-05-24 21:08:05.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    23324 2023-06-04 15:15:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/spectra_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4191 2023-05-21 10:59:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10315 2023-06-04 10:57:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.417723 nef_pipelines-0.1.42/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/translation_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    24946 2023-05-24 21:08:07.000000 nef_pipelines-0.1.42/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5335 2023-05-20 12:46:21.000000 nef_pipelines-0.1.42/src/nef_pipelines/main.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.418104 nef_pipelines-0.1.42/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.451920 nef_pipelines-0.1.42/src/nef_pipelines/tests/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.463766 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/__init__.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.468343 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_list.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.475773 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.481781 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rwxrwxrwx   0 garythompson   (501) staff       (20)      315 2023-05-28 10:49:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)     3065 2023-05-28 10:49:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.483400 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.487728 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     3610 2023-05-06 20:59:13.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_import_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.489197 nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.507508 nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.522798 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.527488 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5990 2023-06-03 15:00:25.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_delete.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1884 2023-05-16 09:49:59.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_tabulate.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    17146 2023-06-04 15:49:53.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_unassign.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.547622 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.558240 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      240 2023-05-23 20:39:35.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
+-rw-r--r--   0 garythompson   (501) staff       (20)      240 2023-05-24 21:21:51.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sparky_CA.out
+-rw-r--r--   0 garythompson   (501) staff       (20)      480 2023-05-24 21:21:51.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sparky_all.out
+-rw-r--r--   0 garythompson   (501) staff       (20)     3331 2023-05-24 21:21:51.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5489 2023-05-24 21:22:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.588092 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.643595 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.674506 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.716590 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.724282 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.729450 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.731312 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.743593 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.745115 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifts/test_make_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.756683 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.773945 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.837902 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      241 2023-04-26 21:06:34.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4311 2023-05-21 12:09:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2370 2023-05-24 21:14:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_sparky_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.850342 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/header.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/test_agv.neff
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_header.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_nef_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     7641 2023-04-24 20:39:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_test.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/test_util.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.852061 nef_pipelines-0.1.42/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.892384 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.898994 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/basic.seq
+-rw-r--r--   0 garythompson   (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     3392 2023-05-21 11:56:45.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1551 2023-05-21 14:27:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8984 2023-05-21 14:27:42.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.912340 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.969737 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.003330 nef_pipelines-0.1.42/src/nef_pipelines/tools/
+-rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.019260 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.026904 nef_pipelines-0.1.42/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.049161 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garythompson   (501) staff       (20)      700 2023-06-04 15:15:37.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-05-21 15:19:25.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7414 2023-05-16 09:49:59.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8977 2023-05-21 15:22:30.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    18444 2023-06-04 15:49:53.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/unassign.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.056586 nef_pipelines-0.1.42/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/res_assign.py_unused
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.061250 nef_pipelines-0.1.42/src/nef_pipelines/tools/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7145 2023-05-21 16:48:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/shifts/make_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.42/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.064846 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.065378 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garythompson   (501) staff       (20)      480 2023-05-28 10:49:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.076138 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    16493 2023-05-28 10:49:25.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.079062 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/
+-rw-r--r--   0 garythompson   (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.083583 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15433 2023-05-21 12:09:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/importers/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.086102 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.089089 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.092400 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-04-24 20:34:49.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.095891 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)      964 2023-05-24 21:21:51.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.133047 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5933 2023-05-24 21:29:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.142334 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11115 2023-05-24 21:25:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11657 2023-04-24 20:38:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.154233 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.168738 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3498 2023-04-24 20:38:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3151 2023-04-24 20:36:47.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    20224 2023-04-24 21:17:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.173606 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.189912 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.214559 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2330 2023-04-24 20:38:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5787 2023-04-24 20:38:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.216766 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.221906 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10943 2023-05-07 09:41:03.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.224655 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.226742 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pdbx/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.230970 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.237257 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.239984 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.259334 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6339 2023-04-24 20:32:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.269052 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.274424 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15804 2023-05-21 16:37:56.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.292371 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7995 2023-05-24 21:20:29.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6463 2023-05-20 13:08:43.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-05-24 21:17:30.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17287 2023-05-24 21:17:28.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/sparky_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.302598 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.309013 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.317524 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/
+-rw-r--r--   0 garythompson   (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.330114 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)     2925 2023-05-21 12:09:19.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2852 2023-05-21 11:00:00.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1899 2023-05-21 14:30:07.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    22539 2023-05-21 14:29:12.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.341735 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.348385 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:22.361227 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-06-04 15:55:21.316404 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-06-04 15:55:20.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)    15289 2023-06-04 15:55:21.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-06-04 15:55:20.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-06-04 15:55:20.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-06-04 15:55:20.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-06-04 15:55:20.000000 nef_pipelines-0.1.42/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.42/tox.ini
```

### Comparing `nef_pipelines-0.1.41/.github/workflows/ci.yml` & `nef_pipelines-0.1.42/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.42/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/.pre-commit-config.yaml` & `nef_pipelines-0.1.42/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/CHANGELOG.md` & `nef_pipelines-0.1.42/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -152,8 +152,14 @@
 ## version 0.1.40
 
 fix a bug: make peaks faaled on generating empty peak lists
 
 ## version 0.1.41
 
 add importers for xeasy [flya dialect] sequences, peaks and shifts
-a  number of gug fixes in the sparky and exhdnia tools
+a  number of bug fixes in the sparky and echidna tools
+
+## version 0.1.42
+
+add the ability to unassign frames in general with support for different sequence_code
+unassignment strategies and the ability to choose what is unassigned (chain_code, sequence_code
+residue_name atom_name)
```

### Comparing `nef_pipelines-0.1.41/CONTRIBUTING.md` & `nef_pipelines-0.1.42/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/LICENSE.txt` & `nef_pipelines-0.1.42/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/PKG-INFO` & `nef_pipelines-0.1.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.41
+Version: 0.1.42
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.41/README.md` & `nef_pipelines-0.1.42/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/TODO.md` & `nef_pipelines-0.1.42/TODO.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 * nmrview output - to do  '!1'
 * nmrpipe output -to do -wait
 * Xplor xplor just xplor violations to nef - do '!2'
 * Aria - needs dedicated time -soon but not immediate
 * nmrstar -peaks sequence - wait
 * Translator -do '!3'
-* xEasy shifts - not important currently
+
 * Xplor shifts export? - can wait
 * missing frame update bug - important '!4'
 * add pipe functions '!5' - started
 * update merging and replacement of save frames and support of empty save frames
 * make tools update meta data
 * test on ubuntu latest
 
 * Missing tests -done
 * mars - nef2mars - done
 * renumber chains -  done
 * test hannah's problems - done
 * Fasta export - done
-
+* xEasy shifts - done
 release - done
```

### Comparing `nef_pipelines-0.1.41/references/Nmr Experiment Nomenclature v2.docx` & `nef_pipelines-0.1.42/references/Nmr Experiment Nomenclature v2.docx`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf` & `nef_pipelines-0.1.42/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/release_to_pypi.sh` & `nef_pipelines-0.1.42/release_to_pypi.sh`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/setup.cfg` & `nef_pipelines-0.1.42/setup.cfg`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/setup.py` & `nef_pipelines-0.1.42/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.42/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/peak_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,18 +70,18 @@
     ShiftData,
 )
 from nef_pipelines.lib.util import (
     _row_to_table,
     exit_error,
     is_float,
     is_int,
+    remove_duplicates_stable,
     unused_to_empty_string,
     unused_to_none,
 )
-from nef_pipelines.transcoders.mars.exporters.fragments import remove_duplicates_stable
 
 
 class BadPositionException(Exception):
     """
     The position of a peak in the frame couldn't be converted to a float
     """
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/sequence_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import string
 from collections import Counter
 from dataclasses import replace
 from enum import auto
 from pathlib import Path
 from textwrap import dedent
-from typing import Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 from ordered_set import OrderedSet
 from pynmrstar import Entry, Loop, Saveframe
 from strenum import LowercaseStrEnum
 
 from nef_pipelines.lib.constants import NEF_UNKNOWN
 from nef_pipelines.lib.nef_lib import UNUSED, loop_row_namespace_iter
@@ -17,14 +17,15 @@
 from nef_pipelines.lib.structures import AtomLabel, Linking, SequenceResidue
 from nef_pipelines.lib.util import (
     chunks,
     exit_error,
     get_display_file_name,
     is_int,
     read_from_file_or_exit,
+    strip_characters_right,
 )
 
 
 class MoleculeType(LowercaseStrEnum):
     PROTEIN = auto()
     RNA = auto()
     DNA = auto()
@@ -698,7 +699,77 @@
     :param sequence: a list of sequence residues
     :return: the lookup table
     """
     result: Dict[Tuple[str, int], str] = {}
     for residue in sequence:
         result[residue.chain_code, residue.sequence_code] = residue.residue_name
     return result
+
+
+def atom_sort_key(item: AtomLabel) -> Tuple[Any, ...]:
+    """
+
+    key based sorter for atom labels that enables them to be sorted in a sensible order including sequence codes
+    which are not numeric...
+
+    :param item: an atom label
+    :return: a tuple baed on the atom label which gives the correct sort order
+    """
+
+    try:
+        items = []
+        residue = item.residue
+        chain_code = residue.chain_code.strip()
+        prefix, numbers = strip_characters_right(chain_code, string.digits)
+
+        if numbers == "":
+            numbers = 0, ""
+        if is_int(numbers):
+            numbers = int(numbers), ""
+        else:
+            numbers = 0, numbers
+
+        if UNUSED in prefix:
+            order = 2
+        elif "@" in prefix or "#" in prefix:
+            order = 1
+        else:
+            order = 0
+
+        items.append([order, prefix, *numbers])
+
+        sequence_code = str(residue.sequence_code).strip()
+        prefix, numbers = strip_characters_right(sequence_code, (string.digits + "+-"))
+
+        if is_int(numbers):
+            numbers = [int(numbers), "", 0]
+        elif "+" in numbers or "-" in numbers:
+            for splitter in "+-":
+                if splitter in numbers:
+                    numbers = numbers.rsplit(splitter, maxsplit=1)
+                    numbers = [numbers[0], splitter, numbers[1]]
+                    break
+            if is_int(numbers[0]) and is_int(numbers[-1]):
+                numbers[0] = int(numbers[0])
+                numbers[-1] = int(numbers[-1])
+        else:
+            numbers = [0, numbers, 0]
+
+        if UNUSED in prefix:
+            order = 2
+        elif "@" in prefix or "#" in prefix:
+            order = 1
+        else:
+            order = 0
+
+        items.append([order, prefix, *numbers])
+
+        items.append(residue.residue_name.lower())
+        items.append(item.atom_name.lower())
+    except Exception as e:
+        msg = f"""
+            I can't sort {item} because it doesn't seem to be behaving like an AtomLabel...
+            [{e}]
+        """
+        raise ValueError(msg)
+
+    return items
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/shift_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/spectra_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/spectra_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/structures.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/test_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,38 +121,38 @@
     lines_reported = reported.split("\n")
 
     if ignore_empty:
         lines_expected = [line for line in lines_expected if len(line.strip()) != 0]
         lines_reported = [line for line in lines_reported if len(line.strip()) != 0]
 
     zip_lines = zip_longest(lines_expected, lines_reported, fillvalue="")
-    for i, (expected_line, reported_line) in enumerate(zip_lines):
+    for i, (expected_line, reported_line) in enumerate(zip_lines, start=1):
 
         expected_line_stripped = expected_line.strip()
         reported_line_stripped = reported_line.strip()
 
         if squash_spaces:
             expected_line_stripped = " ".join(expected_line_stripped.split())
             reported_line_stripped = " ".join(reported_line_stripped.split())
 
         if reported_line_stripped != expected_line_stripped:
 
-            for line in lines_expected:
-                print(f"exp|{line}")
+            for line_no, line in enumerate(lines_expected, start=1):
+                print(f"exp|{line_no}|{line}")
             print()
 
-            for line in lines_reported:
-                print(f"rep|{line}")
+            for line_no, line in enumerate(lines_reported, start=1):
+                print(f"rep|{line_no}|{line}")
             print()
 
             print("line that caused the error:")
             print()
 
-            print(f"exp|{i}|  |{expected_line_stripped}|")
-            print(f"rep|{i}|  |{reported_line_stripped}|")
+            print(f"exp|{i}| {expected_line.strip()}|")
+            print(f"rep|{i}| {reported_line.strip()}|")
 
         assert reported_line_stripped == expected_line_stripped
 
 
 def isolate_frame(target: str, frame_name: str) -> Optional[str]:
     """
     Extract one frame from a NEF file by name as a string
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/translation_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/translation_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.42/src/nef_pipelines/lib/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,26 @@
 import sys
 import traceback
 from argparse import Namespace
 from enum import auto
 from math import floor
 from pathlib import Path
 from textwrap import dedent
-from typing import Any, Dict, Iterator, List, Optional, TextIO, Tuple, TypeVar, Union
+from typing import (
+    Any,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    TextIO,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 import click
 from cacheable_iter import iter_cache
 from pynmrstar import Entry, Loop, Saveframe
 from strenum import StrEnum
 from tabulate import tabulate
 
@@ -888,7 +899,36 @@
     comment = None
     if comment_character in line:
         index = line.index(comment_character)
         comment = line[index + 1 :]
         line = line[:index]
 
     return line, comment
+
+
+# https://stackoverflow.com/questions/480214/how-do-i-remove-duplicates-from-a-list-while-preserving-order
+def remove_duplicates_stable(seq: Iterable) -> List:
+
+    """
+    remove  duplicates from a list while preseving its order, so for example
+    [1 2 2 3 45 2 1 6] would yield 1 2 3 4 5 6
+    :param seq: the iteratble to remove duplicates from
+    :return: the original iterable without the duplicates
+
+    TODO: could this be recast as an iterable returning an iterable
+    """
+
+    seen = set()
+    seen_add = seen.add
+    return [x for x in seq if not (x in seen or seen_add(x))]
+
+
+# https://stackoverflow.com/questions/21303224/iterate-over-all-pairs-of-consecutive-items-in-a-list
+def iter_consecutive_pairs(seq: Iterator) -> Iterator[Tuple]:
+    """
+    iterate over consecutive pairs from a list, for example for the list [1, 7, 3, 5]
+    this will yield the items (1,7), (7,3), (3,5)
+    :param seq: the sequence to iterate pairs from
+    :return: an iteration over the consecutive pairs as tuples
+    """
+    for first, second in zip(seq, seq[1:]):
+        yield first, second
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/main.py` & `nef_pipelines-0.1.42/src/nef_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/conftest.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_import_peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/echidna/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/test_sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/fasta/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_rename.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pales/test_template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/pdbx/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/shifts/test_make_peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/shifts/test_make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_sparky_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/sparky/test_sparky_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         ("HN", "A", "11", "HN", "A", "11"),
         ("?", "", "", "", "A", "11"),
         ("T17H7", "T", "17", "H7", "A", "11"),
         ("?N", "A", "11", "N", "A", "11"),
         ("G16H8", "G", "16", "H8", "A", "11"),
         ('T17H2"', "T", "17", 'H2"', "A", "11"),
         ("H1'", "A", "11", "H1'", "A", "11"),
+        ("N25CA", "N", "25", "CA", None, None),
     ],
 )
 def test_split_assignment(
     input,
     expected_residue_name,
     expected_residue_number,
     expected_atom_name,
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/ubiquitin_short.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_data/ubiquitin_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_util.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_data/basic.peaks` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/basic.peaks`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_import_peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_import_sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_import_shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/about.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/chains/renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,7 +15,8 @@
 
     # import of specific importers must be after app creation to avoid circular imports
     import nef_pipelines.tools.frames.delete  # noqa: F401
     import nef_pipelines.tools.frames.insert  # noqa: F401
     import nef_pipelines.tools.frames.list  # noqa: F401
     import nef_pipelines.tools.frames.rename  # noqa: F401
     import nef_pipelines.tools.frames.tabulate  # noqa: F401
+    import nef_pipelines.tools.frames.unassign  # noqa: F401
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/rename.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     "volume_uncertainty": "vol-err",
     "height_uncertainty": "height-err",
     "position": "pos",
     "position_uncertainty": "pos-err",
     "ccpn_figure_of_merit": "merit",
     "ccpn_annotation": "ann",
     "ccpn_peak_list_serial": "ccpn-serial",
+    "atom-name": "atom",
 }
 
 
 # noinspection PyUnusedLocal
 @frames_app.command(no_args_is_help=True)
 def tabulate(
     pipe: Path = typer.Option(
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/shifts/make_peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/shifts/make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.42/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/importers/peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/echidna/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/fasta/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,8 +19,9 @@
     app.add_typer(import_app, name="import", help="- import mars [shifts]")
 
     # import of specific importers must be after app creation to avoid circular imports
     import nef_pipelines.transcoders.mars.exporters.fragments  # noqa: F401
     import nef_pipelines.transcoders.mars.exporters.input  # noqa: F401
     import nef_pipelines.transcoders.mars.exporters.sequence  # noqa: F401
     import nef_pipelines.transcoders.mars.exporters.shifts  # noqa: F401
+    import nef_pipelines.transcoders.mars.importers.peaks  # noqa: F401
     import nef_pipelines.transcoders.mars.importers.shifts  # noqa: F401
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 # original implementation by esther
 import sys
 from pathlib import Path
 from string import digits
-from typing import Iterable, Iterator, List, Tuple
+from typing import List, Tuple
 
 import typer
 from pynmrstar import Entry, Saveframe
 from tabulate import tabulate
 
 from nef_pipelines.lib.nef_lib import (
     loop_row_namespace_iter,
     read_entry_from_file_or_stdin_or_exit_error,
 )
 from nef_pipelines.lib.structures import LineInfo
-from nef_pipelines.lib.util import STDIN, end_with_ordinal, exit_error
+from nef_pipelines.lib.util import (
+    STDIN,
+    end_with_ordinal,
+    exit_error,
+    iter_consecutive_pairs,
+    remove_duplicates_stable,
+)
 from nef_pipelines.transcoders.mars import export_app
 
 NMR_RESIDUE = "nmr_residue"
 
 NMR_CHAIN = "nmr_chain"
 
 STDOUT_PATH = "-"
 
 app = typer.Typer()
 
 # TODO: name translations
 # TODO: correct weights
-# TODO: move utuilities to lib
+# TODO: move utilities to lib
 # TODO: support multiple chains
 
 REMOVE_DIGITS = str.maketrans("", "", digits)
 
 
 def has_numbers(input: str) -> bool:
     return any(char.isdigit() for char in input)
@@ -48,15 +54,15 @@
     ),
     output_file: str = typer.Argument(
         None,
         help="file name to output to [default <entry_id>_fix_con.tab] for stdout use -",
         metavar="<MARS_SHIFT_FILE>",
     ),
 ):
-    """- convert nef chemical shifts to mars"""
+    """- convert nef chemical shifts to mars fragments"""
 
     entry = read_entry_from_file_or_stdin_or_exit_error(input)
 
     output_file = (
         f"{entry.entry_id}_fix_ass.tab" if output_file is None else output_file
     )
 
@@ -66,28 +72,23 @@
     file_h = sys.stdout if output_file == "-" else open(output_file, "w")
 
     print(tabulate(table, tablefmt="plain"), file=file_h)
 
     if output_file != STDOUT_PATH:
         file_h.close()
 
-    if output_file != STDOUT_PATH:
-        if not sys.stdout.isatty():
-            print(entry)
+    if output_file != STDOUT_PATH and not sys.stdout.isatty():
+        print(entry)
 
 
 def _format_table(table: List[List[Tuple[str, str]]]) -> List[List[str]]:
     max_overall_elem_length = 0
     for chain in table:
-        max_elem_length = max([len(" ".join(prs)) for prs in chain])
-        max_overall_elem_length = (
-            max_elem_length
-            if max_elem_length > max_overall_elem_length
-            else max_overall_elem_length
-        )
+        max_elem_length = max(len(" ".join(prs)) for prs in chain)
+        max_overall_elem_length = max(max_elem_length, max_overall_elem_length)
     for chain in table:
         for i, prs in enumerate(chain):
             pr_length = len(prs[0]) + len(prs[1])
             pad = " " * (max_overall_elem_length - pr_length)
             pr_pair = f"{prs[0]}{pad}{prs[1]}"
             chain[i] = pr_pair
     return table
@@ -101,27 +102,28 @@
 
 def _build_connected_pseudo_residues(connected_residues):
     table = []
     ends = []
     for chain_code, residue_codes in connected_residues.items():
         chain = [
             (f"PR_{first}", f"PR_{second}")
-            for first, second in overlapped_pairs(residue_codes)
+            for first, second in iter_consecutive_pairs(residue_codes)
         ]
         ends.append(f"#{chain_code}")
         table.append(chain)
 
     return table
 
 
 def _get_connected_residues_and_chains(frame: Saveframe, entry: Entry):
-    connected_chains = set()
-    for chain in loop_row_namespace_iter(frame.get_loop(NMR_CHAIN)):
-        if chain.is_connected:
-            connected_chains.add(chain.short_name)
+    connected_chains = {
+        chain.short_name
+        for chain in loop_row_namespace_iter(frame.get_loop(NMR_CHAIN))
+        if chain.is_connected
+    }
     connected_residues = {}
     nmr_residue_loop = frame.get_loop(NMR_RESIDUE)
     for line_no, residue in enumerate(
         loop_row_namespace_iter(nmr_residue_loop), start=1
     ):
         chain_code = residue.chain_code
 
@@ -144,16 +146,15 @@
         exit_error(f"no assignment frame found in entry {entry.name}")
     if len(frames) > 1:
         msg = f"""\
                     there should only be one assignment frame i found {len(frames)} in entry {entry.name}
                     there names were {' '.join([frame.name for frame in frames])}
             """
         exit_error(msg)
-    frame = frames[0]
-    return frame
+    return frames[0]
 
 
 def _get_connected_residue_or_exit_error(residue, line_info: LineInfo):
     sequence_code = residue.sequence_code
     if sequence_code.startswith("@"):
         sequence_code = sequence_code.lstrip("@")
         sequence_code_fields = sequence_code.split("-")
@@ -165,36 +166,18 @@
                 {line_info.line}
             """
             exit_error(msg)
         sequence_code = sequence_code_fields[0]
     return sequence_code
 
 
-# https://stackoverflow.com/questions/480214/how-do-i-remove-duplicates-from-a-list-while-preserving-order
-def remove_duplicates_stable(seq: Iterable) -> List:
-
-    seen = set()
-    seen_add = seen.add
-    return [x for x in seq if not (x in seen or seen_add(x))]
-
-
-# https://stackoverflow.com/questions/21303224/iterate-over-all-pairs-of-consecutive-items-in-a-list
-def overlapped_pairs(seq: Iterator) -> Iterator[Tuple]:
-    for first, second in zip(seq, seq[1:]):
-        yield first, second
-
-
 def _filter_headings_by_pseudoatoms(base_headers, pseudo_residues):
     atom_names = set()
     for pseudo_residue in pseudo_residues.values():
         for pseudo_atom in pseudo_residue.values():
             offset = (
                 f"-{pseudo_atom.negative_offset}"
                 if pseudo_atom.negative_offset == 1
                 else ""
             )
             atom_names.add(f"{pseudo_atom.atom_name.upper()}{offset}")
-    headers = []
-    for header in base_headers:
-        if header == "" or header in atom_names:
-            headers.append(header)
-    return headers
+    return [header for header in base_headers if header == "" or header in atom_names]
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pdbx/importers/sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/pdbx/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/sparky_lib.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,251 +1,260 @@
 import string
 import sys
+from collections import namedtuple
 from itertools import zip_longest
-from pathlib import Path
-from textwrap import dedent
-from typing import Dict, List
-
-import typer
-from fyeah import f
-
-from nef_pipelines.lib.isotope_lib import ATOM_TO_ISOTOPE
-from nef_pipelines.lib.nef_lib import (
-    UNUSED,
-    add_frames_to_entry,
-    read_or_create_entry_exit_error_on_bad_file,
-)
-from nef_pipelines.lib.peak_lib import peaks_to_frame
-from nef_pipelines.lib.sequence_lib import MoleculeTypes, sequence_from_entry
-from nef_pipelines.lib.structures import LineInfo, NewPeak, PeakFitMethod, ShiftData
-from nef_pipelines.lib.translation_lib import translate_new_peak
-from nef_pipelines.lib.util import (
-    STDIN,
-    exit_error,
-    is_float,
-    parse_comma_separated_options,
-)
-from nef_pipelines.transcoders.sparky import import_app
-from nef_pipelines.transcoders.sparky.importers.shifts import (
-    _exit_if_chain_codes_and_file_name_dont_match,
-)
-from nef_pipelines.transcoders.sparky.sparky_lib import parse_assignments
-
-
-# TODO: this needs to be moved to a library
-class SparkyPeakListException(Exception):
-    pass
-
+from typing import Dict, List, Tuple
 
-class IncompatibleDimensionTypesException(SparkyPeakListException):
-    pass
-
-
-app = typer.Typer()
-
-DEFAULT_NUCLEI_HELP = (
-    "nuclei to use for each dimension, if not defined they are guessed from the assignments"
-    "or an error is reported"
+from nef_pipelines.lib.nef_lib import UNUSED
+from nef_pipelines.lib.sequence_lib import (
+    TRANSLATIONS_1_3,
+    MoleculeType,
+    residues_to_residue_name_lookup,
 )
+from nef_pipelines.lib.structures import (
+    AtomLabel,
+    LineInfo,
+    NewPeak,
+    PeakFitMethod,
+    Residue,
+    SequenceResidue,
+    ShiftData,
+)
+from nef_pipelines.lib.util import exit_error, is_float, strip_characters_left
 
+#
+# sparky docs
+#
+# Make peaks on a spectrum from a peak list file (rp).
+#
+# Peaks are read from a peak list file and placed on the selected spectrum.
+# The file should contain a line for each peak. The line should have an
+# assignment followed by chemical shifts for each axis. For example
+#
+# 	C2H5-G1H1      5.395      6.030
+# The assignment can contain ? components. It can omit a group name for a component
+# -- the shorthand G1H1'-H2' where the second group is omitted is equivalent to G1H1'-G1H2'.
+# The residue name is separated from the atom name by looking for a residue number followed
+# by one of the letters H, C, N, Q, or M (upper or lower case). Extra columns become the
+# peak note. Peaks for 3-D or 4-D spectra can be read.
+#
+# what does sparky do with multiple chains?
+#
+# what does ga mean in the sparky output after a volume
+#
+# why does sparky sometime have ga after a volume I presume it's a gausiann peak fit?
+# comment gst 19/04/2023 is ga for a gaussian peak fit?
+#
+#  Assignment       w1      w2      Volume     lw1 (hz)   lw2 (hz)
+#
+#    G16H3'-H8    4.905   8.010   7.15e+06 ga    28.6       20.0
+#    G16H4'-H8    4.439   8.013   5.42e+06 ga    35.3       16.9
+#  T17H6-G16H8    7.205   8.004   1.68e+06
+#  T17H7-G16H8    1.459   8.008   2.09e+07 ga    27.5       24.1
+#   T17H2"-H1'    2.509   5.840   4.68e+07 ga    41.2       17.6
+#
+# what does ta display in a sparky project
+# how does sparky cope with complexes where peaks are between chains
+# which it doesn't define
+#
+
+SparkyAtomLabel = namedtuple("SparkyAtomLabel", "residue_number residue_name atom_name")
+
+
+def parse_single_assignment(
+    assignment: str,
+    previous_residue_name: str = None,
+    previous_residue_number: str = None,
+) -> Tuple[str, str, str]:
+
+    """
+    Parse a single sparky assignment of the form ?, G16H4', H8, T17H6, G16H8 into a tuple of residue_number,
+    residue_name and atom_name. To allow for processing of abbreviated assignments of the form G16H4'-H8 a previous
+    residue number and residue name may be passed in [in this casefor H8  they would be G and 16 to match G16H4']
+
+    :param assignment: the single sparky assignments
+    :param previous_residue_name: a previous residue name to use for an abbreviated assignment
+    :param previous_residue_number: a previous residue number to use for an abbreviated assignment
+    :return: a tuple of the form (residue_number, residue_name , atom_name)
+    """
+
+    target = assignment
+
+    # remove a residue name or question mark
+    residue_name, target = strip_characters_left(target, string.ascii_letters)
+    if len(target) == 0:
+        target = residue_name
+        residue_name = ""
+
+    if target[0] == "?" and len(target) > 0:
+        target = target[1:]
+        residue_name = ""
+
+    # remove residue numbers or question mark
+    residue_number, target = strip_characters_left(target, string.digits)
+
+    if len(residue_number) == 0 and len(target) != 0 and target[0] == "?":
+        target = target[1:]
+        residue_number = ""
+
+    if len(target) > 0:
+        atom_name = target
+    else:
+        atom_name = ""
+
+    # residue name is separated from the atom name by looking for a residue number followed
+    # by one of the letters H, C, N, Q, or M ergo a residue name that starts with one of these
+    # must be wrong, and we have split an atom (though we don't actually need this test?)
+    residue_lower = residue_name.lower()
+    nmr_atoms_lower = "HCNQM".lower()
+    atom_starts_with_nmr_lower = False
+    atom_name_lower = atom_name.lower()
+    len_atom_name = len(atom_name)
+    if len_atom_name > 0 and atom_name_lower[0] in nmr_atoms_lower:
+        atom_starts_with_nmr_lower = True
+
+    if (
+        not atom_starts_with_nmr_lower
+        and residue_name != ""
+        and residue_lower in nmr_atoms_lower
+    ):
+        atom_name = f"{residue_name}{residue_number}{atom_name}"
+        residue_name = ""
+        residue_number = ""
+
+    if (
+        residue_number == ""
+        and previous_residue_number is not None
+        and residue_name == ""
+        and previous_residue_name is not None
+        and atom_name != ""
+    ):
+        residue_number = previous_residue_number
+        residue_name = previous_residue_name
+
+    if residue_name == "" and residue_number == "":
+        for i, character in enumerate(atom_name):
+            if character.lower() in "HCNQM".lower():
+                if i > 0 and atom_name[i - 1] in string.digits:
+                    residue_name_and_number = atom_name[:i]
+                    atom_name = atom_name[i:]
+
+                    residue_name = residue_name_and_number.rstrip(string.digits)
+
+                    residue_number = residue_name_and_number[-len(residue_name) :]
+
+    return SparkyAtomLabel(residue_number, residue_name, atom_name)
+
+
+def parse_assignments(
+    assignments: str,
+    chain_code: str,
+    sequence: List[SequenceResidue],
+    molecule_type: MoleculeType,
+    line_info: LineInfo,
+    allow_pseudo_atoms=False,
+) -> List[AtomLabel]:
+
+    """
+    take a sparky assignment of the form ?, G16H4'-H8 or T17H6-G16H8 into atom labels
+
+    :param assignments: a single assignment or a - separated assignment [including abbreviated assignments]
+    :param chain_code: the chain code to use
+    :param sequence: the sequence to get residue names from and to check the read residue names agains
+    :param molecule_type: the type of the molecule DNA RNS protein etc.
+    :param line_info: file and line  information for error reporting
+    :param allow_pseudo_atoms: if true ignore residue names which aren't in the molecule_type
+    :return: a list of AtomLabels
+    """
 
-# noinspection PyUnusedLocal
-@import_app.command(no_args_is_help=True)
-def peaks(
-    chain_codes: List[str] = typer.Option(
-        None,
-        "--chains",
-        help="chain codes as a list of names separated by commas, repeated calls will add further chains [default A] "
-        "one per file. If only one chain code is supplied it applies to all files",
-        metavar="<CHAIN-CODES>",
-    ),
-    frame_name: str = typer.Option(
-        "sparky_{file_name}",
-        "-f",
-        "--frame-name",
-        help="a templated name for the frame {file_name} will be replaced by input filename",
-    ),
-    input: Path = typer.Option(
-        STDIN,
-        "-i",
-        "--in",
-        metavar="|PIPE|",
-        help="input to read NEF data from [- is stdin]",
-    ),
-    file_names: List[Path] = typer.Argument(
-        ..., help="input files of type peaks.txt", metavar="<SPARKY-peaks>.txt"
-    ),
-    nuclei: List[str] = typer.Option([], help=DEFAULT_NUCLEI_HELP),
-    default_chain_code: str = typer.Option(
-        "A",
-        "-c",
-        "--chain-code",
-        help="default chain code to use if none is provided in the file",
-    ),
-    molecule_type: MoleculeTypes = typer.Option(
-        MoleculeTypes.PROTEIN, help="the type of molecule"
-    ),
-    no_validate: bool = typer.Option(
-        False,
-        help="if set don't validate the peaks against the input sequence if provided",
-    ),
-    spectrometer_frequency: float = typer.Option(
-        600.123456789, help="spectrometer frequency in MHz"
-    ),
-):
-    """convert sparky peaks file <SPARKY-PEAKS>.txt to NEF"""
-
-    chain_codes = parse_comma_separated_options(chain_codes)
-
-    if not chain_codes:
-        chain_codes = ["A"]
+    residue_name_lookup = residues_to_residue_name_lookup(sequence)
 
-    # make this a library function
-    _exit_if_chain_codes_and_file_name_dont_match(chain_codes, file_names)
+    residue_name_translations = TRANSLATIONS_1_3[molecule_type]
 
-    entry = read_or_create_entry_exit_error_on_bad_file(input)
+    fields = assignments.split("-")
 
-    sequence = sequence_from_entry(entry) if not no_validate else None
+    result = []
+    last_sequence_code = None
+    last_residue_name = None
 
-    nuclei = parse_comma_separated_options(nuclei)
+    for field in fields:
 
-    file_names_and_lines = {}
-    for file_name, chain_code in zip_longest(file_names, chain_codes, fillvalue=None):
+        sequence_code, residue_name, atom_name = parse_single_assignment(
+            field,
+            previous_residue_number=last_sequence_code,
+            previous_residue_name=last_residue_name,
+        )
 
-        if file_name is None:
-            continue
+        if sequence_code == "":
+            sequence_code = UNUSED
+        if residue_name == "":
+            residue_name = UNUSED
+
+        if residue_name_translations is not None and residue_name is not UNUSED:
+
+            if residue_name in residue_name_translations:
+                translated_residue_name = residue_name_translations[residue_name]
+            elif allow_pseudo_atoms:
+                translated_residue_name = residue_name
+            else:
+                msg = f"""
+                    The residue name {residue_name} is not defined for the molecule type {molecule_type}
+                    at line {line_info.line_no} in file {line_info.file_name} the line was
+                    {line_info.line}
+                """
+                exit_error(msg)
 
-        if chain_code is None:
-            chain_code = chain_codes[-1]
+        residue_name_key = (chain_code, sequence_code)
 
-        try:
-            with open(file_name, "r") as fp:
-                lines = fp.readlines()
-        except IOError as e:
+        if residue_name == UNUSED and residue_name_lookup is None:
             msg = f"""
-                    while reading sparky peaks file {file_name} there was an error reading the file
-                    the error was: {e}
-                """
-            exit_error(msg, e)
+                no sequence was loaded and the assignment {assignments} while it has a sequence code {sequence_code}
+                and chain code {chain_code} doesn't define a residue type, please provide a sequence in the input
+                stream
+            """
+            exit_error(msg)
+        else:
 
-        file_names_and_lines[file_name] = lines
+            if (
+                residue_name_lookup is not None
+                and residue_name_key in residue_name_lookup
+            ):
+                translated_residue_name = residue_name_lookup[residue_name_key]
 
-    entry = pipe(
-        entry,
-        frame_name,
-        file_names_and_lines,
-        chain_code,
-        sequence,
-        input_dimensions=nuclei,
-        spectrometer_frequency=spectrometer_frequency,
-        molecule_type=molecule_type,
-    )
-
-    print(entry)
-
-
-def pipe(
-    entry,
-    frame_code_template,
-    file_names_and_lines,
-    chain_code,
-    sequence,
-    input_dimensions,
-    spectrometer_frequency,
-    molecule_type=MoleculeTypes.PROTEIN,
-):
+        if len(sequence) > 0 and (residue_name_key not in residue_name_lookup):
+            msg = f"""
+                the chain code {chain_code} and sequence_code {sequence_code} from
+                line {line_info.line_no} in file {line_info.file_name} were not found
+                in the input sequence, the full line was
 
-    sparky_frames = []
+                {line_info.line}
 
-    for file_name, lines in file_names_and_lines.items():
+                if you wish to input the peaks without validating against the input sequence use the
+                --no-validate option of sparky import peaks
+            """
+            exit_error(msg)
 
-        sparky_peaks = _parse_peaks(
-            lines,
-            file_name=file_name,
-            molecule_type=molecule_type,
+        residue = Residue(
             chain_code=chain_code,
-            sequence=sequence,
-        )
-
-        sparky_peaks = [translate_new_peak(peak) for peak in sparky_peaks]
-
-        dimensions = _guess_dimensions_if_not_defined_or_throw(
-            sparky_peaks, input_dimensions
-        )
-
-        dimensions = [{"axis_code": dimension} for dimension in dimensions]
-
-        file_name = Path(file_name).stem  # used in f method...
-
-        frame_code = f(frame_code_template)
-
-        frame = peaks_to_frame(
-            sparky_peaks, dimensions, spectrometer_frequency, frame_code=frame_code
+            sequence_code=sequence_code,
+            residue_name=translated_residue_name,
         )
+        assignment = AtomLabel(residue, atom_name)
 
-        sparky_frames.append(frame)
+        result.append(assignment)
 
-    return add_frames_to_entry(entry, sparky_frames)
-
-
-def parse_header_to_columns(header_line: str, file_name) -> Dict[str, int]:
-    headings_to_columns = {}
-    headings = header_line.split()
-
-    if "Data" in headings:
-        headings.remove("Data")
+        last_sequence_code = sequence_code
+        last_residue_name = residue_name
 
-    while ("(hz)") in headings:
-        headings.remove("(hz)")
-
-    for i, heading in enumerate(headings):
-        if heading in "Assignment Height Volume".split():
-            headings_to_columns[heading] = i
-            continue
-
-        if heading.startswith("w") or heading.startswith("lw"):
-            headings_to_columns[heading] = i
-            continue
-
-        # TODO add a warning function in the library
-        msg = f"""
-            WARNING: unexpected heading {heading} in the file {file_name}...
-                     this heading will be ignored, please send the heading and first
-                     few lines of this file to the developers of NEF-Pipelines if you
-                     believe this is a valid sparky peaks file
-        """
-
-        print(msg, file=sys.stderr)
-
-    assignment_column = headings_to_columns["Assignment"]
-    if assignment_column != 0:
-        msg = f"""
-            The file {file_name} doesn't look like a sparky file the Assignment column should be the first column
-            i got {assignment_column}
-            header was
-            {header_line}
-        """
-        exit(msg)
-
-    return headings_to_columns
-
-
-def _exit_error_if_shift_not_float(shifts, line_info):
-    for i, shift in enumerate(shifts, start=1):
-        if not is_float(shift):
-            msg = f"""
-                file {line_info.file_name} does not look like a sparky file
-                for shift w{i} at line {line_info.line_no} with the value {shift} couldn't be converted to a float
-                the full line was:
-                {line_info.line}
-            """
-            exit_error(msg)
+    return result
 
 
-def _parse_peaks(lines, file_name, molecule_type, chain_code, sequence):
+def parse_peaks(
+    lines, file_name, molecule_type, chain_code, sequence, allow_pseudo_atoms=False
+):
 
     peaks = []
 
     in_data = False
 
     dimension_count = None
 
@@ -292,15 +301,20 @@
                 else:
                     values[column] = UNUSED
 
             assignmnents_column = column_headers_to_indices["Assignment"]
             raw_assignment = fields[assignmnents_column]
 
             assignments = parse_assignments(
-                raw_assignment, chain_code, sequence, molecule_type, line_info
+                raw_assignment,
+                chain_code,
+                sequence,
+                molecule_type,
+                line_info,
+                allow_pseudo_atoms=allow_pseudo_atoms,
             )
 
             shifts = [
                 fields[column_headers_to_indices[f"w{index}"]]
                 for index in range(1, dimension_count + 1)
             ]
 
@@ -373,14 +387,68 @@
             )
 
             peaks.append(peak)
 
     return peaks
 
 
+def parse_header_to_columns(header_line: str, file_name) -> Dict[str, int]:
+    headings_to_columns = {}
+    headings = header_line.split()
+
+    if "Data" in headings:
+        headings.remove("Data")
+
+    while ("(hz)") in headings:
+        headings.remove("(hz)")
+
+    for i, heading in enumerate(headings):
+        if heading in "Assignment Height Volume".split():
+            headings_to_columns[heading] = i
+            continue
+
+        if heading.startswith("w") or heading.startswith("lw"):
+            headings_to_columns[heading] = i
+            continue
+
+        # TODO add a warning function in the library
+        msg = f"""
+            WARNING: unexpected heading {heading} in the file {file_name}...
+                     this heading will be ignored, please send the heading and first
+                     few lines of this file to the developers of NEF-Pipelines if you
+                     believe this is a valid sparky peaks file
+        """
+
+        print(msg, file=sys.stderr)
+
+    assignment_column = headings_to_columns["Assignment"]
+    if assignment_column != 0:
+        msg = f"""
+            The file {file_name} doesn't look like a sparky file the Assignment column should be the first column
+            i got {assignment_column}
+            header was
+            {header_line}
+        """
+        exit(msg)
+
+    return headings_to_columns
+
+
+def _exit_error_if_shift_not_float(shifts, line_info):
+    for i, shift in enumerate(shifts, start=1):
+        if not is_float(shift):
+            msg = f"""
+                file {line_info.file_name} does not look like a sparky file
+                for shift w{i} at line {line_info.line_no} with the value {shift} couldn't be converted to a float
+                the full line was:
+                {line_info.line}
+            """
+            exit_error(msg)
+
+
 def _exit_error_data_but_no_header(line_info):
     msg = f"""
                     the file {line_info.file_name} doesn't look like a sparky file at line {line_info.line_no}
                     there appears to be a data line but no header was detected a head should look like
                     Assignment w1 w2 ... etc
                     the current line data is
                     {line_info.line}
@@ -405,15 +473,15 @@
     if dimension_count < 1:
         msg = f"""
                     sparky peak file {line_info.file_name} doesn't appear to have enough columns [minimum 1]
                     at line {line_info.line_no}
                     the header was:
                     {line_info.line}
                 """
-        sys.exit(msg)
+        exit_error(msg)
 
 
 def _count_dimensions(column_headers_to_indices):
     dimension_count = 0
     for name in [f"w{i}" for i in range(1, 20)]:
         if name in column_headers_to_indices:
             dimension_count += 1
@@ -426,86 +494,7 @@
     msg = f"""
         bad sparky peak file {line_info.file_name} at line no {line_info.line_number} there appears to be a
         second header...
         the line was:
         {line_info.line}
                 """
     exit_error(msg)
-
-
-def _guess_dimensions_if_not_defined_or_throw(
-    peaks: List[NewPeak], input_dimensions: List[str]
-) -> List[str]:
-    results_by_dimension = {
-        i: dimension for i, dimension in enumerate(input_dimensions)
-    }
-
-    guessed_dimensions = {}
-
-    for peak_number, peak in enumerate(peaks, start=1):
-
-        for dimension_index, shift in enumerate(peak.shifts):
-            atom_name = shift.atom.atom_name
-
-            if len(atom_name) == 0:
-                atom_name = None
-
-            atom_type = None
-            if atom_name != UNUSED and atom_name is not None:
-                atom_type = atom_name.strip()[0]
-
-            if atom_type is not None and atom_type.lower() not in string.ascii_letters:
-                atom_type = None
-
-            guessed_dimension_isotopes = guessed_dimensions.setdefault(
-                dimension_index, set()
-            )
-            if atom_type and atom_type in ATOM_TO_ISOTOPE:
-                isotope_code = ATOM_TO_ISOTOPE[atom_type]
-                guessed_dimension_isotopes.add(isotope_code)
-            else:
-                guessed_dimension_isotopes.add(UNUSED)
-
-    for guessed_dimension_index in guessed_dimensions:
-        if guessed_dimension_index not in results_by_dimension:
-
-            guessed_dimension = guessed_dimensions[guessed_dimension_index]
-            if len(guessed_dimension) > 1 and UNUSED in guessed_dimension:
-                guessed_dimension.remove(UNUSED)
-
-            if len(guessed_dimensions[guessed_dimension_index]) > 1:
-
-                _raise_multiple_guessed_isotopes(
-                    guessed_dimensions, guessed_dimension_index
-                )
-
-    for dimension_index in guessed_dimensions:
-        if dimension_index not in results_by_dimension:
-            results_by_dimension[dimension_index] = list(
-                guessed_dimensions[dimension_index]
-            )[0]
-
-    max_dimension = max(results_by_dimension.keys())
-
-    result = []
-    for i in range(max_dimension + 1):
-        result.append(results_by_dimension[i])
-
-    return result
-
-
-def _raise_multiple_guessed_isotopes(guessed_dimensions, guessed_dimension_index):
-    dim_info = []
-    for dimension_index in sorted(guessed_dimensions).keys():
-        dim_data = f"{dimension_index}: {' '.join(guessed_dimensions.values())}"
-        dim_info.append(dim_data)
-    msg = f"""\
-                    no isotope provided for dimension {guessed_dimension_index + 1} and multiple possibilities
-                    found in atom names, please use explicit isotope codes using dimension-nuclei
-
-                    deduced codes for dimensions:
-
-
-                """
-    msg = dedent(msg)
-    msg += dim_info
-    raise IncompatibleDimensionTypesException(msg)
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,34 +59,34 @@
         STDIN,
         "-i",
         "--input",
         metavar="|PIPE|",
         help="input to read NEF data from [- is stdin]",
     ),
     file_names: List[Path] = typer.Argument(
-        ..., help="input files of type nmrview.out", metavar="<NMRVIEW-shifts>.out"
+        ..., help="input files of type shifts.txt", metavar="<SPARKY-shifts>.txt"
     ),
 ):
     """convert sparky shift file <sparky-shifts>.txt to NEF"""
 
     chain_codes = parse_comma_separated_options(chain_codes)
 
     if not chain_codes:
         chain_codes = ["A"]
 
-    _exit_if_chain_codes_and_file_name_dont_match(chain_codes, file_names)
+    _exit_if_chain_codes_and_file_names_dont_match(chain_codes, file_names)
 
     entry = read_entry_from_file_or_stdin_or_exit_error(input)
 
     sequence = sequence_from_entry_or_exit(entry)
 
     pipe(entry, chain_codes, sequence, frame_name, file_names)
 
 
-def _exit_if_chain_codes_and_file_name_dont_match(chain_codes, file_names):
+def _exit_if_chain_codes_and_file_names_dont_match(chain_codes, file_names):
     if len(chain_codes) != len(file_names):
         msg = f"""\
             the number of chains [{len(chain_codes)}] doesn't match the number of files [{len(file_names)}]
             chains were {chain_codes}
             files were {file_names}
         """
         exit_error(msg)
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/importers/peaks.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/importers/sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/importers/shifts.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.42/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.42/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef-pipelines
-Version: 0.1.41
+Version: 0.1.42
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.41/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.42/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,36 +61,45 @@
 src/nef_pipelines/tests/chains/test_clone.py
 src/nef_pipelines/tests/chains/test_list.py
 src/nef_pipelines/tests/chains/test_rename.py
 src/nef_pipelines/tests/chains/test_renumber.py
 src/nef_pipelines/tests/chains/test_data/3aa.nef
 src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
 src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+src/nef_pipelines/tests/csv/test_import_peaks.py
 src/nef_pipelines/tests/csv/test_import_rdcs.py
 src/nef_pipelines/tests/csv/test_data/short.csv
 src/nef_pipelines/tests/csv/test_data/short_complete.csv
+src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
 src/nef_pipelines/tests/echidna/__init__.py
 src/nef_pipelines/tests/echidna/test_import_peaks.py
 src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
 src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
 src/nef_pipelines/tests/fasta/test_sequence.py
 src/nef_pipelines/tests/fasta/test_data/3aa.fasta
 src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
 src/nef_pipelines/tests/frames/__init__.py
 src/nef_pipelines/tests/frames/test_delete.py
 src/nef_pipelines/tests/frames/test_list.py
 src/nef_pipelines/tests/frames/test_rename.py
 src/nef_pipelines/tests/frames/test_tabulate.py
+src/nef_pipelines/tests/frames/test_unassign.py
 src/nef_pipelines/tests/frames/test_data/frames.nef
 src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
 src/nef_pipelines/tests/mars/__init__.py
 src/nef_pipelines/tests/mars/test_export_shifts.py
+src/nef_pipelines/tests/mars/test_import_peaks.py
 src/nef_pipelines/tests/mars/test_import_shifts.py
 src/nef_pipelines/tests/mars/test_data/sec5_short.neff
 src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
+src/nef_pipelines/tests/mars/test_data/sparky_CA.out
+src/nef_pipelines/tests/mars/test_data/sparky_all.out
+src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
 src/nef_pipelines/tests/nmrpipe/__init__.py
 src/nef_pipelines/tests/nmrpipe/test_gdb.py
 src/nef_pipelines/tests/nmrpipe/test_peaks.py
 src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
 src/nef_pipelines/tests/nmrpipe/test_sequence.py
 src/nef_pipelines/tests/nmrpipe/test_shifts.py
 src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
@@ -219,20 +228,22 @@
 src/nef_pipelines/tools/entry/rename.py
 src/nef_pipelines/tools/frames/__init__.py
 src/nef_pipelines/tools/frames/delete.py
 src/nef_pipelines/tools/frames/insert.py
 src/nef_pipelines/tools/frames/list.py
 src/nef_pipelines/tools/frames/rename.py
 src/nef_pipelines/tools/frames/tabulate.py
+src/nef_pipelines/tools/frames/unassign.py
 src/nef_pipelines/tools/peaks/match.py
 src/nef_pipelines/tools/shifts/__init__.py
 src/nef_pipelines/tools/shifts/make_peaks.py
 src/nef_pipelines/transcoders/__init__.py
 src/nef_pipelines/transcoders/csv/__init__.py
 src/nef_pipelines/transcoders/csv/importers/__init__.py
+src/nef_pipelines/transcoders/csv/importers/peaks.py
 src/nef_pipelines/transcoders/csv/importers/rdcs.py
 src/nef_pipelines/transcoders/echidna/__init__.py
 src/nef_pipelines/transcoders/echidna/importers/__init__.py
 src/nef_pipelines/transcoders/echidna/importers/peaks.py
 src/nef_pipelines/transcoders/fasta/__init__.py
 src/nef_pipelines/transcoders/fasta/exporters/__init__.py
 src/nef_pipelines/transcoders/fasta/exporters/sequence.py
@@ -241,14 +252,15 @@
 src/nef_pipelines/transcoders/mars/__init__.py
 src/nef_pipelines/transcoders/mars/exporters/__init__.py
 src/nef_pipelines/transcoders/mars/exporters/fragments.py
 src/nef_pipelines/transcoders/mars/exporters/input.py
 src/nef_pipelines/transcoders/mars/exporters/sequence.py
 src/nef_pipelines/transcoders/mars/exporters/shifts.py
 src/nef_pipelines/transcoders/mars/importers/__init__.py
+src/nef_pipelines/transcoders/mars/importers/peaks.py
 src/nef_pipelines/transcoders/mars/importers/shifts.py
 src/nef_pipelines/transcoders/nmrpipe/__init__.py
 src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
 src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
 src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
 src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
 src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
```

### Comparing `nef_pipelines-0.1.41/tox.ini` & `nef_pipelines-0.1.42/tox.ini`

 * *Files identical despite different names*

