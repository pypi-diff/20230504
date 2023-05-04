# Comparing `tmp/towhee-0.9.0-py3-none-any.whl.zip` & `tmp/towhee-1.0.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,238 +1,146 @@
-Zip file size: 362135 bytes, number of entries: 236
--rw-r--r--  2.0 unx     4274 b- defN 22-Dec-02 13:07 towhee/__init__.py
--rw-r--r--  2.0 unx      665 b- defN 22-Dec-02 13:07 towhee/__main__.py
--rw-r--r--  2.0 unx      766 b- defN 22-Dec-02 13:07 towhee/dc2.py
--rw-r--r--  2.0 unx     1281 b- defN 22-Dec-02 13:07 towhee/errors.py
--rw-r--r--  2.0 unx     1741 b- defN 22-Dec-02 13:07 towhee/pipeline_format.py
--rw-r--r--  2.0 unx      630 b- defN 22-Dec-02 13:07 towhee/_types/__init__.py
--rw-r--r--  2.0 unx      662 b- defN 22-Dec-02 13:07 towhee/_types/image.py
--rw-r--r--  2.0 unx      619 b- defN 22-Dec-02 13:07 towhee/command/__init__.py
--rw-r--r--  2.0 unx     1829 b- defN 22-Dec-02 13:07 towhee/command/cmdline.py
--rw-r--r--  2.0 unx     4668 b- defN 22-Dec-02 13:07 towhee/command/develop.py
--rw-r--r--  2.0 unx     8369 b- defN 22-Dec-02 13:07 towhee/command/execute.py
--rw-r--r--  2.0 unx     4908 b- defN 22-Dec-02 13:07 towhee/command/repo.py
--rw-r--r--  2.0 unx     9829 b- defN 22-Dec-02 13:07 towhee/command/s3.py
--rw-r--r--  2.0 unx     5240 b- defN 22-Dec-02 13:07 towhee/command/user.py
--rw-r--r--  2.0 unx      882 b- defN 22-Dec-02 13:07 towhee/dag/__init__.py
--rw-r--r--  2.0 unx     5713 b- defN 22-Dec-02 13:07 towhee/dag/base_repr.py
--rw-r--r--  2.0 unx     2138 b- defN 22-Dec-02 13:07 towhee/dag/dataframe_repr.py
--rw-r--r--  2.0 unx     3968 b- defN 22-Dec-02 13:07 towhee/dag/graph_builder.py
--rw-r--r--  2.0 unx     9137 b- defN 22-Dec-02 13:07 towhee/dag/graph_repr.py
--rw-r--r--  2.0 unx     4072 b- defN 22-Dec-02 13:07 towhee/dag/operator_repr.py
--rw-r--r--  2.0 unx     1377 b- defN 22-Dec-02 13:07 towhee/dag/variable_repr.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-02 13:07 towhee/data/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-02 13:07 towhee/data/dataset/__init__.py
--rw-r--r--  2.0 unx      662 b- defN 22-Dec-02 13:07 towhee/data/dataset/dataset.py
--rw-r--r--  2.0 unx     2918 b- defN 22-Dec-02 13:07 towhee/data/dataset/image_datasets.py
--rw-r--r--  2.0 unx      714 b- defN 22-Dec-02 13:07 towhee/datacollection/__init__.py
--rw-r--r--  2.0 unx     7581 b- defN 22-Dec-02 13:07 towhee/datacollection/data_collection.py
--rw-r--r--  2.0 unx     3448 b- defN 22-Dec-02 13:07 towhee/datacollection/entity.py
--rw-r--r--  2.0 unx      627 b- defN 22-Dec-02 13:07 towhee/datacollection/mixins/__init__.py
--rw-r--r--  2.0 unx    15202 b- defN 22-Dec-02 13:07 towhee/datacollection/mixins/display.py
--rw-r--r--  2.0 unx      756 b- defN 22-Dec-02 13:07 towhee/dataframe/__init__.py
--rw-r--r--  2.0 unx     1687 b- defN 22-Dec-02 13:07 towhee/dataframe/_schema.py
--rw-r--r--  2.0 unx    27036 b- defN 22-Dec-02 13:07 towhee/dataframe/dataframe.py
--rw-r--r--  2.0 unx     7914 b- defN 22-Dec-02 13:07 towhee/dataframe/iterators.py
--rw-r--r--  2.0 unx      725 b- defN 22-Dec-02 13:07 towhee/dataframe/array/__init__.py
--rw-r--r--  2.0 unx     4602 b- defN 22-Dec-02 13:07 towhee/dataframe/array/array.py
--rw-r--r--  2.0 unx      972 b- defN 22-Dec-02 13:07 towhee/dataframe/array/utils.py
--rw-r--r--  2.0 unx     1222 b- defN 22-Dec-02 13:07 towhee/engine/__init__.py
--rw-r--r--  2.0 unx     4784 b- defN 22-Dec-02 13:07 towhee/engine/engine.py
--rw-r--r--  2.0 unx     9515 b- defN 22-Dec-02 13:07 towhee/engine/factory.py
--rw-r--r--  2.0 unx     4107 b- defN 22-Dec-02 13:07 towhee/engine/graph_context.py
--rw-r--r--  2.0 unx     5561 b- defN 22-Dec-02 13:07 towhee/engine/operator_context.py
--rw-r--r--  2.0 unx     7450 b- defN 22-Dec-02 13:07 towhee/engine/operator_loader.py
--rw-r--r--  2.0 unx     3786 b- defN 22-Dec-02 13:07 towhee/engine/operator_pool.py
--rw-r--r--  2.0 unx     7104 b- defN 22-Dec-02 13:07 towhee/engine/operator_registry.py
--rw-r--r--  2.0 unx     3849 b- defN 22-Dec-02 13:07 towhee/engine/pipeline.py
--rw-r--r--  2.0 unx     1162 b- defN 22-Dec-02 13:07 towhee/engine/status.py
--rw-r--r--  2.0 unx     4494 b- defN 22-Dec-02 13:07 towhee/engine/task_scheduler.py
--rw-r--r--  2.0 unx     3303 b- defN 22-Dec-02 13:07 towhee/engine/thread_pool_task_executor.py
--rw-r--r--  2.0 unx     2034 b- defN 22-Dec-02 13:07 towhee/engine/uri.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-02 13:07 towhee/engine/execution/__init__.py
--rw-r--r--  2.0 unx     1867 b- defN 22-Dec-02 13:07 towhee/engine/execution/base_execution.py
--rw-r--r--  2.0 unx     1192 b- defN 22-Dec-02 13:07 towhee/engine/execution/pandas_execution.py
--rw-r--r--  2.0 unx     1115 b- defN 22-Dec-02 13:07 towhee/engine/execution/stateful_execution.py
--rw-r--r--  2.0 unx     3892 b- defN 22-Dec-02 13:07 towhee/engine/execution/vectorized_execution.py
--rw-r--r--  2.0 unx     1855 b- defN 22-Dec-02 13:07 towhee/engine/operator_io/__init__.py
--rw-r--r--  2.0 unx     1114 b- defN 22-Dec-02 13:07 towhee/engine/operator_io/_mock_reader.py
--rw-r--r--  2.0 unx     5567 b- defN 22-Dec-02 13:07 towhee/engine/operator_io/reader.py
--rw-r--r--  2.0 unx     1770 b- defN 22-Dec-02 13:07 towhee/engine/operator_io/writer.py
--rw-r--r--  2.0 unx     2360 b- defN 22-Dec-02 13:07 towhee/engine/operator_runner/__init__.py
--rw-r--r--  2.0 unx     1543 b- defN 22-Dec-02 13:07 towhee/engine/operator_runner/concat_runner.py
--rw-r--r--  2.0 unx     1256 b- defN 22-Dec-02 13:07 towhee/engine/operator_runner/filter_runner.py
--rw-r--r--  2.0 unx     1489 b- defN 22-Dec-02 13:07 towhee/engine/operator_runner/flatmap_runner.py
--rw-r--r--  2.0 unx     1663 b- defN 22-Dec-02 13:07 towhee/engine/operator_runner/generator_runner.py
--rw-r--r--  2.0 unx      884 b- defN 22-Dec-02 13:07 towhee/engine/operator_runner/map_runner.py
--rw-r--r--  2.0 unx     6750 b- defN 22-Dec-02 13:07 towhee/engine/operator_runner/runner_base.py
--rw-r--r--  2.0 unx     1859 b- defN 22-Dec-02 13:07 towhee/engine/operator_runner/window_runner.py
--rw-r--r--  2.0 unx     7669 b- defN 22-Dec-02 13:07 towhee/functional/__init__.py
--rw-r--r--  2.0 unx    20457 b- defN 22-Dec-02 13:07 towhee/functional/data_collection.py
--rw-r--r--  2.0 unx     5286 b- defN 22-Dec-02 13:07 towhee/functional/entity.py
--rw-r--r--  2.0 unx     4984 b- defN 22-Dec-02 13:07 towhee/functional/option.py
--rw-r--r--  2.0 unx     6413 b- defN 22-Dec-02 13:07 towhee/functional/storages.py
--rw-r--r--  2.0 unx     1790 b- defN 22-Dec-02 13:07 towhee/functional/mixins/__init__.py
--rw-r--r--  2.0 unx     1329 b- defN 22-Dec-02 13:07 towhee/functional/mixins/audio.py
--rw-r--r--  2.0 unx    10246 b- defN 22-Dec-02 13:07 towhee/functional/mixins/column.py
--rw-r--r--  2.0 unx     8253 b- defN 22-Dec-02 13:07 towhee/functional/mixins/compile.py
--rw-r--r--  2.0 unx     6379 b- defN 22-Dec-02 13:07 towhee/functional/mixins/computer_vision.py
--rw-r--r--  2.0 unx     7216 b- defN 22-Dec-02 13:07 towhee/functional/mixins/config.py
--rw-r--r--  2.0 unx    12949 b- defN 22-Dec-02 13:07 towhee/functional/mixins/dag.py
--rw-r--r--  2.0 unx    11767 b- defN 22-Dec-02 13:07 towhee/functional/mixins/data_processing.py
--rw-r--r--  2.0 unx    11197 b- defN 22-Dec-02 13:07 towhee/functional/mixins/dataframe.py
--rw-r--r--  2.0 unx     5687 b- defN 22-Dec-02 13:07 towhee/functional/mixins/dataset.py
--rw-r--r--  2.0 unx     1956 b- defN 22-Dec-02 13:07 towhee/functional/mixins/dispatcher.py
--rw-r--r--  2.0 unx    15429 b- defN 22-Dec-02 13:07 towhee/functional/mixins/display.py
--rw-r--r--  2.0 unx     5802 b- defN 22-Dec-02 13:07 towhee/functional/mixins/faiss.py
--rw-r--r--  2.0 unx     1689 b- defN 22-Dec-02 13:07 towhee/functional/mixins/format_priority.py
--rw-r--r--  2.0 unx     3748 b- defN 22-Dec-02 13:07 towhee/functional/mixins/kv_storage.py
--rw-r--r--  2.0 unx     5739 b- defN 22-Dec-02 13:07 towhee/functional/mixins/list.py
--rw-r--r--  2.0 unx     6969 b- defN 22-Dec-02 13:07 towhee/functional/mixins/metric.py
--rw-r--r--  2.0 unx     4515 b- defN 22-Dec-02 13:07 towhee/functional/mixins/milvus.py
--rw-r--r--  2.0 unx    12029 b- defN 22-Dec-02 13:07 towhee/functional/mixins/parallel.py
--rw-r--r--  2.0 unx     7053 b- defN 22-Dec-02 13:07 towhee/functional/mixins/ray.py
--rw-r--r--  2.0 unx     4260 b- defN 22-Dec-02 13:07 towhee/functional/mixins/safe.py
--rw-r--r--  2.0 unx     7338 b- defN 22-Dec-02 13:07 towhee/functional/mixins/serve.py
--rw-r--r--  2.0 unx     3417 b- defN 22-Dec-02 13:07 towhee/functional/mixins/state.py
--rw-r--r--  2.0 unx     2739 b- defN 22-Dec-02 13:07 towhee/functional/mixins/stream.py
--rw-r--r--  2.0 unx      368 b- defN 22-Dec-02 13:07 towhee/hparam/__init__.py
--rw-r--r--  2.0 unx    15787 b- defN 22-Dec-02 13:07 towhee/hparam/hyperparameter.py
--rw-r--r--  2.0 unx      593 b- defN 22-Dec-02 13:07 towhee/hub/__init__.py
--rw-r--r--  2.0 unx    18524 b- defN 22-Dec-02 13:07 towhee/hub/file_manager.py
--rw-r--r--  2.0 unx     4697 b- defN 22-Dec-02 13:07 towhee/hub/operator_manager.py
--rw-r--r--  2.0 unx     3755 b- defN 22-Dec-02 13:07 towhee/hub/pipeline_manager.py
--rw-r--r--  2.0 unx    10277 b- defN 22-Dec-02 13:07 towhee/hub/repo_manager.py
--rw-r--r--  2.0 unx      592 b- defN 22-Dec-02 13:07 towhee/hub/builtin/__init__.py
--rw-r--r--  2.0 unx      592 b- defN 22-Dec-02 13:07 towhee/hub/builtin/operators/__init__.py
--rw-r--r--  2.0 unx     7046 b- defN 22-Dec-02 13:07 towhee/hub/builtin/operators/computer_vision.py
--rw-r--r--  2.0 unx     2651 b- defN 22-Dec-02 13:07 towhee/hub/builtin/operators/faiss_search.py
--rw-r--r--  2.0 unx     3972 b- defN 22-Dec-02 13:07 towhee/hub/builtin/operators/feature_engineer.py
--rw-r--r--  2.0 unx     4389 b- defN 22-Dec-02 13:07 towhee/hub/builtin/operators/milvus_search.py
--rw-r--r--  2.0 unx     1445 b- defN 22-Dec-02 13:07 towhee/hub/builtin/operators/runas_op.py
--rw-r--r--  2.0 unx     3511 b- defN 22-Dec-02 13:07 towhee/hub/builtin/operators/sklearn.py
--rw-r--r--  2.0 unx     7833 b- defN 22-Dec-02 13:07 towhee/hub/builtin/operators/tensor_like.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-02 13:07 towhee/hub/builtin/pipelines/__init__.py
--rw-r--r--  2.0 unx      934 b- defN 22-Dec-02 13:07 towhee/hub/preclude/__init__.py
--rw-r--r--  2.0 unx      860 b- defN 22-Dec-02 13:07 towhee/operator/__init__.py
--rw-r--r--  2.0 unx     8062 b- defN 22-Dec-02 13:07 towhee/operator/base.py
--rw-r--r--  2.0 unx     2031 b- defN 22-Dec-02 13:07 towhee/operator/concat_operator.py
--rw-r--r--  2.0 unx     1444 b- defN 22-Dec-02 13:07 towhee/operator/nop.py
--rw-r--r--  2.0 unx     3031 b- defN 22-Dec-02 13:07 towhee/operator/stateful_operator.py
--rw-r--r--  2.0 unx      786 b- defN 22-Dec-02 13:07 towhee/runtime/__init__.py
--rw-r--r--  2.0 unx     4235 b- defN 22-Dec-02 13:07 towhee/runtime/check_utils.py
--rw-r--r--  2.0 unx     1413 b- defN 22-Dec-02 13:07 towhee/runtime/constants.py
--rw-r--r--  2.0 unx    12372 b- defN 22-Dec-02 13:07 towhee/runtime/dag_repr.py
--rw-r--r--  2.0 unx     8990 b- defN 22-Dec-02 13:07 towhee/runtime/data_queue.py
--rw-r--r--  2.0 unx     3571 b- defN 22-Dec-02 13:07 towhee/runtime/factory.py
--rw-r--r--  2.0 unx     2467 b- defN 22-Dec-02 13:07 towhee/runtime/node_config.py
--rw-r--r--  2.0 unx     7149 b- defN 22-Dec-02 13:07 towhee/runtime/node_repr.py
--rw-r--r--  2.0 unx    12519 b- defN 22-Dec-02 13:07 towhee/runtime/performance_profiler.py
--rw-r--r--  2.0 unx    16897 b- defN 22-Dec-02 13:07 towhee/runtime/pipeline.py
--rw-r--r--  2.0 unx     2484 b- defN 22-Dec-02 13:07 towhee/runtime/runtime_conf.py
--rw-r--r--  2.0 unx     5381 b- defN 22-Dec-02 13:07 towhee/runtime/runtime_pipeline.py
--rw-r--r--  2.0 unx     2229 b- defN 22-Dec-02 13:07 towhee/runtime/schema_repr.py
--rw-r--r--  2.0 unx     2572 b- defN 22-Dec-02 13:07 towhee/runtime/nodes/__init__.py
--rw-r--r--  2.0 unx     2377 b- defN 22-Dec-02 13:07 towhee/runtime/nodes/_concat.py
--rw-r--r--  2.0 unx     2739 b- defN 22-Dec-02 13:07 towhee/runtime/nodes/_filter.py
--rw-r--r--  2.0 unx     2511 b- defN 22-Dec-02 13:07 towhee/runtime/nodes/_flat_map.py
--rw-r--r--  2.0 unx     3136 b- defN 22-Dec-02 13:07 towhee/runtime/nodes/_map.py
--rw-r--r--  2.0 unx     1496 b- defN 22-Dec-02 13:07 towhee/runtime/nodes/_output.py
--rw-r--r--  2.0 unx     4331 b- defN 22-Dec-02 13:07 towhee/runtime/nodes/_time_window.py
--rw-r--r--  2.0 unx     5677 b- defN 22-Dec-02 13:07 towhee/runtime/nodes/_window.py
--rw-r--r--  2.0 unx     3222 b- defN 22-Dec-02 13:07 towhee/runtime/nodes/_window_all.py
--rw-r--r--  2.0 unx     6165 b- defN 22-Dec-02 13:07 towhee/runtime/nodes/node.py
--rw-r--r--  2.0 unx      872 b- defN 22-Dec-02 13:07 towhee/runtime/operator_manager/__init__.py
--rw-r--r--  2.0 unx     3016 b- defN 22-Dec-02 13:07 towhee/runtime/operator_manager/operator_action.py
--rw-r--r--  2.0 unx     6999 b- defN 22-Dec-02 13:07 towhee/runtime/operator_manager/operator_loader.py
--rw-r--r--  2.0 unx     3634 b- defN 22-Dec-02 13:07 towhee/runtime/operator_manager/operator_pool.py
--rw-r--r--  2.0 unx     2604 b- defN 22-Dec-02 13:07 towhee/runtime/operator_manager/operator_registry.py
--rw-r--r--  2.0 unx     1951 b- defN 22-Dec-02 13:07 towhee/runtime/operator_manager/uri.py
--rw-r--r--  2.0 unx      592 b- defN 22-Dec-02 13:07 towhee/serve/__init__.py
--rw-r--r--  2.0 unx      592 b- defN 22-Dec-02 13:07 towhee/serve/triton/__init__.py
--rw-r--r--  2.0 unx     7938 b- defN 22-Dec-02 13:07 towhee/serve/triton/builder.py
--rw-r--r--  2.0 unx     9988 b- defN 22-Dec-02 13:07 towhee/serve/triton/client.py
--rw-r--r--  2.0 unx      873 b- defN 22-Dec-02 13:07 towhee/serve/triton/constant.py
--rw-r--r--  2.0 unx     1956 b- defN 22-Dec-02 13:07 towhee/serve/triton/docker_image_builder.py
--rw-r--r--  2.0 unx     1065 b- defN 22-Dec-02 13:07 towhee/serve/triton/format_utils.py
--rw-r--r--  2.0 unx    15555 b- defN 22-Dec-02 13:07 towhee/serve/triton/python_model_builder.py
--rw-r--r--  2.0 unx    10800 b- defN 22-Dec-02 13:07 towhee/serve/triton/to_triton_models.py
--rw-r--r--  2.0 unx     8977 b- defN 22-Dec-02 13:07 towhee/serve/triton/triton_config_builder.py
--rw-r--r--  2.0 unx    15914 b- defN 22-Dec-02 13:07 towhee/serve/triton/type_gen.py
--rw-r--r--  2.0 unx      592 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/__init__.py
--rw-r--r--  2.0 unx      934 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/python_backend_wrapper.py
--rw-r--r--  2.0 unx      592 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/caller/__init__.py
--rw-r--r--  2.0 unx     3437 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/caller/local_caller.py
--rw-r--r--  2.0 unx      592 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/mock/__init__.py
--rw-r--r--  2.0 unx     3046 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/mock/mock_pb_util.py
--rw-r--r--  2.0 unx     2755 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/mock/mock_triton_client.py
--rw-r--r--  2.0 unx      592 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/model_runner/__init__.py
--rw-r--r--  2.0 unx     3124 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/model_runner/generator_model.py
--rw-r--r--  2.0 unx     2386 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/model_runner/map_model.py
--rw-r--r--  2.0 unx     4000 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/model_runner/transformer.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/utils/__init__.py
--rw-r--r--  2.0 unx     1482 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/utils/op_config.py
--rw-r--r--  2.0 unx     4294 b- defN 22-Dec-02 13:07 towhee/serve/triton/bls/utils/type_util.py
--rw-r--r--  2.0 unx     1065 b- defN 22-Dec-02 13:07 towhee/serve/triton/dockerfiles/DockerfileCuda113
--rw-r--r--  2.0 unx     1062 b- defN 22-Dec-02 13:07 towhee/serve/triton/dockerfiles/DockerfileCuda114
--rw-r--r--  2.0 unx     1402 b- defN 22-Dec-02 13:07 towhee/serve/triton/dockerfiles/DockerfileCuda114dev
--rw-r--r--  2.0 unx     1062 b- defN 22-Dec-02 13:07 towhee/serve/triton/dockerfiles/DockerfileCuda116
--rw-r--r--  2.0 unx     1235 b- defN 22-Dec-02 13:07 towhee/serve/triton/dockerfiles/__init__.py
--rw-r--r--  2.0 unx      886 b- defN 22-Dec-02 13:07 towhee/trainer/__init__.py
--rw-r--r--  2.0 unx    26505 b- defN 22-Dec-02 13:07 towhee/trainer/callback.py
--rw-r--r--  2.0 unx    10630 b- defN 22-Dec-02 13:07 towhee/trainer/metrics.py
--rw-r--r--  2.0 unx     8861 b- defN 22-Dec-02 13:07 towhee/trainer/modelcard.py
--rw-r--r--  2.0 unx    14904 b- defN 22-Dec-02 13:07 towhee/trainer/scheduler.py
--rw-r--r--  2.0 unx    39466 b- defN 22-Dec-02 13:07 towhee/trainer/trainer.py
--rw-r--r--  2.0 unx    14431 b- defN 22-Dec-02 13:07 towhee/trainer/training_config.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-02 13:07 towhee/trainer/optimization/__init__.py
--rw-r--r--  2.0 unx     7830 b- defN 22-Dec-02 13:07 towhee/trainer/optimization/adafactor.py
--rw-r--r--  2.0 unx     5148 b- defN 22-Dec-02 13:07 towhee/trainer/optimization/adamw.py
--rw-r--r--  2.0 unx    12006 b- defN 22-Dec-02 13:07 towhee/trainer/optimization/optimization.py
--rw-r--r--  2.0 unx      592 b- defN 22-Dec-02 13:07 towhee/trainer/utils/__init__.py
--rw-r--r--  2.0 unx      970 b- defN 22-Dec-02 13:07 towhee/trainer/utils/file_utils.py
--rw-r--r--  2.0 unx     5007 b- defN 22-Dec-02 13:07 towhee/trainer/utils/layer_freezer.py
--rw-r--r--  2.0 unx    16453 b- defN 22-Dec-02 13:07 towhee/trainer/utils/plot_utils.py
--rw-r--r--  2.0 unx     9017 b- defN 22-Dec-02 13:07 towhee/trainer/utils/trainer_utils.py
--rw-r--r--  2.0 unx     1343 b- defN 22-Dec-02 13:07 towhee/types/__init__.py
--rw-r--r--  2.0 unx     4586 b- defN 22-Dec-02 13:07 towhee/types/_frame.py
--rw-r--r--  2.0 unx     2341 b- defN 22-Dec-02 13:07 towhee/types/arg.py
--rw-r--r--  2.0 unx     2141 b- defN 22-Dec-02 13:07 towhee/types/audio_frame.py
--rw-r--r--  2.0 unx     2443 b- defN 22-Dec-02 13:07 towhee/types/image.py
--rw-r--r--  2.0 unx     2016 b- defN 22-Dec-02 13:07 towhee/types/image_utils.py
--rw-r--r--  2.0 unx     5261 b- defN 22-Dec-02 13:07 towhee/types/tensor_array.py
--rw-r--r--  2.0 unx     2649 b- defN 22-Dec-02 13:07 towhee/types/video_frame.py
--rw-r--r--  2.0 unx      592 b- defN 22-Dec-02 13:07 towhee/utils/__init__.py
--rw-r--r--  2.0 unx     1178 b- defN 22-Dec-02 13:07 towhee/utils/cv2_utils.py
--rw-r--r--  2.0 unx     1527 b- defN 22-Dec-02 13:07 towhee/utils/dependency_control.py
--rw-r--r--  2.0 unx     7744 b- defN 22-Dec-02 13:07 towhee/utils/git_utils.py
--rw-r--r--  2.0 unx     1381 b- defN 22-Dec-02 13:07 towhee/utils/hub_file_utils.py
--rw-r--r--  2.0 unx    12654 b- defN 22-Dec-02 13:07 towhee/utils/hub_utils.py
--rw-r--r--  2.0 unx     1266 b- defN 22-Dec-02 13:07 towhee/utils/jit_utils.py
--rw-r--r--  2.0 unx      894 b- defN 22-Dec-02 13:07 towhee/utils/log.py
--rw-r--r--  2.0 unx     2975 b- defN 22-Dec-02 13:07 towhee/utils/matplotlib_utils.py
--rw-r--r--  2.0 unx     4385 b- defN 22-Dec-02 13:07 towhee/utils/ndarray_utils.py
--rw-r--r--  2.0 unx     3034 b- defN 22-Dec-02 13:07 towhee/utils/np_format.py
--rw-r--r--  2.0 unx     2571 b- defN 22-Dec-02 13:07 towhee/utils/pil_utils.py
--rw-r--r--  2.0 unx     8448 b- defN 22-Dec-02 13:07 towhee/utils/repo_normalize.py
--rw-r--r--  2.0 unx     1186 b- defN 22-Dec-02 13:07 towhee/utils/scipy_utils.py
--rw-r--r--  2.0 unx     1102 b- defN 22-Dec-02 13:07 towhee/utils/singleton.py
--rw-r--r--  2.0 unx     1877 b- defN 22-Dec-02 13:07 towhee/utils/sklearn_utils.py
--rw-r--r--  2.0 unx     1519 b- defN 22-Dec-02 13:07 towhee/utils/tritonclient_utils.py
--rw-r--r--  2.0 unx     2535 b- defN 22-Dec-02 13:07 towhee/utils/yaml_utils.py
--rw-r--r--  2.0 unx      592 b- defN 22-Dec-02 13:07 towhee/utils/thirdparty/__init__.py
--rw-r--r--  2.0 unx      839 b- defN 22-Dec-02 13:07 towhee/utils/thirdparty/av_utils.py
--rw-r--r--  2.0 unx     1123 b- defN 22-Dec-02 13:07 towhee/utils/thirdparty/boto3_utils.py
--rw-r--r--  2.0 unx     1893 b- defN 22-Dec-02 13:07 towhee/utils/thirdparty/faiss_utils.py
--rw-r--r--  2.0 unx     1230 b- defN 22-Dec-02 13:07 towhee/utils/thirdparty/ipython_utils.py
--rw-r--r--  2.0 unx     1470 b- defN 22-Dec-02 13:07 towhee/utils/thirdparty/milvus_utils.py
--rw-r--r--  2.0 unx     1154 b- defN 22-Dec-02 13:07 towhee/utils/thirdparty/numba_utils.py
--rw-r--r--  2.0 unx     1130 b- defN 22-Dec-02 13:07 towhee/utils/thirdparty/pandas_utils.py
--rw-r--r--  2.0 unx     1130 b- defN 22-Dec-02 13:07 towhee/utils/thirdparty/plyvel_utils.py
--rw-r--r--  2.0 unx      866 b- defN 22-Dec-02 13:07 towhee/utils/thirdparty/pyarrow_utils.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Dec-02 13:25 towhee-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    13924 b- defN 22-Dec-02 13:25 towhee-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-02 13:25 towhee-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      105 b- defN 22-Dec-02 13:25 towhee-0.9.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 22-Dec-02 13:25 towhee-0.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    21231 b- defN 22-Dec-02 13:25 towhee-0.9.0.dist-info/RECORD
-236 files, 1101052 bytes uncompressed, 328445 bytes compressed:  70.2%
+Zip file size: 207434 bytes, number of entries: 144
+-rw-r--r--  2.0 unx     2855 b- defN 23-Mar-21 08:26 towhee/__init__.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Mar-21 08:26 towhee/__main__.py
+-rw-r--r--  2.0 unx      619 b- defN 23-Mar-21 08:26 towhee/command/__init__.py
+-rw-r--r--  2.0 unx     1627 b- defN 23-Mar-21 08:26 towhee/command/cmdline.py
+-rw-r--r--  2.0 unx     4668 b- defN 23-Mar-21 08:26 towhee/command/develop.py
+-rw-r--r--  2.0 unx     4223 b- defN 23-Mar-21 08:26 towhee/command/execute.py
+-rw-r--r--  2.0 unx     4908 b- defN 23-Mar-21 08:26 towhee/command/repo.py
+-rw-r--r--  2.0 unx     5240 b- defN 23-Mar-21 08:26 towhee/command/user.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-21 08:26 towhee/data/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-21 08:26 towhee/data/dataset/__init__.py
+-rw-r--r--  2.0 unx      662 b- defN 23-Mar-21 08:26 towhee/data/dataset/dataset.py
+-rw-r--r--  2.0 unx     2918 b- defN 23-Mar-21 08:26 towhee/data/dataset/image_datasets.py
+-rw-r--r--  2.0 unx      714 b- defN 23-Mar-21 08:26 towhee/datacollection/__init__.py
+-rw-r--r--  2.0 unx     7581 b- defN 23-Mar-21 08:26 towhee/datacollection/data_collection.py
+-rw-r--r--  2.0 unx     3448 b- defN 23-Mar-21 08:26 towhee/datacollection/entity.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Mar-21 08:26 towhee/datacollection/mixins/__init__.py
+-rw-r--r--  2.0 unx    11315 b- defN 23-Mar-21 08:26 towhee/datacollection/mixins/display.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Mar-21 08:26 towhee/hub/__init__.py
+-rw-r--r--  2.0 unx     3201 b- defN 23-Mar-21 08:26 towhee/hub/cache_manager.py
+-rw-r--r--  2.0 unx     5748 b- defN 23-Apr-27 08:00 towhee/hub/downloader.py
+-rw-r--r--  2.0 unx     4697 b- defN 23-Mar-21 08:26 towhee/hub/operator_manager.py
+-rw-r--r--  2.0 unx     3755 b- defN 23-Mar-21 08:26 towhee/hub/pipeline_manager.py
+-rw-r--r--  2.0 unx    10289 b- defN 23-Mar-21 08:26 towhee/hub/repo_manager.py
+-rw-r--r--  2.0 unx      777 b- defN 23-Mar-21 08:26 towhee/operator/__init__.py
+-rw-r--r--  2.0 unx     7758 b- defN 23-Mar-21 08:26 towhee/operator/base.py
+-rw-r--r--  2.0 unx     2031 b- defN 23-Mar-21 08:26 towhee/operator/concat_operator.py
+-rw-r--r--  2.0 unx     1444 b- defN 23-Mar-21 08:26 towhee/operator/nop.py
+-rw-r--r--  2.0 unx      975 b- defN 23-Mar-21 08:26 towhee/pipelines/__init__.py
+-rw-r--r--  2.0 unx      947 b- defN 23-Mar-21 08:26 towhee/pipelines/_builtin_pipeline.py
+-rw-r--r--  2.0 unx     1471 b- defN 23-Mar-21 08:26 towhee/pipelines/insert_milvus.py
+-rw-r--r--  2.0 unx     1548 b- defN 23-Mar-21 08:26 towhee/pipelines/search_milvus.py
+-rw-r--r--  2.0 unx     2871 b- defN 23-Mar-21 08:26 towhee/pipelines/sentence_embedding.py
+-rw-r--r--  2.0 unx     2306 b- defN 23-Mar-21 08:26 towhee/pipelines/text_image_embedding.py
+-rw-r--r--  2.0 unx     6886 b- defN 23-Mar-21 08:26 towhee/pipelines/video_copy_detection.py
+-rw-r--r--  2.0 unx     4850 b- defN 23-Mar-21 08:26 towhee/pipelines/video_embedding.py
+-rw-r--r--  2.0 unx     1003 b- defN 23-Mar-21 08:26 towhee/runtime/__init__.py
+-rw-r--r--  2.0 unx     8984 b- defN 23-Mar-21 08:26 towhee/runtime/auto_config.py
+-rw-r--r--  2.0 unx     2280 b- defN 23-Mar-21 08:26 towhee/runtime/auto_pipes.py
+-rw-r--r--  2.0 unx     5091 b- defN 23-Mar-21 08:26 towhee/runtime/check_utils.py
+-rw-r--r--  2.0 unx     1413 b- defN 23-Mar-21 08:26 towhee/runtime/constants.py
+-rw-r--r--  2.0 unx    13063 b- defN 23-Mar-21 08:26 towhee/runtime/dag_repr.py
+-rw-r--r--  2.0 unx     9260 b- defN 23-Mar-21 08:26 towhee/runtime/data_queue.py
+-rw-r--r--  2.0 unx     3571 b- defN 23-Mar-21 08:26 towhee/runtime/factory.py
+-rw-r--r--  2.0 unx     6619 b- defN 23-Mar-21 08:26 towhee/runtime/node_config.py
+-rw-r--r--  2.0 unx     7149 b- defN 23-Mar-21 08:26 towhee/runtime/node_repr.py
+-rw-r--r--  2.0 unx    12539 b- defN 23-Mar-21 08:26 towhee/runtime/performance_profiler.py
+-rw-r--r--  2.0 unx    16957 b- defN 23-Mar-21 08:26 towhee/runtime/pipeline.py
+-rw-r--r--  2.0 unx     2018 b- defN 23-Mar-21 08:26 towhee/runtime/pipeline_loader.py
+-rw-r--r--  2.0 unx     2821 b- defN 23-Mar-21 08:26 towhee/runtime/runtime_conf.py
+-rw-r--r--  2.0 unx     6648 b- defN 23-Mar-21 08:26 towhee/runtime/runtime_pipeline.py
+-rw-r--r--  2.0 unx     2335 b- defN 23-Mar-21 08:26 towhee/runtime/schema_repr.py
+-rw-r--r--  2.0 unx     2572 b- defN 23-Mar-21 08:26 towhee/runtime/nodes/__init__.py
+-rw-r--r--  2.0 unx     2377 b- defN 23-Mar-21 08:26 towhee/runtime/nodes/_concat.py
+-rw-r--r--  2.0 unx     2722 b- defN 23-Mar-21 08:26 towhee/runtime/nodes/_filter.py
+-rw-r--r--  2.0 unx     2879 b- defN 23-Mar-21 08:26 towhee/runtime/nodes/_flat_map.py
+-rw-r--r--  2.0 unx     3551 b- defN 23-Mar-21 08:26 towhee/runtime/nodes/_map.py
+-rw-r--r--  2.0 unx     1630 b- defN 23-Mar-21 08:26 towhee/runtime/nodes/_output.py
+-rw-r--r--  2.0 unx     4481 b- defN 23-Mar-21 08:26 towhee/runtime/nodes/_time_window.py
+-rw-r--r--  2.0 unx     5737 b- defN 23-Mar-21 08:26 towhee/runtime/nodes/_window.py
+-rw-r--r--  2.0 unx     3310 b- defN 23-Mar-21 08:26 towhee/runtime/nodes/_window_all.py
+-rw-r--r--  2.0 unx     6165 b- defN 23-Mar-21 08:26 towhee/runtime/nodes/node.py
+-rw-r--r--  2.0 unx      872 b- defN 23-Mar-21 08:26 towhee/runtime/operator_manager/__init__.py
+-rw-r--r--  2.0 unx     3016 b- defN 23-Mar-21 08:26 towhee/runtime/operator_manager/operator_action.py
+-rw-r--r--  2.0 unx     6478 b- defN 23-Mar-21 08:26 towhee/runtime/operator_manager/operator_loader.py
+-rw-r--r--  2.0 unx     3634 b- defN 23-Mar-21 08:26 towhee/runtime/operator_manager/operator_pool.py
+-rw-r--r--  2.0 unx     2867 b- defN 23-Mar-21 08:26 towhee/runtime/operator_manager/operator_registry.py
+-rw-r--r--  2.0 unx     1951 b- defN 23-Mar-21 08:26 towhee/runtime/operator_manager/uri.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Mar-21 08:26 towhee/serve/__init__.py
+-rw-r--r--  2.0 unx     2005 b- defN 23-Mar-21 08:26 towhee/serve/server_builder.py
+-rw-r--r--  2.0 unx      773 b- defN 23-Mar-21 08:26 towhee/serve/triton/__init__.py
+-rw-r--r--  2.0 unx      816 b- defN 23-Mar-21 08:26 towhee/serve/triton/constant.py
+-rw-r--r--  2.0 unx     2330 b- defN 23-Mar-21 08:26 towhee/serve/triton/docker_image_builder.py
+-rw-r--r--  2.0 unx     4500 b- defN 23-Apr-27 08:00 towhee/serve/triton/model_to_triton.py
+-rw-r--r--  2.0 unx     3483 b- defN 23-Apr-27 08:00 towhee/serve/triton/pipe_to_triton.py
+-rw-r--r--  2.0 unx     4286 b- defN 23-Mar-21 08:26 towhee/serve/triton/pipeline_builder.py
+-rw-r--r--  2.0 unx     4051 b- defN 23-Mar-21 08:26 towhee/serve/triton/pipeline_client.py
+-rw-r--r--  2.0 unx     1729 b- defN 23-Mar-21 08:26 towhee/serve/triton/serializer.py
+-rw-r--r--  2.0 unx     2408 b- defN 23-Mar-21 08:26 towhee/serve/triton/triton_client.py
+-rw-r--r--  2.0 unx     2547 b- defN 23-Mar-21 08:26 towhee/serve/triton/triton_config_builder.py
+-rw-r--r--  2.0 unx     1499 b- defN 23-Mar-21 08:26 towhee/serve/triton/triton_files.py
+-rw-r--r--  2.0 unx      706 b- defN 23-Mar-21 08:26 towhee/serve/triton/bls/__init__.py
+-rw-r--r--  2.0 unx     2228 b- defN 23-Mar-21 08:26 towhee/serve/triton/bls/pipeline_model.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Mar-21 08:26 towhee/serve/triton/bls/python_backend_wrapper.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Mar-21 08:26 towhee/serve/triton/bls/caller/__init__.py
+-rw-r--r--  2.0 unx     3437 b- defN 23-Mar-21 08:26 towhee/serve/triton/bls/caller/local_caller.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Mar-21 08:26 towhee/serve/triton/bls/mock/__init__.py
+-rw-r--r--  2.0 unx     4727 b- defN 23-Mar-21 08:26 towhee/serve/triton/bls/mock/mock_pb_util.py
+-rw-r--r--  2.0 unx     2699 b- defN 23-Mar-21 08:26 towhee/serve/triton/bls/mock/mock_triton_client.py
+-rw-r--r--  2.0 unx      750 b- defN 23-Apr-27 08:00 towhee/serve/triton/dockerfiles/DockerfileCuda113
+-rw-r--r--  2.0 unx      748 b- defN 23-Apr-27 08:00 towhee/serve/triton/dockerfiles/DockerfileCuda114
+-rw-r--r--  2.0 unx      748 b- defN 23-Apr-27 08:00 towhee/serve/triton/dockerfiles/DockerfileCuda116
+-rw-r--r--  2.0 unx      748 b- defN 23-Apr-27 08:00 towhee/serve/triton/dockerfiles/DockerfileCuda117
+-rw-r--r--  2.0 unx      956 b- defN 23-Apr-27 08:00 towhee/serve/triton/dockerfiles/DockerfileCuda117dev
+-rw-r--r--  2.0 unx     1317 b- defN 23-Mar-21 08:26 towhee/serve/triton/dockerfiles/__init__.py
+-rw-r--r--  2.0 unx      940 b- defN 23-Mar-21 08:26 towhee/trainer/__init__.py
+-rw-r--r--  2.0 unx    26591 b- defN 23-Mar-21 08:26 towhee/trainer/callback.py
+-rw-r--r--  2.0 unx    10668 b- defN 23-Mar-21 08:26 towhee/trainer/metrics.py
+-rw-r--r--  2.0 unx     8861 b- defN 23-Mar-21 08:26 towhee/trainer/modelcard.py
+-rw-r--r--  2.0 unx    14904 b- defN 23-Mar-21 08:26 towhee/trainer/scheduler.py
+-rw-r--r--  2.0 unx    34675 b- defN 23-Mar-21 08:26 towhee/trainer/trainer.py
+-rw-r--r--  2.0 unx    14667 b- defN 23-Mar-21 08:26 towhee/trainer/training_config.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-21 08:26 towhee/trainer/optimization/__init__.py
+-rw-r--r--  2.0 unx     7830 b- defN 23-Mar-21 08:26 towhee/trainer/optimization/adafactor.py
+-rw-r--r--  2.0 unx     5148 b- defN 23-Mar-21 08:26 towhee/trainer/optimization/adamw.py
+-rw-r--r--  2.0 unx    12006 b- defN 23-Mar-21 08:26 towhee/trainer/optimization/optimization.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Mar-21 08:26 towhee/trainer/utils/__init__.py
+-rw-r--r--  2.0 unx      970 b- defN 23-Mar-21 08:26 towhee/trainer/utils/file_utils.py
+-rw-r--r--  2.0 unx     5007 b- defN 23-Mar-21 08:26 towhee/trainer/utils/layer_freezer.py
+-rw-r--r--  2.0 unx    16453 b- defN 23-Mar-21 08:26 towhee/trainer/utils/plot_utils.py
+-rw-r--r--  2.0 unx     9017 b- defN 23-Mar-21 08:26 towhee/trainer/utils/trainer_utils.py
+-rw-r--r--  2.0 unx      872 b- defN 23-Mar-21 08:26 towhee/types/__init__.py
+-rw-r--r--  2.0 unx     2341 b- defN 23-Mar-21 08:26 towhee/types/arg.py
+-rw-r--r--  2.0 unx     2141 b- defN 23-Mar-21 08:26 towhee/types/audio_frame.py
+-rw-r--r--  2.0 unx     2443 b- defN 23-Mar-21 08:26 towhee/types/image.py
+-rw-r--r--  2.0 unx     2016 b- defN 23-Mar-21 08:26 towhee/types/image_utils.py
+-rw-r--r--  2.0 unx     2649 b- defN 23-Mar-21 08:26 towhee/types/video_frame.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Mar-21 08:26 towhee/utils/__init__.py
+-rw-r--r--  2.0 unx     1178 b- defN 23-Mar-21 08:26 towhee/utils/cv2_utils.py
+-rw-r--r--  2.0 unx     1403 b- defN 23-Mar-21 08:26 towhee/utils/dependency_control.py
+-rw-r--r--  2.0 unx      829 b- defN 23-Mar-21 08:26 towhee/utils/empty_format.py
+-rw-r--r--  2.0 unx     7744 b- defN 23-Mar-21 08:26 towhee/utils/git_utils.py
+-rw-r--r--  2.0 unx     1381 b- defN 23-Mar-21 08:26 towhee/utils/hub_file_utils.py
+-rw-r--r--  2.0 unx    13148 b- defN 23-Mar-21 08:26 towhee/utils/hub_utils.py
+-rw-r--r--  2.0 unx     1301 b- defN 23-Mar-21 08:26 towhee/utils/lazy_import.py
+-rw-r--r--  2.0 unx      894 b- defN 23-Mar-21 08:26 towhee/utils/log.py
+-rw-r--r--  2.0 unx     2975 b- defN 23-Mar-21 08:26 towhee/utils/matplotlib_utils.py
+-rw-r--r--  2.0 unx     4385 b- defN 23-Mar-21 08:26 towhee/utils/ndarray_utils.py
+-rw-r--r--  2.0 unx     2414 b- defN 23-Mar-21 08:26 towhee/utils/np_format.py
+-rw-r--r--  2.0 unx     1156 b- defN 23-Mar-21 08:26 towhee/utils/onnx_utils.py
+-rw-r--r--  2.0 unx     2571 b- defN 23-Mar-21 08:26 towhee/utils/pil_utils.py
+-rw-r--r--  2.0 unx     8448 b- defN 23-Mar-21 08:26 towhee/utils/repo_normalize.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-Mar-21 08:26 towhee/utils/singleton.py
+-rw-r--r--  2.0 unx     1538 b- defN 23-Mar-21 08:26 towhee/utils/triton_httpclient.py
+-rw-r--r--  2.0 unx     2535 b- defN 23-Mar-21 08:26 towhee/utils/yaml_utils.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Mar-21 08:26 towhee/utils/thirdparty/__init__.py
+-rw-r--r--  2.0 unx      845 b- defN 23-Mar-21 08:26 towhee/utils/thirdparty/dill_util.py
+-rw-r--r--  2.0 unx     1230 b- defN 23-Mar-21 08:26 towhee/utils/thirdparty/ipython_utils.py
+-rw-r--r--  2.0 unx     1130 b- defN 23-Mar-21 08:26 towhee/utils/thirdparty/pandas_utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17248 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      114 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    12830 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/RECORD
+144 files, 604582 bytes uncompressed, 187054 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,28 +1,13 @@
 Filename: towhee/__init__.py
 Comment: 
 
 Filename: towhee/__main__.py
 Comment: 
 
-Filename: towhee/dc2.py
-Comment: 
-
-Filename: towhee/errors.py
-Comment: 
-
-Filename: towhee/pipeline_format.py
-Comment: 
-
-Filename: towhee/_types/__init__.py
-Comment: 
-
-Filename: towhee/_types/image.py
-Comment: 
-
 Filename: towhee/command/__init__.py
 Comment: 
 
 Filename: towhee/command/cmdline.py
 Comment: 
 
 Filename: towhee/command/develop.py
@@ -30,41 +15,17 @@
 
 Filename: towhee/command/execute.py
 Comment: 
 
 Filename: towhee/command/repo.py
 Comment: 
 
-Filename: towhee/command/s3.py
-Comment: 
-
 Filename: towhee/command/user.py
 Comment: 
 
-Filename: towhee/dag/__init__.py
-Comment: 
-
-Filename: towhee/dag/base_repr.py
-Comment: 
-
-Filename: towhee/dag/dataframe_repr.py
-Comment: 
-
-Filename: towhee/dag/graph_builder.py
-Comment: 
-
-Filename: towhee/dag/graph_repr.py
-Comment: 
-
-Filename: towhee/dag/operator_repr.py
-Comment: 
-
-Filename: towhee/dag/variable_repr.py
-Comment: 
-
 Filename: towhee/data/__init__.py
 Comment: 
 
 Filename: towhee/data/dataset/__init__.py
 Comment: 
 
 Filename: towhee/data/dataset/dataset.py
@@ -84,282 +45,75 @@
 
 Filename: towhee/datacollection/mixins/__init__.py
 Comment: 
 
 Filename: towhee/datacollection/mixins/display.py
 Comment: 
 
-Filename: towhee/dataframe/__init__.py
-Comment: 
-
-Filename: towhee/dataframe/_schema.py
-Comment: 
-
-Filename: towhee/dataframe/dataframe.py
-Comment: 
-
-Filename: towhee/dataframe/iterators.py
-Comment: 
-
-Filename: towhee/dataframe/array/__init__.py
-Comment: 
-
-Filename: towhee/dataframe/array/array.py
-Comment: 
-
-Filename: towhee/dataframe/array/utils.py
-Comment: 
-
-Filename: towhee/engine/__init__.py
-Comment: 
-
-Filename: towhee/engine/engine.py
-Comment: 
-
-Filename: towhee/engine/factory.py
-Comment: 
-
-Filename: towhee/engine/graph_context.py
-Comment: 
-
-Filename: towhee/engine/operator_context.py
-Comment: 
-
-Filename: towhee/engine/operator_loader.py
-Comment: 
-
-Filename: towhee/engine/operator_pool.py
-Comment: 
-
-Filename: towhee/engine/operator_registry.py
-Comment: 
-
-Filename: towhee/engine/pipeline.py
-Comment: 
-
-Filename: towhee/engine/status.py
-Comment: 
-
-Filename: towhee/engine/task_scheduler.py
-Comment: 
-
-Filename: towhee/engine/thread_pool_task_executor.py
-Comment: 
-
-Filename: towhee/engine/uri.py
-Comment: 
-
-Filename: towhee/engine/execution/__init__.py
-Comment: 
-
-Filename: towhee/engine/execution/base_execution.py
-Comment: 
-
-Filename: towhee/engine/execution/pandas_execution.py
-Comment: 
-
-Filename: towhee/engine/execution/stateful_execution.py
-Comment: 
-
-Filename: towhee/engine/execution/vectorized_execution.py
-Comment: 
-
-Filename: towhee/engine/operator_io/__init__.py
-Comment: 
-
-Filename: towhee/engine/operator_io/_mock_reader.py
-Comment: 
-
-Filename: towhee/engine/operator_io/reader.py
-Comment: 
-
-Filename: towhee/engine/operator_io/writer.py
-Comment: 
-
-Filename: towhee/engine/operator_runner/__init__.py
-Comment: 
-
-Filename: towhee/engine/operator_runner/concat_runner.py
-Comment: 
-
-Filename: towhee/engine/operator_runner/filter_runner.py
-Comment: 
-
-Filename: towhee/engine/operator_runner/flatmap_runner.py
-Comment: 
-
-Filename: towhee/engine/operator_runner/generator_runner.py
-Comment: 
-
-Filename: towhee/engine/operator_runner/map_runner.py
-Comment: 
-
-Filename: towhee/engine/operator_runner/runner_base.py
-Comment: 
-
-Filename: towhee/engine/operator_runner/window_runner.py
-Comment: 
-
-Filename: towhee/functional/__init__.py
-Comment: 
-
-Filename: towhee/functional/data_collection.py
-Comment: 
-
-Filename: towhee/functional/entity.py
-Comment: 
-
-Filename: towhee/functional/option.py
-Comment: 
-
-Filename: towhee/functional/storages.py
-Comment: 
-
-Filename: towhee/functional/mixins/__init__.py
-Comment: 
-
-Filename: towhee/functional/mixins/audio.py
-Comment: 
-
-Filename: towhee/functional/mixins/column.py
-Comment: 
-
-Filename: towhee/functional/mixins/compile.py
-Comment: 
-
-Filename: towhee/functional/mixins/computer_vision.py
-Comment: 
-
-Filename: towhee/functional/mixins/config.py
-Comment: 
-
-Filename: towhee/functional/mixins/dag.py
-Comment: 
-
-Filename: towhee/functional/mixins/data_processing.py
-Comment: 
-
-Filename: towhee/functional/mixins/dataframe.py
-Comment: 
-
-Filename: towhee/functional/mixins/dataset.py
-Comment: 
-
-Filename: towhee/functional/mixins/dispatcher.py
-Comment: 
-
-Filename: towhee/functional/mixins/display.py
-Comment: 
-
-Filename: towhee/functional/mixins/faiss.py
-Comment: 
-
-Filename: towhee/functional/mixins/format_priority.py
-Comment: 
-
-Filename: towhee/functional/mixins/kv_storage.py
-Comment: 
-
-Filename: towhee/functional/mixins/list.py
-Comment: 
-
-Filename: towhee/functional/mixins/metric.py
-Comment: 
-
-Filename: towhee/functional/mixins/milvus.py
-Comment: 
-
-Filename: towhee/functional/mixins/parallel.py
-Comment: 
-
-Filename: towhee/functional/mixins/ray.py
-Comment: 
-
-Filename: towhee/functional/mixins/safe.py
-Comment: 
-
-Filename: towhee/functional/mixins/serve.py
-Comment: 
-
-Filename: towhee/functional/mixins/state.py
-Comment: 
-
-Filename: towhee/functional/mixins/stream.py
-Comment: 
-
-Filename: towhee/hparam/__init__.py
-Comment: 
-
-Filename: towhee/hparam/hyperparameter.py
+Filename: towhee/hub/__init__.py
 Comment: 
 
-Filename: towhee/hub/__init__.py
+Filename: towhee/hub/cache_manager.py
 Comment: 
 
-Filename: towhee/hub/file_manager.py
+Filename: towhee/hub/downloader.py
 Comment: 
 
 Filename: towhee/hub/operator_manager.py
 Comment: 
 
 Filename: towhee/hub/pipeline_manager.py
 Comment: 
 
 Filename: towhee/hub/repo_manager.py
 Comment: 
 
-Filename: towhee/hub/builtin/__init__.py
-Comment: 
-
-Filename: towhee/hub/builtin/operators/__init__.py
-Comment: 
-
-Filename: towhee/hub/builtin/operators/computer_vision.py
+Filename: towhee/operator/__init__.py
 Comment: 
 
-Filename: towhee/hub/builtin/operators/faiss_search.py
+Filename: towhee/operator/base.py
 Comment: 
 
-Filename: towhee/hub/builtin/operators/feature_engineer.py
+Filename: towhee/operator/concat_operator.py
 Comment: 
 
-Filename: towhee/hub/builtin/operators/milvus_search.py
+Filename: towhee/operator/nop.py
 Comment: 
 
-Filename: towhee/hub/builtin/operators/runas_op.py
+Filename: towhee/pipelines/__init__.py
 Comment: 
 
-Filename: towhee/hub/builtin/operators/sklearn.py
+Filename: towhee/pipelines/_builtin_pipeline.py
 Comment: 
 
-Filename: towhee/hub/builtin/operators/tensor_like.py
+Filename: towhee/pipelines/insert_milvus.py
 Comment: 
 
-Filename: towhee/hub/builtin/pipelines/__init__.py
+Filename: towhee/pipelines/search_milvus.py
 Comment: 
 
-Filename: towhee/hub/preclude/__init__.py
+Filename: towhee/pipelines/sentence_embedding.py
 Comment: 
 
-Filename: towhee/operator/__init__.py
+Filename: towhee/pipelines/text_image_embedding.py
 Comment: 
 
-Filename: towhee/operator/base.py
+Filename: towhee/pipelines/video_copy_detection.py
 Comment: 
 
-Filename: towhee/operator/concat_operator.py
+Filename: towhee/pipelines/video_embedding.py
 Comment: 
 
-Filename: towhee/operator/nop.py
+Filename: towhee/runtime/__init__.py
 Comment: 
 
-Filename: towhee/operator/stateful_operator.py
+Filename: towhee/runtime/auto_config.py
 Comment: 
 
-Filename: towhee/runtime/__init__.py
+Filename: towhee/runtime/auto_pipes.py
 Comment: 
 
 Filename: towhee/runtime/check_utils.py
 Comment: 
 
 Filename: towhee/runtime/constants.py
 Comment: 
@@ -381,14 +135,17 @@
 
 Filename: towhee/runtime/performance_profiler.py
 Comment: 
 
 Filename: towhee/runtime/pipeline.py
 Comment: 
 
+Filename: towhee/runtime/pipeline_loader.py
+Comment: 
+
 Filename: towhee/runtime/runtime_conf.py
 Comment: 
 
 Filename: towhee/runtime/runtime_pipeline.py
 Comment: 
 
 Filename: towhee/runtime/schema_repr.py
@@ -441,47 +198,56 @@
 
 Filename: towhee/runtime/operator_manager/uri.py
 Comment: 
 
 Filename: towhee/serve/__init__.py
 Comment: 
 
+Filename: towhee/serve/server_builder.py
+Comment: 
+
 Filename: towhee/serve/triton/__init__.py
 Comment: 
 
-Filename: towhee/serve/triton/builder.py
+Filename: towhee/serve/triton/constant.py
 Comment: 
 
-Filename: towhee/serve/triton/client.py
+Filename: towhee/serve/triton/docker_image_builder.py
 Comment: 
 
-Filename: towhee/serve/triton/constant.py
+Filename: towhee/serve/triton/model_to_triton.py
 Comment: 
 
-Filename: towhee/serve/triton/docker_image_builder.py
+Filename: towhee/serve/triton/pipe_to_triton.py
 Comment: 
 
-Filename: towhee/serve/triton/format_utils.py
+Filename: towhee/serve/triton/pipeline_builder.py
 Comment: 
 
-Filename: towhee/serve/triton/python_model_builder.py
+Filename: towhee/serve/triton/pipeline_client.py
 Comment: 
 
-Filename: towhee/serve/triton/to_triton_models.py
+Filename: towhee/serve/triton/serializer.py
+Comment: 
+
+Filename: towhee/serve/triton/triton_client.py
 Comment: 
 
 Filename: towhee/serve/triton/triton_config_builder.py
 Comment: 
 
-Filename: towhee/serve/triton/type_gen.py
+Filename: towhee/serve/triton/triton_files.py
 Comment: 
 
 Filename: towhee/serve/triton/bls/__init__.py
 Comment: 
 
+Filename: towhee/serve/triton/bls/pipeline_model.py
+Comment: 
+
 Filename: towhee/serve/triton/bls/python_backend_wrapper.py
 Comment: 
 
 Filename: towhee/serve/triton/bls/caller/__init__.py
 Comment: 
 
 Filename: towhee/serve/triton/bls/caller/local_caller.py
@@ -492,45 +258,27 @@
 
 Filename: towhee/serve/triton/bls/mock/mock_pb_util.py
 Comment: 
 
 Filename: towhee/serve/triton/bls/mock/mock_triton_client.py
 Comment: 
 
-Filename: towhee/serve/triton/bls/model_runner/__init__.py
-Comment: 
-
-Filename: towhee/serve/triton/bls/model_runner/generator_model.py
-Comment: 
-
-Filename: towhee/serve/triton/bls/model_runner/map_model.py
-Comment: 
-
-Filename: towhee/serve/triton/bls/model_runner/transformer.py
-Comment: 
-
-Filename: towhee/serve/triton/bls/utils/__init__.py
-Comment: 
-
-Filename: towhee/serve/triton/bls/utils/op_config.py
-Comment: 
-
-Filename: towhee/serve/triton/bls/utils/type_util.py
-Comment: 
-
 Filename: towhee/serve/triton/dockerfiles/DockerfileCuda113
 Comment: 
 
 Filename: towhee/serve/triton/dockerfiles/DockerfileCuda114
 Comment: 
 
-Filename: towhee/serve/triton/dockerfiles/DockerfileCuda114dev
+Filename: towhee/serve/triton/dockerfiles/DockerfileCuda116
 Comment: 
 
-Filename: towhee/serve/triton/dockerfiles/DockerfileCuda116
+Filename: towhee/serve/triton/dockerfiles/DockerfileCuda117
+Comment: 
+
+Filename: towhee/serve/triton/dockerfiles/DockerfileCuda117dev
 Comment: 
 
 Filename: towhee/serve/triton/dockerfiles/__init__.py
 Comment: 
 
 Filename: towhee/trainer/__init__.py
 Comment: 
@@ -579,131 +327,107 @@
 
 Filename: towhee/trainer/utils/trainer_utils.py
 Comment: 
 
 Filename: towhee/types/__init__.py
 Comment: 
 
-Filename: towhee/types/_frame.py
-Comment: 
-
 Filename: towhee/types/arg.py
 Comment: 
 
 Filename: towhee/types/audio_frame.py
 Comment: 
 
 Filename: towhee/types/image.py
 Comment: 
 
 Filename: towhee/types/image_utils.py
 Comment: 
 
-Filename: towhee/types/tensor_array.py
-Comment: 
-
 Filename: towhee/types/video_frame.py
 Comment: 
 
 Filename: towhee/utils/__init__.py
 Comment: 
 
 Filename: towhee/utils/cv2_utils.py
 Comment: 
 
 Filename: towhee/utils/dependency_control.py
 Comment: 
 
+Filename: towhee/utils/empty_format.py
+Comment: 
+
 Filename: towhee/utils/git_utils.py
 Comment: 
 
 Filename: towhee/utils/hub_file_utils.py
 Comment: 
 
 Filename: towhee/utils/hub_utils.py
 Comment: 
 
-Filename: towhee/utils/jit_utils.py
+Filename: towhee/utils/lazy_import.py
 Comment: 
 
 Filename: towhee/utils/log.py
 Comment: 
 
 Filename: towhee/utils/matplotlib_utils.py
 Comment: 
 
 Filename: towhee/utils/ndarray_utils.py
 Comment: 
 
 Filename: towhee/utils/np_format.py
 Comment: 
 
-Filename: towhee/utils/pil_utils.py
+Filename: towhee/utils/onnx_utils.py
 Comment: 
 
-Filename: towhee/utils/repo_normalize.py
+Filename: towhee/utils/pil_utils.py
 Comment: 
 
-Filename: towhee/utils/scipy_utils.py
+Filename: towhee/utils/repo_normalize.py
 Comment: 
 
 Filename: towhee/utils/singleton.py
 Comment: 
 
-Filename: towhee/utils/sklearn_utils.py
-Comment: 
-
-Filename: towhee/utils/tritonclient_utils.py
+Filename: towhee/utils/triton_httpclient.py
 Comment: 
 
 Filename: towhee/utils/yaml_utils.py
 Comment: 
 
 Filename: towhee/utils/thirdparty/__init__.py
 Comment: 
 
-Filename: towhee/utils/thirdparty/av_utils.py
-Comment: 
-
-Filename: towhee/utils/thirdparty/boto3_utils.py
-Comment: 
-
-Filename: towhee/utils/thirdparty/faiss_utils.py
+Filename: towhee/utils/thirdparty/dill_util.py
 Comment: 
 
 Filename: towhee/utils/thirdparty/ipython_utils.py
 Comment: 
 
-Filename: towhee/utils/thirdparty/milvus_utils.py
-Comment: 
-
-Filename: towhee/utils/thirdparty/numba_utils.py
-Comment: 
-
 Filename: towhee/utils/thirdparty/pandas_utils.py
 Comment: 
 
-Filename: towhee/utils/thirdparty/plyvel_utils.py
-Comment: 
-
-Filename: towhee/utils/thirdparty/pyarrow_utils.py
-Comment: 
-
-Filename: towhee-0.9.0.dist-info/LICENSE
+Filename: towhee-1.0.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: towhee-0.9.0.dist-info/METADATA
+Filename: towhee-1.0.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: towhee-0.9.0.dist-info/WHEEL
+Filename: towhee-1.0.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: towhee-0.9.0.dist-info/entry_points.txt
+Filename: towhee-1.0.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: towhee-0.9.0.dist-info/top_level.txt
+Filename: towhee-1.0.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: towhee-0.9.0.dist-info/RECORD
+Filename: towhee-1.0.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## towhee/__init__.py

```diff
@@ -10,79 +10,74 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint: disable=redefined-builtin
 # pylint: disable=import-outside-toplevel
-from typing import Union, List
-from pathlib import Path
-from towhee.engine import register
-from towhee.engine.factory import ops, pipeline, DEFAULT_PIPELINES
-from towhee.hparam import param_scope
-from towhee.hparam import HyperParameter as Document
-from towhee.hub.file_manager import FileManagerConfig
-from towhee.functional import DataCollection, State, Entity, DataFrame
-from towhee.functional import (
-    glob, glob_zip, read_csv, read_json, read_camera, read_video, read_audio, read_zip, dc, api, dummy_input, range, from_df
-)
 
-from towhee import dc2
-from towhee.dc2 import pipe
+import sys
+
+from towhee.runtime import register, pipe, ops, accelerate, AutoConfig, AutoPipes
+from towhee.serve.triton import triton_client
+from towhee.utils.lazy_import import LazyImport
+
+# Legacy towhee._types
+from towhee import types
+_types = types  # pylint: disable=protected-access
+sys.modules['towhee._types'] = sys.modules['towhee.types']
+
+
+datacollection = LazyImport('datacollection', globals(), 'towhee.datacollection')
+server_builder = LazyImport('server_builder', globals(), 'towhee.serve.server_builder')
 
 
-# Place all functions that are meant to be called by towhee.func() here aftering importing them.
 __all__ = [
-    'DEFAULT_PIPELINES',
-    'pipeline',
-    'ops',
-    'register',
-    'param_scope',
     'dataset',
-    'Document',
-    'DataCollection',
-    'DataFrame',
-    'State',
-    'Entity',
-    'range',
-    'glob',
-    'glob_zip',
-    'from_df',
-    'read_audio',
-    'read_camera',
-    'read_csv',
-    'read_json',
-    'read_video',
-    'read_zip',
-    'dc',
-    'api',
-    'dummy_input',
-    'update_default_cache',
-    'add_cache_path',
-    'cache_paths',
-    'default_cache',
-    # the new interface
     'pipe',
-    'dc2'
+    'triton_client',
+    'AutoConfig',
+    'build_docker_image',
+    'build_pipeline_model',
+    'AutoConfig',
+    'AutoPipes'
 ]
 
 __import__('pkg_resources').declare_namespace(__name__)
 
 
+def build_docker_image(*args, **kwargs):
+    """
+    Wrapper for lazy import build_docker_image
+    """
+    return server_builder.build_docker_image(*args, **kwargs)
+
+
+def build_pipeline_model(*args, **kwargs):
+    """
+    Wrapper for lazy import build_pipeline_model
+    """
+    return server_builder.build_pipeline_model(*args, **kwargs)
+
+
+def DataCollection(*args, **kwargs):  # pylint: disable=invalid-name
+    """
+    Wrapper for lazy import DataCollection
+    """
+    return datacollection.DataCollection(*args, **kwargs)
+
+
 def dataset(name: str, *args, **kwargs) -> 'TorchDataSet':
     """Get a dataset by name, and pass into the custom params.
-
     Args:
         name (str): Name of a dataset.
         *args (any): Arguments of the dataset construct method.
         **kwargs (any): Keyword arguments of the dataset construct method.
-
     Returns:
         TorchDataSet: The corresponding `TorchDataSet`.
-
     Examples:
         >>> from towhee import dataset
         >>> type(dataset('fake', size=10))
         <class 'towhee.data.dataset.dataset.TorchDataSet'>
     """
     from torchvision import datasets
     from towhee.data.dataset.dataset import TorchDataSet
@@ -90,51 +85,10 @@
         'mnist': datasets.MNIST, 'cifar10': datasets.cifar.CIFAR10, 'fake': datasets.FakeData
         # 'imdb': IMDB  # ,()
     }
     torch_dataset = dataset_construct_map[name](*args, **kwargs)
     return TorchDataSet(torch_dataset)
 
 
-def update_default_cache(default_path: Union[str, Path]):
-    """Update default cache.
-
-    Args:
-        default_path (Union[str, Path]): The default cache path.
-
-    Examples:
-        >>> import towhee
-        >>> towhee.update_default_cache('mock/path')
-        >>> towhee.default_cache
-        PosixPath('mock/path')
-
-        >>> from towhee.engine import DEFAULT_LOCAL_CACHE_ROOT
-        >>> towhee.update_default_cache(DEFAULT_LOCAL_CACHE_ROOT)
-    """
-    fmc = FileManagerConfig()
-    fmc.update_default_cache(default_path)
-
-
-def add_cache_path(insert_path: Union[str, Path, List[Union[str, Path]]]):
-    """Add a cache location to the front.
-
-    Most recently added paths will be checked first.
-
-    Args:
-        insert_path (str | Path | list[str | Path]): The path that you are trying to add. Accepts multiple inputs at once.
-
-    Examples:
-        >>> import towhee
-        >>> towhee.add_cache_path('mock/path')
-        >>> towhee.cache_paths[0]
-        PosixPath('mock/path')
-    """
-    fmc = FileManagerConfig()
-    fmc.add_cache_path(insert_path)
-
 
-cache_paths = FileManagerConfig().cache_paths
-default_cache = FileManagerConfig().default_cache
 
 
-def build_docker_image(dc_pipeline, image_name, cuda, inference_server='triton'):  # pylint: disable=unused-argument
-    from towhee.serve.triton.docker_image_builder import DockerImageBuilder
-    DockerImageBuilder(dc_pipeline, image_name, cuda).build()
```

## towhee/command/cmdline.py

```diff
@@ -12,32 +12,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 import argparse
 
 from towhee.command.develop import SetupCommand, UninstallCommand
-from towhee.command.execute import ExecuteCommand, PackageCommand, UploadCommand, UploadS3Command, LsS3Command, DownloadS3Command
+from towhee.command.execute import PackageCommand, UploadCommand
 from towhee.command.user import UserCommand, WhoCommand, LogoutCommand
 from towhee.command.repo import RepoCommand
 
 
 def main_body(args):
     parser = argparse.ArgumentParser('towhee', 'towhee')
     subparsers = parser.add_subparsers(dest='action', description='towhee command line tool.')
 
     actions = {
         'upload': UploadCommand,
-        'uploadS3': UploadS3Command,
-        'lsS3': LsS3Command,
-        'downloadS3':DownloadS3Command,
         'package': PackageCommand,
         'install': SetupCommand,
         'uninstall': UninstallCommand,
-        'run': ExecuteCommand,
         'login': UserCommand,
         'logout': LogoutCommand,
         'whoami': WhoCommand,
         'create': RepoCommand
     }
 
     for _, impl in actions.items():
```

## towhee/command/execute.py

```diff
@@ -8,81 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import numpy
 import os
 import sys
 import subprocess
 from datetime import date, datetime
 from pathlib import Path
-from typing import Union, Any, List
+from typing import List
 from setuptools import setup
 
-from towhee import pipeline
-from towhee.command.s3 import S3Bucket
-
-
-class ExecuteCommand: # pragma: no cover
-    """
-    Implementation for subcmd `towhee run`
-    """
-    def __init__(self, args) -> None:
-        self._args = args
-
-    def __call__(self):
-        pipe = pipeline(self._args.pipeline)
-        try:
-            res = pipe(int(self._args.input))
-        except ValueError:
-            res = pipe(self._args.input)
-        if not self._args.output:
-            try:
-                print(res[0][0])
-            except IndexError:
-                print(res)
-        else:
-            path = Path(self._args.output)
-            self.save_result(path, res)
-
-    @staticmethod
-    def install(subparsers):
-        parser_execute = subparsers.add_parser('run', help='execute command: run towhee pipeline')
-
-        parser_execute.add_argument('-i', '--input', required=True, help='input the parameter for pipeline defaults to None')
-        parser_execute.add_argument('-o', '--output', default=None, help='optional, path to the file that will be used to write results], '
-                                                                         'defaults to None which will print the result')
-        parser_execute.add_argument('pipeline', type=str, help='pipeline repo or path to yaml')
-
-    @staticmethod
-    def save_result(output: Union[str, Path], res: Any) -> None:
-        """
-        Save the results to local `output` file.
-
-        Args:
-            output (`str` | `Path`):
-                The path that you are trying to save.
-            res (`Any`):
-                The result with any format.
-        """
-        file_name = Path(output) / 'towhee_output.txt'
-        print(f'writing result to Path({str(output)})/towhee_output.txt')
-        with open(str(file_name), 'w', encoding='utf-8') as f:
-            if isinstance(res, list):
-                f.write('[')
-                for item in res:
-                    f.write(f'{item}')
-                f.write(']\n')
-            elif isinstance(res, numpy.ndarray):
-                numpy.savetxt(str(file_name), res)
-            else:
-                f.write(f'{str(res)}\n')
 
 class PackageCommand: # pragma: no cover
     """
     Implementation for subcmd `towhee package`
     """
     def __init__(self, args) -> None:
         self._args = args
@@ -153,57 +94,7 @@
         install = subparsers.add_parser('upload', help='upload command: upload operator')
         install.add_argument('-r', '--repository', required=False, \
                             help='The repository (package index) to upload the package to. Should be a section in the config file (default: pypi).'\
                                 '(Can also be set via TWINE_REPOSITORY environment variable.)')
         install.add_argument('-ru', '--repositoryurl', required=False, \
                             help='The repository (package index) URL to upload the package to. This overrides --repository.' \
                                 '(Can also be set via TWINE_REPOSITORY_URL environment variable.)')
-
-class UploadS3Command: # pragma: no cover
-    """
-    Implementation for subcmd `towhee uploadS3`
-    """
-    def __init__(self, args) -> None:
-        self._args = args
-
-    def __call__(self) -> None:
-        s3 = S3Bucket()
-        if not s3.upload_files(self._args.pathbucket, self._args.pathlocal):
-            print('upload file to s3 error, please check command.')
-    @staticmethod
-    def install(subparsers):
-        install = subparsers.add_parser('uploadS3', help='uploadS3 command: upload model to S3')
-        install.add_argument('-pb', '--pathbucket', required=True, help='bucket path to save file')
-        install.add_argument('-pl', '--pathlocal', required=True, help='local path to upload file')
-
-class LsS3Command: # pragma: no cover
-    """
-    Implementation for subcmd `towhee lsS3`
-    """
-    def __init__(self, args) -> None:
-        self._args = args
-
-    def __call__(self) -> None:
-        s3 = S3Bucket()
-        files = s3.get_list_s3(self._args.path)
-        print(files)
-    @staticmethod
-    def install(subparsers):
-        install = subparsers.add_parser('lsS3', help='lsS3 command: show files in S3 path')
-        install.add_argument('-p', '--path', required=False, help='bucket path to show files')
-
-class DownloadS3Command:
-    """
-    Implementation for subcmd `towhee DownloadS3`
-    """
-    def __init__(self, args) -> None:
-        self._args = args
-
-    def __call__(self) -> None:
-        s3 = S3Bucket()
-        if not s3.download_files(self._args.pathbucket, self._args.pathlocal):
-            print('download files from s3 error, please check command.')
-    @staticmethod
-    def install(subparsers):
-        install = subparsers.add_parser('downloadS3', help='downloadS3 command: download files in S3 path')
-        install.add_argument('-pb', '--pathbucket', required=True, help='bucket path to download files')
-        install.add_argument('-pl', '--pathlocal', required=True, help='local path to download files')
```

## towhee/datacollection/mixins/display.py

```diff
@@ -7,137 +7,26 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from typing import Tuple
-
 import numpy
 
-from towhee._types import Image
-from towhee.types import AudioFrame
-from towhee.hparam import param_scope
+from towhee.types import Image, VideoFrame, AudioFrame
 from towhee.datacollection.entity import Entity
 # pylint: disable=dangerous-default-value
 
 
-def get_df_on_columns(self, index: Tuple[str]): # pragma: no cover
-    # pylint: disable=import-outside-toplevel
-    from towhee.utils.thirdparty.pandas_utils import pandas as pd
-
-    def inner(entity: Entity):
-        data = {}
-        for feature in index:
-            data[feature] = getattr(entity, feature)
-        return data
-
-    data = map(inner, self)
-    df = pd.DataFrame(data)
-    return df
-
-
-def calc_df(df, feature: str, target: str): # pragma: no cover
-    # pylint: disable=import-outside-toplevel
-    from towhee.utils.thirdparty.pandas_utils import pandas as pd
-    lst = []
-    df[feature] = df[feature].fillna('NULL')
-
-    if target:
-        for i in range(df[feature].nunique()):
-            val = list(df[feature].unique())[i]
-            lst.append([feature,                                                         # Variable
-                        val,                                                             # Value
-                        df[df[feature] == val].count()[feature],                         # All
-                        df[(df[feature] == val) & (df[target] == 0)].count()[feature],   # Good (think: Fraud == 0)
-                        df[(df[feature] == val) & (df[target] == 1)].count()[feature]])  # Bad (think: Fraud == 1)
-
-        data = pd.DataFrame(lst, columns=['Variable', 'Value', 'All', 'Good', 'Bad'])
-        data['Share'] = data['All'] / data['All'].sum()
-        data['Bad Rate'] = data['Bad'] / data['All']
-        data['Distribution Good'] = (data['All'] - data['Bad']) / (data['All'].sum() - data['Bad'].sum())
-        data['Distribution Bad'] = data['Bad'] / data['Bad'].sum()
-        data['WoE'] = numpy.log(data['Distribution Good'] / data['Distribution Bad'])
-
-        data = data.replace({'WoE': {numpy.inf: 0, -numpy.inf: 0}})
-        data['IV'] = data['WoE'] * (data['Distribution Good'] - data['Distribution Bad'])
-
-        data = data.sort_values(by=['Variable', 'Value'], ascending=[True, True])
-        data.index = range(len(data.index))
-
-        iv = data['IV'].sum()
-        print(f'Variable: {feature}\'s IV sum is: {iv}')
-        return data
-    else:
-        for i in range(df[feature].nunique()):
-            val = list(df[feature].unique())[i]
-            lst.append([feature,                                                         # Variable
-                        val,                                                             # Value
-                        df[df[feature] == val].count()[feature]])                        # All
-        data = pd.DataFrame(lst, columns=['Variable', 'Value', 'All'])
-        data['Share'] = data['All'] / data['All'].sum()
-        return data
-
-
-def _feature_summarize_callback(self): # pragma: no cover
-    # pylint: disable=import-outside-toplevel
-    from towhee.utils.thirdparty.pandas_utils import pandas as pd
-
-    def wrapper(_: str, index, *arg, **kws):
-        if isinstance(index, str):
-            index = (index,)
-        index = list(index)
-        if arg:
-            kws['target'], = arg
-
-        target = None
-        if 'target' in kws:
-            target = kws.pop('target')
-            index.append(target)
-
-        df = get_df_on_columns(self, index)
-        summarize = pd.DataFrame()
-        if target:
-            index.remove(target)
-        for feature in index:
-            data = calc_df(df, feature, target)
-            summarize = summarize.append(data)
-
-        # pylint: disable=import-outside-toplevel
-        from towhee.utils.thirdparty import ipython_utils
-        ipython_utils.display(summarize)
-
-    return wrapper
-
-
-def _plot_callback(self): # pragma: no cover
-    # pylint: disable=unused-argument
-    def wrapper(_: str, index, *arg, **kws):
-        if isinstance(index, str):
-            index = (index,)
-        df = get_df_on_columns(self, index)
-        if 'kind' not in kws:
-            kws.update(kind='hist')
-        df.plot(**kws)
-
-    return wrapper
-
-
 class DisplayMixin: # pragma: no cover
     """
     Mixin for displaying data.
     """
 
-    def __init__(self):
-        super().__init__()
-        self.feature_summarize = param_scope().dispatch(_feature_summarize_callback(self))
-        self.plot = param_scope().dispatch(_plot_callback(self))
-
     def as_str(self):
         return self._factory(map(str, self._iterable))
 
     def show(self, limit=5, header=None, tablefmt='html', formatter={}):
         """Print the first n lines of a DataCollection.
 
         Args:
@@ -145,15 +34,15 @@
             header (_type_, optional): The field names. Defaults to None.
             tablefmt (str, optional): The format of the output, supports html, plain, grid.. Defaults to 'html'.
         """
         # pylint: disable=protected-access
         contents = [x for i, x in enumerate(self) if i < limit]
 
         if all(isinstance(x, Entity) for x in contents):
-            header = tuple(contents[0].__dict__) if not header else header
+            header = self._schema
             data = [list(x.__dict__.values()) for x in contents]
         else:
             data = [[x] for x in contents]
 
         table_display(to_printable_table(data, header, tablefmt, formatter), tablefmt)
 
 
@@ -219,25 +108,25 @@
     tb_contents = [[_to_plain_cell(x) for x in r] for r in data]
     return tabulate(tb_contents, headers=header, tablefmt=tablefmt)
 
 
 def _to_plain_cell(data):  # pragma: no cover
     if isinstance(data, str):
         return _text_brief(data)
-    if isinstance(data, Image):
+    if isinstance(data, (Image, VideoFrame)):
         return _image_brief(data)
     elif isinstance(data, AudioFrame):
         return _audio_frame_brief(data)
     elif isinstance(data, numpy.ndarray):
         return _ndarray_brief(data)
 
     elif isinstance(data, (list, tuple)):
         if all(isinstance(x, str) for x in data):
             return _list_brief(data, _text_brief)
-        elif all(isinstance(x, Image) for x in data):
+        elif all(isinstance(x, (Image, VideoFrame)) for x in data):
             return _list_brief(data, _image_brief)
         elif all(isinstance(x, AudioFrame) for x in data):
             return _list_brief(data, _audio_frame_brief)
         elif all(isinstance(x, numpy.ndarray) for x in data):
             return _list_brief(data, _ndarray_brief)
     return _default_brief(data)
 
@@ -255,14 +144,15 @@
     tb_style = 'style="border-collapse: collapse;"'
     th_style = 'style="text-align: center; font-size: 130%; border: none;"'
 
     str_2_callback = {
         'text': _text_brief,
         'image': _image_to_html_cell,
         'audio_frame': _audio_frame_to_html_cell,
+        'video_frame': _image_to_html_cell,
         'video_path': _video_path_to_html_cell,
     }
 
     trs = []
     trs.append('<tr>' + ' '.join(['<th ' + th_style + '>' + x + '</th>' for x in header]) + '</tr>')
 
     to_html_callback = {}
@@ -290,46 +180,53 @@
         return '<td ' + td_style + '>' + content + '</td>'
 
     if callback is not None:
         return wrap_td_tag(callback(data))
 
     if isinstance(data, str):
         return wrap_td_tag(_text_brief(data))
-    if isinstance(data, Image):
+    if isinstance(data, (Image, VideoFrame)):
         return wrap_td_tag(_image_to_html_cell(data))
     elif isinstance(data, AudioFrame):
         return wrap_td_tag(_audio_frame_to_html_cell(data))
     elif isinstance(data, numpy.ndarray):
         return wrap_td_tag(_ndarray_brief(data), align='left')
 
     elif isinstance(data, (list, tuple)):
         if all(isinstance(x, str) for x in data):
             return wrap_td_tag(_text_list_brief(data))
-        elif all(isinstance(x, Image) for x in data):
+        elif all(isinstance(x, (Image, VideoFrame)) for x in data):
             return wrap_td_tag(_images_to_html_cell(data), vertical_align='top')
         elif all(isinstance(x, AudioFrame) for x in data):
             return wrap_td_tag(_audio_frames_to_html_cell(data), vertical_align='top')
         elif all(isinstance(x, numpy.ndarray) for x in data):
             return wrap_td_tag(_list_brief(data, _ndarray_brief), align='left')
         else:
             return wrap_td_tag(_list_brief(data, _default_brief), align='left')
     return wrap_td_tag(_default_brief(data))
 
 
 def _image_to_html_cell(img, width=128, height=128):  # pragma: no cover
     # pylint: disable=import-outside-toplevel
     from towhee.utils.cv2_utils import cv2
+    from towhee.utils.matplotlib_utils import plt
     import base64
-
-    _, img_encode = cv2.imencode('.JPEG', img)
-    src = 'src="data:image/jpeg;base64,' + base64.b64encode(img_encode).decode() + '" '
-    w = 'width = "' + str(width) + 'px" '
-    h = 'height = "' + str(height) + 'px" '
+    from io import BytesIO
+    plt.ioff()
+    fig = plt.figure(figsize=(width / 100, height / 100))
+    img = cv2.resize(img, (width, height))
+    fig.figimage(img)
+    plt.ion()
+    tmpfile = BytesIO()
+    fig.savefig(tmpfile, format='png')
+    data = base64.b64encode(tmpfile.getvalue()).decode('ascii')
+    src = 'src="data:image/png;base64,' + data + '" '
+    w = '128 = "' + str(128) + 'px" '
+    h = '128 = "' + str(128) + 'px" '
     style = 'style = "float:left; padding:2px"'
-
     return '<img ' + src + w + h + style + '>'
 
 
 def _images_to_html_cell(imgs, width=128, height=128):  # pragma: no cover
     return ' '.join([_image_to_html_cell(x, width, height) for x in imgs])
```

## towhee/hub/__init__.py

```diff
@@ -7,7 +7,24 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.s
+
+
+from .cache_manager import CacheManager, set_local_dir
+from .downloader import set_hub_url
+
+_CACHE_MANAGER = CacheManager()
+
+
+def get_operator(operator: str, tag: str, install_reqs: bool = True):
+    return _CACHE_MANAGER.get_operator(operator, tag, install_reqs)
+
+
+__all__ = [
+    'set_local_dir',
+    'set_hub_url',
+    'get_operator'
+]
```

## towhee/hub/repo_manager.py

```diff
@@ -23,15 +23,15 @@
 
 from tqdm import tqdm
 from tempfile import TemporaryFile
 from concurrent.futures import ThreadPoolExecutor
 from towhee.utils.hub_utils import HubUtils
 from towhee.utils.log import engine_log
 
-REPO_TEMPLATE = {'pipeline': 'pipeline-template', 'pyoperator': 'pyop-template', 'nnoperator': 'nnop-template'}
+REPO_TEMPLATE = {'pipeline': 'pipeline-template', 'pyoperator': 'pyoperator-template', 'nnoperator': 'nnoperator-template'}
 
 class RepoManager:
     """
     Base Repo Manager class to create, initialize, download repos.
 
     Args:
         author (`str`):
```

## towhee/operator/__init__.py

```diff
@@ -9,13 +9,12 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from towhee.operator.base import Operator, NNOperator, PyOperator, OperatorFlag, SharedType
-from towhee.operator.stateful_operator import StatefulOperator
 
 __all__ = [
-    'Operator', 'NNOperator', 'PyOperator', 'StatefulOperator', 'OperatorFlag',
+    'Operator', 'NNOperator', 'PyOperator', 'OperatorFlag',
     'SharedType'
 ]
```

## towhee/operator/base.py

```diff
@@ -125,14 +125,18 @@
     def framework(self):
         return self._framework
 
     @framework.setter
     def framework(self, framework: str):
         self._framework = framework
 
+    @property
+    def shared_type(self):
+        return SharedType.Shareable
+
     def save_model(self):
         """
         Save model to local.
         """
         raise NotImplementedError
 
     def supported_model_names(self):
@@ -199,16 +203,23 @@
                 Otherwise, `Trainer` will build dataloader from train_dataset.
             model_card (`ModelCard`):
                 Model card contains the training informations.
         Returns:
 
         """
         from towhee.trainer.trainer import Trainer  # pylint: disable=import-outside-toplevel
+        import torch  # pylint: disable=import-outside-toplevel
         if self._trainer is None:
-            self._trainer = Trainer(self.model,
+            if isinstance(self.model, torch.nn.Module):
+                training_model = self.model
+            elif hasattr(self, '_model') and isinstance(self._model, torch.nn.Module):
+                training_model = self._model
+            else:
+                raise AttributeError('There is no trainable model attr in this operator.')
+            self._trainer = Trainer(training_model,
                                     training_config,
                                     train_dataset,
                                     eval_dataset,
                                     train_dataloader,
                                     eval_dataloader,
                                     model_card)
         else:
@@ -221,40 +232,14 @@
             if train_dataloader is not None:
                 self._trainer.train_dataloader = train_dataloader
             if eval_dataloader is not None:
                 self._trainer.eval_dataloader = eval_dataloader
             if model_card is not None:
                 self._trainer.model_card = model_card
 
-    def load(self, path: str = None):
-        """
-        Load the model checkpoint into an operator.
-
-        Args:
-            path (`str`):
-                The folder path containing the model's checkpoints.
-        """
-        self.trainer.load(path)
-
-    def save(self, path: str, overwrite: bool = True):
-        """
-        Save the model checkpoint into the path.
-
-        Args:
-            path (`str`):
-                The folder path containing the model's checkpoints.
-            overwrite (`bool`):
-                If True, it will overwrite the same name path when existing.
-
-        Raises:
-            (`FileExistsError`)
-                If `overwrite` is False, when there already exists a path, it will raise Error.
-        """
-        self.trainer.save(path, overwrite)
-
 
 class PyOperator(Operator):
     """
     Python function operator, no machine learning frameworks involved.
     """
 
     def __init__(self):
```

## towhee/runtime/__init__.py

```diff
@@ -11,17 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from .factory import ops, register
 from .pipeline import Pipeline as pipe
+from .auto_pipes import AutoPipes
+from .auto_config import AutoConfig
 
-from .runtime_conf import get_sys_config
+from .runtime_conf import get_sys_config, accelerate
+from .node_config import AcceleratorConf
 
 
 __all__ = [
     'pipe',
     'register',
     'ops',
-    'get_sys_config'
+    'get_sys_config',
+    'accelerate',
+    'AcceleratorConf',
+    'AutoConfig',
+    'AutoPipes',
+    'AutoConfig'
 ]
```

## towhee/runtime/check_utils.py

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, Any, Set, Tuple
+
+from towhee.utils.log import engine_log
 from towhee.runtime.constants import (
     WindowConst,
     FilterConst,
     TimeWindowConst
 )
 
 
@@ -24,16 +26,18 @@
     """
     Check if the src is a valid node dictionary to describe.
 
     Args:
         info (`Dict[str, Any]`): The info dictionary.
         essentials (`Set[str]`): The essential keys that node dictionary should contain.
     """
+    if not isinstance(info, dict):
+        raise ValueError(f'Config {str(info)} is not valid, it must be dict.')
     info_keys = set(info.keys())
-    if not isinstance(info, dict) or not essentials.issubset(info_keys):
+    if not essentials.issubset(info_keys):
         raise ValueError(f'Node {str(info)} is not valid, lack attr {essentials - info_keys}')
 
 
 def check_set(inputs: Tuple, all_inputs: Set[str]):
     """
     Check if the inputs in all_inputs.
 
@@ -93,20 +97,40 @@
         check_set(iter_param[TimeWindowConst.param.timestamp_col], all_inputs)
         check_int(iter_param, [TimeWindowConst.param.time_range_sec,
                                TimeWindowConst.param.time_step_sec])
     elif iter_type == WindowConst.name:
         check_int(iter_param, [WindowConst.param.size,
                                WindowConst.param.step])
 
+
 def check_config(info: Dict[str, Any], essentials: Set[str]):
     """
     Check if the src covers all the needed config info.
 
     Args:
         info (`Dict[str, Any]`):
             The info dictionary.
         essentials (`Set[str]`):
             The essential keys that node config dictionary should contain.
     """
+    if not isinstance(info, dict):
+        raise ValueError(f'Config {str(info)} is not valid, it must be dict.')
     info_keys = set(info.keys())
-    if not isinstance(info, dict) or not essentials.issubset(info_keys):
+    if not essentials.issubset(info_keys):
         raise ValueError(f'Config {str(info)} is not valid, lack attr {essentials - info_keys}')
+
+
+def check_supported(info: Dict[str, Any], essentials: Set[str]):
+    """
+    Check if the src is supported and logging warning.
+
+    Args:
+        info (`Dict[str, Any]`):
+            The info dictionary.
+        essentials (`Set[str]`):
+            The essential keys that node config dictionary can contain.
+    """
+    if not isinstance(info, dict):
+        raise ValueError(f'Config {str(info)} is not valid, it must be dict.')
+    info_keys = set(info.keys())
+    if not info_keys.issubset(essentials):
+        engine_log.warning('Config %s is not supported, please make sure the config is in %s', str(info_keys - essentials), essentials)
```

## towhee/runtime/dag_repr.py

```diff
@@ -15,14 +15,15 @@
 import types
 from typing import Dict, Any, Set, List, Tuple
 
 from towhee.runtime.check_utils import check_set, check_node_iter
 from towhee.runtime.node_repr import NodeRepr
 from towhee.runtime.schema_repr import SchemaRepr
 from towhee.runtime.constants import FilterConst, TimeWindowConst, OPType, InputConst, OutputConst
+from towhee.runtime.node_config import TowheeConfig
 
 
 class DAGRepr:
     """
     A `DAGRepr` represents a complete DAG.
 
     Args:
@@ -130,36 +131,41 @@
         Returns:
            Set: A set of the used schema behind the node.
         """
         ahead_schema = ahead_edge.copy()
         used_schema = set()
         stack = [name]
         visited = [name]
+        outputs_schema = ()
         while stack:
             n = stack.pop()
+            check_schema = nodes[n].inputs
             used_col = DAGRepr.get_base_col(nodes[n])
             if used_col is not None:
                 if isinstance(used_col, str):
-                    used_schema.add(used_col)
+                    check_schema += (used_col,)
                 else:
-                    for c in used_col:
-                        used_schema.add(c)
+                    check_schema += tuple(used_col)
 
-            common_schema = set(nodes[n].inputs) & ahead_schema
+            common_schema = (set(check_schema)-set(outputs_schema)) & ahead_schema
             for x in common_schema:
                 ahead_schema.remove(x)
                 used_schema.add(x)
             next_nodes = nodes[n].next_nodes
-            if len(ahead_schema) == 0 or next_nodes is None:
+            if len(ahead_schema) == 0:
                 break
+            if next_nodes is None:
+                continue
 
             for i in next_nodes[::-1]:
                 if i not in visited:
                     stack.append(i)
-                    visited.append(i)
+            visited.append(n)
+            outputs_schema += nodes[n].outputs
+
         return used_schema
 
     @staticmethod
     def get_base_col(nodes: NodeRepr):
         if nodes.iter_info.type == FilterConst.name:
             return nodes.iter_info.param[FilterConst.param.filter_by]
         if nodes.iter_info.type == TimeWindowConst.name:
@@ -192,15 +198,20 @@
 
         edge_schemas = {}
         for d in schema:
             if d not in ahead_schemas:
                 inputs_type = [ahead_schemas[inp].type for inp in inputs]
                 edge_schemas[d] = SchemaRepr.from_dag(d, iter_type, inputs_type)
             elif d in outputs:
-                edge_schemas[d] = SchemaRepr.from_dag(d, iter_type, [ahead_schemas[d].type])
+                if iter_type == 'concat':
+                    inputs_type = [ahead_schemas[d].type]
+                else:
+                    inputs_type = [ahead_schemas[inp].type for inp in inputs]
+                    inputs_type.append(ahead_schemas[d].type)
+                edge_schemas[d] = SchemaRepr.from_dag(d, iter_type, inputs_type)
             else:
                 edge_schemas[d] = SchemaRepr.from_dag(d, 'map', [ahead_schemas[d].type])
         edge = {'schema': edge_schemas, 'data': [(s, t.type) for s, t in edge_schemas.items()]}
         return edge
 
     @staticmethod
     def set_edges(nodes: Dict[str, NodeRepr]):
@@ -273,14 +284,19 @@
                     name = fn.__class__.__name__
 
             return name
 
         nodes = {}
         node_index = 0
         for key, val in dag.items():
+            # Deal with AutoConfig
+            if 'config' in val and val['config'] is not None and isinstance(val['config'], TowheeConfig):
+                val['config'] = val['config'].config
+                assert isinstance(val['config'], dict)
+
             # Deal with input and output.
             if key in [InputConst.name, OutputConst.name]:
                 val['config'] = {'name': key}
 
             # Concat nodes does not have op_info.
             elif val['iter_info']['type'] == 'concat':
                 val['config'] = {'name': 'concat-' + str(node_index)}
@@ -296,11 +312,10 @@
             elif isinstance(val['config'], dict):
                 if 'name' not in val['config']:
                     name = _get_name(val)
                     val['config']['name'] = name + '-' + str(node_index)
                     node_index += 1
 
             nodes[key] = NodeRepr.from_dict(key, val)
-
         DAGRepr.check_nodes(nodes)
         dag_nodes, schema_edges = DAGRepr.set_edges(nodes)
         return DAGRepr(dag_nodes, schema_edges)
```

## towhee/runtime/data_queue.py

```diff
@@ -131,14 +131,21 @@
                 ret[name] = data[i]
         else:
             for i, name in enumerate(names):
                 if name in cols:
                     ret[name] = data[i]
         return ret
 
+    def to_list(self, kv_format=False):
+        if not self.sealed:
+            raise RuntimeError('The queue is not sealed')
+        if not kv_format:
+            return [self.get() for _ in range(self.size)]
+        return [self.get_dict() for _ in range(self.size)]
+
     @property
     def max_size(self):
         return self._max_size
 
     @max_size.setter
     def max_size(self, max_size):
         with self._not_full:
```

## towhee/runtime/node_config.py

```diff
@@ -8,85 +8,222 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Dict, Any, Optional
+from typing import Dict, Any, Optional, List
 
-from towhee.runtime.check_utils import check_config
+from towhee.runtime.check_utils import check_config, check_supported
 
 
 class NodeConfig:
     """
     The config of nodes.
     """
     def __init__(self, *, name: str,
                  device: int,
-                 acc_info: Optional[Dict]):
+                 acc_info: Optional[Dict],
+                 server_info: Optional[Dict]):
         self._name = name
         self._device = device
         self._acc_conf = AcceleratorConf.from_dict(acc_info) if acc_info is not None else None
+        self._server_conf = ServerConf.from_dict(server_info) if server_info is not None else None
 
     @property
     def name(self):
         return self._name
 
     @property
     def device(self):
         return self._device
 
     @property
     def acc_conf(self):
         return self._acc_conf
 
+    @acc_conf.setter
+    def acc_conf(self, acc_conf):
+        self._acc_conf = acc_conf
+
+    @property
+    def server_conf(self):
+        return self._server_conf
+
     @staticmethod
     def from_dict(conf: Dict[str, Any]):
         essentials = {'name'}
         check_config(conf, essentials)
         return NodeConfig(
             name=conf['name'],
             device=conf.get('device', -1),
-            acc_info=conf.get('acc_info')
+            acc_info=conf.get('acc_info'),
+            server_info=conf.get('server')
         )
 
 
 class AcceleratorConf:
     """
     AcceleratorConf
     """
     def __init__(self, acc_type: str, conf: Dict):
         self._type = acc_type
         if self._type == 'triton':
-            self._conf = TritonConf.from_dict(conf)
+            self._conf = TritonClientConf.from_dict(conf)
+        elif self._type == 'mock':
+            pass
         else:
             raise ValueError(f'Unkown accelerator: {acc_type}')
 
     def is_triton(self):
         return self._type == 'triton'
 
+    def is_mock(self):
+        return self._type == 'mock'
+
     @property
     def triton(self):
         return self._conf
 
     @staticmethod
     def from_dict(acc_conf: Dict[str, Any]):
         return AcceleratorConf(acc_conf['type'], acc_conf['params'])
 
 
-class TritonConf:
+class TritonClientConf:
     """
     Triton client config.
     """
-    def __init__(self, model_name: str):
+    def __init__(self, model_name: str, inputs: List[str], outputs: List[str]):
         self._model_name = model_name
+        self._inputs = inputs
+        self._outputs = outputs
 
     @property
     def model_name(self):
         return self._model_name
 
+    @property
+    def inputs(self):
+        return self._inputs
+
+    @property
+    def outputs(self):
+        return self._outputs
+
     @staticmethod
     def from_dict(conf):
-        if 'model_name' not in conf:
-            raise ValueError('Triton accelerator lost model_name config')
-        return TritonConf(conf['model_name'])
+        return TritonClientConf(conf['model_name'], conf['inputs'], conf['outputs'])
+
+
+class ServerConf:
+    """
+    ServerConf
+    """
+    def __init__(self, device_ids,
+                 max_batch_size,
+                 batch_latency_micros,
+                 num_instances_per_device,
+                 triton: 'TritonServerConf'):
+        self._device_ids = device_ids
+        self._max_batch_size = max_batch_size
+        self._batch_latency_micros = batch_latency_micros
+        self._num_instances_per_device = num_instances_per_device
+        self._triton = triton
+
+    @property
+    def device_ids(self):
+        return self._device_ids
+
+    @property
+    def max_batch_size(self):
+        return self._max_batch_size
+
+    @property
+    def batch_latency_micros(self):
+        return self._batch_latency_micros
+
+    @property
+    def num_instances_per_device(self):
+        return self._num_instances_per_device
+
+    @property
+    def triton(self):
+        return self._triton
+
+    @staticmethod
+    def from_dict(server_info: Dict[str, Any]):
+        check_supported(server_info, {'device_ids', 'max_batch_size', 'batch_latency_micros', 'num_instances_per_device', 'triton'})
+        triton_conf = TritonServerConf.from_dict(server_info.get('triton'))
+        return ServerConf(server_info.get('device_ids'), server_info.get('max_batch_size'), server_info.get('batch_latency_micros'),
+                          server_info.get('num_instances_per_device'), triton_conf)
+
+
+class TritonServerConf:
+    """
+    Triton server config.
+    """
+    def __init__(self, preferred_batch_size: str = None):
+        self._preferred_batch_size = preferred_batch_size
+
+    @property
+    def preferred_batch_size(self):
+        return self._preferred_batch_size
+
+    @staticmethod
+    def from_dict(triton_info: Dict[str, Any]):
+        if triton_info is None:
+            return TritonServerConf()
+        check_supported(triton_info, {'preferred_batch_size'})
+        if 'preferred_batch_size' not in triton_info:
+            return TritonServerConf()
+        return TritonServerConf(triton_info.get('preferred_batch_size'))
+
+
+class TowheeConfig:
+    """
+    TowheeConfig mapping for AutoConfig.
+    """
+    def __init__(self, config: Dict):
+        self._config = config
+
+    @property
+    def config(self) -> Dict:
+        return self._config
+
+    @classmethod
+    def set_local_config(cls, device: int) -> 'TowheeConfig':
+        config = {
+            'device': device
+        }
+        return cls(config)
+
+    @classmethod
+    def set_triton_config(cls,
+                          device_ids: list,
+                          num_instances_per_device: int,
+                          max_batch_size: int,
+                          batch_latency_micros: int,
+                          preferred_batch_size: list) -> 'TowheeConfig':
+        config = {
+            'server': {
+                'device_ids': device_ids,
+                'num_instances_per_device': num_instances_per_device,
+                'max_batch_size': max_batch_size,
+                'batch_latency_micros': batch_latency_micros,
+                'triton': {
+                    'preferred_batch_size': preferred_batch_size
+                }
+            }
+        }
+        return cls(config)
+
+    def __add__(self, other: 'TowheeConfig') -> 'TowheeConfig':
+        if isinstance(self._config, dict):
+            self._config.update(other.config)
+        else:
+            self._config = other.config
+        return self
+
+    def __or__(self, other: 'TowheeConfig') -> 'TowheeConfig':
+        return self + other
```

## towhee/runtime/performance_profiler.py

```diff
@@ -25,26 +25,24 @@
     """
     PipelineProfiler to trace one pipeline.
     """
     def __init__(self, dag: 'DAGRepr'):
         self.time_in = None
         self.time_out = None
         self.data = None
-        self.dag = dag
         self.node_tracer = {}
         self.node_report = {}
         for uid, node in dag.nodes.items():
             self.node_tracer[uid] = dict(name=node.name, iter=node.iter_info.type, init_in=[], init_out=[], queue_in=[], queue_out=[],
                                          process_in=[], process_out=[])
 
-    def add_node_tracer(self, name, event, ts, data):
+    def add_node_tracer(self, name, event, ts):
         ts = int(ts) / 1000000
         if event == Event.pipe_in:
             self.time_in = ts
-            self.data = data
         elif event == Event.pipe_out:
             self.time_out = ts
             self.set_node_report()
         else:
             self.node_tracer[name][event].append(ts)
 
     def set_node_report(self):
@@ -146,30 +144,30 @@
 
 
 class PerformanceProfiler:
     """
     PerformanceProfiler to analysis the time profiler.
     """
 
-    def __init__(self, time_records: list, dag: 'DAGRepr'):
-        self.time_records = time_records
+    def __init__(self, time_prfilers: list, dag: 'DAGRepr'):
+        self._time_prfilers = time_prfilers
         self.dag = dag
         self.timing = None
         self.pipes_profiler = []
         self.node_report = {}
         self.make_report()
 
     def make_report(self):
-        p_tracer = PipelineProfiler(self.dag)
-        for ts_info in self.time_records:
-            name, event, ts, data = ts_info.split('::')
-            p_tracer.add_node_tracer(name, event, ts, data)
-            if event == Event.pipe_out:
-                self.pipes_profiler.append(p_tracer)
-                p_tracer = PipelineProfiler(self.dag)
+        for tf in self._time_prfilers:
+            p_tracer = PipelineProfiler(self.dag)
+            p_tracer.data = tf.inputs
+            for ts_info in tf.time_record:
+                name, event, ts = ts_info.split('::')
+                p_tracer.add_node_tracer(name, event, ts)
+            self.pipes_profiler.append(p_tracer)
         self.set_node_report()
         self.timing = self.get_timing_report()
 
     def set_node_report(self):
         self.node_report = deepcopy(self.pipes_profiler[0].node_report)
         for p_tracer in self.pipes_profiler[1:]:
             for node_id, node_tracer in p_tracer.node_report.items():
@@ -177,21 +175,22 @@
                 self.node_report[node_id]['total_time'] += node_tracer['total_time']
                 self.node_report[node_id]['init'] += node_tracer['init']
                 self.node_report[node_id]['wait_data'] += node_tracer['wait_data']
                 self.node_report[node_id]['call_op'] += node_tracer['call_op']
                 self.node_report[node_id]['output_data'] += node_tracer['output_data']
 
     def get_timing_report(self):
+        timeline = self.pipes_profiler[-1].time_out - self.pipes_profiler[0].time_in
         timing_list = []
         for p_tracer in self.pipes_profiler:
             timing_list.append(p_tracer.time_out - p_tracer.time_in)
         timing_list.sort()
         total_time = sum(timing_list)
         avg_time = total_time / len(timing_list)
-        return round(total_time, 4), round(avg_time, 4), round(timing_list[-1], 4), round(timing_list[0], 4)
+        return round(timeline, 4), round(avg_time, 4), round(timing_list[-1], 4), round(timing_list[0], 4)
 
     def show(self):
         print('Total count: ', len(self.pipes_profiler))
         print('Total time(s): ', self.timing[0])
         print('Avg time(s): ', self.timing[1])
         print('Max time(s): ', self.timing[2])
         print('Min time(s): ', self.timing[3])
@@ -238,23 +237,24 @@
     queue_out = 'queue_out'
 
 
 class TimeProfiler:
     """
     TimeProfiler to record the event and timestamp.
     """
-    def __init__(self):
-        self._enable = False
+    def __init__(self, enable=False):
+        self._enable = enable
         self.time_record = []
+        self.inputs = None
 
-    def record(self, uid, event, pipe_input=None):
+    def record(self, uid, event):
         if not self._enable:
             return
         timestamp = int(round(time.time() * 1000000))
-        self.time_record.append(f'{uid}::{event}::{timestamp}::{pipe_input}')
+        self.time_record.append(f'{uid}::{event}::{timestamp}')
 
     def enable(self):
         self._enable = True
 
     def disable(self):
         self._enable = False
```

## towhee/runtime/pipeline.py

```diff
@@ -263,14 +263,15 @@
             >>> pipe(1, 12).get()
             None
             >>> pipe(11, 12).get()
             [12]
         """
         output_schema = self._check_schema(output_schema)
         input_schema = self._check_schema(input_schema)
+        filter_columns = self._check_schema(filter_columns)
 
         uid = uuid.uuid4().hex
         fn_action = self._to_action(fn)
         dag_dict = deepcopy(self._dag)
         dag_dict[uid] = {
             'inputs': input_schema,
             'outputs': output_schema,
```

## towhee/runtime/runtime_conf.py

```diff
@@ -8,20 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+#pylint: disable=import-outside-toplevel
 import contextvars
 import contextlib
 import functools
 
 
-
 class RuntimeConf:
     """
     Runtime config, passed by contextvars
     """
     def __init__(self, sys_conf=None, acc=None):
         self._sys_config = sys_conf
         self._accelerator = acc
@@ -79,19 +79,25 @@
     except:  # pylint: disable=bare-except
         return None
 
 
 def accelerate(model):
     @functools.wraps(model)
     def _decorated(*args, **kwargs):
-        runtime_conf = _RUNTIME_CONF_VAR.get()
-        if runtime_conf.accelerator is None:
+        runtime_conf = _RUNTIME_CONF_VAR.get(None)
+        if runtime_conf is None or runtime_conf.accelerator is None:
             return model(*args, **kwargs)
         elif runtime_conf.accelerator.is_triton():
-            return TritonClient(runtime_conf.accelerator.triton.model_name)
+            from towhee.serve.triton.triton_client import TritonClient
+            triton_conf = runtime_conf.accelerator.triton
+            return TritonClient(triton_conf.model_name, triton_conf.inputs, triton_conf.outputs)
+        elif runtime_conf.accelerator.is_mock():
+            return MockModel()
         else:
             return None
     return _decorated
 
 
-class TritonClient:
-    pass
+class MockModel:
+    def __call__(self, data):
+        return data
+
```

## towhee/runtime/runtime_pipeline.py

```diff
@@ -9,136 +9,178 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from typing import Dict, Any
+from typing import Dict, Any, Union, Tuple, List
 from concurrent.futures import ThreadPoolExecutor
 
 from towhee.utils.log import engine_log
 from .operator_manager import OperatorPool
 from .data_queue import DataQueue
 from .dag_repr import DAGRepr
 from .nodes import create_node, NodeStatus
 from .node_repr import NodeRepr
 from .performance_profiler import PerformanceProfiler, TimeProfiler, Event
 from .constants import TracerConst
 
 
-class Graph:
+class _GraphResult:
+    def __init__(self, graph: '_Graph'):
+        self._graph = graph
+
+    def result(self):
+        ret = self._graph.result()
+        del self._graph
+        return ret
+
+
+class _Graph:
     """
     Graph.
 
     Args:
         nodes(`Dict[str, NodeRepr]`): The pipeline nodes from DAGRepr.nodes.
         edges(`Dict[str, Any]`): The pipeline edges from DAGRepr.edges.
         operator_pool(`OperatorPool`): The operator pool.
         thread_pool(`OperatorPool`): The ThreadPoolExecutor.
     """
     def __init__(self,
                  nodes: Dict[str, NodeRepr],
                  edges: Dict[str, Any],
                  operator_pool: 'OperatorPool',
                  thread_pool: 'ThreadPoolExecutor',
-                 time_profiler: 'TimeProfiler' = None):
+                 enable_trance: bool = False):
         self._nodes = nodes
         self._edges = edges
         self._operator_pool = operator_pool
         self._thread_pool = thread_pool
-        self._time_profiler = time_profiler
+        self._time_profiler = TimeProfiler(enable_trance)
         self._node_runners = None
         self._data_queues = None
+        self.features = None
+        self.time_profiler.record(Event.pipe_name, Event.pipe_in)
         self.initialize()
+        self._input_queue = self._data_queues[0]
 
     def initialize(self):
         self._node_runners = []
         self._data_queues = dict((name, DataQueue(edge['data'])) for name, edge in self._edges.items())
         for name in self._nodes:
             in_queues = [self._data_queues[edge] for edge in self._nodes[name].in_edges]
             out_queues = [self._data_queues[edge] for edge in self._nodes[name].out_edges]
             node = create_node(self._nodes[name], self._operator_pool, in_queues, out_queues, self._time_profiler)
             if not node.initialize():
                 raise RuntimeError(node.err_msg)
             self._node_runners.append(node)
 
     def result(self) -> any:
+        for f in self.features:
+            f.result()
         errs = ''
         for node in self._node_runners:
             if node.status != NodeStatus.FINISHED:
                 if node.status ==NodeStatus.FAILED:
                     errs += node.err_msg + '\n'
         if errs:
             raise RuntimeError(errs)
         end_edge_num = self._nodes['_output'].out_edges[0]
         res = self._data_queues[end_edge_num]
+        self.time_profiler.record(Event.pipe_name, Event.pipe_out)
         return res
 
-    def __call__(self, *inputs):
-        self._data_queues[0].put(*inputs)
-        self._data_queues[0].seal()
-        features = []
+    def async_call(self, inputs: Union[Tuple, List]):
+        self.time_profiler.inputs = inputs
+        self._input_queue.put(inputs)
+        self._input_queue.seal()
+        self.features = []
         for node in self._node_runners:
-            features.append(self._thread_pool.submit(node.process))
+            self.features.append(self._thread_pool.submit(node.process))
+        return _GraphResult(self)
 
-        _ = [f.result() for f in features]
-        return self.result()
+    def __call__(self, inputs: Union[Tuple, List]):
+        f = self.async_call(inputs)
+        return f.result()
+
+    @property
+    def time_profiler(self):
+        return self._time_profiler
+
+    @property
+    def input_col_size(self):
+        return self._input_queue.col_size
 
 
 class RuntimePipeline:
     """
     Manage the pipeline and runs it as a single instance.
 
 
     Args:
         dag_dict(`Dict`): The DAG Dictionary from the user pipeline.
         max_workers(`int`): The maximum number of threads.
     """
 
-    def __init__(self, dag_dict: Dict, max_workers: int = None, config: dict = None):
-        self._dag_repr = DAGRepr.from_dict(dag_dict)
+    def __init__(self, dag: Union[Dict, DAGRepr], max_workers: int = None, config: dict = None):
+        if isinstance(dag, Dict):
+            self._dag_repr = DAGRepr.from_dict(dag)
+        else:
+            self._dag_repr = dag
         self._operator_pool = OperatorPool()
         self._thread_pool = ThreadPoolExecutor(max_workers=max_workers)
         self._time_profiler_list = []
-        self._config = config
+        self._config = {} if config is None else config
+        self._enable_trace = self._config.get(TracerConst.name, False)
 
     def preload(self):
         """
         Preload the operators.
         """
-        _ = Graph(self._dag_repr.nodes, self._dag_repr.edges, self._operator_pool, self._thread_pool)
+        return _Graph(self._dag_repr.nodes, self._dag_repr.edges, self._operator_pool, self._thread_pool)
 
     def __call__(self, *inputs):
         """
         Output with ordering matching the input `DataQueue`.
         """
-        time_profiler = TimeProfiler()
-        if self._config is not None and TracerConst.name in self._config and self._config[TracerConst.name]:
-            time_profiler.enable()
-
-        time_profiler.record(Event.pipe_name, Event.pipe_in, inputs)
-        graph = Graph(self._dag_repr.nodes, self._dag_repr.edges, self._operator_pool, self._thread_pool, time_profiler)
-        outputs = graph(inputs)
-        time_profiler.record(Event.pipe_name, Event.pipe_out)
-
-        self._time_profiler_list.append(time_profiler)
-        return outputs
+        graph = _Graph(self._dag_repr.nodes, self._dag_repr.edges, self._operator_pool, self._thread_pool, self._enable_trace)
+        if self._enable_trace:
+            self._time_profiler_list.append(graph.time_profiler)
+        return graph(inputs)
+
+    def batch(self, batch_inputs):
+        graph_res = []
+        for inputs in batch_inputs:
+            gh = _Graph(self._dag_repr.nodes, self._dag_repr.edges, self._operator_pool, self._thread_pool, self._enable_trace)
+            if self._enable_trace:
+                self._time_profiler_list.append(gh.time_profiler)
+            if gh.input_col_size == 1:
+                inputs = (inputs, )
+            graph_res.append(gh.async_call(inputs))
+
+        rets = []
+        for gf in graph_res:
+            ret = gf.result()
+            rets.append(ret)
+        return rets
+
+    @property
+    def dag_repr(self):
+        return self._dag_repr
 
     def profiler(self):
         """
         Report the performance results after running the pipeline, and please note that you need to set tracer to True when you declare a pipeline.
         """
-        records = []
-        for time_profiler in self._time_profiler_list:
-            records += time_profiler.time_record
-        if len(records) == 0:
+        if not self._enable_trace or not self._time_profiler_list:
             engine_log.warning('Please set tracer to True or you need to run it first, there is nothing to report.')
             return None
-        performance_profiler = PerformanceProfiler(records, self._dag_repr)
+
+        performance_profiler = PerformanceProfiler(self._time_profiler_list, self._dag_repr)
         return performance_profiler
 
     def reset_tracer(self):
         """
         Reset the tracer, reset the record to None.
         """
         self._time_profiler_list = []
```

## towhee/runtime/schema_repr.py

```diff
@@ -47,19 +47,22 @@
             col_name (`str`): Schema name.
             iter_type (`Dict[str, Any]`): The iteration type of this node.
             inputs_type (`List`): A list of the inputs schema type.
 
         Returns:
             SchemaRepr object.
         """
-        if iter_type in ['flat_map', 'window', 'window_all', 'time_window', 'concat']:
+        if iter_type in ['flat_map', 'window', 'time_window']:
             col_type = ColumnType.QUEUE
-        elif inputs_type is None:
+        elif iter_type == 'concat':
+            col_type = inputs_type[0]
+        elif iter_type == 'window_all':
             col_type = ColumnType.SCALAR
         elif iter_type in ['map', 'filter']:
-            col_type = ColumnType.SCALAR
-            if ColumnType.QUEUE in inputs_type:
+            if inputs_type is not None and ColumnType.QUEUE in inputs_type:
                 col_type = ColumnType.QUEUE
+            else:
+                col_type = ColumnType.SCALAR
         else:
             engine_log.error('Unknown iteration type: %s', iter_type)
             raise ValueError(f'Unknown iteration type: {iter_type}')
         return SchemaRepr(col_name, col_type)
```

## towhee/runtime/nodes/_filter.py

```diff
@@ -35,39 +35,38 @@
                  op_pool: 'OperatorPool',
                  in_ques: List['DataQueue'],
                  out_ques: List['DataQueue'],
                  time_profiler: 'TimeProfiler'):
         super().__init__(node_repr, op_pool, in_ques, out_ques, time_profiler)
         self._input_q = self._in_ques[0]
         self._key_map = dict(zip(self._node_repr.outputs, self._node_repr.inputs))
-        self._same_keys = list(set(self._input_q.schema) & set(self._node_repr.outputs))
+        self._side_by_keys = list(set(self._input_q.schema) - set(self._node_repr.outputs))
 
     def process_step(self) -> bool:
         self._time_profiler.record(self.uid, Event.queue_in)
         data = self._input_q.get_dict()
         if data is None:
             self._set_finished()
             return True
+        side_by = dict((k, data[k]) for k in self._side_by_keys)
 
         process_data = [data.get(key) for key in self._node_repr.iter_info.param[FilterConst.param.filter_by]]
         if not any((i is Empty() for i in process_data)):
             self._time_profiler.record(self.uid, Event.process_in)
-            succ, outputs, msg = self._call(process_data)
+            succ, is_need, msg = self._call(process_data)
             self._time_profiler.record(self.uid, Event.process_out)
             if not succ:
                 self._set_failed(msg)
                 return True
 
-            if outputs:
+            if is_need:
                 output_map = {new_key: data[old_key] for new_key, old_key in self._key_map.items()}
-                data.update(output_map)
-            else:
-                for k in self._same_keys:
-                    del data[k]
+                side_by.update(output_map)
+
         self._time_profiler.record(self.uid, Event.queue_out)
 
         for out_que in self._output_ques:
-            if not out_que.put_dict(data):
+            if not out_que.put_dict(side_by):
                 self._set_stopped()
                 return True
 
         return False
```

## towhee/runtime/nodes/_flat_map.py

```diff
@@ -25,25 +25,31 @@
     FlatMap transforms the iterable/nested outputs into one or more elements, i.e. split elements, unnest iterables.
 
     i.e.
             ---[0, 1, 2, 3]--->
         [    FlatMap('input', 'output', lambda i: i)    ]
             ---0---1---2---3--->
     """
+    def __init__(self, node_repr, op_pool, in_ques, out_ques, time_profiler):
+        super().__init__(node_repr, op_pool, in_ques, out_ques, time_profiler)
+        self._input_q = self._in_ques[0]
+        self._side_by_keys = list(set(self._input_q.schema) - set(self._node_repr.outputs))
+
     def process_step(self) -> List[Any]:
         self._time_profiler.record(self.uid, Event.queue_in)
         data = self._in_ques[0].get_dict()
         if data is None:
             self._set_finished()
             return True
 
+        side_by = dict((k, data[k]) for k in self._side_by_keys)
         process_data = [data.get(key) for key in self._node_repr.inputs]
         if any((i is Empty() for i in process_data)):
             for out_que in self._output_ques:
-                if not out_que.put_dict(data):
+                if not out_que.put_dict(side_by):
                     self._set_stopped()
                     return True
         else:
             self._time_profiler.record(self.uid, Event.process_in)
             succ, outputs, msg = self._call(process_data)
             if not succ:
                 self._set_failed(msg)
@@ -53,19 +59,19 @@
 
             for output in outputs:
                 if size > 1:
                     output_map = {self._node_repr.outputs[i]: output[i] for i in range(size)}
                 else:
                     output_map = {self._node_repr.outputs[0]: output}
 
-                data.update(output_map)
+                side_by.update(output_map)
 
                 for out_que in self._output_ques:
-                    if not out_que.put_dict(data):
+                    if not out_que.put_dict(side_by):
                         self._set_stopped()
                         return True
 
-                data = {}
+                side_by = {}
             self._time_profiler.record(self.uid, Event.process_out)
             self._time_profiler.record(self.uid, Event.queue_out)
 
         return False
```

## towhee/runtime/nodes/_map.py

```diff
@@ -40,50 +40,60 @@
                     num += 1
 
                ---1---2---3---4--->
            [   map('input', 'output', func)    ]
                ---[0]---[0, 1]---[0, 1, 2]---[0, 1, 2, 3]--->
     """
 
+    def __init__(self, node_repr, op_pool, in_ques, out_ques, time_profiler):
+        super().__init__(node_repr, op_pool, in_ques, out_ques, time_profiler)
+        self._input_q = self._in_ques[0]
+        self._side_by_keys = list(set(self._input_q.schema) - set(self._node_repr.outputs))
+
     def process_step(self) -> bool:
         """
         Called for each element.
         """
         self._time_profiler.record(self.uid, Event.queue_in)
         data = self._in_ques[0].get_dict()
         if data is None:
             self._set_finished()
             return True
 
+        side_by = dict((k, data[k]) for k in self._side_by_keys)
+
         process_data = [data.get(key) for key in self._node_repr.inputs]
         if not any((i is Empty() for i in process_data)):
             self._time_profiler.record(self.uid, Event.process_in)
             succ, outputs, msg = self._call(process_data)
             if not succ:
                 self._set_failed(msg)
                 return True
             if isinstance(outputs, Generator):
                 outputs = self._get_from_generator(outputs, len(self._node_repr.outputs))
             self._time_profiler.record(self.uid, Event.process_out)
 
             size = len(self._node_repr.outputs)
             if size > 1:
                 output_map = dict((self._node_repr.outputs[i], outputs[i])
-                                for i in range(size))
+                                  for i in range(size))
             elif size == 0:
                 output_map = {}
             else:
                 output_map = {}
                 output_map[self._node_repr.outputs[0]] = outputs
 
-            data.update(output_map)
+            side_by.update(output_map)
         self._time_profiler.record(self.uid, Event.queue_out)
 
+        if not side_by:
+            return False
+
         for out_que in self._output_ques:
-            if not out_que.put_dict(data):
+            if not out_que.put_dict(side_by):
                 self._set_stopped()
                 return True
 
         return False
 
     def _get_from_generator(self, gen, size):
         if size == 1:
```

## towhee/runtime/nodes/_output.py

```diff
@@ -19,14 +19,19 @@
 
 class Output(Node):
     """Output the data as input
 
        Examples:
            p1 = towhee.pipe.input('url').output('url')
     """
+    def initialize(self) -> bool:
+        for q in self._output_ques:
+            q.max_size = 0
+        return super().initialize()
+
     def process_step(self) -> bool:
         self._time_profiler.record(self.uid, Event.queue_in)
         all_data = {}
         for q in self._in_ques:
             data = q.get_dict()
             if data:
                 all_data.update(data)
```

## towhee/runtime/nodes/_time_window.py

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from towhee.runtime.constants import TimeWindowConst
+from towhee.runtime.data_queue import Empty
 
 from ._window import Window
 
 
 class TimeWindow(Window):
     """Window operator
 
@@ -57,14 +58,18 @@
                     return self._to_cols(ret)
                 else:
                     return None
 
             self._row_buffer.append(data)
 
             timestamp = data[self._timestamp_index]
+            if timestamp is Empty():
+                # end of the timestamp col
+                continue
+
             if self._buffer(data, timestamp) and self._buffer.data:
                 ret = self._buffer.data
                 self._buffer = self._buffer.next()
                 return self._to_cols(ret)
 
 
 class _TimeWindowBuffer:
```

## towhee/runtime/nodes/_window.py

```diff
@@ -102,14 +102,17 @@
                         self._set_stopped()
                         return True
                 self._row_buffer = []
             self._set_finished()
             return True
 
         process_data = [in_buffer.get(key) for key in self._node_repr.inputs]
+        if not any(process_data):
+            return False
+
         self._time_profiler.record(self.uid, Event.process_in)
         succ, outputs, msg = self._call(process_data)
         self._time_profiler.record(self.uid, Event.process_out)
         if not succ:
             self._set_failed(msg)
             return True
```

## towhee/runtime/nodes/_window_all.py

```diff
@@ -49,15 +49,15 @@
 
     def _get_buffer(self):
         data = self._input_que.get()
         if not data:
             return None
         else:
             assert len(self._schema) == len(data)
-            cols = [[i] for i in data]
+            cols = [[i] if i is not Empty() else [] for i in data]
 
         while True:
             data = self._input_que.get()
             if data is None:
                 break
 
             for i in range(len(self._schema)):
@@ -76,14 +76,17 @@
         self._time_profiler.record(self.uid, Event.queue_in)
         in_buffer = self._get_buffer()
         if in_buffer is None:
             self._set_finished()
             return True
 
         process_data = [in_buffer.get(key) for key in self._node_repr.inputs]
+        if not any(process_data):
+            return False
+
         self._time_profiler.record(self.uid, Event.process_in)
         succ, outputs, msg = self._call(process_data)
         self._time_profiler.record(self.uid, Event.process_out)
         if not succ:
             self._set_failed(msg)
             return True
```

## towhee/runtime/operator_manager/operator_loader.py

```diff
@@ -14,149 +14,143 @@
 
 import importlib
 import sys
 import subprocess
 from pathlib import Path
 from typing import Any, List, Dict, Union
 import re
+import traceback
 import pkg_resources
 
 from towhee.operator import Operator
 from towhee.operator.nop import NOPNodeOperator
-from towhee.hub.file_manager import FileManager
+from towhee.hub import get_operator
 from towhee.runtime.constants import InputConst, OutputConst
+from towhee.utils.log import engine_log
 from .operator_registry import OperatorRegistry
 
 
 class OperatorLoader:
     """
     Wrapper class used to load operators from either local cache or a remote
     location.
 
     Args:
         cache_path: (`str`)
             Local cache path to use. If not specified, it will default to
             `$HOME/.towhee/operators`.
     """
 
-    def _load_interal_op(self, op_name: str, arg: List[Any], kws: Dict[str, Any]): # pylint: disable=unused-argument
-        if op_name in [InputConst.name, OutputConst.name]:
+    def _load_operator_from_internal(self, function: str, arg: List[Any], kws: Dict[str, Any], tag: str) -> Operator:  # pylint: disable=unused-argument
+        if function in [InputConst.name, OutputConst.name]:
             return NOPNodeOperator()
         else:
-            # Not a interal operator
             return None
 
-    def load_operator_from_internal(self, function: str, arg: List[Any], kws: Dict[str, Any], tag: str) -> Operator:  # pylint: disable=unused-argument
-        return self._load_interal_op(function, arg, kws)
-
-    def load_operator_from_registry(self, function: str, arg: List[Any], kws: Dict[str, Any], tag: str) -> Operator:  # pylint: disable=unused-argument
+    def _load_operator_from_registry(self, function: str, arg: List[Any], kws: Dict[str, Any], tag: str) -> Operator:  # pylint: disable=unused-argument
         op = OperatorRegistry.resolve(function)
-        return self.instance_operator(op, arg, kws) if op is not None else None
+        return self._instance_operator(op, arg, kws) if op is not None else None
 
-    def load_operator_from_packages(self, function: str, arg: List[Any], kws: Dict[str, Any], tag: str) -> Operator:  # pylint: disable=unused-argument
-        try:
-            module, fname = function.split('/')
-            fname = fname.replace('-', '_')
-            op_cls = ''.join(x.capitalize() or '_' for x in fname.split('_'))
-
-            # module = '.'.join([module, fname, fname])
-            module = '.'.join(['towheeoperator', '{}_{}'.format(module, fname), fname])
-            op = getattr(importlib.import_module(module), op_cls)
-            return self.instance_operator(op, arg, kws) if op is not None else None
-        except Exception:  # pylint: disable=broad-except
+    def _load_legacy_op(self, modname, path, fname):
+        # support old version operator API
+        file_name = path / (fname + '.py')
+        spec = importlib.util.spec_from_file_location(modname, file_name.resolve())
+        # Create the module and then execute the module in its own namespace.
+
+        module = importlib.util.module_from_spec(spec)
+        sys.modules[modname] = module
+        spec.loader.exec_module(module)
+        # Instantiate the operator object and return it to the caller for
+        # `load_operator`. By convention, the operator class is simply the CamelCase
+        # version of the snake_case operator.
+        op_cls = ''.join(x.capitalize() or '_' for x in fname.split('_'))
+        op = getattr(module, op_cls)
+        return op
+
+    def _load_op(self, modname, path, fname):
+        # support latest version operator API
+        init_path = path / '__init__.py'
+        if not init_path.is_file():
             return None
+        spec = importlib.util.spec_from_file_location(modname, init_path)
+        module = importlib.util.module_from_spec(spec)
+        sys.modules[modname] = module
+        spec.loader.exec_module(module)
+        op = getattr(module, fname, None)
+
+        return op
 
-    def load_operator_from_path(self, path: Union[str, Path], arg: List[Any], kws: Dict[str, Any]) -> Operator:
+    def _load_operator_from_path(self, path: Union[str, Path], function: str, arg: List[Any], kws: Dict[str, Any]) -> Operator:
         """
         Load operator form local path.
         Args:
             path (`Union[str, Path]`):
                 Path to the operator python file.
             arg (`List[str, Any]`):
                 The init args for OperatorClass.
             kws (`Dict[str, Any]`):
                 The init kwargs for OperatorClass.
         Returns
             (`typing.Any`)
                 The `Operator` output.
         """
         path = Path(path)
-        fname = Path(path).stem
-        modname = 'towhee.operator.' + fname
+        fname = function.split('/')[1].replace('-', '_')
+        op_name = function.replace('-', '_').replace('/', '.')
+        modname = 'towhee.operator.' + op_name
 
         all_pkg = [item.project_name for item in list(pkg_resources.working_set)]
         if 'requirements.txt' in (i.name for i in path.parent.iterdir()):
             with open(path.parent / 'requirements.txt', 'r', encoding='utf-8') as f:
                 reqs = f.read().split('\n')
             for req in reqs:
                 if not req:
                     continue
                 pkg_name = re.split(r'(~|>|<|=|!| )', req)[0]
                 pkg_name = pkg_name.replace('_', '-')
                 if pkg_name not in all_pkg:
                     subprocess.check_call([sys.executable, '-m', 'pip', 'install', req])
-        try:
-            # support for ver1 operator API
-            spec = importlib.util.spec_from_file_location(modname, path.resolve())
 
-            # Create the module and then execute the module in its own namespace.
-            module = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(module)
-
-            # Instantiate the operator object and return it to the caller for
-            # `load_operator`. By convention, the operator class is simply the CamelCase
-            # version of the snake_case operator.
-            op_cls = ''.join(x.capitalize() or '_' for x in fname.split('_'))
-            op = getattr(module, op_cls)
-        except Exception:  # pylint: disable=broad-except
-            # support for ver2 operator API
-            path = path.parent / '__init__.py'
-            spec = importlib.util.spec_from_file_location(modname, path.resolve())
-            module = importlib.util.module_from_spec(spec)
-            sys.modules[modname] = module
-            spec.loader.exec_module(module)
-            op = getattr(module, fname)
+        op = self._load_op(modname, path, fname)
+        if not op:
+            engine_log.warning('Load operator %s:%s:%s failed, try to use the legacy type' , modname, path, fname)
+            op = self._load_legacy_op(modname, path, fname)
 
-        return self.instance_operator(op, arg, kws) if op is not None else None
+        return self._instance_operator(op, arg, kws) if op is not None else None
 
-    def load_operator_from_cache(self, function: str, arg: List[Any], kws: Dict[str, Any], tag: str) -> Operator:  # pylint: disable=unused-argument
+    def _load_operator_from_hub(self, function: str, arg: List[Any], kws: Dict[str, Any], tag: str) -> Operator:
         if '/' not in function:
             function = 'towhee/'+function
         try:
-            fm = FileManager()
-            path = fm.get_operator(operator=function, tag=tag)
-        except ValueError as e:
-            raise ValueError('operator {} not found!'.format(function)) from e
-
-        if path is None:
-            raise FileExistsError('Cannot find operator.')
+            path = get_operator(operator=function, tag=tag)
+        except Exception as e:  # pylint: disable=broad-except
+            err = '{}, {}'.format(str(e), traceback.format_exc())
+            engine_log.error(err)
+            return None
 
-        return self.load_operator_from_path(path, arg, kws)
+        return self._load_operator_from_path(path, function, arg, kws)
 
     def load_operator(self, function: str, arg: List[Any], kws: Dict[str, Any], tag: str) -> Operator:
         """
         Attempts to load an operator from cache. If it does not exist, looks up the
         operator in a remote location and downloads it to cache instead. By standard
         convention, the operator must be called `Operator` and all associated data must
         be contained within a single directory.
 
         Args:
             function: (`str`)
                 Origin and method/class name of the operator. Used to look up the proper
                 operator in cache.
-        Raises:
-            FileExistsError
-                Cannot find operator.
         """
-        for factory in [self.load_operator_from_internal,
-                        self.load_operator_from_registry,
-                        self.load_operator_from_packages,
-                        self.load_operator_from_cache]:
+        for factory in [self._load_operator_from_internal,
+                        self._load_operator_from_registry,
+                        self._load_operator_from_hub]:
             op = factory(function, arg, kws, tag)
             if op is not None:
                 return op
-        return None
+        if op is None:
+            raise RuntimeError('Load operator failed')
 
-    def instance_operator(self, op, arg: List[Any], kws: Dict[str, Any]) -> Operator:
+    def _instance_operator(self, op, arg: List[Any], kws: Dict[str, Any]) -> Operator:
         if arg is None:
             arg = ()
         return op(*arg, **kws) if kws is not None else op(*arg)
```

## towhee/runtime/operator_manager/operator_registry.py

```diff
@@ -38,21 +38,27 @@
         ]:
             if n in OperatorRegistry.REGISTRY:
                 return OperatorRegistry.REGISTRY[n]
         return None
 
     @staticmethod
     def register(
-            name: str = None):
+            name: str = None,
+            input_schema=None,  # pylint: disable=unused-argument
+            output_schema=None, # pylint: disable=unused-argument
+            flag=None # pylint: disable=unused-argument
+    ):
         """
         Register a class, function, or callable as a towhee operator.
 
         Args:
             name (str, optional): operator name, will use the class/function name if None.
 
+            input_schema, output_schema, flag for legacy operators.
+
         Returns:
             [type]: [description]
         """
         if callable(name):
             # the decorator is called directly without any arguments,
             # relaunch the register
             cls = name
```

## towhee/serve/triton/__init__.py

```diff
@@ -7,7 +7,17 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+
+from towhee.utils.lazy_import import LazyImport
+
+triton_client = LazyImport('triton_client', globals(), 'towhee.serve.triton.pipeline_client')
+
+
+__all__ = [
+    'triton_client'
+]
```

## towhee/serve/triton/constant.py

```diff
@@ -9,24 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-EMPTY_OPS = ['dummy_input', 'end']
-NNOPERATOR = 'NNOperator'
-PYOPERATOR = 'PyOperator'
-
-
-PREPROCESS = 'preprocess'
-POSTPROCESS = 'postprocess'
-
-
 OP_CONFIG = 'op_config'
+SERVER_CONFIG = 'server_config'
 FORMAT_PRIORITY = 'format_priority'
+PARALLELISM = 'parallelism'
 
 
 # bls
 
 OP_CONFIG_FILE = 'config.json'
 DC_CONFIG_FILE = 'dc_config.json'
+
+PIPELINE_NAME = 'pipeline'
```

## towhee/serve/triton/docker_image_builder.py

```diff
@@ -15,42 +15,48 @@
 import json
 import shutil
 import subprocess
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 from towhee.serve.triton.dockerfiles import get_dockerfile
-
+# pylint: disable=import-outside-toplevel
+# pylint: disable=unspecified-encoding
 
 class DockerImageBuilder:
     '''
     Build triton image
     '''
-    def __init__(self, towhee_pipeline: 'towhee.dc', image_name: str, cuda: str):
+    def __init__(self, towhee_pipeline: 'towhee.RuntimePipeline', image_name: str, server_config: dict, cuda_version: str):
         self._towhee_pipeline = towhee_pipeline
         self._image_name = image_name
-        self._cuda = cuda
+        self._server_config = server_config
+        self._cuda_version = cuda_version
 
     def prepare_dag(self, workspace: Path):
-        dag = self._towhee_pipeline.dag_info
-        for v in dag.values():
-            del v['call_args']
-        with open(workspace / 'dag.json', 'wt', encoding='utf-8') as f:
-            json.dump(dag, f)
+        from towhee.utils.thirdparty.dill_util import dill as pickle
+        dag = self._towhee_pipeline.dag_repr
+        with open(workspace / 'dag.pickle', 'wb') as f:
+            pickle.dump(dag, f, recurse=True)
+
+    def prepare_config(self, workspace: Path):
+        config = self._server_config
+        with open(workspace / 'server_config.json', 'w') as f:
+            json.dump(config, f)
 
     def build_image(self, workspace: Path):
-        cmd = 'cd {} && docker build -t {} .'.format(workspace,
-                                                     self._image_name)
+        cmd = 'cd {} && docker build -t {} .'.format(workspace, self._image_name)
         subprocess.run(cmd, shell=True, check=True)
 
     def docker_file(self) -> Path:
-        return get_dockerfile(self._cuda)
+        return get_dockerfile(self._cuda_version)
 
     def build(self) -> bool:
         with TemporaryDirectory(dir='./') as workspace:
             self.prepare_dag(Path(workspace))
+            self.prepare_config(Path(workspace))
             file_path = self.docker_file()
             if file_path is None:
                 return False
             shutil.copy(file_path, Path(workspace) / 'Dockerfile')
             self.build_image(workspace)
             return True
```

## towhee/serve/triton/triton_config_builder.py

```diff
@@ -8,100 +8,68 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Dict, List, Tuple, Any
-
-import towhee.serve.triton.type_gen as tygen
-
-
-class TritonModelConfigBuilder:
-    """
-    This class is used to generate a triton model config file.
-    """
-
-    def __init__(self, model_spec: Dict):
-        self.model_spec = model_spec
-
-    @staticmethod
-    def _get_triton_schema(schema: List[Tuple[Any, Tuple]], var_prefix):
-
-        type_info_list = tygen.get_type_info(schema)
-        attr_info_list = [attr_info for type_info in type_info_list for attr_info in type_info.attr_info]
-
-        schema = {}
-        for i, attr_info in enumerate(attr_info_list):
-            var = var_prefix + str(i)
-            dtype = attr_info.triton_dtype
-            shape = list(attr_info.shape)
-            schema[var] = (dtype, shape)
-
-        return schema
-
-    @staticmethod
-    def get_input_schema(schema: List[Tuple[Any, Tuple]]):
-        return TritonModelConfigBuilder._get_triton_schema(schema, 'INPUT')
-
-    @staticmethod
-    def get_output_schema(schema: List[Tuple[Any, Tuple]]):
-        return TritonModelConfigBuilder._get_triton_schema(schema, 'OUTPUT')
-
 
 def create_modelconfig(model_name, max_batch_size, inputs, outputs, backend,
                        enable_dynamic_batching=False, preferred_batch_size=None,
                        max_queue_delay_microseconds=None,
                        instance_count=1, device_ids=None):
     '''
     example of input and output:
         {
             INPUT0': ('TYPE_INT8', [-1, -1, 3]),
             INPUT1': ('TYPE_FP32', [-1, -1, 3])
         }
     '''
     config = 'name: "{}"\n'.format(model_name)
     config += 'backend: "{}"\n'.format(backend)
-    config += 'max_batch_size: {}\n'.format(max_batch_size)
+    if max_batch_size is not None:
+        config += 'max_batch_size: {}\n'.format(max_batch_size)
     if enable_dynamic_batching:
         config += '''
 dynamic_batching {
 '''
         if preferred_batch_size is not None:
             config += '''
     preferred_batch_size: {}
 '''.format(preferred_batch_size)
         if max_queue_delay_microseconds is not None:
             config += '''
     max_queue_delay_microseconds: {}
 '''.format(max_queue_delay_microseconds)
         config += '''
 }\n'''
-    for input_name in inputs.keys():
-        data_type, shape = inputs[input_name]
-        config += '''
+    if inputs is not None:
+        for input_name in inputs.keys():
+            data_type, shape = inputs[input_name]
+            config += '''
 input [
   {{
     name: \"{}\"
     data_type: {}
     dims: {}
   }}
 ]\n'''.format(input_name, data_type, shape)
-    for output_name in outputs.keys():
-        data_type, shape = outputs[output_name]
-        config += '''
+    if outputs is not None:
+        for output_name in outputs.keys():
+            data_type, shape = outputs[output_name]
+            config += '''
 output [
   {{
     name: \"{}\"
     data_type: {}
     dims: {}
   }}
 ]\n'''.format(output_name, data_type, shape)
 
+    instance_count = 1 if instance_count is None else instance_count
     if device_ids is not None:
         config += '''
 instance_group [
     {{
         kind: KIND_GPU
         count: {}
         gpus: {}
@@ -113,198 +81,7 @@
     {{
         kind: KIND_CPU
         count: {}
     }}
 ]\n'''.format(instance_count)
 
     return config
-
-
-class EnsembleConfigBuilder:
-    '''
-    Create ensemble config. Currently, we just support a chain struct graph.
-
-    Example of input dag:
-    triton_dag = {
-    0: {
-        'id': 0,
-        'mode_name': 'image_decode',
-        'model_version': 1,
-        'inputs': {
-            'INPUT0': ('TYPE_STRING', []),
-        },
-        'outputs': {
-            'OUTPUT0': ('TYPE_INT8', [-1, -1, 3]),
-            'OUTPUT1': ('TYPE_STRING', []),
-        },
-        'child_ids': [1]
-    },
-    1: {
-        'id': 1,
-        'mode_name': 'clip_preprocess',
-        'model_version': 1,
-        'inputs': {
-            'IUTPUT0': ('TYPE_INT8', [-1, -1, 3]),
-            'IUTPUT1': ('TYPE_STRING', []),
-        },
-        'outputs': {
-            'OUTPUT0': ('TYPE_FP32', [-1, 3, 224, 224])
-        },
-        'child_ids': [2]
-    },
-    2: {
-        'id': 2,
-        'mode_name': 'clip_model',
-        'model_version': 1,
-        'inputs': {
-            'IUTPUT0': ('TYPE_FP32', [-1, 3, 224, 224])
-        },
-        'outputs': {
-            'OUTPUT0': ('TYPE_FP32', [-1, 512])
-        },
-        'child_ids': [3]
-    },
-    3: {
-        'id': 3,
-        'mode_name': 'clip_postprocess',
-        'model_version': 1,
-        'inputs': {
-            'IUTPUT0': ('TYPE_FP32', [-1, 512])
-        },
-        'outputs': {
-            'OUTPUT0': ('TYPE_FP32', [512])
-        },
-        'child_ids': []
-    }
-}
-    '''
-    def __init__(self, dag, model_name, max_batch_size):
-        self._dag = dag
-        self._model_name = model_name
-        self._max_batch_size = max_batch_size
-        self._head = None
-        self._tail = None
-
-    def _process_dag(self):
-        '''
-        Find out head and tail.
-        Add input_map and output_map for every node.
-        '''
-        all_keys = list(self._dag.keys())
-        no_root = []
-        for k, v in self._dag.items():
-            if v['child_ids']:
-                no_root.extend(v['child_ids'])
-                for name in v['child_ids']:
-                    if self._dag[name].get('parent_ids') is None:
-                        self._dag[name]['parent_ids'] = []
-                    self._dag[name]['parent_ids'].append(k)
-            else:
-                self._tail = v
-        head = set(all_keys) - set(no_root)
-        assert len(head) == 1
-        self._head = self._dag[list(head)[0]]
-        self._dag[list(head)[0]]['parent_ids'] = []
-        self._head['input_map'] = [(input, input) for input in self._head['input'].keys()]
-        self._tail['output_map'] = [(output, output) for output in self._tail['output'].keys()]
-
-        # add output_map
-        for name, v in self._dag.items():
-            if name == self._tail['id']:
-                continue
-            output_map = []
-            for output in v['output']:
-                output_map.append((output, '_'.join([str(name), output])))
-            v['output_map'] = output_map
-
-        # add input_map
-        for name, v in self._dag.items():
-            if len(v['parent_ids']) == 0:
-                continue
-            input_map = []
-            assert len(v['parent_ids']) == 1
-            parent_id = v['parent_ids'][0]
-            parent_outputs = self._dag[parent_id]['output_map']
-            inputs = list(v['input'].keys())
-            assert len(parent_outputs) == len(inputs)
-            for i in range(len(parent_outputs)):
-                input_map.append((inputs[i], parent_outputs[i][1]))
-            v['input_map'] = input_map
-
-    def _gen_header(self):
-        config = 'name: "{}"\n'.format(self._model_name)
-        config += 'platform: "ensemble"\n'
-        config += 'max_batch_size: {}\n'.format(self._max_batch_size)
-        for input_name in self._head['input'].keys():
-            data_type, shape = self._head['input'][input_name]
-            config += '''
-input [
-  {{
-    name: \"{}\"
-    data_type: {}
-    dims: {}
-  }}
-]\n'''.format(input_name, data_type, shape)
-        for output_name in self._tail['output'].keys():
-            data_type, shape = self._tail['output'][output_name]
-            config += '''
-output [
-  {{
-    name: \"{}\"
-    data_type: {}
-    dims: {}
-  }}
-]\n'''.format(output_name, data_type, shape)
-        return config
-
-    def _gen_single_step(self, model_name, inputs, outputs, is_tail):
-        config = '''    {{
-      model_name: \"{}\"
-      model_version: {}
-'''.format(model_name, 1)
-
-        for data in inputs:
-            config += '''
-      input_map {{
-        key: \"{}\"
-        value: \"{}\"
-      }}
-'''.format(data[0], data[1])
-
-        for output in outputs:
-            config += '''
-      output_map {{
-        key: \"{}\"
-        value: \"{}\"
-      }}
-'''.format(output[0], output[1])
-
-        config += '    }'
-        if not is_tail:
-            config += ',\n'
-        else:
-            config += '\n'
-        return config
-
-    def _gen_steps(self):
-        config = '''
-  step [\n'''
-        items = list(self._dag.values())
-        size = len(items)
-        for i in range(size):
-            step = items[i]
-            config += self._gen_single_step(step['model_name'], step['input_map'], step['output_map'], i == size - 1)
-        config += '  ]\n'
-        return config
-
-    def _gen_ensemble_scheduling(self):
-        config = '''
-ensemble_scheduling: {\n'''
-        config += self._gen_steps()
-        config += '}'
-        return config
-
-    def gen_config(self):
-        self._process_dag()
-        config = self._gen_header()
-        config += self._gen_ensemble_scheduling()
-        return config
```

## towhee/serve/triton/bls/__init__.py

```diff
@@ -7,7 +7,13 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+
+import os
+
+
+PIPELINE_MODEL_FILE = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'pipeline_model.py')
```

## towhee/serve/triton/bls/mock/mock_pb_util.py

```diff
@@ -8,105 +8,165 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pylint: skip-file
+# pylint: disable=import-outside-toplevel
+# pylint: disable=broad-except
+from typing import List, Any
 
-from typing import List
 
-
-class MockTritonPythonBackendUtils:
-    '''
-    mock triton_python_backend_utils, used in UT.
-    '''
-
-    TRITONSERVER_RESPONSE_COMPLETE_FINAL = 1
-
-    @staticmethod
-    def get_input_tensor_by_name(r, input_key):
-        '''
-        Args:
-            r: MockInferenceRequest
-            input_key: str
-        return:
-            MockTritonPythonBackendTensor
-        '''
-        for item in r.inputs():
-            if item.name() == input_key:
-                return item
-        return None
-
-    @staticmethod
-    def InferenceResponse(output_tensors: List['MockTritonPythonBackendTensor'], err=None):  # pylint: disable=invalid-name
-        return MockInferenceResponse(output_tensors, err)
-
-    @staticmethod
-    def InferenceRequest(inputs: 'MockTritonPythonBackendTensor'):  # pylint: disable=invalid-name
-        return MockInferenceRequest(inputs)
-
-    @staticmethod
-    def TritonError(msg):  # pylint: disable=invalid-name
-        return MockTritonError(msg)
-
-    @staticmethod
-    def Tensor(name: str, data: 'ndarray'):  # pylint: disable=invalid-name
-        return MockTritonPythonBackendTensor(name, data)
-
-
-class MockTritonPythonBackendTensor:
-    '''
+class _MockTritonPythonBackendTensor:
+    """
     Mock python_backend tensor object.
-    '''
+    """
     def __init__(self, name:str, data: 'ndarray'):
         self._name = name
         self._data = data
 
     def name(self):
         return self._name
 
     def as_numpy(self):
         return self._data
 
-
-class MockResponseSender:
-    def __init__(self, callback):
-        self._callback = callback
+class _MockInferenceResponseSender:
+    """
+    MockInferenceResponseSender.
+    """
+    # def __init__(self, callback):
+    #     self._callback = callback
 
     def send(self, response=None, flags=0):
-        if flags != MockTritonPythonBackendUtils.TRITONSERVER_RESPONSE_COMPLETE_FINAL:
-            self._callback(response, None)
-        else:
-            self._callback(None, None)
-
-
-class MockInferenceRequest:
-    def __init__(self, tensors: MockTritonPythonBackendTensor, callback=None):
-        self._tensors = tensors
-        self._sender = MockResponseSender(callback)
+        # if flags != MockTritonPythonBackendUtils.TRITONSERVER_RESPONSE_COMPLETE_FINAL:
+        #     self._callback(response, None)
+        # else:
+        #     self._callback(None, None)
+        pass
+
+
+class _MockInferenceRequest:
+    """
+    MockInferenceResponse.
+    """
+    model_dict = {}
+
+    def __init__(self, inputs: _MockTritonPythonBackendTensor,
+                 requested_output_names: List[str],
+                 model_name: str):
+        self._tensors = inputs
+        self._requested_output_names = requested_output_names
+        self._model_name = model_name
+        self._model = self.model_dict.get(self._model_name, None)
+
+    @classmethod
+    def set_model(cls, model_name, model):
+        cls.model_dict[model_name] = model
 
     def inputs(self):
         return self._tensors
 
+    def exec(self):
+        try:
+            inputs = [tensor.as_numpy() for tensor in self._tensors]
+            outputs = self._model(*inputs)
+            if len(self._requested_output_names) == 1:
+                outputs = [outputs]
+            res = [MockTritonPythonBackendUtils.Tensor(name, arr) for name, arr in zip(self._requested_output_names, outputs)]
+            return MockTritonPythonBackendUtils.InferenceResponse(res)
+        except Exception as e:
+            return MockTritonPythonBackendUtils.InferenceResponse(None, MockTritonPythonBackendUtils.TritonError(e.message))
+
+    def requested_output_names(self):
+        pass
+
     def get_response_sender(self):
-        return self._sender
+        pass
 
 
-class MockInferenceResponse:
-    def __init__(self, tensors, err):
-        self._tensors = tensors
-        self._err = err
+class _MockInferenceResponse:
+    """
+    MockInferenceResponse.
+    """
+    def __init__(self, output_tensors, error=None):
+        self._tensors = output_tensors
+        self._err = error
 
     def output_tensors(self):
         return self._tensors
 
     def has_error(self):
         return self._err is not None
 
+    def error(self):
+        return self._err
 
-class MockTritonError:
+
+class _MockTritonError:
+    """
+    MockTritonError.
+    """
     def __init__(self, msg):
         self._msg = msg
 
     def message(self):
         return self._msg
+
+
+class _MockTritonModelException(Exception):
+    """
+    MockTritonModelException.
+    """
+    def __init__(self, msg):
+        self._msg = msg
+
+    def message(self):
+        return self._msg
+
+
+class MockTritonPythonBackendUtils:
+    """
+    mock triton_python_backend_utils, used in UT.
+    """
+
+    TRITONSERVER_RESPONSE_COMPLETE_FINAL = 1
+
+    InferenceResponse = _MockInferenceResponse
+    InferenceRequest = _MockInferenceRequest
+    TritonError = _MockTritonError
+    Tensor = _MockTritonPythonBackendTensor
+    TritonModelException = _MockTritonModelException
+
+    @staticmethod
+    def get_input_tensor_by_name(r, input_key):
+        """
+        Args:
+            r (`MockInferenceRequest`):
+                The InferenceRequest to get the tensor from.
+            input_key (`str`):
+                The name of the tensor.
+        return:
+            MockTritonPythonBackendTensor
+        """
+        for item in r.inputs():
+            if item.name() == input_key:
+                return item
+        return None
+
+    @staticmethod
+    def get_output_tensor_by_name(r, input_key):
+        """
+        Args:
+            r (`MockInferenceResponse`):
+                The InferenceResponse to get the tensor from.
+            input_key (`str`):
+                The name of the tensor.
+        return:
+            MockTritonPythonBackendTensor
+        """
+        for item in r.output_tensors():
+            if item.name() == input_key:
+                return item
+        return None
```

## towhee/serve/triton/bls/mock/mock_triton_client.py

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from typing import List, Dict
-from towhee.serve.triton.bls.mock import mock_pb_util
+from towhee.serve.triton.bls.python_backend_wrapper import pb_utils
 
 
 class MockInferInput:
     '''
     Mock InferInput
     '''
     def __init__(self, name, shape, datatype):
@@ -64,30 +64,30 @@
     '''
     def __init__(self, models: Dict):
         self._models = models
 
     def infer(self, model_name: str, inputs: List[MockInferInput]) -> 'InferResult':
         if model_name not in self._models:
             return None
-        request = mock_pb_util.MockInferenceRequest(
-            [mock_pb_util.MockTritonPythonBackendTensor(item.name(), item.data())
+        request = pb_utils.InferenceRequest(
+            [pb_utils.Tensor(item.name(), item.data())
              for item in inputs]
         )
 
         responses = self._models[model_name].execute([request])
         assert len(responses) == 1
         return MockInferResult(responses[0])
 
     def start_stream(self, callback):
         self._callback = CallbackWrapper(callback)
 
     def async_stream_infer(self, model_name, inputs: List[MockInferInput]):
         assert self._callback is not None
-        request = mock_pb_util.MockInferenceRequest(
-            [mock_pb_util.MockTritonPythonBackendTensor(item.name(), item.data())
+        request = pb_utils.InferenceRequest(
+            [pb_utils.Tensor(item.name(), item.data())
              for item in inputs],
             self._callback
         )
 
         self._models[model_name].execute([request])
 
     def stop_stream(self):
```

## towhee/serve/triton/dockerfiles/DockerfileCuda113

```diff
@@ -1,37 +1,28 @@
 FROM nvcr.io/nvidia/tritonserver:21.06.1-py3
 
-
-RUN apt-key adv --fetch-keys \
-    https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2004/x86_64/3bf863cc.pub && \
-    apt-get update                                && \
-    apt-get install -y software-properties-common && \
-    add-apt-repository ppa:deadsnakes/ppa         && \
-    apt-get update                                && \
+RUN apt-get update          && \
     apt-get install -y         \
               zip              \
               wget             \
               unzip            \
               python3.8        \
               python3-pip      \
               libgl1-mesa-glx
 
 RUN pip3 install -U pip
 
 RUN pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu113
 
-RUN pip3 install pyarrow onnxruntime
-
-RUN pip3 install towhee.compiler
-RUN pip3 install towhee towhee.models
-
-RUN apt-get install git-lfs && \
-    git lfs install
+RUN pip3 install onnxruntime onnx
 
 WORKDIR /workspace
 
 RUN mkdir -p /workspace/models
 
-COPY ./dag.json /workspace/dag.json
+COPY ./dag.pickle /workspace/dag.pickle
+
+COPY ./server_config.json /workspace/server_config.json
+
+RUN pip3 install towhee towhee.models
 
-RUN triton_builder /workspace/dag.json /workspace/models
- 
+RUN triton_builder /workspace/dag.pickle /workspace/models /workspace/server_config.json
```

## towhee/serve/triton/dockerfiles/DockerfileCuda114

```diff
@@ -1,36 +1,28 @@
 FROM nvcr.io/nvidia/tritonserver:21.10-py3
 
-RUN apt-key adv --fetch-keys \
-    https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2004/x86_64/3bf863cc.pub && \
-    apt-get update                                && \
-    apt-get install -y software-properties-common && \
-    add-apt-repository ppa:deadsnakes/ppa         && \
-    apt-get update                                && \
+RUN apt-get update          && \
     apt-get install -y         \
               zip              \
               wget             \
               unzip            \
               python3.8        \
               python3-pip      \
               libgl1-mesa-glx
 
 RUN pip3 install -U pip
 
 RUN pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu113
 
-RUN pip3 install pyarrow onnxruntime
-
-RUN pip3 install towhee.compiler
-RUN pip3 install towhee towhee.models
-
-RUN apt-get install git-lfs && \
-    git lfs install
+RUN pip3 install onnxruntime onnx
 
 WORKDIR /workspace
 
 RUN mkdir -p /workspace/models
 
-COPY ./dag.json /workspace/dag.json
+COPY ./dag.pickle /workspace/dag.pickle
+
+COPY ./server_config.json /workspace/server_config.json
+
+RUN pip3 install towhee towhee.models
 
-RUN triton_builder /workspace/dag.json /workspace/models
- 
+RUN triton_builder /workspace/dag.pickle /workspace/models /workspace/server_config.json
```

## towhee/serve/triton/dockerfiles/DockerfileCuda116

```diff
@@ -1,37 +1,28 @@
 FROM nvcr.io/nvidia/tritonserver:22.04-py3
 
-
-RUN apt-key adv --fetch-keys \
-    https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2004/x86_64/3bf863cc.pub && \
-    apt-get update                                && \
-    apt-get install -y software-properties-common && \
-    add-apt-repository ppa:deadsnakes/ppa         && \
-    apt-get update                                && \
+RUN apt-get update          && \
     apt-get install -y         \
               zip              \
               wget             \
               unzip            \
               python3.8        \
               python3-pip      \
               libgl1-mesa-glx
 
 RUN pip3 install -U pip
 
 RUN pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu116
 
-RUN pip3 install pyarrow onnxruntime
-
-RUN pip3 install towhee.compiler
-RUN pip3 install towhee towhee.models
-
-RUN apt-get install git-lfs && \
-    git lfs install
+RUN pip3 install onnxruntime onnx
 
 WORKDIR /workspace
 
 RUN mkdir -p /workspace/models
 
-COPY ./dag.json /workspace/dag.json
+COPY ./dag.pickle /workspace/dag.pickle
+
+COPY ./server_config.json /workspace/server_config.json
 
-RUN triton_builder /workspace/dag.json /workspace/models
+RUN pip3 install towhee towhee.models
 
+RUN triton_builder /workspace/dag.pickle /workspace/models /workspace/server_config.json
```

## towhee/serve/triton/dockerfiles/__init__.py

```diff
@@ -23,14 +23,16 @@
 def get_dockerfile(cuda_version: str) -> Path:
     if cuda_version == '11.3':
         file_name = 'DockerfileCuda113'
     elif cuda_version == '11.4':
         file_name = 'DockerfileCuda114'
     elif cuda_version == '11.6':
         file_name = 'DockerfileCuda116'
-    elif cuda_version == 'dev':
+    elif cuda_version == '11.7':
+        file_name = 'DockerfileCuda117'
+    elif cuda_version == '117dev':
         # for QA to test towhee
-        file_name = 'DockerfileCuda114dev'
+        file_name = 'DockerfileCuda117dev'
     else:
-        logger.error("Towhee serve doesn't support cuda %s, the support cuda: 11.3, 11.4, 11.6", cuda_version)
+        logger.error("Towhee serve doesn't support cuda %s, the support cuda: 11.3, 11.4, 11.6, 11.7", cuda_version)
         return None
     return Path(__file__).absolute().parent / file_name
```

## towhee/trainer/__init__.py

```diff
@@ -21,9 +21,10 @@
 try:
     import torchvision
 except ModuleNotFoundError:
     os.system("pip install torchvision")
 
 try:
     import torchmetrics
+    assert torchmetrics.__version__ == "0.7.0"
 except ModuleNotFoundError:
-    os.system("pip install torchmetrics")
+    os.system("pip install torchmetrics==0.7.0")
```

## towhee/trainer/callback.py

```diff
@@ -15,16 +15,15 @@
 import importlib
 from typing import Dict, Tuple, List, Callable
 
 import numpy as np
 import torch
 from torch import nn
 from torch.optim import Optimizer
-from tqdm import tqdm
-
+from tqdm.auto import tqdm
 from towhee.utils.log import trainer_log
 from towhee.trainer.utils.trainer_utils import is_main_process
 from towhee.trainer.utils.file_utils import is_tensorboard_available
 
 __all__ = [
     "Callback",
     "CallbackList",
@@ -758,26 +757,27 @@
         self.description = ""
 
     def on_train_batch_end(self, batch: Tuple, logs: Dict) -> None:
         if is_main_process():
             self.now_tqdm_train_dataloader.update(1)
             self.description = "[epoch {}/{}] loss={}, metric={}".format(logs["epoch"],
                                                                          int(self.total_epoch_num),
-                                                                         round(logs["epoch_loss"], 3),
-                                                                         round(logs["epoch_metric"], 3))
+                                                                         format(logs["epoch_loss"], ".3f"),
+                                                                         format(logs["epoch_metric"], ".3f"))
             self.now_tqdm_train_dataloader.set_description(self.description)
 
     def on_epoch_begin(self, epochs: int, logs: Dict) -> None:
         if is_main_process():
             self.now_tqdm_train_dataloader = None
             self.now_tqdm_train_dataloader = tqdm(self.raw_train_dataloader,
                                                   total=len(self.raw_train_dataloader),
-                                                  unit="step")  # , file=sys.stdout)
+                                                  unit="step",
+                                                  )  # , file=sys.stdout)
 
     def on_eval_batch_end(self, batch: Tuple, logs: Dict) -> None:
         if is_main_process():
             self.description = "[epoch {}/{}] loss={}, metric={}, eval_loss={}, eval_metric={}".format(
                 logs["epoch"],
                 int(self.total_epoch_num),
-                round(logs["epoch_loss"], 3),
-                round(logs["epoch_metric"], 3), round(logs["eval_epoch_loss"], 3), round(logs["eval_epoch_metric"], 3))
+                format(logs["epoch_loss"], ".3f"),
+                format(logs["epoch_metric"], ".3f"), format(logs["eval_epoch_loss"], ".3f"), format(logs["eval_epoch_metric"], ".3f"))
             self.now_tqdm_train_dataloader.set_description(self.description)
```

## towhee/trainer/metrics.py

```diff
@@ -179,18 +179,18 @@
         cls._metrics_list['WordInfoLost'] = tm.WordInfoLost
         cls._metrics_list['WordInfoPreserved'] = tm.WordInfoPreserved
         cls._metrics_list['MinMaxMetric'] = tm.MinMaxMetric
         cls._metrics_list['MeanAveragePrecision'] = MeanAveragePrecision
 
         return list(cls._metrics_list.keys())
 
-    def __init__(self, metric_name: str):
+    def __init__(self, metric_name: str, **kwargs):
         super().__init__(metric_name)
         assert metric_name in TMMetrics._metrics_list
-        self._metric = TMMetrics._metrics_list[metric_name]()
+        self._metric = TMMetrics._metrics_list[metric_name](**kwargs)
 
     def update(self, *_: Any, **__: Any) -> None:
         self._metric.update(*_,**__)
 
     def compute(self) -> str:
         return self._metric.compute()
 
@@ -227,15 +227,15 @@
         >>> aval_metrics = show_avaliable_metrics()
         >>> 'TMMetrics' in aval_metrics
         True
     """
     global _metrics_meta
     return _metrics_meta
 
-def get_metric_by_name(metric_name: str, metric_impl: str = 'TMMetrics') -> Metrics:
+def get_metric_by_name(metric_name: str, metric_impl: str = 'TMMetrics', **kwargs) -> Metrics:
     """
     Get the `Metrics` class by metric names, and metric_impl should be the specific implementation class.
 
     Args:
         metric_name (`str`):
             The metric name used to evaluate. (e.g. Accuracy)
         metric_impl (`str`):
@@ -249,10 +249,10 @@
         >>> from towhee.trainer.metrics import show_avaliable_metrics, get_metric_by_name
         >>> from towhee.trainer.metrics import TMMetrics
         >>> metric = get_metric_by_name('Accuracy', 'TMMetrics')
         >>> isinstance(metric, TMMetrics)
         True
     """
     global _metrics_impls
-    return _metrics_impls[metric_impl](metric_name)
+    return _metrics_impls[metric_impl](metric_name, **kwargs)
 
 _generate_meta_info()
```

## towhee/trainer/trainer.py

```diff
@@ -12,25 +12,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
 import os
 import torch
-import torch.distributed as dist
 
 from typing import Union, Any, Optional
 from pathlib import Path
 from collections.abc import Iterable
 from torch import nn
 from torch import optim
 from torch.optim import Optimizer
 from torch.utils.data.dataloader import DataLoader
 from torch.utils.data.dataset import Dataset
-import torch.multiprocessing as mp
 
 from towhee.data.dataset.dataset import TowheeDataSet, TorchDataSet
 
 from towhee.trainer.callback import TensorBoardCallBack, ProgressBarCallBack, PrintCallBack, ModelCheckpointCallback, \
     EarlyStoppingCallback, TrainerControl, Callback
 from towhee.trainer.metrics import get_metric_by_name
 from towhee.trainer.modelcard import ModelCard, MODEL_CARD_NAME
@@ -212,93 +210,50 @@
     def train(self, resume_checkpoint_path: Optional[str] = None):
         """
         Start to train.
         Args:
             resume_checkpoint_path (`int`):
                 The path to start resume training.
         """
-        if self.configs.device_str == "cuda":
-            self.distributed = True
-            self._spawn_train_process(resume_checkpoint_path)
-        else:
-            self.distributed = False
-            self.run_train(None, None, resume_checkpoint_path)
-
-    def _spawn_train_process(self, resume_checkpoint_path: Optional[str]):
-        world_size = torch.cuda.device_count()
-        mp.spawn(self.run_train,
-                 args=(world_size, resume_checkpoint_path),
-                 nprocs=world_size,  # opt.world_size,
-                 join=True)
-
-    def _init_distributed(self, rank: int, world_size: int):
-        if self.distributed:
-            if torch.cuda.is_available() is False:
-                raise EnvironmentError("not find GPU device for training.")
-            os.environ["MASTER_ADDR"] = "localhost"
-            os.environ["MASTER_PORT"] = "12355"
-            trainer_log.warning("_init_distributed(), rank=%s", rank)
-            torch.cuda.set_device(rank)
-            dist_backend = "nccl"
-            dist_url = "env://"
-            trainer_log.warning("| distributed init (rank %s): %s", rank, dist_url)
-            dist.init_process_group(backend=dist_backend, init_method=dist_url,
-                                    world_size=world_size, rank=rank)
-            dist.barrier()
+        self._run_train(resume_checkpoint_path)
 
-    def _load_before_train(self, resume_checkpoint_path: Optional[str], rank: Optional[int]):
-        sync_bn = self.configs.sync_bn
+    def _load_before_train(self, resume_checkpoint_path: Optional[str]):
         if resume_checkpoint_path is not None:
-            # weights_dict = torch.load(weights_path, map_location=device)
-            # load_weights_dict = {k: v for k, v in weights_dict.items()
-            #                      if model.state_dict()[k].numel() == v.numel()}
-            # model.load_state_dict(load_weights_dict, strict=False)
             self.load(resume_checkpoint_path)
-        else:  # if using multi gpu and not resume, must keep model replicas in all processes are the same
-            if self.distributed:
-                # checkpoint_path = os.path.join(tempfile.gettempdir(), TEMP_INIT_WEIGHTS)
-                checkpoint_path = TEMP_INIT_WEIGHTS
-                if rank == 0:
-                    torch.save(self.model.state_dict(), checkpoint_path)
-                dist.barrier()
-                self.model.load_state_dict(torch.load(checkpoint_path, map_location=self.configs.device))
-        if self.distributed:
-            self.model = torch.nn.parallel.DistributedDataParallel(self.model, device_ids=[rank])
-            if sync_bn:
-                self.model = torch.nn.SyncBatchNorm.convert_sync_batchnorm(self.model).to(self.configs.device)
 
     def _create_logs(self):
         logs = {"global_step": 0, "epoch": self.epoch}
         if self.configs.eval_strategy not in no_option_list:
             logs["eval_global_step"] = 0
         return logs
 
     def prepare_inputs(self, inputs: Any):
         return send_to_device(inputs, self.configs.device)
 
-    def run_train(self, rank: int = None, world_size: int = None, resume_checkpoint_path: str = None):
+    def _run_train(self, resume_checkpoint_path: str = None):
         """
         Main training entry point.
         It is not recommended for users to use it unless over rewriting Trainer.
         Instead, it is recommended to use `trainer.train()` to start training.
 
         Args:
-            rank (`int`):
-                Process rank when using multi gpus.
-            world_size (`int`):
-                Total processes count.
             resume_checkpoint_path (`str`):
                 Last checkpoint path.
         """
         set_seed(self.configs.seed)
-        self._init_distributed(rank, world_size)
-        self.model = self.model.to(self.configs.device)
-        model = self.model
+
         self.trainercontrol = TrainerControl()
-        self._load_before_train(resume_checkpoint_path, rank)
+        self._load_before_train(resume_checkpoint_path)
+
+        if self.configs.device_str == "cuda":
+            self.model = nn.DataParallel(self.model)
+        else:
+            self.model = self.model.to(self.configs.device)
+        model = self.model
+
         # Keeping track whether we can can len() on the dataset or not
         # train_dataset_is_sized = isinstance(self.train_dataset, collections.abc.Sized)
 
         train_dataloader = self.get_train_dataloader()
 
         total_train_batch_size = self.configs.train_batch_size
         # if train_dataset_is_sized:
@@ -321,17 +276,14 @@
         logs = self._create_logs()
         self.callbacks.on_train_begin(logs)
         for epoch in range(train_last_epoch + 1, self.configs.epoch_num + 1):
             self.epoch = logs["epoch"] = epoch
             self.set_train_mode(model)
             self._reset_controller()
             self.optimizer.zero_grad()
-            # if self.distributed: # todo
-                # self.train_sampler.set_epoch(self.epoch)
-            # batch_loss_sum = 0.0
             self.callbacks.on_epoch_begin(self.epoch, logs)
             self.loss_metric.reset()
             self.metric.reset()
             for step, inputs in enumerate(train_dataloader):
                 self.callbacks.on_train_batch_begin(inputs, logs)
                 inputs = self.prepare_inputs(inputs)
                 step_logs = self.train_step(model, inputs)  # , train_dataloader)
@@ -358,15 +310,14 @@
                 break
             if self.trainercontrol.should_save:
                 self.save(
                     path=Path(self.configs.output_dir).joinpath("epoch_" + str(self.epoch)),
                     overwrite=self.configs.overwrite_output_dir
                 )
         trainer_log.info("\nTraining completed.\n")
-        self._cleanup_distributed(rank)
         self.callbacks.on_train_end(logs)
         self.save(
             path=Path(self.configs.output_dir).joinpath("final_epoch"),
             overwrite=self.configs.overwrite_output_dir
         )
 
     def set_train_mode(self, model: nn.Module):
@@ -537,35 +488,25 @@
                 Pytorch tensor or tensor collection.
 
         Returns:
             (`dict`)
                 Step logs which contains the step loss and metric infos.
         """
         step_loss = self.compute_loss(model, inputs)
-        step_loss = reduce_value(step_loss, average=True)
         step_loss.backward()
         step_loss = step_loss.detach()
 
         loss_metric, epoch_metric = self.update_metrics(model, inputs, step_loss, training=True)
 
         self.optimizer.step()
         self.lr_scheduler.step()
         self.optimizer.zero_grad()
         step_logs = {"step_loss": step_loss.item(), "epoch_loss": loss_metric, "epoch_metric": epoch_metric}
         return step_logs
 
-    def _cleanup_distributed(self, rank: int):
-        if self.distributed:
-            if rank == 0:
-                if Path(TEMP_INIT_WEIGHTS).exists() is True:
-                    os.remove(TEMP_INIT_WEIGHTS)
-            # if is_main_process():
-            # self.model = unwrap_model(self.model)
-            dist.destroy_process_group()
-
     def compute_loss(self, model: nn.Module, inputs: Any):
         """
         Compute the step loss.
         It is recommended to subclass `Trainer` and override this method when deal with custom loss in custom task.
         When it is overridden, another method `compute_metric()` often needs to be overridden.
 
         Args:
@@ -683,38 +624,22 @@
         if self.train_dataloader is not None:
             return self.train_dataloader
         if self.train_dataset is None:
             raise ValueError("Trainer: training requires a train_dataset.")
         if isinstance(self.train_dataset, TorchDataSet):
             self.train_dataset = self.train_dataset.dataset
         num_workers = self._get_num_workers()
-        # if isinstance(self.train_dataset, IterableDataset):
-        #     return DataLoader(
-        #         self.train_dataset,
-        #         batch_size=self.configs.train_batch_size,
-        #     )
-        if not self.distributed:
-            return DataLoader(
-                self.train_dataset,
-                batch_size=self.configs.train_batch_size,
-                shuffle=True,
-                num_workers=num_workers,  # self.configs.dataloader_num_workers,
-                pin_memory=self.configs.dataloader_pin_memory,
-                drop_last=self.configs.dataloader_drop_last
-            )
-        else:
-            # self.train_sampler = torch.utils.data.distributed.DistributedSampler(self.train_dataset)
-            train_sampler = torch.utils.data.distributed.DistributedSampler(self.train_dataset)
-            train_batch_sampler = torch.utils.data.BatchSampler(
-                train_sampler, self.configs.batch_size, drop_last=True)
-            return torch.utils.data.DataLoader(self.train_dataset,
-                                               batch_sampler=train_batch_sampler,
-                                               num_workers=num_workers,  # self.configs.dataloader_num_workers,
-                                               pin_memory=self.configs.dataloader_pin_memory,
-                                               )
+        return DataLoader(
+            self.train_dataset,
+            batch_size=self.configs.train_batch_size,
+            shuffle=True,
+            num_workers=num_workers,  # self.configs.dataloader_num_workers,
+            pin_memory=self.configs.dataloader_pin_memory,
+            drop_last=self.configs.dataloader_drop_last
+        )
 
     def get_eval_dataloader(self) -> Optional[DataLoader]:
         """
         Get the eval dataloader.
 
         Returns:
             (`Optional[DataLoader]`)
@@ -723,37 +648,22 @@
         if self.eval_dataloader is not None:
             return self.eval_dataloader
         if self.eval_dataset is None:
             trainer_log.warning("Trainer: eval requires a train_dataset.")
             return None
         if isinstance(self.eval_dataset, TorchDataSet):
             self.eval_dataset = self.eval_dataset.dataset
-        # if isinstance(self.eval_dataset, IterableDataset):
-        #     return DataLoader(
-        #         self.eval_dataset,
-        #         batch_size=self.configs.eval_batch_size,
-        #     )
         num_workers = self._get_num_workers()
-        if not self.distributed:
-            return DataLoader(
-                self.eval_dataset,
-                batch_size=self.configs.eval_batch_size,
-                num_workers=num_workers,  # self.configs.dataloader_num_workers,
-                pin_memory=self.configs.dataloader_pin_memory,
-                drop_last=self.configs.dataloader_drop_last
-            )
-        else:
-            eval_sampler = torch.utils.data.distributed.DistributedSampler(self.eval_dataset)
-            eval_batch_sampler = torch.utils.data.BatchSampler(
-                eval_sampler, self.configs.batch_size, drop_last=True)
-            return torch.utils.data.DataLoader(self.eval_dataset,
-                                               batch_sampler=eval_batch_sampler,
-                                               num_workers=num_workers,  # self.configs.dataloader_num_workers,
-                                               pin_memory=self.configs.dataloader_pin_memory,
-                                               )
+        return DataLoader(
+            self.eval_dataset,
+            batch_size=self.configs.eval_batch_size,
+            num_workers=num_workers,  # self.configs.dataloader_num_workers,
+            pin_memory=self.configs.dataloader_pin_memory,
+            drop_last=self.configs.dataloader_drop_last
+        )
 
     def setup_before_train(self, num_training_steps: int, init_lr: float):
         """
         Setup some configs before training.
 
         Args:
             num_training_steps (`int`):
@@ -786,15 +696,15 @@
             summary_writer_constructor = _get_summary_writer_constructor()
             if summary_writer_constructor is not None:
                 self.callbacks.add_callback(
                     TensorBoardCallBack(summary_writer_constructor,
                                         **self.configs.tensorboard))
 
     def _create_metric(self):
-        self.metric = get_metric_by_name(self.configs.metric)
+        self.metric = get_metric_by_name(self.configs.metric)  # , dist_sync_on_step=True)
         self.metric.to(self.configs.device)
         self.loss_metric = get_metric_by_name("MeanMetric")
         self.loss_metric.to(self.configs.device)
 
     def _create_loss(self):
         if self.override_loss is True:
             return
@@ -804,14 +714,18 @@
         if self.override_optimizer is True:
             return
         self.optimizer = _construct_optimizer_from_config(
             optim,
             self.configs.optimizer,
             model=self.model,
         )
+        if isinstance(self.configs.optimizer, dict) and "lr" in self.configs.optimizer:
+            trainer_log.warning(
+                "`lr=%s` in TrainingConfig directly will override `lr=%s` in optimizer construction of TrainingConfig.",
+                init_lr, self.configs.optimizer["lr"])
         for param in self.optimizer.param_groups:
             param.setdefault("initial_lr", init_lr)
         self.optimizer.lr = init_lr
 
     def _create_scheduler(self, num_training_steps: int, optimizer: torch.optim.Optimizer = None):
         if isinstance(self.configs.lr_scheduler_type, str):
             self.lr_scheduler = get_scheduler(
```

## towhee/trainer/training_config.py

```diff
@@ -41,30 +41,39 @@
     Dump a default yaml, which can be overridden by the custom operator.
     """
     training_config = TrainingConfig()
     training_config.save_to_yaml(path2yaml=yaml_path)
     trainer_log.info("dump default yaml to %s", yaml_path)
 
 
-def get_config_help():
+def get_config_help() -> Dict:
     """
     Get config setting infos.
     Returns:
         (`dict`)
             The help dict.
     """
-    config_fields = fields(TrainingConfig)
+    return get_dataclasses_help(TrainingConfig)
+
+
+def get_dataclasses_help(cls) -> Dict:
+    """
+    Get dataclasses infos.
+    Returns:
+        (`dict`)
+            The help dict.
+    """
+    config_fields = fields(cls)
     help_dict = {}
+    default_dict = {}
     for config_field in config_fields:
-        metadata_dict = config_field.metadata
-        help_dict[config_field.name] = metadata_dict
+        default_dict[config_field.name] = config_field.default
+        help_dict[config_field.name] = config_field.metadata
     for field_name, metadata_dict in help_dict.items():
-        print("- " + field_name)
-        print(metadata_dict)
-        print("")
+        print(f"- {field_name} \n  default: {default_dict[field_name]} \n  metadata_dict: {metadata_dict} \n")
     return help_dict
 
 
 def _early_stopping_factory():
     return {"monitor": "eval_epoch_metric", "patience": 4, "mode": "max"}
 
 
@@ -104,15 +113,15 @@
         dataloader_pin_memory (`bool`):
             Drop the last incomplete batch if it is not divisible by the batch size.
         dataloader_drop_last (`bool`):
             Drop the last incomplete batch if it is not divisible by the batch size.
         dataloader_num_workers (`int`):
             Number of subprocesses to use for data loading.
         lr (`float`):
-            The initial learning rate for AdamW.
+            The initial learning rate.
         metric (`str`):
             The metric to use to compare two different models.
         print_steps (`int`):
             If None, use the tqdm progress bar, otherwise it will print the logs on the screen every `print_steps`.
         load_best_model_at_end (`bool`):
             Whether or not to load the best model found during training at the end of training.
         early_stopping (`Union[dict, str]`):
@@ -127,16 +136,14 @@
             Pytorch optimizer Class name in torch.optim package.
         lr_scheduler_type (`str`):
             The scheduler type to use.
         warmup_ratio (`float`):
             Linear warmup over warmup_ratio fraction of total steps.
         device_str (`str`):
             Device string.
-        sync_bn (`bool`):
-            It will be work if device_str is `cuda`, the True sync_bn would make training slower but acc better.
         freeze_bn (`bool`):
             It will completely freeze all BatchNorm layers during training.
     """
     output_dir: str = field(
         default="./output_dir",
         metadata={
             HELP: "The output directory where the model predictions and checkpoints will be written.", CATEGORY: "train"
@@ -170,31 +177,31 @@
             HELP: "Drop the last incomplete batch if it is not divisible by the batch size.", CATEGORY: "train"
         }
     )
     dataloader_num_workers: int = field(
         default=0,
         metadata={
             HELP:
-                "Number of subprocesses to use for data loading."
-                "default 0 means that the data will be loaded in the main process."
-                "-1 means using all the cpu kernels,"
+                "Number of subprocesses to use for data loading. "
+                "Default 0 means that the data will be loaded in the main process. "
+                "-1 means using all the cpu kernels, "
                 "it will greatly improve the speed when distributed training.",
             CATEGORY:
                 "train"
         },
     )
-    lr: float = field(default=5e-5, metadata={HELP: "The initial learning rate for AdamW.", CATEGORY: "learning"})
+    lr: float = field(default=5e-5, metadata={HELP: "The initial learning rate.", CATEGORY: "learning"})
     metric: Optional[str] = field(default="Accuracy",
                                   metadata={HELP: "The metric to use to compare two different models.",
                                             CATEGORY: "metrics"})
 
     print_steps: Optional[int] = field(
         default=None,
         metadata={
-            HELP: "if None, use the tqdm progress bar, otherwise it will print the logs on the screen every `print_steps`",
+            HELP: "If None, use the tqdm progress bar, otherwise it will print the logs on the screen every `print_steps`",
             CATEGORY: "logging"
         }
     )
     load_best_model_at_end: Optional[bool] = field(
         default=False,
         metadata={
             HELP: "Whether or not to load the best model found during training at the end of training.",
@@ -228,25 +235,24 @@
     warmup_ratio: float = field(default=0.0, metadata={HELP: "Linear warmup over warmup_ratio fraction of total steps.",
                                                        CATEGORY: "learning"})
     warmup_steps: int = field(default=0, metadata={HELP: "Linear warmup over warmup_steps.", CATEGORY: "learning"})
     device_str: str = field(
         default=None,
         metadata={
             HELP:
-                ("None -> if there is a cuda env in the machine, it will use cuda:0, else cpu;"
-                 "`cpu` -> use cpu only;"
-                 "`cuda:2` -> use the No.2 gpu."),
+                ("None -> If there is a cuda env in the machine, it will use cuda:0, else cpu.\n"
+                 "`cpu` -> Use cpu only.\n"
+                 "`cuda:2` -> Use the No.2 gpu, the same for other numbers.\n"
+                 "`cuda` -> Use all available gpu, using data parallel. "
+                 "If you want to use several specified gpus to run, you can specify the environment variable "
+                 "`CUDA_VISIBLE_DEVICES` as the number of gpus you need before running your training script."),
             CATEGORY:
                 "device"
         }
     )
-    sync_bn: bool = field(default=False, metadata={
-        HELP: "will be work if device_str is `cuda`, the True sync_bn would make training slower but acc better.",
-        CATEGORY: "device"
-    })
     freeze_bn: bool = field(default=False,
                             metadata={HELP: "will completely freeze all BatchNorm layers during training.",
                                       CATEGORY: "train"})
 
     def __post_init__(self):
         if self.output_dir is not None:
             self.output_dir = os.path.expanduser(self.output_dir)
```

## towhee/types/__init__.py

```diff
@@ -12,26 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from towhee.types.image import Image
 from towhee.types.audio_frame import AudioFrame
 from towhee.types.video_frame import VideoFrame
 from towhee.types.arg import arg, to_image_color
-from towhee.types.tensor_array import TensorArray
+
 
 __all__ = [
     'Image',
     'AudioFrame',
     'arg',
     'to_image_color',
-    'VideoFrame',
-    'TensorArray'
+    'VideoFrame'
 ]
-
-equivalents = {
-    'towhee.types.image.Image': 'towhee.types.Image',
-    'towhee.types.audio_frame.AudioFrame': 'towhee.types.AudioFrame',
-    'towhee.types.video_frame.VideoFrame': 'towhee.types.VideoFrame',
-    'towhee.types.arg.arg': 'towhee.types.arg',
-    'towhee.types.arg.to_image_color': 'towhee.types.to_image_color',
-    'towhee.types.tensor_array.TensorArray': 'towhee.types.TensorArray'
-}
```

## towhee/utils/dependency_control.py

```diff
@@ -9,28 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import subprocess
 import sys
-import os
+# import os
 
 
 def prompt_install(package): # pragma: no cover
     """
     Function used to prompt user to install a package. If TOWHEE_WORKER env variable is set
     to True then the package will be automatically installed.
     """
-    if os.getenv('TOWHEE_WORKER', 'False') == 'True' or get_yes_no(f'Do you want to install {package}?'):
-        try:
-            subprocess.check_call([sys.executable, '-m', 'pip', 'install', package])
-            print(f'{package} installed successfully!')
-        except subprocess.CalledProcessError:
-            print(f'Ran into error installing {package}.')
+    try:
+        subprocess.check_call([sys.executable, '-m', 'pip', 'install', package])
+        print(f'{package} installed successfully!')
+    except subprocess.CalledProcessError:
+        print(f'Ran into error installing {package}.')
 
 def get_yes_no(question): # pragma: no cover
     while True:
         answer = input(question + ' [y/n]: ').lower()
         if 'yes'.startswith(answer.lower()):
             return True
         elif 'no'.startswith(answer.lower()):
```

## towhee/utils/hub_utils.py

```diff
@@ -8,19 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import requests
 import random
+import traceback
+import requests
 from requests.exceptions import HTTPError
 from requests.auth import HTTPBasicAuth
 
+from towhee.utils.log import engine_log
+
 
 class HubUtils:
     """
     The Hub Utils to deal with the http request. And other staticmethod for hub.
 
     Args:
         author (`str`):
@@ -424,7 +427,18 @@
         with open(file, 'r', encoding='utf-8') as f1:
             file_text = f1.read()
         # Replace the target string
         for ori_str, tar_str in zip(ori_str_list, tar_str_list):
             file_text = file_text.replace(ori_str, tar_str)
         with open(new_file, 'w', encoding='utf-8') as f2:
             f2.write(file_text)
+
+    def branch_tree(self, tag):
+        url = f'{self._root}/towhee-api/v1/repos/{self._author}/{self._repo}/tree?recursive=true&ref={tag}'
+        try:
+            r = requests.get(url)
+            r.raise_for_status()
+            return r.json()
+        except Exception as e:  # pylint: disable=broad-except
+            err = '{}, {}'.format(str(e), traceback.format_exc())
+            engine_log.error(err)
+            return None
```

## towhee/utils/np_format.py

```diff
@@ -7,62 +7,35 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-
-import json
 import numpy as np
 
 
-class NumpyArrayEncoder(json.JSONEncoder):
-    """
-    Support numpy to json
-    """
-    def default(self, o):
-        if isinstance(o, np.ndarray):
-            return _NumpyFormat(o).to_dict()
-
-        return json.JSONEncoder.default(self, o)
-
-class NumpyArrayDecoder(json.JSONDecoder):
-    """
-    Load numpy from json
-    """
-    def __init__(self, *args, **kwargs):
-        super().__init__(object_hook=self.object_hook, *args, **kwargs)
-
-    def object_hook(self, dct):  # pylint: disable=method-hidden
-        if '_NP' in dct:
-            return _NumpyFormat.from_dict(dct)
-        return dct
-
-
-
-class _NumpyFormat:
+class NumpyFormat:
     """
-    _NumpyFormat:
+    NumpyFormat:
     """
 
     def __init__(self, data: 'ndarray'):
         self._data = data
 
     def to_dict(self):
         return {
             '_NP': True,
-            'dtype': _NumpyFormat.from_numpyt_type(self._data.dtype),
+            'dtype': NumpyFormat.from_numpyt_type(self._data.dtype),
             'data': self._data.tolist()
         }
 
     @staticmethod
     def from_dict(dct):
-        return np.array(dct['data'], _NumpyFormat.to_numpy_type(dct['dtype']))
+        return np.array(dct['data'], NumpyFormat.to_numpy_type(dct['dtype']))
 
     @staticmethod
     def from_numpyt_type(dtype):
         if dtype == np.uint8:
             return 1
         if dtype == np.uint16:
             return 2
```

## Comparing `towhee/dc2.py` & `towhee/utils/empty_format.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from towhee.runtime.data_queue import Empty
 
 
-from towhee.runtime import register, pipe, ops
-from towhee.datacollection import DataCollection
+class EmptyFormat:
+    """
+    EmptyFormat:
+    """
+    def to_dict(self):
+        return {
+            '_EMP': True,
+        }
 
-
-__all__ = [
-    'register',
-    'pipe',
-    'ops',
-    'DataCollection'
-]
+    @staticmethod
+    def from_dict():
+        return Empty()
```

## Comparing `towhee/pipeline_format.py` & `towhee/serve/triton/serializer.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,57 +7,49 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import json
 
-from abc import ABC, abstractmethod
+import numpy as np
+from towhee.runtime.data_queue import Empty
+from towhee.utils.np_format import NumpyFormat
+from towhee.utils.empty_format import EmptyFormat
 
-from towhee.dataframe.iterators import MapIterator
-from towhee.types._frame import _Frame
 
-
-class OutputFormat(ABC):
+class TritonSerializer(json.JSONEncoder):
     """
-    Format pipeline's output.
+    Support data that might occur in a towhee pipeline to json.
     """
+    def default(self, o):
+        if isinstance(o, np.ndarray):
+            return NumpyFormat(o).to_dict()
+        if o is Empty():
+            return EmptyFormat().to_dict()
 
-    @abstractmethod
-    def __call__(self, itr: MapIterator):
-        pass
-
-    @staticmethod
-    def get_format_handler(pipeline_type: str):
-        if pipeline_type == 'image-embedding':
-            return ImageEmbeddingFormat()
-        else:
-            return NormalFormat()
-
+        return json.JSONEncoder.default(self, o)
 
-class ImageEmbeddingFormat(OutputFormat):
-    """Image embedding pipeline format.
 
-    If pipeline's type is image-embedding, use the pipeline.
+class TritonParser(json.JSONDecoder):
+    """
+    Support data that might occur in a towhee pipeline from json.
     """
+    def __init__(self, *args, **kwargs):
+        super().__init__(object_hook=self.object_hook, *args, **kwargs)
 
-    def __call__(self, itr: MapIterator):
-        data = next(itr)
-        return data[0][0]
+    def object_hook(self, dct):  # pylint: disable=method-hidden
+        if '_NP' in dct:
+            return NumpyFormat.from_dict(dct)
+        if '_EMP' in dct:
+            return EmptyFormat.from_dict()
+        return dct
 
 
-class NormalFormat(OutputFormat):
-    """
-    Normal format.
-    """
+def to_triton_data(data):
+    return json.dumps(data, cls=TritonSerializer)
+
 
-    def __call__(self, itr: MapIterator):
-        res = []
-        for data in itr:
-            # data is Tuple
-            data_value = []
-            for item in data[0]:
-                if item is not None and not isinstance(item, _Frame):
-                    data_value.append(item)
-            res.append(tuple(data_value))
-        return res
+def from_triton_data(data):
+    return json.loads(data, cls=TritonParser)
```

## Comparing `towhee/dataframe/__init__.py` & `towhee/pipelines/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from towhee.dataframe.dataframe import DataFrame
-from towhee.dataframe.iterators import DataFrameIterator
 
+from pathlib import Path
 
-__all__ = [
-    'DataFrame',
-    'DataFrameIterator'
-]
+from towhee.utils.log import engine_log
+
+
+BUILT_IN_PIPES_ROOT = Path(__file__).absolute().parent
+
+
+def get_builtin_pipe_file(name: str) -> Path:
+    file_name = name + '.py'
+    file_path = BUILT_IN_PIPES_ROOT / file_name
+    if not file_path.is_file():
+        engine_log.info('%s not a built-in pipeline', name)
+        return None
+    return file_path
```

## Comparing `towhee/dataframe/_schema.py` & `towhee/serve/triton/triton_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,55 +8,55 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import torch
+from typing import List
 
-from towhee.utils.log import engine_log
+from towhee.serve.triton.bls.python_backend_wrapper import pb_utils
 
 
-class _Schema:
-    """
-    Schema of dataframe.
-    Every dataframe has _Frame cols.
+class TritonClient:
     """
+    The TritonClient to access model on Triton server.
 
-    def __init__(self):
-        self._cols = []
-        self._key_index = {}
-        self._sealed = False
-
-    def add_col(self, name: str, col_type: str) -> bool:
-        if self._sealed:
-            engine_log.error('Schema already sealed, can not change cols')
-            return False
-
-        if name in self._key_index:
-            engine_log.error('Col name {%s} already exist', name)
-            return False
-
-        self._cols.append((name, col_type))
-        self._key_index[name] = len(self._cols) - 1
-        return True
-
-    def col_index(self, col_name: str) -> int:
-        return self._key_index[col_name]
-
-    def col_key(self, index: int) -> str:
-        return self._cols[index][0]
-
-    def col_type(self, index: int):
-        return self._cols[index][1]
-
-    def seal(self):
-        self._sealed = True
-
-    @property
-    def col_count(self):
-        return len(self._cols)
-
-    @property
-    def cols(self):
-        return self._cols
+    Args:
+        model_name (`str`):
+            The name of the model.
+        input_names (`List[str]`):
+            The list of the input names.
+        output_names (`List[str]`):
+            The list of the output names.
+    """
+    def __init__(self, model_name: str, input_names: List[str], output_names: List[str]):
+        self._model_name = model_name
+        self._input_names = input_names
+        self._output_names = output_names
+
+    def _torch_tensor_to_pbtenor(self, name: str, array: 'Tensor'):
+        return pb_utils.Tensor(name, array.numpy() if array.device.type == 'cpu' else array.cpu().numpy())
+
+    def __call__(self, *args, **kwargs):
+        inputs = [
+            self._torch_tensor_to_pbtenor(name, array)
+            for array, name in zip(args, self._input_names)
+        ]
+
+        for name, array in kwargs.items():
+            inputs.append(self._torch_tensor_to_pbtenor(name, array))
+
+        inference_request = pb_utils.InferenceRequest(model_name=self._model_name, requested_output_names=self._output_names, inputs=inputs)
+
+        inference_response = inference_request.exec()
+
+        if inference_response.has_error():
+            raise pb_utils.TritonModelException(inference_response.error().message())
+        else:
+            if len(self._output_names) == 1:
+                outputs = torch.tensor(pb_utils.get_output_tensor_by_name(inference_response, self._output_names[0]).as_numpy())
+            else:
+                outputs = [torch.tensor(pb_utils.get_output_tensor_by_name(inference_response, name).as_numpy()) for name in self._output_names]
 
+        return outputs
```

## Comparing `towhee/dataframe/array/utils.py` & `towhee/pipelines/_builtin_pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,23 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from towhee import pipe, AutoPipes, AutoConfig
 
-from itertools import repeat
-from towhee.dataframe.array.array import Array
 
-
-def full(size: int, fill_value):
+@AutoConfig.register
+class MyConfig:
+    """
+    For UT
     """
-    Return a new `Array` of given shape filled with `fill_value`
+    def __init__(self):
+        self.param = 1
 
-    Args:
-        size (`int`):
-            Size of the new `Array`
-        fill_value (`numpy.dtype` or `str`):
-            Fill value
+
+@AutoPipes.register
+def pipeline(config):
+    """
+    For UT
     """
-    return Array(list(repeat(fill_value, size)))
+    return (
+        pipe.input('num')
+        .map('num', 'ret', lambda x: x + config.param)
+        .output('ret')
+    )
```

## Comparing `towhee/engine/operator_io/_mock_reader.py` & `towhee/utils/lazy_import.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from queue import Queue
+import importlib
+from types import ModuleType
 
-from towhee.engine.operator_io.reader import ReaderBase
 
-class StopFrame:
-    pass
-
-
-class MockReader(ReaderBase):
+class LazyImport(ModuleType):
     """
-    MockReader for engine test
+    Lazily import a module.
     """
-    def __init__(self, queue: Queue):
-        self._queue = queue
-
-    def read(self):
-        # Blocking if queue is empty
-        data = self._queue.get()
-
-        if not isinstance(data, StopFrame):
-            return data
-        else:
-            raise StopIteration()
-
-    def close(self):
-        self._queue.put(StopFrame())
+    def __init__(self, local_name, parent_module_globals, name):
+        self._local_name = local_name
+        self._parent_module_globals = parent_module_globals
+        super().__init__(name)
+
+    def _load(self):
+        module = importlib.import_module(self.__name__)
+        self._parent_module_globals[self._local_name] = module
+        self.__dict__.update(module.__dict__)
+        return module
+
+    def __getattr__(self, item):
+        module = self._load()
+        return getattr(module, item)
+
+    def __dir__(self):
+        module = self._load()
+        return dir(module)
```

## Comparing `towhee/serve/triton/dockerfiles/DockerfileCuda114dev` & `towhee/serve/triton/dockerfiles/DockerfileCuda117dev`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,30 @@
-FROM nvcr.io/nvidia/tritonserver:21.10-py3
+FROM nvcr.io/nvidia/tritonserver:22.07-py3
 
-RUN apt-key adv --fetch-keys \
-    https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2004/x86_64/3bf863cc.pub && \
-    apt-get update                                && \
-    apt-get install -y software-properties-common && \
-    add-apt-repository ppa:deadsnakes/ppa         && \
-    apt-get update                                && \
+
+RUN apt-get update          && \
     apt-get install -y         \
               zip              \
               wget             \
               unzip            \
               python3.8        \
               python3-pip      \
               libgl1-mesa-glx
 
 RUN pip3 install -U pip
 
-RUN pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu113
-
-RUN pip3 install pyarrow onnxruntime
-
-RUN pip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple towhee --pre
-RUN pip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple towhee.models --pre
+RUN pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu117
 
-RUN apt-get install git-lfs && \
-    git lfs install
+RUN pip3 install onnxruntime onnx
 
 WORKDIR /workspace
 
-RUN git clone -b nebullvm https://github.com/towhee-io/towhee-compiler.git
-RUN cd towhee-compiler && pip install -r requirements.txt &&  python3 setup.py develop
-RUN python3 -c "import nebullvm"
-
 RUN mkdir -p /workspace/models
 
-COPY ./dag.json /workspace/dag.json
+COPY ./dag.pickle /workspace/dag.pickle
+
+COPY ./server_config.json /workspace/server_config.json
+
+RUN pip install --no-cache-dir -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple towhee --pre
+RUN pip install --no-cache-dir -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple towhee.models --pre
 
-RUN triton_builder /workspace/dag.json /workspace/models
- 
+RUN triton_builder /workspace/dag.pickle /workspace/models /workspace/server_config.json
```

## Comparing `towhee/utils/scipy_utils.py` & `towhee/utils/onnx_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 try:
     # pylint: disable=unused-import,ungrouped-imports
-    from scipy import sparse
+    import onnx
 except ModuleNotFoundError as moduleNotFound:
     try:
         from towhee.utils.dependency_control import prompt_install
-        prompt_install('scipy')
+        prompt_install('onnx')
         # pylint: disable=unused-import,ungrouped-imports
-        from scipy import sparse
+        import onnx
     except:
         from towhee.utils.log import engine_log
-        engine_log.error('scipy not found, you can install via `pip install scipy`.')
-        raise ModuleNotFoundError('scipy not found, you can install via `pip install scipy`.') from moduleNotFound
+        engine_log.error('onnx not found, you can install via `pip install onnx`.')
+        raise ModuleNotFoundError('onnx not found, you can install via `pip install onnx`.') from moduleNotFound
```

## Comparing `towhee/utils/tritonclient_utils.py` & `towhee/utils/triton_httpclient.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 try:
     # pylint: disable=unused-import,ungrouped-imports
-    import tritonclient.grpc as grpcclient
     import tritonclient.http as httpclient
+    import tritonclient.http.aio as aio_httpclient
     from tritonclient.utils import InferenceServerException, np_to_triton_dtype
 except ModuleNotFoundError as moduleNotFound:
     try:
         from towhee.utils.dependency_control import prompt_install
-        prompt_install('tritonclient[all]')
+        prompt_install('tritonclient[http]')
         # pylint: disable=unused-import,ungrouped-imports
-        import tritonclient.grpc as grpcclient
         import tritonclient.http as httpclient
+        import tritonclient.http.aio as aio_httpclient
         from tritonclient.utils import InferenceServerException, np_to_triton_dtype
     except:
         from towhee.utils.log import engine_log
-        engine_log.error('tritonclient not found, you can install via `pip install tritonclient[all]`.')
-        raise ModuleNotFoundError('tritonclient not found, you can install via `pip install tritonclient[all]`.') from moduleNotFound
+        engine_log.error('tritonclient not found, you can install via `pip install tritonclient[http]`.')
+        raise ModuleNotFoundError('tritonclient not found, you can install via `pip install tritonclient[http]`.') from moduleNotFound
```

## Comparing `towhee/utils/thirdparty/av_utils.py` & `towhee/utils/thirdparty/dill_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 try:
     # pylint: disable=unused-import
-    import av
+    import dill
 except ModuleNotFoundError as e: # pragma: no cover
     from towhee.utils.dependency_control import prompt_install
-    prompt_install('av')
-    import av # pylint: disable=ungrouped-imports
+    prompt_install('dill')
+    import dill # pylint: disable=ungrouped-imports
```

## Comparing `towhee-0.9.0.dist-info/LICENSE` & `towhee-1.0.0rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `towhee-0.9.0.dist-info/METADATA` & `towhee-1.0.0rc1.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towhee
-Version: 0.9.0
+Version: 1.0.0rc1
 Summary: Towhee is a framework that helps you encode your unstructured data into embeddings.
 Home-page: https://github.com/towhee-io/towhee
 Author: Towhee Team
 Author-email: towhee-team@zilliz.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Platform: unix
 Platform: linux
@@ -12,18 +12,16 @@
 Platform: win32
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (>=2.12.5)
 Requires-Dist: tqdm (>=4.59.0)
 Requires-Dist: tabulate
 Requires-Dist: numpy
-Requires-Dist: pygit2 (<=1.10.1)
-Requires-Dist: pgzip
-Requires-Dist: pyarrow
 Requires-Dist: twine
+Requires-Dist: contextvars ; python_version <= "3.6"
 Requires-Dist: importlib-resources ; python_version<'3.7'
 
 &nbsp;
 
 <p align="center">
     <img src="towhee_logo.png#gh-light-mode-only" width="60%"/>
     <img src="assets/towhee_logo_dark.png#gh-dark-mode-only" width="60%"/>
@@ -71,19 +69,70 @@
 
 :package:&emsp;**Data Processing:** Towhee also provides traditional methods alongside neural network models to help you build practical data processing pipelines. We have a rich pool of operators available, such as video decoding, audio slicing, frame sampling, feature vector dimension reduction, ensembling, and database operations.
 
 :snake:&emsp;**Pythonic API:** Towhee includes a Pythonic method-chaining API for describing custom data processing pipelines. We also support schemas, which makes processing unstructured data as easy as handling tabular data.
 
 ## What's New
 
+**v0.9.0 Dec. 2, 2022**
+* Added one video classification model:
+[*Vis4mer*](https://github.com/towhee-io/towhee/tree/branch0.9.0/towhee/models/vis4mer)
+* Added three visual backbones:
+[*MCProp*](https://github.com/towhee-io/towhee/tree/branch0.9.0/towhee/models/mcprop), 
+[*RepLKNet*](https://github.com/towhee-io/towhee/tree/branch0.9.0/towhee/models/replknet), 
+[*Shunted Transformer*](https://github.com/towhee-io/towhee/tree/branch0.9.0/towhee/models/shunted_transformer)
+* Add two code search operators:
+[*code_search.codebert*](https://towhee.io/code-search/codebert), 
+[*code_search.unixcoder*](https://towhee.io/code-search/unixcoder)
+* Add five image captioning operators: 
+[*image_captioning.expansionnet-v2*](https://towhee.io/image-captioning/expansionnet-v2), 
+[*image_captioning.magic*](https://towhee.io/image-captioning/magic),
+[*image_captioning.clip_caption_reward*](https://towhee.io/image-captioning/clip-caption-reward), 
+[*image_captioning.blip*](https://towhee.io/image-captioning/blip), 
+[*image_captioning.clipcap*](https://towhee.io/image-captioning/clipcap)
+* Add five image-text embedding operators: 
+[*image_text_embedding.albef*](https://towhee.io/image-text-embedding/albef), 
+[*image_text_embedding.ru_clip*](https://towhee.io/image-text-embedding/ru-clip), 
+[*image_text_embedding.japanese_clip*](https://towhee.io/image-text-embedding/japanese-clip),
+[*image_text_embedding.taiyi*](https://towhee.io/image-text-embedding/taiyi),
+[*image_text_embedding.slip*](https://towhee.io/image-text-embedding/slip)
+* Add one machine-translation operator: 
+[*machine_translation.opus_mt*](https://towhee.io/machine-translation/opus-mt)
+* Add one filter-tiny-segments operator:
+[*video-copy-detection.filter-tiny-segments*](https://towhee.io/video-copy-detection/filter-tiny-segments)
+* Add an advanced tutorial for audio fingerprinting: 
+[*Audio Fingerprint II: Music Detection with Temporal Localization*](https://github.com/towhee-io/examples/blob/main/audio/audio_fingerprint/audio_fingerprint_advanced.ipynb) (increased accuracy from 84% to 90%)
+
+**v0.8.1 Sep. 30, 2022**
+
+* Added four visual backbones:
+[*ISC*](https://github.com/towhee-io/towhee/tree/branch0.8.1/towhee/models/isc),
+[*MetaFormer*](https://github.com/towhee-io/towhee/tree/branch0.8.1/towhee/models/metaformer),
+[*ConvNext*](https://github.com/towhee-io/towhee/tree/branch0.8.1/towhee/models/convnext),
+[*HorNet*](https://github.com/towhee-io/towhee/tree/branch0.8.1/towhee/models/hornet)
+* Add two video de-copy operators:
+[*select-video*](https://towhee.io/video-copy-detection/select-video), 
+[*temporal-network*](https://towhee.io/video-copy-detection/temporal-network)
+* Add one image embedding operator specifically designed for image retrieval and video de-copy with SOTA performance on VCSL dataset:
+[*isc*](https://towhee.io/image-embedding/isc)
+* Add one audio embedding operator specified for audio fingerprint:
+[*audio_embedding.nnfp*](https://towhee.io/audio-embedding/nnfp) (with pretrained weights)
+* Add one tutorial for video de-copy: 
+[*How to Build a Video Segment Copy Detection System*](https://github.com/towhee-io/examples/blob/main/video/video_deduplication/segment_level/video_deduplication_at_segment_level.ipynb)
+* Add one beginner tutorial for audio fingerprint:
+[*Audio Fingerprint I: Build a Demo with Towhee & Milvus*](https://github.com/towhee-io/examples/blob/main/audio/audio_fingerprint/audio_fingerprint_beginner.ipynb)
+
+
 **v0.8.0 Aug. 16, 2022**
 
 * Towhee now supports generating an Nvidia Triton Server from a Towhee pipeline, with aditional support for GPU image decoding.
-* Added one audio fingerprinting model: [**nnfp**](https://github.com/towhee-io/towhee/tree/branch0.8.0/towhee/models/nnfp)
-* Added two image embedding models: [**RepMLP**](https://github.com/towhee-io/towhee/tree/branch0.8.0/towhee/models/repmlp), [**WaveViT**](https://github.com/towhee-io/towhee/tree/branch0.8.0/towhee/models/wave_vit)
+* Added one audio fingerprinting model: 
+[*nnfp*](https://github.com/towhee-io/towhee/tree/branch0.8.0/towhee/models/nnfp)
+* Added two image embedding models: 
+[*RepMLP*](https://github.com/towhee-io/towhee/tree/branch0.8.0/towhee/models/repmlp), [**WaveViT**](https://github.com/towhee-io/towhee/tree/branch0.8.0/towhee/models/wave_vit)
 
 **v0.7.3 Jul. 27, 2022**
 * Added one multimodal (text/image) model:
 [*CoCa*](https://github.com/towhee-io/towhee/tree/branch0.7.3/towhee/models/coca).
 * Added two video models for grounded situation recognition & repetitive action counting:
 [*CoFormer*](https://github.com/towhee-io/towhee/tree/branch0.7.3/towhee/models/coformer),
 [*TransRAC*](https://github.com/towhee-io/towhee/tree/branch0.7.3/towhee/models/transrac).
@@ -143,23 +192,23 @@
 ```python
 import towhee
 
 # create image embeddings and build index
 (
     towhee.glob['file_name']('./*.png')
           .image_decode['file_name', 'img']()
-          .image_text_embedding.clip['img', 'vec'](model_name='clip_vit_b32', modality='image')
+          .image_text_embedding.clip['img', 'vec'](model_name='clip_vit_base_patch32', modality='image')
           .tensor_normalize['vec','vec']()
           .to_faiss[('file_name', 'vec')](findex='./index.bin')
 )
 
 # search image by text
 results = (
     towhee.dc['text'](['puppy Corgi'])
-          .image_text_embedding.clip['text', 'vec'](model_name='clip_vit_b32', modality='text')
+          .image_text_embedding.clip['text', 'vec'](model_name='clip_vit_base_patch32', modality='text')
           .tensor_normalize['vec', 'vec']()
           .faiss_search['vec', 'results'](findex='./index.bin', k=3)
           .select['text', 'results']()
 )
 ```
 <img src="assets/towhee_example.png" style="width: 60%; height: 60%">
 
@@ -179,15 +228,15 @@
 
 ## Contributing
 
 Writing code is not the only way to contribute! Submitting issues, answering questions, and improving documentation are just some of the many ways you can help our growing community. Check out our [contributing page](https://github.com/towhee-io/towhee/blob/main/CONTRIBUTING.md) for more information.
 
 Special thanks goes to these folks for contributing to Towhee, either on Github, our Towhee Hub, or elsewhere:
 <br><!-- Do not remove start of hero-bot --><br>
-<img src="https://img.shields.io/badge/all--contributors-34-orange"><br>
+<img src="https://img.shields.io/badge/all--contributors-33-orange"><br>
 <a href="https://github.com/AniTho"><img src="https://avatars.githubusercontent.com/u/34787227?v=4" width="30px" /></a>
 <a href="https://github.com/Chiiizzzy"><img src="https://avatars.githubusercontent.com/u/72550076?v=4" width="30px" /></a>
 <a href="https://github.com/GuoRentong"><img src="https://avatars.githubusercontent.com/u/57477222?v=4" width="30px" /></a>
 <a href="https://github.com/NicoYuan1986"><img src="https://avatars.githubusercontent.com/u/109071306?v=4" width="30px" /></a>
 <a href="https://github.com/Tumao727"><img src="https://avatars.githubusercontent.com/u/20420181?v=4" width="30px" /></a>
 <a href="https://github.com/YuDongPan"><img src="https://avatars.githubusercontent.com/u/88148730?v=4" width="30px" /></a>
 <a href="https://github.com/binbinlv"><img src="https://avatars.githubusercontent.com/u/83755740?v=4" width="30px" /></a>
@@ -195,15 +244,14 @@
 <a href="https://github.com/dreamfireyu"><img src="https://avatars.githubusercontent.com/u/47691077?v=4" width="30px" /></a>
 <a href="https://github.com/filip-halt"><img src="https://avatars.githubusercontent.com/u/81822489?v=4" width="30px" /></a>
 <a href="https://github.com/fzliu"><img src="https://avatars.githubusercontent.com/u/6334158?v=4" width="30px" /></a>
 <a href="https://github.com/gexy185"><img src="https://avatars.githubusercontent.com/u/103474331?v=4" width="30px" /></a>
 <a href="https://github.com/hyf3513OneGO"><img src="https://avatars.githubusercontent.com/u/67197231?v=4" width="30px" /></a>
 <a href="https://github.com/jaelgu"><img src="https://avatars.githubusercontent.com/u/86251631?v=4" width="30px" /></a>
 <a href="https://github.com/jeffoverflow"><img src="https://avatars.githubusercontent.com/u/24581746?v=4" width="30px" /></a>
-<a href="https://github.com/jennyli-z"><img src="https://avatars.githubusercontent.com/u/93511422?v=4" width="30px" /></a>
 <a href="https://github.com/jingkl"><img src="https://avatars.githubusercontent.com/u/34296482?v=4" width="30px" /></a>
 <a href="https://github.com/jinlingxu06"><img src="https://avatars.githubusercontent.com/u/106302799?v=4" width="30px" /></a>
 <a href="https://github.com/junjiejiangjjj"><img src="https://avatars.githubusercontent.com/u/14136703?v=4" width="30px" /></a>
 <a href="https://github.com/krishnakatyal"><img src="https://avatars.githubusercontent.com/u/37455387?v=4" width="30px" /></a>
 <a href="https://github.com/omartarek206"><img src="https://avatars.githubusercontent.com/u/40853054?v=4" width="30px" /></a>
 <a href="https://github.com/oneseer"><img src="https://avatars.githubusercontent.com/u/28955741?v=4" width="30px" /></a>
 <a href="https://github.com/pravee42"><img src="https://avatars.githubusercontent.com/u/65100038?v=4" width="30px" /></a>
```

### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: towhee Version: 0.9.0 Summary: Towhee is a
+Metadata-Version: 2.1 Name: towhee Version: 1.0.0rc1 Summary: Towhee is a
 framework that helps you encode your unstructured data into embeddings. Home-
 page: https://github.com/towhee-io/towhee Author: Towhee Team Author-email:
 towhee-team@zilliz.com License: http://www.apache.org/licenses/LICENSE-2.0
 Platform: unix Platform: linux Platform: osx Platform: win32 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: requests
 (>=2.12.5) Requires-Dist: tqdm (>=4.59.0) Requires-Dist: tabulate Requires-
-Dist: numpy Requires-Dist: pygit2 (<=1.10.1) Requires-Dist: pgzip Requires-
-Dist: pyarrow Requires-Dist: twine Requires-Dist: importlib-resources ;
-python_version<'3.7'  
+Dist: numpy Requires-Dist: twine Requires-Dist: contextvars ; python_version <=
+"3.6" Requires-Dist: importlib-resources ; python_version<'3.7'  
 [towhee_logo.png#gh-light-mode-only] [assets/towhee_logo_dark.png#gh-dark-mode-
                                      only]
                    **** x2vec, Towhee is all you need! ****
                        **** ENGLISH | ä¸­æææ¡£ ****
 [join-slack] [twitter] [license] [github_actions] [coverage]
   [Towhee](https://towhee.io) makes it easy to build neural data processing
 pipelines for AI applications. We provide hundreds of models, algorithms, and
@@ -27,94 +26,139 @@
 provides traditional methods alongside neural network models to help you build
 practical data processing pipelines. We have a rich pool of operators
 available, such as video decoding, audio slicing, frame sampling, feature
 vector dimension reduction, ensembling, and database operations. :snake:
 &emsp;**Pythonic API:** Towhee includes a Pythonic method-chaining API for
 describing custom data processing pipelines. We also support schemas, which
 makes processing unstructured data as easy as handling tabular data. ## What's
-New **v0.8.0 Aug. 16, 2022** * Towhee now supports generating an Nvidia Triton
-Server from a Towhee pipeline, with aditional support for GPU image decoding. *
-Added one audio fingerprinting model: [**nnfp**](https://github.com/towhee-io/
-towhee/tree/branch0.8.0/towhee/models/nnfp) * Added two image embedding models:
-[**RepMLP**](https://github.com/towhee-io/towhee/tree/branch0.8.0/towhee/
-models/repmlp), [**WaveViT**](https://github.com/towhee-io/towhee/tree/
-branch0.8.0/towhee/models/wave_vit) **v0.7.3 Jul. 27, 2022** * Added one
-multimodal (text/image) model: [*CoCa*](https://github.com/towhee-io/towhee/
-tree/branch0.7.3/towhee/models/coca). * Added two video models for grounded
-situation recognition & repetitive action counting: [*CoFormer*](https://
-github.com/towhee-io/towhee/tree/branch0.7.3/towhee/models/coformer),
-[*TransRAC*](https://github.com/towhee-io/towhee/tree/branch0.7.3/towhee/
-models/transrac). * Added two SoTA models for image tasks (image retrieval,
-image classification, etc.): [*CVNet*](https://github.com/towhee-io/towhee/
-tree/branch0.7.3/towhee/models/cvnet), [*MaxViT*](https://github.com/towhee-io/
-towhee/tree/branch0.7.3/towhee/models/max_vit) **v0.7.1 Jul. 1, 2022** * Added
-one image embedding model: [*MPViT*](https://towhee.io/image-embedding/mpvit).
-* Added two video retrieval models: [*BridgeFormer*](https://towhee.io/video-
-text-embedding/bridge-former), [*collaborative-experts*](https://towhee.io/
-video-text-embedding/collaborative-experts). * Added FAISS-based ANNSearch
-operators: *to_faiss*, *faiss_search*. **v0.7.0 Jun. 24, 2022** * Added six
-video understanding/classification models: [*Video Swin Transformer*](https://
-towhee.io/action-classification/video-swin-transformer), [*TSM*](https://
-towhee.io/action-classification/tsm), [*Uniformer*](https://towhee.io/action-
-classification/uniformer), [*OMNIVORE*](https://towhee.io/action-
-classification/omnivore), [*TimeSformer*](https://towhee.io/action-
-classification/timesformer), [*MoViNets*](https://towhee.io/action-
-classification/movinet). * Added four video retrieval models: [*CLIP4Clip*]
-(https://towhee.io/video-text-embedding/clip4clip), [*DRL*](https://towhee.io/
-video-text-embedding/drl), [*Frozen in Time*](https://towhee.io/video-text-
-embedding/frozen-in-time), [*MDMMT*](https://towhee.io/video-text-embedding/
-mdmmt). **v0.6.1 May. 13, 2022** * Added three text-image retrieval models:
-[*CLIP*](https://towhee.io/image-text-embedding/clip), [*BLIP*](https://
-towhee.io/image-text-embedding/blip), [*LightningDOT*](https://towhee.io/image-
-text-embedding/lightningdot). * Added six video understanding/classification
-models from PyTorchVideo: [*I3D*](https://towhee.io/action-classification/
-pytorchvideo), [*C2D*](https://towhee.io/action-classification/pytorchvideo),
-[*Slow*](https://towhee.io/action-classification/pytorchvideo), [*SlowFast*]
-(https://towhee.io/action-classification/pytorchvideo), [*X3D*](https://
-towhee.io/action-classification/pytorchvideo), [*MViT*](https://towhee.io/
-action-classification/pytorchvideo). ## Getting started Towhee requires Python
-3.6+. You can install Towhee via `pip`: ```bash pip install towhee
-towhee.models ``` If you run into any pip-related install problems, please try
-to upgrade pip with `pip install -U pip`. Let's try your first Towhee pipeline.
-Below is an example for how to create a CLIP-based cross modal retrieval
-pipeline with only 15 lines of code. ```python import towhee # create image
-embeddings and build index ( towhee.glob['file_name']('./*.png') .image_decode
-['file_name', 'img']() .image_text_embedding.clip['img', 'vec']
-(model_name='clip_vit_b32', modality='image') .tensor_normalize['vec','vec']()
-.to_faiss[('file_name', 'vec')](findex='./index.bin') ) # search image by text
-results = ( towhee.dc['text'](['puppy Corgi']) .image_text_embedding.clip
-['text', 'vec'](model_name='clip_vit_b32', modality='text') .tensor_normalize
-['vec', 'vec']() .faiss_search['vec', 'results'](findex='./index.bin', k=3)
-.select['text', 'results']() ) ``` [assets/towhee_example.png] Learn more
-examples from the [Towhee Bootcamp](https://codelabs.towhee.io/). ## Core
-Concepts Towhee is composed of four main building blocks - `Operators`,
-`Pipelines`, `DataCollection API` and `Engine`. - __Operators__: An operator is
-a single building block of a neural data processing pipeline. Different
-implementations of operators are categorized by tasks, with each task having a
-standard interface. An operator can be a deep learning model, a data processing
-method, or a Python function. - __Pipelines__: A pipeline is composed of
-several operators interconnected in the form of a DAG (directed acyclic graph).
-This DAG can direct complex functionalities, such as embedding feature
-extraction, data tagging, and cross modal data analysis. - __DataCollection
-API__: A Pythonic and method-chaining style API for building custom pipelines.
-A pipeline defined by the DataColltion API can be run locally on a laptop for
-fast prototyping and then be converted to a docker image, with end-to-end
-optimizations, for production-ready environments. - __Engine__: The engine sits
-at Towhee's core. Given a pipeline, the engine will drive dataflow among
-individual operators, schedule tasks, and monitor compute resource usage (CPU/
-GPU/etc). We provide a basic engine within Towhee to run pipelines on a single-
-instance machine and a Triton-based engine for docker containers. ##
-Contributing Writing code is not the only way to contribute! Submitting issues,
-answering questions, and improving documentation are just some of the many ways
-you can help our growing community. Check out our [contributing page](https://
-github.com/towhee-io/towhee/blob/main/CONTRIBUTING.md) for more information.
-Special thanks goes to these folks for contributing to Towhee, either on
-Github, our Towhee Hub, or elsewhere:
+New **v0.9.0 Dec. 2, 2022** * Added one video classification model: [*Vis4mer*]
+(https://github.com/towhee-io/towhee/tree/branch0.9.0/towhee/models/vis4mer) *
+Added three visual backbones: [*MCProp*](https://github.com/towhee-io/towhee/
+tree/branch0.9.0/towhee/models/mcprop), [*RepLKNet*](https://github.com/towhee-
+io/towhee/tree/branch0.9.0/towhee/models/replknet), [*Shunted Transformer*]
+(https://github.com/towhee-io/towhee/tree/branch0.9.0/towhee/models/
+shunted_transformer) * Add two code search operators: [*code_search.codebert*]
+(https://towhee.io/code-search/codebert), [*code_search.unixcoder*](https://
+towhee.io/code-search/unixcoder) * Add five image captioning operators:
+[*image_captioning.expansionnet-v2*](https://towhee.io/image-captioning/
+expansionnet-v2), [*image_captioning.magic*](https://towhee.io/image-
+captioning/magic), [*image_captioning.clip_caption_reward*](https://towhee.io/
+image-captioning/clip-caption-reward), [*image_captioning.blip*](https://
+towhee.io/image-captioning/blip), [*image_captioning.clipcap*](https://
+towhee.io/image-captioning/clipcap) * Add five image-text embedding operators:
+[*image_text_embedding.albef*](https://towhee.io/image-text-embedding/albef),
+[*image_text_embedding.ru_clip*](https://towhee.io/image-text-embedding/ru-
+clip), [*image_text_embedding.japanese_clip*](https://towhee.io/image-text-
+embedding/japanese-clip), [*image_text_embedding.taiyi*](https://towhee.io/
+image-text-embedding/taiyi), [*image_text_embedding.slip*](https://towhee.io/
+image-text-embedding/slip) * Add one machine-translation operator:
+[*machine_translation.opus_mt*](https://towhee.io/machine-translation/opus-mt)
+* Add one filter-tiny-segments operator: [*video-copy-detection.filter-tiny-
+segments*](https://towhee.io/video-copy-detection/filter-tiny-segments) * Add
+an advanced tutorial for audio fingerprinting: [*Audio Fingerprint II: Music
+Detection with Temporal Localization*](https://github.com/towhee-io/examples/
+blob/main/audio/audio_fingerprint/audio_fingerprint_advanced.ipynb) (increased
+accuracy from 84% to 90%) **v0.8.1 Sep. 30, 2022** * Added four visual
+backbones: [*ISC*](https://github.com/towhee-io/towhee/tree/branch0.8.1/towhee/
+models/isc), [*MetaFormer*](https://github.com/towhee-io/towhee/tree/
+branch0.8.1/towhee/models/metaformer), [*ConvNext*](https://github.com/towhee-
+io/towhee/tree/branch0.8.1/towhee/models/convnext), [*HorNet*](https://
+github.com/towhee-io/towhee/tree/branch0.8.1/towhee/models/hornet) * Add two
+video de-copy operators: [*select-video*](https://towhee.io/video-copy-
+detection/select-video), [*temporal-network*](https://towhee.io/video-copy-
+detection/temporal-network) * Add one image embedding operator specifically
+designed for image retrieval and video de-copy with SOTA performance on VCSL
+dataset: [*isc*](https://towhee.io/image-embedding/isc) * Add one audio
+embedding operator specified for audio fingerprint: [*audio_embedding.nnfp*]
+(https://towhee.io/audio-embedding/nnfp) (with pretrained weights) * Add one
+tutorial for video de-copy: [*How to Build a Video Segment Copy Detection
+System*](https://github.com/towhee-io/examples/blob/main/video/
+video_deduplication/segment_level/video_deduplication_at_segment_level.ipynb) *
+Add one beginner tutorial for audio fingerprint: [*Audio Fingerprint I: Build a
+Demo with Towhee & Milvus*](https://github.com/towhee-io/examples/blob/main/
+audio/audio_fingerprint/audio_fingerprint_beginner.ipynb) **v0.8.0 Aug. 16,
+2022** * Towhee now supports generating an Nvidia Triton Server from a Towhee
+pipeline, with aditional support for GPU image decoding. * Added one audio
+fingerprinting model: [*nnfp*](https://github.com/towhee-io/towhee/tree/
+branch0.8.0/towhee/models/nnfp) * Added two image embedding models: [*RepMLP*]
+(https://github.com/towhee-io/towhee/tree/branch0.8.0/towhee/models/repmlp),
+[**WaveViT**](https://github.com/towhee-io/towhee/tree/branch0.8.0/towhee/
+models/wave_vit) **v0.7.3 Jul. 27, 2022** * Added one multimodal (text/image)
+model: [*CoCa*](https://github.com/towhee-io/towhee/tree/branch0.7.3/towhee/
+models/coca). * Added two video models for grounded situation recognition &
+repetitive action counting: [*CoFormer*](https://github.com/towhee-io/towhee/
+tree/branch0.7.3/towhee/models/coformer), [*TransRAC*](https://github.com/
+towhee-io/towhee/tree/branch0.7.3/towhee/models/transrac). * Added two SoTA
+models for image tasks (image retrieval, image classification, etc.): [*CVNet*]
+(https://github.com/towhee-io/towhee/tree/branch0.7.3/towhee/models/cvnet),
+[*MaxViT*](https://github.com/towhee-io/towhee/tree/branch0.7.3/towhee/models/
+max_vit) **v0.7.1 Jul. 1, 2022** * Added one image embedding model: [*MPViT*]
+(https://towhee.io/image-embedding/mpvit). * Added two video retrieval models:
+[*BridgeFormer*](https://towhee.io/video-text-embedding/bridge-former),
+[*collaborative-experts*](https://towhee.io/video-text-embedding/collaborative-
+experts). * Added FAISS-based ANNSearch operators: *to_faiss*, *faiss_search*.
+**v0.7.0 Jun. 24, 2022** * Added six video understanding/classification models:
+[*Video Swin Transformer*](https://towhee.io/action-classification/video-swin-
+transformer), [*TSM*](https://towhee.io/action-classification/tsm),
+[*Uniformer*](https://towhee.io/action-classification/uniformer), [*OMNIVORE*]
+(https://towhee.io/action-classification/omnivore), [*TimeSformer*](https://
+towhee.io/action-classification/timesformer), [*MoViNets*](https://towhee.io/
+action-classification/movinet). * Added four video retrieval models:
+[*CLIP4Clip*](https://towhee.io/video-text-embedding/clip4clip), [*DRL*](https:
+//towhee.io/video-text-embedding/drl), [*Frozen in Time*](https://towhee.io/
+video-text-embedding/frozen-in-time), [*MDMMT*](https://towhee.io/video-text-
+embedding/mdmmt). **v0.6.1 May. 13, 2022** * Added three text-image retrieval
+models: [*CLIP*](https://towhee.io/image-text-embedding/clip), [*BLIP*](https:/
+/towhee.io/image-text-embedding/blip), [*LightningDOT*](https://towhee.io/
+image-text-embedding/lightningdot). * Added six video understanding/
+classification models from PyTorchVideo: [*I3D*](https://towhee.io/action-
+classification/pytorchvideo), [*C2D*](https://towhee.io/action-classification/
+pytorchvideo), [*Slow*](https://towhee.io/action-classification/pytorchvideo),
+[*SlowFast*](https://towhee.io/action-classification/pytorchvideo), [*X3D*]
+(https://towhee.io/action-classification/pytorchvideo), [*MViT*](https://
+towhee.io/action-classification/pytorchvideo). ## Getting started Towhee
+requires Python 3.6+. You can install Towhee via `pip`: ```bash pip install
+towhee towhee.models ``` If you run into any pip-related install problems,
+please try to upgrade pip with `pip install -U pip`. Let's try your first
+Towhee pipeline. Below is an example for how to create a CLIP-based cross modal
+retrieval pipeline with only 15 lines of code. ```python import towhee # create
+image embeddings and build index ( towhee.glob['file_name']('./*.png')
+.image_decode['file_name', 'img']() .image_text_embedding.clip['img', 'vec']
+(model_name='clip_vit_base_patch32', modality='image') .tensor_normalize
+['vec','vec']() .to_faiss[('file_name', 'vec')](findex='./index.bin') ) #
+search image by text results = ( towhee.dc['text'](['puppy Corgi'])
+.image_text_embedding.clip['text', 'vec'](model_name='clip_vit_base_patch32',
+modality='text') .tensor_normalize['vec', 'vec']() .faiss_search['vec',
+'results'](findex='./index.bin', k=3) .select['text', 'results']() ) ```
+[assets/towhee_example.png] Learn more examples from the [Towhee Bootcamp]
+(https://codelabs.towhee.io/). ## Core Concepts Towhee is composed of four main
+building blocks - `Operators`, `Pipelines`, `DataCollection API` and `Engine`.
+- __Operators__: An operator is a single building block of a neural data
+processing pipeline. Different implementations of operators are categorized by
+tasks, with each task having a standard interface. An operator can be a deep
+learning model, a data processing method, or a Python function. -
+__Pipelines__: A pipeline is composed of several operators interconnected in
+the form of a DAG (directed acyclic graph). This DAG can direct complex
+functionalities, such as embedding feature extraction, data tagging, and cross
+modal data analysis. - __DataCollection API__: A Pythonic and method-chaining
+style API for building custom pipelines. A pipeline defined by the DataColltion
+API can be run locally on a laptop for fast prototyping and then be converted
+to a docker image, with end-to-end optimizations, for production-ready
+environments. - __Engine__: The engine sits at Towhee's core. Given a pipeline,
+the engine will drive dataflow among individual operators, schedule tasks, and
+monitor compute resource usage (CPU/GPU/etc). We provide a basic engine within
+Towhee to run pipelines on a single-instance machine and a Triton-based engine
+for docker containers. ## Contributing Writing code is not the only way to
+contribute! Submitting issues, answering questions, and improving documentation
+are just some of the many ways you can help our growing community. Check out
+our [contributing page](https://github.com/towhee-io/towhee/blob/main/
+CONTRIBUTING.md) for more information. Special thanks goes to these folks for
+contributing to Towhee, either on Github, our Towhee Hub, or elsewhere:
 
-[https://img.shields.io/badge/all--contributors-34-orange]
+[https://img.shields.io/badge/all--contributors-33-orange]
 [https://avatars.githubusercontent.com/u/34787227?v=4] [https://
 avatars.githubusercontent.com/u/72550076?v=4] [https://
 avatars.githubusercontent.com/u/57477222?v=4] [https://
 avatars.githubusercontent.com/u/109071306?v=4] [https://
 avatars.githubusercontent.com/u/20420181?v=4] [https://
 avatars.githubusercontent.com/u/88148730?v=4] [https://
 avatars.githubusercontent.com/u/83755740?v=4] [https://
@@ -122,15 +166,14 @@
 avatars.githubusercontent.com/u/47691077?v=4] [https://
 avatars.githubusercontent.com/u/81822489?v=4] [https://
 avatars.githubusercontent.com/u/6334158?v=4] [https://
 avatars.githubusercontent.com/u/103474331?v=4] [https://
 avatars.githubusercontent.com/u/67197231?v=4] [https://
 avatars.githubusercontent.com/u/86251631?v=4] [https://
 avatars.githubusercontent.com/u/24581746?v=4] [https://
-avatars.githubusercontent.com/u/93511422?v=4] [https://
 avatars.githubusercontent.com/u/34296482?v=4] [https://
 avatars.githubusercontent.com/u/106302799?v=4] [https://
 avatars.githubusercontent.com/u/14136703?v=4] [https://
 avatars.githubusercontent.com/u/37455387?v=4] [https://
 avatars.githubusercontent.com/u/40853054?v=4] [https://
 avatars.githubusercontent.com/u/28955741?v=4] [https://
 avatars.githubusercontent.com/u/65100038?v=4] [https://
```

