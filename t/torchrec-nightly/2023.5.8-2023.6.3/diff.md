# Comparing `tmp/torchrec_nightly-2023.5.8-py39-none-any.whl.zip` & `tmp/torchrec_nightly-2023.6.3-py39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,141 +1,144 @@
-Zip file size: 339240 bytes, number of entries: 139
--rw-r--r--  2.0 unx      811 b- defN 23-May-08 11:18 torchrec/__init__.py
--rw-r--r--  2.0 unx     1638 b- defN 23-May-08 11:18 torchrec/streamable.py
--rw-r--r--  2.0 unx      854 b- defN 23-May-08 11:18 torchrec/types.py
--rw-r--r--  2.0 unx     1153 b- defN 23-May-08 11:18 torchrec/datasets/__init__.py
--rw-r--r--  2.0 unx    41469 b- defN 23-May-08 11:18 torchrec/datasets/criteo.py
--rw-r--r--  2.0 unx     4548 b- defN 23-May-08 11:18 torchrec/datasets/movielens.py
--rw-r--r--  2.0 unx     6539 b- defN 23-May-08 11:18 torchrec/datasets/random.py
--rw-r--r--  2.0 unx    10909 b- defN 23-May-08 11:18 torchrec/datasets/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-08 11:18 torchrec/datasets/scripts/__init__.py
--rw-r--r--  2.0 unx     2448 b- defN 23-May-08 11:18 torchrec/datasets/scripts/contiguous_preproc_criteo.py
--rw-r--r--  2.0 unx     2847 b- defN 23-May-08 11:18 torchrec/datasets/scripts/npy_preproc_criteo.py
--rw-r--r--  2.0 unx     3077 b- defN 23-May-08 11:18 torchrec/datasets/scripts/shuffle_preproc_criteo.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-08 11:18 torchrec/datasets/test_utils/__init__.py
--rw-r--r--  2.0 unx     5308 b- defN 23-May-08 11:18 torchrec/datasets/test_utils/criteo_test_utils.py
--rw-r--r--  2.0 unx     1912 b- defN 23-May-08 11:18 torchrec/distributed/__init__.py
--rw-r--r--  2.0 unx    36972 b- defN 23-May-08 11:18 torchrec/distributed/batched_embedding_kernel.py
--rw-r--r--  2.0 unx     2069 b- defN 23-May-08 11:18 torchrec/distributed/collective_utils.py
--rw-r--r--  2.0 unx     4988 b- defN 23-May-08 11:18 torchrec/distributed/comm.py
--rw-r--r--  2.0 unx    55820 b- defN 23-May-08 11:18 torchrec/distributed/comm_ops.py
--rw-r--r--  2.0 unx    35443 b- defN 23-May-08 11:18 torchrec/distributed/dist_data.py
--rw-r--r--  2.0 unx    29817 b- defN 23-May-08 11:18 torchrec/distributed/embedding.py
--rw-r--r--  2.0 unx     3872 b- defN 23-May-08 11:18 torchrec/distributed/embedding_kernel.py
--rw-r--r--  2.0 unx    27189 b- defN 23-May-08 11:18 torchrec/distributed/embedding_lookup.py
--rw-r--r--  2.0 unx    14990 b- defN 23-May-08 11:18 torchrec/distributed/embedding_sharding.py
--rw-r--r--  2.0 unx    37089 b- defN 23-May-08 11:18 torchrec/distributed/embedding_tower_sharding.py
--rw-r--r--  2.0 unx    15021 b- defN 23-May-08 11:18 torchrec/distributed/embedding_types.py
--rw-r--r--  2.0 unx    34625 b- defN 23-May-08 11:18 torchrec/distributed/embeddingbag.py
--rw-r--r--  2.0 unx     7373 b- defN 23-May-08 11:18 torchrec/distributed/fbgemm_qcomm_codec.py
--rw-r--r--  2.0 unx     5273 b- defN 23-May-08 11:18 torchrec/distributed/fused_embedding.py
--rw-r--r--  2.0 unx     5110 b- defN 23-May-08 11:18 torchrec/distributed/fused_embeddingbag.py
--rw-r--r--  2.0 unx     1699 b- defN 23-May-08 11:18 torchrec/distributed/fused_params.py
--rw-r--r--  2.0 unx     3807 b- defN 23-May-08 11:18 torchrec/distributed/grouped_position_weighted.py
--rw-r--r--  2.0 unx    19528 b- defN 23-May-08 11:18 torchrec/distributed/model_parallel.py
--rw-r--r--  2.0 unx    13316 b- defN 23-May-08 11:18 torchrec/distributed/quant_embedding.py
--rw-r--r--  2.0 unx    13385 b- defN 23-May-08 11:18 torchrec/distributed/quant_embedding_kernel.py
--rw-r--r--  2.0 unx    10510 b- defN 23-May-08 11:18 torchrec/distributed/quant_embeddingbag.py
--rw-r--r--  2.0 unx     9261 b- defN 23-May-08 11:18 torchrec/distributed/shard.py
--rw-r--r--  2.0 unx    19218 b- defN 23-May-08 11:18 torchrec/distributed/sharding_plan.py
--rw-r--r--  2.0 unx    22330 b- defN 23-May-08 11:18 torchrec/distributed/train_pipeline.py
--rw-r--r--  2.0 unx    24927 b- defN 23-May-08 11:18 torchrec/distributed/types.py
--rw-r--r--  2.0 unx    11373 b- defN 23-May-08 11:18 torchrec/distributed/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-08 11:18 torchrec/distributed/composable/__init__.py
--rw-r--r--  2.0 unx     3207 b- defN 23-May-08 11:18 torchrec/distributed/composable/table_batched_embedding_slice.py
--rw-r--r--  2.0 unx     1025 b- defN 23-May-08 11:18 torchrec/distributed/planner/__init__.py
--rw-r--r--  2.0 unx     3135 b- defN 23-May-08 11:18 torchrec/distributed/planner/constants.py
--rw-r--r--  2.0 unx    10318 b- defN 23-May-08 11:18 torchrec/distributed/planner/enumerators.py
--rw-r--r--  2.0 unx    12485 b- defN 23-May-08 11:18 torchrec/distributed/planner/partitioners.py
--rw-r--r--  2.0 unx      824 b- defN 23-May-08 11:18 torchrec/distributed/planner/perf_models.py
--rw-r--r--  2.0 unx    12224 b- defN 23-May-08 11:18 torchrec/distributed/planner/planners.py
--rw-r--r--  2.0 unx    11094 b- defN 23-May-08 11:18 torchrec/distributed/planner/proposers.py
--rw-r--r--  2.0 unx    40173 b- defN 23-May-08 11:18 torchrec/distributed/planner/shard_estimators.py
--rw-r--r--  2.0 unx    21410 b- defN 23-May-08 11:18 torchrec/distributed/planner/stats.py
--rw-r--r--  2.0 unx     9125 b- defN 23-May-08 11:18 torchrec/distributed/planner/storage_reservations.py
--rw-r--r--  2.0 unx    12879 b- defN 23-May-08 11:18 torchrec/distributed/planner/types.py
--rw-r--r--  2.0 unx     1119 b- defN 23-May-08 11:18 torchrec/distributed/planner/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-08 11:18 torchrec/distributed/sharding/__init__.py
--rw-r--r--  2.0 unx     2539 b- defN 23-May-08 11:18 torchrec/distributed/sharding/cw_sequence_sharding.py
--rw-r--r--  2.0 unx     9519 b- defN 23-May-08 11:18 torchrec/distributed/sharding/cw_sharding.py
--rw-r--r--  2.0 unx     2802 b- defN 23-May-08 11:18 torchrec/distributed/sharding/dp_sequence_sharding.py
--rw-r--r--  2.0 unx     7452 b- defN 23-May-08 11:18 torchrec/distributed/sharding/dp_sharding.py
--rw-r--r--  2.0 unx     5041 b- defN 23-May-08 11:18 torchrec/distributed/sharding/rw_sequence_sharding.py
--rw-r--r--  2.0 unx    12850 b- defN 23-May-08 11:18 torchrec/distributed/sharding/rw_sharding.py
--rw-r--r--  2.0 unx     3114 b- defN 23-May-08 11:18 torchrec/distributed/sharding/sequence_sharding.py
--rw-r--r--  2.0 unx     7609 b- defN 23-May-08 11:18 torchrec/distributed/sharding/tw_sequence_sharding.py
--rw-r--r--  2.0 unx    16061 b- defN 23-May-08 11:18 torchrec/distributed/sharding/tw_sharding.py
--rw-r--r--  2.0 unx     1284 b- defN 23-May-08 11:18 torchrec/distributed/sharding/twcw_sharding.py
--rw-r--r--  2.0 unx    19898 b- defN 23-May-08 11:18 torchrec/distributed/sharding/twrw_sharding.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-08 11:18 torchrec/distributed/test_utils/__init__.py
--rw-r--r--  2.0 unx    10125 b- defN 23-May-08 11:18 torchrec/distributed/test_utils/infer_utils.py
--rw-r--r--  2.0 unx     4868 b- defN 23-May-08 11:18 torchrec/distributed/test_utils/multi_process.py
--rw-r--r--  2.0 unx    34114 b- defN 23-May-08 11:18 torchrec/distributed/test_utils/test_model.py
--rw-r--r--  2.0 unx    11193 b- defN 23-May-08 11:18 torchrec/distributed/test_utils/test_model_parallel.py
--rw-r--r--  2.0 unx    25075 b- defN 23-May-08 11:18 torchrec/distributed/test_utils/test_model_parallel_base.py
--rw-r--r--  2.0 unx    15367 b- defN 23-May-08 11:18 torchrec/distributed/test_utils/test_sharding.py
--rw-r--r--  2.0 unx      422 b- defN 23-May-08 11:18 torchrec/fx/__init__.py
--rw-r--r--  2.0 unx     6477 b- defN 23-May-08 11:18 torchrec/fx/tracer.py
--rw-r--r--  2.0 unx     4401 b- defN 23-May-08 11:18 torchrec/fx/utils.py
--rw-r--r--  2.0 unx     1223 b- defN 23-May-08 11:18 torchrec/inference/__init__.py
--rw-r--r--  2.0 unx     3614 b- defN 23-May-08 11:18 torchrec/inference/client.py
--rw-r--r--  2.0 unx     3957 b- defN 23-May-08 11:18 torchrec/inference/model_packager.py
--rw-r--r--  2.0 unx     7834 b- defN 23-May-08 11:18 torchrec/inference/modules.py
--rw-r--r--  2.0 unx     3797 b- defN 23-May-08 11:18 torchrec/inference/state_dict_transform.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-08 11:18 torchrec/metrics/__init__.py
--rw-r--r--  2.0 unx    12728 b- defN 23-May-08 11:18 torchrec/metrics/auc.py
--rw-r--r--  2.0 unx     3703 b- defN 23-May-08 11:18 torchrec/metrics/calibration.py
--rw-r--r--  2.0 unx     3465 b- defN 23-May-08 11:18 torchrec/metrics/ctr.py
--rw-r--r--  2.0 unx     3836 b- defN 23-May-08 11:18 torchrec/metrics/mae.py
--rw-r--r--  2.0 unx    17812 b- defN 23-May-08 11:18 torchrec/metrics/metric_module.py
--rw-r--r--  2.0 unx     6615 b- defN 23-May-08 11:18 torchrec/metrics/metrics_config.py
--rw-r--r--  2.0 unx     3643 b- defN 23-May-08 11:18 torchrec/metrics/metrics_namespace.py
--rw-r--r--  2.0 unx     3904 b- defN 23-May-08 11:18 torchrec/metrics/model_utils.py
--rw-r--r--  2.0 unx     4631 b- defN 23-May-08 11:18 torchrec/metrics/mse.py
--rw-r--r--  2.0 unx     5605 b- defN 23-May-08 11:18 torchrec/metrics/multiclass_recall.py
--rw-r--r--  2.0 unx     6811 b- defN 23-May-08 11:18 torchrec/metrics/ne.py
--rw-r--r--  2.0 unx    30881 b- defN 23-May-08 11:18 torchrec/metrics/rec_metric.py
--rw-r--r--  2.0 unx    10490 b- defN 23-May-08 11:18 torchrec/metrics/recall_session.py
--rw-r--r--  2.0 unx     6057 b- defN 23-May-08 11:18 torchrec/metrics/throughput.py
--rw-r--r--  2.0 unx    10622 b- defN 23-May-08 11:18 torchrec/metrics/tower_qps.py
--rw-r--r--  2.0 unx     2867 b- defN 23-May-08 11:18 torchrec/metrics/weighted_avg.py
--rw-r--r--  2.0 unx    16441 b- defN 23-May-08 11:18 torchrec/metrics/test_utils/__init__.py
--rw-r--r--  2.0 unx      913 b- defN 23-May-08 11:18 torchrec/models/__init__.py
--rw-r--r--  2.0 unx    11410 b- defN 23-May-08 11:18 torchrec/models/deepfm.py
--rw-r--r--  2.0 unx    30000 b- defN 23-May-08 11:18 torchrec/models/dlrm.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-08 11:18 torchrec/models/experimental/__init__.py
--rw-r--r--  2.0 unx     9823 b- defN 23-May-08 11:18 torchrec/models/experimental/test_transformerdlrm.py
--rw-r--r--  2.0 unx     7434 b- defN 23-May-08 11:18 torchrec/models/experimental/transformerdlrm.py
--rw-r--r--  2.0 unx     1179 b- defN 23-May-08 11:18 torchrec/modules/__init__.py
--rw-r--r--  2.0 unx     1456 b- defN 23-May-08 11:18 torchrec/modules/activation.py
--rw-r--r--  2.0 unx    15163 b- defN 23-May-08 11:18 torchrec/modules/crossnet.py
--rw-r--r--  2.0 unx     8415 b- defN 23-May-08 11:18 torchrec/modules/deepfm.py
--rw-r--r--  2.0 unx     5131 b- defN 23-May-08 11:18 torchrec/modules/embedding_configs.py
--rw-r--r--  2.0 unx    12822 b- defN 23-May-08 11:18 torchrec/modules/embedding_modules.py
--rw-r--r--  2.0 unx     4858 b- defN 23-May-08 11:18 torchrec/modules/embedding_tower.py
--rw-r--r--  2.0 unx    12360 b- defN 23-May-08 11:18 torchrec/modules/feature_processor.py
--rw-r--r--  2.0 unx    31184 b- defN 23-May-08 11:18 torchrec/modules/fused_embedding_modules.py
--rw-r--r--  2.0 unx    10696 b- defN 23-May-08 11:18 torchrec/modules/lazy_extension.py
--rw-r--r--  2.0 unx     6309 b- defN 23-May-08 11:18 torchrec/modules/mlp.py
--rw-r--r--  2.0 unx     4022 b- defN 23-May-08 11:18 torchrec/modules/utils.py
--rw-r--r--  2.0 unx     1639 b- defN 23-May-08 11:18 torchrec/optim/__init__.py
--rw-r--r--  2.0 unx     2012 b- defN 23-May-08 11:18 torchrec/optim/apply_optimizer_in_backward.py
--rw-r--r--  2.0 unx     1569 b- defN 23-May-08 11:18 torchrec/optim/clipping.py
--rw-r--r--  2.0 unx     1353 b- defN 23-May-08 11:18 torchrec/optim/fused.py
--rw-r--r--  2.0 unx    16069 b- defN 23-May-08 11:18 torchrec/optim/keyed.py
--rw-r--r--  2.0 unx     4420 b- defN 23-May-08 11:18 torchrec/optim/optimizers.py
--rw-r--r--  2.0 unx     7405 b- defN 23-May-08 11:18 torchrec/optim/rowwise_adagrad.py
--rw-r--r--  2.0 unx     4865 b- defN 23-May-08 11:18 torchrec/optim/warmup.py
--rw-r--r--  2.0 unx      560 b- defN 23-May-08 11:18 torchrec/optim/test_utils/__init__.py
--rw-r--r--  2.0 unx     1140 b- defN 23-May-08 11:18 torchrec/quant/__init__.py
--rw-r--r--  2.0 unx    22824 b- defN 23-May-08 11:18 torchrec/quant/embedding_modules.py
--rw-r--r--  2.0 unx     3691 b- defN 23-May-08 11:18 torchrec/quant/utils.py
--rw-r--r--  2.0 unx     1163 b- defN 23-May-08 11:18 torchrec/sparse/__init__.py
--rw-r--r--  2.0 unx    52763 b- defN 23-May-08 11:18 torchrec/sparse/jagged_tensor.py
--rw-r--r--  2.0 unx     1430 b- defN 23-May-08 11:18 torchrec/sparse/test_utils/__init__.py
--rw-r--r--  2.0 unx     5661 b- defN 23-May-08 11:18 torchrec/test_utils/__init__.py
--rw-r--r--  2.0 unx     1530 b- defN 23-May-08 11:22 torchrec_nightly-2023.5.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     5011 b- defN 23-May-08 11:22 torchrec_nightly-2023.5.8.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-May-08 11:22 torchrec_nightly-2023.5.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-08 11:22 torchrec_nightly-2023.5.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    12974 b- defN 23-May-08 11:22 torchrec_nightly-2023.5.8.dist-info/RECORD
-139 files, 1379639 bytes uncompressed, 318480 bytes compressed:  76.9%
+Zip file size: 349042 bytes, number of entries: 142
+-rw-r--r--  2.0 unx      811 b- defN 23-Jun-03 11:17 torchrec/__init__.py
+-rw-r--r--  2.0 unx     1638 b- defN 23-Jun-03 11:17 torchrec/streamable.py
+-rw-r--r--  2.0 unx      854 b- defN 23-Jun-03 11:17 torchrec/types.py
+-rw-r--r--  2.0 unx     1153 b- defN 23-Jun-03 11:17 torchrec/datasets/__init__.py
+-rw-r--r--  2.0 unx    41469 b- defN 23-Jun-03 11:17 torchrec/datasets/criteo.py
+-rw-r--r--  2.0 unx     4548 b- defN 23-Jun-03 11:17 torchrec/datasets/movielens.py
+-rw-r--r--  2.0 unx     6539 b- defN 23-Jun-03 11:17 torchrec/datasets/random.py
+-rw-r--r--  2.0 unx    10909 b- defN 23-Jun-03 11:17 torchrec/datasets/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 11:17 torchrec/datasets/scripts/__init__.py
+-rw-r--r--  2.0 unx     2448 b- defN 23-Jun-03 11:17 torchrec/datasets/scripts/contiguous_preproc_criteo.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jun-03 11:17 torchrec/datasets/scripts/npy_preproc_criteo.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-Jun-03 11:17 torchrec/datasets/scripts/shuffle_preproc_criteo.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 11:17 torchrec/datasets/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5308 b- defN 23-Jun-03 11:17 torchrec/datasets/test_utils/criteo_test_utils.py
+-rw-r--r--  2.0 unx     1912 b- defN 23-Jun-03 11:17 torchrec/distributed/__init__.py
+-rw-r--r--  2.0 unx    37053 b- defN 23-Jun-03 11:17 torchrec/distributed/batched_embedding_kernel.py
+-rw-r--r--  2.0 unx     2069 b- defN 23-Jun-03 11:17 torchrec/distributed/collective_utils.py
+-rw-r--r--  2.0 unx     4988 b- defN 23-Jun-03 11:17 torchrec/distributed/comm.py
+-rw-r--r--  2.0 unx    55918 b- defN 23-Jun-03 11:17 torchrec/distributed/comm_ops.py
+-rw-r--r--  2.0 unx    35580 b- defN 23-Jun-03 11:17 torchrec/distributed/dist_data.py
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-03 11:17 torchrec/distributed/embedding.py
+-rw-r--r--  2.0 unx     3872 b- defN 23-Jun-03 11:17 torchrec/distributed/embedding_kernel.py
+-rw-r--r--  2.0 unx    28994 b- defN 23-Jun-03 11:17 torchrec/distributed/embedding_lookup.py
+-rw-r--r--  2.0 unx    18564 b- defN 23-Jun-03 11:17 torchrec/distributed/embedding_sharding.py
+-rw-r--r--  2.0 unx    37089 b- defN 23-Jun-03 11:17 torchrec/distributed/embedding_tower_sharding.py
+-rw-r--r--  2.0 unx    15030 b- defN 23-Jun-03 11:17 torchrec/distributed/embedding_types.py
+-rw-r--r--  2.0 unx    35078 b- defN 23-Jun-03 11:17 torchrec/distributed/embeddingbag.py
+-rw-r--r--  2.0 unx     7373 b- defN 23-Jun-03 11:17 torchrec/distributed/fbgemm_qcomm_codec.py
+-rw-r--r--  2.0 unx     5542 b- defN 23-Jun-03 11:17 torchrec/distributed/fp_embeddingbag.py
+-rw-r--r--  2.0 unx     5273 b- defN 23-Jun-03 11:17 torchrec/distributed/fused_embedding.py
+-rw-r--r--  2.0 unx     5110 b- defN 23-Jun-03 11:17 torchrec/distributed/fused_embeddingbag.py
+-rw-r--r--  2.0 unx     1709 b- defN 23-Jun-03 11:17 torchrec/distributed/fused_params.py
+-rw-r--r--  2.0 unx     3807 b- defN 23-Jun-03 11:17 torchrec/distributed/grouped_position_weighted.py
+-rw-r--r--  2.0 unx    19520 b- defN 23-Jun-03 11:17 torchrec/distributed/model_parallel.py
+-rw-r--r--  2.0 unx    13729 b- defN 23-Jun-03 11:17 torchrec/distributed/quant_embedding.py
+-rw-r--r--  2.0 unx    13343 b- defN 23-Jun-03 11:17 torchrec/distributed/quant_embedding_kernel.py
+-rw-r--r--  2.0 unx    10931 b- defN 23-Jun-03 11:17 torchrec/distributed/quant_embeddingbag.py
+-rw-r--r--  2.0 unx     9261 b- defN 23-Jun-03 11:17 torchrec/distributed/shard.py
+-rw-r--r--  2.0 unx    19411 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding_plan.py
+-rw-r--r--  2.0 unx    34059 b- defN 23-Jun-03 11:17 torchrec/distributed/train_pipeline.py
+-rw-r--r--  2.0 unx    24927 b- defN 23-Jun-03 11:17 torchrec/distributed/types.py
+-rw-r--r--  2.0 unx    11373 b- defN 23-Jun-03 11:17 torchrec/distributed/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 11:17 torchrec/distributed/composable/__init__.py
+-rw-r--r--  2.0 unx     3207 b- defN 23-Jun-03 11:17 torchrec/distributed/composable/table_batched_embedding_slice.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/__init__.py
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/constants.py
+-rw-r--r--  2.0 unx    10318 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/enumerators.py
+-rw-r--r--  2.0 unx    12642 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/partitioners.py
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/perf_models.py
+-rw-r--r--  2.0 unx    13288 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/planners.py
+-rw-r--r--  2.0 unx    11134 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/proposers.py
+-rw-r--r--  2.0 unx    40395 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/shard_estimators.py
+-rw-r--r--  2.0 unx    23617 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/stats.py
+-rw-r--r--  2.0 unx     9125 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/storage_reservations.py
+-rw-r--r--  2.0 unx    13899 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/types.py
+-rw-r--r--  2.0 unx     1119 b- defN 23-Jun-03 11:17 torchrec/distributed/planner/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/__init__.py
+-rw-r--r--  2.0 unx     2539 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/cw_sequence_sharding.py
+-rw-r--r--  2.0 unx     9519 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/cw_sharding.py
+-rw-r--r--  2.0 unx     2802 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/dp_sequence_sharding.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/dp_sharding.py
+-rw-r--r--  2.0 unx     5041 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/rw_sequence_sharding.py
+-rw-r--r--  2.0 unx    12850 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/rw_sharding.py
+-rw-r--r--  2.0 unx     3114 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/sequence_sharding.py
+-rw-r--r--  2.0 unx     7692 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/tw_sequence_sharding.py
+-rw-r--r--  2.0 unx    16315 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/tw_sharding.py
+-rw-r--r--  2.0 unx     1284 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/twcw_sharding.py
+-rw-r--r--  2.0 unx    19898 b- defN 23-Jun-03 11:17 torchrec/distributed/sharding/twrw_sharding.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 11:17 torchrec/distributed/test_utils/__init__.py
+-rw-r--r--  2.0 unx    10213 b- defN 23-Jun-03 11:17 torchrec/distributed/test_utils/infer_utils.py
+-rw-r--r--  2.0 unx     4868 b- defN 23-Jun-03 11:17 torchrec/distributed/test_utils/multi_process.py
+-rw-r--r--  2.0 unx    34114 b- defN 23-Jun-03 11:17 torchrec/distributed/test_utils/test_model.py
+-rw-r--r--  2.0 unx    11193 b- defN 23-Jun-03 11:17 torchrec/distributed/test_utils/test_model_parallel.py
+-rw-r--r--  2.0 unx    25075 b- defN 23-Jun-03 11:17 torchrec/distributed/test_utils/test_model_parallel_base.py
+-rw-r--r--  2.0 unx    15367 b- defN 23-Jun-03 11:17 torchrec/distributed/test_utils/test_sharding.py
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-03 11:17 torchrec/fx/__init__.py
+-rw-r--r--  2.0 unx     6477 b- defN 23-Jun-03 11:17 torchrec/fx/tracer.py
+-rw-r--r--  2.0 unx     4401 b- defN 23-Jun-03 11:17 torchrec/fx/utils.py
+-rw-r--r--  2.0 unx     1223 b- defN 23-Jun-03 11:17 torchrec/inference/__init__.py
+-rw-r--r--  2.0 unx     3614 b- defN 23-Jun-03 11:17 torchrec/inference/client.py
+-rw-r--r--  2.0 unx     3957 b- defN 23-Jun-03 11:17 torchrec/inference/model_packager.py
+-rw-r--r--  2.0 unx     7834 b- defN 23-Jun-03 11:17 torchrec/inference/modules.py
+-rw-r--r--  2.0 unx     3797 b- defN 23-Jun-03 11:17 torchrec/inference/state_dict_transform.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 11:17 torchrec/metrics/__init__.py
+-rw-r--r--  2.0 unx    12549 b- defN 23-Jun-03 11:17 torchrec/metrics/auc.py
+-rw-r--r--  2.0 unx     3703 b- defN 23-Jun-03 11:17 torchrec/metrics/calibration.py
+-rw-r--r--  2.0 unx     3465 b- defN 23-Jun-03 11:17 torchrec/metrics/ctr.py
+-rw-r--r--  2.0 unx     3836 b- defN 23-Jun-03 11:17 torchrec/metrics/mae.py
+-rw-r--r--  2.0 unx    17812 b- defN 23-Jun-03 11:17 torchrec/metrics/metric_module.py
+-rw-r--r--  2.0 unx     6752 b- defN 23-Jun-03 11:17 torchrec/metrics/metrics_config.py
+-rw-r--r--  2.0 unx     3643 b- defN 23-Jun-03 11:17 torchrec/metrics/metrics_namespace.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-Jun-03 11:17 torchrec/metrics/model_utils.py
+-rw-r--r--  2.0 unx     4631 b- defN 23-Jun-03 11:17 torchrec/metrics/mse.py
+-rw-r--r--  2.0 unx     5605 b- defN 23-Jun-03 11:17 torchrec/metrics/multiclass_recall.py
+-rw-r--r--  2.0 unx     6811 b- defN 23-Jun-03 11:17 torchrec/metrics/ne.py
+-rw-r--r--  2.0 unx    31495 b- defN 23-Jun-03 11:17 torchrec/metrics/rec_metric.py
+-rw-r--r--  2.0 unx    10490 b- defN 23-Jun-03 11:17 torchrec/metrics/recall_session.py
+-rw-r--r--  2.0 unx     6057 b- defN 23-Jun-03 11:17 torchrec/metrics/throughput.py
+-rw-r--r--  2.0 unx    10622 b- defN 23-Jun-03 11:17 torchrec/metrics/tower_qps.py
+-rw-r--r--  2.0 unx     2867 b- defN 23-Jun-03 11:17 torchrec/metrics/weighted_avg.py
+-rw-r--r--  2.0 unx    16441 b- defN 23-Jun-03 11:17 torchrec/metrics/test_utils/__init__.py
+-rw-r--r--  2.0 unx      913 b- defN 23-Jun-03 11:17 torchrec/models/__init__.py
+-rw-r--r--  2.0 unx    11410 b- defN 23-Jun-03 11:17 torchrec/models/deepfm.py
+-rw-r--r--  2.0 unx    30000 b- defN 23-Jun-03 11:17 torchrec/models/dlrm.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 11:17 torchrec/models/experimental/__init__.py
+-rw-r--r--  2.0 unx     9825 b- defN 23-Jun-03 11:17 torchrec/models/experimental/test_transformerdlrm.py
+-rw-r--r--  2.0 unx     7434 b- defN 23-Jun-03 11:17 torchrec/models/experimental/transformerdlrm.py
+-rw-r--r--  2.0 unx     1179 b- defN 23-Jun-03 11:17 torchrec/modules/__init__.py
+-rw-r--r--  2.0 unx     1456 b- defN 23-Jun-03 11:17 torchrec/modules/activation.py
+-rw-r--r--  2.0 unx    15163 b- defN 23-Jun-03 11:17 torchrec/modules/crossnet.py
+-rw-r--r--  2.0 unx     8415 b- defN 23-Jun-03 11:17 torchrec/modules/deepfm.py
+-rw-r--r--  2.0 unx     5537 b- defN 23-Jun-03 11:17 torchrec/modules/embedding_configs.py
+-rw-r--r--  2.0 unx    14021 b- defN 23-Jun-03 11:17 torchrec/modules/embedding_modules.py
+-rw-r--r--  2.0 unx     4858 b- defN 23-Jun-03 11:17 torchrec/modules/embedding_tower.py
+-rw-r--r--  2.0 unx    12360 b- defN 23-Jun-03 11:17 torchrec/modules/feature_processor.py
+-rw-r--r--  2.0 unx     2169 b- defN 23-Jun-03 11:17 torchrec/modules/feature_processor_.py
+-rw-r--r--  2.0 unx     4028 b- defN 23-Jun-03 11:17 torchrec/modules/fp_embedding_modules.py
+-rw-r--r--  2.0 unx    31193 b- defN 23-Jun-03 11:17 torchrec/modules/fused_embedding_modules.py
+-rw-r--r--  2.0 unx    10696 b- defN 23-Jun-03 11:17 torchrec/modules/lazy_extension.py
+-rw-r--r--  2.0 unx     6309 b- defN 23-Jun-03 11:17 torchrec/modules/mlp.py
+-rw-r--r--  2.0 unx     4022 b- defN 23-Jun-03 11:17 torchrec/modules/utils.py
+-rw-r--r--  2.0 unx     1639 b- defN 23-Jun-03 11:17 torchrec/optim/__init__.py
+-rw-r--r--  2.0 unx     2012 b- defN 23-Jun-03 11:17 torchrec/optim/apply_optimizer_in_backward.py
+-rw-r--r--  2.0 unx     1569 b- defN 23-Jun-03 11:17 torchrec/optim/clipping.py
+-rw-r--r--  2.0 unx     1353 b- defN 23-Jun-03 11:17 torchrec/optim/fused.py
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-03 11:17 torchrec/optim/keyed.py
+-rw-r--r--  2.0 unx     4420 b- defN 23-Jun-03 11:17 torchrec/optim/optimizers.py
+-rw-r--r--  2.0 unx     7405 b- defN 23-Jun-03 11:17 torchrec/optim/rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4865 b- defN 23-Jun-03 11:17 torchrec/optim/warmup.py
+-rw-r--r--  2.0 unx      560 b- defN 23-Jun-03 11:17 torchrec/optim/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1140 b- defN 23-Jun-03 11:17 torchrec/quant/__init__.py
+-rw-r--r--  2.0 unx    22933 b- defN 23-Jun-03 11:17 torchrec/quant/embedding_modules.py
+-rw-r--r--  2.0 unx     4100 b- defN 23-Jun-03 11:17 torchrec/quant/utils.py
+-rw-r--r--  2.0 unx     1163 b- defN 23-Jun-03 11:17 torchrec/sparse/__init__.py
+-rw-r--r--  2.0 unx    55649 b- defN 23-Jun-03 11:17 torchrec/sparse/jagged_tensor.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Jun-03 11:17 torchrec/sparse/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Jun-03 11:17 torchrec/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1530 b- defN 23-Jun-03 11:22 torchrec_nightly-2023.6.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5011 b- defN 23-Jun-03 11:22 torchrec_nightly-2023.6.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-03 11:22 torchrec_nightly-2023.6.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-03 11:22 torchrec_nightly-2023.6.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    13262 b- defN 23-Jun-03 11:22 torchrec_nightly-2023.6.3.dist-info/RECORD
+142 files, 1421946 bytes uncompressed, 327820 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -78,14 +78,17 @@
 
 Filename: torchrec/distributed/embeddingbag.py
 Comment: 
 
 Filename: torchrec/distributed/fbgemm_qcomm_codec.py
 Comment: 
 
+Filename: torchrec/distributed/fp_embeddingbag.py
+Comment: 
+
 Filename: torchrec/distributed/fused_embedding.py
 Comment: 
 
 Filename: torchrec/distributed/fused_embeddingbag.py
 Comment: 
 
 Filename: torchrec/distributed/fused_params.py
@@ -336,14 +339,20 @@
 
 Filename: torchrec/modules/embedding_tower.py
 Comment: 
 
 Filename: torchrec/modules/feature_processor.py
 Comment: 
 
+Filename: torchrec/modules/feature_processor_.py
+Comment: 
+
+Filename: torchrec/modules/fp_embedding_modules.py
+Comment: 
+
 Filename: torchrec/modules/fused_embedding_modules.py
 Comment: 
 
 Filename: torchrec/modules/lazy_extension.py
 Comment: 
 
 Filename: torchrec/modules/mlp.py
@@ -396,23 +405,23 @@
 
 Filename: torchrec/sparse/test_utils/__init__.py
 Comment: 
 
 Filename: torchrec/test_utils/__init__.py
 Comment: 
 
-Filename: torchrec_nightly-2023.5.8.dist-info/LICENSE
+Filename: torchrec_nightly-2023.6.3.dist-info/LICENSE
 Comment: 
 
-Filename: torchrec_nightly-2023.5.8.dist-info/METADATA
+Filename: torchrec_nightly-2023.6.3.dist-info/METADATA
 Comment: 
 
-Filename: torchrec_nightly-2023.5.8.dist-info/WHEEL
+Filename: torchrec_nightly-2023.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: torchrec_nightly-2023.5.8.dist-info/top_level.txt
+Filename: torchrec_nightly-2023.6.3.dist-info/top_level.txt
 Comment: 
 
-Filename: torchrec_nightly-2023.5.8.dist-info/RECORD
+Filename: torchrec_nightly-2023.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torchrec/distributed/batched_embedding_kernel.py

```diff
@@ -9,19 +9,21 @@
 import copy
 import itertools
 from dataclasses import dataclass
 from typing import Any, cast, Dict, Iterator, List, Optional, Tuple, Union
 
 import torch
 import torch.distributed as dist
-from fbgemm_gpu.split_table_batched_embeddings_ops import (
+from fbgemm_gpu.split_table_batched_embeddings_ops_inference import (
+    IntNBitTableBatchedEmbeddingBagsCodegen,
+)
+from fbgemm_gpu.split_table_batched_embeddings_ops_training import (
     ComputeDevice,
     DenseTableBatchedEmbeddingBagsCodegen,
     EmbeddingLocation,
-    IntNBitTableBatchedEmbeddingBagsCodegen,
     PoolingMode,
     SparseType,
     SplitTableBatchedEmbeddingBagsCodegen,
 )
 from torch import nn
 from torchrec.distributed.composable.table_batched_embedding_slice import (
     TableBatchedEmbeddingSlice,
```

## torchrec/distributed/comm_ops.py

```diff
@@ -38,14 +38,19 @@
 
 
 def set_gradient_division(val: bool) -> None:
     global GRADIENT_DIVISION
     GRADIENT_DIVISION = val
 
 
+def get_gradient_division() -> bool:
+    global GRADIENT_DIVISION
+    return GRADIENT_DIVISION
+
+
 """
 Some commonly used notations for comm ops:
     B - batch size
     T - number of embedding tables
     D - embedding dimension
 """
 
@@ -662,14 +667,15 @@
     ) -> Tensor:
         my_rank = dist.get_rank(pg)
         (B_global, D_local_sum) = input_embeddings.shape
 
         dim_sum_per_rank = a2ai.dim_sum_per_rank
         batch_size_per_rank = a2ai.batch_size_per_rank
         B_local = batch_size_per_rank[my_rank]
+
         assert B_global == sum(batch_size_per_rank)
 
         sharded_input_embeddings = input_embeddings.view(-1)
 
         if a2ai.codecs is not None:
             codecs = none_throws(a2ai.codecs)
             qcomm_ctx = codecs.forward.create_context()
```

## torchrec/distributed/dist_data.py

```diff
@@ -139,25 +139,23 @@
         device (torch.device): device on which buffers are allocated.
         pg (dist.ProcessGroup): ProcessGroup for AlltoAll communication.
     """
 
     def __init__(
         self,
         input_tensors: List[torch.Tensor],
-        num_workers: int,
-        device: torch.device,
         pg: dist.ProcessGroup,
     ) -> None:
         super().__init__()
-        self.num_workers: int = num_workers
+        self.num_workers: int = pg.size()
 
         with record_function("## all2all_data:kjt splits ##"):
             self._output_tensor: torch.Tensor = torch.empty(
-                [num_workers * len(input_tensors)],
-                device=device,
+                [self.num_workers * len(input_tensors)],
+                device=input_tensors[0].device,
                 dtype=input_tensors[0].dtype,
             )
             input_tensor = torch.stack(input_tensors, dim=1).flatten()
             self._splits_awaitable: dist.Work = dist.all_to_all_single(
                 output=self._output_tensor,
                 input=input_tensor,
                 group=pg,
@@ -328,17 +326,15 @@
             torch.tensor(split, device=device) for split in self._input_splits
         ]
         batch_size_tensor = torch.tensor(
             [input.stride()] * self._workers, device=device
         )
         input_tensors.append(batch_size_tensor)
 
-        self._splits_awaitable = SplitsAllToAllAwaitable(
-            input_tensors, self._workers, self._device, self._pg
-        )
+        self._splits_awaitable = SplitsAllToAllAwaitable(input_tensors, self._pg)
 
     def _wait_impl(self) -> KJTAllToAllTensorsAwaitable:
         """
         Overwrites wait function as we don't handle callbacks here.
 
         Returns:
             KJTAllToAllTensorsAwaitable.
@@ -427,17 +423,15 @@
         splits: List[int],
         device: Optional[torch.device] = None,
         stagger: int = 1,
     ) -> None:
         super().__init__()
         assert len(splits) == pg.size()
         self._pg: dist.ProcessGroup = pg
-        self._workers: int = pg.size()
         self._splits = splits
-        self._no_dist: bool = all(s == 0 for s in splits)
         self._splits_cumsum: List[int] = [0] + list(itertools.accumulate(splits))
         self._stagger = stagger
 
     def forward(
         self, input: KeyedJaggedTensor
     ) -> Awaitable[KJTAllToAllTensorsAwaitable]:
         """
@@ -450,15 +444,14 @@
             input (KeyedJaggedTensor): `KeyedJaggedTensor` of values to distribute.
 
         Returns:
             Awaitable[KJTAllToAllTensorsAwaitable]: awaitable of a `KJTAllToAllTensorsAwaitable`.
         """
 
         device = input.values().device
-
         with torch.no_grad():
             assert len(input.keys()) == sum(self._splits)
             rank = dist.get_rank(self._pg)
             local_keys = input.keys()[
                 self._splits_cumsum[rank] : self._splits_cumsum[rank + 1]
             ]
 
@@ -482,24 +475,29 @@
     Implementation utilizes OnetoAll function, which essentially P2P copies the feature
     to the devices.
 
     Args:
         splits (List[int]): lengths of features to split the `KeyJaggedTensor` features
             into before copying them.
         world_size (int): number of devices in the topology.
+        device (torch.device): the device on which the KJTs will be allocated.
     """
 
     def __init__(
         self,
         splits: List[int],
         world_size: int,
+        device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
         self._splits = splits
         self._world_size = world_size
+        self._device_type = (
+            "cuda" if device is None or device.type == "cuda" else "meta"
+        )
         assert self._world_size == len(splits)
 
     def forward(self, kjt: KeyedJaggedTensor) -> KJTList:
         """
         Splits features first and then sends the slices to the corresponding devices.
 
         Args:
@@ -507,15 +505,17 @@
 
         Returns:
             Awaitable[List[KeyedJaggedTensor]]: awaitable of `KeyedJaggedTensor` splits.
         """
         fx_marker("KJT_ONE_TO_ALL_FORWARD_BEGIN", kjt)
         kjts: List[KeyedJaggedTensor] = kjt.split(self._splits)
         dist_kjts = [
-            kjts[rank].to(torch.device("cuda", rank), non_blocking=True)
+            kjts[rank]
+            if self._device_type == "meta"
+            else kjts[rank].to(torch.device(self._device_type, rank), non_blocking=True)
             for rank in range(self._world_size)
         ]
         ret = KJTList(dist_kjts)
         fx_marker("KJT_ONE_TO_ALL_FORWARD_END", kjt)
         return ret
```

## torchrec/distributed/embedding.py

```diff
@@ -514,14 +514,26 @@
                 destination[destination_key] = sharded_t
 
         self._register_state_dict_hook(post_state_dict_hook)
         self._register_load_state_dict_pre_hook(
             self._pre_load_state_dict_hook, with_module=True
         )
 
+        self.reset_parameters()
+
+    def reset_parameters(self) -> None:
+        if self._device and self._device.type == "meta":
+            return
+        # Initialize embedding weights with init_fn
+        for table_config in self._embedding_configs:
+            assert table_config.init_fn is not None
+            param = self.embeddings[f"{table_config.name}"].weight
+            # pyre-ignore
+            table_config.init_fn(param)
+
     def _generate_permute_indices_per_feature(
         self,
         embedding_configs: List[EmbeddingConfig],
         table_name_to_parameter_sharding: Dict[str, ParameterSharding],
     ) -> None:
         """
         Generates permute indices per feature for column-wise sharding.
```

## torchrec/distributed/embedding_lookup.py

```diff
@@ -8,27 +8,30 @@
 import logging
 from abc import ABC
 from collections import OrderedDict
 from typing import Any, cast, Dict, Iterator, List, Optional, Tuple, Union
 
 import torch
 import torch.distributed as dist
-from fbgemm_gpu.split_table_batched_embeddings_ops import (
+from fbgemm_gpu.split_table_batched_embeddings_ops_inference import (
     IntNBitTableBatchedEmbeddingBagsCodegen,
 )
 from torch import nn
+
+from torch.autograd.function import FunctionCtx
 from torch.nn.modules.module import _IncompatibleKeys
 from torchrec.distributed.batched_embedding_kernel import (
     BaseBatchedEmbedding,
     BaseBatchedEmbeddingBag,
     BatchedDenseEmbedding,
     BatchedDenseEmbeddingBag,
     BatchedFusedEmbedding,
     BatchedFusedEmbeddingBag,
 )
+from torchrec.distributed.comm_ops import get_gradient_division
 from torchrec.distributed.composable.table_batched_embedding_slice import (
     TableBatchedEmbeddingSlice,
 )
 from torchrec.distributed.embedding_kernel import BaseEmbedding
 from torchrec.distributed.embedding_types import (
     BaseEmbeddingLookup,
     BaseGroupedFeatureProcessor,
@@ -235,27 +238,52 @@
             for (
                 table_name,
                 tbe_slice,
             ) in embedding_kernel.named_parameters_by_table():
                 yield (table_name, tbe_slice)
 
 
+class CommOpGradientScaling(torch.autograd.Function):
+    @staticmethod
+    # pyre-ignore
+    def forward(
+        ctx: FunctionCtx, input_tensor: torch.Tensor, scale_gradient_factor: int
+    ) -> torch.Tensor:
+        # pyre-ignore
+        ctx.scale_gradient_factor = scale_gradient_factor
+        return input_tensor
+
+    @staticmethod
+    # pyre-ignore[14]: `forward` overrides method defined in `Function` inconsistently.
+    def backward(
+        ctx: FunctionCtx, grad_output: torch.Tensor
+    ) -> Tuple[torch.Tensor, None]:
+        # When gradient division is on, we scale down the gradient by world size
+        # at alltoall backward for model parallelism. However weights
+        # is controlled by DDP so it already has gradient division, so we scale
+        # the gradient back up
+        # pyre-ignore[16]: `FunctionCtx` has no attribute `scale_gradient_factor`
+        grad_output.mul_(ctx.scale_gradient_factor)
+        return grad_output, None
+
+
 class GroupedPooledEmbeddingsLookup(
     BaseEmbeddingLookup[KeyedJaggedTensor, torch.Tensor]
 ):
     """
     Lookup modules for Pooled embeddings (i.e EmbeddingBags)
     """
 
     def __init__(
         self,
         grouped_configs: List[GroupedEmbeddingConfig],
         device: Optional[torch.device] = None,
         pg: Optional[dist.ProcessGroup] = None,
         feature_processor: Optional[BaseGroupedFeatureProcessor] = None,
+        scale_weight_gradients: bool = True,
     ) -> None:
         # TODO rename to _create_embedding_kernel
         def _create_lookup(
             config: GroupedEmbeddingConfig,
             device: Optional[torch.device] = None,
         ) -> BaseEmbedding:
             if config.compute_kernel == EmbeddingComputeKernel.DENSE:
@@ -294,14 +322,20 @@
                 requires_grad=True,
             ),
         )
 
         self.grouped_configs = grouped_configs
         self._feature_processor = feature_processor
 
+        self._scale_gradient_factor: int = (
+            dist.get_world_size(pg)
+            if scale_weight_gradients and get_gradient_division()
+            else 1
+        )
+
     def forward(
         self,
         sparse_features: KeyedJaggedTensor,
     ) -> torch.Tensor:
         embeddings: List[torch.Tensor] = []
         if len(self._emb_modules) > 0:
             assert sparse_features is not None
@@ -313,15 +347,22 @@
             ):
                 if (
                     config.has_feature_processor
                     and self._feature_processor is not None
                     and isinstance(self._feature_processor, BaseGroupedFeatureProcessor)
                 ):
                     features = self._feature_processor(features)
+
+                if config.is_weighted:
+                    features._weights = CommOpGradientScaling.apply(
+                        features._weights, self._scale_gradient_factor
+                    )
+
                 embeddings.append(emb_op(features))
+
         return embeddings_cat_empty_rank_handle(
             embeddings,
             fx_wrap_tensor_view2d(self._dummy_embs_tensor, sparse_features.stride(), 0),
             dim=1,
         )
 
     # pyre-fixme[14]: `state_dict` overrides method defined in `Module` inconsistently.
@@ -702,26 +743,29 @@
     TBEToRegisterMixIn,
 ):
     def __init__(
         self,
         grouped_configs_per_rank: List[List[GroupedEmbeddingConfig]],
         world_size: int,
         fused_params: Optional[Dict[str, Any]] = None,
+        device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
         self._embedding_lookups_per_rank: List[
             MetaInferGroupedPooledEmbeddingsLookup
         ] = []
+
+        device_type = "cuda" if device is None or device.type == "cuda" else "meta"
         for rank in range(world_size):
             self._embedding_lookups_per_rank.append(
                 # TODO add position weighted module support
                 MetaInferGroupedPooledEmbeddingsLookup(
                     grouped_configs=grouped_configs_per_rank[rank],
                     # syntax for torchscript
-                    device=torch.device(f"cuda:{rank}"),
+                    device=torch.device(type=device_type, index=rank),
                     fused_params=fused_params,
                 )
             )
 
     def get_tbes_to_register(
         self,
     ) -> Dict[IntNBitTableBatchedEmbeddingBagsCodegen, GroupedEmbeddingConfig]:
@@ -734,23 +778,27 @@
     TBEToRegisterMixIn,
 ):
     def __init__(
         self,
         grouped_configs_per_rank: List[List[GroupedEmbeddingConfig]],
         world_size: int,
         fused_params: Optional[Dict[str, Any]] = None,
+        device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
         self._embedding_lookups_per_rank: List[MetaInferGroupedEmbeddingsLookup] = []
+
+        device_type = "cuda" if device is None or device.type == "cuda" else "meta"
+
         for rank in range(world_size):
             self._embedding_lookups_per_rank.append(
                 MetaInferGroupedEmbeddingsLookup(
                     grouped_configs=grouped_configs_per_rank[rank],
                     # syntax for torchscript
-                    device=torch.device(f"cuda:{rank}"),
+                    device=torch.device(type=device_type, index=rank),
                     fused_params=fused_params,
                 )
             )
 
     def get_tbes_to_register(
         self,
     ) -> Dict[IntNBitTableBatchedEmbeddingBagsCodegen, GroupedEmbeddingConfig]:
```

## torchrec/distributed/embedding_sharding.py

```diff
@@ -6,16 +6,19 @@
 # LICENSE file in the root directory of this source tree.
 
 import abc
 from dataclasses import dataclass, field
 from typing import Any, Dict, Generic, List, Optional, Tuple, TypeVar, Union
 
 import torch
-from torch import nn
-from torchrec.distributed.dist_data import KJTAllToAllTensorsAwaitable
+from torch import distributed as dist, nn
+from torchrec.distributed.dist_data import (
+    KJTAllToAllTensorsAwaitable,
+    SplitsAllToAllAwaitable,
+)
 from torchrec.distributed.embedding_types import (
     BaseEmbeddingLookup,
     BaseGroupedFeatureProcessor,
     EmbeddingComputeKernel,
     FeatureShardingMixIn,
     GroupedEmbeddingConfig,
     KJTList,
@@ -229,14 +232,40 @@
             KJTList: synced `KJTList`.
         """
 
         return KJTList([w.wait() for w in self.awaitables])
 
 
 C = TypeVar("C", bound=Multistreamable)
+T = TypeVar("T")
+
+
+def _set_sharding_context(
+    tensors_awaitables: List[Awaitable[KeyedJaggedTensor]],
+    ctx: C,
+) -> None:
+    for awaitable, sharding_context in zip(
+        tensors_awaitables,
+        getattr(ctx, "sharding_contexts", []),
+    ):
+        if isinstance(awaitable, KJTAllToAllTensorsAwaitable):
+            if hasattr(sharding_context, "batch_size_per_rank"):
+                sharding_context.batch_size_per_rank = awaitable._batch_size_per_rank
+            if hasattr(sharding_context, "input_splits"):
+                sharding_context.input_splits = awaitable._input_splits["values"]
+            if hasattr(sharding_context, "output_splits"):
+                sharding_context.output_splits = awaitable._output_splits["values"]
+            if hasattr(sharding_context, "sparse_features_recat"):
+                sharding_context.sparse_features_recat = awaitable._recat
+
+
+def _split(flat_list: List[T], splits: List[int]) -> List[List[T]]:
+    return [
+        flat_list[sum(splits[:i]) : sum(splits[:i]) + n] for i, n in enumerate(splits)
+    ]
 
 
 class KJTListSplitsAwaitable(Awaitable[Awaitable[KJTList]], Generic[C]):
     """
     Awaitable of Awaitable of KJTList.
 
     Args:
@@ -263,32 +292,107 @@
         The first wait gets the result of splits AlltoAll and returns the tensors
         awaitable.
 
         Returns:
             KJTListAwaitable: awaitables for tensors of the sparse features.
         """
         tensors_awaitables = [w.wait() for w in self.awaitables]
-        for awaitable, sharding_context in zip(
-            tensors_awaitables,
-            getattr(self.ctx, "sharding_contexts", []),
-        ):
-            if isinstance(awaitable, KJTAllToAllTensorsAwaitable):
-                if hasattr(sharding_context, "batch_size_per_rank"):
-                    sharding_context.batch_size_per_rank = (
-                        awaitable._batch_size_per_rank
-                    )
-                if hasattr(sharding_context, "input_splits"):
-                    sharding_context.input_splits = awaitable._input_splits["values"]
-                if hasattr(sharding_context, "output_splits"):
-                    sharding_context.output_splits = awaitable._output_splits["values"]
-                if hasattr(sharding_context, "sparse_features_recat"):
-                    sharding_context.sparse_features_recat = awaitable._recat
+        _set_sharding_context(tensors_awaitables, self.ctx)
         return KJTListAwaitable(tensors_awaitables)
 
 
+@dataclass
+class KJTSplitsAllToAllMeta:
+    pg: dist.ProcessGroup
+    input: KeyedJaggedTensor
+    splits: List[int]
+    splits_tensors: List[torch.Tensor]
+    input_splits: List[List[int]]
+    input_tensors: List[torch.Tensor]
+    labels: List[str]
+    keys: List[str]
+    device: torch.device
+    stagger: int
+
+
+class FusedKJTListSplitsAwaitable(Awaitable[List[KJTListAwaitable]]):
+    def __init__(
+        self,
+        requests: List[KJTListSplitsAwaitable[C]],
+        contexts: List[C],
+        pg: Optional[dist.ProcessGroup],
+    ) -> None:
+        super().__init__()
+        self._contexts = contexts
+        self._awaitables: List[
+            Union[KJTSplitsAllToAllMeta, Awaitable[Awaitable[KeyedJaggedTensor]]]
+        ] = [awaitable for request in requests for awaitable in request.awaitables]
+        self._output_lengths: List[int] = [
+            len(request.awaitables) for request in requests
+        ]
+        self._lengths: List[int] = [
+            len(awaitable.splits_tensors)
+            if isinstance(awaitable, KJTSplitsAllToAllMeta)
+            else 0
+            for awaitable in self._awaitables
+        ]
+        splits_tensors = [
+            splits_tensor
+            for awaitable in self._awaitables
+            for splits_tensor in (
+                awaitable.splits_tensors
+                if isinstance(awaitable, KJTSplitsAllToAllMeta)
+                else []
+            )
+        ]
+        self._splits_awaitable: Optional[SplitsAllToAllAwaitable] = (
+            SplitsAllToAllAwaitable(
+                input_tensors=splits_tensors,
+                pg=pg,
+            )
+            if splits_tensors and pg
+            else None
+        )
+
+    def _wait_impl(self) -> List[KJTListAwaitable]:
+        if self._splits_awaitable:
+            splits_list = self._splits_awaitable.wait()
+            splits_per_awaitable = _split(splits_list, self._lengths)
+        else:
+            splits_per_awaitable = [[] for _ in range(len(self._lengths))]
+        tensors_awaitables = []
+        for splits, awaitable in zip(splits_per_awaitable, self._awaitables):
+            if not splits:  # NoWait
+                tensors_awaitables.append(awaitable.wait())
+                continue
+            output_splits = splits[:-1]
+            batch_size_per_rank = splits[-1]
+            tensors_awaitables.append(
+                KJTAllToAllTensorsAwaitable(
+                    pg=awaitable.pg,
+                    input=awaitable.input,
+                    splits=awaitable.splits,
+                    input_splits=awaitable.input_splits,
+                    output_splits=output_splits,
+                    input_tensors=awaitable.input_tensors,
+                    labels=awaitable.labels,
+                    batch_size_per_rank=batch_size_per_rank,
+                    keys=awaitable.keys,
+                    device=awaitable.device,
+                    stagger=awaitable.stagger,
+                )
+            )
+        output = []
+        awaitables_per_output = _split(tensors_awaitables, self._output_lengths)
+        for awaitables, ctx in zip(awaitables_per_output, self._contexts):
+            _set_sharding_context(awaitables, ctx)
+            output.append(KJTListAwaitable(awaitables))
+        return output
+
+
 class ListOfKJTListAwaitable(Awaitable[ListOfKJTList]):
     """
     This module handles the tables-wise sharding input features distribution for
     inference.
 
     Args:
         awaitables (List[Awaitable[KJTList]]): list of `Awaitable` of `KJTList`.
```

## torchrec/distributed/embedding_types.py

```diff
@@ -7,15 +7,15 @@
 
 import abc
 from dataclasses import dataclass
 from enum import Enum, unique
 from typing import Any, Dict, Generic, Iterator, List, Optional, TypeVar
 
 import torch
-from fbgemm_gpu.split_table_batched_embeddings_ops import EmbeddingLocation
+from fbgemm_gpu.split_table_batched_embeddings_ops_training import EmbeddingLocation
 from torch import fx, nn
 from torch.nn.modules.module import _addindent
 from torchrec.distributed.types import (
     ModuleSharder,
     ParameterStorage,
     QuantizedCommCodecs,
     ShardedModule,
```

## torchrec/distributed/embeddingbag.py

```diff
@@ -544,14 +544,26 @@
                 destination_key = f"{prefix}embedding_bags.{table_name}.weight"
                 destination[destination_key] = sharded_t
 
         self._register_state_dict_hook(post_state_dict_hook)
         self._register_load_state_dict_pre_hook(
             self._pre_load_state_dict_hook, with_module=True
         )
+        self.reset_parameters()
+
+    def reset_parameters(self) -> None:
+        if self._device and self._device.type == "meta":
+            return
+
+        # Initialize embedding bags weights with init_fn
+        for table_config in self._embedding_bag_configs:
+            assert table_config.init_fn is not None
+            param = self.embedding_bags[f"{table_config.name}"].weight
+            # pyre-ignore
+            table_config.init_fn(param)
 
     def _create_input_dist(
         self,
         input_feature_names: List[str],
     ) -> None:
         feature_names: List[str] = []
         for sharding in self._sharding_type_to_sharding.values():
```

## torchrec/distributed/fused_params.py

```diff
@@ -5,15 +5,15 @@
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Any, Dict, Iterable, Optional
 
 import torch
 
-from fbgemm_gpu.split_table_batched_embeddings_ops import (
+from fbgemm_gpu.split_table_batched_embeddings_ops_inference import (
     IntNBitTableBatchedEmbeddingBagsCodegen,
 )
 from torchrec.distributed.embedding_types import GroupedEmbeddingConfig
 
 FUSED_PARAM_REGISTER_TBE_BOOL: str = "__register_tbes_in_named_modules"
```

## torchrec/distributed/model_parallel.py

```diff
@@ -3,23 +3,24 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import abc
 from collections import OrderedDict
-from typing import Any, cast, Dict, Iterator, List, Optional, Tuple
+from typing import Any, cast, Dict, Iterator, List, Optional, Tuple, Type
 
 import torch
 import torch.distributed as dist
 from torch import nn
 from torch.distributed.fsdp import FullyShardedDataParallel
 from torch.nn.modules.module import _IncompatibleKeys
 from torch.nn.parallel import DistributedDataParallel
 from torchrec.distributed.comm import get_local_size
+
 from torchrec.distributed.planner import (
     EmbeddingShardingPlanner,
     sharder_name,
     Topology,
 )
 from torchrec.distributed.sharding_plan import get_default_sharders
 from torchrec.distributed.types import (
@@ -203,16 +204,17 @@
 
         if device is None:
             device = torch.device("cpu")
         self.device: torch.device = device
 
         if sharders is None:
             sharders = get_default_sharders()
-        self._sharder_map: Dict[str, ModuleSharder[nn.Module]] = {
-            sharder_name(sharder.module_type): sharder for sharder in sharders
+
+        self._sharder_map: Dict[Type[nn.Module], ModuleSharder[nn.Module]] = {
+            sharder.module_type: sharder for sharder in sharders
         }
 
         if data_parallel_wrapper is None:
             data_parallel_wrapper = DefaultDataParallelWrapper()
         self._data_parallel_wrapper: DataParallelWrapper = data_parallel_wrapper
 
         if plan is None:
@@ -321,15 +323,15 @@
         # pre-sharded module
         if isinstance(module, ShardedModule):
             return module
 
         # shardable module
         module_sharding_plan = self._plan.get_plan_for_module(path)
         if module_sharding_plan:
-            sharder_key = sharder_name(type(module))
+            sharder_key = type(module)
             module = self._sharder_map[sharder_key].shard(
                 module,
                 module_sharding_plan,
                 self._env,
                 self.device,
             )
             return module
```

## torchrec/distributed/quant_embedding.py

```diff
@@ -6,15 +6,15 @@
 # LICENSE file in the root directory of this source tree.
 
 
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Type
 
 import torch
-from fbgemm_gpu.split_table_batched_embeddings_ops import (
+from fbgemm_gpu.split_table_batched_embeddings_ops_inference import (
     IntNBitTableBatchedEmbeddingBagsCodegen,
 )
 from torch import nn
 from torchrec.distributed.embedding import (
     create_sharding_infos_by_sharding,
     EmbeddingShardingInfo,
 )
@@ -152,14 +152,15 @@
 
     def __init__(
         self,
         module: QuantEmbeddingCollection,
         table_name_to_parameter_sharding: Dict[str, ParameterSharding],
         env: ShardingEnv,
         fused_params: Optional[Dict[str, Any]] = None,
+        device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
 
         self._embedding_configs: List[EmbeddingConfig] = module.embedding_configs()
 
         sharding_type_to_sharding_infos = create_sharding_infos_by_sharding(
             module, table_name_to_parameter_sharding, fused_params
@@ -175,28 +176,31 @@
         ] = {
             sharding_type: create_infer_embedding_sharding(
                 sharding_type, embedding_confings, env
             )
             for sharding_type, embedding_confings in sharding_type_to_sharding_infos.items()
         }
 
+        self._device = device
         self._input_dists: List[nn.Module] = []
         self._lookups: List[nn.Module] = []
-        self._create_lookups(fused_params)
+        self._create_lookups(fused_params, device)
         self._output_dists: List[nn.Module] = []
 
         self._feature_splits: List[int] = []
         self._features_order: List[int] = []
 
         self._has_uninitialized_input_dist: bool = True
         self._has_uninitialized_output_dist: bool = True
 
         self._embedding_dim: int = module.embedding_dim()
         self._need_indices: bool = module.need_indices()
 
+        self._fused_params = fused_params
+
         # This provides consistency between this class and the EmbeddingBagCollection's
         # nn.Module API calls (state_dict, named_modules, etc)
         # Currently, Sharded Quant EC only uses TW sharding, and returns non-sharded tensors as part of state dict
         # TODO - revisit if we state_dict can be represented as sharded tensor
         self.embeddings: nn.ModuleDict = nn.ModuleDict()
         for table in self._embedding_configs:
             self.embeddings[table.name] = torch.nn.Module()
@@ -222,19 +226,22 @@
 
             self.tbes: torch.nn.ModuleList = torch.nn.ModuleList(tbes.keys())
 
     def _create_input_dist(
         self,
         input_feature_names: List[str],
         device: torch.device,
+        input_dist_device: Optional[torch.device] = None,
     ) -> None:
         feature_names: List[str] = []
         self._feature_splits: List[int] = []
         for sharding in self._sharding_type_to_sharding.values():
-            self._input_dists.append(sharding.create_input_dist())
+            self._input_dists.append(
+                sharding.create_input_dist(device=input_dist_device)
+            )
             feature_names.extend(sharding.feature_names())
             self._feature_splits.append(len(sharding.feature_names()))
         self._features_order: List[int] = []
         for f in feature_names:
             self._features_order.append(input_feature_names.index(f))
         self._features_order = (
             []
@@ -243,17 +250,23 @@
         )
         self.register_buffer(
             "_features_order_tensor",
             torch.tensor(self._features_order, device=device, dtype=torch.int32),
             persistent=False,
         )
 
-    def _create_lookups(self, fused_params: Optional[Dict[str, Any]]) -> None:
+    def _create_lookups(
+        self,
+        fused_params: Optional[Dict[str, Any]],
+        device: Optional[torch.device] = None,
+    ) -> None:
         for sharding in self._sharding_type_to_sharding.values():
-            self._lookups.append(sharding.create_lookup(fused_params=fused_params))
+            self._lookups.append(
+                sharding.create_lookup(fused_params=fused_params, device=device)
+            )
 
     def _create_output_dist(
         self,
         device: Optional[torch.device] = None,
     ) -> None:
         for sharding in self._sharding_type_to_sharding.values():
             self._output_dists.append(sharding.create_output_dist(device))
@@ -265,14 +278,15 @@
         ctx: EmbeddingCollectionContext,
         features: KeyedJaggedTensor,
     ) -> ListOfKJTList:
         if self._has_uninitialized_input_dist:
             self._create_input_dist(
                 input_feature_names=features.keys() if features is not None else [],
                 device=features.device(),
+                input_dist_device=self._device,
             )
             self._has_uninitialized_input_dist = False
         if self._has_uninitialized_output_dist:
             self._create_output_dist(features.device())
             self._has_uninitialized_output_dist = False
         with torch.no_grad():
             features_by_sharding = []
```

## torchrec/distributed/quant_embedding_kernel.py

```diff
@@ -8,15 +8,15 @@
 import copy
 import logging
 from typing import Any, Dict, Iterator, List, Optional, Tuple
 
 import torch
 import torch.distributed as dist
 from fbgemm_gpu.split_embedding_configs import SparseType
-from fbgemm_gpu.split_table_batched_embeddings_ops import (
+from fbgemm_gpu.split_table_batched_embeddings_ops_inference import (
     EmbeddingLocation,
     IntNBitTableBatchedEmbeddingBagsCodegen,
     PoolingMode,
     rounded_row_size_in_bytes,
 )
 from torchrec.distributed.batched_embedding_kernel import (
     BaseBatchedEmbedding,
@@ -153,15 +153,15 @@
             device=device,
             pooling_mode=self._pooling,
             feature_table_map=self._feature_table_map,
             row_alignment=16,
             uvm_host_mapped=True,  # Use cudaHostAlloc for UVM CACHING to fix imbalance numa memory issue
             **(tbe_fused_params(fused_params) or {}),
         )
-        if device is not None and device.type != "meta":
+        if device is not None:
             self._emb_module.initialize_weights()
 
     def init_parameters(self) -> None:
         pass
 
     @property
     def emb_module(
@@ -276,15 +276,15 @@
             device=device,
             pooling_mode=PoolingMode.NONE,
             feature_table_map=self._feature_table_map,
             row_alignment=16,
             uvm_host_mapped=True,  # Use cudaHostAlloc for UVM CACHING to fix imbalance numa memory issue
             **(tbe_fused_params(fused_params) or {}),
         )
-        if device is not None and device.type != "meta":
+        if device is not None:
             self._emb_module.initialize_weights()
 
     @property
     def emb_module(
         self,
     ) -> IntNBitTableBatchedEmbeddingBagsCodegen:
         return self._emb_module
```

## torchrec/distributed/quant_embeddingbag.py

```diff
@@ -4,15 +4,15 @@
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Any, Dict, List, Optional, Type
 
 import torch
-from fbgemm_gpu.split_table_batched_embeddings_ops import (
+from fbgemm_gpu.split_table_batched_embeddings_ops_inference import (
     IntNBitTableBatchedEmbeddingBagsCodegen,
 )
 from torch import nn
 from torchrec.distributed.embedding_sharding import (
     EmbeddingSharding,
     EmbeddingShardingInfo,
 )
@@ -80,14 +80,15 @@
 
     def __init__(
         self,
         module: EmbeddingBagCollectionInterface,
         table_name_to_parameter_sharding: Dict[str, ParameterSharding],
         env: ShardingEnv,
         fused_params: Optional[Dict[str, Any]] = None,
+        device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
         self._embedding_bag_configs: List[
             EmbeddingBagConfig
         ] = module.embedding_bag_configs()
         sharding_type_to_sharding_infos = create_sharding_infos_by_sharding(
             module, table_name_to_parameter_sharding, "embedding_bags.", fused_params
@@ -102,19 +103,19 @@
             ],
         ] = {
             sharding_type: create_infer_embedding_bag_sharding(
                 sharding_type, embedding_confings, env
             )
             for sharding_type, embedding_confings in sharding_type_to_sharding_infos.items()
         }
-
+        self._device = device
         self._is_weighted: bool = module.is_weighted()
         self._input_dists: List[nn.Module] = []
         self._lookups: List[nn.Module] = []
-        self._create_lookups(fused_params)
+        self._create_lookups(fused_params, device)
         self._output_dists: List[nn.Module] = []
         self._embedding_names: List[str] = []
         self._embedding_dims: List[int] = []
         self._feature_splits: List[int] = []
         self._features_order: List[int] = []
 
         # forward pass flow control
@@ -150,40 +151,47 @@
             ] = get_tbes_to_register_from_iterable(self._lookups)
 
             self.tbes: torch.nn.ModuleList = torch.nn.ModuleList(tbes.keys())
 
     def _create_input_dist(
         self,
         input_feature_names: List[str],
-        device: torch.device,
+        features_device: torch.device,
+        input_dist_device: Optional[torch.device] = None,
     ) -> None:
         feature_names: List[str] = []
         for sharding in self._sharding_type_to_sharding.values():
-            self._input_dists.append(sharding.create_input_dist())
+            self._input_dists.append(
+                sharding.create_input_dist(device=input_dist_device)
+            )
             feature_names.extend(sharding.feature_names())
             self._feature_splits.append(len(sharding.feature_names()))
 
         if feature_names == input_feature_names:
             self._has_features_permute = False
         else:
             for f in feature_names:
                 self._features_order.append(input_feature_names.index(f))
             self.register_buffer(
                 "_features_order_tensor",
-                torch.tensor(self._features_order, device=device, dtype=torch.int32),
+                torch.tensor(
+                    self._features_order, device=features_device, dtype=torch.int32
+                ),
                 persistent=False,
             )
 
     def _create_lookups(
         self,
         fused_params: Optional[Dict[str, Any]],
+        device: Optional[torch.device] = None,
     ) -> None:
         for sharding in self._sharding_type_to_sharding.values():
             self._lookups.append(
                 sharding.create_lookup(
+                    device=device,
                     fused_params=fused_params,
                 )
             )
 
     def _create_output_dist(self, device: Optional[torch.device] = None) -> None:
         for sharding in self._sharding_type_to_sharding.values():
             self._output_dists.append(sharding.create_output_dist(device))
@@ -192,15 +200,19 @@
 
     # pyre-ignore [14]
     # pyre-ignore
     def input_dist(
         self, ctx: NullShardedModuleContext, features: KeyedJaggedTensor
     ) -> ListOfKJTList:
         if self._has_uninitialized_input_dist:
-            self._create_input_dist(features.keys(), features.device())
+            self._create_input_dist(
+                features.keys(),
+                features.device(),
+                self._device,
+            )
             self._has_uninitialized_input_dist = False
         if self._has_uninitialized_output_dist:
             self._create_output_dist(features.device())
             self._has_uninitialized_output_dist = False
         with torch.no_grad():
             if self._has_features_permute:
                 features = features.permute(
```

## torchrec/distributed/sharding_plan.py

```diff
@@ -12,14 +12,17 @@
 
 import torch
 from torch import distributed as dist, nn
 from torchrec.distributed.comm import get_local_size
 from torchrec.distributed.embedding import EmbeddingCollectionSharder
 from torchrec.distributed.embedding_types import EmbeddingComputeKernel
 from torchrec.distributed.embeddingbag import EmbeddingBagCollectionSharder
+from torchrec.distributed.fp_embeddingbag import (
+    FeatureProcessedEmbeddingBagCollectionSharder,
+)
 from torchrec.distributed.fused_embeddingbag import FusedEmbeddingBagCollectionSharder
 from torchrec.distributed.quant_embedding import QuantEmbeddingCollectionSharder
 from torchrec.distributed.quant_embeddingbag import QuantEmbeddingBagCollectionSharder
 from torchrec.distributed.types import (
     EmbeddingModuleShardingPlan,
     EnumerableShardingSpec,
     ModuleSharder,
@@ -31,14 +34,15 @@
 
 MIN_CW_DIM: int = 128
 
 
 def get_default_sharders() -> List[ModuleSharder[nn.Module]]:
     return [
         cast(ModuleSharder[nn.Module], EmbeddingBagCollectionSharder()),
+        cast(ModuleSharder[nn.Module], FeatureProcessedEmbeddingBagCollectionSharder()),
         cast(ModuleSharder[nn.Module], EmbeddingCollectionSharder()),
         cast(ModuleSharder[nn.Module], FusedEmbeddingBagCollectionSharder()),
         cast(ModuleSharder[nn.Module], QuantEmbeddingBagCollectionSharder()),
         cast(ModuleSharder[nn.Module], QuantEmbeddingCollectionSharder()),
     ]
```

## torchrec/distributed/train_pipeline.py

```diff
@@ -1,37 +1,51 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+"""
+NOTE: Due to an internal packaging issue, `train_pipeline.py` must be compatible with
+older versions of TorchRec. Importing new modules from other files may break model
+publishing flows.
+"""
 import abc
+import itertools
 import logging
+from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import (
     Any,
     cast,
     Dict,
     Generic,
     Iterator,
     List,
     Optional,
     Set,
     Tuple,
     TypeVar,
+    Union,
 )
 
 import torch
+from torch import distributed as dist
 from torch.autograd.profiler import record_function
-from torch.cuda import Event
 from torch.fx.node import Node
+from torchrec.distributed.dist_data import KJTAllToAll, KJTAllToAllTensorsAwaitable
+from torchrec.distributed.embedding_sharding import (
+    KJTListAwaitable,
+    KJTListSplitsAwaitable,
+)
 from torchrec.distributed.model_parallel import DistributedModelParallel, ShardedModule
 from torchrec.distributed.types import Awaitable
 from torchrec.modules.feature_processor import BaseGroupedFeatureProcessor
+from torchrec.sparse.jagged_tensor import KeyedJaggedTensor
 from torchrec.streamable import Multistreamable, Pipelineable
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 In = TypeVar("In", bound=Pipelineable)
 Out = TypeVar("Out")
@@ -158,19 +172,196 @@
 
     def is_leaf_module(self, m: torch.nn.Module, module_qualified_name: str) -> bool:
         if isinstance(m, ShardedModule) or module_qualified_name in self._leaf_modules:
             return True
         return super().is_leaf_module(m, module_qualified_name)
 
 
+# TODO: remove after packaging issue is resolved.
+class SplitsAllToAllAwaitable(Awaitable[List[List[int]]]):
+    def __init__(
+        self,
+        input_tensors: List[torch.Tensor],
+        pg: dist.ProcessGroup,
+    ) -> None:
+        super().__init__()
+        self.num_workers: int = pg.size()
+        with record_function("## all2all_data:kjt splits ##"):
+            self._output_tensor: torch.Tensor = torch.empty(
+                [self.num_workers * len(input_tensors)],
+                device=input_tensors[0].device,
+                dtype=input_tensors[0].dtype,
+            )
+            input_tensor = torch.stack(input_tensors, dim=1).flatten()
+            self._splits_awaitable: dist.Work = dist.all_to_all_single(
+                output=self._output_tensor,
+                input=input_tensor,
+                group=pg,
+                async_op=True,
+            )
+
+    def _wait_impl(self) -> List[List[int]]:
+        self._splits_awaitable.wait()
+        return self._output_tensor.view(self.num_workers, -1).T.tolist()
+
+
+# TODO: remove after packaging issue is resolved.
+C = TypeVar("C", bound=Multistreamable)
+T = TypeVar("T")
+
+
+# TODO: remove after packaging issue is resolved.
+def _set_sharding_context(
+    tensors_awaitables: List[Awaitable[KeyedJaggedTensor]],
+    ctx: C,
+) -> None:
+    for awaitable, sharding_context in zip(
+        tensors_awaitables,
+        getattr(ctx, "sharding_contexts", []),
+    ):
+        if isinstance(awaitable, KJTAllToAllTensorsAwaitable):
+            if hasattr(sharding_context, "batch_size_per_rank"):
+                sharding_context.batch_size_per_rank = awaitable._batch_size_per_rank
+            if hasattr(sharding_context, "input_splits"):
+                sharding_context.input_splits = awaitable._input_splits["values"]
+            if hasattr(sharding_context, "output_splits"):
+                sharding_context.output_splits = awaitable._output_splits["values"]
+            if hasattr(sharding_context, "sparse_features_recat"):
+                sharding_context.sparse_features_recat = awaitable._recat
+
+
+# TODO: remove after packaging issue is resolved.
+@dataclass
+class KJTSplitsAllToAllMeta:
+    pg: dist.ProcessGroup
+    input: KeyedJaggedTensor
+    splits: List[int]
+    splits_tensors: List[torch.Tensor]
+    input_splits: List[List[int]]
+    input_tensors: List[torch.Tensor]
+    labels: List[str]
+    keys: List[str]
+    device: torch.device
+    stagger: int
+
+
+# TODO: remove after packaging issue is resolved.
+def _split(flat_list: List[T], splits: List[int]) -> List[List[T]]:
+    return [
+        flat_list[sum(splits[:i]) : sum(splits[:i]) + n] for i, n in enumerate(splits)
+    ]
+
+
+# TODO: remove after packaging issue is resolved.
+class FusedKJTListSplitsAwaitable(Awaitable[List[KJTListAwaitable]]):
+    def __init__(
+        self,
+        requests: List[KJTListSplitsAwaitable[C]],
+        contexts: List[C],
+        pg: Optional[dist.ProcessGroup],
+    ) -> None:
+        super().__init__()
+        self._contexts = contexts
+        self._awaitables: List[
+            Union[KJTSplitsAllToAllMeta, Awaitable[Awaitable[KeyedJaggedTensor]]]
+        ] = [awaitable for request in requests for awaitable in request.awaitables]
+        self._output_lengths: List[int] = [
+            len(request.awaitables) for request in requests
+        ]
+        self._lengths: List[int] = [
+            len(awaitable.splits_tensors)
+            if isinstance(awaitable, KJTSplitsAllToAllMeta)
+            else 0
+            for awaitable in self._awaitables
+        ]
+        splits_tensors = [
+            splits_tensor
+            for awaitable in self._awaitables
+            for splits_tensor in (
+                awaitable.splits_tensors
+                if isinstance(awaitable, KJTSplitsAllToAllMeta)
+                else []
+            )
+        ]
+        self._splits_awaitable: Optional[SplitsAllToAllAwaitable] = (
+            SplitsAllToAllAwaitable(
+                input_tensors=splits_tensors,
+                pg=pg,
+            )
+            if splits_tensors and pg
+            else None
+        )
+
+    def _wait_impl(self) -> List[KJTListAwaitable]:
+        if self._splits_awaitable:
+            splits_list = self._splits_awaitable.wait()
+            splits_per_awaitable = _split(splits_list, self._lengths)
+        else:
+            splits_per_awaitable = [[] for _ in range(len(self._lengths))]
+        tensors_awaitables = []
+        for splits, awaitable in zip(splits_per_awaitable, self._awaitables):
+            if not splits:  # NoWait
+                tensors_awaitables.append(awaitable.wait())
+                continue
+            output_splits = splits[:-1]
+            batch_size_per_rank = splits[-1]
+            tensors_awaitables.append(
+                KJTAllToAllTensorsAwaitable(
+                    pg=awaitable.pg,
+                    input=awaitable.input,
+                    splits=awaitable.splits,
+                    input_splits=awaitable.input_splits,
+                    output_splits=output_splits,
+                    input_tensors=awaitable.input_tensors,
+                    labels=awaitable.labels,
+                    batch_size_per_rank=batch_size_per_rank,
+                    keys=awaitable.keys,
+                    device=awaitable.device,
+                    stagger=awaitable.stagger,
+                )
+            )
+        output = []
+        awaitables_per_output = _split(tensors_awaitables, self._output_lengths)
+        for awaitables, ctx in zip(awaitables_per_output, self._contexts):
+            _set_sharding_context(awaitables, ctx)
+            output.append(KJTListAwaitable(awaitables))
+        return output
+
+
 @dataclass
 class TrainPipelineContext:
+    """
+    Context information for a `TrainPipelineSparseDist` instance.
+
+    Attributes:
+        input_dist_splits_requests (Dict[str, Awaitable[Any]]): Stores input dist
+            requests in the splits awaitable stage, which occurs after starting the
+            input dist.
+        input_dist_tensors_requests (Dict[str, Awaitable[Any]]): Stores input dist
+            requests in the tensors awaitable stage, which occurs after calling `wait()`
+            on the splits awaitable.
+        module_contexts (Dict[str, Multistreamable]): Stores module contexts from the
+            input dist for the current batch.
+        module_contexts_next_batch (Dict[str, Multistreamable]): Stores module contexts
+            from the input dist for the next batch.
+        fused_splits_awaitables (List[Tuple[List[str], FusedKJTListSplitsAwaitable]]):
+            List of fused splits input dist awaitable and the corresponding module names
+            of each awaitable.
+        feature_processor_forwards (List[Any]): List of feature processor forwards.
+    """
+
     # pyre-ignore [4]
-    input_dist_requests: Dict[str, Awaitable[Any]] = field(default_factory=dict)
+    input_dist_splits_requests: Dict[str, Awaitable[Any]] = field(default_factory=dict)
+    # pyre-ignore [4]
+    input_dist_tensors_requests: Dict[str, Awaitable[Any]] = field(default_factory=dict)
     module_contexts: Dict[str, Multistreamable] = field(default_factory=dict)
+    module_contexts_next_batch: Dict[str, Multistreamable] = field(default_factory=dict)
+    fused_splits_awaitables: List[
+        Tuple[List[str], FusedKJTListSplitsAwaitable]
+    ] = field(default_factory=list)
     # pyre-ignore [4]
     feature_processor_forwards: List[Any] = field(default_factory=list)
 
 
 @dataclass
 class ArgInfo:
     """
@@ -202,16 +393,16 @@
         self._args = args
         self._module = module
         self._context = context
         self._dist_stream = dist_stream
 
     # pyre-ignore [2, 24]
     def __call__(self, *input, **kwargs) -> Awaitable:
-        assert self._name in self._context.input_dist_requests
-        request = self._context.input_dist_requests[self._name]
+        assert self._name in self._context.input_dist_tensors_requests
+        request = self._context.input_dist_tensors_requests[self._name]
         assert isinstance(request, Awaitable)
         with record_function("## wait_sparse_data_dist ##"):
             # Finish waiting on the dist_stream,
             # in case some delayed stream scheduling happens during the wait() call.
             with torch.cuda.stream(self._dist_stream):
                 data = request.wait()
 
@@ -245,21 +436,61 @@
         return self._name
 
     @property
     def args(self) -> List[ArgInfo]:
         return self._args
 
 
+class KJTAllToAllForward:
+    def __init__(
+        self, pg: dist.ProcessGroup, splits: List[int], stagger: int = 1
+    ) -> None:
+        self._pg = pg
+        self._splits = splits
+        self._stagger = stagger
+        self._splits_cumsum: List[int] = [0] + list(itertools.accumulate(splits))
+
+    def __call__(self, input: KeyedJaggedTensor) -> KJTSplitsAllToAllMeta:
+        with torch.no_grad():
+            assert len(input.keys()) == sum(self._splits)
+            rank = dist.get_rank(self._pg)
+            local_keys = input.keys()[
+                self._splits_cumsum[rank] : self._splits_cumsum[rank + 1]
+            ]
+            input_splits = input.dist_splits(self._splits)
+            device = input.values().device
+            splits_tensors = [
+                torch.tensor(split, device=device) for split in input_splits
+            ]
+            batch_size_tensor = torch.tensor(
+                [input.stride()] * self._pg.size(), device=device
+            )
+            splits_tensors.append(batch_size_tensor)
+            return KJTSplitsAllToAllMeta(
+                pg=self._pg,
+                input=input,
+                splits=self._splits,
+                splits_tensors=splits_tensors,
+                input_splits=input_splits,
+                input_tensors=input.dist_tensors(),
+                labels=input.dist_labels(),
+                keys=local_keys,
+                device=device,
+                stagger=self._stagger,
+            )
+
+
 def _start_data_dist(
     pipelined_modules: List[ShardedModule],
     batch: In,
     context: TrainPipelineContext,
 ) -> None:
-    context.input_dist_requests.clear()
-    context.module_contexts.clear()
+    context.input_dist_splits_requests.clear()
+    context.module_contexts_next_batch.clear()
+    context.fused_splits_awaitables.clear()
     for module in pipelined_modules:
         forward = module.forward
         assert isinstance(forward, PipelinedForward)
 
         # Retrieve argument for the input_dist of EBC
         # is_getitem True means this argument could be retrieved by a list
         # False means this argument is getting while getattr
@@ -279,22 +510,48 @@
                     kwargs[arg_info.name] = arg
                 else:
                     args.append(arg)
             else:
                 args.append(None)
         # Start input distribution.
         module_ctx = module.create_context()
-        context.module_contexts[forward.name] = module_ctx
-        context.input_dist_requests[forward.name] = module.input_dist(
+        context.module_contexts_next_batch[forward.name] = module_ctx
+        context.input_dist_splits_requests[forward.name] = module.input_dist(
             module_ctx, *args, **kwargs
         )
+    _fuse_input_dist_splits(context)
 
-    # Call wait on the first awaitable in the input dist for the tensor splits
-    for key, awaitable in context.input_dist_requests.items():
-        context.input_dist_requests[key] = awaitable.wait()
+
+def _fuse_input_dist_splits(context: TrainPipelineContext) -> None:
+    names_per_pg = defaultdict(list)
+    for name, request in context.input_dist_splits_requests.items():
+        pg = None
+        if isinstance(request, KJTListSplitsAwaitable):
+            for awaitable in request.awaitables:
+                if isinstance(awaitable, KJTSplitsAllToAllMeta):
+                    pg = awaitable.pg
+                    break
+        names_per_pg[pg].append(name)
+
+    for pg, names in names_per_pg.items():
+        context.fused_splits_awaitables.append(
+            (
+                names,
+                FusedKJTListSplitsAwaitable(
+                    # pyre-ignore[6]
+                    requests=[
+                        context.input_dist_splits_requests[name] for name in names
+                    ],
+                    contexts=[
+                        context.module_contexts_next_batch[name] for name in names
+                    ],
+                    pg=pg,
+                ),
+            )
+        )
 
 
 def _get_node_args_helper(
     # pyre-ignore
     arguments,
     num_found: int,
     feature_processor_arguments: Optional[List[Node]] = None,
@@ -460,14 +717,39 @@
                     context,
                     dist_stream,
                 )
                 ret.append(child)
     return ret
 
 
+def _override_input_dist_forwards(pipelined_modules: List[ShardedModule]) -> None:
+    """
+    Overrides each input dist forward to support fusing the splits collective.
+    NOTE: this can only be called after the input dists are initialized.
+    """
+    for module in pipelined_modules:
+        for child_fqn, child_module in module.named_modules():
+            if hasattr(child_module, "_has_uninitialized_input_dist"):
+                assert (
+                    not child_module._has_uninitialized_input_dist
+                ), f"{child_fqn} has uninitialized input dist"
+
+            if not hasattr(child_module, "_input_dists"):
+                continue
+
+            for input_dist in child_module._input_dists:
+                if hasattr(input_dist, "_dist"):
+                    assert isinstance(input_dist._dist, KJTAllToAll)
+                    input_dist._dist.forward = KJTAllToAllForward(
+                        pg=input_dist._dist._pg,
+                        splits=input_dist._dist._splits,
+                        stagger=input_dist._dist._stagger,
+                    )
+
+
 class TrainPipelineSparseDist(TrainPipeline[In, Out]):
     """
     This pipeline overlaps device transfer, and `ShardedModule.input_dist()` with
     forward and backward. This helps hide the all2all latency while preserving the
     training forward / backward ordering.
 
     stage 3: forward, backward - uses default CUDA stream
@@ -521,43 +803,46 @@
     def _fill_pipeline(self, dataloader_iter: Iterator[In]) -> None:
         # pipeline is already filled
         if self._batch_i and self._batch_ip1:
             return
         # executes last batch in pipeline
         if self._batch_i and self._execute_all_batches:
             return
-        self._init_pipelined_modules()
 
         # batch 1
         self._batch_i = self._copy_batch_to_gpu(dataloader_iter)
         if self._batch_i is None:
             raise StopIteration
-        self._sparse_data_dist(self._batch_i)
+
+        self._init_pipelined_modules(self._batch_i)
+        self._start_sparse_data_dist(self._batch_i)
+        self._wait_sparse_data_dist()
 
         # batch 2
         self._batch_ip1 = self._copy_batch_to_gpu(dataloader_iter)
 
     def progress(self, dataloader_iter: Iterator[In]) -> Out:
         self._fill_pipeline(dataloader_iter)
 
         if self._model.training:
             with record_function("## zero_grad ##"):
                 self._optimizer.zero_grad()
 
-        self._batch_ip2 = self._copy_batch_to_gpu(dataloader_iter)
-
         with record_function("## wait_for_batch ##"):
             _wait_for_batch(cast(In, self._batch_i), self._data_dist_stream)
 
+        self._start_sparse_data_dist(self._batch_ip1)
+
+        self._batch_ip2 = self._copy_batch_to_gpu(dataloader_iter)
+
         # forward
         with record_function("## forward ##"):
-            event = self._record_forward_event()
             losses, output = cast(Tuple[torch.Tensor, Out], self._model(self._batch_i))
 
-        self._sparse_data_dist(self._batch_ip1, event)
+        self._wait_sparse_data_dist()
 
         if self._model.training:
             # backward
             with record_function("## backward ##"):
                 torch.sum(losses, dim=0).backward()
 
             # update
@@ -565,58 +850,64 @@
                 self._optimizer.step()
 
         self._batch_i = self._batch_ip1
         self._batch_ip1 = self._batch_ip2
 
         return output
 
-    def _init_pipelined_modules(self) -> None:
+    def _init_pipelined_modules(self, batch: In) -> None:
+        """
+        Retrieves the pipelined modules after overriding their forwards, initializes the
+        modules' input dists, and overrides the input dist forwards to support fusing
+        the splits collective in the input dist.
+        """
         if self._pipelined_modules:
             return
         self._pipelined_modules = _rewrite_model(
             self._model, self._context, self._data_dist_stream
         )
+        # initializes input dist, so we can override input dist forwards
+        self._start_sparse_data_dist(self._batch_i)
+        _override_input_dist_forwards(self._pipelined_modules)
 
     def _copy_batch_to_gpu(self, dataloader_iter: Iterator[In]) -> Optional[In]:
         """
         Retrieves batch from dataloader and moves it to the provided device.
 
-        Raises StopIteration when dataloader iterator is exhausted; unless
-        execute_all_batches=True, then returns None.
+        Raises:
+            StopIteration: if the dataloader iterator is exhausted; unless
+                `self._execute_all_batches=True`, then returns None.
         """
         with record_function("## copy_batch_to_gpu ##"):
             with torch.cuda.stream(self._memcpy_stream):
                 batch = next(dataloader_iter, None)
                 if batch is not None:
                     batch = _to_device(batch, self._device, non_blocking=True)
                 elif not self._execute_all_batches:
                     raise StopIteration
                 return batch
 
-    def _sparse_data_dist(
-        self, batch: Optional[In], event: Optional[Event] = None
-    ) -> None:
+    def _start_sparse_data_dist(self, batch: Optional[In]) -> None:
         """
-        Waits for batch to finish getting copied to GPU and forward pass to complete,
-        then starts the input distribution.
+        Waits for batch to finish getting copied to GPU, then starts the input dist.
         """
         if batch is None:
             return
-        with record_function("## sparse_data_dist ##"):
+        with record_function("## start_sparse_data_dist ##"):
             with torch.cuda.stream(self._data_dist_stream):
                 _wait_for_batch(batch, self._memcpy_stream)
-                # ensure event in default stream is called before starting data dist
-                if event is not None:
-                    # pyre-ignore[16]
-                    self._data_dist_stream.wait_event(event)
                 _start_data_dist(self._pipelined_modules, batch, self._context)
 
-    def _record_forward_event(self) -> Optional[Event]:
+    def _wait_sparse_data_dist(self) -> None:
         """
-        Creates an event in the default stream if using multiple streams (ie. CUDA),
-        before starting forward pass.
+        Waits on the input dist splits requests to get the input dist tensors requests,
+        and populates the context with them.
         """
-        return (
-            torch.cuda.current_stream().record_event()
-            if self._data_dist_stream
-            else None
-        )
+        with record_function("## wait_sparse_data_dist ##"):
+            with torch.cuda.stream(self._data_dist_stream):
+                self._context.module_contexts = (
+                    self._context.module_contexts_next_batch.copy()
+                )
+                self._context.input_dist_tensors_requests.clear()
+                for names, awaitable in self._context.fused_splits_awaitables:
+                    for name, request in zip(names, awaitable.wait()):
+                        self._context.input_dist_tensors_requests[name] = request
```

## torchrec/distributed/planner/partitioners.py

```diff
@@ -9,14 +9,15 @@
 from dataclasses import dataclass
 from typing import cast, List
 
 from torchrec.distributed.planner.types import (
     DeviceHardware,
     PartitionByType,
     Partitioner,
+    Perf,
     PlannerError,
     PlannerErrorType,
     ShardingOption,
     Storage,
     Topology,
 )
 from torchrec.distributed.types import ShardingType
@@ -24,15 +25,15 @@
 
 def _sort_devices_by_perf(
     devices: List[List[DeviceHardware]],
 ) -> List[List[DeviceHardware]]:
     def _get_perf_sum(device_list: List[DeviceHardware]) -> float:
         perf = 0
         for device in device_list:
-            perf += device.perf
+            perf += device.perf.total
         return perf
 
     return sorted(devices, key=_get_perf_sum)
 
 
 def _get_uniform_sharding_options(
     sharding_options: List[ShardingOption],
@@ -123,23 +124,23 @@
                             ]),
                 ]
             topology = Topology(world_size=2)
 
             # First [sharding_options[0] and sharding_options[1]] will be placed on the
             # topology with the uniform strategy, resulting in
 
-            topology.devices[0].perf = (1,2)
-            topology.devices[1].perf = (1,2)
+            topology.devices[0].perf.total = (1,2)
+            topology.devices[1].perf.total = (1,2)
 
             # Finally sharding_options[2] and sharding_options[3]] will be placed on the
             # topology with the device strategy (see docstring of `partition_by_device` for
             # more details).
 
-            topology.devices[0].perf = (1,2) + (3,4)
-            topology.devices[1].perf = (1,2) + (3,4)
+            topology.devices[0].perf.total = (1,2) + (3,4)
+            topology.devices[1].perf.total = (1,2) + (3,4)
 
             # The topology updates are done after the end of all the placements (the other
             # in the example is just for clarity).
         """
 
         _topology: Topology = copy.deepcopy(storage_constraint)
         # shallow copy to keep an almost sorted list around
@@ -195,31 +196,31 @@
         for shard in sharding_option.shards:
             devices.sort(
                 # We use the "local_rank" as the secondary key for sorting. This
                 # is to even out the pressure on different hosts. For example, in UVM
                 # case, we will allocate UVM table with the global rank order, and host0
                 # will use a lot more CPU memory than the others. With local rank as the
                 # secondary key, we could even out CPU memory pressure on different host
-                key=lambda device: (
-                    device.perf,
-                    device.rank % local_world_size,
-                )
+                key=lambda device: (device.perf.total, device.rank % local_world_size),
             )
             success = False
             for device in devices:
                 if cast(Storage, shard.storage).fits_in(device.storage):
                     shard.rank = device.rank
                     device.storage -= cast(Storage, shard.storage)
-                    device.perf += cast(float, shard.perf)
+                    device.perf += cast(Perf, shard.perf)
                     success = True
                     break
             if not success:
                 raise PlannerError(
                     error_type=PlannerErrorType.PARTITION,
-                    message=f"Device partition failed. Couldn't find a rank for shard {shard}, devices: {devices}",
+                    message=(
+                        f"Device partition failed. Couldn't find a rank for shard {shard} of table {sharding_option.name}, "
+                        f"largest device storage: {max(devices, key=lambda device: device.storage).storage}"
+                    ),
                 )
 
     @staticmethod
     def _cohost_partition(
         sharding_option_group: ShardingOptionGroup,
         _host_level_devices: List[List[DeviceHardware]],
     ) -> None:
@@ -296,8 +297,8 @@
                     raise PlannerError(
                         error_type=PlannerErrorType.PARTITION,
                         message=f"Shard of size {storage_needed} bytes does not fit on any rank. Device memory cap: {devices[i].storage}.",
                     )
                 else:
                     sharding_option.shards[i].rank = devices[i].rank
                     devices[i].storage -= storage_needed
-                    devices[i].perf += cast(float, sharding_option.shards[i].perf)
+                    devices[i].perf += cast(Perf, sharding_option.shards[i].perf)
```

## torchrec/distributed/planner/perf_models.py

```diff
@@ -3,22 +3,22 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import cast, List
 
-from torchrec.distributed.planner.types import PerfModel, ShardingOption, Topology
+from torchrec.distributed.planner.types import Perf, PerfModel, ShardingOption, Topology
 
 
 class NoopPerfModel(PerfModel):
     def __init__(self, topology: Topology) -> None:
         self._topology = topology
 
     def rate(self, plan: List[ShardingOption]) -> float:
         perfs = [0] * self._topology.world_size
         for sharding_option in plan:
             for shard in sharding_option.shards:
                 # pyre-ignore [6]: Expected `typing_extensions.SupportsIndex`
-                perfs[shard.rank] += cast(float, shard.perf)
+                perfs[shard.rank] += cast(Perf, shard.perf).total
 
         return max(perfs)
```

## torchrec/distributed/planner/planners.py

```diff
@@ -196,14 +196,15 @@
     ) -> ShardingPlan:
 
         self._num_proposals = 0
         self._num_plans = 0
         start_time = perf_counter()
         best_plan = None
         lowest_storage = Storage(MAX_SIZE, MAX_SIZE)
+        last_planner_error: Optional[PlannerError] = None
         best_perf_rating = MAX_SIZE
 
         storage_constraint: Topology = self._storage_reservation.reserve(
             topology=self._topology,
             batch_size=self._batch_size,
             module=module,
             sharders=sharders,
@@ -253,15 +254,16 @@
                     if perf_rating < best_perf_rating:
                         best_perf_rating = perf_rating
                         best_plan = copy.deepcopy(plan)
                     proposal_cache[proposal_key] = (True, plan, perf_rating)
                     proposer.feedback(
                         partitionable=True, plan=plan, perf_rating=perf_rating
                     )
-                except PlannerError:
+                except PlannerError as planner_error:
+                    last_planner_error = planner_error
                     current_storage = cast(
                         Storage,
                         reduce(
                             lambda x, y: x + y,
                             [
                                 shard.storage
                                 for option in proposal
@@ -302,30 +304,44 @@
                 lambda x, y: x + y,
                 [device.storage for device in self._topology.devices],
             )
             global_storage_constraints = reduce(
                 lambda x, y: x + y,
                 [device.storage for device in storage_constraint.devices],
             )
+            storage_reservation_solution = (
+                (
+                    f"\n\t  Storage reservation percentage: {self._storage_reservation._percentage}, "
+                    f"\n\t  Storage reservation dense storage: {self._storage_reservation._dense_storage}, "
+                    f"\n\t  Storage reservation kjt storage: {self._storage_reservation._kjt_storage}, "
+                )
+                if isinstance(self._storage_reservation, HeuristicalStorageReservation)
+                else f"\n\t  Storage reservation percentage: {self._storage_reservation._percentage}, "  # pyre-ignore[16]
+            )
             no_plan_solution = (
                 f"Planner evaluated {self._num_proposals} proposals."
                 "\nPossible solutions:"
                 f"\n  1) Increase the number of devices ({self._topology.world_size})"
                 f"\n  2) Reduce the model size ("
                 f"\n\t  Global storage: {global_storage_capacity.hbm}, "
-                f"\n\t  Available for model parallel: {global_storage_constraints},"
+                f"\n\t  Hardware memory: {self._topology.devices[0].storage}, "
+                f"{storage_reservation_solution}"
+                f"\n\t  Available for model parallel: {global_storage_constraints}, "
                 f"\n\t  Requirement for model parallel: {lowest_storage})"
                 f"\n  3) Reduce local batch size ({self._batch_size})"
                 "\n  4) Remove planner constraints that might be reducing search space or available storage\n"
             )
+            last_planner_error_info = f"Last planner error: \n\t{last_planner_error}\n"
             if not lowest_storage.fits_in(global_storage_constraints):
                 raise PlannerError(
                     error_type=PlannerErrorType.INSUFFICIENT_STORAGE,
                     message="Unable to find a plan for this model because of insufficient storage. \n"
-                    + no_plan_solution,
+                    + no_plan_solution
+                    + last_planner_error_info,
                 )
             else:
                 raise PlannerError(
                     error_type=PlannerErrorType.STRICT_CONSTRAINTS,
                     message="Unable to find a plan for this model because of the strict constraints. \n"
-                    + no_plan_solution,
+                    + no_plan_solution
+                    + last_planner_error_info,
                 )
```

## torchrec/distributed/planner/proposers.py

```diff
@@ -6,15 +6,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import itertools
 import logging
 from decimal import Decimal
 from typing import cast, Dict, List, Optional, Set, Tuple
 
-from torchrec.distributed.planner.types import Proposer, ShardingOption
+from torchrec.distributed.planner.types import Perf, Proposer, ShardingOption
 from torchrec.distributed.planner.utils import prod
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 MAX_PROPOSALS: int = int(1e4)
 
 
@@ -24,15 +24,16 @@
 
     Sorts sharding options for each shardable parameter by perf.
     On each iteration, finds parameter with largest current storage usage and tries its
     next sharding option.
 
     Args:
         use_depth (bool): When enabled, sharding_options of a fqn are sorted based on
-            `max(shard.perf)`, otherwise sharding_options are sorted by `sum(shard.perf)`.
+            `max(shard.perf.total)`, otherwise sharding_options are sorted by
+            `sum(shard.perf.total)`.
         threshold (Optional[int]): Threshold for early stopping. When specified, the
             proposer stops proposing when the proposals have consecutive worse perf_rating
             than best_perf_rating.
     """
 
     def __init__(self, use_depth: bool = True, threshold: Optional[int] = None) -> None:
         self._use_depth: bool = use_depth
@@ -248,17 +249,17 @@
         self._proposal_index += 1
 
 
 def _sharding_option_score(
     sharding_option: ShardingOption, use_depth: bool = True
 ) -> float:
     return (
-        max([cast(float, shard.perf) for shard in sharding_option.shards])
+        max([cast(Perf, shard.perf).total for shard in sharding_option.shards])
         if use_depth
-        else sum([cast(float, shard.perf) for shard in sharding_option.shards])
+        else sum([cast(Perf, shard.perf).total for shard in sharding_option.shards])
     )
 
 
 def proposers_to_proposals_list(
     proposers_list: List[Proposer], search_space: List[ShardingOption]
 ) -> List[List[ShardingOption]]:
     """
```

## torchrec/distributed/planner/shard_estimators.py

```diff
@@ -22,14 +22,15 @@
     kernel_bw_lookup,
     QUARTER_BLOCK_PENALTY,
     UVM_CACHING_RATIO,
     WEIGHTED_KERNEL_MULTIPLIER,
 )
 from torchrec.distributed.planner.types import (
     ParameterConstraints,
+    Perf,
     PlannerError,
     ShardEstimator,
     ShardingOption,
     Storage,
     Topology,
 )
 from torchrec.distributed.planner.utils import prod, sharder_name
@@ -169,15 +170,15 @@
     intra_host_bw: float,
     inter_host_bw: float,
     is_pooled: bool,
     is_weighted: bool = False,
     has_feature_processor: bool = False,
     caching_ratio: Optional[float] = None,
     is_inference: bool = False,
-) -> List[float]:
+) -> List[Perf]:
     """
     Attempts to model perfs as a function of relative wall times.
 
     Args:
         shard_sizes (List[List[int]]): the list of (local_rows, local_cols) of each
             shard.
         compute_kernel (str): compute kernel.
@@ -329,15 +330,15 @@
     device_bw: float,
     inter_host_bw: float,
     intra_host_bw: float,
     is_pooled: bool,
     is_weighted: bool = False,
     is_inference: bool = False,
     has_feature_processor: bool = False,
-) -> float:
+) -> Perf:
     batch_inputs = sum(
         [x * y * z for x, y, z in zip(input_lengths, num_poolings, batch_sizes)]
     )
     batch_outputs = (
         sum([x * y for x, y in zip(num_poolings, batch_sizes)])
         if is_pooled
         else batch_inputs
@@ -373,35 +374,36 @@
     fwd_compute = (
         (input_read_size + embedding_lookup_size + fwd_output_write_size)
         * block_usage_penalty
         / device_bw
     )
     if is_inference:
         # only consider forward compute and comms for inference
-        return fwd_compute + fwd_comms
+        return Perf(
+            fwd_compute=fwd_compute, fwd_comms=fwd_comms, bwd_compute=0, bwd_comms=0
+        )
 
     bwd_comms = bwd_output_write_size / comms_bw
 
     bwd_grad_indice_weights_kernel = (
         fwd_compute * WEIGHTED_KERNEL_MULTIPLIER
         if is_weighted or has_feature_processor
         else 0
     )
 
     # includes fused optimizers
     bwd_compute = fwd_compute * BWD_COMPUTE_MULTIPLIER
 
     # in order of model parallel execution, starting with:
     # BWD DP -> BWD MP ... FWD MP -> FWD DP
-    return (
-        bwd_comms
-        + bwd_grad_indice_weights_kernel
-        + bwd_compute
-        + fwd_compute
-        + fwd_comms
+    return Perf(
+        fwd_compute=fwd_compute,
+        fwd_comms=fwd_comms,
+        bwd_compute=bwd_compute + bwd_grad_indice_weights_kernel,
+        bwd_comms=bwd_comms,
     )
 
 
 def _get_rw_sharding_perf(
     batch_sizes: List[int],
     world_size: int,
     local_world_size: int,
@@ -416,15 +418,15 @@
     num_poolings: List[float],
     device_bw: float,
     inter_host_bw: float,
     intra_host_bw: float,
     is_pooled: bool,
     is_weighted: bool = False,
     has_feature_processor: bool = False,
-) -> float:
+) -> Perf:
     batch_inputs = (
         sum([x * y * z for x, y, z in zip(input_lengths, num_poolings, batch_sizes)])
         / world_size
     )
     batch_outputs = (
         sum([x * y for x, y in zip(num_poolings, batch_sizes)])
         if is_pooled
@@ -463,21 +465,19 @@
         fwd_compute * WEIGHTED_KERNEL_MULTIPLIER
         if is_weighted or has_feature_processor
         else 0
     )
 
     bwd_compute = fwd_compute * BWD_COMPUTE_MULTIPLIER
 
-    return (
-        bwd_comms
-        + bwd_batched_copy
-        + bwd_grad_indice_weights_kernel
-        + bwd_compute
-        + fwd_compute
-        + fwd_comms
+    return Perf(
+        fwd_compute=fwd_compute,
+        fwd_comms=fwd_comms,
+        bwd_compute=bwd_compute + bwd_grad_indice_weights_kernel,
+        bwd_comms=bwd_comms + bwd_batched_copy,
     )
 
 
 def _get_twrw_sharding_perf(
     batch_sizes: List[int],
     world_size: int,
     local_world_size: int,
@@ -492,15 +492,15 @@
     num_poolings: List[float],
     device_bw: float,
     inter_host_bw: float,
     intra_host_bw: float,
     is_pooled: bool,
     is_weighted: bool = False,
     has_feature_processor: bool = False,
-) -> float:
+) -> Perf:
     batch_inputs = (
         sum([x * y * z for x, y, z in zip(input_lengths, num_poolings, batch_sizes)])
         / local_world_size
     )
     batch_outputs = (
         sum([x * y for x, y in zip(num_poolings, batch_sizes)])
         if is_pooled
@@ -546,21 +546,19 @@
         else 0
     )
 
     bwd_batched_copy = bwd_output_write_size * BATCHED_COPY_PERF_FACTOR / device_bw
 
     bwd_compute = fwd_compute * BWD_COMPUTE_MULTIPLIER
 
-    return (
-        bwd_comms
-        + bwd_batched_copy
-        + bwd_grad_indice_weights_kernel
-        + bwd_compute
-        + fwd_compute
-        + fwd_comms
+    return Perf(
+        fwd_compute=fwd_compute,
+        fwd_comms=fwd_comms,
+        bwd_compute=bwd_compute + bwd_grad_indice_weights_kernel,
+        bwd_comms=bwd_comms + bwd_batched_copy,
     )
 
 
 def _get_dp_sharding_perf(
     batch_sizes: List[int],
     world_size: int,
     local_world_size: int,
@@ -571,15 +569,15 @@
     table_data_type_size: float,
     num_poolings: List[float],
     device_bw: float,
     inter_host_bw: float,
     is_pooled: bool,
     is_weighted: bool = False,
     has_feature_processor: bool = False,
-) -> float:
+) -> Perf:
     batch_inputs = sum(
         [x * y * z for x, y, z in zip(input_lengths, num_poolings, batch_sizes)]
     )
     batch_outputs = (
         sum([x * y for x, y in zip(num_poolings, batch_sizes)])
         if is_pooled
         else batch_inputs
@@ -618,20 +616,19 @@
 
     bwd_grad_indice_weights_kernel = (
         fwd_compute * WEIGHTED_KERNEL_MULTIPLIER
         if is_weighted or has_feature_processor
         else 0
     )
 
-    return (
-        all_reduce
-        + optimizer_kernels
-        + bwd_grad_indice_weights_kernel
-        + bwd_compute
-        + fwd_compute
+    return Perf(
+        fwd_compute=fwd_compute,
+        fwd_comms=0,
+        bwd_compute=bwd_compute + bwd_grad_indice_weights_kernel,
+        bwd_comms=all_reduce + optimizer_kernels,
     )
 
 
 def _extract_comm_data_type_size(
     sharder: ModuleSharder[nn.Module], sharding_option: ShardingOption
 ) -> Tuple[float, float, float, float]:
     table_data_type_size = sharding_option.tensor.element_size()
```

## torchrec/distributed/planner/stats.py

```diff
@@ -14,14 +14,15 @@
 from torchrec.distributed.planner.storage_reservations import (
     FixedPercentageStorageReservation,
     HeuristicalStorageReservation,
     InferenceStorageReservation,
 )
 from torchrec.distributed.planner.types import (
     ParameterConstraints,
+    Perf,
     ShardingOption,
     Stats,
     Storage,
     StorageReservation,
     Topology,
 )
 from torchrec.distributed.planner.utils import bytes_to_gb, bytes_to_mb
@@ -146,22 +147,25 @@
                 count = stats[rank]["type"].get(sharding_type_abbr, 0)
                 stats[rank]["type"][sharding_type_abbr] = count + 1
                 stats[rank]["input_sizes"] += input_sizes[i]
                 stats[rank]["output_sizes"] += output_sizes[i]
 
         used_hbm = [0] * topology.world_size
         used_ddr = [0] * topology.world_size
-        perf = [0.0] * topology.world_size
+        perf = [
+            Perf(fwd_compute=0, fwd_comms=0, bwd_compute=0, bwd_comms=0)
+            for _ in range(topology.world_size)
+        ]
         for sharding_option in best_plan:
             for shard in sharding_option.shards:
                 shard_storage = cast(Storage, shard.storage)
                 rank = cast(int, shard.rank)
                 used_hbm[rank] += shard_storage.hbm
                 used_ddr[rank] += shard_storage.ddr
-                perf[rank] += cast(float, shard.perf)
+                perf[rank] += cast(Perf, shard.perf)
 
         used_hbm = [hbm + dense_storage.hbm + kjt_storage.hbm for hbm in used_hbm]
         used_ddr = [ddr + dense_storage.ddr + kjt_storage.ddr for ddr in used_ddr]
 
         table: List[List[Union[str, int]]] = [
             [
                 "Rank",
@@ -196,15 +200,15 @@
             )
             for sharding_type in used_sharding_types:
                 if sharding_type not in stats[rank]["type"]:
                     stats[rank]["type"][sharding_type] = 0
 
             rank_hbm = f"{round(used_hbm_gb, 1)} ({used_hbm_ratio:.0%})"
             rank_ddr = f"{round(used_ddr_gb, 1)} ({used_ddr_ratio:.0%})"
-            rank_perf = f"{round(perf[rank], 3)}"
+            rank_perf = _format_perf_breakdown(perf[rank])
             rank_input = f"{round(stats[rank]['input_sizes'], 2)}"
             rank_output = f"{round(stats[rank]['output_sizes'], 2)}"
             rank_shards = " ".join(
                 f"{sharding_type}: {num_tables}"
                 for sharding_type, num_tables in sorted(stats[rank]["type"].items())
             )
             table.append(
@@ -258,17 +262,21 @@
             ]
             if include_batch_sizes := any(feat_batch_sizes):
                 param_table[0].append("Batch Sizes")
                 param_table[1].append("-------------")
             for i, so in enumerate(best_plan):
                 ranks = sorted([cast(int, shard.rank) for shard in so.shards])
                 ranks = _collapse_consecutive_ranks(ranks)
-                shard_perfs = str(
-                    round(sum([cast(float, shard.perf) for shard in so.shards]), 3)
-                )
+
+                so_perf = Perf(fwd_compute=0, fwd_comms=0, bwd_compute=0, bwd_comms=0)
+                for shard in so.shards:
+                    so_perf += cast(Perf, shard.perf)
+
+                shard_perfs = _format_perf_breakdown(so_perf)
+
                 pooling_factor = str(round(sum(so.input_lengths), 3))
                 num_poolings = (
                     cast(List[float], constraints[so.name].num_poolings)
                     if constraints
                     and constraints.get(so.name)
                     and constraints[so.name].num_poolings
                     else [NUM_POOLINGS] * len(so.input_lengths)
@@ -313,17 +321,19 @@
 
         divider = "-" * (self._width - 4)
         self._stats_table.append(f"#{divider: ^{self._width-2}}#")
 
         for row in formatted_table:
             self._stats_table.append(f"# {row: <{self._width-3}}#")
 
+        perf_breakdown = "Perf: Total perf (Forward compute, Forward comms, Backward compute, Backward comms)"
         legend = "Input: MB/iteration, Output: MB/iteration, Shards: number of tables"
         hbm_info = "HBM: estimated peak memory usage for shards, dense tensors, and features (KJT)"
         self._stats_table.append(f"#{'' : ^{self._width-2}}#")
+        self._stats_table.append(f"# {perf_breakdown: <{self._width-3}}#")
         self._stats_table.append(f"# {legend: <{self._width-3}}#")
         self._stats_table.append(f"# {hbm_info: <{self._width-3}}#")
 
         if debug:
             self._stats_table.append(f"#{'' : ^{self._width-2}}#")
             self._stats_table.append(f"# {'Parameter Info:' : <{self._width-3}}#")
             for row in formatted_param_table:
@@ -403,25 +413,37 @@
         )
 
         input_sizes = [bytes_to_mb(input_size) for input_size in input_sizes]
         output_sizes = [bytes_to_mb(output_size) for output_size in output_sizes]
 
         return ranks, input_sizes, output_sizes
 
-    def _log_max_perf_and_max_hbm(self, perf: List[float], used_hbm: List[int]) -> None:
-        max_perf = max(perf)
-        max_perf_indices = [i for i in range(len(perf)) if perf[i] == max_perf]
-        rank_text = "ranks" if len(max_perf_indices) > 1 else "rank"
-        max_perf_indices = _collapse_consecutive_ranks(max_perf_indices)
-        max_perf_ranks = f"{rank_text} {','.join(max_perf_indices)}"
-        longest_critical_path = (
-            f"Longest Critical Path: {round(max_perf, 3)} ms on {max_perf_ranks}"
+    def _log_max_perf_and_max_hbm(self, perfs: List[Perf], used_hbm: List[int]) -> None:
+
+        max_total_perf_text = f"Longest Critical Path (Maximum of Total Perf): {_generate_max_text([perf.total for perf in perfs])}"
+        max_fwd_compute_perf_text = f"Maximum of Forward Compute: {_generate_max_text([perf.fwd_compute for perf in perfs])}"
+        max_fwd_comms_perf_text = f"Maximum of Forward Comms: {_generate_max_text([perf.fwd_comms for perf in perfs])}"
+        max_bwd_compute_perf_text = f"Maximum of Backward Compute: {_generate_max_text([perf.bwd_compute for perf in perfs])}"
+        max_bwd_comms_perf_text = f"Maximum of Backward Comms: {_generate_max_text([perf.bwd_comms for perf in perfs])}"
+
+        sum_of_maxima = (
+            max(perf.fwd_compute for perf in perfs)
+            + max(perf.fwd_comms for perf in perfs)
+            + max(perf.bwd_compute for perf in perfs)
+            + max(perf.bwd_comms for perf in perfs)
         )
+        sum_of_maxima_text = f"Sum of Maxima: {round(sum_of_maxima, 3)} ms"
+
         self._stats_table.append(f"#{'' : ^{self._width-2}}#")
-        self._stats_table.append(f"# {longest_critical_path : <{self._width-3}}#")
+        self._stats_table.append(f"# {max_total_perf_text : <{self._width-3}}#")
+        self._stats_table.append(f"# {max_fwd_compute_perf_text : <{self._width-3}}#")
+        self._stats_table.append(f"# {max_fwd_comms_perf_text : <{self._width-3}}#")
+        self._stats_table.append(f"# {max_bwd_compute_perf_text : <{self._width-3}}#")
+        self._stats_table.append(f"# {max_bwd_comms_perf_text : <{self._width-3}}#")
+        self._stats_table.append(f"# {sum_of_maxima_text : <{self._width-3}}#")
 
         max_hbm = max(used_hbm)
         max_hbm_indices = [i for i in range(len(used_hbm)) if used_hbm[i] == max_hbm]
         rank_text = "ranks" if len(max_hbm_indices) > 1 else "rank"
         max_hbm_indices = _collapse_consecutive_ranks(max_hbm_indices)
         max_hbm_ranks = f"{rank_text} {','.join(max_hbm_indices)}"
         peak_memory_pressure = f"Peak Memory Pressure: {round(bytes_to_gb(max_hbm), 3)} GB on {max_hbm_ranks}"
@@ -478,14 +500,25 @@
         ]
         self._stats_table.append(f"#{'' : ^{self._width-2}}#")
         self._stats_table.append(f"# {'Compute Kernels:' : <{self._width-3}}#")
         for compute_kernel_count in compute_kernels_count:
             self._stats_table.append(f"#    {compute_kernel_count : <{self._width-6}}#")
 
 
+def _generate_max_text(perfs: List[float]) -> str:
+    max_perf = max(perfs)
+
+    max_perf_indices = [i for i in range(len(perfs)) if perfs[i] == max_perf]
+    rank_text = "ranks" if len(max_perf_indices) > 1 else "rank"
+    max_perf_indices = _collapse_consecutive_ranks(max_perf_indices)
+    max_perf_ranks = f"{rank_text} {','.join(max_perf_indices)}"
+
+    return f"{round(max_perf, 3)} ms on {max_perf_ranks}"
+
+
 def _get_sharding_type_abbr(sharding_type: str) -> str:
     if sharding_type == ShardingType.DATA_PARALLEL.value:
         return "DP"
     elif sharding_type == ShardingType.TABLE_WISE.value:
         return "TW"
     elif sharding_type == ShardingType.COLUMN_WISE.value:
         return "CW"
@@ -497,14 +530,32 @@
         return "TWCW"
     else:
         raise ValueError(
             f"Unrecognized or unsupported sharding type provided: {sharding_type}"
         )
 
 
+def _format_perf_breakdown(perf: Perf) -> str:
+    breakdown = [
+        perf.fwd_compute,
+        perf.fwd_comms,
+        perf.bwd_compute,
+        perf.bwd_comms,
+    ]
+    breakdown_string = ",".join(
+        [str(round(num)) if num >= 1 else round_to_one_sigfig(num) for num in breakdown]
+    )
+
+    return f"{str(round(perf.total, 3))} ({breakdown_string})"
+
+
+def round_to_one_sigfig(x: float) -> str:
+    return f'{float(f"{x:.1g}"):g}'
+
+
 def _format_table(table: List[List[Union[str, int]]]) -> List[str]:
     longest_cols = [
         (max([len(str(row[i])) for row in table]) + 3) for i in range(len(table[0]))
     ]
     row_format = "".join(
         ["{:>" + str(longest_col) + "}" for longest_col in longest_cols]
     )
```

## torchrec/distributed/planner/types.py

```diff
@@ -22,14 +22,52 @@
     HBM_MEM_BW,
     INTRA_NODE_BANDWIDTH,
     POOLING_FACTOR,
 )
 from torchrec.distributed.types import ModuleSharder, ShardingPlan
 from torchrec.modules.embedding_modules import EmbeddingCollectionInterface
 
+# ---- Perf ---- #
+
+
+@dataclass(repr=True, eq=True)
+class Perf:
+    """
+    Representation of the breakdown of the perf estimate a single shard of an
+    embedding table.
+    """
+
+    fwd_compute: float
+    fwd_comms: float
+    bwd_compute: float
+    bwd_comms: float
+
+    @property
+    def total(self) -> float:
+        return self.fwd_compute + self.bwd_compute + self.fwd_comms + self.bwd_comms
+
+    def __add__(self, other: "Perf") -> "Perf":
+        return Perf(
+            fwd_compute=self.fwd_compute + other.fwd_compute,
+            fwd_comms=self.fwd_comms + other.fwd_comms,
+            bwd_compute=self.bwd_compute + other.bwd_compute,
+            bwd_comms=self.bwd_comms + other.bwd_comms,
+        )
+
+    def __hash__(self) -> int:
+        return hash(
+            (
+                self.fwd_compute,
+                self.fwd_comms,
+                self.bwd_compute,
+                self.bwd_comms,
+            )
+        )
+
+
 # ---- TOPOLOGY ---- #
 
 
 @dataclass(repr=True, order=True, eq=True)
 class Storage:
     """
     Representation of the storage capacities of a hardware used in training.
@@ -62,15 +100,15 @@
     """
     Representation of a device in a process group. 'perf' is an estimation of network,
     CPU, and storage usages.
     """
 
     rank: int
     storage: Storage
-    perf: float = 0
+    perf: Perf
 
 
 class Topology:
     def __init__(
         self,
         world_size: int,
         compute_device: str,
@@ -101,14 +139,15 @@
 
         self._devices: List[DeviceHardware] = []
         for rank in range(world_size):
             self._devices.append(
                 DeviceHardware(
                     rank=rank,
                     storage=Storage(hbm=hbm_per_device, ddr=ddr_cap),
+                    perf=Perf(fwd_compute=0, fwd_comms=0, bwd_compute=0, bwd_comms=0),
                 )
             )
 
         self._local_world_size: int = (
             local_world_size if local_world_size else world_size
         )
         self._hbm_mem_bw = hbm_mem_bw
@@ -170,15 +209,15 @@
     determine the tensors in the shard. 'storage' is an estimation of how much it takes
     to store the shard with an estimation 'perf'.
     """
 
     size: List[int]
     offset: List[int]
     storage: Optional[Storage] = None
-    perf: Optional[float] = None
+    perf: Optional[Perf] = None
     rank: Optional[int] = None
 
     def __hash__(self) -> int:
         return hash(
             (
                 tuple(self.size),
                 tuple(self.offset),
```

## torchrec/distributed/sharding/dp_sharding.py

```diff
@@ -198,14 +198,17 @@
         feature_processor: Optional[BaseGroupedFeatureProcessor] = None,
     ) -> BaseEmbeddingLookup:
         return GroupedPooledEmbeddingsLookup(
             grouped_configs=self._grouped_embedding_configs,
             pg=self._env.process_group,
             device=device if device is not None else self._device,
             feature_processor=feature_processor,
+            # For data parallel we need to turn always gradient scaling in for weights
+            # because get_gradient_scaling from comm_ops only affects model_parallel tables, not DP
+            scale_weight_gradients=False,
         )
 
     def create_output_dist(
         self,
         device: Optional[torch.device] = None,
     ) -> BaseEmbeddingDist[EmbeddingShardingContext, torch.Tensor, torch.Tensor]:
         return DpPooledEmbeddingDist()
```

## torchrec/distributed/sharding/tw_sequence_sharding.py

```diff
@@ -200,28 +200,30 @@
     placed entirely on a selected rank, for inference.
     """
 
     def create_input_dist(
         self, device: Optional[torch.device] = None
     ) -> BaseSparseFeaturesDist[KJTList]:
         return InferTwSparseFeaturesDist(
-            self.features_per_rank(),
-            self._world_size,
+            features_per_rank=self.features_per_rank(),
+            world_size=self._world_size,
+            device=device,
         )
 
     def create_lookup(
         self,
         device: Optional[torch.device] = None,
         fused_params: Optional[Dict[str, Any]] = None,
         feature_processor: Optional[BaseGroupedFeatureProcessor] = None,
     ) -> BaseEmbeddingLookup[KJTList, List[torch.Tensor]]:
         return InferGroupedEmbeddingsLookup(
             grouped_configs_per_rank=self._grouped_embedding_configs_per_rank,
             world_size=self._world_size,
             fused_params=fused_params,
+            device=device,
         )
 
     def create_output_dist(
         self,
         device: Optional[torch.device] = None,
     ) -> BaseEmbeddingDist[
         InferSequenceShardingContext, List[torch.Tensor], List[torch.Tensor]
```

## torchrec/distributed/sharding/tw_sharding.py

```diff
@@ -352,25 +352,28 @@
 class InferTwSparseFeaturesDist(BaseSparseFeaturesDist[KJTList]):
     """
     Redistributes sparse features to all devices for inference.
 
     Args:
         features_per_rank (List[int]): number of features to send to each rank.
         world_size (int): number of devices in the topology.
+        fused_params (Dict[str, Any]): fused parameters of the model.
     """
 
     def __init__(
         self,
         features_per_rank: List[int],
         world_size: int,
+        device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
         self._dist = KJTOneToAll(
-            features_per_rank,
-            world_size,
+            splits=features_per_rank,
+            world_size=world_size,
+            device=device,
         )
 
     def forward(
         self,
         sparse_features: KeyedJaggedTensor,
     ) -> KJTList:
         """
@@ -429,31 +432,34 @@
     ]
 ):
     """
     Shards embedding bags table-wise for inference
     """
 
     def create_input_dist(
-        self, device: Optional[torch.device] = None
+        self,
+        device: Optional[torch.device] = None,
     ) -> BaseSparseFeaturesDist[KJTList]:
         return InferTwSparseFeaturesDist(
-            self.features_per_rank(),
-            self._world_size,
+            features_per_rank=self.features_per_rank(),
+            world_size=self._world_size,
+            device=device,
         )
 
     def create_lookup(
         self,
         device: Optional[torch.device] = None,
         fused_params: Optional[Dict[str, Any]] = None,
         feature_processor: Optional[BaseGroupedFeatureProcessor] = None,
     ) -> BaseEmbeddingLookup[KJTList, List[torch.Tensor]]:
         return InferGroupedPooledEmbeddingsLookup(
             grouped_configs_per_rank=self._grouped_embedding_configs_per_rank,
             world_size=self._world_size,
             fused_params=fused_params,
+            device=device,
         )
 
     def create_output_dist(
         self,
         device: Optional[torch.device] = None,
     ) -> BaseEmbeddingDist[NullShardingContext, List[torch.Tensor], torch.Tensor]:
         device = device if device is not None else self._device
```

## torchrec/distributed/test_utils/infer_utils.py

```diff
@@ -204,19 +204,24 @@
         )
         fused_params[FUSED_PARAM_REGISTER_TBE_BOOL] = True
         return ShardedQuantEmbeddingBagCollection(
             module=module,
             table_name_to_parameter_sharding=params,
             env=env,
             fused_params=fused_params,
+            device=device,
         )
 
 
 class TestQuantECSharder(QuantEmbeddingCollectionSharder):
-    def __init__(self, sharding_type: str, kernel_type: str) -> None:
+    def __init__(
+        self,
+        sharding_type: str,
+        kernel_type: str,
+    ) -> None:
         super().__init__()
         self._sharding_type = sharding_type
         self._kernel_type = kernel_type
 
     def sharding_types(self, compute_device_type: str) -> List[str]:
         return [self._sharding_type]
 
@@ -233,15 +238,17 @@
         device: Optional[torch.device] = None,
     ) -> ShardedQuantEmbeddingCollection:
         fused_params = self.fused_params if self.fused_params else {}
         fused_params["output_dtype"] = data_type_to_sparse_type(
             dtype_to_data_type(module.output_dtype())
         )
         fused_params[FUSED_PARAM_REGISTER_TBE_BOOL] = True
-        return ShardedQuantEmbeddingCollection(module, params, env, fused_params)
+        return ShardedQuantEmbeddingCollection(
+            module, params, env, fused_params, device
+        )
 
 
 class KJTInputWrapper(torch.nn.Module):
     def __init__(
         self,
         module_kjt_input: torch.nn.Module,
     ) -> None:
```

## torchrec/metrics/auc.py

```diff
@@ -25,15 +25,15 @@
 GROUPING_KEYS = "grouping_keys"
 REQUIRED_INPUTS = "required_inputs"
 
 
 def _compute_auc_helper(
     predictions: torch.Tensor, labels: torch.Tensor, weights: torch.Tensor
 ) -> torch.Tensor:
-    _, sorted_indices = torch.sort(predictions, descending=True, dim=-1)
+    sorted_indices = torch.argsort(predictions, descending=True, dim=-1)
     sorted_labels = torch.index_select(labels, dim=0, index=sorted_indices)
     sorted_weights = torch.index_select(weights, dim=0, index=sorted_indices)
     cum_fp = torch.cumsum(sorted_weights * (1.0 - sorted_labels), dim=0)
     cum_tp = torch.cumsum(sorted_weights * sorted_labels, dim=0)
     auc = torch.where(
         cum_fp[-1] * cum_tp[-1] == 0,
         0.5,  # 0.5 is the no-signal default value for auc.
@@ -50,17 +50,14 @@
 
     Args:
         n_tasks (int): number of tasks.
         predictions (torch.Tensor): tensor of size (n_tasks, n_examples).
         labels (torch.Tensor): tensor of size (n_tasks, n_examples).
         weights (torch.Tensor): tensor of size (n_tasks, n_examples).
     """
-    # The return values are sorted_predictions, sorted_index but only
-    # sorted_predictions is needed.
-    _, sorted_indices = torch.sort(predictions, descending=True, dim=-1)
     aucs = []
     for predictions_i, labels_i, weights_i in zip(predictions, labels, weights):
         auc = _compute_auc_helper(predictions_i, labels_i, weights_i)
         aucs.append(auc.view(1))
     return torch.cat(aucs)
```

## torchrec/metrics/metrics_config.py

```diff
@@ -75,15 +75,16 @@
     Args:
         rec_tasks (List[RecTaskInfo]): this and next fields specify the RecTask
             information. ``rec_tasks`` specifies the RecTask information while
             ``rec_task_indices`` represents the indices that point to the
             RecTask information stored in the parent ``MetricsConfig``. Only one
             of the two fields should be specified.
         rec_task_indices (List[int]): see the doscstring of ``rec_tasks``.
-        window_size (int): the window size for this metric.
+        window_size (int): the window size for this metric. Note that this is global window size.
+            The local window size is window_size / world_size, and must be larger than batch size.
         arguments (Optional[Dict[str, Any]]): any propritary arguments to be used
             by this Metric.
     """
 
     rec_tasks: List[RecTaskInfo] = field(default_factory=list)
     rec_task_indices: List[int] = field(default_factory=list)
     window_size: int = _DEFAULT_WINDOW_SIZE
```

## torchrec/metrics/rec_metric.py

```diff
@@ -245,14 +245,25 @@
                 return self._compute()
             else:
                 return []
 
     def local_compute(self) -> List[MetricComputationReport]:
         return self._compute()
 
+    def reset(self) -> None:
+        super().reset()
+        if self._batch_window_buffers is not None:
+            self._batch_window_buffers = {
+                name: WindowBuffer(
+                    max_size=self._window_size,
+                    max_buffer_count=MAX_BUFFER_COUNT,
+                )
+                for name in self._batch_window_buffers
+            }
+
 
 class RecMetric(nn.Module, abc.ABC):
     r"""The main class template to implement a recommendation metric.
     This class contains the recommendation tasks information (RecTaskInfo) and
     the actual computation object (RecMetricComputation). RecMetric processes
     all the information related to RecTaskInfo and models, and passes the required
     signals to the computation object, allowing the implementation of
@@ -342,14 +353,19 @@
         self._default_weights = {}
         self._required_inputs = set()
         self._update_buffers = {
             self.PREDICTIONS: [],
             self.LABELS: [],
             self.WEIGHTS: [],
         }
+        if self._window_size < self._batch_size:
+            raise ValueError(
+                f"Local window size must be larger than batch size. Got local window size {self._window_size} and batch size {self._batch_size}."
+            )
+
         if compute_mode == RecComputeMode.FUSED_TASKS_COMPUTATION:
             task_per_metric = len(self._tasks)
             self._tasks_iter = self._fused_tasks_iter
         else:
             task_per_metric = 1
             self._tasks_iter = self._unfused_tasks_iter
```

## torchrec/models/experimental/test_transformerdlrm.py

```diff
@@ -220,15 +220,15 @@
             offsets=torch.tensor([0, 2, 4, 6, 8, 10, 11]),
         )
         logits = sparse_nn(
             dense_features=features,
             sparse_features=sparse_features,
         )
         self.assertEqual(logits.size(), (B, 1))
-        expected_logits = torch.tensor([[0.1659], [0.3247]])
+        expected_logits = torch.tensor([[-0.2593], [-0.1043]])
         self.assertTrue(
             torch.allclose(
                 logits,
                 expected_logits,
                 rtol=1e-4,
                 atol=1e-4,
             )
```

## torchrec/modules/embedding_configs.py

```diff
@@ -3,20 +3,21 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from dataclasses import dataclass, field
 from enum import Enum, unique
+from functools import partial
 from math import sqrt
-from typing import Dict, List, Optional
+from typing import Callable, Dict, List, Optional
 
 import torch
 from fbgemm_gpu.split_embedding_configs import SparseType
-from fbgemm_gpu.split_table_batched_embeddings_ops import PoolingMode
+from fbgemm_gpu.split_table_batched_embeddings_ops_training import PoolingMode
 
 
 @unique
 class PoolingType(Enum):
     SUM = "SUM"
     MEAN = "MEAN"
     NONE = "NONE"
@@ -81,17 +82,17 @@
     elif pooling_type.value == PoolingType.NONE.value:
         return PoolingMode.NONE
     else:
         raise Exception(f"Invalid pooling type {pooling_type}")
 
 
 def pooling_type_to_str(pooling_type: PoolingType) -> str:
-    if pooling_type == PoolingType.SUM:
+    if pooling_type.value == PoolingType.SUM.value:
         return "sum"
-    elif pooling_type == PoolingType.MEAN:
+    elif pooling_type.value == PoolingType.MEAN.value:
         return "mean"
     else:
         raise ValueError(f"Unsupported pooling type {pooling_type}")
 
 
 def data_type_to_sparse_type(data_type: DataType) -> SparseType:
     if data_type == DataType.FP32:
@@ -134,14 +135,16 @@
     num_embeddings: int
     embedding_dim: int
     name: str = ""
     data_type: DataType = DataType.FP32
     feature_names: List[str] = field(default_factory=list)
     weight_init_max: Optional[float] = None
     weight_init_min: Optional[float] = None
+
+    init_fn: Optional[Callable[[torch.Tensor], Optional[torch.Tensor]]] = None
     # when the position_weighted feature is in this table config,
     # enable this flag to support rw_sharding
     need_pos: bool = False
 
     def get_weight_init_max(self) -> float:
         if self.weight_init_max is None:
             return sqrt(1 / self.num_embeddings)
@@ -153,14 +156,22 @@
             return -sqrt(1 / self.num_embeddings)
         else:
             return self.weight_init_min
 
     def num_features(self) -> int:
         return len(self.feature_names)
 
+    def __post_init__(self) -> None:
+        if self.init_fn is None:
+            self.init_fn = partial(
+                torch.nn.init.uniform_,
+                a=self.get_weight_init_min(),
+                b=self.get_weight_init_max(),
+            )
+
 
 # this class will be deprecated after migration
 # and all the following code in sharding itself
 # which contains has_feature_processor
 @dataclass
 class EmbeddingTableConfig(BaseEmbeddingConfig):
     pooling: PoolingType = PoolingType.SUM
```

## torchrec/modules/embedding_modules.py

```diff
@@ -147,30 +147,32 @@
                 if embedding_config.data_type == DataType.FP32
                 else torch.float16
             )
             self.embedding_bags[embedding_config.name] = nn.EmbeddingBag(
                 num_embeddings=embedding_config.num_embeddings,
                 embedding_dim=embedding_config.embedding_dim,
                 mode=pooling_type_to_str(embedding_config.pooling),
-                device=device,
+                device=self._device,
                 include_last_offset=True,
                 dtype=dtype,
             )
+
             if not embedding_config.feature_names:
                 embedding_config.feature_names = [embedding_config.name]
             self._lengths_per_embedding.extend(
                 len(embedding_config.feature_names) * [embedding_config.embedding_dim]
             )
 
         self._embedding_names: List[str] = [
             embedding
             for embeddings in get_embedding_names_by_table(tables)
             for embedding in embeddings
         ]
         self._feature_names: List[List[str]] = [table.feature_names for table in tables]
+        self.reset_parameters()
 
     def forward(self, features: KeyedJaggedTensor) -> KeyedTensor:
         """
         Args:
             features (KeyedJaggedTensor): KJT of form [F X B X L].
 
         Returns:
@@ -202,14 +204,26 @@
     def embedding_bag_configs(self) -> List[EmbeddingBagConfig]:
         return self._embedding_bag_configs
 
     @property
     def device(self) -> torch.device:
         return self._device
 
+    def reset_parameters(self) -> None:
+        if (isinstance(self.device, torch.device) and self.device.type == "meta") or (
+            isinstance(self.device, str) and self.device == "meta"
+        ):
+            return
+        # Initialize embedding bags weights with init_fn
+        for table_config in self._embedding_bag_configs:
+            assert table_config.init_fn is not None
+            param = self.embedding_bags[f"{table_config.name}"].weight
+            # pyre-ignore
+            table_config.init_fn(param)
+
 
 class EmbeddingCollectionInterface(abc.ABC, nn.Module):
     """
     Interface for `EmbeddingCollection`.
     """
 
     @abc.abstractmethod
@@ -326,14 +340,17 @@
             )
             self.embeddings[config.name] = nn.Embedding(
                 num_embeddings=config.num_embeddings,
                 embedding_dim=config.embedding_dim,
                 device=device,
                 dtype=dtype,
             )
+            if config.init_fn is not None:
+                config.init_fn(self.embeddings[config.name].weight)
+
             if not config.feature_names:
                 config.feature_names = [config.name]
 
         self._embedding_names_by_table: List[List[str]] = get_embedding_names_by_table(
             tables
         )
         self._feature_names: List[List[str]] = [table.feature_names for table in tables]
@@ -379,7 +396,19 @@
 
     def embedding_names_by_table(self) -> List[List[str]]:
         return self._embedding_names_by_table
 
     @property
     def device(self) -> torch.device:
         return self._device
+
+    def reset_parameters(self) -> None:
+        if (isinstance(self.device, torch.device) and self.device.type == "meta") or (
+            isinstance(self.device, str) and self.device == "meta"
+        ):
+            return
+        # Initialize embedding bags weights with init_fn
+        for table_config in self._embedding_configs:
+            assert table_config.init_fn is not None
+            param = self.embeddings[f"{table_config.name}"].weight
+            # pyre-ignore
+            table_config.init_fn(param)
```

## torchrec/modules/fused_embedding_modules.py

```diff
@@ -12,15 +12,15 @@
 from collections import defaultdict
 from typing import Any, cast, Dict, Iterator, List, Optional, Set, Tuple, Type
 
 import torch
 import torch.nn as nn
 import torchrec.optim as trec_optim
 from fbgemm_gpu.split_embedding_configs import EmbOptimType
-from fbgemm_gpu.split_table_batched_embeddings_ops import (
+from fbgemm_gpu.split_table_batched_embeddings_ops_training import (
     ComputeDevice,
     EmbeddingLocation,
     SplitTableBatchedEmbeddingBagsCodegen,
 )
 from torchrec.modules.embedding_configs import (
     BaseEmbeddingConfig,
     DataType,
```

## torchrec/quant/embedding_modules.py

```diff
@@ -3,25 +3,26 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import copy
 import itertools
-from collections import defaultdict, OrderedDict
-from typing import Any, Dict, List, Optional, Tuple
+from collections import defaultdict
+from typing import Dict, List, Optional, Tuple
 
 import torch
 import torch.nn as nn
-from fbgemm_gpu.split_table_batched_embeddings_ops import (
+from fbgemm_gpu.split_table_batched_embeddings_ops_inference import (
     EmbeddingLocation,
     IntNBitTableBatchedEmbeddingBagsCodegen,
     PoolingMode,
 )
 from torch import Tensor
+from torchrec.distributed.utils import none_throws
 from torchrec.modules.embedding_configs import (
     DATA_TYPE_NUM_BITS,
     data_type_to_sparse_type,
     DataType,
     dtype_to_data_type,
     EmbeddingBagConfig,
     EmbeddingConfig,
@@ -219,32 +220,33 @@
         location = (
             EmbeddingLocation.HOST if device.type == "cpu" else EmbeddingLocation.DEVICE
         )
 
         for key, emb_configs in self._key_to_tables.items():
             (pooling, data_type) = key
             embedding_specs = []
-            weight_lists: Optional[List[Tuple[torch.Tensor, torch.Tensor]]] = (
-                [] if table_name_to_quantized_weights else None
-            )
+            weight_lists: Optional[
+                List[Tuple[torch.Tensor, Optional[torch.Tensor]]]
+            ] = ([] if table_name_to_quantized_weights else None)
             feature_table_map: List[int] = []
 
             for idx, table in enumerate(emb_configs):
                 embedding_specs.append(
                     (
                         table.name,
                         table.num_embeddings,
                         table.embedding_dim,
                         data_type_to_sparse_type(data_type),
                         location,
                     )
                 )
                 if table_name_to_quantized_weights:
-                    # pyre-ignore
-                    weight_lists.append(table_name_to_quantized_weights[table.name])
+                    none_throws(weight_lists).append(
+                        table_name_to_quantized_weights[table.name]
+                    )
                 feature_table_map.extend([idx] * table.num_features())
 
             emb_module = IntNBitTableBatchedEmbeddingBagsCodegen(
                 embedding_specs=embedding_specs,
                 pooling_mode=pooling_type_to_pooling_mode(pooling),
                 weight_lists=weight_lists,
                 device=device,
@@ -474,20 +476,21 @@
             self._embedding_dim = (
                 config.embedding_dim if self._embedding_dim < 0 else self._embedding_dim
             )
             if self._embedding_dim != config.embedding_dim:
                 raise ValueError(
                     "All tables in a EmbeddingCollection are required to have same embedding dimension."
                 )
-            weight_lists: Optional[List[Tuple[torch.Tensor, torch.Tensor]]] = (
-                [] if table_name_to_quantized_weights else None
-            )
+            weight_lists: Optional[
+                List[Tuple[torch.Tensor, Optional[torch.Tensor]]]
+            ] = ([] if table_name_to_quantized_weights else None)
             if table_name_to_quantized_weights:
-                # pyre-ignore
-                weight_lists.append(table_name_to_quantized_weights[config.name])
+                none_throws(weight_lists).append(
+                    table_name_to_quantized_weights[config.name]
+                )
             emb_module = IntNBitTableBatchedEmbeddingBagsCodegen(
                 embedding_specs=[
                     (
                         "",
                         config.num_embeddings,
                         config.embedding_dim,
                         data_type_to_sparse_type(config.data_type),
```

## torchrec/quant/utils.py

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 
-from typing import Union
+from typing import Optional, Union
 
 import torch
 from torch import nn
 from torchrec.distributed.model_parallel import DistributedModelParallel
 from torchrec.distributed.quant_embeddingbag import ShardedQuantEmbeddingBagCollection
 from torchrec.quant.embedding_modules import (
     EmbeddingBagCollection as QuantEmbeddingBagCollection,
@@ -57,31 +57,45 @@
     ):
         populate_fx_names(module)
         return
     for submodule in module.children():
         recursive_populate_fx_names(submodule)
 
 
-def meta_to_cpu_placement(module: DistributedModelParallel) -> None:
-    assert hasattr(module, "_dmp_wrapped_module")
-    _meta_to_cpu_placement(module.module, module, "_dmp_wrapped_module")
+def meta_to_cpu_placement(module: torch.nn.Module) -> None:
+    if hasattr(module, "_dmp_wrapped_module"):
+        # for placement update of dmp module, we need to fetch .module (read access) and write
+        # to .dmp_wrapped_module (write access)
+        assert type(module) == DistributedModelParallel
+        _meta_to_cpu_placement(module.module, module, "_dmp_wrapped_module")
+    else:
+        # shard module case
+        _meta_to_cpu_placement(module, module)
 
 
 def _meta_to_cpu_placement(
-    module: nn.Module, root_module: nn.Module, name: str
+    module: nn.Module, root_module: nn.Module, name: Optional[str] = None
 ) -> None:
-    if isinstance(module, QuantEmbeddingBagCollection) and module.device.type == "meta":
+    if (
+        name is not None
+        and isinstance(module, QuantEmbeddingBagCollection)
+        and module.device.type == "meta"
+    ):
         qebc_cpu = QuantEmbeddingBagCollection(
             tables=module.embedding_bag_configs(),
             is_weighted=module.is_weighted(),
             device=torch.device("cpu"),
             output_dtype=module.output_dtype(),
         )
         setattr(root_module, name, qebc_cpu)
-    elif isinstance(module, QuantEmbeddingCollection) and module.device.type == "meta":
+    elif (
+        name is not None
+        and isinstance(module, QuantEmbeddingCollection)
+        and module.device.type == "meta"
+    ):
         qec_cpu = QuantEmbeddingCollection(
             tables=module.embedding_configs(),
             device=torch.device("cpu"),
             need_indices=module.need_indices(),
             output_dtype=module.output_dtype(),
         )
         setattr(root_module, name, qec_cpu)
```

## torchrec/sparse/jagged_tensor.py

```diff
@@ -288,28 +288,28 @@
             values=values_tensor,
             weights=weights_tensor,
             lengths=lengths,
         )
 
     def to_dense(self) -> List[torch.Tensor]:
         """
-        Constructs dense-reprensentation tensor from JT.
+        Constructs a dense-representation of the JT's values.
 
         Returns:
             List[torch.Tensor]: list of tensors.
 
         Example::
 
             values = torch.Tensor([1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0])
             offsets = torch.IntTensor([0, 2, 2, 3, 4, 5, 8])
             jt = JaggedTensor(values=values, offsets=offsets)
 
-            torch_list = jt.to_dense()
+            values_list = jt.to_dense()
 
-            # torch_list = [
+            # values_list = [
             #     torch.tensor([1.0, 2.0]),
             #     torch.tensor([]),
             #     torch.tensor([3.0]),
             #     torch.tensor([4.0]),
             #     torch.tensor([5.0]),
             #     torch.tensor([6.0, 7.0, 8.0]),
             # ]
@@ -317,21 +317,55 @@
         tensor_list = []
         for index in range(self.offsets().size(0) - 1):
             offset = self.offsets()[index].item()
             next_offset = self.offsets()[index + 1].item()
             tensor_list.append(self.values()[offset:next_offset])
         return tensor_list
 
+    def to_dense_weights(self) -> Optional[List[torch.Tensor]]:
+        """
+        Constructs a dense-representation of the JT's weights.
+
+        Returns:
+            Optional[List[torch.Tensor]]: list of tensors, `None` if no weights.
+
+        Example::
+
+            values = torch.Tensor([1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0])
+            weights = torch.Tensor([0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8])
+            offsets = torch.IntTensor([0, 2, 2, 3, 4, 5, 8])
+            jt = JaggedTensor(values=values, weights=weights, offsets=offsets)
+
+            weights_list = jt.to_dense_weights()
+
+            # weights_list = [
+            #     torch.tensor([0.1, 0.2]),
+            #     torch.tensor([]),
+            #     torch.tensor([0.3]),
+            #     torch.tensor([0.4]),
+            #     torch.tensor([0.5]),
+            #     torch.tensor([0.6, 0.7, 0.8]),
+            # ]
+        """
+        if self.weights_or_none() is None:
+            return None
+        tensor_list = []
+        for index in range(self.offsets().size(0) - 1):
+            offset = self.offsets()[index].item()
+            next_offset = self.offsets()[index + 1].item()
+            tensor_list.append(self.weights()[offset:next_offset])
+        return tensor_list
+
     def to_padded_dense(
         self,
         desired_length: Optional[int] = None,
         padding_value: float = 0.0,
     ) -> torch.Tensor:
         """
-        Constructs 2D dense Tensor from JT to shape (B, N,).
+        Constructs a 2D dense tensor from the JT's values of shape (B, N,).
 
         Note that `B` is the length of self.lengths() and `N` is the longest feature
         length or `desired_length`.
 
         If `desired_length` > `length` we will pad with `padding_value`, otherwise we
         will select the last value at `desired_length`.
 
@@ -355,25 +389,77 @@
 
             # dt = [
             #     [1.0, 2.0],
             #     [10.0, 10.0],
             #     [3.0, 10.0],
             #     [4.0, 10.0],
             #     [5.0, 10.0],
-            #     [7.0, 8.0],
+            #     [6.0, 7.0],
             # ]
         """
         if desired_length is None:
             N = int(torch.max(self.lengths()).item())
         else:
             N = desired_length
         return torch.ops.fbgemm.jagged_to_padded_dense(
             self.values(), [self.offsets()], [N], padding_value
         )
 
+    def to_padded_dense_weights(
+        self,
+        desired_length: Optional[int] = None,
+        padding_value: float = 0.0,
+    ) -> Optional[torch.Tensor]:
+        """
+        Constructs a 2D dense tensor from the JT's weights of shape (B, N,).
+
+        Note that `B` is the length of self.lengths() and `N` is the longest feature
+        length or `desired_length`.
+
+        If `desired_length` > `length` we will pad with `padding_value`, otherwise we
+        will select the last value at `desired_length`.
+
+        Args:
+            desired_length (int): the length of the tensor.
+            padding_value (float): padding value if we need to pad.
+
+        Returns:
+            Optional[torch.Tensor]: 2d dense tensor, `None` if no weights.
+
+        Example::
+
+            values = torch.Tensor([1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0])
+            weights = torch.Tensor([0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8])
+            offsets = torch.IntTensor([0, 2, 2, 3, 4, 5, 8])
+            jt = JaggedTensor(values=values, weights=weights, offsets=offsets)
+
+            d_wt = jt.to_padded_dense_weights(
+                desired_length=2,
+                padding_value=1.0,
+            )
+
+            # d_wt = [
+            #     [0.1, 0.2],
+            #     [1.0, 1.0],
+            #     [0.3, 1.0],
+            #     [0.4, 1.0],
+            #     [0.5, 1.0],
+            #     [0.6, 0.7],
+            # ]
+        """
+        if self.weights_or_none() is None:
+            return None
+        if desired_length is None:
+            N = int(torch.max(self.lengths()).item())
+        else:
+            N = desired_length
+        return torch.ops.fbgemm.jagged_to_padded_dense(
+            self.weights(), [self.offsets()], [N], padding_value
+        )
+
     def lengths(self) -> torch.Tensor:
         _lengths = _maybe_compute_lengths(self._lengths, self._offsets)
         self._lengths = _lengths
         return _lengths
 
     def lengths_or_none(self) -> Optional[torch.Tensor]:
         return self._lengths
@@ -929,30 +1015,26 @@
         kjt_vals = torch.concat(tuple(jt.values() for jt in jt_dict.values()))
         kjt_lens = torch.concat(tuple(jt.lengths() for jt in jt_dict.values()))
         kjt_weights = tuple(
             jt.weights_or_none()
             for jt in jt_dict.values()
             if jt.weights_or_none() is not None
         )
-        kjt_length_per_key = [
-            int(torch.sum(jt.lengths()).item()) for jt in jt_dict.values()
-        ]
         # pyre-ignore[6]: Incompatible parameter type [6]:
         # In call `torch._C._VariableFunctions.concat`,
         # for 1st positional only parameter
         # expected `Union[List[Tensor], typing.Tuple[Tensor, ...]]`
         # but got `typing.Tuple[Optional[Tensor], ...]`
         kjt_weights = torch.concat(kjt_weights) if kjt_weights else None
         kjt = KeyedJaggedTensor(
             keys=kjt_keys,
             values=kjt_vals,
             weights=kjt_weights,
             lengths=kjt_lens,
-            length_per_key=kjt_length_per_key,
-        )
+        ).sync()
         return kjt
 
     def sync(self) -> "KeyedJaggedTensor":
         self.length_per_key()
         self.offset_per_key()
         return self
```

## Comparing `torchrec_nightly-2023.5.8.dist-info/LICENSE` & `torchrec_nightly-2023.6.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchrec_nightly-2023.5.8.dist-info/METADATA` & `torchrec_nightly-2023.6.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchrec-nightly
-Version: 2023.5.8
+Version: 2023.6.3
 Summary: Pytorch domain library for recommendation systems
 Home-page: https://github.com/pytorch/torchrec
 Author: TorchRec Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: pytorch,recommendation systems,sharding
 Classifier: Development Status :: 4 - Beta
```

## Comparing `torchrec_nightly-2023.5.8.dist-info/RECORD` & `torchrec_nightly-2023.6.3.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -9,131 +9,134 @@
 torchrec/datasets/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/datasets/scripts/contiguous_preproc_criteo.py,sha256=8jjtDiQScJH6R4FfKLgJ3fm-FzfnJxyfbV52zj3SM_8,2448
 torchrec/datasets/scripts/npy_preproc_criteo.py,sha256=QOyHZpPGL6HtPrVijk7qTALvnDqgecWPEZxKB_eVA94,2847
 torchrec/datasets/scripts/shuffle_preproc_criteo.py,sha256=PC1t5EkJkG6qu3ioewAVZM-Bnzo01HKMUH92IprFth0,3077
 torchrec/datasets/test_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/datasets/test_utils/criteo_test_utils.py,sha256=Ob2fJniGOsfbWNF_Gy2RJhrGAVnLAFPSlUTJOp2kay4,5308
 torchrec/distributed/__init__.py,sha256=VCy8GKOM-1dejxUWNSA3gozG3HQ4x5-Y9c9-WFbAMGg,1912
-torchrec/distributed/batched_embedding_kernel.py,sha256=nRkTFv6KK7aHD3Lwwmy7J-Q2pmIeyIr-orfMBtVsztk,36972
+torchrec/distributed/batched_embedding_kernel.py,sha256=_LWPI3zO_rObQgg0J0f-iojtpmazMfDfgHHg63hr_tE,37053
 torchrec/distributed/collective_utils.py,sha256=r7Aawq-KSVC-HjjEd6U8k0vNnRMx_-8_sAhYdElGaJw,2069
 torchrec/distributed/comm.py,sha256=21Std9n_HJCF3Nsw9O4yQQOJuL2DUVzZzoRhH3M6my8,4988
-torchrec/distributed/comm_ops.py,sha256=vrTHX7h81UxYoS5X3ufY4lE6WC2Ufo4mMJpGQC4dyV0,55820
-torchrec/distributed/dist_data.py,sha256=TwNB0e24k_tmn0XARaXKjUCf-92bgFDzBncj8BcXobY,35443
-torchrec/distributed/embedding.py,sha256=Ew0hvvY4XxwxYmvtCXa4Y6D_yhNkYdcHx0BOA_2nKbw,29817
+torchrec/distributed/comm_ops.py,sha256=C63THNJOnJWkfRYGuNw5opFyKsdlpZs9_23u-DHSrAQ,55918
+torchrec/distributed/dist_data.py,sha256=pWuAzn98i5O4lNHmv2wMGa4gksYEh_DOJT4rzRp_nYg,35580
+torchrec/distributed/embedding.py,sha256=it9ImgDu3u42W94lOolqXAtI-duxPVu45dGGPi6NOIU,30257
 torchrec/distributed/embedding_kernel.py,sha256=SNpvTbW1V4HtjSmAzPPa5imrUzSOe7zuQDkK3GFudHc,3872
-torchrec/distributed/embedding_lookup.py,sha256=JrLfam6U0B7X-QdC6nLeqxItyiV-tXoOxhRUqkPDhE0,27189
-torchrec/distributed/embedding_sharding.py,sha256=_4xDvyTm9Ut5XwnQGiANmvko3AzkgaB50d9Ooxr55xI,14990
+torchrec/distributed/embedding_lookup.py,sha256=1D7xO_ljztKkIIZJ7iziCI5mF65-S-l9hZ4Z6RAc1rY,28994
+torchrec/distributed/embedding_sharding.py,sha256=Kp8zJRIuBo_3XswENCCym9vnVId28Zh0HMoVqmcEoJI,18564
 torchrec/distributed/embedding_tower_sharding.py,sha256=ypr4JbTZUh_35dYUoKWoOSJNEVG3c6gV9g5gt-fs6lQ,37089
-torchrec/distributed/embedding_types.py,sha256=RAyug556PJTk5QlutuiXbo3ip4r9YXAmJupTNLhqKuk,15021
-torchrec/distributed/embeddingbag.py,sha256=6H9HFiHGgX9LXt67GKfFazrp5iWrbD30HleJZP8btas,34625
+torchrec/distributed/embedding_types.py,sha256=QbDVqeT2wb1RpnGZxrFtFdHYDsOHKW7SH8fLWmN_d0E,15030
+torchrec/distributed/embeddingbag.py,sha256=JffPXLKq_K0HAeSe8R3W3PrQuKowtdPTyHHez3qgdBs,35078
 torchrec/distributed/fbgemm_qcomm_codec.py,sha256=StYltKC6Eq6SE_YiX6GsVW3ZF0VyqTcGHXuCYmPAFlU,7373
+torchrec/distributed/fp_embeddingbag.py,sha256=tbwvTzBZXCBo_SSlyd7JnQOW6qWx1jdjmdeqnAnOaWM,5542
 torchrec/distributed/fused_embedding.py,sha256=uIgeaoEPujTgkcq8S2OPRYBe03J4TUF04uOOy_iRsMk,5273
 torchrec/distributed/fused_embeddingbag.py,sha256=7DIMc5sHdsDAgqCnNomcPo6V4aIH1wlkzyshHeJB3pc,5110
-torchrec/distributed/fused_params.py,sha256=WnPW8Crs9SSDFF33f4RZx_ok51I8-ql0yeA8N93aMtw,1699
+torchrec/distributed/fused_params.py,sha256=THLZYo_6mErDx2DGMB3Fi_VFPpLKCrq6Amvg8CckjsA,1709
 torchrec/distributed/grouped_position_weighted.py,sha256=q-QE0U306BiPkXIAlJGIQ80EUDZj-FXTbWwjz3EyvLI,3807
-torchrec/distributed/model_parallel.py,sha256=yfk_pYRT7ZrBh6UrukOgYbzHpg0yd6pFSU5NfA4SXxo,19528
-torchrec/distributed/quant_embedding.py,sha256=yFLsrmulaC0jopBSfjb6X-DaJ-08_sf-7lWqG6NlNdQ,13316
-torchrec/distributed/quant_embedding_kernel.py,sha256=wdCN5ZMGg3T-0sErGqLMJtDDVzVT44zX5rfQ-rWWUMM,13385
-torchrec/distributed/quant_embeddingbag.py,sha256=asSGkfXeG0hCB4pJlVhw_Wx97AjYwotIZd0h_e0ZbVg,10510
+torchrec/distributed/model_parallel.py,sha256=GiDEkZ89gFUBE_7psmbpEVGqQ17UkryIGlxEXWSxnyk,19520
+torchrec/distributed/quant_embedding.py,sha256=tbUP4_-iVvfAZlJ7gCf5ZJb6snH35EFLeJrZhATUZD8,13729
+torchrec/distributed/quant_embedding_kernel.py,sha256=FNEKKje7yvnOI28ODg5POQy2pmeKWNmPvf193JF8iEw,13343
+torchrec/distributed/quant_embeddingbag.py,sha256=MxFdFDn4HAJ9PRc3ko_6q4O0KuWkh3_Y1BHajX0E9aY,10931
 torchrec/distributed/shard.py,sha256=4Dr5ixWCoMEFEuL5WN4fL2gIdl9wmSUjZWsiF-kdCdQ,9261
-torchrec/distributed/sharding_plan.py,sha256=1CZyCmPp_lJPeitOgufRNfe77aXp9WtxsKDqVOm8XnU,19218
-torchrec/distributed/train_pipeline.py,sha256=RotmGdM_UduxSbrf3l8JKrowIeMhrB2DaNJHFwXPjIY,22330
+torchrec/distributed/sharding_plan.py,sha256=vVQhmXy2w4FmXyuJa1t6PyfaqEEVSxoLZ5ChWlc7TbU,19411
+torchrec/distributed/train_pipeline.py,sha256=0twZDc4PIt2Sz6q2DEvyaz6P6jHb7-fmj_bTiA7ir7E,34059
 torchrec/distributed/types.py,sha256=tNd_B5PXjaOqPmUXxSZLXB3a71sjU8LBtSY9kuGxe7I,24927
 torchrec/distributed/utils.py,sha256=isPXbyPhHlbjiA0280ZY0V_wPUBuvDvvH4w6ziP5XA8,11373
 torchrec/distributed/composable/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/distributed/composable/table_batched_embedding_slice.py,sha256=x439M8TTXQtzoihan1OKKbmGYkqJlAxxTHCDz5295RY,3207
 torchrec/distributed/planner/__init__.py,sha256=UWnxb-SuE211uJGdwtSkKRVADT3plQozB2l6fvs6Ve0,1025
 torchrec/distributed/planner/constants.py,sha256=MkeVqYO2QGg57i6fs29lZb2dScaaR9mdQVsee4NxyFc,3135
 torchrec/distributed/planner/enumerators.py,sha256=hZzhnfMrOz65lBoddxTKBb01hm43R_5tdpysJFSzCLE,10318
-torchrec/distributed/planner/partitioners.py,sha256=AwIuyCyyJGhy_WmzEipIdglx9PbOGAEmvp6qgLVCzpU,12485
-torchrec/distributed/planner/perf_models.py,sha256=srFJ0AkOhLVhumdcuyYzl5J1qzezt6knt-TxZvK6Zy4,824
-torchrec/distributed/planner/planners.py,sha256=dPfT-SjjKgv9jYZ-piwWPw9fhgzVWSqSb1CNCJt2Zcg,12224
-torchrec/distributed/planner/proposers.py,sha256=A-adzCCshGZUIyCP7DPOGDuh4hbojawWuObxsIf-rOg,11094
-torchrec/distributed/planner/shard_estimators.py,sha256=H9rZJV9_BwgRyImzXT0YXiymJ6FhRzudTg9NXrLoTOs,40173
-torchrec/distributed/planner/stats.py,sha256=my1OB-r1HO-ixc7joRz1CltZlQJDBrjJOtLIXDY7B5c,21410
+torchrec/distributed/planner/partitioners.py,sha256=k-rzm6oMZ_sLpGHT8yAu2tIMkMumhJMvAFeY0cdNirk,12642
+torchrec/distributed/planner/perf_models.py,sha256=vYIjVr0NG6sZItfxVuRWF7AS8lGGtbRn66O0flNJpoU,835
+torchrec/distributed/planner/planners.py,sha256=LjMOoQTu_IlwlG-wl03H39c886oxBgfEQMKsouYI1pM,13288
+torchrec/distributed/planner/proposers.py,sha256=s8nDZcZWiGmaFVHr8J3wmuoUYFGpe6n1NPLtprOqSgk,11134
+torchrec/distributed/planner/shard_estimators.py,sha256=JTdL0OI0kpFbkxdCZN9qK46PN6v2kv2mIMdXLIZMsOE,40395
+torchrec/distributed/planner/stats.py,sha256=oIhRnFQybUdx-2NEH3ZBhyx0nqtiR4VkQKnS7YLW6CY,23617
 torchrec/distributed/planner/storage_reservations.py,sha256=rPqeD03f3mg8yoSqy9CZfOmxVMUGrCz98nPqwvxhApc,9125
-torchrec/distributed/planner/types.py,sha256=16iitmowdWqzenpyeCvkWzQZW7OSOMjbpZzKDo3WDUo,12879
+torchrec/distributed/planner/types.py,sha256=JG39UMXzWQ7_G38aG2qo3h601s2UsII_OPyHJ068kOM,13899
 torchrec/distributed/planner/utils.py,sha256=YwOUrqb-D6HaVtWCRFz9RWhBdMRBqjMaYYhoQgyOkQg,1119
 torchrec/distributed/sharding/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/distributed/sharding/cw_sequence_sharding.py,sha256=o8RZAs2zivNP8MZ5QUWF0alw7KwWZnJVG9iKHM4EJdE,2539
 torchrec/distributed/sharding/cw_sharding.py,sha256=PLJHgxkQvX_sNI8RJlz4xIemb4vO2KHOe_9PylZ2je8,9519
 torchrec/distributed/sharding/dp_sequence_sharding.py,sha256=zQmERguEGVd5IAbmVsIhqdKXb0f2g8tQamN838qVvfM,2802
-torchrec/distributed/sharding/dp_sharding.py,sha256=GwbU9BOOdqucVD6qqW3SwbBOcB8No5P5wvXqSeSaUAs,7452
+torchrec/distributed/sharding/dp_sharding.py,sha256=HSedwv3zCoi-WGElzucyqDMolrviB6tyqs1jN-6RTEY,7681
 torchrec/distributed/sharding/rw_sequence_sharding.py,sha256=66tW1TyIp8kSdT3t8EsVsHcv7_kAzbCX3xT_pDmc_NE,5041
 torchrec/distributed/sharding/rw_sharding.py,sha256=k3ym1GGjdQeRnLeUheZm5o9D8co_U4dUQgHrF771XUQ,12850
 torchrec/distributed/sharding/sequence_sharding.py,sha256=LBUW1PvAV9WNwf-m-x9bYIcU96PL75mPE_uQK9dLAOU,3114
-torchrec/distributed/sharding/tw_sequence_sharding.py,sha256=MNlniKPVzshZWYwGoqA3bt5FsZrhBISk9b2TOrMa4eU,7609
-torchrec/distributed/sharding/tw_sharding.py,sha256=dbVwsNbUtLntRODZJjMWMFQq-IVsSn9iiTmnMG6644E,16061
+torchrec/distributed/sharding/tw_sequence_sharding.py,sha256=SR_G_rniSZx_DBnrWW14HEMoeqwRnMPN3LdQlnptLL8,7692
+torchrec/distributed/sharding/tw_sharding.py,sha256=JtI2GW9YR-eg1VuQDwDa6qaR6sOgBAzGx3Y3XkEOBZM,16315
 torchrec/distributed/sharding/twcw_sharding.py,sha256=LyOowcADWmRdkRn-eEW6QB0b0xYi0vM-Ubrr6N2zwwA,1284
 torchrec/distributed/sharding/twrw_sharding.py,sha256=k69AX5oKj3ep38tM_RI_NkwyZ4z_U8kVQpLtDjRYPKI,19898
 torchrec/distributed/test_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-torchrec/distributed/test_utils/infer_utils.py,sha256=OTsqNFGMgT5VWF-Ww94JbLsCDmv2KqB5R50O-ynK0Sg,10125
+torchrec/distributed/test_utils/infer_utils.py,sha256=v3OLVjfmy612aSSDPpFeu8m7K9omDAO9JFWQ08NHcZI,10213
 torchrec/distributed/test_utils/multi_process.py,sha256=6AxYe2cO44EGdw-Lt5YNwqmWZW8Ldu7bVGTluIIOFbA,4868
 torchrec/distributed/test_utils/test_model.py,sha256=x4DxsGp6YfBBJMyrkBwOZTFpotm6VB8V6tLxuanHNFM,34114
 torchrec/distributed/test_utils/test_model_parallel.py,sha256=oN_fl-QOaAarrZwnr7q5Lz4f9xiqxxof9Bk_4PM13hM,11193
 torchrec/distributed/test_utils/test_model_parallel_base.py,sha256=05SOQyzfHS5jyZkSzUNmhGa3sT43cX2M_w_FiWrZhBw,25075
 torchrec/distributed/test_utils/test_sharding.py,sha256=DlB6N5-qlRp-xQfEEFElDkNffnEX6LO4vOrDCGp8VkQ,15367
 torchrec/fx/__init__.py,sha256=TxNjllMWlB_rpDy4SNSA_e-xbZbhxGGTb9AxpZGcaFk,422
 torchrec/fx/tracer.py,sha256=iXfWWgPNdFlRs89RbA18Nel0Tl9z8UprRWPfTQbLx5k,6477
 torchrec/fx/utils.py,sha256=N50AfwlUhyS9r1Sv21fSbqRxiOk4KRX0MX9sDjCaQcA,4401
 torchrec/inference/__init__.py,sha256=vi2C_o1Bvsp6hS3_uVZTL7kShgxw5qFZp248Svee2Og,1223
 torchrec/inference/client.py,sha256=jS6ldQxBRY3Bp_LwDLUNSlPt2VYMc-Hsd4iKKoHfDVU,3614
 torchrec/inference/model_packager.py,sha256=HxOEbnqXB2K4uUB9dBBJAL49ZYJME4xTFyVzKjpsjy4,3957
 torchrec/inference/modules.py,sha256=4Qfea1MUXjX-qknC7VO8BkodJU8-BA-kMQUGjdq2j64,7834
 torchrec/inference/state_dict_transform.py,sha256=eFejfFRzU3pL7CmiJtkjq2mpz6Ue_NOUuO2g8-LnLig,3797
 torchrec/metrics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-torchrec/metrics/auc.py,sha256=-aRUv-fVdnTAYAhoV6fp5zvcoadl54BAOzzBFLIPF2I,12728
+torchrec/metrics/auc.py,sha256=vyUUEJc6Kp1R5kSHBH0t0lI1ZdZzCr0dad6v0aVxJIA,12549
 torchrec/metrics/calibration.py,sha256=hngIvPjcAHusdz1KBrPvwMZX6OkyS0nv18EAmMcyIl0,3703
 torchrec/metrics/ctr.py,sha256=2HY53CX9If6wYcOErvYCT73NH8UdY8oI0UIitoREsMs,3465
 torchrec/metrics/mae.py,sha256=QDPT7l4LCBtTgoxEeEm9vFzCEDtEIlfzs58PtH1oS_U,3836
 torchrec/metrics/metric_module.py,sha256=Zb871gbVS2ymaoslwJIaFbps0tEjDiOiCStoppMj_bA,17812
-torchrec/metrics/metrics_config.py,sha256=eZW2aD6fLK9eqhFU6G62Ph5R0KwkDUjErj7Irbg0k68,6615
+torchrec/metrics/metrics_config.py,sha256=ASCrwplAR7ivkgJ5arUrXVjVsU5PY49bfeCvj8_yTk4,6752
 torchrec/metrics/metrics_namespace.py,sha256=nHQCcGJujWcHR8KWDRgGY2yLpKvqtNTAL42o953nPck,3643
 torchrec/metrics/model_utils.py,sha256=WNMsAKK9b5OVPWeuRrNDZ2HjwKuAw3gjNG3OdE99EXw,3904
 torchrec/metrics/mse.py,sha256=tkK3yBV8Uu9Z8Mw_3c1k4kYAhp1jUQkFEJxc0l2LtWU,4631
 torchrec/metrics/multiclass_recall.py,sha256=7NqjkA4IUy4Db90du3hVt8cJxoWS18PBaOourHETkEs,5605
 torchrec/metrics/ne.py,sha256=wXEb9Eh5Mn3D_uuAIaUb3CvJ1eDs06ahVxaWOjR4CtU,6811
-torchrec/metrics/rec_metric.py,sha256=OLiACQ0nL9LCRtJt23_pax02VVdKV9Hq6O-3af3Ml1E,30881
+torchrec/metrics/rec_metric.py,sha256=Oq6SRk_TVOXba3qgKbNc7X2ExsiaHNA00J_ZhhkYpHY,31495
 torchrec/metrics/recall_session.py,sha256=24aDBSi8V5XXSnwpqCR5bWcm2CWslBBZ9_a0LQ6VGeg,10490
 torchrec/metrics/throughput.py,sha256=A_WqccFNgu4XpBZzZxnGxAT84Xp2ld43qQM6R1zaqik,6057
 torchrec/metrics/tower_qps.py,sha256=YC-EzaU2hbAQ3VZ1GJDHjWNKLD8fEvyyM5A5WerjwZU,10622
 torchrec/metrics/weighted_avg.py,sha256=dX-qwha2__F-p-R5u27152OwlGRS6Xfnbt1DEIBw8NQ,2867
 torchrec/metrics/test_utils/__init__.py,sha256=p_uep7Hg7_aY3rOg8CxtS-REopQ4ywQq075KFoso1Lw,16441
 torchrec/models/__init__.py,sha256=iYpG-yLxFaa3ZdN-UU9PWNIdgm9EXoEj_QzJ2OLKGJQ,913
 torchrec/models/deepfm.py,sha256=-SxFKF-kHKFEzC0XIsLigQh673-B_Lu6xFlZPkR5t2g,11410
 torchrec/models/dlrm.py,sha256=37v6MOb8P06DtXfDDqokvSKSDyhDVGFEPsRoBSRtCTY,30000
 torchrec/models/experimental/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-torchrec/models/experimental/test_transformerdlrm.py,sha256=cdmMgbpJiK_6AMdv1ALmcoK9zCuSagdtVH0ozh9ds-E,9823
+torchrec/models/experimental/test_transformerdlrm.py,sha256=pxdu5k-EdTdYX5RblAe1A97GuiHAUmm6oJwfG_qX8Vw,9825
 torchrec/models/experimental/transformerdlrm.py,sha256=-mWI0-_Au5wIIzGuXBri59RWHs4u5SiEal4rzm5DOeE,7434
 torchrec/modules/__init__.py,sha256=Eho7Nd68vOa0p-WuM7-cRSc_vhA38JU88PTcdfuWEvA,1179
 torchrec/modules/activation.py,sha256=o3rGyy40bmmsplyxQy3dDMe8kITRERLJQF7oa5VTKfE,1456
 torchrec/modules/crossnet.py,sha256=hiE375Y0atKsyWYK3GLPtx5VzqkaoNl79r9HsxtMBVA,15163
 torchrec/modules/deepfm.py,sha256=05ZM2sB1YMVliZwrLHvtMYf3eWGguLFopaZwGZK16bs,8415
-torchrec/modules/embedding_configs.py,sha256=hefNZ3uhbtzGY3rvPhJDiUlwetLYp3oKQefGQtO-mAA,5131
-torchrec/modules/embedding_modules.py,sha256=TbOVicALMAku13yzqhhIr4eJKVz8Hj-kCoBKckLinhA,12822
+torchrec/modules/embedding_configs.py,sha256=97g9ui8baC7RdqzB6EPxgkLvGaiX_-r24igTSlXyfcs,5537
+torchrec/modules/embedding_modules.py,sha256=ezRcQ2BqgEEdDF-86Aeribm44YHtaA21NrgOvfr_KYM,14021
 torchrec/modules/embedding_tower.py,sha256=rHiMEUUMoMZUxIPKBE2HyI7I5uNthGQsZIxH038TmoI,4858
 torchrec/modules/feature_processor.py,sha256=UqDELZQ7cRpAQb_6LyxwVByJDdM5NPDfAyEk4qYQmKM,12360
-torchrec/modules/fused_embedding_modules.py,sha256=LZ5vk4A6nA8StOSc5WlfXlOV9j2QN2jqmjF4BQsZuzs,31184
+torchrec/modules/feature_processor_.py,sha256=P4gttrqiWmdmMB7sceB8D0Nn-oKTn4LzXpocK7voCd8,2169
+torchrec/modules/fp_embedding_modules.py,sha256=v6dNQqlB4TnJ-3CMmJDjHBZ60dQheBkx0OZ40wYgTHU,4028
+torchrec/modules/fused_embedding_modules.py,sha256=a0mRx3JGTGtMoEwagOhJyW5DTI85iagUT7l6WN0YJOE,31193
 torchrec/modules/lazy_extension.py,sha256=0yOchNRZsOT3A2n5DN5wZhYHjIZkc0F6z_xWX_ULGp0,10696
 torchrec/modules/mlp.py,sha256=lV3vCEmNLI1kDtF4eGlCaGvtG3FQ8UEMs4Hcc6Nf3pM,6309
 torchrec/modules/utils.py,sha256=Ohx144TmZCEHbv3oEUsBf8e4DkGjmyPf98N4mA8kCxo,4022
 torchrec/optim/__init__.py,sha256=4-nuv6JsmuWBtzyUvCKJ0b9-m7oFi8QB2b3krFF0KgQ,1639
 torchrec/optim/apply_optimizer_in_backward.py,sha256=0wjamGai9i0rXvIf4GNYNhCz7NtkH_9expuepk1qcbI,2012
 torchrec/optim/clipping.py,sha256=sDotlb8Sf4D7-lbBxhzRDFHoiO_DVx34F1J8vOEWq8I,1569
 torchrec/optim/fused.py,sha256=J4u2PWaHD65PIEdg0wTWoK_riZCoSKAVKYPGuZtfKLY,1353
 torchrec/optim/keyed.py,sha256=5QASHSkw2oYwu3OVHU5JJ2mm5tQaSCOQ3z_vBVRLPtk,16069
 torchrec/optim/optimizers.py,sha256=tmf-ww_47F_tu04ufffVCczM2AOMR5yTNh_8S-gJl-8,4420
 torchrec/optim/rowwise_adagrad.py,sha256=jHpCZDFWRrXbwlKiwROg2dl0qK1lG2uXMJkTtbZ_uSg,7405
 torchrec/optim/warmup.py,sha256=QaMcWU-jMZbDOfRHEH_x9r7EsjtI_LRgOGAmEgzJWSQ,4865
 torchrec/optim/test_utils/__init__.py,sha256=mkNZr5iNV3kseuamPBnnAeknjbv4ELPFMGyJ1lWiJGU,560
 torchrec/quant/__init__.py,sha256=A6NIA6ztq6iP1JTLRLNzlgnCcd-LaN8efnxGub3Ii4A,1140
-torchrec/quant/embedding_modules.py,sha256=V4lPuXukSXBXz92AqQ1PBpQcQXh03TiK-GNtlJNiqug,22824
-torchrec/quant/utils.py,sha256=2oUJIsrzE7ijvPs5DYUa06wOfmRvU1KdU1aQI7DUccs,3691
+torchrec/quant/embedding_modules.py,sha256=RLuYVywThBXgLEZeHrH2F1sGEA1XydzBg4S9v2rivgY,22933
+torchrec/quant/utils.py,sha256=PkgXn7wnnBIqJ5JAidJMvpAVre1YL8oiYGiPuV_gU2c,4100
 torchrec/sparse/__init__.py,sha256=dLqSye4Jo6obnNNTUKdPDxPQb9sL2U4weemSn-DjpYk,1163
-torchrec/sparse/jagged_tensor.py,sha256=MoyqQJC8ezXOPLLEGK1o4zzI_SQ18tUUQ3zzOlW-_b4,52763
+torchrec/sparse/jagged_tensor.py,sha256=t0QsLwPZ9l2M5by3FpGOPXL6KeSWQqOp7hLayDF-DAc,55649
 torchrec/sparse/test_utils/__init__.py,sha256=BLxfGKJvwjjCiQM64O5wGAA_Cea0sG-buw9lTDWuqug,1430
 torchrec/test_utils/__init__.py,sha256=JncJcXS4N3gI7-fsizQ2-qiWM6MhIrpvskF_9gDf0Go,5661
-torchrec_nightly-2023.5.8.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
-torchrec_nightly-2023.5.8.dist-info/METADATA,sha256=rZjE_5lkGM1WowcU0fGdz3e2rlljTQi6Uj1f-IO01_8,5011
-torchrec_nightly-2023.5.8.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
-torchrec_nightly-2023.5.8.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
-torchrec_nightly-2023.5.8.dist-info/RECORD,,
+torchrec_nightly-2023.6.3.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
+torchrec_nightly-2023.6.3.dist-info/METADATA,sha256=2uRzUeXbi1fpn1mkRrVfF5oIeJH8RFeIGlrH8zJ49Ec,5011
+torchrec_nightly-2023.6.3.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
+torchrec_nightly-2023.6.3.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
+torchrec_nightly-2023.6.3.dist-info/RECORD,,
```

