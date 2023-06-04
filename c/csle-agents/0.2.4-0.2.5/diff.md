# Comparing `tmp/csle_agents-0.2.4.tar.gz` & `tmp/csle_agents-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_agents-0.2.4.tar", last modified: Wed May 31 13:45:15 2023, max compression
+gzip compressed data, was "csle_agents-0.2.5.tar", last modified: Sun Jun  4 07:14:54 2023, max compression
```

## Comparing `csle_agents-0.2.4.tar` & `csle_agents-0.2.5.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.135732 csle_agents-0.2.4/
--rw-r--r--   0 kimham     (501) staff       (20)      653 2023-05-31 13:45:15.135917 csle_agents-0.2.4/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     4154 2023-01-11 18:45:47.000000 csle_agents-0.2.4/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      671 2023-02-12 08:59:32.000000 csle_agents-0.2.4/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1410 2023-05-31 13:45:15.136566 csle_agents-0.2.4/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_agents-0.2.4/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.098604 csle_agents-0.2.4/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.104905 csle_agents-0.2.4/src/csle_agents/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 13:42:03.000000 csle_agents-0.2.4/src/csle_agents/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.107172 csle_agents-0.2.4/src/csle_agents/agents/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/__init__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.107635 csle_agents-0.2.4/src/csle_agents/agents/base/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/base/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     1854 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/base/base_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.108408 csle_agents-0.2.4/src/csle_agents/agents/bayesian_optimization/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-04-25 08:30:10.000000 csle_agents-0.2.4/src/csle_agents/agents/bayesian_optimization/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    28162 2023-04-25 11:33:39.000000 csle_agents-0.2.4/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.109529 csle_agents-0.2.4/src/csle_agents/agents/cross_entropy/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/cross_entropy/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    26958 2023-05-24 17:32:13.000000 csle_agents-0.2.4/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.111794 csle_agents-0.2.4/src/csle_agents/agents/dfsp_local/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/dfsp_local/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    37993 2023-05-24 17:19:50.000000 csle_agents-0.2.4/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py
--rw-r--r--   0 kimham     (501) staff       (20)    39891 2023-05-24 17:19:50.000000 csle_agents-0.2.4/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.112890 csle_agents-0.2.4/src/csle_agents/agents/differential_evolution/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/differential_evolution/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    31471 2023-05-24 17:30:57.000000 csle_agents-0.2.4/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.114066 csle_agents-0.2.4/src/csle_agents/agents/dqn/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/dqn/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    19153 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/dqn/dqn_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.115133 csle_agents-0.2.4/src/csle_agents/agents/dynasec/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/dynasec/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    75392 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/dynasec/dynasec_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.116252 csle_agents-0.2.4/src/csle_agents/agents/fp/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/fp/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    18259 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/fp/fictitious_play_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.117226 csle_agents-0.2.4/src/csle_agents/agents/hsvi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/hsvi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    49313 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/hsvi/hsvi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.118083 csle_agents-0.2.4/src/csle_agents/agents/hsvi_os_posg/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/hsvi_os_posg/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    75255 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.119253 csle_agents-0.2.4/src/csle_agents/agents/kiefer_wolfowitz/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    28849 2023-04-25 09:34:50.000000 csle_agents-0.2.4/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.120323 csle_agents-0.2.4/src/csle_agents/agents/lp_nf/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/lp_nf/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    18360 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.121497 csle_agents-0.2.4/src/csle_agents/agents/pi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/pi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    17642 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/pi/pi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.122201 csle_agents-0.2.4/src/csle_agents/agents/ppo/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/ppo/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    25589 2023-05-02 09:52:34.000000 csle_agents-0.2.4/src/csle_agents/agents/ppo/ppo_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.123247 csle_agents-0.2.4/src/csle_agents/agents/q_learning/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/q_learning/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    17360 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/q_learning/q_learning_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.123942 csle_agents-0.2.4/src/csle_agents/agents/random_search/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/random_search/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    26175 2023-04-25 09:38:36.000000 csle_agents-0.2.4/src/csle_agents/agents/random_search/random_search_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.125034 csle_agents-0.2.4/src/csle_agents/agents/reinforce/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/reinforce/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    25109 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/reinforce/reinforce_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.126973 csle_agents-0.2.4/src/csle_agents/agents/sarsa/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/sarsa/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    17456 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/sarsa/sarsa_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.127639 csle_agents-0.2.4/src/csle_agents/agents/shapley_iteration/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/shapley_iteration/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    15788 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.128228 csle_agents-0.2.4/src/csle_agents/agents/sondik_vi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/sondik_vi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    22182 2023-03-31 11:14:06.000000 csle_agents-0.2.4/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.128910 csle_agents-0.2.4/src/csle_agents/agents/t_fp/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/t_fp/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    41988 2023-05-01 11:12:26.000000 csle_agents-0.2.4/src/csle_agents/agents/t_fp/t_fp_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.129979 csle_agents-0.2.4/src/csle_agents/agents/t_spsa/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/t_spsa/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    32117 2023-05-24 17:29:31.000000 csle_agents-0.2.4/src/csle_agents/agents/t_spsa/t_spsa_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.130998 csle_agents-0.2.4/src/csle_agents/agents/vi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/agents/vi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    16358 2023-04-29 14:22:16.000000 csle_agents-0.2.4/src/csle_agents/agents/vi/vi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.133493 csle_agents-0.2.4/src/csle_agents/common/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/common/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     5759 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/common/actor_critic_net.py
--rw-r--r--   0 kimham     (501) staff       (20)     4595 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/common/fnn_w_gaussian.py
--rw-r--r--   0 kimham     (501) staff       (20)     3936 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/common/fnn_w_linear.py
--rw-r--r--   0 kimham     (501) staff       (20)     3460 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/common/pruning.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.134472 csle_agents-0.2.4/src/csle_agents/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    11876 2023-05-01 11:24:17.000000 csle_agents-0.2.4/src/csle_agents/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.135232 csle_agents-0.2.4/src/csle_agents/job_controllers/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/job_controllers/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2459 2022-11-28 13:00:49.000000 csle_agents-0.2.4/src/csle_agents/job_controllers/training_job_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:15.106937 csle_agents-0.2.4/src/csle_agents.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      653 2023-05-31 13:45:14.000000 csle_agents-0.2.4/src/csle_agents.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3034 2023-05-31 13:45:15.000000 csle_agents-0.2.4/src/csle_agents.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 13:45:14.000000 csle_agents-0.2.4/src/csle_agents.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:28.000000 csle_agents-0.2.4/src/csle_agents.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      371 2023-05-31 13:45:14.000000 csle_agents-0.2.4/src/csle_agents.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       12 2023-05-31 13:45:15.000000 csle_agents-0.2.4/src/csle_agents.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.137156 csle_agents-0.2.5/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-06-04 07:14:54.137156 csle_agents-0.2.5/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4154 2023-03-28 14:03:22.000000 csle_agents-0.2.5/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-03-28 14:03:22.000000 csle_agents-0.2.5/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1410 2023-06-04 07:14:54.137156 csle_agents-0.2.5/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_agents-0.2.5/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.125156 csle_agents-0.2.5/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.125156 csle_agents-0.2.5/src/csle_agents/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 07:13:34.000000 csle_agents-0.2.5/src/csle_agents/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.125156 csle_agents-0.2.5/src/csle_agents/agents/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.125156 csle_agents-0.2.5/src/csle_agents/agents/base/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/base/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1854 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/base/base_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.125156 csle_agents-0.2.5/src/csle_agents/agents/bayesian_optimization/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/bayesian_optimization/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28162 2023-04-30 06:59:23.000000 csle_agents-0.2.5/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.125156 csle_agents-0.2.5/src/csle_agents/agents/cross_entropy/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/cross_entropy/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    26958 2023-05-30 09:03:51.000000 csle_agents-0.2.5/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.129156 csle_agents-0.2.5/src/csle_agents/agents/dfsp_local/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-03 08:18:28.000000 csle_agents-0.2.5/src/csle_agents/agents/dfsp_local/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    37993 2023-05-22 08:32:58.000000 csle_agents-0.2.5/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    39891 2023-05-03 13:32:44.000000 csle_agents-0.2.5/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.129156 csle_agents-0.2.5/src/csle_agents/agents/differential_evolution/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/differential_evolution/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    31471 2023-05-30 09:03:51.000000 csle_agents-0.2.5/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.129156 csle_agents-0.2.5/src/csle_agents/agents/dqn/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/dqn/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19153 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/dqn/dqn_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.129156 csle_agents-0.2.5/src/csle_agents/agents/dynasec/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/dynasec/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    75392 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/dynasec/dynasec_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.129156 csle_agents-0.2.5/src/csle_agents/agents/fp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/fp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18259 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/fp/fictitious_play_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.129156 csle_agents-0.2.5/src/csle_agents/agents/hsvi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/hsvi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    49313 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/hsvi/hsvi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.129156 csle_agents-0.2.5/src/csle_agents/agents/hsvi_os_posg/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/hsvi_os_posg/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    75255 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.129156 csle_agents-0.2.5/src/csle_agents/agents/kiefer_wolfowitz/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28849 2023-04-30 06:59:23.000000 csle_agents-0.2.5/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.133156 csle_agents-0.2.5/src/csle_agents/agents/lp_nf/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/lp_nf/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18360 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.133156 csle_agents-0.2.5/src/csle_agents/agents/pi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/pi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17642 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/pi/pi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.133156 csle_agents-0.2.5/src/csle_agents/agents/ppo/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/ppo/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    25589 2023-05-03 08:18:28.000000 csle_agents-0.2.5/src/csle_agents/agents/ppo/ppo_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.133156 csle_agents-0.2.5/src/csle_agents/agents/q_learning/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/q_learning/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17360 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/q_learning/q_learning_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.133156 csle_agents-0.2.5/src/csle_agents/agents/random_search/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/random_search/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    26175 2023-04-30 06:59:23.000000 csle_agents-0.2.5/src/csle_agents/agents/random_search/random_search_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.133156 csle_agents-0.2.5/src/csle_agents/agents/reinforce/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/reinforce/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    25109 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/reinforce/reinforce_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.133156 csle_agents-0.2.5/src/csle_agents/agents/sarsa/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/sarsa/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17456 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/sarsa/sarsa_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.133156 csle_agents-0.2.5/src/csle_agents/agents/shapley_iteration/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/shapley_iteration/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15788 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.133156 csle_agents-0.2.5/src/csle_agents/agents/sondik_vi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/sondik_vi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22182 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.133156 csle_agents-0.2.5/src/csle_agents/agents/t_fp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/t_fp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    41988 2023-05-03 08:18:28.000000 csle_agents-0.2.5/src/csle_agents/agents/t_fp/t_fp_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.133156 csle_agents-0.2.5/src/csle_agents/agents/t_spsa/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/t_spsa/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    32117 2023-05-30 09:03:51.000000 csle_agents-0.2.5/src/csle_agents/agents/t_spsa/t_spsa_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.137156 csle_agents-0.2.5/src/csle_agents/agents/vi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/agents/vi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16358 2023-04-30 06:59:23.000000 csle_agents-0.2.5/src/csle_agents/agents/vi/vi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.137156 csle_agents-0.2.5/src/csle_agents/common/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/common/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5759 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/common/actor_critic_net.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4595 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/common/fnn_w_gaussian.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/common/fnn_w_linear.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3460 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/common/pruning.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.137156 csle_agents-0.2.5/src/csle_agents/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11876 2023-05-03 08:18:28.000000 csle_agents-0.2.5/src/csle_agents/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.137156 csle_agents-0.2.5/src/csle_agents/job_controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/job_controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2459 2023-03-28 14:03:22.000000 csle_agents-0.2.5/src/csle_agents/job_controllers/training_job_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:54.125156 csle_agents-0.2.5/src/csle_agents.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-06-04 07:14:53.000000 csle_agents-0.2.5/src/csle_agents.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3034 2023-06-04 07:14:54.000000 csle_agents-0.2.5/src/csle_agents.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 07:14:53.000000 csle_agents-0.2.5/src/csle_agents.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:05.000000 csle_agents-0.2.5/src/csle_agents.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      371 2023-06-04 07:14:54.000000 csle_agents-0.2.5/src/csle_agents.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       12 2023-06-04 07:14:54.000000 csle_agents-0.2.5/src/csle_agents.egg-info/top_level.txt
```

### Comparing `csle_agents-0.2.4/PKG-INFO` & `csle_agents-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_agents
-Version: 0.2.4
+Version: 0.2.5
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.2.4/README.md` & `csle_agents-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/pyproject.toml` & `csle_agents-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/setup.cfg` & `csle_agents-0.2.5/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.2.4
-	csle-collector>=0.2.4
-	csle-attacker>=0.2.4
-	csle-defender>=0.2.4
-	csle-system-identification>=0.2.4
-	gym-csle-stopping-game>=0.2.4
+	csle-common>=0.2.5
+	csle-collector>=0.2.5
+	csle-attacker>=0.2.5
+	csle-defender>=0.2.5
+	csle-system-identification>=0.2.5
+	gym-csle-stopping-game>=0.2.5
 	stable-baselines3>=1.8.0
 	pulp>=2.7.0
 	bayesian-optimization>=1.3.1
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
```

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/base/base_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/base/base_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/dqn/dqn_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/dqn/dqn_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/dynasec/dynasec_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/dynasec/dynasec_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/fp/fictitious_play_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/fp/fictitious_play_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/hsvi/hsvi_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/hsvi/hsvi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/pi/pi_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/pi/pi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/ppo/ppo_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/ppo/ppo_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/q_learning/q_learning_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/q_learning/q_learning_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/random_search/random_search_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/random_search/random_search_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/reinforce/reinforce_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/reinforce/reinforce_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/sarsa/sarsa_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/sarsa/sarsa_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/t_fp/t_fp_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/t_fp/t_fp_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/t_spsa/t_spsa_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/t_spsa/t_spsa_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/agents/vi/vi_agent.py` & `csle_agents-0.2.5/src/csle_agents/agents/vi/vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/common/actor_critic_net.py` & `csle_agents-0.2.5/src/csle_agents/common/actor_critic_net.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/common/fnn_w_gaussian.py` & `csle_agents-0.2.5/src/csle_agents/common/fnn_w_gaussian.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/common/fnn_w_linear.py` & `csle_agents-0.2.5/src/csle_agents/common/fnn_w_linear.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/common/pruning.py` & `csle_agents-0.2.5/src/csle_agents/common/pruning.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/constants/constants.py` & `csle_agents-0.2.5/src/csle_agents/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents/job_controllers/training_job_manager.py` & `csle_agents-0.2.5/src/csle_agents/job_controllers/training_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.4/src/csle_agents.egg-info/PKG-INFO` & `csle_agents-0.2.5/src/csle_agents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-agents
-Version: 0.2.4
+Version: 0.2.5
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.2.4/src/csle_agents.egg-info/SOURCES.txt` & `csle_agents-0.2.5/src/csle_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

