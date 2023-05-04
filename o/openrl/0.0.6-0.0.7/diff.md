# Comparing `tmp/openrl-0.0.6.tar.gz` & `tmp/openrl-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrl-0.0.6.tar", last modified: Fri Apr 28 10:05:16 2023, max compression
+gzip compressed data, was "openrl-0.0.7.tar", last modified: Thu May  4 10:36:38 2023, max compression
```

## Comparing `openrl-0.0.6.tar` & `openrl-0.0.7.tar`

### file list

```diff
@@ -1,173 +1,174 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.776518 openrl-0.0.6/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-28 07:15:42.000000 openrl-0.0.6/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)    11261 2023-04-28 10:05:16.776305 openrl-0.0.6/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)    10202 2023-04-28 07:15:42.000000 openrl-0.0.6/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.752503 openrl-0.0.6/openrl/
--rw-r--r--   0 4paradigm   (501) staff       (20)      194 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.753887 openrl-0.0.6/openrl/algorithms/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/algorithms/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2916 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/algorithms/base_algorithm.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    16410 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/algorithms/ppo.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.754560 openrl-0.0.6/openrl/buffers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/buffers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/buffers/normal_buffer.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    54804 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/buffers/replay_data.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.755583 openrl-0.0.6/openrl/buffers/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/buffers/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1938 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/buffers/utils/obs_data.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/buffers/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.756098 openrl-0.0.6/openrl/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2551 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/cli/cli.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1579 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/cli/train.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.756418 openrl-0.0.6/openrl/configs/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/configs/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    31231 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/configs/config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.757152 openrl-0.0.6/openrl/drivers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/drivers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      238 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/drivers/base_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9929 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/drivers/onpolicy_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      841 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/drivers/rl_driver.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.757300 openrl-0.0.6/openrl/envs/
--rw-r--r--   0 4paradigm   (501) staff       (20)       79 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.757794 openrl-0.0.6/openrl/envs/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      739 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1621 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/common/build_envs.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3305 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/common/registration.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.758126 openrl-0.0.6/openrl/envs/gymnasium/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1425 2023-04-28 09:05:04.000000 openrl-0.0.6/openrl/envs/gymnasium/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.759657 openrl-0.0.6/openrl/envs/mpe/
--rw-r--r--   0 4paradigm   (501) staff       (20)      628 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/core.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      615 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/mpe_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/multi_discrete.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/multiagent_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11650 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/rendering.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      343 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/scenario.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.760034 openrl-0.0.6/openrl/envs/mpe/scenarios/
--rw-r--r--   0 4paradigm   (501) staff       (20)      145 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/scenarios/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4405 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/mpe/scenarios/simple_spread.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.760570 openrl-0.0.6/openrl/envs/nlp/
--rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7514 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/nlp/daily_dialog_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      347 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/nlp_env.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.761850 openrl-0.0.6/openrl/envs/nlp/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2765 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/custom_text_generation_pools.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4515 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/distribution.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1823 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/evaluation_utils.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.762196 openrl-0.0.6/openrl/envs/nlp/utils/metrics/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/metrics/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7088 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/metrics/meteor.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7201 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/observation.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1363 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/sampler.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/nlp/utils/text_generation_pool.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.762935 openrl-0.0.6/openrl/envs/vec_env/
--rw-r--r--   0 4paradigm   (501) staff       (20)      348 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    30978 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/envs/vec_env/async_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7845 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/vec_env/base_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/envs/vec_env/sync_venv.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.763829 openrl-0.0.6/openrl/envs/vec_env/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/vec_env/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6518 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/envs/vec_env/utils/numpy_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7902 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/envs/vec_env/utils/share_memory.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/vec_env/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.764491 openrl-0.0.6/openrl/envs/vec_env/vec_info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1058 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/vec_info/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      585 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/vec_info/base_vec_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2323 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/vec_info/nlp_vec_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1222 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/vec_info/simple_vec_info.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.765234 openrl-0.0.6/openrl/envs/vec_env/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/vec_env/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9266 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/envs/vec_env/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2046 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/wrappers/reward_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1544 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.766127 openrl-0.0.6/openrl/envs/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1612 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/envs/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2454 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/wrappers/extra_wrappers.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/wrappers/multiagent_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/envs/wrappers/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.766960 openrl-0.0.6/openrl/modules/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/base_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.767532 openrl-0.0.6/openrl/modules/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)       57 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/common/base_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3441 2023-04-28 09:15:51.000000 openrl-0.0.6/openrl/modules/common/ppo_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1210 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/model_config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.768638 openrl-0.0.6/openrl/modules/networks/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/base_policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1191 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/base_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6445 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/policy_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3991 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/modules/networks/policy_value_network_gpt.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.770506 openrl-0.0.6/openrl/modules/networks/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7389 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9343 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/attention.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2270 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/cnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      805 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/distributed_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3551 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/distributions.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    10432 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/mix.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5904 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/mlp.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.771122 openrl-0.0.6/openrl/modules/networks/utils/nlp/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/nlp/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11814 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/nlp/base_policy.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    10986 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/modules/networks/utils/nlp/causal_policy.py
--rw-r--r--   0 4paradigm   (501) staff       (20)   188639 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/modules/networks/utils/nlp/hf_generation_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3973 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/popart.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3515 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/rnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3344 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/transformer_act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      317 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/networks/value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7053 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/ppo_module.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5206 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/rl_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.772313 openrl-0.0.6/openrl/modules/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      631 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3599 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/modules/utils/valuenorm.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.772893 openrl-0.0.6/openrl/rewards/
--rw-r--r--   0 4paradigm   (501) staff       (20)      919 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/rewards/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1102 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/rewards/base_reward.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3467 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/rewards/nlp_reward.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.773041 openrl-0.0.6/openrl/runners/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/runners/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.773713 openrl-0.0.6/openrl/runners/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      156 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/runners/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1263 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/runners/common/base_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3185 2023-04-28 09:15:51.000000 openrl-0.0.6/openrl/runners/common/chat_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6083 2023-04-28 09:44:16.000000 openrl-0.0.6/openrl/runners/common/ppo_agent.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.773856 openrl-0.0.6/openrl/supports/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.773989 openrl-0.0.6/openrl/supports/opendata/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/opendata/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.774266 openrl-0.0.6/openrl/supports/opendata/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/opendata/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2132 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/opendata/utils/opendata_utils.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.774787 openrl-0.0.6/openrl/supports/opengpu/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/opengpu/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3897 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/supports/opengpu/gpu_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7051 2023-04-28 09:05:05.000000 openrl-0.0.6/openrl/supports/opengpu/manager.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.775355 openrl-0.0.6/openrl/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5744 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/utils/logger.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1482 2023-04-28 07:15:42.000000 openrl-0.0.6/openrl/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.753259 openrl-0.0.6/openrl.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11261 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     4542 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      284 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-04-28 10:05:16.000000 openrl-0.0.6/openrl.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-04-28 10:05:16.776564 openrl-0.0.6/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     3066 2023-04-28 09:15:51.000000 openrl-0.0.6/setup.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.775497 openrl-0.0.6/tests/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/tests/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.775786 openrl-0.0.6/tests/project/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/tests/project/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      972 2023-04-28 07:15:42.000000 openrl-0.0.6/tests/project/test_version.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-28 10:05:16.776072 openrl-0.0.6/tests/test_buffer/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.6/tests/test_buffer/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-28 07:15:42.000000 openrl-0.0.6/tests/test_buffer/test_buffer.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.431155 openrl-0.0.7/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-28 07:15:42.000000 openrl-0.0.7/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11342 2023-03-23 09:43:52.000000 openrl-0.0.7/LICENSE.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11973 2023-05-04 10:36:38.428981 openrl-0.0.7/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10888 2023-05-04 10:32:54.000000 openrl-0.0.7/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.383222 openrl-0.0.7/openrl/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      194 2023-05-04 10:35:02.000000 openrl-0.0.7/openrl/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.385693 openrl-0.0.7/openrl/algorithms/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/algorithms/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2916 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/algorithms/base_algorithm.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    16410 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/algorithms/ppo.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.386699 openrl-0.0.7/openrl/buffers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/buffers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/buffers/normal_buffer.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    54804 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/buffers/replay_data.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.387857 openrl-0.0.7/openrl/buffers/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/buffers/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1938 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/buffers/utils/obs_data.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/buffers/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.388436 openrl-0.0.7/openrl/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2551 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/cli/cli.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1579 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/cli/train.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.388715 openrl-0.0.7/openrl/configs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/configs/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    31231 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/configs/config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.389502 openrl-0.0.7/openrl/drivers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/drivers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      238 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/drivers/base_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9929 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/drivers/onpolicy_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      841 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/drivers/rl_driver.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.389661 openrl-0.0.7/openrl/envs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       79 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.390182 openrl-0.0.7/openrl/envs/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      739 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1621 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/common/build_envs.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3305 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/common/registration.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.390327 openrl-0.0.7/openrl/envs/gymnasium/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1425 2023-04-28 09:05:04.000000 openrl-0.0.7/openrl/envs/gymnasium/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.391733 openrl-0.0.7/openrl/envs/mpe/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      628 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/core.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      615 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/mpe_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/multi_discrete.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/multiagent_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11650 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/rendering.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      343 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/scenario.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.392297 openrl-0.0.7/openrl/envs/mpe/scenarios/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      145 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/scenarios/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4405 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/scenarios/simple_spread.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.392932 openrl-0.0.7/openrl/envs/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7514 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/nlp/daily_dialog_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      347 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/nlp_env.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.394245 openrl-0.0.7/openrl/envs/nlp/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2765 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/custom_text_generation_pools.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4515 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/distribution.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1823 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/evaluation_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.394627 openrl-0.0.7/openrl/envs/nlp/utils/metrics/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/metrics/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7088 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/metrics/meteor.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7201 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/observation.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1363 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/sampler.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/text_generation_pool.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.395372 openrl-0.0.7/openrl/envs/vec_env/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      348 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/vec_env/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    30978 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/envs/vec_env/async_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7845 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/vec_env/base_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/envs/vec_env/sync_venv.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.396500 openrl-0.0.7/openrl/envs/vec_env/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/vec_env/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6518 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/envs/vec_env/utils/numpy_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7902 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/envs/vec_env/utils/share_memory.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/vec_env/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.397307 openrl-0.0.7/openrl/envs/vec_env/vec_info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1058 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/vec_env/vec_info/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      585 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/vec_env/vec_info/base_vec_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2323 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/vec_env/vec_info/nlp_vec_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1221 2023-05-04 10:32:54.000000 openrl-0.0.7/openrl/envs/vec_env/vec_info/simple_vec_info.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.398342 openrl-0.0.7/openrl/envs/vec_env/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/vec_env/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9266 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/envs/vec_env/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2227 2023-05-04 10:32:54.000000 openrl-0.0.7/openrl/envs/vec_env/wrappers/reward_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1544 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.399772 openrl-0.0.7/openrl/envs/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1612 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2454 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/wrappers/extra_wrappers.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/wrappers/multiagent_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/wrappers/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.400999 openrl-0.0.7/openrl/modules/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/base_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.401662 openrl-0.0.7/openrl/modules/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       57 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/common/base_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3441 2023-04-28 09:15:51.000000 openrl-0.0.7/openrl/modules/common/ppo_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1210 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/model_config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.403369 openrl-0.0.7/openrl/modules/networks/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/base_policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1191 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/base_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6445 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/policy_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3991 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/modules/networks/policy_value_network_gpt.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.406198 openrl-0.0.7/openrl/modules/networks/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7389 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9343 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/attention.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2270 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/cnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      805 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/distributed_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3551 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/distributions.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10432 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/mix.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5904 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/mlp.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.407541 openrl-0.0.7/openrl/modules/networks/utils/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11814 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/nlp/base_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10986 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/modules/networks/utils/nlp/causal_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)   188639 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/modules/networks/utils/nlp/hf_generation_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3973 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/popart.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3515 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/rnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3344 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/transformer_act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      317 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7053 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/ppo_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5206 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/rl_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.409066 openrl-0.0.7/openrl/modules/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      631 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3599 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/utils/valuenorm.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.411385 openrl-0.0.7/openrl/rewards/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      919 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/rewards/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      588 2023-05-04 10:32:54.000000 openrl-0.0.7/openrl/rewards/base_reward.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3467 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/rewards/nlp_reward.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.411672 openrl-0.0.7/openrl/runners/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/runners/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.414173 openrl-0.0.7/openrl/runners/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      156 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/runners/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1263 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/runners/common/base_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3185 2023-04-28 09:15:51.000000 openrl-0.0.7/openrl/runners/common/chat_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6083 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/runners/common/ppo_agent.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.415883 openrl-0.0.7/openrl/supports/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/supports/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.416110 openrl-0.0.7/openrl/supports/opendata/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/supports/opendata/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.418315 openrl-0.0.7/openrl/supports/opendata/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/supports/opendata/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2132 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/supports/opendata/utils/opendata_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.421928 openrl-0.0.7/openrl/supports/opengpu/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/supports/opengpu/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4184 2023-05-04 10:32:54.000000 openrl-0.0.7/openrl/supports/opengpu/gpu_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7113 2023-05-04 10:32:54.000000 openrl-0.0.7/openrl/supports/opengpu/manager.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.422781 openrl-0.0.7/openrl/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5744 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/utils/logger.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1482 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.384760 openrl-0.0.7/openrl.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11973 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4554 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      292 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-05-04 10:36:38.431210 openrl-0.0.7/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3089 2023-05-04 10:32:55.000000 openrl-0.0.7/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.422927 openrl-0.0.7/tests/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/tests/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.424859 openrl-0.0.7/tests/project/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/tests/project/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      972 2023-04-28 07:15:42.000000 openrl-0.0.7/tests/project/test_version.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.428701 openrl-0.0.7/tests/test_buffer/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/tests/test_buffer/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-28 07:15:42.000000 openrl-0.0.7/tests/test_buffer/test_buffer.py
```

### Comparing `openrl-0.0.6/LICENSE` & `openrl-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/PKG-INFO` & `openrl-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrl
-Version: 0.0.6
+Version: 0.0.7
 Summary: unified reinforcement learning framework
 Home-page: https://github.com/OpenRL-Lab/openrl
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openrl
 Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
 Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
@@ -18,14 +18,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: mpe
 Provides-Extra: nlp
 License-File: LICENSE
+License-File: LICENSE.txt
 
 <div align="center">
     <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="./docs/images/openrl_text.png"></a>
 </div>
 
 ---
 [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/openrl/)
@@ -47,15 +48,15 @@
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.6 is updated on April 28, 2023 
+OpenRL-v0.0.7 is updated on April 29, 2023 
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
 OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
 目前，OpenRL支持的特性包括：
@@ -89,14 +90,15 @@
 - [反馈和贡献](#反馈和贡献)
 - [维护人员](#维护人员)
 - [支持者](#支持者)
   - [&#8627; Stargazers](#-stargazers)
   - [&#8627; Forkers](#-forkers)
 - [Citing OpenRL](#citing-openrl)
 - [License](#license)
+- [Acknowledgments](#acknowledgments)
 
 ## 安装
 
 用户可以直接通过pip安装OpenRL:
 ```bash
 pip install openrl
 ```
@@ -190,14 +192,15 @@
 - 加入QQ群：[OpenRL官方交流群](./docs/images/qq.png)
 
 <div align="center">
     <a href="./docs/images/qq.png"><img width="250px" height="auto" src="./docs/images/qq.png"></a>
 </div>
 
 - 加入 [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) 群组，与我们一起讨论OpenRL的使用和开发。
+- 加入 [Discord](https://discord.gg/tyy96TGbep) 群组，与我们一起讨论OpenRL的使用和开发。
 - 发送邮件到: [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)
 - 加入 [GitHub Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
 
 OpenRL框架目前还在持续开发和文档建设，欢迎加入我们让该项目变得更好：
 
 - 如何贡献代码：阅读 [贡献者手册](./CONTRIBUTING.md)
 - [OpenRL开发计划](https://github.com/OpenRL-Lab/openrl/issues/2)
@@ -235,7 +238,18 @@
 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/#OpenRL-Lab/openrl&Date)
 
 ## License
 OpenRL under the Apache 2.0 license.
+
+## Acknowledgments
+The development of the OpenRL framework has drawn on the strengths of other reinforcement learning frameworks:
+
+- Stable-baselines3: https://github.com/DLR-RM/stable-baselines3
+- pytorch-a2c-ppo-acktr-gail: https://github.com/ikostrikov/pytorch-a2c-ppo-acktr-gail
+- MAPPO: https://github.com/marlbenchmark/on-policy
+- Gymnasium: https://github.com/Farama-Foundation/Gymnasium
+- DI-engine: https://github.com/opendilab/DI-engine/
+- Tianshou: https://github.com/thu-ml/tianshou
+- RL4LMs: https://github.com/allenai/RL4LMs
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: openrl Version: 0.0.6 Summary: unified
+Metadata-Version: 2.1 Name: openrl Version: 0.0.7 Summary: unified
 reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
 openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
 URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
 https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
 multi-agent reinforcement-learning-algorithms pytorch machine-learning
 baselines toolbox python data-science gym gymnasium Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Provides-Extra: test Provides-Extra: dev Provides-Extra: mpe Provides-Extra:
-nlp License-File: LICENSE
+nlp License-File: LICENSE License-File: LICENSE.txt
                         [./docs/images/openrl_text.png]
 --- [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/
 openrl/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 openrl) [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/
 version.svg)](https://anaconda.org/openrl/openrl) [![Anaconda-Server Badge]
 (https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://
 anaconda.org/openrl/openrl) [![Anaconda-Server Badge](https://anaconda.org/
@@ -39,15 +39,15 @@
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.6 is updated on April 28,
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.7 is updated on April 29,
 2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£](https://
 openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-
 docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
 OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
 ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
@@ -70,16 +70,17 @@
 CONTRIBUTING.md)ï¼ä¸èµ·ä¸ºå¼ºåå­¦ä¹ çåå±ååºè´¡ç®ã
 å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
 docs.readthedocs.io/zh/latest/)ã ## ç®å½ - [æ¬¢è¿æ¥å°OpenRL]
 (#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [å¿«éä¸æ]
 (#å¿«éä¸æ) - [Gallery](#Gallery) - [ä½¿ç¨OpenRLçé¡¹ç®]
 (#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®](#åé¦åè´¡ç®) - [ç»´æ¤äººå]
 (#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) - [↳ Stargazers](#-stargazers) - [↳
-Forkers](#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) ##
-å®è£ ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
+Forkers](#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
+[Acknowledgments](#acknowledgments) ## å®è£
+ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
 å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
 ```bash conda install -c openrl openrl ```
 ç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone https://github.com/
 OpenRL-Lab/openrl && cd openrl pip install -e . ```
 å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
 ```bash openrl --version ``` ## å¿«éä¸æ
 OpenRLä¸ºå¼ºåå­¦ä¹ å¥é¨ç¨æ·æä¾äºç®åæç¨çæ¥å£ï¼
@@ -127,14 +128,16 @@
 å¦æä½ å¨ç ç©¶é¡¹ç®ä¸­ä½¿ç¨äºOpenRLï¼ä¹æ¬¢è¿å å¥è¯¥åè¡¨ã ##
 åé¦åè´¡ç® - æé®é¢ååç°bugså¯ä»¥å° [Issues](https://github.com/
 OpenRL-Lab/openrl/issues) å¤è¿è¡æ¥è¯¢ææé® - å å¥QQç¾¤ï¼
 [OpenRLå®æ¹äº¤æµç¾¤](./docs/images/qq.png)
                             [./docs/images/qq.png]
 - å å¥ [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-
 Eeh0IxQ~DIaGqYXoW2IUQg)
+ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - å å¥ [Discord]
+(https://discord.gg/tyy96TGbep)
 ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - åéé®ä»¶å°:
 [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) - å å¥ [GitHub
 Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
 OpenRLæ¡æ¶ç®åè¿å¨æç»­å¼ååææ¡£å»ºè®¾ï¼æ¬¢è¿å å¥æä»¬è®©è¯¥é¡¹ç®åå¾æ´å¥½ï¼
 - å¦ä½è´¡ç®ä»£ç ï¼éè¯» [è´¡ç®èæå](./CONTRIBUTING.md) -
 [OpenRLå¼åè®¡å](https://github.com/OpenRL-Lab/openrl/issues/2) ##
 ç»´æ¤äººå ç®åï¼OpenRLç±ä»¥ä¸ç»´æ¤äººåç»´æ¤ï¼ - [Shiyu Huang]
@@ -149,8 +152,16 @@
 //reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/
 openrl/network/members) ## Citing OpenRL
 å¦ææä»¬çå·¥ä½å¯¹ä½ æå¸®å©ï¼æ¬¢è¿å¼ç¨æä»¬: ```latex @misc
 {openrl2023, title={OpenRL}, author={OpenRL Contributors}, publisher =
 {GitHub}, howpublished = {\url{https://github.com/OpenRL-Lab/openrl}}, year=
 {2023}, } ``` ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/
-#OpenRL-Lab/openrl&Date) ## License OpenRL under the Apache 2.0 license.
+#OpenRL-Lab/openrl&Date) ## License OpenRL under the Apache 2.0 license. ##
+Acknowledgments The development of the OpenRL framework has drawn on the
+strengths of other reinforcement learning frameworks: - Stable-baselines3:
+https://github.com/DLR-RM/stable-baselines3 - pytorch-a2c-ppo-acktr-gail:
+https://github.com/ikostrikov/pytorch-a2c-ppo-acktr-gail - MAPPO: https://
+github.com/marlbenchmark/on-policy - Gymnasium: https://github.com/Farama-
+Foundation/Gymnasium - DI-engine: https://github.com/opendilab/DI-engine/ -
+Tianshou: https://github.com/thu-ml/tianshou - RL4LMs: https://github.com/
+allenai/RL4LMs
```

### Comparing `openrl-0.0.6/README.md` & `openrl-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.6 is updated on April 28, 2023 
+OpenRL-v0.0.7 is updated on April 29, 2023 
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
 OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
 目前，OpenRL支持的特性包括：
@@ -64,14 +64,15 @@
 - [反馈和贡献](#反馈和贡献)
 - [维护人员](#维护人员)
 - [支持者](#支持者)
   - [&#8627; Stargazers](#-stargazers)
   - [&#8627; Forkers](#-forkers)
 - [Citing OpenRL](#citing-openrl)
 - [License](#license)
+- [Acknowledgments](#acknowledgments)
 
 ## 安装
 
 用户可以直接通过pip安装OpenRL:
 ```bash
 pip install openrl
 ```
@@ -165,14 +166,15 @@
 - 加入QQ群：[OpenRL官方交流群](./docs/images/qq.png)
 
 <div align="center">
     <a href="./docs/images/qq.png"><img width="250px" height="auto" src="./docs/images/qq.png"></a>
 </div>
 
 - 加入 [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) 群组，与我们一起讨论OpenRL的使用和开发。
+- 加入 [Discord](https://discord.gg/tyy96TGbep) 群组，与我们一起讨论OpenRL的使用和开发。
 - 发送邮件到: [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)
 - 加入 [GitHub Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
 
 OpenRL框架目前还在持续开发和文档建设，欢迎加入我们让该项目变得更好：
 
 - 如何贡献代码：阅读 [贡献者手册](./CONTRIBUTING.md)
 - [OpenRL开发计划](https://github.com/OpenRL-Lab/openrl/issues/2)
@@ -210,7 +212,18 @@
 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/#OpenRL-Lab/openrl&Date)
 
 ## License
 OpenRL under the Apache 2.0 license.
+
+## Acknowledgments
+The development of the OpenRL framework has drawn on the strengths of other reinforcement learning frameworks:
+
+- Stable-baselines3: https://github.com/DLR-RM/stable-baselines3
+- pytorch-a2c-ppo-acktr-gail: https://github.com/ikostrikov/pytorch-a2c-ppo-acktr-gail
+- MAPPO: https://github.com/marlbenchmark/on-policy
+- Gymnasium: https://github.com/Farama-Foundation/Gymnasium
+- DI-engine: https://github.com/opendilab/DI-engine/
+- Tianshou: https://github.com/thu-ml/tianshou
+- RL4LMs: https://github.com/allenai/RL4LMs
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.6 is updated on April 28,
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.7 is updated on April 29,
 2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£](https://
 openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-
 docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
 OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
 ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
@@ -55,16 +55,17 @@
 CONTRIBUTING.md)ï¼ä¸èµ·ä¸ºå¼ºåå­¦ä¹ çåå±ååºè´¡ç®ã
 å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
 docs.readthedocs.io/zh/latest/)ã ## ç®å½ - [æ¬¢è¿æ¥å°OpenRL]
 (#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [å¿«éä¸æ]
 (#å¿«éä¸æ) - [Gallery](#Gallery) - [ä½¿ç¨OpenRLçé¡¹ç®]
 (#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®](#åé¦åè´¡ç®) - [ç»´æ¤äººå]
 (#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) - [↳ Stargazers](#-stargazers) - [↳
-Forkers](#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) ##
-å®è£ ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
+Forkers](#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
+[Acknowledgments](#acknowledgments) ## å®è£
+ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
 å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
 ```bash conda install -c openrl openrl ```
 ç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone https://github.com/
 OpenRL-Lab/openrl && cd openrl pip install -e . ```
 å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
 ```bash openrl --version ``` ## å¿«éä¸æ
 OpenRLä¸ºå¼ºåå­¦ä¹ å¥é¨ç¨æ·æä¾äºç®åæç¨çæ¥å£ï¼
@@ -112,14 +113,16 @@
 å¦æä½ å¨ç ç©¶é¡¹ç®ä¸­ä½¿ç¨äºOpenRLï¼ä¹æ¬¢è¿å å¥è¯¥åè¡¨ã ##
 åé¦åè´¡ç® - æé®é¢ååç°bugså¯ä»¥å° [Issues](https://github.com/
 OpenRL-Lab/openrl/issues) å¤è¿è¡æ¥è¯¢ææé® - å å¥QQç¾¤ï¼
 [OpenRLå®æ¹äº¤æµç¾¤](./docs/images/qq.png)
                             [./docs/images/qq.png]
 - å å¥ [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-
 Eeh0IxQ~DIaGqYXoW2IUQg)
+ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - å å¥ [Discord]
+(https://discord.gg/tyy96TGbep)
 ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - åéé®ä»¶å°:
 [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) - å å¥ [GitHub
 Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
 OpenRLæ¡æ¶ç®åè¿å¨æç»­å¼ååææ¡£å»ºè®¾ï¼æ¬¢è¿å å¥æä»¬è®©è¯¥é¡¹ç®åå¾æ´å¥½ï¼
 - å¦ä½è´¡ç®ä»£ç ï¼éè¯» [è´¡ç®èæå](./CONTRIBUTING.md) -
 [OpenRLå¼åè®¡å](https://github.com/OpenRL-Lab/openrl/issues/2) ##
 ç»´æ¤äººå ç®åï¼OpenRLç±ä»¥ä¸ç»´æ¤äººåç»´æ¤ï¼ - [Shiyu Huang]
@@ -134,8 +137,16 @@
 //reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/
 openrl/network/members) ## Citing OpenRL
 å¦ææä»¬çå·¥ä½å¯¹ä½ æå¸®å©ï¼æ¬¢è¿å¼ç¨æä»¬: ```latex @misc
 {openrl2023, title={OpenRL}, author={OpenRL Contributors}, publisher =
 {GitHub}, howpublished = {\url{https://github.com/OpenRL-Lab/openrl}}, year=
 {2023}, } ``` ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/
-#OpenRL-Lab/openrl&Date) ## License OpenRL under the Apache 2.0 license.
+#OpenRL-Lab/openrl&Date) ## License OpenRL under the Apache 2.0 license. ##
+Acknowledgments The development of the OpenRL framework has drawn on the
+strengths of other reinforcement learning frameworks: - Stable-baselines3:
+https://github.com/DLR-RM/stable-baselines3 - pytorch-a2c-ppo-acktr-gail:
+https://github.com/ikostrikov/pytorch-a2c-ppo-acktr-gail - MAPPO: https://
+github.com/marlbenchmark/on-policy - Gymnasium: https://github.com/Farama-
+Foundation/Gymnasium - DI-engine: https://github.com/opendilab/DI-engine/ -
+Tianshou: https://github.com/thu-ml/tianshou - RL4LMs: https://github.com/
+allenai/RL4LMs
```

### Comparing `openrl-0.0.6/openrl/algorithms/__init__.py` & `openrl-0.0.7/openrl/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/algorithms/base_algorithm.py` & `openrl-0.0.7/openrl/algorithms/base_algorithm.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/algorithms/ppo.py` & `openrl-0.0.7/openrl/algorithms/ppo.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/buffers/__init__.py` & `openrl-0.0.7/openrl/buffers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/buffers/normal_buffer.py` & `openrl-0.0.7/openrl/buffers/normal_buffer.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/buffers/replay_data.py` & `openrl-0.0.7/openrl/buffers/replay_data.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/buffers/utils/__init__.py` & `openrl-0.0.7/openrl/buffers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/buffers/utils/obs_data.py` & `openrl-0.0.7/openrl/buffers/utils/obs_data.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/buffers/utils/util.py` & `openrl-0.0.7/openrl/buffers/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/cli/__init__.py` & `openrl-0.0.7/openrl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/cli/cli.py` & `openrl-0.0.7/openrl/cli/cli.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/cli/train.py` & `openrl-0.0.7/openrl/cli/train.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/configs/__init__.py` & `openrl-0.0.7/openrl/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/configs/config.py` & `openrl-0.0.7/openrl/configs/config.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/drivers/__init__.py` & `openrl-0.0.7/openrl/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/drivers/onpolicy_driver.py` & `openrl-0.0.7/openrl/drivers/onpolicy_driver.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/drivers/rl_driver.py` & `openrl-0.0.7/openrl/drivers/rl_driver.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/common/__init__.py` & `openrl-0.0.7/openrl/envs/common/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/common/build_envs.py` & `openrl-0.0.7/openrl/envs/common/build_envs.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/common/registration.py` & `openrl-0.0.7/openrl/envs/common/registration.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/gymnasium/__init__.py` & `openrl-0.0.7/openrl/envs/gymnasium/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/mpe/__init__.py` & `openrl-0.0.7/openrl/envs/mpe/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/mpe/core.py` & `openrl-0.0.7/openrl/envs/mpe/core.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/mpe/mpe_env.py` & `openrl-0.0.7/openrl/envs/mpe/mpe_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/mpe/multi_discrete.py` & `openrl-0.0.7/openrl/envs/mpe/multi_discrete.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/mpe/multiagent_env.py` & `openrl-0.0.7/openrl/envs/mpe/multiagent_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/mpe/rendering.py` & `openrl-0.0.7/openrl/envs/mpe/rendering.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/mpe/scenarios/simple_spread.py` & `openrl-0.0.7/openrl/envs/mpe/scenarios/simple_spread.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/nlp/__init__.py` & `openrl-0.0.7/openrl/envs/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/nlp/daily_dialog_env.py` & `openrl-0.0.7/openrl/envs/nlp/daily_dialog_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/nlp/utils/custom_text_generation_pools.py` & `openrl-0.0.7/openrl/envs/nlp/utils/custom_text_generation_pools.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/nlp/utils/distribution.py` & `openrl-0.0.7/openrl/envs/nlp/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/nlp/utils/evaluation_utils.py` & `openrl-0.0.7/openrl/envs/nlp/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/nlp/utils/metrics/__init__.py` & `openrl-0.0.7/openrl/envs/nlp/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/nlp/utils/metrics/meteor.py` & `openrl-0.0.7/openrl/envs/nlp/utils/metrics/meteor.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/nlp/utils/observation.py` & `openrl-0.0.7/openrl/envs/nlp/utils/observation.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/nlp/utils/sampler.py` & `openrl-0.0.7/openrl/envs/nlp/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/nlp/utils/text_generation_pool.py` & `openrl-0.0.7/openrl/envs/nlp/utils/text_generation_pool.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/async_venv.py` & `openrl-0.0.7/openrl/envs/vec_env/async_venv.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/base_venv.py` & `openrl-0.0.7/openrl/envs/vec_env/base_venv.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/sync_venv.py` & `openrl-0.0.7/openrl/envs/vec_env/sync_venv.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/utils/__init__.py` & `openrl-0.0.7/openrl/envs/vec_env/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/utils/numpy_utils.py` & `openrl-0.0.7/openrl/envs/vec_env/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/utils/share_memory.py` & `openrl-0.0.7/openrl/envs/vec_env/utils/share_memory.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/utils/util.py` & `openrl-0.0.7/openrl/envs/vec_env/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/vec_info/__init__.py` & `openrl-0.0.7/openrl/envs/vec_env/vec_info/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/vec_info/base_vec_info.py` & `openrl-0.0.7/openrl/envs/vec_env/vec_info/base_vec_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/vec_info/nlp_vec_info.py` & `openrl-0.0.7/openrl/envs/vec_env/vec_info/nlp_vec_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/vec_info/simple_vec_info.py` & `openrl-0.0.7/openrl/envs/vec_env/vec_info/simple_vec_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.infos = []
 
         self.start_time = time.time()
         self.total_step = 0
 
     def statistics(self, buffer: Any) -> Dict[str, Any]:
         # this function should be called each episode
-        rewards = buffer.data.rewardsc.copy()
+        rewards = buffer.data.rewards.copy()
         self.total_step += np.prod(rewards.shape[:2])
         rewards = rewards.transpose(2, 1, 0, 3)
         info_dict = {}
         ep_rewards = []
         for i in range(self.agent_num):
             agent_reward = rewards[i].mean(0).sum()
             ep_rewards.append(agent_reward)
```

### Comparing `openrl-0.0.6/openrl/envs/vec_env/wrappers/__init__.py` & `openrl-0.0.7/openrl/envs/vec_env/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/wrappers/base_wrapper.py` & `openrl-0.0.7/openrl/envs/vec_env/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/vec_env/wrappers/reward_wrapper.py` & `openrl-0.0.7/openrl/envs/vec_env/wrappers/reward_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,13 +43,17 @@
             extra_data.update({"rewards": rewards})
             extra_data.update({"dones": dones})
             extra_data.update({"infos": infos})
             rewards, new_infos = self.reward_class.step_reward(data=extra_data)
 
             num_envs = len(infos)
             for i in range(num_envs):
-                infos[i].update(new_infos[i])
+                if isinstance(infos[i], list):
+                    for j in range(len(infos[i])):
+                        infos[i][j].update(new_infos[i])
+                else:
+                    infos[i].update(new_infos[i])
 
         return obs, rewards, dones, infos
 
     def batch_rewards(self, buffer):
         return self.reward_class.batch_rewards(buffer)
```

### Comparing `openrl-0.0.6/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py` & `openrl-0.0.7/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/wrappers/base_wrapper.py` & `openrl-0.0.7/openrl/envs/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/wrappers/extra_wrappers.py` & `openrl-0.0.7/openrl/envs/wrappers/extra_wrappers.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/wrappers/multiagent_wrapper.py` & `openrl-0.0.7/openrl/envs/wrappers/multiagent_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/envs/wrappers/util.py` & `openrl-0.0.7/openrl/envs/wrappers/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/__init__.py` & `openrl-0.0.7/openrl/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/base_module.py` & `openrl-0.0.7/openrl/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/common/base_net.py` & `openrl-0.0.7/openrl/modules/common/base_net.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/common/ppo_net.py` & `openrl-0.0.7/openrl/modules/common/ppo_net.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/model_config.py` & `openrl-0.0.7/openrl/modules/model_config.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/__init__.py` & `openrl-0.0.7/openrl/modules/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/base_policy_network.py` & `openrl-0.0.7/openrl/modules/networks/base_policy_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/base_value_network.py` & `openrl-0.0.7/openrl/modules/networks/base_value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/policy_network.py` & `openrl-0.0.7/openrl/modules/networks/policy_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/policy_value_network.py` & `openrl-0.0.7/openrl/modules/networks/policy_value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/policy_value_network_gpt.py` & `openrl-0.0.7/openrl/modules/networks/policy_value_network_gpt.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/act.py` & `openrl-0.0.7/openrl/modules/networks/utils/act.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/attention.py` & `openrl-0.0.7/openrl/modules/networks/utils/attention.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/cnn.py` & `openrl-0.0.7/openrl/modules/networks/utils/cnn.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/distributed_utils.py` & `openrl-0.0.7/openrl/modules/networks/utils/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/distributions.py` & `openrl-0.0.7/openrl/modules/networks/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/mix.py` & `openrl-0.0.7/openrl/modules/networks/utils/mix.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/mlp.py` & `openrl-0.0.7/openrl/modules/networks/utils/mlp.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/nlp/base_policy.py` & `openrl-0.0.7/openrl/modules/networks/utils/nlp/base_policy.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/nlp/causal_policy.py` & `openrl-0.0.7/openrl/modules/networks/utils/nlp/causal_policy.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/nlp/hf_generation_utils.py` & `openrl-0.0.7/openrl/modules/networks/utils/nlp/hf_generation_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/popart.py` & `openrl-0.0.7/openrl/modules/networks/utils/popart.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/rnn.py` & `openrl-0.0.7/openrl/modules/networks/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/utils/transformer_act.py` & `openrl-0.0.7/openrl/modules/networks/utils/transformer_act.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/networks/value_network.py` & `openrl-0.0.7/openrl/modules/networks/value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/ppo_module.py` & `openrl-0.0.7/openrl/modules/ppo_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/rl_module.py` & `openrl-0.0.7/openrl/modules/rl_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/utils/__init__.py` & `openrl-0.0.7/openrl/modules/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/utils/util.py` & `openrl-0.0.7/openrl/modules/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/modules/utils/valuenorm.py` & `openrl-0.0.7/openrl/modules/utils/valuenorm.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/rewards/__init__.py` & `openrl-0.0.7/openrl/rewards/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/rewards/nlp_reward.py` & `openrl-0.0.7/openrl/rewards/nlp_reward.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/runners/__init__.py` & `openrl-0.0.7/openrl/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/runners/common/base_agent.py` & `openrl-0.0.7/openrl/runners/common/base_agent.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/runners/common/chat_agent.py` & `openrl-0.0.7/openrl/runners/common/chat_agent.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/runners/common/ppo_agent.py` & `openrl-0.0.7/openrl/runners/common/ppo_agent.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/supports/__init__.py` & `openrl-0.0.7/openrl/supports/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/supports/opendata/__init__.py` & `openrl-0.0.7/openrl/supports/opendata/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/supports/opendata/utils/__init__.py` & `openrl-0.0.7/openrl/supports/opendata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/supports/opendata/utils/opendata_utils.py` & `openrl-0.0.7/openrl/supports/opendata/utils/opendata_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/supports/opengpu/__init__.py` & `openrl-0.0.7/openrl/supports/opengpu/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/supports/opengpu/gpu_info.py` & `openrl-0.0.7/openrl/supports/opengpu/gpu_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,23 +63,33 @@
             return self.memory_total < other.memory_total
 
 
 def get_local_GPU_info():
     cmd = "gpustat --json"
 
     output = subprocess.getoutput(cmd)
+    if "not found" in output:
+        print(
+            "Can not find gpustat. "
+            "Please install gpustat first! "
+            "You can install gpustat by 'pip install gpustat'"
+        )
+        return []
 
     # Deal with vGPU
     output = output.split("\n")
     new_output = []
     for line in output:
         if "4pdvGPU" not in line:
             new_output.append(line)
     output = "\n".join(new_output)
 
+    if "NVML Shared Library Not Found" in output:
+        return []
+
     gpu_dict = json.loads(output)
 
     gpus = gpu_dict["gpus"]
 
     gpu_list = []
 
     if "CUDA_VISIBLE_DEVICES" in os.environ:
```

### Comparing `openrl-0.0.6/openrl/supports/opengpu/manager.py` & `openrl-0.0.7/openrl/supports/opengpu/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import argparse
 import logging
 import traceback
-from typing import List
+from typing import List, Union
 
 from openrl.supports.opengpu.gpu_info import get_local_GPU_info, get_remote_GPU_info
 
 
 class RemoteGPUManager:
     def __init__(self, pytorch_config=None, check: bool = False):
         self.gpu_info_dict = get_remote_GPU_info()
@@ -105,15 +105,15 @@
         return gpu_infos
 
 
 class LocalGPUManager:
     def __init__(self, args: argparse.Namespace = None):
         self.args = args
         self.gpus = []
-        self.learner_num = None if args is None else args.learner_num
+        self.learner_num = 0 if args is None else args.learner_num
         if args is None or not self.args.disable_cuda:
             try:
                 print("LocalGPUManager fetch gpu infos....")
                 self.gpus = get_local_GPU_info()
                 print("LocalGPUManager fetch gpu infos done!")
             except Exception:
                 print("can not find GPU")
@@ -129,16 +129,16 @@
             return self.gpus[0].gpu_id
 
         if self.args.disable_cuda:
             return None
         else:
             return self.gpus[0].gpu_id
 
-    def get_learner_gpu(self, learner_id: int = 0) -> int:
-        if self.args.disable_cuda or len(self.gpus) == 0:
+    def get_learner_gpu(self, learner_id: int = 0) -> Union[int, None]:
+        if self.args is None or (self.args.disable_cuda or len(self.gpus) == 0):
             return None
 
         if self.args.gpu_usage_type == "auto":
             return self.gpus[
                 learner_id if learner_id < len(self.gpus) else len(self.gpus) - 1
             ].gpu_id
         elif self.args.gpu_usage_type == "single":
@@ -168,15 +168,15 @@
                 logging.warning(
                     "unknown gpu usage type:{}!".format(self.args.gpu_usage_type)
                 )
                 gpus.append(None)
         return gpus
 
     def get_worker_gpu(self, worker_id: int = 0) -> int:
-        if self.args.disable_cuda or len(self.gpus) == 0:
+        if self.args is None or (self.args.disable_cuda or len(self.gpus) == 0):
             return None
 
         worker_id += self.args.learner_num
 
         if self.args.gpu_usage_type == "auto":
             return self.gpus[
                 worker_id if worker_id < len(self.gpus) else len(self.gpus) - 1
@@ -190,8 +190,8 @@
             return None
 
     def log_info(self):
         if self.args and self.args.disable_cuda:
             return
 
         for gpu in self.gpus:
-            print(gpu)
+            print(gpu)
```

### Comparing `openrl-0.0.6/openrl/utils/__init__.py` & `openrl-0.0.7/openrl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/utils/logger.py` & `openrl-0.0.7/openrl/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl/utils/util.py` & `openrl-0.0.7/openrl/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/openrl.egg-info/PKG-INFO` & `openrl-0.0.7/openrl.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrl
-Version: 0.0.6
+Version: 0.0.7
 Summary: unified reinforcement learning framework
 Home-page: https://github.com/OpenRL-Lab/openrl
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openrl
 Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
 Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
@@ -18,14 +18,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: mpe
 Provides-Extra: nlp
 License-File: LICENSE
+License-File: LICENSE.txt
 
 <div align="center">
     <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="./docs/images/openrl_text.png"></a>
 </div>
 
 ---
 [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/openrl/)
@@ -47,15 +48,15 @@
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.6 is updated on April 28, 2023 
+OpenRL-v0.0.7 is updated on April 29, 2023 
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
 OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
 目前，OpenRL支持的特性包括：
@@ -89,14 +90,15 @@
 - [反馈和贡献](#反馈和贡献)
 - [维护人员](#维护人员)
 - [支持者](#支持者)
   - [&#8627; Stargazers](#-stargazers)
   - [&#8627; Forkers](#-forkers)
 - [Citing OpenRL](#citing-openrl)
 - [License](#license)
+- [Acknowledgments](#acknowledgments)
 
 ## 安装
 
 用户可以直接通过pip安装OpenRL:
 ```bash
 pip install openrl
 ```
@@ -190,14 +192,15 @@
 - 加入QQ群：[OpenRL官方交流群](./docs/images/qq.png)
 
 <div align="center">
     <a href="./docs/images/qq.png"><img width="250px" height="auto" src="./docs/images/qq.png"></a>
 </div>
 
 - 加入 [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) 群组，与我们一起讨论OpenRL的使用和开发。
+- 加入 [Discord](https://discord.gg/tyy96TGbep) 群组，与我们一起讨论OpenRL的使用和开发。
 - 发送邮件到: [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)
 - 加入 [GitHub Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
 
 OpenRL框架目前还在持续开发和文档建设，欢迎加入我们让该项目变得更好：
 
 - 如何贡献代码：阅读 [贡献者手册](./CONTRIBUTING.md)
 - [OpenRL开发计划](https://github.com/OpenRL-Lab/openrl/issues/2)
@@ -235,7 +238,18 @@
 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/#OpenRL-Lab/openrl&Date)
 
 ## License
 OpenRL under the Apache 2.0 license.
+
+## Acknowledgments
+The development of the OpenRL framework has drawn on the strengths of other reinforcement learning frameworks:
+
+- Stable-baselines3: https://github.com/DLR-RM/stable-baselines3
+- pytorch-a2c-ppo-acktr-gail: https://github.com/ikostrikov/pytorch-a2c-ppo-acktr-gail
+- MAPPO: https://github.com/marlbenchmark/on-policy
+- Gymnasium: https://github.com/Farama-Foundation/Gymnasium
+- DI-engine: https://github.com/opendilab/DI-engine/
+- Tianshou: https://github.com/thu-ml/tianshou
+- RL4LMs: https://github.com/allenai/RL4LMs
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: openrl Version: 0.0.6 Summary: unified
+Metadata-Version: 2.1 Name: openrl Version: 0.0.7 Summary: unified
 reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
 openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
 URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
 https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
 multi-agent reinforcement-learning-algorithms pytorch machine-learning
 baselines toolbox python data-science gym gymnasium Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Provides-Extra: test Provides-Extra: dev Provides-Extra: mpe Provides-Extra:
-nlp License-File: LICENSE
+nlp License-File: LICENSE License-File: LICENSE.txt
                         [./docs/images/openrl_text.png]
 --- [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/
 openrl/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 openrl) [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/
 version.svg)](https://anaconda.org/openrl/openrl) [![Anaconda-Server Badge]
 (https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://
 anaconda.org/openrl/openrl) [![Anaconda-Server Badge](https://anaconda.org/
@@ -39,15 +39,15 @@
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.6 is updated on April 28,
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.7 is updated on April 29,
 2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£](https://
 openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-
 docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
 OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
 ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
@@ -70,16 +70,17 @@
 CONTRIBUTING.md)ï¼ä¸èµ·ä¸ºå¼ºåå­¦ä¹ çåå±ååºè´¡ç®ã
 å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
 docs.readthedocs.io/zh/latest/)ã ## ç®å½ - [æ¬¢è¿æ¥å°OpenRL]
 (#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [å¿«éä¸æ]
 (#å¿«éä¸æ) - [Gallery](#Gallery) - [ä½¿ç¨OpenRLçé¡¹ç®]
 (#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®](#åé¦åè´¡ç®) - [ç»´æ¤äººå]
 (#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) - [↳ Stargazers](#-stargazers) - [↳
-Forkers](#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) ##
-å®è£ ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
+Forkers](#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
+[Acknowledgments](#acknowledgments) ## å®è£
+ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
 å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
 ```bash conda install -c openrl openrl ```
 ç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone https://github.com/
 OpenRL-Lab/openrl && cd openrl pip install -e . ```
 å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
 ```bash openrl --version ``` ## å¿«éä¸æ
 OpenRLä¸ºå¼ºåå­¦ä¹ å¥é¨ç¨æ·æä¾äºç®åæç¨çæ¥å£ï¼
@@ -127,14 +128,16 @@
 å¦æä½ å¨ç ç©¶é¡¹ç®ä¸­ä½¿ç¨äºOpenRLï¼ä¹æ¬¢è¿å å¥è¯¥åè¡¨ã ##
 åé¦åè´¡ç® - æé®é¢ååç°bugså¯ä»¥å° [Issues](https://github.com/
 OpenRL-Lab/openrl/issues) å¤è¿è¡æ¥è¯¢ææé® - å å¥QQç¾¤ï¼
 [OpenRLå®æ¹äº¤æµç¾¤](./docs/images/qq.png)
                             [./docs/images/qq.png]
 - å å¥ [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-
 Eeh0IxQ~DIaGqYXoW2IUQg)
+ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - å å¥ [Discord]
+(https://discord.gg/tyy96TGbep)
 ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - åéé®ä»¶å°:
 [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) - å å¥ [GitHub
 Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
 OpenRLæ¡æ¶ç®åè¿å¨æç»­å¼ååææ¡£å»ºè®¾ï¼æ¬¢è¿å å¥æä»¬è®©è¯¥é¡¹ç®åå¾æ´å¥½ï¼
 - å¦ä½è´¡ç®ä»£ç ï¼éè¯» [è´¡ç®èæå](./CONTRIBUTING.md) -
 [OpenRLå¼åè®¡å](https://github.com/OpenRL-Lab/openrl/issues/2) ##
 ç»´æ¤äººå ç®åï¼OpenRLç±ä»¥ä¸ç»´æ¤äººåç»´æ¤ï¼ - [Shiyu Huang]
@@ -149,8 +152,16 @@
 //reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/
 openrl/network/members) ## Citing OpenRL
 å¦ææä»¬çå·¥ä½å¯¹ä½ æå¸®å©ï¼æ¬¢è¿å¼ç¨æä»¬: ```latex @misc
 {openrl2023, title={OpenRL}, author={OpenRL Contributors}, publisher =
 {GitHub}, howpublished = {\url{https://github.com/OpenRL-Lab/openrl}}, year=
 {2023}, } ``` ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/
-#OpenRL-Lab/openrl&Date) ## License OpenRL under the Apache 2.0 license.
+#OpenRL-Lab/openrl&Date) ## License OpenRL under the Apache 2.0 license. ##
+Acknowledgments The development of the OpenRL framework has drawn on the
+strengths of other reinforcement learning frameworks: - Stable-baselines3:
+https://github.com/DLR-RM/stable-baselines3 - pytorch-a2c-ppo-acktr-gail:
+https://github.com/ikostrikov/pytorch-a2c-ppo-acktr-gail - MAPPO: https://
+github.com/marlbenchmark/on-policy - Gymnasium: https://github.com/Farama-
+Foundation/Gymnasium - DI-engine: https://github.com/opendilab/DI-engine/ -
+Tianshou: https://github.com/thu-ml/tianshou - RL4LMs: https://github.com/
+allenai/RL4LMs
```

### Comparing `openrl-0.0.6/openrl.egg-info/SOURCES.txt` & `openrl-0.0.7/openrl.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+LICENSE.txt
 README.md
 setup.py
 openrl/__init__.py
 openrl.egg-info/PKG-INFO
 openrl.egg-info/SOURCES.txt
 openrl.egg-info/dependency_links.txt
 openrl.egg-info/entry_points.txt
```

### Comparing `openrl-0.0.6/setup.py` & `openrl-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         "test": [
             "pytest",
             "pytest-cov",
             "mypy",
             "isort",
             "black",
             "ruff",
+            "gpustat",
         ],
         "dev": ["build", "twine"],
         "mpe": ["pyglet==1.5.27"],
         "nlp": [
             "stable-baselines3==1.5.1a5",
             "transformers==4.18.0",
             "datasets",
```

### Comparing `openrl-0.0.6/tests/__init__.py` & `openrl-0.0.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/tests/project/__init__.py` & `openrl-0.0.7/tests/project/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/tests/project/test_version.py` & `openrl-0.0.7/tests/project/test_version.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/tests/test_buffer/__init__.py` & `openrl-0.0.7/tests/test_buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.6/tests/test_buffer/test_buffer.py` & `openrl-0.0.7/tests/test_buffer/test_buffer.py`

 * *Files identical despite different names*

