# Comparing `tmp/most_queue-1.21.tar.gz` & `tmp/most_queue-1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "most_queue-1.21.tar", last modified: Sat Jun  3 07:33:16 2023, max compression
+gzip compressed data, was "most_queue-1.22.tar", last modified: Sat Jun  3 22:17:33 2023, max compression
```

## Comparing `most_queue-1.21.tar` & `most_queue-1.22.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.269953 most_queue-1.21/
--rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most_queue-1.21/LICENSE
--rw-rw-rw-   0        0        0     6337 2023-06-03 07:33:16.268981 most_queue-1.21/PKG-INFO
--rw-rw-rw-   0        0        0     4545 2023-05-17 17:25:06.000000 most_queue-1.21/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.198447 most_queue-1.21/most_queue/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.21/most_queue/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.215939 most_queue-1.21/most_queue/sim/
--rw-rw-rw-   0        0        0       78 2023-05-17 17:58:01.000000 most_queue-1.21/most_queue/sim/__init__.py
--rw-rw-rw-   0        0        0     3853 2023-06-03 06:16:25.000000 most_queue-1.21/most_queue/sim/batch_sim.py
--rw-rw-rw-   0        0        0    13909 2023-06-03 06:25:11.000000 most_queue-1.21/most_queue/sim/fj_delta_sim.py
--rw-rw-rw-   0        0        0    11136 2023-06-03 06:21:42.000000 most_queue-1.21/most_queue/sim/fj_sim.py
--rw-rw-rw-   0        0        0    10039 2023-06-03 06:30:19.000000 most_queue-1.21/most_queue/sim/flow_sum_sim.py
--rw-rw-rw-   0        0        0     7702 2023-06-03 06:35:08.000000 most_queue-1.21/most_queue/sim/impatient_queue_sim.py
--rw-rw-rw-   0        0        0     9329 2023-06-03 06:35:08.000000 most_queue-1.21/most_queue/sim/priority_network.py
--rw-rw-rw-   0        0        0    38069 2023-06-03 06:30:19.000000 most_queue-1.21/most_queue/sim/priority_queue_sim.py
--rw-rw-rw-   0        0        0    31166 2023-06-03 06:16:25.000000 most_queue-1.21/most_queue/sim/qs_sim.py
--rw-rw-rw-   0        0        0    12393 2023-06-03 06:35:08.000000 most_queue-1.21/most_queue/sim/queue_finite_source_sim.py
--rw-rw-rw-   0        0        0    37275 2023-05-17 17:54:25.000000 most_queue-1.21/most_queue/sim/rand_destribution.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.241586 most_queue-1.21/most_queue/tests/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.21/most_queue/tests/__init__.py
--rw-rw-rw-   0        0        0     3571 2023-06-03 07:00:47.000000 most_queue-1.21/most_queue/tests/ek_d_n.py
--rw-rw-rw-   0        0        0     5109 2023-06-03 07:00:47.000000 most_queue-1.21/most_queue/tests/fj_calc.py
--rw-rw-rw-   0        0        0     5554 2023-06-03 07:02:09.000000 most_queue-1.21/most_queue/tests/fj_im.py
--rw-rw-rw-   0        0        0     4292 2023-06-03 07:03:43.000000 most_queue-1.21/most_queue/tests/flow_sum.py
--rw-rw-rw-   0        0        0     5166 2023-06-03 07:07:00.000000 most_queue-1.21/most_queue/tests/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     5302 2023-06-03 07:08:42.000000 most_queue-1.21/most_queue/tests/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2287 2023-06-03 07:09:19.000000 most_queue-1.21/most_queue/tests/m_d_n_calc.py
--rw-rw-rw-   0        0        0     3148 2023-06-03 07:12:12.000000 most_queue-1.21/most_queue/tests/m_h2_h2warm.py
--rw-rw-rw-   0        0        0     6737 2023-06-03 07:16:26.000000 most_queue-1.21/most_queue/tests/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     2779 2023-06-03 07:16:26.000000 most_queue-1.21/most_queue/tests/mg1_calc.py
--rw-rw-rw-   0        0        0      792 2023-06-03 07:17:42.000000 most_queue-1.21/most_queue/tests/mg1_warm_calc.py
--rw-rw-rw-   0        0        0     4248 2023-06-03 07:19:07.000000 most_queue-1.21/most_queue/tests/mgn_tt.py
--rw-rw-rw-   0        0        0     3358 2023-06-03 07:23:03.000000 most_queue-1.21/most_queue/tests/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0     2860 2023-06-03 07:23:03.000000 most_queue-1.21/most_queue/tests/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     6535 2023-06-03 07:23:03.000000 most_queue-1.21/most_queue/tests/network_im_prty.py
--rw-rw-rw-   0        0        0     2207 2023-06-03 07:25:02.000000 most_queue-1.21/most_queue/tests/smo_im.py
--rw-rw-rw-   0        0        0     4974 2023-06-03 07:31:47.000000 most_queue-1.21/most_queue/tests/smo_im_prty.py
--rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most_queue-1.21/most_queue/tests/weibull.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.262405 most_queue-1.21/most_queue/theory/
--rw-rw-rw-   0        0        0       76 2023-05-17 17:43:06.000000 most_queue-1.21/most_queue/theory/__init__.py
--rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most_queue-1.21/most_queue/theory/batch_mm1.py
--rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most_queue-1.21/most_queue/theory/convolution_sum_calc.py
--rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most_queue-1.21/most_queue/theory/diff5dots.py
--rw-rw-rw-   0        0        0     6030 2023-06-03 06:39:46.000000 most_queue-1.21/most_queue/theory/ek_d_n_calc.py
--rw-rw-rw-   0        0        0     4741 2023-06-02 19:50:03.000000 most_queue-1.21/most_queue/theory/engset_model.py
--rw-rw-rw-   0        0        0    19297 2023-06-03 06:39:46.000000 most_queue-1.21/most_queue/theory/fj_calc.py
--rw-rw-rw-   0        0        0    10652 2023-06-03 06:43:21.000000 most_queue-1.21/most_queue/theory/flow_sum.py
--rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most_queue-1.21/most_queue/theory/generate_pareto_noise.py
--rw-rw-rw-   0        0        0     4285 2023-06-03 07:04:51.000000 most_queue-1.21/most_queue/theory/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     6205 2023-06-03 06:46:05.000000 most_queue-1.21/most_queue/theory/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most_queue-1.21/most_queue/theory/impatience_calc.py
--rw-rw-rw-   0        0        0     4228 2023-06-03 06:46:46.000000 most_queue-1.21/most_queue/theory/m_d_n_calc.py
--rw-rw-rw-   0        0        0    27856 2023-06-03 06:48:34.000000 most_queue-1.21/most_queue/theory/m_h2_h2warm.py
--rw-rw-rw-   0        0        0    29755 2023-06-03 06:50:55.000000 most_queue-1.21/most_queue/theory/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     4708 2023-06-03 06:52:44.000000 most_queue-1.21/most_queue/theory/mg1_calc.py
--rw-rw-rw-   0        0        0     1383 2023-06-03 06:52:44.000000 most_queue-1.21/most_queue/theory/mg1_warm_calc.py
--rw-rw-rw-   0        0        0    17386 2023-06-03 06:53:31.000000 most_queue-1.21/most_queue/theory/mgn_tt.py
--rw-rw-rw-   0        0        0    18846 2023-06-03 06:54:14.000000 most_queue-1.21/most_queue/theory/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0    26736 2023-06-03 06:54:45.000000 most_queue-1.21/most_queue/theory/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     1994 2023-06-03 07:29:46.000000 most_queue-1.21/most_queue/theory/mmnr_calc.py
--rw-rw-rw-   0        0        0     5777 2023-05-17 17:54:25.000000 most_queue-1.21/most_queue/theory/network_calc.py
--rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most_queue-1.21/most_queue/theory/network_viewer.py
--rw-rw-rw-   0        0        0    40877 2023-05-18 21:35:04.000000 most_queue-1.21/most_queue/theory/passage_time.py
--rw-rw-rw-   0        0        0    17662 2023-05-17 17:54:25.000000 most_queue-1.21/most_queue/theory/priority_calc.py
--rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most_queue-1.21/most_queue/theory/q_poisson_arrival_calc.py
--rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most_queue-1.21/most_queue/theory/student_stat.py
--rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most_queue-1.21/most_queue/theory/weibull.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.265409 most_queue-1.21/most_queue/utils/
--rw-rw-rw-   0        0        0        0 2023-05-17 17:19:33.000000 most_queue-1.21/most_queue/utils/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-05-17 17:18:48.000000 most_queue-1.21/most_queue/utils/approx_cdf_make.py
--rw-rw-rw-   0        0        0      319 2023-05-18 16:11:27.000000 most_queue-1.21/most_queue/utils/binom_probs.py
--rw-rw-rw-   0        0        0     2761 2023-06-02 20:11:23.000000 most_queue-1.21/most_queue/utils/tables.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.265946 most_queue-1.21/most_queue/visualisation/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.21/most_queue/visualisation/__init__.py
--rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most_queue-1.21/most_queue/visualisation/smo_im_vis.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.268981 most_queue-1.21/most_queue/visualisation/utils/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.21/most_queue/visualisation/utils/__init__.py
--rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most_queue-1.21/most_queue/visualisation/utils/result_table.py
--rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most_queue-1.21/most_queue/visualisation/utils/settings_window.py
--rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most_queue-1.21/most_queue/visualisation/utils/splash_screen.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.205174 most_queue-1.21/most_queue.egg-info/
--rw-rw-rw-   0        0        0     6337 2023-06-03 07:33:16.000000 most_queue-1.21/most_queue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2556 2023-06-03 07:33:16.000000 most_queue-1.21/most_queue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 07:33:16.000000 most_queue-1.21/most_queue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most_queue-1.21/most_queue.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      114 2023-06-03 07:33:16.000000 most_queue-1.21/most_queue.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-03 07:33:16.000000 most_queue-1.21/most_queue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      508 2023-06-03 07:33:06.000000 most_queue-1.21/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-03 07:33:16.269953 most_queue-1.21/setup.cfg
--rw-rw-rw-   0        0        0     1000 2023-06-03 07:32:58.000000 most_queue-1.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:17:33.086727 most_queue-1.22/
+-rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most_queue-1.22/LICENSE
+-rw-rw-rw-   0        0        0     6337 2023-06-03 22:17:33.085802 most_queue-1.22/PKG-INFO
+-rw-rw-rw-   0        0        0     4545 2023-05-17 17:25:06.000000 most_queue-1.22/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 22:17:32.915980 most_queue-1.22/most_queue/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.22/most_queue/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:17:32.944079 most_queue-1.22/most_queue/sim/
+-rw-rw-rw-   0        0        0       78 2023-05-17 17:58:01.000000 most_queue-1.22/most_queue/sim/__init__.py
+-rw-rw-rw-   0        0        0     3853 2023-06-03 06:16:25.000000 most_queue-1.22/most_queue/sim/batch_sim.py
+-rw-rw-rw-   0        0        0    13936 2023-06-03 22:04:28.000000 most_queue-1.22/most_queue/sim/fj_delta_sim.py
+-rw-rw-rw-   0        0        0    11136 2023-06-03 06:21:42.000000 most_queue-1.22/most_queue/sim/fj_sim.py
+-rw-rw-rw-   0        0        0    10039 2023-06-03 06:30:19.000000 most_queue-1.22/most_queue/sim/flow_sum_sim.py
+-rw-rw-rw-   0        0        0     7702 2023-06-03 06:35:08.000000 most_queue-1.22/most_queue/sim/impatient_queue_sim.py
+-rw-rw-rw-   0        0        0     9370 2023-06-03 22:04:28.000000 most_queue-1.22/most_queue/sim/priority_network.py
+-rw-rw-rw-   0        0        0    38130 2023-06-03 22:08:10.000000 most_queue-1.22/most_queue/sim/priority_queue_sim.py
+-rw-rw-rw-   0        0        0    31127 2023-06-03 22:09:07.000000 most_queue-1.22/most_queue/sim/qs_sim.py
+-rw-rw-rw-   0        0        0    12393 2023-06-03 06:35:08.000000 most_queue-1.22/most_queue/sim/queue_finite_source_sim.py
+-rw-rw-rw-   0        0        0    37275 2023-05-17 17:54:25.000000 most_queue-1.22/most_queue/sim/rand_destribution.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:17:33.015687 most_queue-1.22/most_queue/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.22/most_queue/tests/__init__.py
+-rw-rw-rw-   0        0        0     3571 2023-06-03 07:00:47.000000 most_queue-1.22/most_queue/tests/ek_d_n.py
+-rw-rw-rw-   0        0        0     5109 2023-06-03 07:00:47.000000 most_queue-1.22/most_queue/tests/fj_calc.py
+-rw-rw-rw-   0        0        0     5554 2023-06-03 07:02:09.000000 most_queue-1.22/most_queue/tests/fj_im.py
+-rw-rw-rw-   0        0        0     4292 2023-06-03 07:03:43.000000 most_queue-1.22/most_queue/tests/flow_sum.py
+-rw-rw-rw-   0        0        0     5166 2023-06-03 07:07:00.000000 most_queue-1.22/most_queue/tests/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     5302 2023-06-03 07:08:42.000000 most_queue-1.22/most_queue/tests/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2287 2023-06-03 07:09:19.000000 most_queue-1.22/most_queue/tests/m_d_n_calc.py
+-rw-rw-rw-   0        0        0     3148 2023-06-03 07:12:12.000000 most_queue-1.22/most_queue/tests/m_h2_h2warm.py
+-rw-rw-rw-   0        0        0     6745 2023-06-03 22:16:35.000000 most_queue-1.22/most_queue/tests/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     2779 2023-06-03 07:16:26.000000 most_queue-1.22/most_queue/tests/mg1_calc.py
+-rw-rw-rw-   0        0        0      792 2023-06-03 07:17:42.000000 most_queue-1.22/most_queue/tests/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0     4248 2023-06-03 07:19:07.000000 most_queue-1.22/most_queue/tests/mgn_tt.py
+-rw-rw-rw-   0        0        0     3358 2023-06-03 07:23:03.000000 most_queue-1.22/most_queue/tests/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0     2860 2023-06-03 07:23:03.000000 most_queue-1.22/most_queue/tests/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     6535 2023-06-03 07:23:03.000000 most_queue-1.22/most_queue/tests/network_im_prty.py
+-rw-rw-rw-   0        0        0     2207 2023-06-03 07:25:02.000000 most_queue-1.22/most_queue/tests/smo_im.py
+-rw-rw-rw-   0        0        0     4986 2023-06-03 22:16:35.000000 most_queue-1.22/most_queue/tests/smo_im_prty.py
+-rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most_queue-1.22/most_queue/tests/weibull.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:17:33.067621 most_queue-1.22/most_queue/theory/
+-rw-rw-rw-   0        0        0       76 2023-05-17 17:43:06.000000 most_queue-1.22/most_queue/theory/__init__.py
+-rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most_queue-1.22/most_queue/theory/batch_mm1.py
+-rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most_queue-1.22/most_queue/theory/convolution_sum_calc.py
+-rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most_queue-1.22/most_queue/theory/diff5dots.py
+-rw-rw-rw-   0        0        0     6030 2023-06-03 06:39:46.000000 most_queue-1.22/most_queue/theory/ek_d_n_calc.py
+-rw-rw-rw-   0        0        0     4782 2023-06-03 22:10:41.000000 most_queue-1.22/most_queue/theory/engset_model.py
+-rw-rw-rw-   0        0        0    19298 2023-06-03 22:13:16.000000 most_queue-1.22/most_queue/theory/fj_calc.py
+-rw-rw-rw-   0        0        0    10652 2023-06-03 06:43:21.000000 most_queue-1.22/most_queue/theory/flow_sum.py
+-rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most_queue-1.22/most_queue/theory/generate_pareto_noise.py
+-rw-rw-rw-   0        0        0     4285 2023-06-03 07:04:51.000000 most_queue-1.22/most_queue/theory/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     6205 2023-06-03 06:46:05.000000 most_queue-1.22/most_queue/theory/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most_queue-1.22/most_queue/theory/impatience_calc.py
+-rw-rw-rw-   0        0        0     4228 2023-06-03 06:46:46.000000 most_queue-1.22/most_queue/theory/m_d_n_calc.py
+-rw-rw-rw-   0        0        0    27856 2023-06-03 06:48:34.000000 most_queue-1.22/most_queue/theory/m_h2_h2warm.py
+-rw-rw-rw-   0        0        0    29755 2023-06-03 06:50:55.000000 most_queue-1.22/most_queue/theory/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     4708 2023-06-03 06:52:44.000000 most_queue-1.22/most_queue/theory/mg1_calc.py
+-rw-rw-rw-   0        0        0     1383 2023-06-03 06:52:44.000000 most_queue-1.22/most_queue/theory/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0    17386 2023-06-03 06:53:31.000000 most_queue-1.22/most_queue/theory/mgn_tt.py
+-rw-rw-rw-   0        0        0    18846 2023-06-03 06:54:14.000000 most_queue-1.22/most_queue/theory/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0    26736 2023-06-03 06:54:45.000000 most_queue-1.22/most_queue/theory/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     1994 2023-06-03 07:29:46.000000 most_queue-1.22/most_queue/theory/mmnr_calc.py
+-rw-rw-rw-   0        0        0     5808 2023-06-03 22:06:37.000000 most_queue-1.22/most_queue/theory/network_calc.py
+-rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most_queue-1.22/most_queue/theory/network_viewer.py
+-rw-rw-rw-   0        0        0    40877 2023-05-18 21:35:04.000000 most_queue-1.22/most_queue/theory/passage_time.py
+-rw-rw-rw-   0        0        0    17662 2023-05-17 17:54:25.000000 most_queue-1.22/most_queue/theory/priority_calc.py
+-rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most_queue-1.22/most_queue/theory/q_poisson_arrival_calc.py
+-rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most_queue-1.22/most_queue/theory/student_stat.py
+-rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most_queue-1.22/most_queue/theory/weibull.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:17:33.075133 most_queue-1.22/most_queue/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-17 17:19:33.000000 most_queue-1.22/most_queue/utils/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-05-17 17:18:48.000000 most_queue-1.22/most_queue/utils/approx_cdf_make.py
+-rw-rw-rw-   0        0        0      319 2023-05-18 16:11:27.000000 most_queue-1.22/most_queue/utils/binom_probs.py
+-rw-rw-rw-   0        0        0     2761 2023-06-02 20:11:23.000000 most_queue-1.22/most_queue/utils/tables.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:17:33.078244 most_queue-1.22/most_queue/visualisation/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.22/most_queue/visualisation/__init__.py
+-rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most_queue-1.22/most_queue/visualisation/smo_im_vis.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:17:33.084683 most_queue-1.22/most_queue/visualisation/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.22/most_queue/visualisation/utils/__init__.py
+-rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most_queue-1.22/most_queue/visualisation/utils/result_table.py
+-rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most_queue-1.22/most_queue/visualisation/utils/settings_window.py
+-rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most_queue-1.22/most_queue/visualisation/utils/splash_screen.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:17:32.925388 most_queue-1.22/most_queue.egg-info/
+-rw-rw-rw-   0        0        0     6337 2023-06-03 22:17:32.000000 most_queue-1.22/most_queue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2556 2023-06-03 22:17:32.000000 most_queue-1.22/most_queue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 22:17:32.000000 most_queue-1.22/most_queue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most_queue-1.22/most_queue.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      114 2023-06-03 22:17:32.000000 most_queue-1.22/most_queue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 22:17:32.000000 most_queue-1.22/most_queue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      508 2023-06-03 22:17:10.000000 most_queue-1.22/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 22:17:33.086727 most_queue-1.22/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2023-06-03 22:16:59.000000 most_queue-1.22/setup.py
```

### Comparing `most_queue-1.21/LICENSE` & `most_queue-1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/PKG-INFO` & `most_queue-1.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: most_queue
-Version: 1.21
+Version: 1.22
 Summary: Software package for calculation and simulation of queuing systems
 Home-page: https://github.com/xabarov/mps
 Author: Xabarov Roman
 Author-email: Xabarov Roman <xabarov1985@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `most_queue-1.21/README.md` & `most_queue-1.22/README.md`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/sim/batch_sim.py` & `most_queue-1.22/most_queue/sim/batch_sim.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/sim/fj_delta_sim.py` & `most_queue-1.22/most_queue/sim/fj_delta_sim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from fj_sim import ForkJoinSim
 from fj_sim import SubTask as SubTask
 from fj_sim import Task as Task
 from qs_sim import Server
-from most_queue.theory import sv_sum_calc
+from most_queue.theory import convolution_sum_calc
 
 import rand_destribution as rd
 
 
 class ServerWarmUp(Server):
     """
     Канал обслуживания
@@ -36,15 +36,15 @@
                 elif self.dist.type == 'C':
                     b = rd.Cox_dist.calc_theory_moments(*self.dist.params)
                 elif self.dist.type == 'Pa':
                     b = rd.Pareto_dist.calc_theory_moments(*self.dist.params)
                 elif self.dist.type == 'Gamma':
                     b = rd.Gamma.calc_theory_moments(*self.dist.params)
 
-                f_summ = sv_sum_calc.get_moments(b, self.delta)
+                f_summ = convolution_sum_calc.get_moments(b, self.delta)
                 # variance = f_summ[1] - math.pow(f_summ[0], 2)
                 # coev = math.sqrt(variance)/f_summ[0]
                 params = rd.Gamma.get_mu_alpha(f_summ)
                 self.time_to_end_service = ttek + rd.Gamma.generate_static(*params)
 
 
 class SubTaskDelta(SubTask):
@@ -123,15 +123,15 @@
                     self.free_channels -= 1
                     self.serv_task_id = t.id
 
             for i in range(1, self.k):
                 if not isinstance(self.delta, list):
                     t.subtasks[i].future_arr_time = self.ttek + i * self.delta
                 else:
-                    b_delta = sv_sum_calc.get_self_concolution(self.delta, i)
+                    b_delta = convolution_sum_calc.get_self_concolution(self.delta, i)
                     params_delta = rd.Gamma.get_mu_alpha(b_delta)
                     t.subtasks[i].future_arr_time = self.ttek + rd.Gamma.generate_static(*params_delta)
                 self.subtask_arr_queue.append(t.subtasks[i])
 
     def subtask_arrival(self, subtask_num):
 
         subtsk = self.subtask_arr_queue.pop(subtask_num)
```

### Comparing `most_queue-1.21/most_queue/sim/fj_sim.py` & `most_queue-1.22/most_queue/sim/fj_sim.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/sim/flow_sum_sim.py` & `most_queue-1.22/most_queue/sim/flow_sum_sim.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/sim/impatient_queue_sim.py` & `most_queue-1.22/most_queue/sim/impatient_queue_sim.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/sim/priority_network.py` & `most_queue-1.22/most_queue/sim/priority_network.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import sys
 
 from colorama import init
 from colorama import Fore, Style
 
 init()
 
+
 class PriorityNetwork:
     """
     Имитационная модель СеМО с многоканальными узлами и приоритетами
     """
 
     def __init__(self, k_num, L, R, n, prty, serv_params, nodes_prty):
 
@@ -41,22 +42,22 @@
                 param_serv_reset.append(serv_params[m][nodes_prty[m][k]])
 
             self.smos[m].set_servers(param_serv_reset)
             time.sleep(0.1)
 
         self.arrival_time = []
         self.sources = []
-        self.v_semo = []
-        self.w_semo = []
+        self.v_network = []
+        self.w_network = []
         for k in range(k_num):
             self.sources.append(rd.Exp_dist(L[k]))
             self.arrival_time.append(self.sources[k].generate())
             time.sleep(0.1)
-            self.v_semo.append([0.0] * 3)
-            self.w_semo.append([0.0] * 3)
+            self.v_network.append([0.0] * 3)
+            self.w_network.append([0.0] * 3)
 
         self.ttek = 0
         self.total = 0
         self.served = [0] * self.k_num
         self.in_sys = [0] * self.k_num
         self.t_old = [0] * self.k_num
         self.arrived = [0] * self.k_num
@@ -68,21 +69,21 @@
             sum_p += self.R[real_class][current_node + 1, i]
             if sum_p > p:
                 return i
         return 0
 
     def refresh_v_stat(self, k, new_a):
         for i in range(3):
-            self.v_semo[k][i] = self.v_semo[k][i] * (1.0 - (1.0 / self.served[k])) + math.pow(new_a, i + 1) / \
-                                self.served[k]
+            self.v_network[k][i] = self.v_network[k][i] * (1.0 - (1.0 / self.served[k])) + math.pow(new_a, i + 1) / \
+                                   self.served[k]
 
     def refresh_w_stat(self, k, new_a):
         for i in range(3):
-            self.w_semo[k][i] = self.w_semo[k][i] * (1.0 - (1.0 / self.served[k])) + math.pow(new_a, i + 1) / \
-                                self.served[k]
+            self.w_network[k][i] = self.w_network[k][i] * (1.0 - (1.0 / self.served[k])) + math.pow(new_a, i + 1) / \
+                                   self.served[k]
 
     def run_one_step(self):
         num_of_serv_ch_earlier = -1  # номер канала узла, мин время до окончания обслуживания
         num_of_k_earlier = -1  # номер класса, прибывающего через мин время
         num_of_node_earlier = -1  # номер узла, в котором раньше всех закончится обслуживание
         arrival_earlier = 1e10  # момент прибытия ближайшего
         serving_earlier = 1e10  # момент ближайшего обслуживания
@@ -124,16 +125,16 @@
             real_class = ts.k
             next_node = self.play_next_node(real_class, num_of_node_earlier)
 
             if next_node == self.n_num:
                 self.served[real_class] += 1
                 self.in_sys[real_class] -= 1
 
-                self.refresh_v_stat(real_class, self.ttek - ts.arr_semo)
-                self.refresh_w_stat(real_class, ts.wait_semo)
+                self.refresh_v_stat(real_class, self.ttek - ts.arr_network)
+                self.refresh_w_stat(real_class, ts.wait_network)
 
             else:
                 next_node_class = self.nodes_prty[next_node][real_class]
 
                 self.smos[next_node].arrival(next_node_class, self.ttek, ts)
 
     def run(self, job_served, is_real_served=False):
@@ -150,15 +151,14 @@
             for i in tqdm(range(job_served)):
                 self.run_one_step()
 
             print(Fore.GREEN + '\rSimulation is finished')
             print(Style.RESET_ALL)
 
 
-
 if __name__ == '__main__':
 
     from most_queue.utils.tables import times_print_with_classes
 
     k_num = 3
     n_num = 5
     n = [3, 2, 3, 4, 3]
@@ -200,19 +200,19 @@
             b[k].append(rd.H2_dist.calc_theory_moments(*h2_params[m], 4))
 
     prty = ['NP'] * n_num
     qn = PriorityNetwork(k_num, L, R, n, prty, serv_params, nodes_prty)
 
     qn.run(jobs_num)
 
-    v_im = qn.v_semo
+    v_sim = qn.v_network
 
-    semo_calc = network_calc.network_prty_calc(R, b, n, L, prty, nodes_prty)
-    v_ch = semo_calc['v']
-    loads = semo_calc['loads']
+    calc_res = network_calc.network_prty_calc(R, b, n, L, prty, nodes_prty)
+    v_ch = calc_res['v']
+    loads = calc_res['loads']
 
     print("\n")
     print("-" * 60)
     print("{0:^60s}\n{1:^60s}".format("Сравнение данных ИМ и результатов расчета времени пребывания",
                                       "в СеМО с многоканальными узлами и приоритетами"))
     print("-" * 60)
     print("Количество каналов в узлах:")
@@ -222,24 +222,24 @@
     for load in loads:
         print("{0:^1.3f}".format(load), end=" ")
     print("\n")
     print("-" * 60)
     print("{0:^60s}".format("Относительный приоритет"))
 
     print("-" * 60)
-    times_print_with_classes(v_im, v_ch, is_w=False)
+    times_print_with_classes(v_sim, v_ch, is_w=False)
 
     prty = ['PR'] * n_num
     qn = PriorityNetwork(k_num, L, R, n, prty, serv_params, nodes_prty)
 
     qn.run(jobs_num)
 
-    v_im = qn.v_semo
+    v_sim = qn.v_network
 
-    semo_calc = network_calc.network_prty_calc(R, b, n, L, prty, nodes_prty)
-    v_ch = semo_calc['v']
+    calc_res = network_calc.network_prty_calc(R, b, n, L, prty, nodes_prty)
+    v_ch = calc_res['v']
 
     print("-" * 60)
     print("{0:^60s}".format("Абсолютный приоритет"))
     print("-" * 60)
 
-    times_print_with_classes(v_im, v_ch, is_w=False)
+    times_print_with_classes(v_sim, v_ch, is_w=False)
```

### Comparing `most_queue-1.21/most_queue/sim/priority_queue_sim.py` & `most_queue-1.22/most_queue/sim/priority_queue_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         num_of_channels - количество каналов СМО
         num_of_classes - количество классов заявок
         prty_type - тип приоритета:
             No  - без приоритетов, FIFO
             PR  -  preemptive resume, с дообслуживанием прерванной заявки
             RS  -  preemptive repeat with resampling, обслуживание заново с новой случайной длительностью
             RW  - preemptive repeat without resampling, обслуживание заново с прежней длительностью
-            NP  - non preemptive, относиттельный приоритет
+            NP  - non preemptive, относительный приоритет
         buffer - максимальная длина очереди
 
         Для запуска ИМ необходимо:
         - вызвать конструктор с параметрами
         - задать вх поток с помощью метода set_sorces() экземпляра созданного класса PriorityQueueSimulator
         - задать распределение обслуживания с помощью метода set_servers() экземпляра класса PriorityQueueSimulator
         - запустить ИМ с помощью метода run() экземпляра созданного класса PriorityQueueSimulator,
@@ -316,15 +316,15 @@
         """
         if moment:
             self.ttek = moment
             self.p[k][self.in_sys[k]] += moment - self.t_old[k]
             new_tsk = ts
             new_tsk.in_node_class_num = k
             new_tsk.arr_time = moment
-            new_tsk.wait_time = 0  # в текущем узле обнуляем время ожидания. Общее время ожидания - ts.wait_semo
+            new_tsk.wait_time = 0  # в текущем узле обнуляем время ожидания. Общее время ожидания - ts.wait_network
             new_tsk.is_pr = False
             new_tsk.start_waiting_time = -1
             new_tsk.time_to_end_service = 0
 
         else:
             self.ttek = self.arrival_time[k]
             self.p[k][self.in_sys[k]] += self.arrival_time[k] - self.t_old[k]
@@ -385,15 +385,15 @@
                                 dropped_tsk.time_to_end_service = c.dist[k].generate()
                             elif self.prty_type == "RW":
                                 dropped_tsk.time_to_end_service = total_time
 
                             is_found_weekier = True
                             if moment:
                                 self.queue[dropped_tsk.in_node_class_num].append(dropped_tsk)
-                                c.start_service(new_tsk, self.ttek, is_semo=True)
+                                c.start_service(new_tsk, self.ttek, is_network=True)
                             else:
                                 self.queue[dropped_tsk.k].append(dropped_tsk)
                                 c.start_service(new_tsk, self.ttek)
 
                             break
                     if not is_found_weekier:
                         if not self.buffer:  # не задана длина очередиб т.е бесконечная очередь
@@ -416,43 +416,43 @@
                     new_tsk.start_waiting_time = self.ttek
                     self.queue[k].append(new_tsk)
 
         else:  # there are free channels:
             if self.free_channels == self.n and self.is_warm_up_set == True:
                 self.taked[k] += 1
                 if moment:
-                    self.servers[0].start_service(new_tsk, self.ttek, self.warm_up[k], is_semo=True)
+                    self.servers[0].start_service(new_tsk, self.ttek, self.warm_up[k], is_network=True)
                 else:
                     self.servers[0].start_service(new_tsk, self.ttek, self.warm_up[k])
                 self.free_channels -= 1
             else:
                 for s in self.servers:
                     if s.is_free:
                         self.taked[k] += 1
                         if moment:
-                            s.start_service(new_tsk, self.ttek, is_semo=True)
+                            s.start_service(new_tsk, self.ttek, is_network=True)
                         else:
                             s.start_service(new_tsk, self.ttek)
                         self.free_channels -= 1
                         break
             # Проверям, не наступил ли ПНЗ:
             if self.free_channels == 0:
                 if self.in_sys[k] == self.n:
                     self.start_ppnz = self.ttek
                     self.class_ppnz_started = k
 
-    def serving(self, c, is_semo=False):
+    def serving(self, c, is_network=False):
         """
         Дейтсвия по поступлению заявки на обслуживание
         с - номер канала
-        is_semo - является ли СМО частью СеМО
+        is_network - является ли СМО частью СеМО
         """
         time_to_end = self.servers[c].time_to_end_service
         end_ts = self.servers[c].end_service()
-        if is_semo:
+        if is_network:
             k = end_ts.in_node_class_num
         else:
             k = end_ts.k
 
         self.p[k][self.in_sys[k]] += time_to_end - self.t_old[k]
 
         self.ttek = time_to_end
@@ -484,17 +484,17 @@
 
                     if self.free_channels == 1 and kk != end_ts.k:
                         self.start_ppnz = self.ttek
                         self.class_ppnz_started = kk
 
                     self.taked[kk] += 1
                     que_ts.wait_time += self.ttek - que_ts.start_waiting_time
-                    if is_semo:
-                        que_ts.wait_semo += self.ttek - que_ts.start_waiting_time
-                        self.servers[c].start_service(que_ts, self.ttek, is_semo=True)
+                    if is_network:
+                        que_ts.wait_network += self.ttek - que_ts.start_waiting_time
+                        self.servers[c].start_service(que_ts, self.ttek, is_network=True)
                     else:
                         self.servers[c].start_service(que_ts, self.ttek)
 
                     self.free_channels -= 1
                     break
         else:
             # одна очередь
@@ -506,15 +506,15 @@
                     self.start_ppnz[k] = self.ttek
                     self.class_ppnz_started = k
 
                 self.taked[k] += 1
                 que_ts.wait_time += self.ttek - que_ts.start_waiting_time
                 self.servers[c].start_service(que_ts, self.ttek)
                 self.free_channels -= 1
-        if is_semo:
+        if is_network:
             return end_ts
 
     def swop_queue(self, last_class, new_class):
         buf = self.queue[last_class]
         self.queue[last_class] = self.queue[new_class]
         self.queue[new_class] = buf
 
@@ -693,22 +693,22 @@
 
 class Task:
     """
     Заявка
     """
     id = 0
 
-    def __init__(self, k, arr_time, is_semo=False):
+    def __init__(self, k, arr_time, is_network=False):
         """
         arr_time: Момент прибытия в СМО
         k - номер класса
         """
-        if is_semo:
-            self.arr_semo = arr_time
-            self.wait_semo = 0
+        if is_network:
+            self.arr_network = arr_time
+            self.wait_network = 0
             self.in_node_class_num = -1
 
         self.arr_time = arr_time
         self.k = k
         self.start_waiting_time = -1
 
         self.wait_time = 0
@@ -765,18 +765,18 @@
         self.prty_type = prty_type
         self.is_free = True
         self.class_on_service = None
         self.tsk_on_service = None
         Server.id += 1
         self.id = Server.id
 
-    def start_service(self, ts, ttek, warm_up=None, is_semo=False):
+    def start_service(self, ts, ttek, warm_up=None, is_network=False):
 
         self.tsk_on_service = ts
-        if is_semo:
+        if is_network:
             self.class_on_service = ts.in_node_class_num
         else:
             self.class_on_service = ts.k
         if warm_up:
             self.total_time_to_serve = warm_up.generate()
             self.time_to_end_service = ttek + self.total_time_to_serve
             self.tsk_on_service.time_to_end_service = self.time_to_end_service
@@ -807,15 +807,15 @@
             res += "\tServing...\n"
             res += "\tTask on service:\n"
             res += "\t\t" + str(self.tsk_on_service.__str__("\t"))
         return res
 
 
 if __name__ == "__main__":
-    from most_queue.theory import prty_calc
+    from most_queue.theory import priority_calc
     import math
     import rand_destribution as rd
     from most_queue.utils.tables import times_print_with_classes
 
     n = 5
     k = 3
     l = [0.2, 0.3, 0.4]
@@ -853,15 +853,15 @@
     qs.set_sources(sources)
     qs.set_servers(servers_params)
 
     qs.run(num_of_jobs)
 
     v_im = qs.v
 
-    v_teor = prty_calc.get_v_prty_invar(l, b, n, 'PR')
+    v_teor = priority_calc.get_v_prty_invar(l, b, n, 'PR')
 
     times_print_with_classes(v_im, v_teor, is_w=False)
 
     print("Относительный приоритет")
 
     qs = PriorityQueueSimulator(n, k, "NP")
     sources = []
@@ -873,10 +873,10 @@
     qs.set_sources(sources)
     qs.set_servers(servers_params)
 
     qs.run(num_of_jobs)
 
     v_im = qs.v
 
-    v_teor = prty_calc.get_v_prty_invar(l, b, n, 'NP')
+    v_teor = priority_calc.get_v_prty_invar(l, b, n, 'NP')
 
     times_print_with_classes(v_im, v_teor, is_w=False)
```

### Comparing `most_queue-1.21/most_queue/sim/qs_sim.py` & `most_queue-1.22/most_queue/sim/qs_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -719,26 +719,25 @@
     from most_queue.utils.tables import times_print, probs_print
 
     n = 3
     l = 1.0
     r = 100
     ro = 0.8
     num_of_jobs = 300000
-    is_cuda = False
 
     mu = l / (ro * n)
 
-    qs = QueueingSystemSimulator(n, buffer=r, cuda=is_cuda)
+    qs = QueueingSystemSimulator(n, buffer=r)
 
     qs.set_sources(l, 'M')
     qs.set_servers(mu, 'M')
 
     qs.run(num_of_jobs)
 
-    w = mmnr_calc.M_M_n_formula.get_w(l, mu, n, r)
+    w = mmnr_calc.MMnr_calc.get_w(l, mu, n, r)
 
     w_im = qs.w
 
     print("Time spent ", qs.time_spent)
 
     times_print(w_im, w)
```

### Comparing `most_queue-1.21/most_queue/sim/queue_finite_source_sim.py` & `most_queue-1.22/most_queue/sim/queue_finite_source_sim.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/sim/rand_destribution.py` & `most_queue-1.22/most_queue/sim/rand_destribution.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/ek_d_n.py` & `most_queue-1.22/most_queue/tests/ek_d_n.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/fj_calc.py` & `most_queue-1.22/most_queue/tests/fj_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/fj_im.py` & `most_queue-1.22/most_queue/tests/fj_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/flow_sum.py` & `most_queue-1.22/most_queue/tests/flow_sum.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/gi_m_1_calc.py` & `most_queue-1.22/most_queue/tests/gi_m_1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/gi_m_n_calc.py` & `most_queue-1.22/most_queue/tests/gi_m_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/m_d_n_calc.py` & `most_queue-1.22/most_queue/tests/m_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/m_h2_h2warm.py` & `most_queue-1.22/most_queue/tests/m_h2_h2warm.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/m_ph_n_prty.py` & `most_queue-1.22/most_queue/tests/m_ph_n_prty.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from most_queue.sim.priority_queue_sim import PriorityQueueSimulator
 from most_queue.sim import rand_destribution as rd
-from most_queue.theory import prty_calc
+from most_queue.theory import priority_calc
 import time
 from most_queue.theory.m_ph_n_prty import m_ph_n_prty
 
 
 def test():
     """
     Тестирование расчета СМО M/PH, M/n с 2-мя классами заявок, абсолютным приоритетом
@@ -85,15 +85,15 @@
         b = []
         b.append(bH)
         b.append(bL)
 
         L = [l_H, l_L]
 
         invar_start = time.process_time()
-        v = prty_calc.get_v_prty_invar(L, b, n=n, type='PR', num=2)
+        v = priority_calc.get_v_prty_invar(L, b, n=n, type='PR', num=2)
         v2_invar_mass.append(v[1][0])
         invar_times.append(time.process_time() - invar_start)
 
         im_start = time.process_time()
 
         for i in range(iteration):
             print("Start IM iteration: {0:d}".format(i + 1))
```

### Comparing `most_queue-1.21/most_queue/tests/mg1_calc.py` & `most_queue-1.22/most_queue/tests/mg1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/mg1_warm_calc.py` & `most_queue-1.22/most_queue/tests/mg1_warm_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/mgn_tt.py` & `most_queue-1.22/most_queue/tests/mgn_tt.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/mmn3_pnz_cox_approx.py` & `most_queue-1.22/most_queue/tests/mmn3_pnz_cox_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/mmn_prty_pnz_approx.py` & `most_queue-1.22/most_queue/tests/mmn_prty_pnz_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/network_im_prty.py` & `most_queue-1.22/most_queue/tests/network_im_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/smo_im.py` & `most_queue-1.22/most_queue/tests/smo_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/tests/smo_im_prty.py` & `most_queue-1.22/most_queue/tests/smo_im_prty.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from most_queue.sim.priority_queue_sim import PriorityQueueSimulator
-from most_queue.theory import prty_calc
+from most_queue.theory import priority_calc
 from most_queue.sim import rand_destribution as rd
 from most_queue.utils.tables import probs_print, times_print_with_classes
 
 def test():
     """
     Тестирование имитационной модели СМО с приоритетами
     Для верификации - сравнение с результатами расчета СМО с методом инвариантов отношения:
@@ -72,15 +72,15 @@
     qs.run(num_of_jobs)
 
     # получение начальных моментов времени пребывания
 
     v_sim = qs.v
 
     # расчет их же методом инвариантов отношения (для сравнения)
-    v_teor = prty_calc.get_v_prty_invar(l, b, n, 'PR')
+    v_teor = priority_calc.get_v_prty_invar(l, b, n, 'PR')
 
     times_print_with_classes(v_sim, v_teor, False)
 
     print("Относительный приоритет")
 
     # Тоже самое для относительного приоритета (NP)
     qs = PriorityQueueSimulator(n, k, "NP")
@@ -93,13 +93,13 @@
     qs.set_sources(sources)
     qs.set_servers(servers_params)
 
     qs.run(num_of_jobs)
 
     v_sim = qs.v
 
-    v_teor = prty_calc.get_v_prty_invar(l, b, n, 'NP')
+    v_teor = priority_calc.get_v_prty_invar(l, b, n, 'NP')
 
     times_print_with_classes(v_sim, v_teor, False)
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.21/most_queue/tests/weibull.py` & `most_queue-1.22/most_queue/tests/weibull.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/batch_mm1.py` & `most_queue-1.22/most_queue/theory/batch_mm1.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/convolution_sum_calc.py` & `most_queue-1.22/most_queue/theory/convolution_sum_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/diff5dots.py` & `most_queue-1.22/most_queue/theory/diff5dots.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/ek_d_n_calc.py` & `most_queue-1.22/most_queue/theory/ek_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/engset_model.py` & `most_queue-1.22/most_queue/theory/engset_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from diff5dots import diff5dots
-import sv_sum_calc
+from most_queue.theory import convolution_sum_calc
 
 
 class Engset:
     """
     Расчет СМО М\М\1 с конечным числом источников m
     """
 
@@ -115,15 +115,15 @@
 
     def get_v(self):
         """
         Начальные моменты времени пребывания через свертку с обслуживанием и дифф ПЛС времени ожидания
         """
         w = self.get_w()
         b = [1.0 / self.mu, 2.0 / pow(self.mu, 2), 6.0 / pow(self.mu, 3)]
-        return sv_sum_calc.get_moments(w, b)
+        return convolution_sum_calc.get_moments(w, b)
 
 
 if __name__ == '__main__':
     from most_queue.utils.tables import times_print
 
     lam = 0.3
     mu = 1.0
```

### Comparing `most_queue-1.21/most_queue/theory/fj_calc.py` & `most_queue-1.22/most_queue/theory/fj_calc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import mmnr_calc
 import mgn_tt
 import mg1_calc
-import sv_sum_calc
+import convolution_sum_calc
 
 import matplotlib.pyplot as plt
 from most_queue.sim import rand_destribution as rd
 import math
 import time
 
 
@@ -300,16 +300,16 @@
 
 
 def get_v1_fj_invar(l, mu, n, r=100):
     mu2 = mu / 2
     mu_n = mu / n
 
     v1_fj2 = get_v1_fj2(l, mu)
-    v1_mmn = mmnr_calc.M_M_n_formula.get_v(l, mu_n, n, r=r)[0]
-    v1_mm2 = mmnr_calc.M_M_n_formula.get_v(l, mu2, 2, r=r)[0]
+    v1_mmn = mmnr_calc.MMnr_calc.get_v(l, mu_n, n, r=r)[0]
+    v1_mm2 = mmnr_calc.MMnr_calc.get_v(l, mu2, 2, r=r)[0]
 
     return v1_fj2 * v1_mmn / v1_mm2
 
 
 def get_v1_fj_invar_sj(l, mu, n):
     mu2 = mu / 2
     mu_n = mu / n
```

### Comparing `most_queue-1.21/most_queue/theory/flow_sum.py` & `most_queue-1.22/most_queue/theory/flow_sum.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/generate_pareto_noise.py` & `most_queue-1.22/most_queue/theory/generate_pareto_noise.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/gi_m_1_calc.py` & `most_queue-1.22/most_queue/theory/gi_m_1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/gi_m_n_calc.py` & `most_queue-1.22/most_queue/theory/gi_m_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/impatience_calc.py` & `most_queue-1.22/most_queue/theory/impatience_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/m_d_n_calc.py` & `most_queue-1.22/most_queue/theory/m_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/m_h2_h2warm.py` & `most_queue-1.22/most_queue/theory/m_h2_h2warm.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/m_ph_n_prty.py` & `most_queue-1.22/most_queue/theory/m_ph_n_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/mg1_calc.py` & `most_queue-1.22/most_queue/theory/mg1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/mg1_warm_calc.py` & `most_queue-1.22/most_queue/theory/mg1_warm_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/mgn_tt.py` & `most_queue-1.22/most_queue/theory/mgn_tt.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/mmn3_pnz_cox_approx.py` & `most_queue-1.22/most_queue/theory/mmn3_pnz_cox_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/mmn_prty_pnz_approx.py` & `most_queue-1.22/most_queue/theory/mmn_prty_pnz_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/mmnr_calc.py` & `most_queue-1.22/most_queue/theory/mmnr_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/network_calc.py` & `most_queue-1.22/most_queue/theory/network_calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from diff5dots import diff5dots
 from most_queue.sim import rand_destribution as rd
 
 import numpy as np
 import math
-import prty_calc
+from most_queue.theory import priority_calc
 
 
 def balance_equation(L, R):
     rows = R.shape[0]
     cols = R.shape[1]
 
     # определяем нулевые строки и столбцы
@@ -135,15 +135,15 @@
 
         for j in range(4):
             for k in range(k_num):
                 b_sr[j] += b_order[i][k][j]
             b_sr[j] /= k_num
 
         res['loads'][i] = l_sum * b_sr[0] / n[i]
-        res['v_node'].append(prty_calc.get_v_prty_invar(l_order[i], b_order[i], n[i], prty[i]))
+        res['v_node'].append(priority_calc.get_v_prty_invar(l_order[i], b_order[i], n[i], prty[i]))
         for k in range(k_num):
             res['v_node'][i][nodes_prty[i][k]] = res['v_node'][i][k]
 
     h = 0.0001
     s = [0.0] * 4
     for i in range(4):
         s[i] = h * (i + 1)
```

### Comparing `most_queue-1.21/most_queue/theory/network_viewer.py` & `most_queue-1.22/most_queue/theory/network_viewer.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/passage_time.py` & `most_queue-1.22/most_queue/theory/passage_time.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/priority_calc.py` & `most_queue-1.22/most_queue/theory/priority_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/q_poisson_arrival_calc.py` & `most_queue-1.22/most_queue/theory/q_poisson_arrival_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/student_stat.py` & `most_queue-1.22/most_queue/theory/student_stat.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/theory/weibull.py` & `most_queue-1.22/most_queue/theory/weibull.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/utils/approx_cdf_make.py` & `most_queue-1.22/most_queue/utils/approx_cdf_make.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/utils/tables.py` & `most_queue-1.22/most_queue/utils/tables.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/visualisation/smo_im_vis.py` & `most_queue-1.22/most_queue/visualisation/smo_im_vis.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/visualisation/utils/result_table.py` & `most_queue-1.22/most_queue/visualisation/utils/result_table.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/visualisation/utils/settings_window.py` & `most_queue-1.22/most_queue/visualisation/utils/settings_window.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue/visualisation/utils/splash_screen.py` & `most_queue-1.22/most_queue/visualisation/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/most_queue.egg-info/PKG-INFO` & `most_queue-1.22/most_queue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: most-queue
-Version: 1.21
+Version: 1.22
 Summary: Software package for calculation and simulation of queuing systems
 Home-page: https://github.com/xabarov/mps
 Author: Xabarov Roman
 Author-email: Xabarov Roman <xabarov1985@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `most_queue-1.21/most_queue.egg-info/SOURCES.txt` & `most_queue-1.22/most_queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `most_queue-1.21/setup.py` & `most_queue-1.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='most-queue',
-      version='1.21',
+      version='1.22',
       description="Software package for calculation and simulation of queuing systems",
       author='Xabarov Roman',
       author_email='xabarov1985@gmail.com',
       url='https://github.com/xabarov/mps',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
```

