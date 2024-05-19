# Comparing `tmp/continuous_eval-0.3.7.tar.gz` & `tmp/continuous_eval-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuous_eval-0.3.7.tar", max compression
+gzip compressed data, was "continuous_eval-0.3.8.tar", max compression
```

## Comparing `continuous_eval-0.3.7.tar` & `continuous_eval-0.3.8.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0    11357 2023-12-10 20:19:38.190467 continuous_eval-0.3.7/LICENSE
--rw-r--r--   0        0        0     9137 2024-04-25 01:13:40.195509 continuous_eval-0.3.7/README.md
--rw-r--r--   0        0        0        0 2024-02-25 01:21:36.780803 continuous_eval-0.3.7/continuous_eval/__init__.py
--rw-r--r--   0        0        0       64 2024-01-12 14:57:28.874524 continuous_eval-0.3.7/continuous_eval/classifiers/__init__.py
--rw-r--r--   0        0        0     3058 2024-04-01 22:15:42.805184 continuous_eval-0.3.7/continuous_eval/classifiers/ensemble.py
--rw-r--r--   0        0        0      652 2024-04-01 22:15:42.806178 continuous_eval-0.3.7/continuous_eval/classifiers/utils.py
--rw-r--r--   0        0        0     3031 2024-02-25 01:21:36.781330 continuous_eval-0.3.7/continuous_eval/data_downloader.py
--rw-r--r--   0        0        0     3609 2024-04-01 22:15:42.806551 continuous_eval-0.3.7/continuous_eval/datatypes.py
--rw-r--r--   0        0        0      251 2024-02-25 01:21:36.781535 continuous_eval-0.3.7/continuous_eval/eval/__init__.py
--rw-r--r--   0        0        0     6234 2024-04-25 01:13:40.196141 continuous_eval-0.3.7/continuous_eval/eval/dataset.py
--rw-r--r--   0        0        0     9394 2024-03-08 16:03:17.678226 continuous_eval-0.3.7/continuous_eval/eval/manager.py
--rw-r--r--   0        0        0     1627 2024-02-25 01:21:36.781780 continuous_eval-0.3.7/continuous_eval/eval/modules.py
--rw-r--r--   0        0        0     4539 2024-02-25 01:21:36.781864 continuous_eval-0.3.7/continuous_eval/eval/pipeline.py
--rw-r--r--   0        0        0     4420 2024-04-01 22:15:42.808392 continuous_eval-0.3.7/continuous_eval/eval/result_types.py
--rw-r--r--   0        0        0     1380 2024-02-25 01:21:36.782015 continuous_eval-0.3.7/continuous_eval/eval/tests.py
--rw-r--r--   0        0        0      122 2024-02-25 01:21:36.782079 continuous_eval-0.3.7/continuous_eval/eval/types.py
--rw-r--r--   0        0        0     1107 2024-03-04 17:53:52.558401 continuous_eval-0.3.7/continuous_eval/eval/utils.py
--rw-r--r--   0        0        0       69 2024-01-12 14:57:28.877604 continuous_eval-0.3.7/continuous_eval/generators/__init__.py
--rw-r--r--   0        0        0    12800 2024-03-26 21:20:35.487618 continuous_eval-0.3.7/continuous_eval/generators/simple.py
--rw-r--r--   0        0        0    10016 2024-04-25 01:36:49.832110 continuous_eval-0.3.7/continuous_eval/llm_factory.py
--rw-r--r--   0        0        0        0 2024-04-01 22:15:42.809284 continuous_eval-0.3.7/continuous_eval/llms/__init__.py
--rw-r--r--   0        0        0      780 2024-04-01 22:15:42.809509 continuous_eval-0.3.7/continuous_eval/llms/bedrock.py
--rw-r--r--   0        0        0       48 2024-02-25 01:21:36.782270 continuous_eval-0.3.7/continuous_eval/metrics/__init__.py
--rw-r--r--   0        0        0     1732 2024-04-01 22:15:42.809855 continuous_eval-0.3.7/continuous_eval/metrics/_utils/simple_tokenizer.py
--rw-r--r--   0        0        0     2471 2024-03-08 16:03:17.679836 continuous_eval-0.3.7/continuous_eval/metrics/base.py
--rw-r--r--   0        0        0       91 2024-02-27 06:34:50.556016 continuous_eval-0.3.7/continuous_eval/metrics/classification/__init__.py
--rw-r--r--   0        0        0     2233 2024-02-27 06:34:50.556112 continuous_eval-0.3.7/continuous_eval/metrics/classification/classification.py
--rw-r--r--   0        0        0      111 2024-03-08 16:03:17.679999 continuous_eval-0.3.7/continuous_eval/metrics/code/python/__init__.py
--rw-r--r--   0        0        0    11635 2024-03-08 16:03:17.680796 continuous_eval-0.3.7/continuous_eval/metrics/code/python/code_deterministic_metrics.py
--rw-r--r--   0        0        0      678 2024-03-26 21:20:35.488791 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/__init__.py
--rw-r--r--   0        0        0     3109 2024-03-26 21:20:35.489197 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/bert.py
--rw-r--r--   0        0        0     2879 2024-04-01 22:15:42.810274 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/custom.py
--rw-r--r--   0        0        0     4814 2024-03-08 16:03:17.681650 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/deterministic.py
--rw-r--r--   0        0        0    11472 2024-04-01 22:15:42.811029 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/llm_based.py
--rw-r--r--   0        0        0     5741 2024-03-26 21:20:35.489763 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/semantic.py
--rw-r--r--   0        0        0     2865 2024-04-01 22:15:42.811345 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/utils.py
--rw-r--r--   0        0        0      437 2024-04-25 01:13:57.116186 continuous_eval-0.3.7/continuous_eval/metrics/retrieval/__init__.py
--rw-r--r--   0        0        0     6541 2024-03-26 21:20:35.490910 continuous_eval-0.3.7/continuous_eval/metrics/retrieval/llm_based.py
--rw-r--r--   0        0        0     1918 2024-04-25 01:13:52.350927 continuous_eval-0.3.7/continuous_eval/metrics/retrieval/matching_strategy.py
--rw-r--r--   0        0        0     2470 2024-04-25 01:13:40.196878 continuous_eval-0.3.7/continuous_eval/metrics/retrieval/precision_recall_f1.py
--rw-r--r--   0        0        0     3394 2024-04-25 01:13:40.198789 continuous_eval-0.3.7/continuous_eval/metrics/retrieval/ranked.py
--rw-r--r--   0        0        0     1500 2024-02-25 01:21:36.783877 continuous_eval-0.3.7/continuous_eval/metrics/tools/match.py
--rw-r--r--   0        0        0     4013 2024-02-27 06:34:50.556585 continuous_eval-0.3.7/continuous_eval/utils/telemetry.py
--rw-r--r--   0        0        0     1850 2024-04-25 01:38:41.759442 continuous_eval-0.3.7/pyproject.toml
--rw-r--r--   0        0        0    11375 1970-01-01 00:00:00.000000 continuous_eval-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-17 21:26:45.588731 continuous_eval-0.3.8/LICENSE
+-rw-r--r--   0        0        0     9731 2024-05-19 17:18:08.444721 continuous_eval-0.3.8/README.md
+-rw-r--r--   0        0        0        0 2024-02-25 04:22:14.516782 continuous_eval-0.3.8/continuous_eval/__init__.py
+-rw-r--r--   0        0        0       64 2024-02-17 05:39:52.426571 continuous_eval-0.3.8/continuous_eval/classifiers/__init__.py
+-rw-r--r--   0        0        0     3071 2024-05-16 15:09:47.554528 continuous_eval-0.3.8/continuous_eval/classifiers/ensemble.py
+-rw-r--r--   0        0        0      652 2024-03-22 00:45:46.211844 continuous_eval-0.3.8/continuous_eval/classifiers/utils.py
+-rw-r--r--   0        0        0     3014 2024-05-19 17:18:08.445148 continuous_eval-0.3.8/continuous_eval/data_downloader.py
+-rw-r--r--   0        0        0     3740 2024-05-16 15:14:21.930240 continuous_eval-0.3.8/continuous_eval/datatypes.py
+-rw-r--r--   0        0        0      308 2024-05-19 17:18:08.445480 continuous_eval-0.3.8/continuous_eval/eval/__init__.py
+-rw-r--r--   0        0        0     6829 2024-05-19 17:18:08.445900 continuous_eval-0.3.8/continuous_eval/eval/dataset.py
+-rw-r--r--   0        0        0     3238 2024-05-19 17:18:08.446195 continuous_eval-0.3.8/continuous_eval/eval/logger.py
+-rw-r--r--   0        0        0     1637 2024-05-19 17:18:08.446528 continuous_eval-0.3.8/continuous_eval/eval/modules.py
+-rw-r--r--   0        0        0     4539 2024-05-17 18:58:11.809843 continuous_eval-0.3.8/continuous_eval/eval/pipeline.py
+-rw-r--r--   0        0        0     5883 2024-05-19 17:18:08.447080 continuous_eval-0.3.8/continuous_eval/eval/result_types.py
+-rw-r--r--   0        0        0     3609 2024-05-19 17:18:08.447290 continuous_eval-0.3.8/continuous_eval/eval/runner.py
+-rw-r--r--   0        0        0     1380 2024-02-25 04:22:14.518180 continuous_eval-0.3.8/continuous_eval/eval/tests.py
+-rw-r--r--   0        0        0      288 2024-05-19 17:18:08.447591 continuous_eval-0.3.8/continuous_eval/eval/types.py
+-rw-r--r--   0        0        0     1107 2024-05-18 03:37:31.360398 continuous_eval-0.3.8/continuous_eval/eval/utils.py
+-rw-r--r--   0        0        0       69 2024-02-17 05:39:52.427862 continuous_eval-0.3.8/continuous_eval/generators/__init__.py
+-rw-r--r--   0        0        0    12878 2024-05-19 17:18:08.447912 continuous_eval-0.3.8/continuous_eval/generators/simple.py
+-rw-r--r--   0        0        0    10016 2024-04-30 03:48:52.158450 continuous_eval-0.3.8/continuous_eval/llm_factory.py
+-rw-r--r--   0        0        0        0 2024-03-27 04:22:00.195998 continuous_eval-0.3.8/continuous_eval/llms/__init__.py
+-rw-r--r--   0        0        0      780 2024-03-27 05:39:44.227478 continuous_eval-0.3.8/continuous_eval/llms/bedrock.py
+-rw-r--r--   0        0        0       48 2024-02-25 04:22:14.519065 continuous_eval-0.3.8/continuous_eval/metrics/__init__.py
+-rw-r--r--   0        0        0     1732 2024-03-27 04:07:30.402986 continuous_eval-0.3.8/continuous_eval/metrics/_utils/simple_tokenizer.py
+-rw-r--r--   0        0        0     2471 2024-03-08 08:55:45.593923 continuous_eval-0.3.8/continuous_eval/metrics/base.py
+-rw-r--r--   0        0        0       91 2024-02-27 06:09:06.065186 continuous_eval-0.3.8/continuous_eval/metrics/classification/__init__.py
+-rw-r--r--   0        0        0     2233 2024-02-27 06:09:06.065562 continuous_eval-0.3.8/continuous_eval/metrics/classification/classification.py
+-rw-r--r--   0        0        0      111 2024-03-08 07:02:54.302236 continuous_eval-0.3.8/continuous_eval/metrics/code/python/__init__.py
+-rw-r--r--   0        0        0    11635 2024-03-08 08:55:45.681607 continuous_eval-0.3.8/continuous_eval/metrics/code/python/code_deterministic_metrics.py
+-rw-r--r--   0        0        0      678 2024-03-17 22:25:39.167477 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/__init__.py
+-rw-r--r--   0        0        0     3769 2024-05-16 15:14:21.925777 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/bert.py
+-rw-r--r--   0        0        0     2945 2024-05-16 15:14:21.919758 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/custom.py
+-rw-r--r--   0        0        0     4814 2024-05-18 03:37:32.100141 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/deterministic.py
+-rw-r--r--   0        0        0    11472 2024-03-27 05:39:44.567238 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/llm_based.py
+-rw-r--r--   0        0        0     5770 2024-05-16 15:14:21.670171 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/semantic.py
+-rw-r--r--   0        0        0     2865 2024-03-27 05:39:44.530970 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/utils.py
+-rw-r--r--   0        0        0      437 2024-02-25 04:22:14.520214 continuous_eval-0.3.8/continuous_eval/metrics/retrieval/__init__.py
+-rw-r--r--   0        0        0     6541 2024-04-05 23:59:38.533703 continuous_eval-0.3.8/continuous_eval/metrics/retrieval/llm_based.py
+-rw-r--r--   0        0        0     1918 2024-02-25 04:22:14.520478 continuous_eval-0.3.8/continuous_eval/metrics/retrieval/matching_strategy.py
+-rw-r--r--   0        0        0     2470 2024-04-02 16:24:12.028818 continuous_eval-0.3.8/continuous_eval/metrics/retrieval/precision_recall_f1.py
+-rw-r--r--   0        0        0     3394 2024-04-02 16:24:12.029049 continuous_eval-0.3.8/continuous_eval/metrics/retrieval/ranked.py
+-rw-r--r--   0        0        0     1867 2024-05-19 17:18:08.448171 continuous_eval-0.3.8/continuous_eval/metrics/tools/match.py
+-rw-r--r--   0        0        0     4013 2024-02-26 23:53:19.235416 continuous_eval-0.3.8/continuous_eval/utils/telemetry.py
+-rw-r--r--   0        0        0     1671 2024-05-19 17:18:08.456046 continuous_eval-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0    11364 1970-01-01 00:00:00.000000 continuous_eval-0.3.8/PKG-INFO
```

### Comparing `continuous_eval-0.3.7/LICENSE` & `continuous_eval-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/README.md` & `continuous_eval-0.3.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   <a href="https://pypi.python.org/pypi/continuous-eval/">![https://github.com/Naereen/badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)</a>
   <a a href="https://github.com/relari-ai/continuous-eval/blob/main/LICENSE">![https://pypi.python.org/pypi/continuous-eval/](https://img.shields.io/pypi/l/continuous-eval.svg)</a>
 
 
 </div>
 
 <h2 align="center">
-  <p>Open-Source Evaluation for GenAI Application Pipelines</p>
+  <p>Open-Source Evaluation for GenAI Applications</p>
 </h2>
 
 
 
 ## Overview
 
 `continuous-eval` is an open-source package created for granular and holistic evaluation of GenAI application pipelines. 
@@ -139,20 +139,21 @@
         <td>Define your own metrics</td>
     </tr>
 </table>
 
 To define your own metrics, you only need to extend the [Metric](continuous_eval/metrics/base.py#L23C7-L23C13) class implementing the `__call__` method.
 Optional methods are `batch` (if it is possible to implement optimizations for batch processing) and `aggregate` (to aggregate metrics results over multiple samples_).
 
-## Run evaluation on pipeline modules
+## Run evaluation on a pipeline
 
 Define modules in your pipeline and select corresponding metrics.
 
 ```python
-from continuous_eval.eval import Module, ModuleOutput, Pipeline, Dataset
+from continuous_eval.eval import Module, ModuleOutput, Pipeline, Dataset, EvaluationRunner
+from continuous_eval.eval.logger import PipelineLogger
 from continuous_eval.metrics.retrieval import PrecisionRecallF1, RankedRetrievalMetrics
 from continuous_eval.metrics.generation.text import DeterministicAnswerCorrectness
 from typing import List, Dict
 
 dataset = Dataset("dataset_folder")
 
 # Simple 3-step RAG pipeline with Retriever->Reranker->Generation
@@ -195,55 +196,60 @@
 pipeline = Pipeline([retriever, reranker, llm], dataset=dataset)
 print(pipeline.graph_repr()) # optional: visualize the pipeline
 ```
 
 Now you can run the evaluation on your pipeline
 
 ```python
-eval_manager.start_run()
-  while eval_manager.is_running():
-    if eval_manager.curr_sample is None:
-      break
-    q = eval_manager.curr_sample["question"] # get the question or any other field
-    # run your pipeline ...
-    eval_manager.next_sample()
-```
+pipelog = PipelineLogger(pipeline=pipeline)
 
-To **log** the results you just need to call the `eval_manager.log` method with the module name and the output, for example:
+# now run your LLM application pipeline, and for each module, log the results:
+pipelog.log(uid=sample_uid, module="module_name", value=data)
 
-```python
-eval_manager.log("answer_generator", response)
+# Once you finish logging the data, you can use the EvaluationRunner to evaluate the logs
+evalrunner = EvaluationRunner(pipeline)
+metrics = evalrunner.evaluate(pipelog)
+metrics.results() # returns a dictionary with the results
 ```
 
-The evaluator manager also offers
+To run evaluation over an existing dataset (BYODataset), you can run the following:
 
-- `eval_manager.run_metrics()` to run all the metrics defined in the pipeline
-- `eval_manager.run_tests()` to run the tests defined in the pipeline (see the documentation [docs](docs.relari.ai) for more details)
+```python
+dataset = Dataset(...)
+evalrunner = EvaluationRunner(pipeline)
+metrics = evalrunner.evaluate(dataset)
+```
 
 ## Synthetic Data Generation
 
 Ground truth data, or reference data, is important for evaluation as it can offer a comprehensive and consistent measurement of system performance. However, it is often costly and time-consuming to manually curate such a golden dataset.
 We have created a synthetic data pipeline that can custom generate user interaction data for a variety of use cases such as RAG, agents, copilots. They can serve a starting point for a golden dataset for evaluation or for other training purposes. Below is an example for Coding Agents. Try out this demo: [Synthetic Data Demo](https://www.relari.ai/synthetic-data-demo)
 
 <h1 align="center">
   <img
     src="docs/public/synthetic-data-demo.png"
   >
 </h1>
 
+## 💡 Contributing
+
+Interested in contributing? Contributions to LlamaIndex core as well as contributing
+integrations that build on the core are both accepted and highly encouraged! See our [Contribution Guide](CONTRIBUTING.md) for more details.
 
 ## Resources
 
 - **Docs:** [link](https://docs.relari.ai/)
 - **Examples Repo**: [end-to-end example repo](https://github.com/relari-ai/examples)
 - **Blog Posts:**
   - Practical Guide to RAG Pipeline Evaluation: [Part 1: Retrieval](https://medium.com/relari/a-practical-guide-to-rag-pipeline-evaluation-part-1-27a472b09893), [Part 2: Generation](https://medium.com/relari/a-practical-guide-to-rag-evaluation-part-2-generation-c79b1bde0f5d)
   - How important is a Golden Dataset for LLM evaluation?
  [(link)](https://medium.com/relari/how-important-is-a-golden-dataset-for-llm-pipeline-evaluation-4ef6deb14dc5)
   - How to evaluate complex GenAI Apps: a granular approach [(link)](https://medium.com/relari/how-to-evaluate-complex-genai-apps-a-granular-approach-0ab929d5b3e2)
+  - How to Make the Most Out of LLM Production Data: Simulated User Feedback [(link)](https://medium.com/towards-data-science/how-to-make-the-most-out-of-llm-production-data-simulated-user-feedback-843c444febc7)
+  - Generate Synthetic Data to Test LLM Applications [(link)](https://medium.com/relari/generate-synthetic-data-to-test-llm-applications-4bffeb51b80e)
 - **Discord:** Join our community of LLM developers [Discord](https://discord.gg/GJnM8SRsHr)
 - **Reach out to founders:** [Email](mailto:founders@relari.ai) or [Schedule a chat](https://cal.com/pasquale/continuous-eval)
 
 ## License
 
 This project is licensed under the Apache 2.0 - see the [LICENSE](LICENSE) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
    _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_!_[_h_t_t_p_s_:_/_/_p_y_p_i_._p_y_t_h_o_n_._o_r_g_/_p_y_p_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_/_]_(_h_t_t_p_s_:_/_/
    _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_._s_v_g_) _!_[_h_t_t_p_s_:_/_/_G_i_t_H_u_b_._c_o_m_/
   _r_e_l_a_r_i_-_a_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_/_r_e_l_e_a_s_e_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/
    _r_e_l_a_r_i_-_a_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_) _!_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_N_a_e_r_e_e_n_/_b_a_d_g_e_s_/_]_(_h_t_t_p_s_:_/_/
    _b_a_d_g_e_n_._n_e_t_/_b_a_d_g_e_/_O_p_e_n_%_2_0_S_o_u_r_c_e_%_2_0_%_3_F_/_Y_e_s_%_2_1_/_b_l_u_e_?_i_c_o_n_=_g_i_t_h_u_b_) ![https://
      pypi.python.org/pypi/continuous-eval/](https://img.shields.io/pypi/l/
                              continuous-eval.svg)
-      ********** OOppeenn--SSoouurrccee EEvvaalluuaattiioonn ffoorr GGeennAAII AApppplliiccaattiioonn PPiippeelliinneess **********
+           ********** OOppeenn--SSoouurrccee EEvvaalluuaattiioonn ffoorr GGeennAAII AApppplliiccaattiioonnss **********
 ## Overview `continuous-eval` is an open-source package created for granular
 and holistic evaluation of GenAI application pipelines.
                ************ [[ddooccss//ppuubblliicc//mmoodduullee--lleevveell--eevvaall..ppnngg]] ************
 ## How is continuous-eval different? - **Modularized Evaluation**: Measure each
 module in the pipeline with tailored metrics. - **Comprehensive Metric
 Library**: Covers Retrieval-Augmented Generation (RAG), Code Generation, Agent
 Tool Use, Classification and a variety of other LLM use cases. Mix and match
@@ -46,17 +46,18 @@
                 LLM-based     LLMBasedCodeGeneration
 Agent Tools     Deterministic ToolSelectionAccuracy
 Custom                        Define your own metrics
 To define your own metrics, you only need to extend the [Metric]
 (continuous_eval/metrics/base.py#L23C7-L23C13) class implementing the
 `__call__` method. Optional methods are `batch` (if it is possible to implement
 optimizations for batch processing) and `aggregate` (to aggregate metrics
-results over multiple samples_). ## Run evaluation on pipeline modules Define
-modules in your pipeline and select corresponding metrics. ```python from
-continuous_eval.eval import Module, ModuleOutput, Pipeline, Dataset from
+results over multiple samples_). ## Run evaluation on a pipeline Define modules
+in your pipeline and select corresponding metrics. ```python from
+continuous_eval.eval import Module, ModuleOutput, Pipeline, Dataset,
+EvaluationRunner from continuous_eval.eval.logger import PipelineLogger from
 continuous_eval.metrics.retrieval import PrecisionRecallF1,
 RankedRetrievalMetrics from continuous_eval.metrics.generation.text import
 DeterministicAnswerCorrectness from typing import List, Dict dataset = Dataset
 ("dataset_folder") # Simple 3-step RAG pipeline with Retriever->Reranker-
 >Generation retriever = Module( name="Retriever", input=dataset.question,
 output=List[str], eval=[ PrecisionRecallF1().use
 ( retrieved_context=ModuleOutput(),
@@ -66,44 +67,51 @@
 ground_truth_context=dataset.ground_truth_context, ), ], ) llm = Module
 ( name="answer_generator", input=reranker, output=str, eval=
 [ FleschKincaidReadability().use(answer=ModuleOutput()),
 DeterministicAnswerCorrectness().use( answer=ModuleOutput(),
 ground_truth_answers=dataset.ground_truths ), ], ) pipeline = Pipeline(
 [retriever, reranker, llm], dataset=dataset) print(pipeline.graph_repr()) #
 optional: visualize the pipeline ``` Now you can run the evaluation on your
-pipeline ```python eval_manager.start_run() while eval_manager.is_running(): if
-eval_manager.curr_sample is None: break q = eval_manager.curr_sample
-["question"] # get the question or any other field # run your pipeline ...
-eval_manager.next_sample() ``` To **log** the results you just need to call the
-`eval_manager.log` method with the module name and the output, for example:
-```python eval_manager.log("answer_generator", response) ``` The evaluator
-manager also offers - `eval_manager.run_metrics()` to run all the metrics
-defined in the pipeline - `eval_manager.run_tests()` to run the tests defined
-in the pipeline (see the documentation [docs](docs.relari.ai) for more details)
-## Synthetic Data Generation Ground truth data, or reference data, is important
-for evaluation as it can offer a comprehensive and consistent measurement of
-system performance. However, it is often costly and time-consuming to manually
-curate such a golden dataset. We have created a synthetic data pipeline that
-can custom generate user interaction data for a variety of use cases such as
-RAG, agents, copilots. They can serve a starting point for a golden dataset for
-evaluation or for other training purposes. Below is an example for Coding
-Agents. Try out this demo: [Synthetic Data Demo](https://www.relari.ai/
-synthetic-data-demo)
+pipeline ```python pipelog = PipelineLogger(pipeline=pipeline) # now run your
+LLM application pipeline, and for each module, log the results: pipelog.log
+(uid=sample_uid, module="module_name", value=data) # Once you finish logging
+the data, you can use the EvaluationRunner to evaluate the logs evalrunner =
+EvaluationRunner(pipeline) metrics = evalrunner.evaluate(pipelog)
+metrics.results() # returns a dictionary with the results ``` To run evaluation
+over an existing dataset (BYODataset), you can run the following: ```python
+dataset = Dataset(...) evalrunner = EvaluationRunner(pipeline) metrics =
+evalrunner.evaluate(dataset) ``` ## Synthetic Data Generation Ground truth
+data, or reference data, is important for evaluation as it can offer a
+comprehensive and consistent measurement of system performance. However, it is
+often costly and time-consuming to manually curate such a golden dataset. We
+have created a synthetic data pipeline that can custom generate user
+interaction data for a variety of use cases such as RAG, agents, copilots. They
+can serve a starting point for a golden dataset for evaluation or for other
+training purposes. Below is an example for Coding Agents. Try out this demo:
+[Synthetic Data Demo](https://www.relari.ai/synthetic-data-demo)
               ************ [[ddooccss//ppuubblliicc//ssyynntthheettiicc--ddaattaa--ddeemmoo..ppnngg]] ************
-## Resources - **Docs:** [link](https://docs.relari.ai/) - **Examples Repo**:
-[end-to-end example repo](https://github.com/relari-ai/examples) - **Blog
-Posts:** - Practical Guide to RAG Pipeline Evaluation: [Part 1: Retrieval]
-(https://medium.com/relari/a-practical-guide-to-rag-pipeline-evaluation-part-1-
-27a472b09893), [Part 2: Generation](https://medium.com/relari/a-practical-
-guide-to-rag-evaluation-part-2-generation-c79b1bde0f5d) - How important is a
-Golden Dataset for LLM evaluation? [(link)](https://medium.com/relari/how-
-important-is-a-golden-dataset-for-llm-pipeline-evaluation-4ef6deb14dc5) - How
-to evaluate complex GenAI Apps: a granular approach [(link)](https://
-medium.com/relari/how-to-evaluate-complex-genai-apps-a-granular-approach-
-0ab929d5b3e2) - **Discord:** Join our community of LLM developers [Discord]
+## ð¡ Contributing Interested in contributing? Contributions to LlamaIndex
+core as well as contributing integrations that build on the core are both
+accepted and highly encouraged! See our [Contribution Guide](CONTRIBUTING.md)
+for more details. ## Resources - **Docs:** [link](https://docs.relari.ai/) -
+**Examples Repo**: [end-to-end example repo](https://github.com/relari-ai/
+examples) - **Blog Posts:** - Practical Guide to RAG Pipeline Evaluation: [Part
+1: Retrieval](https://medium.com/relari/a-practical-guide-to-rag-pipeline-
+evaluation-part-1-27a472b09893), [Part 2: Generation](https://medium.com/
+relari/a-practical-guide-to-rag-evaluation-part-2-generation-c79b1bde0f5d) -
+How important is a Golden Dataset for LLM evaluation? [(link)](https://
+medium.com/relari/how-important-is-a-golden-dataset-for-llm-pipeline-
+evaluation-4ef6deb14dc5) - How to evaluate complex GenAI Apps: a granular
+approach [(link)](https://medium.com/relari/how-to-evaluate-complex-genai-apps-
+a-granular-approach-0ab929d5b3e2) - How to Make the Most Out of LLM Production
+Data: Simulated User Feedback [(link)](https://medium.com/towards-data-science/
+how-to-make-the-most-out-of-llm-production-data-simulated-user-feedback-
+843c444febc7) - Generate Synthetic Data to Test LLM Applications [(link)]
+(https://medium.com/relari/generate-synthetic-data-to-test-llm-applications-
+4bffeb51b80e) - **Discord:** Join our community of LLM developers [Discord]
 (https://discord.gg/GJnM8SRsHr) - **Reach out to founders:** [Email](mailto:
 founders@relari.ai) or [Schedule a chat](https://cal.com/pasquale/continuous-
 eval) ## License This project is licensed under the Apache 2.0 - see the
 [LICENSE](LICENSE) file for details. ## Open Analytics We monitor basic
 anonymous usage statistics to understand our users' preferences, inform new
 features, and identify areas that might need improvement. You can take a look
 at exactly what we track in the [telemetry code](continuous_eval/utils/
```

### Comparing `continuous_eval-0.3.7/continuous_eval/classifiers/ensemble.py` & `continuous_eval-0.3.8/continuous_eval/classifiers/ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,53 +7,55 @@
 from sklearn.linear_model import LogisticRegression
 from sklearn.model_selection import GridSearchCV
 
 from continuous_eval.datatypes import XYData
 from continuous_eval.utils.telemetry import telemetry
 
 
+def _default_regressor(X: pd.DataFrame, y: pd.Series):
+    classifier = LogisticRegression()
+    parameters = {
+        "penalty": ["l1", "l2"],
+        "C": [0.1, 1, 10],
+        "solver": ["liblinear"],
+    }
+    clf = GridSearchCV(classifier, parameters)
+    clf.fit(X, y)
+    return clf
+
+
 class EnsembleMetric:
     def __init__(
         self,
         training: XYData,
         calibration: XYData,
         alpha: float = 0.1,
         random_state: Optional[int] = None,
+        predictor_factory: Callable = _default_regressor,
     ) -> None:
         telemetry.log_metric_call(self.__class__.__name__)
         # fmt: off
         assert alpha > 0.0 and alpha < 1.0, "Alpha must be between 0 and 1"
         assert isinstance(training, XYData), "Training data must be an XYData object"
         assert isinstance(calibration, XYData), "Calibration data must be an XYData object"
         assert (len(training.X.columns) > 0) and (len(training) > 0), "Training data must not be empty"
         assert (len(calibration.X.columns) > 0) and (len(calibration) > 0), "Calibration data must not be empty"
         assert (set(training.X.columns) == set(calibration.X.columns)), "Training and calibration data must have the same features"
         # fmt: on
         self.features = training.X.columns
-        self._regressor = self._make_regressor(training.X, training.y)
+        self._regressor = predictor_factory(training.X, training.y)
         self._alpha = alpha
         self._classifier = MapieClassifier(
             estimator=self._regressor,  # type: ignore
             cv="prefit",
             method="lac",
             random_state=random_state,
         )
         self._classifier.fit(calibration.X, calibration.y)
 
-    def _make_regressor(self, X: pd.DataFrame, y: pd.Series):
-        classifier = LogisticRegression()
-        parameters = {
-            "penalty": ["l1", "l2"],
-            "C": [0.1, 1, 10],
-            "solver": ["liblinear"],
-        }
-        clf = GridSearchCV(classifier, parameters)
-        clf.fit(X, y)
-        return clf
-
     def predict(
         self, X: pd.DataFrame, judicator: Optional[Callable] = None, quiet=False
     ) -> Tuple[np.ndarray, np.ndarray]:
         assert isinstance(X, pd.DataFrame), "X must be a pandas DataFrame"
         y_pred, y_set = self._classifier.predict(X, alpha=self._alpha)
         if judicator is None:
             return y_pred, y_set
```

### Comparing `continuous_eval-0.3.7/continuous_eval/classifiers/utils.py` & `continuous_eval-0.3.8/continuous_eval/classifiers/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/data_downloader.py` & `continuous_eval-0.3.8/continuous_eval/data_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
             force_download=force_download,
         )
         return file
     elif res["type"] == "txt":
         out_dir = destination_dir / resource
         return _download_and_extract_zip(EXAMPLES_DATA_URL + res["filename"], out_dir, force_download=force_download)
     elif res["type"] == "chromadb":
-        from langchain.embeddings.openai import OpenAIEmbeddings
-        from langchain.vectorstores import Chroma
+        from langchain_chroma import Chroma
+        from langchain_openai import OpenAIEmbeddings
 
         out_dir = destination_dir / resource
         _download_and_extract_zip(EXAMPLES_DATA_URL + res["filename"], out_dir, force_download=force_download)
         return Chroma(
             persist_directory=str(out_dir),
             embedding_function=OpenAIEmbeddings(),
         )
```

### Comparing `continuous_eval-0.3.7/continuous_eval/datatypes.py` & `continuous_eval-0.3.8/continuous_eval/datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,14 @@
     def __new__(cls, X, y):
         if not isinstance(X, pd.DataFrame):
             raise TypeError("X must be a pandas DataFrame")
         if not isinstance(y, np.ndarray):
             raise TypeError("y must be a numpy ndarray")
         if len(X) != len(y):
             raise ValueError("X and y must have the same number of rows")
-        if len(X.columns) < 1:
-            raise ValueError("X must not be empty")
         if len(y.shape) != 1:
             raise ValueError("y must be a 1-dimensional array")
         return super().__new__(cls, (X, y))
 
     def __len__(self) -> int:
         return len(self.X)
 
@@ -45,16 +43,16 @@
 
 
 class DataSplit:
     def __init__(
         self,
         X: pd.DataFrame,
         y: Union[np.ndarray, pd.Series, Iterable],
-        features: List[str],
         split_ratios: SplitRatios,
+        features: Optional[List[str]] = None,
         oversample: bool = False,
         random_state: Optional[int] = None,
     ):
         if isinstance(y, Iterable):
             y = np.array(list(y))
         elif isinstance(y, pd.Series):
             y = y.to_numpy()
@@ -62,14 +60,17 @@
         assert isinstance(X, pd.DataFrame), "X must be a pandas DataFrame"
         assert isinstance(y, np.ndarray), "y must be a numpy ndarray"
         assert len(X) == len(y), "X and y must have the same number of rows"
         assert len(X.columns) > 0, "X must not be empty"
         assert len(y.shape) == 1, "y must be a 1-dimensional array"
 
         self.features = features
+        if self.features is None:
+            # If no features are provided, assume all numeric columns are features
+            self.features = X.select_dtypes(include=np.number).columns.tolist()
 
         # Split the data into training, testing and calibration sets
         X_temp, X_test, y_temp, y_test = train_test_split(X, y, test_size=split_ratios.test, random_state=random_state)
         X_train, X_cal, y_train, y_cal = train_test_split(
             X_temp,
             y_temp,
             test_size=split_ratios.calibration / (1 - split_ratios.test),
```

### Comparing `continuous_eval-0.3.7/continuous_eval/eval/dataset.py` & `continuous_eval-0.3.8/continuous_eval/eval/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import typing
 from dataclasses import dataclass
 from pathlib import Path
 
 import yaml
 
-from continuous_eval.eval.types import UUID, ToolCall
+from continuous_eval.eval.types import UID, ToolCall
 from continuous_eval.eval.utils import type_hint_to_str
 
 _SAFE_DICT = {k: v for k, v in typing.__dict__.items() if not k.startswith("__")}
-_SAFE_DICT["UUID"] = UUID
+_SAFE_DICT["UID"] = UID
 _SAFE_DICT["ToolCall"] = ToolCall
 
 
 @dataclass(frozen=True)
 class DatasetField:
     name: str
     type: type = typing.Any  # type: ignore
@@ -179,7 +179,22 @@
 
     def __len__(self):
         return len(self._data)
 
     def filter(self, fcn: typing.Callable):
         self._data = [x for x in self._data if fcn(x)]
         return self
+
+    def sample(self, size: typing.Union[float, int]):
+        import random
+
+        if size > 1 and isinstance(size, int):
+            assert size <= len(self._data), f"Sample size {size} is larger than the dataset size {len(self._data)}"
+            k = size
+        elif size > 0 and size < 1 and isinstance(size, float):
+            k = int(len(self._data) * size)
+        else:
+            raise ValueError(f"Invalid sample size {size}")
+        idx = random.choices(range(len(self._data)), k=k)
+        idx = sorted(idx)
+        self._data = [self._data[i] for i in idx]
+        return self
```

### Comparing `continuous_eval-0.3.7/continuous_eval/eval/modules.py` & `continuous_eval-0.3.8/continuous_eval/eval/modules.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 from continuous_eval.eval.dataset import DatasetField
 from continuous_eval.eval.tests import Test
 from continuous_eval.metrics import Metric
 
 
 @dataclass(frozen=True, eq=True)
```

### Comparing `continuous_eval-0.3.7/continuous_eval/eval/pipeline.py` & `continuous_eval-0.3.8/continuous_eval/eval/pipeline.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/eval/result_types.py` & `continuous_eval-0.3.8/continuous_eval/eval/result_types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 import json
 from collections import ChainMap
+from copy import deepcopy
 from functools import cached_property, lru_cache
 from pathlib import Path
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
+from continuous_eval.eval.dataset import Dataset
 from continuous_eval.eval.modules import AgentModule
 from continuous_eval.eval.pipeline import Pipeline
 from continuous_eval.eval.utils import instantiate_type
 
 TOOL_PREFIX = "_tool__"
 
 
-class EvaluationResults:
-    def __init__(self, pipeline: Optional[Pipeline] = None) -> None:
-        if pipeline is None:
-            self.results: List[Dict] = list()
-        else:
-            num_samples = len(pipeline.dataset.data)
-            self.results: List[Dict] = [self._build_empty_samples(pipeline) for _ in range(num_samples)]
+class PipelineResults:
+    def __init__(self) -> None:
+        self.results: List[Dict] = list()
+
+    @classmethod
+    def from_dataset(cls, dataset: Dataset):
+        eval_results = cls()
+        eval_results.results = dataset.data
+        return eval_results
+
+    @classmethod
+    def from_logs(cls, logs):
+        eval_results = cls()
+        for datum in logs.pipeline.dataset.data:
+            if datum["uid"] not in logs.data:
+                continue
+            eval_results.results.append({**datum, **logs.data[datum["uid"]]})
+        assert len(eval_results) == len(logs.data), "Could not find some uid in the dataset"
+        return eval_results
+
+    def initialize(self, pipeline: Pipeline):
+        num_samples = len(pipeline.dataset.data)
+        self.results: List[Dict] = [self._build_empty_samples(pipeline) for _ in range(num_samples)]
 
     def __len__(self):
         return len(self.results)
 
     def is_empty(self) -> bool:
         return not bool(self.results)
 
@@ -46,63 +64,86 @@
     def load(self, filepath: Path):
         assert filepath.suffix == ".jsonl", "File must be a JSONL file"
         with open(filepath, "r") as f:
             self.results = [json.loads(line) for line in f]
 
 
 class MetricsResults:
-    def __init__(self) -> None:
-        self.pipeline: Optional[Pipeline] = None
-        self.samples: Dict = dict()
+    def __init__(self, pipeline: Optional[Pipeline]) -> None:
+        self.pipeline = pipeline
+        self.samples = dict()
 
     def is_empty(self) -> bool:
         return not bool(self.samples)
 
     @cached_property
     def results(self) -> Dict:
+        """
+        Returns a dictionary containing the evaluation results for each module.
+
+        The dictionary is structured as follows:
+        - The keys are the names of the modules.
+        - The values are lists of dictionaries, where each dictionary represents a result.
+        """
         return {
             module_name: [dict(ChainMap(*x)) for x in zip(*eval_res.values())]
             for module_name, eval_res in self.samples.items()
         }
 
     def to_pandas(self):
+        """
+        Converts the results to a pandas DataFrame.
+
+        Returns:
+            pandas.DataFrame: The results as a pandas DataFrame.
+        """
         import pandas as pd
 
         if len(self.results) > 1:
             flatten = [
                 {f"{outer_key}_{key}": value for key, value in inner_dict.items()}
                 for outer_key, dict_list in self.results.items()
                 for inner_dict in dict_list
             ]
         else:
             flatten = list(*self.results.values())
         return pd.DataFrame(flatten)
 
     @lru_cache(maxsize=1)
     def aggregate(self):
+        """
+        Aggregates the metric values for each module and metric name in the samples.
+
+        Returns:
+            dict: A dictionary containing the aggregated metric values for each module and metric name.
+        """
         if self.pipeline is None:
             raise ValueError("Pipeline not set")
         aggregated_samples = dict()
         for module_name, metrics_results in self.samples.items():
             aggregated_samples[module_name] = dict()
             for metric_name, metric_values in metrics_results.items():
                 metric = self.pipeline.get_metric(module_name, metric_name)
                 aggregated_samples[module_name][metric_name] = metric.aggregate(metric_values)
         actual_results = {
             module_name: dict(ChainMap(*metrics.values())) for module_name, metrics in aggregated_samples.items()
         }
         return actual_results
 
-    def save(self, filepath: Path):
+    def save(self, filepath: Union[str, Path]):
+        if isinstance(filepath, str):
+            filepath = Path(filepath)
         assert filepath.suffix == ".json", "File must be a JSON file"
         assert self.samples, "No samples to save"
         with open(filepath, "w") as f:
             json.dump(self.samples, f, ensure_ascii=False)
 
-    def load(self, filepath: Path):
+    def load(self, filepath: Union[str, Path]):
+        if isinstance(filepath, str):
+            filepath = Path(filepath)
         assert filepath.suffix == ".json", "File must be a JSON file"
         with open(filepath, "r") as f:
             self.samples = json.load(f)
         return self
 
 
 class TestResults:
```

### Comparing `continuous_eval-0.3.7/continuous_eval/eval/tests.py` & `continuous_eval-0.3.8/continuous_eval/eval/tests.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/eval/utils.py` & `continuous_eval-0.3.8/continuous_eval/eval/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/generators/simple.py` & `continuous_eval-0.3.8/continuous_eval/generators/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import itertools
 import logging
 import random
 
 import numpy as np
-from langchain.vectorstores import VectorStore
+from langchain_community.vectorstores import VectorStore
 from tqdm import tqdm
 
 from continuous_eval.llm_factory import LLMFactory, LLMInterface
 from continuous_eval.utils.telemetry import telemetry
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(level=logging.WARNING)
 
-
 COMMON_RULES = """
 The user is unaware of any specific context, so make sure the question makes sense to those who are not aware of the context.
 Avoid phrases like "According to context / given provided context..."
 Avoid questions that uses references references like he / she / you / they.
 Make sure the context has enough information to provide a full answer to the question.
 If the context is not enough to generate a reasonable question, respond with exactly "Generation Error".
 """
@@ -272,11 +271,13 @@
             except Exception as e:
                 print(f"Error: {e}")
                 num_single_hop_tries += 1
                 continue
 
         pbar.close()
         dataset = single_hop_questions + multi_hop_questions
+        for idx, d in enumerate(dataset):
+            d["uid"] = idx
         if len(dataset) < num_questions:
             raise Warning(f"Could not generate enough questions. Generated {len(dataset)} questions.")
 
         return dataset
```

### Comparing `continuous_eval-0.3.7/continuous_eval/llm_factory.py` & `continuous_eval-0.3.8/continuous_eval/llm_factory.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/llms/bedrock.py` & `continuous_eval-0.3.8/continuous_eval/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/_utils/simple_tokenizer.py` & `continuous_eval-0.3.8/continuous_eval/metrics/_utils/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/base.py` & `continuous_eval-0.3.8/continuous_eval/metrics/base.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/classification/classification.py` & `continuous_eval-0.3.8/continuous_eval/metrics/classification/classification.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/code/python/code_deterministic_metrics.py` & `continuous_eval-0.3.8/continuous_eval/metrics/code/python/code_deterministic_metrics.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/__init__.py` & `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/__init__.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/bert.py` & `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/bert.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     raise ImportError("To use BertSimilarity, please install sentence-transformers and transformers.")
 from continuous_eval.metrics.base import Metric
 
 
 class DebertaScores:
     def __init__(self):
         self._model = CrossEncoder("cross-encoder/nli-deberta-v3-large")
-        self._batch_size = 8
+        self._batch_size = 32
 
     @property
     def device(self):
         return self._model._target_device
 
     def _batch_predict(self, sentence_pairs, batch_size):
         """
@@ -42,16 +42,33 @@
 class BertSimilarity(Metric):
     def __init__(self, pooler_output: bool = False):
         super().__init__()
         # Load pre-trained BERT model and tokenizer
         self._tokenizer = BertTokenizer.from_pretrained("bert-base-uncased")
         self._model = BertModel.from_pretrained("bert-base-uncased")
         self._pooler_output = pooler_output
+        self.batch_size = 32
 
     def batch(self, prediction: List[str], reference: List[str]):
+        # Function to yield batches of data
+        def mini_batches(data, batch_size):
+            for i in range(0, len(data), batch_size):
+                yield data[i : i + batch_size]
+
+        # Process batches
+        all_similarities = []
+        for pred_batch, ref_batch in zip(
+            mini_batches(prediction, self.batch_size),
+            mini_batches(reference, self.batch_size),
+        ):
+            batch_result = self._subprocess(pred_batch, ref_batch)
+            all_similarities.extend(batch_result)
+        return {"bert_similarity": all_similarities}
+
+    def _subprocess(self, prediction: List[str], reference: List[str]):
         predictions = self._tokenizer(prediction, padding=True)
         references = self._tokenizer(reference, padding=True)
 
         # Get BERT embeddings for the tokens
         with torch.no_grad():
             pred_embedding = self._model(  # type: ignore
                 torch.tensor(predictions["input_ids"]),
@@ -67,12 +84,12 @@
             else:
                 pred_embedding = pred_embedding[0].mean(dim=1)
                 ref_embedding = ref_embedding[0].mean(dim=1)
 
         cosine_similarity = torch.nn.CosineSimilarity(dim=0)
         semantic_similarity = cosine_similarity(pred_embedding.T, ref_embedding.T)
         semantic_similarity = torch.clip(semantic_similarity, min=0.0, max=1.0)
-        return {"bert_similarity": semantic_similarity.tolist()}
+        return semantic_similarity.tolist()
 
     def __call__(self, prediction: str, reference: str):
         res = self.batch(prediction=[prediction], reference=[reference])
         return {"bert_similarity": res["bert_similarity"][0]}
```

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/custom.py` & `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/custom.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 @dataclass
 class EvaluationExample:
     input: Union[str, Dict[str, Any]]
     score: Any
     justification: Optional[str] = ""
 
     def __str__(self):
-        in_str = self.input if isinstance(self.input, str) else "\n".join([f"{k}: {v}" for k, v in self.input.items()])
+        in_str = (
+            self.input
+            if isinstance(self.input, str)
+            else "\n".join([f"{k.replace('_', ' ')}: {v}" for k, v in self.input.items()])
+        )
         just_str = f"\nJustification: {self.justification}" if self.justification else ""
         return f"Input: {in_str}\nScore: {self.score}{just_str}"
 
     def todict(self):
         return {k: str(v) for k, v in asdict(self).items()}
```

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/deterministic.py` & `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/deterministic.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/llm_based.py` & `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/llm_based.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/semantic.py` & `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/semantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         return [{"bert_answer_similarity": x} for x in ret["bert_answer_similarity"]]
 
 
 class DebertaAnswerScores(Metric):
     def __init__(self, reverse: bool = False):
         super().__init__()
         self.reverse = reverse
+        self.batch_size = 32
 
     def _ret_keys(self):
         reverse = "reverse_" if self.reverse else ""
         entailment_key = f"deberta_{reverse}answer_entailment"
         contradiction_key = f"deberta_{reverse}answer_contradiction"
         return entailment_key, contradiction_key
```

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/utils.py` & `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/retrieval/llm_based.py` & `continuous_eval-0.3.8/continuous_eval/metrics/retrieval/llm_based.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/retrieval/matching_strategy.py` & `continuous_eval-0.3.8/continuous_eval/metrics/retrieval/matching_strategy.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/retrieval/precision_recall_f1.py` & `continuous_eval-0.3.8/continuous_eval/metrics/retrieval/precision_recall_f1.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/retrieval/ranked.py` & `continuous_eval-0.3.8/continuous_eval/metrics/retrieval/ranked.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/continuous_eval/metrics/tools/match.py` & `continuous_eval-0.3.8/continuous_eval/metrics/tools/match.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,19 +17,27 @@
                 for i, tool in enumerate(tools)
                 if i < len(ground_truths)
                 and tool["name"] == ground_truths[i]["name"]
                 and tool["kwargs"] == ground_truths[i]["kwargs"]
             )
         else:
             # Convert ground_truth to a format that's easy to check for "contains"
-            ground_truth_set = {
-                frozenset(tool.items()) for tool in [{"name": tool["name"], **tool["kwargs"]} for tool in ground_truths]
-            }
+            use_kwargs = all("kwargs" in tool for tool in ground_truths)
+            if use_kwargs:
+                ground_truth_set = {
+                    frozenset(tool.items())
+                    for tool in [{"name": tool["name"], **tool["kwargs"]} for tool in ground_truths]
+                }
+            else:
+                ground_truth_set = {frozenset(tool.items()) for tool in ground_truths}
             # Score
             num_correct, matched_executions = 0, set()
             for tool in tools:
-                tool_set = frozenset({"name": tool["name"], **tool["kwargs"]}.items())
+                if use_kwargs:
+                    tool_set = frozenset({"name": tool["name"], **tool["kwargs"]}.items())
+                else:
+                    tool_set = frozenset({"name": tool["name"]}.items())
                 if tool_set in ground_truth_set and tool_set not in matched_executions:
                     num_correct += 1
                 matched_executions.add(tool_set)
 
         return {"num_correct": num_correct, "score": num_correct / len(ground_truths)}
```

### Comparing `continuous_eval-0.3.7/continuous_eval/utils/telemetry.py` & `continuous_eval-0.3.8/continuous_eval/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.7/pyproject.toml` & `continuous_eval-0.3.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,69 @@
 [tool.poetry]
 name = "continuous-eval"
-version = "0.3.7"
+version = "0.3.8"
 description = "Open-Source Evaluation for GenAI Application Pipelines."
 authors = ["Yi Zhang <yi@relari.ai>", "Pasquale Antonante <pasquale@relari.ai>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "continuous_eval"}]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4.0"
+python = ">=3.9,<3.12"
 python-dotenv = "^1.0.0"
 nltk = "^3.8.1"
 rouge = "^1.0.1"
 openai = "^1.3.7"
-transformers = {version = "^4.35.2", optional = true}
-sentence-transformers = {version = "^2.2.2", optional = true}
-torch = {version = "^2.1.1", optional = true}
-anthropic = {version = "^0.7.7", optional = true}
-google-generativeai = {version = "^0.3.1", optional = true}
 mapie = "^0.7.0"
 imbalanced-learn = "^0.11.0"
 pandas = "^2.1.4"
 protobuf = "^4.23.4"
 tqdm = "^4.66.1"
 requests = "^2.31.0"
-pinecone-client = {version = "^2.2.4", optional = true}
-chromadb = {version = "^0.4.21", optional = true}
-tiktoken = {version = "^0.5.2", optional = true}
-unstructured = {version = "^0.11.6", optional = true}
+pyyaml = "^6.0.1"
 appdirs = "^1.4.4"
 munkres = "^1.1.4"
 thefuzz = "^0.22.1"
 sentencepiece = "^0.2.0"
-cohere = {version = "^4.54", optional = true}
 tenacity = "^8.2.3"
-boto3 = {version = "^1.34.70", optional = true}
+
 langchain-community = {version = "^0.0.29", optional = true}
-pyyaml = "^6.0.1"
+cohere = {version = "^4.54", optional = true}
+boto3 = {version = "^1.34.70", optional = true}
+google-generativeai = {version = "^0.3.1", optional = true}
+anthropic = {version = "^0.7.7", optional = true}
+
+[tool.poetry.group.semantic]
+optional = true
+[tool.poetry.group.semantic.dependencies]
+torch = "^2.1.1"
+transformers = "^4.35.2"
+sentence-transformers = "^2.2.2"
+
+[tool.poetry.group.generators]
+optional = true
+[tool.poetry.group.generators.dependencies]
+unstructured ="^0.13.7"
+tiktoken = "^0.7.0"
+chromadb = "^0.5.0"
+langchain-openai = "^0.1.7"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.11.0"
+isort = "^5.12.0"
+pytest = "^7.4.3"
+pre-commit = "^3.6.0"
 
 [tool.poetry.extras]
 langchain = ["langchain-community"]
-semantic = ["transformers", "sentence-transformers", "torch"]
 anthropic = ["anthropic"]
 bedrock = ["boto3"]
 gemini = ["google-generativeai"]
 cohere = ["cohere"]
-generators = ["unstructured", "tiktoken", "pinecone-client", "chromadb", "langchain-community"]
 
-[tool.poetry.group.dev.dependencies]
-black = "^23.11.0"
-isort = "^5.12.0"
-pytest = "^7.4.3"
-pre-commit = "^3.6.0"
 
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `continuous_eval-0.3.7/PKG-INFO` & `continuous_eval-0.3.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,46 @@
 Metadata-Version: 2.1
 Name: continuous-eval
-Version: 0.3.7
+Version: 0.3.8
 Summary: Open-Source Evaluation for GenAI Application Pipelines.
 License: Apache-2.0
 Author: Yi Zhang
 Author-email: yi@relari.ai
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: anthropic
 Provides-Extra: bedrock
 Provides-Extra: cohere
 Provides-Extra: gemini
-Provides-Extra: generators
 Provides-Extra: langchain
-Provides-Extra: semantic
 Requires-Dist: anthropic (>=0.7.7,<0.8.0) ; extra == "anthropic"
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: boto3 (>=1.34.70,<2.0.0) ; extra == "bedrock"
-Requires-Dist: chromadb (>=0.4.21,<0.5.0) ; extra == "generators"
 Requires-Dist: cohere (>=4.54,<5.0) ; extra == "cohere"
 Requires-Dist: google-generativeai (>=0.3.1,<0.4.0) ; extra == "gemini"
 Requires-Dist: imbalanced-learn (>=0.11.0,<0.12.0)
-Requires-Dist: langchain-community (>=0.0.29,<0.0.30) ; extra == "langchain" or extra == "generators"
+Requires-Dist: langchain-community (>=0.0.29,<0.0.30) ; extra == "langchain"
 Requires-Dist: mapie (>=0.7.0,<0.8.0)
 Requires-Dist: munkres (>=1.1.4,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=1.3.7,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
-Requires-Dist: pinecone-client (>=2.2.4,<3.0.0) ; extra == "generators"
 Requires-Dist: protobuf (>=4.23.4,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rouge (>=1.0.1,<2.0.0)
-Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "semantic"
 Requires-Dist: sentencepiece (>=0.2.0,<0.3.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: thefuzz (>=0.22.1,<0.23.0)
-Requires-Dist: tiktoken (>=0.5.2,<0.6.0) ; extra == "generators"
-Requires-Dist: torch (>=2.1.1,<3.0.0) ; extra == "semantic"
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
-Requires-Dist: transformers (>=4.35.2,<5.0.0) ; extra == "semantic"
-Requires-Dist: unstructured (>=0.11.6,<0.12.0) ; extra == "generators"
 Description-Content-Type: text/markdown
 
 <h3 align="center">
   <img
     src="docs/public/continuous-eval-logo.png"
     width="350"
   >
@@ -65,15 +55,15 @@
   <a href="https://pypi.python.org/pypi/continuous-eval/">![https://github.com/Naereen/badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)</a>
   <a a href="https://github.com/relari-ai/continuous-eval/blob/main/LICENSE">![https://pypi.python.org/pypi/continuous-eval/](https://img.shields.io/pypi/l/continuous-eval.svg)</a>
 
 
 </div>
 
 <h2 align="center">
-  <p>Open-Source Evaluation for GenAI Application Pipelines</p>
+  <p>Open-Source Evaluation for GenAI Applications</p>
 </h2>
 
 
 
 ## Overview
 
 `continuous-eval` is an open-source package created for granular and holistic evaluation of GenAI application pipelines. 
@@ -190,20 +180,21 @@
         <td>Define your own metrics</td>
     </tr>
 </table>
 
 To define your own metrics, you only need to extend the [Metric](continuous_eval/metrics/base.py#L23C7-L23C13) class implementing the `__call__` method.
 Optional methods are `batch` (if it is possible to implement optimizations for batch processing) and `aggregate` (to aggregate metrics results over multiple samples_).
 
-## Run evaluation on pipeline modules
+## Run evaluation on a pipeline
 
 Define modules in your pipeline and select corresponding metrics.
 
 ```python
-from continuous_eval.eval import Module, ModuleOutput, Pipeline, Dataset
+from continuous_eval.eval import Module, ModuleOutput, Pipeline, Dataset, EvaluationRunner
+from continuous_eval.eval.logger import PipelineLogger
 from continuous_eval.metrics.retrieval import PrecisionRecallF1, RankedRetrievalMetrics
 from continuous_eval.metrics.generation.text import DeterministicAnswerCorrectness
 from typing import List, Dict
 
 dataset = Dataset("dataset_folder")
 
 # Simple 3-step RAG pipeline with Retriever->Reranker->Generation
@@ -246,55 +237,60 @@
 pipeline = Pipeline([retriever, reranker, llm], dataset=dataset)
 print(pipeline.graph_repr()) # optional: visualize the pipeline
 ```
 
 Now you can run the evaluation on your pipeline
 
 ```python
-eval_manager.start_run()
-  while eval_manager.is_running():
-    if eval_manager.curr_sample is None:
-      break
-    q = eval_manager.curr_sample["question"] # get the question or any other field
-    # run your pipeline ...
-    eval_manager.next_sample()
-```
+pipelog = PipelineLogger(pipeline=pipeline)
 
-To **log** the results you just need to call the `eval_manager.log` method with the module name and the output, for example:
+# now run your LLM application pipeline, and for each module, log the results:
+pipelog.log(uid=sample_uid, module="module_name", value=data)
 
-```python
-eval_manager.log("answer_generator", response)
+# Once you finish logging the data, you can use the EvaluationRunner to evaluate the logs
+evalrunner = EvaluationRunner(pipeline)
+metrics = evalrunner.evaluate(pipelog)
+metrics.results() # returns a dictionary with the results
 ```
 
-The evaluator manager also offers
+To run evaluation over an existing dataset (BYODataset), you can run the following:
 
-- `eval_manager.run_metrics()` to run all the metrics defined in the pipeline
-- `eval_manager.run_tests()` to run the tests defined in the pipeline (see the documentation [docs](docs.relari.ai) for more details)
+```python
+dataset = Dataset(...)
+evalrunner = EvaluationRunner(pipeline)
+metrics = evalrunner.evaluate(dataset)
+```
 
 ## Synthetic Data Generation
 
 Ground truth data, or reference data, is important for evaluation as it can offer a comprehensive and consistent measurement of system performance. However, it is often costly and time-consuming to manually curate such a golden dataset.
 We have created a synthetic data pipeline that can custom generate user interaction data for a variety of use cases such as RAG, agents, copilots. They can serve a starting point for a golden dataset for evaluation or for other training purposes. Below is an example for Coding Agents. Try out this demo: [Synthetic Data Demo](https://www.relari.ai/synthetic-data-demo)
 
 <h1 align="center">
   <img
     src="docs/public/synthetic-data-demo.png"
   >
 </h1>
 
+## 💡 Contributing
+
+Interested in contributing? Contributions to LlamaIndex core as well as contributing
+integrations that build on the core are both accepted and highly encouraged! See our [Contribution Guide](CONTRIBUTING.md) for more details.
 
 ## Resources
 
 - **Docs:** [link](https://docs.relari.ai/)
 - **Examples Repo**: [end-to-end example repo](https://github.com/relari-ai/examples)
 - **Blog Posts:**
   - Practical Guide to RAG Pipeline Evaluation: [Part 1: Retrieval](https://medium.com/relari/a-practical-guide-to-rag-pipeline-evaluation-part-1-27a472b09893), [Part 2: Generation](https://medium.com/relari/a-practical-guide-to-rag-evaluation-part-2-generation-c79b1bde0f5d)
   - How important is a Golden Dataset for LLM evaluation?
  [(link)](https://medium.com/relari/how-important-is-a-golden-dataset-for-llm-pipeline-evaluation-4ef6deb14dc5)
   - How to evaluate complex GenAI Apps: a granular approach [(link)](https://medium.com/relari/how-to-evaluate-complex-genai-apps-a-granular-approach-0ab929d5b3e2)
+  - How to Make the Most Out of LLM Production Data: Simulated User Feedback [(link)](https://medium.com/towards-data-science/how-to-make-the-most-out-of-llm-production-data-simulated-user-feedback-843c444febc7)
+  - Generate Synthetic Data to Test LLM Applications [(link)](https://medium.com/relari/generate-synthetic-data-to-test-llm-applications-4bffeb51b80e)
 - **Discord:** Join our community of LLM developers [Discord](https://discord.gg/GJnM8SRsHr)
 - **Reach out to founders:** [Email](mailto:founders@relari.ai) or [Schedule a chat](https://cal.com/pasquale/continuous-eval)
 
 ## License
 
 This project is licensed under the Apache 2.0 - see the [LICENSE](LICENSE) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,47 +1,38 @@
-Metadata-Version: 2.1 Name: continuous-eval Version: 0.3.7 Summary: Open-Source
+Metadata-Version: 2.1 Name: continuous-eval Version: 0.3.8 Summary: Open-Source
 Evaluation for GenAI Application Pipelines. License: Apache-2.0 Author: Yi
-Zhang Author-email: yi@relari.ai Requires-Python: >=3.9,<4.0 Classifier:
+Zhang Author-email: yi@relari.ai Requires-Python: >=3.9,<3.12 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: anthropic Provides-Extra: bedrock Provides-Extra: cohere
-Provides-Extra: gemini Provides-Extra: generators Provides-Extra: langchain
-Provides-Extra: semantic Requires-Dist: anthropic (>=0.7.7,<0.8.0) ; extra ==
-"anthropic" Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-Dist: boto3
-(>=1.34.70,<2.0.0) ; extra == "bedrock" Requires-Dist: chromadb
-(>=0.4.21,<0.5.0) ; extra == "generators" Requires-Dist: cohere (>=4.54,<5.0) ;
-extra == "cohere" Requires-Dist: google-generativeai (>=0.3.1,<0.4.0) ; extra
-== "gemini" Requires-Dist: imbalanced-learn (>=0.11.0,<0.12.0) Requires-Dist:
-langchain-community (>=0.0.29,<0.0.30) ; extra == "langchain" or extra ==
-"generators" Requires-Dist: mapie (>=0.7.0,<0.8.0) Requires-Dist: munkres
-(>=1.1.4,<2.0.0) Requires-Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist: openai
-(>=1.3.7,<2.0.0) Requires-Dist: pandas (>=2.1.4,<3.0.0) Requires-Dist:
-pinecone-client (>=2.2.4,<3.0.0) ; extra == "generators" Requires-Dist:
-protobuf (>=4.23.4,<5.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: requests
+Language :: Python :: 3.11 Provides-Extra: anthropic Provides-Extra: bedrock
+Provides-Extra: cohere Provides-Extra: gemini Provides-Extra: langchain
+Requires-Dist: anthropic (>=0.7.7,<0.8.0) ; extra == "anthropic" Requires-Dist:
+appdirs (>=1.4.4,<2.0.0) Requires-Dist: boto3 (>=1.34.70,<2.0.0) ; extra ==
+"bedrock" Requires-Dist: cohere (>=4.54,<5.0) ; extra == "cohere" Requires-
+Dist: google-generativeai (>=0.3.1,<0.4.0) ; extra == "gemini" Requires-Dist:
+imbalanced-learn (>=0.11.0,<0.12.0) Requires-Dist: langchain-community
+(>=0.0.29,<0.0.30) ; extra == "langchain" Requires-Dist: mapie (>=0.7.0,<0.8.0)
+Requires-Dist: munkres (>=1.1.4,<2.0.0) Requires-Dist: nltk (>=3.8.1,<4.0.0)
+Requires-Dist: openai (>=1.3.7,<2.0.0) Requires-Dist: pandas (>=2.1.4,<3.0.0)
+Requires-Dist: protobuf (>=4.23.4,<5.0.0) Requires-Dist: python-dotenv
+(>=1.0.0,<2.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: requests
 (>=2.31.0,<3.0.0) Requires-Dist: rouge (>=1.0.1,<2.0.0) Requires-Dist:
-sentence-transformers (>=2.2.2,<3.0.0) ; extra == "semantic" Requires-Dist:
 sentencepiece (>=0.2.0,<0.3.0) Requires-Dist: tenacity (>=8.2.3,<9.0.0)
-Requires-Dist: thefuzz (>=0.22.1,<0.23.0) Requires-Dist: tiktoken
-(>=0.5.2,<0.6.0) ; extra == "generators" Requires-Dist: torch (>=2.1.1,<3.0.0)
-; extra == "semantic" Requires-Dist: tqdm (>=4.66.1,<5.0.0) Requires-Dist:
-transformers (>=4.35.2,<5.0.0) ; extra == "semantic" Requires-Dist:
-unstructured (>=0.11.6,<0.12.0) ; extra == "generators" Description-Content-
-Type: text/markdown
+Requires-Dist: thefuzz (>=0.22.1,<0.23.0) Requires-Dist: tqdm (>=4.66.1,<5.0.0)
+Description-Content-Type: text/markdown
                ******** [[ddooccss//ppuubblliicc//ccoonnttiinnuuoouuss--eevvaall--llooggoo..ppnngg]] ********
    _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_!_[_h_t_t_p_s_:_/_/_p_y_p_i_._p_y_t_h_o_n_._o_r_g_/_p_y_p_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_/_]_(_h_t_t_p_s_:_/_/
    _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_._s_v_g_) _!_[_h_t_t_p_s_:_/_/_G_i_t_H_u_b_._c_o_m_/
   _r_e_l_a_r_i_-_a_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_/_r_e_l_e_a_s_e_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/
    _r_e_l_a_r_i_-_a_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_) _!_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_N_a_e_r_e_e_n_/_b_a_d_g_e_s_/_]_(_h_t_t_p_s_:_/_/
    _b_a_d_g_e_n_._n_e_t_/_b_a_d_g_e_/_O_p_e_n_%_2_0_S_o_u_r_c_e_%_2_0_%_3_F_/_Y_e_s_%_2_1_/_b_l_u_e_?_i_c_o_n_=_g_i_t_h_u_b_) ![https://
      pypi.python.org/pypi/continuous-eval/](https://img.shields.io/pypi/l/
                              continuous-eval.svg)
-      ********** OOppeenn--SSoouurrccee EEvvaalluuaattiioonn ffoorr GGeennAAII AApppplliiccaattiioonn PPiippeelliinneess **********
+           ********** OOppeenn--SSoouurrccee EEvvaalluuaattiioonn ffoorr GGeennAAII AApppplliiccaattiioonnss **********
 ## Overview `continuous-eval` is an open-source package created for granular
 and holistic evaluation of GenAI application pipelines.
                ************ [[ddooccss//ppuubblliicc//mmoodduullee--lleevveell--eevvaall..ppnngg]] ************
 ## How is continuous-eval different? - **Modularized Evaluation**: Measure each
 module in the pipeline with tailored metrics. - **Comprehensive Metric
 Library**: Covers Retrieval-Augmented Generation (RAG), Code Generation, Agent
 Tool Use, Classification and a variety of other LLM use cases. Mix and match
@@ -77,17 +68,18 @@
                 LLM-based     LLMBasedCodeGeneration
 Agent Tools     Deterministic ToolSelectionAccuracy
 Custom                        Define your own metrics
 To define your own metrics, you only need to extend the [Metric]
 (continuous_eval/metrics/base.py#L23C7-L23C13) class implementing the
 `__call__` method. Optional methods are `batch` (if it is possible to implement
 optimizations for batch processing) and `aggregate` (to aggregate metrics
-results over multiple samples_). ## Run evaluation on pipeline modules Define
-modules in your pipeline and select corresponding metrics. ```python from
-continuous_eval.eval import Module, ModuleOutput, Pipeline, Dataset from
+results over multiple samples_). ## Run evaluation on a pipeline Define modules
+in your pipeline and select corresponding metrics. ```python from
+continuous_eval.eval import Module, ModuleOutput, Pipeline, Dataset,
+EvaluationRunner from continuous_eval.eval.logger import PipelineLogger from
 continuous_eval.metrics.retrieval import PrecisionRecallF1,
 RankedRetrievalMetrics from continuous_eval.metrics.generation.text import
 DeterministicAnswerCorrectness from typing import List, Dict dataset = Dataset
 ("dataset_folder") # Simple 3-step RAG pipeline with Retriever->Reranker-
 >Generation retriever = Module( name="Retriever", input=dataset.question,
 output=List[str], eval=[ PrecisionRecallF1().use
 ( retrieved_context=ModuleOutput(),
@@ -97,44 +89,51 @@
 ground_truth_context=dataset.ground_truth_context, ), ], ) llm = Module
 ( name="answer_generator", input=reranker, output=str, eval=
 [ FleschKincaidReadability().use(answer=ModuleOutput()),
 DeterministicAnswerCorrectness().use( answer=ModuleOutput(),
 ground_truth_answers=dataset.ground_truths ), ], ) pipeline = Pipeline(
 [retriever, reranker, llm], dataset=dataset) print(pipeline.graph_repr()) #
 optional: visualize the pipeline ``` Now you can run the evaluation on your
-pipeline ```python eval_manager.start_run() while eval_manager.is_running(): if
-eval_manager.curr_sample is None: break q = eval_manager.curr_sample
-["question"] # get the question or any other field # run your pipeline ...
-eval_manager.next_sample() ``` To **log** the results you just need to call the
-`eval_manager.log` method with the module name and the output, for example:
-```python eval_manager.log("answer_generator", response) ``` The evaluator
-manager also offers - `eval_manager.run_metrics()` to run all the metrics
-defined in the pipeline - `eval_manager.run_tests()` to run the tests defined
-in the pipeline (see the documentation [docs](docs.relari.ai) for more details)
-## Synthetic Data Generation Ground truth data, or reference data, is important
-for evaluation as it can offer a comprehensive and consistent measurement of
-system performance. However, it is often costly and time-consuming to manually
-curate such a golden dataset. We have created a synthetic data pipeline that
-can custom generate user interaction data for a variety of use cases such as
-RAG, agents, copilots. They can serve a starting point for a golden dataset for
-evaluation or for other training purposes. Below is an example for Coding
-Agents. Try out this demo: [Synthetic Data Demo](https://www.relari.ai/
-synthetic-data-demo)
+pipeline ```python pipelog = PipelineLogger(pipeline=pipeline) # now run your
+LLM application pipeline, and for each module, log the results: pipelog.log
+(uid=sample_uid, module="module_name", value=data) # Once you finish logging
+the data, you can use the EvaluationRunner to evaluate the logs evalrunner =
+EvaluationRunner(pipeline) metrics = evalrunner.evaluate(pipelog)
+metrics.results() # returns a dictionary with the results ``` To run evaluation
+over an existing dataset (BYODataset), you can run the following: ```python
+dataset = Dataset(...) evalrunner = EvaluationRunner(pipeline) metrics =
+evalrunner.evaluate(dataset) ``` ## Synthetic Data Generation Ground truth
+data, or reference data, is important for evaluation as it can offer a
+comprehensive and consistent measurement of system performance. However, it is
+often costly and time-consuming to manually curate such a golden dataset. We
+have created a synthetic data pipeline that can custom generate user
+interaction data for a variety of use cases such as RAG, agents, copilots. They
+can serve a starting point for a golden dataset for evaluation or for other
+training purposes. Below is an example for Coding Agents. Try out this demo:
+[Synthetic Data Demo](https://www.relari.ai/synthetic-data-demo)
               ************ [[ddooccss//ppuubblliicc//ssyynntthheettiicc--ddaattaa--ddeemmoo..ppnngg]] ************
-## Resources - **Docs:** [link](https://docs.relari.ai/) - **Examples Repo**:
-[end-to-end example repo](https://github.com/relari-ai/examples) - **Blog
-Posts:** - Practical Guide to RAG Pipeline Evaluation: [Part 1: Retrieval]
-(https://medium.com/relari/a-practical-guide-to-rag-pipeline-evaluation-part-1-
-27a472b09893), [Part 2: Generation](https://medium.com/relari/a-practical-
-guide-to-rag-evaluation-part-2-generation-c79b1bde0f5d) - How important is a
-Golden Dataset for LLM evaluation? [(link)](https://medium.com/relari/how-
-important-is-a-golden-dataset-for-llm-pipeline-evaluation-4ef6deb14dc5) - How
-to evaluate complex GenAI Apps: a granular approach [(link)](https://
-medium.com/relari/how-to-evaluate-complex-genai-apps-a-granular-approach-
-0ab929d5b3e2) - **Discord:** Join our community of LLM developers [Discord]
+## ð¡ Contributing Interested in contributing? Contributions to LlamaIndex
+core as well as contributing integrations that build on the core are both
+accepted and highly encouraged! See our [Contribution Guide](CONTRIBUTING.md)
+for more details. ## Resources - **Docs:** [link](https://docs.relari.ai/) -
+**Examples Repo**: [end-to-end example repo](https://github.com/relari-ai/
+examples) - **Blog Posts:** - Practical Guide to RAG Pipeline Evaluation: [Part
+1: Retrieval](https://medium.com/relari/a-practical-guide-to-rag-pipeline-
+evaluation-part-1-27a472b09893), [Part 2: Generation](https://medium.com/
+relari/a-practical-guide-to-rag-evaluation-part-2-generation-c79b1bde0f5d) -
+How important is a Golden Dataset for LLM evaluation? [(link)](https://
+medium.com/relari/how-important-is-a-golden-dataset-for-llm-pipeline-
+evaluation-4ef6deb14dc5) - How to evaluate complex GenAI Apps: a granular
+approach [(link)](https://medium.com/relari/how-to-evaluate-complex-genai-apps-
+a-granular-approach-0ab929d5b3e2) - How to Make the Most Out of LLM Production
+Data: Simulated User Feedback [(link)](https://medium.com/towards-data-science/
+how-to-make-the-most-out-of-llm-production-data-simulated-user-feedback-
+843c444febc7) - Generate Synthetic Data to Test LLM Applications [(link)]
+(https://medium.com/relari/generate-synthetic-data-to-test-llm-applications-
+4bffeb51b80e) - **Discord:** Join our community of LLM developers [Discord]
 (https://discord.gg/GJnM8SRsHr) - **Reach out to founders:** [Email](mailto:
 founders@relari.ai) or [Schedule a chat](https://cal.com/pasquale/continuous-
 eval) ## License This project is licensed under the Apache 2.0 - see the
 [LICENSE](LICENSE) file for details. ## Open Analytics We monitor basic
 anonymous usage statistics to understand our users' preferences, inform new
 features, and identify areas that might need improvement. You can take a look
 at exactly what we track in the [telemetry code](continuous_eval/utils/
```

