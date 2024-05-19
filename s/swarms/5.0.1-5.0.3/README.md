# Comparing `tmp/swarms-5.0.1.tar.gz` & `tmp/swarms-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-5.0.1.tar", max compression
+gzip compressed data, was "swarms-5.0.3.tar", max compression
```

## Comparing `swarms-5.0.1.tar` & `swarms-5.0.3.tar`

### file list

```diff
@@ -1,218 +1,217 @@
--rw-r--r--   0        0        0    15674 2024-03-27 19:29:36.857220 swarms-5.0.1/LICENSE
--rw-r--r--   0        0        0    38811 2024-05-12 02:54:30.662552 swarms-5.0.1/README.md
--rw-r--r--   0        0        0     1811 2024-05-14 16:06:07.673358 swarms-5.0.1/pyproject.toml
--rw-r--r--   0        0        0      590 2024-05-10 15:36:40.566920 swarms-5.0.1/swarms/__init__.py
--rw-r--r--   0        0        0      864 2024-03-15 22:19:21.000202 swarms-5.0.1/swarms/agents/__init__.py
--rw-r--r--   0        0        0      881 2024-03-15 22:19:21.001107 swarms-5.0.1/swarms/agents/agent_wrapper.py
--rw-r--r--   0        0        0     3342 2024-03-21 23:46:38.264917 swarms-5.0.1/swarms/agents/base.py
--rw-r--r--   0        0        0     4201 2024-03-15 22:19:21.002271 swarms-5.0.1/swarms/agents/developer_agents.py
--rw-r--r--   0        0        0     2950 2024-03-27 19:12:09.754781 swarms-5.0.1/swarms/agents/omni_modal_agent.py
--rw-r--r--   0        0        0     3491 2024-04-27 21:17:36.621105 swarms-5.0.1/swarms/agents/simple_agent.py
--rw-r--r--   0        0        0      484 2024-03-15 22:19:21.004680 swarms-5.0.1/swarms/agents/stopping_conditions.py
--rw-r--r--   0        0        0     4940 2024-04-27 21:17:36.621832 swarms-5.0.1/swarms/agents/tool_agent.py
--rw-r--r--   0        0        0     5504 2024-05-08 21:09:56.813124 swarms-5.0.1/swarms/agents/worker_agent.py
--rw-r--r--   0        0        0      167 2024-03-15 22:19:21.006869 swarms-5.0.1/swarms/artifacts/__init__.py
--rw-r--r--   0        0        0     1675 2024-03-15 22:19:21.007269 swarms-5.0.1/swarms/artifacts/base_artifact.py
--rw-r--r--   0        0        0     2299 2024-03-27 19:27:30.716559 swarms-5.0.1/swarms/artifacts/text_artifact.py
--rw-r--r--   0        0        0      613 2024-04-27 21:17:36.623130 swarms-5.0.1/swarms/memory/__init__.py
--rw-r--r--   0        0        0      433 2024-03-15 22:19:21.012591 swarms-5.0.1/swarms/memory/action_subtask.py
--rw-r--r--   0        0        0     3475 2024-03-15 22:19:21.012989 swarms-5.0.1/swarms/memory/base_db.py
--rw-r--r--   0        0        0     2823 2024-04-27 21:17:36.624819 swarms-5.0.1/swarms/memory/base_vectordb.py
--rw-r--r--   0        0        0     2895 2024-03-15 22:19:21.014370 swarms-5.0.1/swarms/memory/dict_internal_memory.py
--rw-r--r--   0        0        0     3306 2024-04-18 12:42:39.319739 swarms-5.0.1/swarms/memory/dict_shared_memory.py
--rw-r--r--   0        0        0     5499 2024-04-18 12:43:26.648904 swarms-5.0.1/swarms/memory/short_term_memory.py
--rw-r--r--   0        0        0     3371 2024-03-15 22:19:21.018970 swarms-5.0.1/swarms/memory/visual_memory.py
--rw-r--r--   0        0        0     2608 2024-05-08 21:09:56.817128 swarms-5.0.1/swarms/models/__init__.py
--rw-r--r--   0        0        0     2060 2024-04-18 12:43:26.678061 swarms-5.0.1/swarms/models/base_embedding_model.py
--rw-r--r--   0        0        0    13168 2024-04-27 21:17:36.635065 swarms-5.0.1/swarms/models/base_llm.py
--rw-r--r--   0        0        0    12604 2024-04-18 12:43:27.187223 swarms-5.0.1/swarms/models/base_multimodal_model.py
--rw-r--r--   0        0        0     2475 2024-04-27 21:17:36.635700 swarms-5.0.1/swarms/models/base_tts.py
--rw-r--r--   0        0        0     3163 2024-04-27 21:17:36.636332 swarms-5.0.1/swarms/models/base_ttv.py
--rw-r--r--   0        0        0    16743 2024-04-18 12:43:27.429345 swarms-5.0.1/swarms/models/cog_vlm.py
--rw-r--r--   0        0        0    10760 2024-04-18 12:43:27.137440 swarms-5.0.1/swarms/models/dalle3.py
--rw-r--r--   0        0        0     6449 2024-04-18 12:43:26.972838 swarms-5.0.1/swarms/models/distilled_whisperx.py
--rw-r--r--   0        0        0      682 2024-04-18 12:43:26.722086 swarms-5.0.1/swarms/models/embeddings_base.py
--rw-r--r--   0        0        0     2726 2024-04-27 21:17:36.637208 swarms-5.0.1/swarms/models/fire_function.py
--rw-r--r--   0        0        0     3022 2024-03-15 22:19:21.032963 swarms-5.0.1/swarms/models/fuyu.py
--rw-r--r--   0        0        0     7762 2024-04-18 12:42:39.844485 swarms-5.0.1/swarms/models/gemini.py
--rw-r--r--   0        0        0    14236 2024-05-14 15:55:46.753852 swarms-5.0.1/swarms/models/gpt4_vision_api.py
--rw-r--r--   0        0        0    12996 2024-04-27 21:17:36.638023 swarms-5.0.1/swarms/models/huggingface.py
--rw-r--r--   0        0        0     1826 2024-04-27 21:17:36.638977 swarms-5.0.1/swarms/models/huggingface_pipeline.py
--rw-r--r--   0        0        0     5601 2024-04-18 12:43:27.069960 swarms-5.0.1/swarms/models/idefics.py
--rw-r--r--   0        0        0    10672 2024-04-18 12:43:27.705223 swarms-5.0.1/swarms/models/kosmos_two.py
--rw-r--r--   0        0        0     1448 2024-03-15 22:19:21.037679 swarms-5.0.1/swarms/models/layoutlm_document_qa.py
--rw-r--r--   0        0        0     6581 2024-04-27 21:17:36.639950 swarms-5.0.1/swarms/models/llama_function_caller.py
--rw-r--r--   0        0        0     2762 2024-03-15 22:19:21.038340 swarms-5.0.1/swarms/models/llava.py
--rw-r--r--   0        0        0     4286 2024-04-27 21:17:36.641073 swarms-5.0.1/swarms/models/mistral.py
--rw-r--r--   0        0        0     2147 2024-04-27 21:17:36.642823 swarms-5.0.1/swarms/models/mixtral.py
--rw-r--r--   0        0        0     2056 2024-03-15 22:19:21.041522 swarms-5.0.1/swarms/models/moondream_mm.py
--rw-r--r--   0        0        0     6448 2024-04-18 12:43:27.582607 swarms-5.0.1/swarms/models/mpt.py
--rw-r--r--   0        0        0     2823 2024-04-18 12:43:27.453365 swarms-5.0.1/swarms/models/nougat.py
--rw-r--r--   0        0        0     2366 2024-03-15 22:19:21.043550 swarms-5.0.1/swarms/models/open_dalle.py
--rw-r--r--   0        0        0     2464 2024-04-27 21:17:36.644597 swarms-5.0.1/swarms/models/open_router.py
--rw-r--r--   0        0        0      106 2024-04-25 14:24:46.757474 swarms-5.0.1/swarms/models/openai_embeddings.py
--rw-r--r--   0        0        0     3167 2024-04-27 21:17:36.645494 swarms-5.0.1/swarms/models/openai_tts.py
--rw-r--r--   0        0        0       93 2024-04-25 14:24:46.757393 swarms-5.0.1/swarms/models/palm.py
--rw-r--r--   0        0        0     2160 2024-05-08 21:09:56.821210 swarms-5.0.1/swarms/models/popular_llms.py
--rw-r--r--   0        0        0     4813 2024-04-18 12:43:27.720842 swarms-5.0.1/swarms/models/qwen.py
--rw-r--r--   0        0        0     3547 2024-04-18 12:43:27.606549 swarms-5.0.1/swarms/models/sam.py
--rw-r--r--   0        0        0    12675 2024-04-18 12:43:28.000334 swarms-5.0.1/swarms/models/sampling_params.py
--rw-r--r--   0        0        0     7621 2024-04-18 12:43:27.738035 swarms-5.0.1/swarms/models/speecht5.py
--rw-r--r--   0        0        0     8244 2024-04-18 12:43:28.025933 swarms-5.0.1/swarms/models/ssd_1b.py
--rw-r--r--   0        0        0     5189 2024-04-18 12:43:27.897205 swarms-5.0.1/swarms/models/stable_diffusion.py
--rw-r--r--   0        0        0     1794 2024-03-15 22:19:21.052816 swarms-5.0.1/swarms/models/timm.py
--rw-r--r--   0        0        0     3948 2024-04-27 21:17:36.646243 swarms-5.0.1/swarms/models/together.py
--rw-r--r--   0        0        0      592 2024-03-15 22:19:21.054281 swarms-5.0.1/swarms/models/types.py
--rw-r--r--   0        0        0     1731 2024-03-15 22:19:21.054977 swarms-5.0.1/swarms/models/vilt.py
--rw-r--r--   0        0        0     2846 2024-03-15 22:19:21.055732 swarms-5.0.1/swarms/models/vip_llava.py
--rw-r--r--   0        0        0     3681 2024-04-18 12:43:27.995338 swarms-5.0.1/swarms/models/zeroscope.py
--rw-r--r--   0        0        0        0 2024-05-01 03:43:07.020028 swarms-5.0.1/swarms/prebuilt_swarms/__init__.py
--rw-r--r--   0        0        0      692 2024-05-08 21:09:56.824718 swarms-5.0.1/swarms/prompts/__init__.py
--rw-r--r--   0        0        0    11320 2024-03-15 22:19:21.061563 swarms-5.0.1/swarms/prompts/accountant_swarm_prompts.py
--rw-r--r--   0        0        0     9156 2024-03-15 22:19:21.062133 swarms-5.0.1/swarms/prompts/aga.py
--rw-r--r--   0        0        0     1451 2024-03-15 22:19:21.062911 swarms-5.0.1/swarms/prompts/agent_output_parser.py
--rw-r--r--   0        0        0     2705 2024-04-18 12:43:28.068653 swarms-5.0.1/swarms/prompts/agent_prompt.py
--rw-r--r--   0        0        0     6886 2024-03-15 22:19:21.064160 swarms-5.0.1/swarms/prompts/agent_prompts.py
--rw-r--r--   0        0        0     7113 2024-05-08 21:09:56.832506 swarms-5.0.1/swarms/prompts/agent_system_prompts.py
--rw-r--r--   0        0        0     5233 2024-03-15 22:19:21.065787 swarms-5.0.1/swarms/prompts/ai_research_team.py
--rw-r--r--   0        0        0     1148 2024-05-01 03:43:07.021040 swarms-5.0.1/swarms/prompts/aot_prompt.py
--rw-r--r--   0        0        0    13981 2024-03-15 22:19:21.066513 swarms-5.0.1/swarms/prompts/autobloggen.py
--rw-r--r--   0        0        0     5605 2024-03-15 22:19:21.068224 swarms-5.0.1/swarms/prompts/autoswarm.py
--rw-r--r--   0        0        0     7542 2024-04-18 12:43:28.353296 swarms-5.0.1/swarms/prompts/base.py
--rw-r--r--   0        0        0     3801 2024-04-18 12:43:28.227538 swarms-5.0.1/swarms/prompts/chat_prompt.py
--rw-r--r--   0        0        0     2235 2024-03-15 22:19:21.069096 swarms-5.0.1/swarms/prompts/code_interpreter.py
--rw-r--r--   0        0        0     4106 2024-03-15 22:19:21.069652 swarms-5.0.1/swarms/prompts/code_spawner.py
--rw-r--r--   0        0        0     1566 2024-03-15 22:19:21.069820 swarms-5.0.1/swarms/prompts/debate.py
--rw-r--r--   0        0        0     7044 2024-03-15 22:19:21.070670 swarms-5.0.1/swarms/prompts/documentation.py
--rw-r--r--   0        0        0     1767 2024-03-15 22:19:21.071442 swarms-5.0.1/swarms/prompts/education.py
--rw-r--r--   0        0        0     4180 2024-03-15 22:19:21.071791 swarms-5.0.1/swarms/prompts/finance_agent_prompt.py
--rw-r--r--   0        0        0     4117 2024-03-15 22:19:21.072144 swarms-5.0.1/swarms/prompts/growth_agent_prompt.py
--rw-r--r--   0        0        0      880 2024-03-15 22:19:21.072694 swarms-5.0.1/swarms/prompts/idea2img.py
--rw-r--r--   0        0        0     3346 2024-03-15 22:19:21.072990 swarms-5.0.1/swarms/prompts/legal_agent_prompt.py
--rw-r--r--   0        0        0     4785 2024-03-15 22:19:21.073912 swarms-5.0.1/swarms/prompts/logistics.py
--rw-r--r--   0        0        0     3374 2024-04-10 15:42:56.140463 swarms-5.0.1/swarms/prompts/meta_system_prompt.py
--rw-r--r--   0        0        0    10662 2024-03-15 22:19:21.074621 swarms-5.0.1/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
--rw-r--r--   0        0        0     3511 2024-03-15 22:19:21.075295 swarms-5.0.1/swarms/prompts/multi_modal_prompts.py
--rw-r--r--   0        0        0     3225 2024-03-15 22:19:21.075646 swarms-5.0.1/swarms/prompts/multi_modal_visual_prompts.py
--rw-r--r--   0        0        0     3454 2024-03-15 22:19:21.076012 swarms-5.0.1/swarms/prompts/operations_agent_prompt.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.076143 swarms-5.0.1/swarms/prompts/orchestrator_prompt.py
--rw-r--r--   0        0        0     2149 2024-03-15 22:19:21.076733 swarms-5.0.1/swarms/prompts/personal_stylist.py
--rw-r--r--   0        0        0     8333 2024-03-15 22:19:21.077280 swarms-5.0.1/swarms/prompts/product_agent_prompt.py
--rw-r--r--   0        0        0    10144 2024-03-15 22:19:21.078026 swarms-5.0.1/swarms/prompts/programming.py
--rw-r--r--   0        0        0     2128 2024-03-15 22:19:21.078275 swarms-5.0.1/swarms/prompts/project_manager.py
--rw-r--r--   0        0        0    13215 2024-04-18 12:43:28.152390 swarms-5.0.1/swarms/prompts/python.py
--rw-r--r--   0        0        0     2960 2024-03-15 22:19:21.079805 swarms-5.0.1/swarms/prompts/react.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.080059 swarms-5.0.1/swarms/prompts/refiner_agent_prompt.py
--rw-r--r--   0        0        0     5126 2024-03-15 22:19:21.080659 swarms-5.0.1/swarms/prompts/sales.py
--rw-r--r--   0        0        0     5013 2024-03-15 22:19:21.081280 swarms-5.0.1/swarms/prompts/sales_prompts.py
--rw-r--r--   0        0        0     2679 2024-03-15 22:19:21.083072 swarms-5.0.1/swarms/prompts/security_team.py
--rw-r--r--   0        0        0     3252 2024-04-18 12:43:28.128596 swarms-5.0.1/swarms/prompts/self_operating_prompt.py
--rw-r--r--   0        0        0     4147 2024-03-15 22:19:21.084066 swarms-5.0.1/swarms/prompts/sop_generator_agent_prompt.py
--rw-r--r--   0        0        0     4640 2024-03-15 22:19:21.084386 swarms-5.0.1/swarms/prompts/summaries_prompts.py
--rw-r--r--   0        0        0     3984 2024-03-15 22:19:21.084631 swarms-5.0.1/swarms/prompts/support_agent_prompt.py
--rw-r--r--   0        0        0     4280 2024-03-15 22:19:21.085244 swarms-5.0.1/swarms/prompts/swarm_manager_agent.py
--rw-r--r--   0        0        0      728 2024-03-15 22:19:21.085725 swarms-5.0.1/swarms/prompts/task_assignment_prompt.py
--rw-r--r--   0        0        0     4271 2024-04-18 12:43:28.167424 swarms-5.0.1/swarms/prompts/tests.py
--rw-r--r--   0        0        0     4288 2024-03-15 22:19:21.086625 swarms-5.0.1/swarms/prompts/tools.py
--rw-r--r--   0        0        0     2398 2024-03-15 22:19:21.087352 swarms-5.0.1/swarms/prompts/urban_planning.py
--rw-r--r--   0        0        0     3675 2024-03-15 22:19:21.087654 swarms-5.0.1/swarms/prompts/visual_cot.py
--rw-r--r--   0        0        0     5596 2024-05-08 21:09:56.838185 swarms-5.0.1/swarms/prompts/worker_prompt.py
--rw-r--r--   0        0        0     2349 2024-03-15 22:19:21.088382 swarms-5.0.1/swarms/prompts/xray_swarm_prompt.py
--rw-r--r--   0        0        0     4067 2024-05-12 02:54:30.718662 swarms-5.0.1/swarms/structs/__init__.py
--rw-r--r--   0        0        0    60053 2024-05-11 00:24:43.040147 swarms-5.0.1/swarms/structs/agent.py
--rw-r--r--   0        0        0      574 2024-03-15 22:19:21.092491 swarms-5.0.1/swarms/structs/agent_job.py
--rw-r--r--   0        0        0     2937 2024-04-22 15:42:05.980151 swarms-5.0.1/swarms/structs/agent_process.py
--rw-r--r--   0        0        0     3718 2024-04-18 12:43:28.377820 swarms-5.0.1/swarms/structs/async_workflow.py
--rw-r--r--   0        0        0     5579 2024-04-22 14:27:36.702871 swarms-5.0.1/swarms/structs/auto_swarm.py
--rw-r--r--   0        0        0    12437 2024-04-23 01:08:13.052177 swarms-5.0.1/swarms/structs/base_structure.py
--rw-r--r--   0        0        0    19446 2024-05-08 21:09:56.884181 swarms-5.0.1/swarms/structs/base_swarm.py
--rw-r--r--   0        0        0    12161 2024-05-08 21:09:56.888358 swarms-5.0.1/swarms/structs/base_workflow.py
--rw-r--r--   0        0        0     1056 2024-03-15 22:19:21.095125 swarms-5.0.1/swarms/structs/block_wrapper.py
--rw-r--r--   0        0        0     3188 2024-04-18 02:05:51.225713 swarms-5.0.1/swarms/structs/blocks_dict.py
--rw-r--r--   0        0        0     4851 2024-04-18 12:43:28.719057 swarms-5.0.1/swarms/structs/blocks_list.py
--rw-r--r--   0        0        0     5206 2024-04-18 12:43:28.754865 swarms-5.0.1/swarms/structs/company.py
--rw-r--r--   0        0        0     4471 2024-04-18 12:43:28.724904 swarms-5.0.1/swarms/structs/concurrent_workflow.py
--rw-r--r--   0        0        0    14685 2024-04-26 04:55:42.709791 swarms-5.0.1/swarms/structs/conversation.py
--rw-r--r--   0        0        0    12549 2024-04-18 12:43:29.326347 swarms-5.0.1/swarms/structs/debate.py
--rw-r--r--   0        0        0     3041 2024-03-15 22:19:21.099360 swarms-5.0.1/swarms/structs/document.py
--rw-r--r--   0        0        0     4775 2024-04-26 04:55:42.710484 swarms-5.0.1/swarms/structs/groupchat.py
--rw-r--r--   0        0        0     4545 2024-03-15 22:19:21.101122 swarms-5.0.1/swarms/structs/long_swarm.py
--rw-r--r--   0        0        0     7012 2024-04-18 12:43:29.037949 swarms-5.0.1/swarms/structs/majority_voting.py
--rw-r--r--   0        0        0      745 2024-04-22 15:59:38.669639 swarms-5.0.1/swarms/structs/message.py
--rw-r--r--   0        0        0     7338 2024-04-18 12:43:29.012263 swarms-5.0.1/swarms/structs/message_pool.py
--rw-r--r--   0        0        0      855 2024-04-27 21:17:36.650763 swarms-5.0.1/swarms/structs/meta_system_prompt.py
--rw-r--r--   0        0        0     5751 2024-04-18 12:43:29.210773 swarms-5.0.1/swarms/structs/model_parallizer.py
--rw-r--r--   0        0        0     8390 2024-04-22 15:59:38.738279 swarms-5.0.1/swarms/structs/multi_agent_collab.py
--rw-r--r--   0        0        0     5623 2024-04-18 12:43:29.243594 swarms-5.0.1/swarms/structs/multi_process_workflow.py
--rw-r--r--   0        0        0     5272 2024-04-18 12:42:41.990321 swarms-5.0.1/swarms/structs/multi_threaded_workflow.py
--rw-r--r--   0        0        0      371 2024-04-27 21:17:36.651437 swarms-5.0.1/swarms/structs/omni_agent_types.py
--rw-r--r--   0        0        0      182 2024-04-28 21:24:54.081857 swarms-5.0.1/swarms/structs/plan.py
--rw-r--r--   0        0        0     7207 2024-05-11 02:57:32.266553 swarms-5.0.1/swarms/structs/rearrange.py
--rw-r--r--   0        0        0     2727 2024-04-18 12:42:41.946623 swarms-5.0.1/swarms/structs/recursive_workflow.py
--rw-r--r--   0        0        0     3256 2024-05-13 20:15:02.129223 swarms-5.0.1/swarms/structs/round_robin.py
--rw-r--r--   0        0        0     6764 2024-04-23 01:17:51.964275 swarms-5.0.1/swarms/structs/schemas.py
--rw-r--r--   0        0        0     2956 2024-05-08 21:09:56.891925 swarms-5.0.1/swarms/structs/sequential_workflow.py
--rw-r--r--   0        0        0     2337 2024-03-27 19:47:31.068657 swarms-5.0.1/swarms/structs/sermon_swarm.py
--rw-r--r--   0        0        0      709 2024-05-08 21:09:56.895373 swarms-5.0.1/swarms/structs/step.py
--rw-r--r--   0        0        0    10684 2024-04-18 12:43:29.602325 swarms-5.0.1/swarms/structs/swarm_net.py
--rw-r--r--   0        0        0     6426 2024-04-18 12:43:29.666155 swarms-5.0.1/swarms/structs/swarming_architectures.py
--rw-r--r--   0        0        0     8179 2024-04-18 12:43:29.569178 swarms-5.0.1/swarms/structs/task.py
--rw-r--r--   0        0        0     1989 2024-03-27 19:12:09.705030 swarms-5.0.1/swarms/structs/task_queue_base.py
--rw-r--r--   0        0        0     3511 2024-04-18 12:42:42.279735 swarms-5.0.1/swarms/structs/utils.py
--rw-r--r--   0        0        0     7403 2024-04-24 00:20:16.136940 swarms-5.0.1/swarms/structs/yaml_model.py
--rw-r--r--   0        0        0      891 2024-03-27 19:12:09.674045 swarms-5.0.1/swarms/telemetry/__init__.py
--rw-r--r--   0        0        0      513 2024-04-18 12:43:29.468850 swarms-5.0.1/swarms/telemetry/auto_upgrade_swarms.py
--rw-r--r--   0        0        0      385 2024-04-02 02:30:28.437471 swarms-5.0.1/swarms/telemetry/bootup.py
--rw-r--r--   0        0        0     1073 2024-04-18 12:42:42.280090 swarms-5.0.1/swarms/telemetry/check_update.py
--rw-r--r--   0        0        0      807 2024-03-15 22:19:21.114471 swarms-5.0.1/swarms/telemetry/log_all.py
--rw-r--r--   0        0        0      496 2024-03-22 00:42:19.696403 swarms-5.0.1/swarms/telemetry/sentry_active.py
--rw-r--r--   0        0        0     2675 2024-04-23 23:56:19.053195 swarms-5.0.1/swarms/telemetry/sys_info.py
--rw-r--r--   0        0        0     1879 2024-04-24 21:57:07.051275 swarms-5.0.1/swarms/telemetry/user_utils.py
--rw-r--r--   0        0        0     1680 2024-05-08 21:09:56.899526 swarms-5.0.1/swarms/tools/__init__.py
--rw-r--r--   0        0        0    12525 2024-05-08 21:09:56.906505 swarms-5.0.1/swarms/tools/base_tool.py
--rw-r--r--   0        0        0     6653 2024-04-18 12:47:32.769219 swarms-5.0.1/swarms/tools/code_interpreter.py
--rw-r--r--   0        0        0     5367 2024-05-08 21:09:56.913861 swarms-5.0.1/swarms/tools/exec_tool.py
--rw-r--r--   0        0        0      773 2024-04-03 12:10:21.536239 swarms-5.0.1/swarms/tools/function_util.py
--rw-r--r--   0        0        0    14241 2024-04-27 21:17:36.654062 swarms-5.0.1/swarms/tools/json_former.py
--rw-r--r--   0        0        0     1316 2024-03-21 23:46:38.581600 swarms-5.0.1/swarms/tools/json_utils.py
--rw-r--r--   0        0        0     2455 2024-04-18 12:42:42.475166 swarms-5.0.1/swarms/tools/logits_processor.py
--rw-r--r--   0        0        0     1461 2024-04-18 12:43:30.100050 swarms-5.0.1/swarms/tools/math_eval.py
--rw-r--r--   0        0        0      978 2024-04-23 23:18:25.950155 swarms-5.0.1/swarms/tools/openai_func_calling_schema.py
--rw-r--r--   0        0        0    13875 2024-05-08 21:09:56.921184 swarms-5.0.1/swarms/tools/openai_tool_creator_decorator.py
--rw-r--r--   0        0        0    15564 2024-04-27 21:17:36.657668 swarms-5.0.1/swarms/tools/py_func_to_openai_func_str.py
--rw-r--r--   0        0        0     4275 2024-05-08 21:09:56.925611 swarms-5.0.1/swarms/tools/pydantic_to_json.py
--rw-r--r--   0        0        0      157 2024-03-24 04:12:12.223834 swarms-5.0.1/swarms/tools/tool.py
--rw-r--r--   0        0        0     6170 2024-05-08 21:09:56.930060 swarms-5.0.1/swarms/tools/tool_utils.py
--rw-r--r--   0        0        0     5466 2024-03-15 22:19:21.122024 swarms-5.0.1/swarms/utils/README.md
--rw-r--r--   0        0        0     1956 2024-04-18 15:06:06.195732 swarms-5.0.1/swarms/utils/__init__.py
--rw-r--r--   0        0        0     3507 2024-04-18 12:42:42.565998 swarms-5.0.1/swarms/utils/apa.py
--rw-r--r--   0        0        0     6065 2024-04-18 12:42:42.646659 swarms-5.0.1/swarms/utils/check_function_result.py
--rw-r--r--   0        0        0     1008 2024-03-15 22:19:21.124143 swarms-5.0.1/swarms/utils/class_args_wrapper.py
--rw-r--r--   0        0        0     1234 2024-04-18 12:42:42.478906 swarms-5.0.1/swarms/utils/concurrent_utils.py
--rw-r--r--   0        0        0     1865 2024-04-18 12:42:42.546898 swarms-5.0.1/swarms/utils/data_to_text.py
--rw-r--r--   0        0        0     2451 2024-04-18 12:43:29.983708 swarms-5.0.1/swarms/utils/decorators.py
--rw-r--r--   0        0        0     1311 2024-03-15 22:19:21.127902 swarms-5.0.1/swarms/utils/disable_logging.py
--rw-r--r--   0        0        0      890 2024-03-15 22:19:21.128555 swarms-5.0.1/swarms/utils/download_img.py
--rw-r--r--   0        0        0     1127 2024-03-15 22:19:21.129540 swarms-5.0.1/swarms/utils/execute_futures.py
--rw-r--r--   0        0        0     1113 2024-03-15 22:19:21.130281 swarms-5.0.1/swarms/utils/exponential_backoff.py
--rw-r--r--   0        0        0      854 2024-03-15 22:19:21.130759 swarms-5.0.1/swarms/utils/fetch_init_params.py
--rw-r--r--   0        0        0      500 2024-03-15 22:19:21.131255 swarms-5.0.1/swarms/utils/file_extension_seach.py
--rw-r--r--   0        0        0     3266 2024-04-18 12:42:42.739802 swarms-5.0.1/swarms/utils/file_processing.py
--rw-r--r--   0        0        0      630 2024-04-18 12:43:29.910068 swarms-5.0.1/swarms/utils/find_img_path.py
--rw-r--r--   0        0        0     4184 2024-04-18 12:43:30.069758 swarms-5.0.1/swarms/utils/get_logger.py
--rw-r--r--   0        0        0     2848 2024-04-18 12:43:30.028262 swarms-5.0.1/swarms/utils/json_output_parser.py
--rw-r--r--   0        0        0     1831 2024-04-18 12:42:42.783557 swarms-5.0.1/swarms/utils/jsonl_utils.py
--rw-r--r--   0        0        0      932 2024-03-15 22:19:21.135261 swarms-5.0.1/swarms/utils/llm_metrics_decorator.py
--rw-r--r--   0        0        0     2209 2024-04-18 12:43:30.070521 swarms-5.0.1/swarms/utils/logger.py
--rw-r--r--   0        0        0    16186 2024-04-18 12:43:30.846131 swarms-5.0.1/swarms/utils/loggers.py
--rw-r--r--   0        0        0      453 2024-03-27 19:12:09.738695 swarms-5.0.1/swarms/utils/loguru_logger.py
--rw-r--r--   0        0        0      711 2024-03-27 19:12:09.676603 swarms-5.0.1/swarms/utils/markdown_message.py
--rw-r--r--   0        0        0      600 2024-03-15 22:19:21.139501 swarms-5.0.1/swarms/utils/parse_code.py
--rw-r--r--   0        0        0     1177 2024-04-18 12:43:30.100653 swarms-5.0.1/swarms/utils/pdf_to_text.py
--rw-r--r--   0        0        0     1353 2024-03-15 22:19:21.141276 swarms-5.0.1/swarms/utils/remove_json_whitespace.py
--rw-r--r--   0        0        0     1278 2024-04-18 12:42:42.936792 swarms-5.0.1/swarms/utils/save_logs.py
--rw-r--r--   0        0        0     4774 2024-04-18 12:42:43.138354 swarms-5.0.1/swarms/utils/serializable.py
--rw-r--r--   0        0        0     1315 2024-04-25 14:49:22.838126 swarms-5.0.1/swarms/utils/try_except_wrapper.py
--rw-r--r--   0        0        0     2668 2024-04-18 12:43:30.304280 swarms-5.0.1/swarms/utils/yaml_output_parser.py
--rw-r--r--   0        0        0    41490 1970-01-01 00:00:00.000000 swarms-5.0.1/setup.py
--rw-r--r--   0        0        0    40367 1970-01-01 00:00:00.000000 swarms-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0    15674 2024-03-27 19:29:36.857220 swarms-5.0.3/LICENSE
+-rw-r--r--   0        0        0    37907 2024-05-17 04:37:25.650827 swarms-5.0.3/README.md
+-rw-r--r--   0        0        0     1790 2024-05-19 03:24:03.190053 swarms-5.0.3/pyproject.toml
+-rw-r--r--   0        0        0      590 2024-05-10 15:36:40.566920 swarms-5.0.3/swarms/__init__.py
+-rw-r--r--   0        0        0      864 2024-03-15 22:19:21.000202 swarms-5.0.3/swarms/agents/__init__.py
+-rw-r--r--   0        0        0      881 2024-03-15 22:19:21.001107 swarms-5.0.3/swarms/agents/agent_wrapper.py
+-rw-r--r--   0        0        0     3342 2024-03-21 23:46:38.264917 swarms-5.0.3/swarms/agents/base.py
+-rw-r--r--   0        0        0     4201 2024-03-15 22:19:21.002271 swarms-5.0.3/swarms/agents/developer_agents.py
+-rw-r--r--   0        0        0     2950 2024-03-27 19:12:09.754781 swarms-5.0.3/swarms/agents/omni_modal_agent.py
+-rw-r--r--   0        0        0     3491 2024-04-27 21:17:36.621105 swarms-5.0.3/swarms/agents/simple_agent.py
+-rw-r--r--   0        0        0      484 2024-03-15 22:19:21.004680 swarms-5.0.3/swarms/agents/stopping_conditions.py
+-rw-r--r--   0        0        0     4940 2024-04-27 21:17:36.621832 swarms-5.0.3/swarms/agents/tool_agent.py
+-rw-r--r--   0        0        0     5504 2024-05-08 21:09:56.813124 swarms-5.0.3/swarms/agents/worker_agent.py
+-rw-r--r--   0        0        0      167 2024-03-15 22:19:21.006869 swarms-5.0.3/swarms/artifacts/__init__.py
+-rw-r--r--   0        0        0     1675 2024-03-15 22:19:21.007269 swarms-5.0.3/swarms/artifacts/base_artifact.py
+-rw-r--r--   0        0        0     2299 2024-03-27 19:27:30.716559 swarms-5.0.3/swarms/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      613 2024-04-27 21:17:36.623130 swarms-5.0.3/swarms/memory/__init__.py
+-rw-r--r--   0        0        0      433 2024-03-15 22:19:21.012591 swarms-5.0.3/swarms/memory/action_subtask.py
+-rw-r--r--   0        0        0     3475 2024-03-15 22:19:21.012989 swarms-5.0.3/swarms/memory/base_db.py
+-rw-r--r--   0        0        0     2823 2024-04-27 21:17:36.624819 swarms-5.0.3/swarms/memory/base_vectordb.py
+-rw-r--r--   0        0        0     2895 2024-03-15 22:19:21.014370 swarms-5.0.3/swarms/memory/dict_internal_memory.py
+-rw-r--r--   0        0        0     3306 2024-04-18 12:42:39.319739 swarms-5.0.3/swarms/memory/dict_shared_memory.py
+-rw-r--r--   0        0        0     5499 2024-04-18 12:43:26.648904 swarms-5.0.3/swarms/memory/short_term_memory.py
+-rw-r--r--   0        0        0     3371 2024-03-15 22:19:21.018970 swarms-5.0.3/swarms/memory/visual_memory.py
+-rw-r--r--   0        0        0     2533 2024-05-18 23:20:02.171975 swarms-5.0.3/swarms/models/__init__.py
+-rw-r--r--   0        0        0     2060 2024-04-18 12:43:26.678061 swarms-5.0.3/swarms/models/base_embedding_model.py
+-rw-r--r--   0        0        0    13168 2024-04-27 21:17:36.635065 swarms-5.0.3/swarms/models/base_llm.py
+-rw-r--r--   0        0        0    12604 2024-04-18 12:43:27.187223 swarms-5.0.3/swarms/models/base_multimodal_model.py
+-rw-r--r--   0        0        0     2475 2024-04-27 21:17:36.635700 swarms-5.0.3/swarms/models/base_tts.py
+-rw-r--r--   0        0        0     3163 2024-04-27 21:17:36.636332 swarms-5.0.3/swarms/models/base_ttv.py
+-rw-r--r--   0        0        0    16743 2024-04-18 12:43:27.429345 swarms-5.0.3/swarms/models/cog_vlm.py
+-rw-r--r--   0        0        0    10760 2024-04-18 12:43:27.137440 swarms-5.0.3/swarms/models/dalle3.py
+-rw-r--r--   0        0        0     6449 2024-04-18 12:43:26.972838 swarms-5.0.3/swarms/models/distilled_whisperx.py
+-rw-r--r--   0        0        0      682 2024-04-18 12:43:26.722086 swarms-5.0.3/swarms/models/embeddings_base.py
+-rw-r--r--   0        0        0     2726 2024-04-27 21:17:36.637208 swarms-5.0.3/swarms/models/fire_function.py
+-rw-r--r--   0        0        0     3022 2024-03-15 22:19:21.032963 swarms-5.0.3/swarms/models/fuyu.py
+-rw-r--r--   0        0        0     7762 2024-04-18 12:42:39.844485 swarms-5.0.3/swarms/models/gemini.py
+-rw-r--r--   0        0        0    14236 2024-05-14 15:55:46.753852 swarms-5.0.3/swarms/models/gpt4_vision_api.py
+-rw-r--r--   0        0        0    12996 2024-04-27 21:17:36.638023 swarms-5.0.3/swarms/models/huggingface.py
+-rw-r--r--   0        0        0     1826 2024-04-27 21:17:36.638977 swarms-5.0.3/swarms/models/huggingface_pipeline.py
+-rw-r--r--   0        0        0     5601 2024-04-18 12:43:27.069960 swarms-5.0.3/swarms/models/idefics.py
+-rw-r--r--   0        0        0    10672 2024-04-18 12:43:27.705223 swarms-5.0.3/swarms/models/kosmos_two.py
+-rw-r--r--   0        0        0     1448 2024-03-15 22:19:21.037679 swarms-5.0.3/swarms/models/layoutlm_document_qa.py
+-rw-r--r--   0        0        0     2529 2024-05-18 17:55:07.794536 swarms-5.0.3/swarms/models/llama3_hosted.py
+-rw-r--r--   0        0        0     6581 2024-04-27 21:17:36.639950 swarms-5.0.3/swarms/models/llama_function_caller.py
+-rw-r--r--   0        0        0     2762 2024-03-15 22:19:21.038340 swarms-5.0.3/swarms/models/llava.py
+-rw-r--r--   0        0        0     4286 2024-04-27 21:17:36.641073 swarms-5.0.3/swarms/models/mistral.py
+-rw-r--r--   0        0        0     2147 2024-04-27 21:17:36.642823 swarms-5.0.3/swarms/models/mixtral.py
+-rw-r--r--   0        0        0     2056 2024-03-15 22:19:21.041522 swarms-5.0.3/swarms/models/moondream_mm.py
+-rw-r--r--   0        0        0     2881 2024-05-18 16:58:15.348268 swarms-5.0.3/swarms/models/nougat.py
+-rw-r--r--   0        0        0     2366 2024-03-15 22:19:21.043550 swarms-5.0.3/swarms/models/open_dalle.py
+-rw-r--r--   0        0        0     2464 2024-04-27 21:17:36.644597 swarms-5.0.3/swarms/models/open_router.py
+-rw-r--r--   0        0        0      106 2024-04-25 14:24:46.757474 swarms-5.0.3/swarms/models/openai_embeddings.py
+-rw-r--r--   0        0        0     3167 2024-04-27 21:17:36.645494 swarms-5.0.3/swarms/models/openai_tts.py
+-rw-r--r--   0        0        0       93 2024-04-25 14:24:46.757393 swarms-5.0.3/swarms/models/palm.py
+-rw-r--r--   0        0        0     2160 2024-05-08 21:09:56.821210 swarms-5.0.3/swarms/models/popular_llms.py
+-rw-r--r--   0        0        0     4813 2024-04-18 12:43:27.720842 swarms-5.0.3/swarms/models/qwen.py
+-rw-r--r--   0        0        0     3561 2024-05-18 05:48:32.478953 swarms-5.0.3/swarms/models/sam.py
+-rw-r--r--   0        0        0    12675 2024-04-18 12:43:28.000334 swarms-5.0.3/swarms/models/sampling_params.py
+-rw-r--r--   0        0        0     7621 2024-04-18 12:43:27.738035 swarms-5.0.3/swarms/models/speecht5.py
+-rw-r--r--   0        0        0     8244 2024-04-18 12:43:28.025933 swarms-5.0.3/swarms/models/ssd_1b.py
+-rw-r--r--   0        0        0     3948 2024-04-27 21:17:36.646243 swarms-5.0.3/swarms/models/together.py
+-rw-r--r--   0        0        0      592 2024-03-15 22:19:21.054281 swarms-5.0.3/swarms/models/types.py
+-rw-r--r--   0        0        0     1731 2024-03-15 22:19:21.054977 swarms-5.0.3/swarms/models/vilt.py
+-rw-r--r--   0        0        0     2846 2024-03-15 22:19:21.055732 swarms-5.0.3/swarms/models/vip_llava.py
+-rw-r--r--   0        0        0     3666 2024-05-18 16:58:15.352844 swarms-5.0.3/swarms/models/zeroscope.py
+-rw-r--r--   0        0        0        0 2024-05-01 03:43:07.020028 swarms-5.0.3/swarms/prebuilt_swarms/__init__.py
+-rw-r--r--   0        0        0      692 2024-05-08 21:09:56.824718 swarms-5.0.3/swarms/prompts/__init__.py
+-rw-r--r--   0        0        0    11320 2024-03-15 22:19:21.061563 swarms-5.0.3/swarms/prompts/accountant_swarm_prompts.py
+-rw-r--r--   0        0        0     9156 2024-03-15 22:19:21.062133 swarms-5.0.3/swarms/prompts/aga.py
+-rw-r--r--   0        0        0     1451 2024-03-15 22:19:21.062911 swarms-5.0.3/swarms/prompts/agent_output_parser.py
+-rw-r--r--   0        0        0     2705 2024-04-18 12:43:28.068653 swarms-5.0.3/swarms/prompts/agent_prompt.py
+-rw-r--r--   0        0        0     6886 2024-03-15 22:19:21.064160 swarms-5.0.3/swarms/prompts/agent_prompts.py
+-rw-r--r--   0        0        0     7113 2024-05-08 21:09:56.832506 swarms-5.0.3/swarms/prompts/agent_system_prompts.py
+-rw-r--r--   0        0        0     5233 2024-03-15 22:19:21.065787 swarms-5.0.3/swarms/prompts/ai_research_team.py
+-rw-r--r--   0        0        0     1148 2024-05-01 03:43:07.021040 swarms-5.0.3/swarms/prompts/aot_prompt.py
+-rw-r--r--   0        0        0    13981 2024-03-15 22:19:21.066513 swarms-5.0.3/swarms/prompts/autobloggen.py
+-rw-r--r--   0        0        0     5605 2024-03-15 22:19:21.068224 swarms-5.0.3/swarms/prompts/autoswarm.py
+-rw-r--r--   0        0        0     7542 2024-04-18 12:43:28.353296 swarms-5.0.3/swarms/prompts/base.py
+-rw-r--r--   0        0        0     3801 2024-04-18 12:43:28.227538 swarms-5.0.3/swarms/prompts/chat_prompt.py
+-rw-r--r--   0        0        0     2235 2024-03-15 22:19:21.069096 swarms-5.0.3/swarms/prompts/code_interpreter.py
+-rw-r--r--   0        0        0     4106 2024-03-15 22:19:21.069652 swarms-5.0.3/swarms/prompts/code_spawner.py
+-rw-r--r--   0        0        0     1566 2024-03-15 22:19:21.069820 swarms-5.0.3/swarms/prompts/debate.py
+-rw-r--r--   0        0        0     7152 2024-05-18 17:23:48.186668 swarms-5.0.3/swarms/prompts/documentation.py
+-rw-r--r--   0        0        0     1767 2024-03-15 22:19:21.071442 swarms-5.0.3/swarms/prompts/education.py
+-rw-r--r--   0        0        0     4180 2024-03-15 22:19:21.071791 swarms-5.0.3/swarms/prompts/finance_agent_prompt.py
+-rw-r--r--   0        0        0     4117 2024-03-15 22:19:21.072144 swarms-5.0.3/swarms/prompts/growth_agent_prompt.py
+-rw-r--r--   0        0        0      880 2024-03-15 22:19:21.072694 swarms-5.0.3/swarms/prompts/idea2img.py
+-rw-r--r--   0        0        0     3346 2024-03-15 22:19:21.072990 swarms-5.0.3/swarms/prompts/legal_agent_prompt.py
+-rw-r--r--   0        0        0     4785 2024-03-15 22:19:21.073912 swarms-5.0.3/swarms/prompts/logistics.py
+-rw-r--r--   0        0        0     3374 2024-04-10 15:42:56.140463 swarms-5.0.3/swarms/prompts/meta_system_prompt.py
+-rw-r--r--   0        0        0    10662 2024-03-15 22:19:21.074621 swarms-5.0.3/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
+-rw-r--r--   0        0        0     3511 2024-03-15 22:19:21.075295 swarms-5.0.3/swarms/prompts/multi_modal_prompts.py
+-rw-r--r--   0        0        0     3225 2024-03-15 22:19:21.075646 swarms-5.0.3/swarms/prompts/multi_modal_visual_prompts.py
+-rw-r--r--   0        0        0     3454 2024-03-15 22:19:21.076012 swarms-5.0.3/swarms/prompts/operations_agent_prompt.py
+-rw-r--r--   0        0        0     2149 2024-03-15 22:19:21.076733 swarms-5.0.3/swarms/prompts/personal_stylist.py
+-rw-r--r--   0        0        0     8333 2024-03-15 22:19:21.077280 swarms-5.0.3/swarms/prompts/product_agent_prompt.py
+-rw-r--r--   0        0        0    10144 2024-03-15 22:19:21.078026 swarms-5.0.3/swarms/prompts/programming.py
+-rw-r--r--   0        0        0     2128 2024-03-15 22:19:21.078275 swarms-5.0.3/swarms/prompts/project_manager.py
+-rw-r--r--   0        0        0    13215 2024-04-18 12:43:28.152390 swarms-5.0.3/swarms/prompts/python.py
+-rw-r--r--   0        0        0     2960 2024-03-15 22:19:21.079805 swarms-5.0.3/swarms/prompts/react.py
+-rw-r--r--   0        0        0        0 2024-03-15 22:19:21.080059 swarms-5.0.3/swarms/prompts/refiner_agent_prompt.py
+-rw-r--r--   0        0        0     5126 2024-03-15 22:19:21.080659 swarms-5.0.3/swarms/prompts/sales.py
+-rw-r--r--   0        0        0     5013 2024-03-15 22:19:21.081280 swarms-5.0.3/swarms/prompts/sales_prompts.py
+-rw-r--r--   0        0        0     2679 2024-03-15 22:19:21.083072 swarms-5.0.3/swarms/prompts/security_team.py
+-rw-r--r--   0        0        0     3252 2024-04-18 12:43:28.128596 swarms-5.0.3/swarms/prompts/self_operating_prompt.py
+-rw-r--r--   0        0        0     4147 2024-03-15 22:19:21.084066 swarms-5.0.3/swarms/prompts/sop_generator_agent_prompt.py
+-rw-r--r--   0        0        0     4640 2024-03-15 22:19:21.084386 swarms-5.0.3/swarms/prompts/summaries_prompts.py
+-rw-r--r--   0        0        0     3984 2024-03-15 22:19:21.084631 swarms-5.0.3/swarms/prompts/support_agent_prompt.py
+-rw-r--r--   0        0        0     4280 2024-03-15 22:19:21.085244 swarms-5.0.3/swarms/prompts/swarm_manager_agent.py
+-rw-r--r--   0        0        0      728 2024-03-15 22:19:21.085725 swarms-5.0.3/swarms/prompts/task_assignment_prompt.py
+-rw-r--r--   0        0        0     4271 2024-04-18 12:43:28.167424 swarms-5.0.3/swarms/prompts/tests.py
+-rw-r--r--   0        0        0     4288 2024-03-15 22:19:21.086625 swarms-5.0.3/swarms/prompts/tools.py
+-rw-r--r--   0        0        0     2398 2024-03-15 22:19:21.087352 swarms-5.0.3/swarms/prompts/urban_planning.py
+-rw-r--r--   0        0        0     3675 2024-03-15 22:19:21.087654 swarms-5.0.3/swarms/prompts/visual_cot.py
+-rw-r--r--   0        0        0     5554 2024-05-19 03:25:09.324726 swarms-5.0.3/swarms/prompts/worker_prompt.py
+-rw-r--r--   0        0        0     2349 2024-03-15 22:19:21.088382 swarms-5.0.3/swarms/prompts/xray_swarm_prompt.py
+-rw-r--r--   0        0        0     4152 2024-05-19 03:30:07.885255 swarms-5.0.3/swarms/structs/__init__.py
+-rw-r--r--   0        0        0    60110 2024-05-16 20:36:45.500176 swarms-5.0.3/swarms/structs/agent.py
+-rw-r--r--   0        0        0      574 2024-03-15 22:19:21.092491 swarms-5.0.3/swarms/structs/agent_job.py
+-rw-r--r--   0        0        0     2937 2024-04-22 15:42:05.980151 swarms-5.0.3/swarms/structs/agent_process.py
+-rw-r--r--   0        0        0     3718 2024-04-18 12:43:28.377820 swarms-5.0.3/swarms/structs/async_workflow.py
+-rw-r--r--   0        0        0     5579 2024-04-22 14:27:36.702871 swarms-5.0.3/swarms/structs/auto_swarm.py
+-rw-r--r--   0        0        0    12437 2024-04-23 01:08:13.052177 swarms-5.0.3/swarms/structs/base_structure.py
+-rw-r--r--   0        0        0    19446 2024-05-08 21:09:56.884181 swarms-5.0.3/swarms/structs/base_swarm.py
+-rw-r--r--   0        0        0    12161 2024-05-08 21:09:56.888358 swarms-5.0.3/swarms/structs/base_workflow.py
+-rw-r--r--   0        0        0     1056 2024-03-15 22:19:21.095125 swarms-5.0.3/swarms/structs/block_wrapper.py
+-rw-r--r--   0        0        0     3188 2024-04-18 02:05:51.225713 swarms-5.0.3/swarms/structs/blocks_dict.py
+-rw-r--r--   0        0        0     4851 2024-04-18 12:43:28.719057 swarms-5.0.3/swarms/structs/blocks_list.py
+-rw-r--r--   0        0        0     5206 2024-04-18 12:43:28.754865 swarms-5.0.3/swarms/structs/company.py
+-rw-r--r--   0        0        0     4471 2024-04-18 12:43:28.724904 swarms-5.0.3/swarms/structs/concurrent_workflow.py
+-rw-r--r--   0        0        0    14685 2024-04-26 04:55:42.709791 swarms-5.0.3/swarms/structs/conversation.py
+-rw-r--r--   0        0        0    12549 2024-04-18 12:43:29.326347 swarms-5.0.3/swarms/structs/debate.py
+-rw-r--r--   0        0        0     3041 2024-03-15 22:19:21.099360 swarms-5.0.3/swarms/structs/document.py
+-rw-r--r--   0        0        0     4775 2024-04-26 04:55:42.710484 swarms-5.0.3/swarms/structs/groupchat.py
+-rw-r--r--   0        0        0     3699 2024-05-19 03:27:26.615693 swarms-5.0.3/swarms/structs/hiearchical_swarm.py
+-rw-r--r--   0        0        0     4545 2024-03-15 22:19:21.101122 swarms-5.0.3/swarms/structs/long_swarm.py
+-rw-r--r--   0        0        0     7012 2024-04-18 12:43:29.037949 swarms-5.0.3/swarms/structs/majority_voting.py
+-rw-r--r--   0        0        0      745 2024-04-22 15:59:38.669639 swarms-5.0.3/swarms/structs/message.py
+-rw-r--r--   0        0        0     7338 2024-04-18 12:43:29.012263 swarms-5.0.3/swarms/structs/message_pool.py
+-rw-r--r--   0        0        0      855 2024-04-27 21:17:36.650763 swarms-5.0.3/swarms/structs/meta_system_prompt.py
+-rw-r--r--   0        0        0     5751 2024-04-18 12:43:29.210773 swarms-5.0.3/swarms/structs/model_parallizer.py
+-rw-r--r--   0        0        0     8390 2024-04-22 15:59:38.738279 swarms-5.0.3/swarms/structs/multi_agent_collab.py
+-rw-r--r--   0        0        0     5623 2024-04-18 12:43:29.243594 swarms-5.0.3/swarms/structs/multi_process_workflow.py
+-rw-r--r--   0        0        0     5272 2024-04-18 12:42:41.990321 swarms-5.0.3/swarms/structs/multi_threaded_workflow.py
+-rw-r--r--   0        0        0      371 2024-05-16 00:24:04.336048 swarms-5.0.3/swarms/structs/omni_agent_types.py
+-rw-r--r--   0        0        0      182 2024-04-28 21:24:54.081857 swarms-5.0.3/swarms/structs/plan.py
+-rw-r--r--   0        0        0    11353 2024-05-16 01:32:38.721849 swarms-5.0.3/swarms/structs/rearrange.py
+-rw-r--r--   0        0        0     2727 2024-04-18 12:42:41.946623 swarms-5.0.3/swarms/structs/recursive_workflow.py
+-rw-r--r--   0        0        0     3256 2024-05-13 20:15:02.129223 swarms-5.0.3/swarms/structs/round_robin.py
+-rw-r--r--   0        0        0     6764 2024-04-23 01:17:51.964275 swarms-5.0.3/swarms/structs/schemas.py
+-rw-r--r--   0        0        0     2956 2024-05-08 21:09:56.891925 swarms-5.0.3/swarms/structs/sequential_workflow.py
+-rw-r--r--   0        0        0     2337 2024-03-27 19:47:31.068657 swarms-5.0.3/swarms/structs/sermon_swarm.py
+-rw-r--r--   0        0        0      709 2024-05-08 21:09:56.895373 swarms-5.0.3/swarms/structs/step.py
+-rw-r--r--   0        0        0    10684 2024-04-18 12:43:29.602325 swarms-5.0.3/swarms/structs/swarm_net.py
+-rw-r--r--   0        0        0     6426 2024-04-18 12:43:29.666155 swarms-5.0.3/swarms/structs/swarming_architectures.py
+-rw-r--r--   0        0        0     8179 2024-04-18 12:43:29.569178 swarms-5.0.3/swarms/structs/task.py
+-rw-r--r--   0        0        0     1989 2024-03-27 19:12:09.705030 swarms-5.0.3/swarms/structs/task_queue_base.py
+-rw-r--r--   0        0        0     3511 2024-04-18 12:42:42.279735 swarms-5.0.3/swarms/structs/utils.py
+-rw-r--r--   0        0        0     7403 2024-04-24 00:20:16.136940 swarms-5.0.3/swarms/structs/yaml_model.py
+-rw-r--r--   0        0        0      891 2024-03-27 19:12:09.674045 swarms-5.0.3/swarms/telemetry/__init__.py
+-rw-r--r--   0        0        0      513 2024-04-18 12:43:29.468850 swarms-5.0.3/swarms/telemetry/auto_upgrade_swarms.py
+-rw-r--r--   0        0        0      385 2024-04-02 02:30:28.437471 swarms-5.0.3/swarms/telemetry/bootup.py
+-rw-r--r--   0        0        0     1073 2024-04-18 12:42:42.280090 swarms-5.0.3/swarms/telemetry/check_update.py
+-rw-r--r--   0        0        0      807 2024-03-15 22:19:21.114471 swarms-5.0.3/swarms/telemetry/log_all.py
+-rw-r--r--   0        0        0      496 2024-03-22 00:42:19.696403 swarms-5.0.3/swarms/telemetry/sentry_active.py
+-rw-r--r--   0        0        0     2675 2024-04-23 23:56:19.053195 swarms-5.0.3/swarms/telemetry/sys_info.py
+-rw-r--r--   0        0        0     1879 2024-04-24 21:57:07.051275 swarms-5.0.3/swarms/telemetry/user_utils.py
+-rw-r--r--   0        0        0     1680 2024-05-08 21:09:56.899526 swarms-5.0.3/swarms/tools/__init__.py
+-rw-r--r--   0        0        0    12525 2024-05-08 21:09:56.906505 swarms-5.0.3/swarms/tools/base_tool.py
+-rw-r--r--   0        0        0     6653 2024-04-18 12:47:32.769219 swarms-5.0.3/swarms/tools/code_interpreter.py
+-rw-r--r--   0        0        0     5367 2024-05-08 21:09:56.913861 swarms-5.0.3/swarms/tools/exec_tool.py
+-rw-r--r--   0        0        0      773 2024-04-03 12:10:21.536239 swarms-5.0.3/swarms/tools/function_util.py
+-rw-r--r--   0        0        0    14241 2024-04-27 21:17:36.654062 swarms-5.0.3/swarms/tools/json_former.py
+-rw-r--r--   0        0        0     1316 2024-03-21 23:46:38.581600 swarms-5.0.3/swarms/tools/json_utils.py
+-rw-r--r--   0        0        0     2455 2024-04-18 12:42:42.475166 swarms-5.0.3/swarms/tools/logits_processor.py
+-rw-r--r--   0        0        0     1461 2024-04-18 12:43:30.100050 swarms-5.0.3/swarms/tools/math_eval.py
+-rw-r--r--   0        0        0      978 2024-04-23 23:18:25.950155 swarms-5.0.3/swarms/tools/openai_func_calling_schema.py
+-rw-r--r--   0        0        0    13875 2024-05-08 21:09:56.921184 swarms-5.0.3/swarms/tools/openai_tool_creator_decorator.py
+-rw-r--r--   0        0        0    15564 2024-04-27 21:17:36.657668 swarms-5.0.3/swarms/tools/py_func_to_openai_func_str.py
+-rw-r--r--   0        0        0     4275 2024-05-08 21:09:56.925611 swarms-5.0.3/swarms/tools/pydantic_to_json.py
+-rw-r--r--   0        0        0      157 2024-03-24 04:12:12.223834 swarms-5.0.3/swarms/tools/tool.py
+-rw-r--r--   0        0        0     6170 2024-05-08 21:09:56.930060 swarms-5.0.3/swarms/tools/tool_utils.py
+-rw-r--r--   0        0        0     5466 2024-03-15 22:19:21.122024 swarms-5.0.3/swarms/utils/README.md
+-rw-r--r--   0        0        0     1956 2024-04-18 15:06:06.195732 swarms-5.0.3/swarms/utils/__init__.py
+-rw-r--r--   0        0        0     3507 2024-04-18 12:42:42.565998 swarms-5.0.3/swarms/utils/apa.py
+-rw-r--r--   0        0        0     6065 2024-04-18 12:42:42.646659 swarms-5.0.3/swarms/utils/check_function_result.py
+-rw-r--r--   0        0        0     1008 2024-03-15 22:19:21.124143 swarms-5.0.3/swarms/utils/class_args_wrapper.py
+-rw-r--r--   0        0        0     1234 2024-04-18 12:42:42.478906 swarms-5.0.3/swarms/utils/concurrent_utils.py
+-rw-r--r--   0        0        0     1865 2024-04-18 12:42:42.546898 swarms-5.0.3/swarms/utils/data_to_text.py
+-rw-r--r--   0        0        0     2451 2024-04-18 12:43:29.983708 swarms-5.0.3/swarms/utils/decorators.py
+-rw-r--r--   0        0        0     1311 2024-03-15 22:19:21.127902 swarms-5.0.3/swarms/utils/disable_logging.py
+-rw-r--r--   0        0        0      890 2024-03-15 22:19:21.128555 swarms-5.0.3/swarms/utils/download_img.py
+-rw-r--r--   0        0        0     1127 2024-03-15 22:19:21.129540 swarms-5.0.3/swarms/utils/execute_futures.py
+-rw-r--r--   0        0        0     1113 2024-03-15 22:19:21.130281 swarms-5.0.3/swarms/utils/exponential_backoff.py
+-rw-r--r--   0        0        0      854 2024-03-15 22:19:21.130759 swarms-5.0.3/swarms/utils/fetch_init_params.py
+-rw-r--r--   0        0        0      500 2024-03-15 22:19:21.131255 swarms-5.0.3/swarms/utils/file_extension_seach.py
+-rw-r--r--   0        0        0     3266 2024-04-18 12:42:42.739802 swarms-5.0.3/swarms/utils/file_processing.py
+-rw-r--r--   0        0        0      630 2024-04-18 12:43:29.910068 swarms-5.0.3/swarms/utils/find_img_path.py
+-rw-r--r--   0        0        0     4184 2024-04-18 12:43:30.069758 swarms-5.0.3/swarms/utils/get_logger.py
+-rw-r--r--   0        0        0     4232 2024-05-17 00:01:56.878497 swarms-5.0.3/swarms/utils/get_total_gpus.py
+-rw-r--r--   0        0        0     2848 2024-04-18 12:43:30.028262 swarms-5.0.3/swarms/utils/json_output_parser.py
+-rw-r--r--   0        0        0     1831 2024-04-18 12:42:42.783557 swarms-5.0.3/swarms/utils/jsonl_utils.py
+-rw-r--r--   0        0        0      932 2024-03-15 22:19:21.135261 swarms-5.0.3/swarms/utils/llm_metrics_decorator.py
+-rw-r--r--   0        0        0     2209 2024-04-18 12:43:30.070521 swarms-5.0.3/swarms/utils/logger.py
+-rw-r--r--   0        0        0    16186 2024-04-18 12:43:30.846131 swarms-5.0.3/swarms/utils/loggers.py
+-rw-r--r--   0        0        0      453 2024-03-27 19:12:09.738695 swarms-5.0.3/swarms/utils/loguru_logger.py
+-rw-r--r--   0        0        0      711 2024-03-27 19:12:09.676603 swarms-5.0.3/swarms/utils/markdown_message.py
+-rw-r--r--   0        0        0      600 2024-03-15 22:19:21.139501 swarms-5.0.3/swarms/utils/parse_code.py
+-rw-r--r--   0        0        0     1177 2024-04-18 12:43:30.100653 swarms-5.0.3/swarms/utils/pdf_to_text.py
+-rw-r--r--   0        0        0     1353 2024-03-15 22:19:21.141276 swarms-5.0.3/swarms/utils/remove_json_whitespace.py
+-rw-r--r--   0        0        0     1278 2024-04-18 12:42:42.936792 swarms-5.0.3/swarms/utils/save_logs.py
+-rw-r--r--   0        0        0     4774 2024-04-18 12:42:43.138354 swarms-5.0.3/swarms/utils/serializable.py
+-rw-r--r--   0        0        0     1315 2024-04-25 14:49:22.838126 swarms-5.0.3/swarms/utils/try_except_wrapper.py
+-rw-r--r--   0        0        0     2668 2024-04-18 12:43:30.304280 swarms-5.0.3/swarms/utils/yaml_output_parser.py
+-rw-r--r--   0        0        0    40527 1970-01-01 00:00:00.000000 swarms-5.0.3/setup.py
+-rw-r--r--   0        0        0    39413 1970-01-01 00:00:00.000000 swarms-5.0.3/PKG-INFO
```

### Comparing `swarms-5.0.1/LICENSE` & `swarms-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/README.md` & `swarms-5.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1166,15 +1166,15 @@
 # Run the AutoSwarm
 autoswarm.run("Analyze these financial data and give me a summary")
 
 
 ```
 
 ## `AgentRearrange`
-Inspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships
+Inspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships. [Docs Available:](https://swarms.apac.ai/en/latest/swarms/structs/agent_rearrange/)
 
 ```python
 from swarms import Agent, AgentRearrange, rearrange, Anthropic
 
 
 # Initialize the director agent
 
@@ -1252,14 +1252,33 @@
 ---
 
 ## Documentation
 Documentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)
 
 ----
 
+## File Structure
+The swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs` that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.
+
+```sh
+├── __init__.py
+├── agents
+├── artifacts
+├── memory
+├── models
+├── prompts
+├── structs
+├── telemetry
+├── tools
+├── utils
+└── workers
+```
+
+----
+
 ## 🫶 Contributions:
 
 The easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)
 
 Swarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!
 
 <a href="https://github.com/kyegomez/swarms/graphs/contributors">
@@ -1282,66 +1301,22 @@
 
 ---
 
 ## Discovery Call
 Book a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)
 
 
-
 ## Accelerate Backlog
-Help us accelerate our backlog by supporting us financially! Note, we're an open source corporation and so all the revenue we generate is through donations at the moment ;)
+Accelerate Bugs, Features, and Demos to implement by supporting us here:
 
 <a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>
 
 
-## File Structure
-The swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs` that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.
-
-```sh
-├── __init__.py
-├── agents
-├── artifacts
-├── chunkers
-├── cli
-├── loaders
-├── memory
-├── models
-├── prompts
-├── structs
-├── telemetry
-├── tokenizers
-├── tools
-├── utils
-└── workers
-```
-
 ## Docker Instructions
-
-This application uses Docker with CUDA support. To build and run the Docker container, follow these steps:
-
-### Prerequisites
-
-- Make sure you have [Docker installed](https://docs.docker.com/get-docker/) on your machine.
-- Ensure your machine has an NVIDIA GPU and [NVIDIA Docker support](https://github.com/NVIDIA/nvidia-docker) installed.
-
-### Building the Docker Image
-
-To build the Docker image, navigate to the root directory containing the `Dockerfile` and run the following command:
-
-```bash
-docker build --gpus all -t swarms
-``` 
-### Running the Docker Container
-To run the Docker container, use the following command:
-
-`docker run --gpus all -p 4000:80 swarms`
-
-Replace swarms with the name of your Docker image, and replace 4000:80 with your actual port mapping. The format is hostPort:containerPort.
-
-Now, your application should be running with CUDA support!
+- [Learn More Here About Deployments In Docker]()
 
 
 ## Swarm Newsletter 🤖 🤖 🤖 📧 
 Sign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊
 
 
 [CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)
```

### Comparing `swarms-5.0.1/pyproject.toml` & `swarms-5.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "swarms"
-version = "5.0.1"
+version = "5.0.3"
 description = "Swarms - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/swarms"
 documentation = "https://swarms.world"
 readme = "README.md"
 repository = "https://github.com/kyegomez/swarms"
@@ -44,16 +44,15 @@
 loguru = "0.7.2"
 pydantic = "2.7.1"
 tenacity = "8.2.3"
 Pillow = "10.3.0"
 psutil = "*"
 sentry-sdk = "*"
 python-dotenv = "*"
-accelerate = "0.28.0"
-opencv-python = "^4.9.0.80"
+opencv-python-headless = "*"
 PyYAML = "*"
 docstring_parser = "0.16"
 
 [tool.poetry.group.lint.dependencies]
 black = ">=23.1,<25.0"
 ruff = ">=0.0.249,<0.4.3"
 types-toml = "^0.10.8.1"
```

### Comparing `swarms-5.0.1/swarms/__init__.py` & `swarms-5.0.3/swarms/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/agents/__init__.py` & `swarms-5.0.3/swarms/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/agents/agent_wrapper.py` & `swarms-5.0.3/swarms/agents/agent_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/agents/base.py` & `swarms-5.0.3/swarms/agents/base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/agents/developer_agents.py` & `swarms-5.0.3/swarms/agents/developer_agents.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/agents/omni_modal_agent.py` & `swarms-5.0.3/swarms/agents/omni_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/agents/simple_agent.py` & `swarms-5.0.3/swarms/agents/simple_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/agents/tool_agent.py` & `swarms-5.0.3/swarms/agents/tool_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/agents/worker_agent.py` & `swarms-5.0.3/swarms/agents/worker_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/artifacts/base_artifact.py` & `swarms-5.0.3/swarms/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/artifacts/text_artifact.py` & `swarms-5.0.3/swarms/artifacts/text_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/memory/__init__.py` & `swarms-5.0.3/swarms/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/memory/base_db.py` & `swarms-5.0.3/swarms/memory/base_db.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/memory/base_vectordb.py` & `swarms-5.0.3/swarms/memory/base_vectordb.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/memory/dict_internal_memory.py` & `swarms-5.0.3/swarms/memory/dict_internal_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/memory/dict_shared_memory.py` & `swarms-5.0.3/swarms/memory/dict_shared_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/memory/short_term_memory.py` & `swarms-5.0.3/swarms/memory/short_term_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/memory/visual_memory.py` & `swarms-5.0.3/swarms/memory/visual_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/__init__.py` & `swarms-5.0.3/swarms/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from swarms.models.base_embedding_model import BaseEmbeddingModel
 from swarms.models.base_llm import BaseLLM  # noqa: E402
 from swarms.models.base_multimodal_model import BaseMultiModalModel
-from swarms.models.fire_function import FireFunctionCaller
 from swarms.models.fuyu import Fuyu  # noqa: E402
 from swarms.models.gpt4_vision_api import GPT4VisionAPI  # noqa: E402
 from swarms.models.huggingface import HuggingfaceLLM  # noqa: E402
 from swarms.models.idefics import Idefics  # noqa: E402
 from swarms.models.kosmos_two import Kosmos  # noqa: E402
 from swarms.models.layoutlm_document_qa import LayoutLMDocumentQA
 from swarms.models.llava import LavaMultiModal  # noqa: E402
 from swarms.models.mistral import Mistral  # noqa: E402
 from swarms.models.mixtral import Mixtral  # noqa: E402
-from swarms.models.mpt import MPT7B  # noqa: E402
 from swarms.models.nougat import Nougat  # noqa: E402
 from swarms.models.palm import GooglePalm as Palm  # noqa: E402
 from swarms.models.openai_tts import OpenAITTS  # noqa: E402
 from swarms.models.popular_llms import Anthropic as Anthropic
 from swarms.models.popular_llms import (
     AzureOpenAILLM as AzureOpenAI,
 )
@@ -38,45 +36,45 @@
     ImageModality,
     MultimodalData,
     TextModality,
     VideoModality,
 )
 from swarms.models.vilt import Vilt  # noqa: E402
 from swarms.models.openai_embeddings import OpenAIEmbeddings
+from swarms.models.llama3_hosted import llama3Hosted
 
 __all__ = [
-    "BaseLLM",
-    "Anthropic",
-    "AzureOpenAI",
     "BaseEmbeddingModel",
+    "BaseLLM",
     "BaseMultiModalModel",
-    "Cohere",
-    "FireFunctionCaller",
     "Fuyu",
     "GPT4VisionAPI",
     "HuggingfaceLLM",
     "Idefics",
     "Kosmos",
     "LayoutLMDocumentQA",
     "LavaMultiModal",
     "Mistral",
     "Mixtral",
-    "MPT7B",
     "Nougat",
-    "OpenAI",
-    "OpenAIChat",
-    "OpenAIEmbeddings",
+    "Palm",
     "OpenAITTS",
+    "Anthropic",
+    "AzureOpenAI",
+    "Cohere",
+    "OpenAIChat",
+    "OpenAI",
     "OctoAIChat",
-    "Palm",
     "QwenVLMultiModal",
     "Replicate",
     "SamplingParams",
     "SamplingType",
-    "TextModality",
-    "MultimodalData",
-    "ImageModality",
+    "TogetherLLM",
     "AudioModality",
+    "ImageModality",
+    "MultimodalData",
+    "TextModality",
     "VideoModality",
-    "TogetherLLM",
     "Vilt",
+    "OpenAIEmbeddings",
+    "llama3Hosted",
 ]
```

### Comparing `swarms-5.0.1/swarms/models/base_embedding_model.py` & `swarms-5.0.3/swarms/models/base_embedding_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/base_llm.py` & `swarms-5.0.3/swarms/models/base_llm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/base_multimodal_model.py` & `swarms-5.0.3/swarms/models/base_multimodal_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/base_tts.py` & `swarms-5.0.3/swarms/models/base_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/base_ttv.py` & `swarms-5.0.3/swarms/models/base_ttv.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/cog_vlm.py` & `swarms-5.0.3/swarms/models/cog_vlm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/dalle3.py` & `swarms-5.0.3/swarms/models/dalle3.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/distilled_whisperx.py` & `swarms-5.0.3/swarms/models/distilled_whisperx.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/embeddings_base.py` & `swarms-5.0.3/swarms/models/embeddings_base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/fire_function.py` & `swarms-5.0.3/swarms/models/fire_function.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/fuyu.py` & `swarms-5.0.3/swarms/models/fuyu.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/gemini.py` & `swarms-5.0.3/swarms/models/gemini.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/gpt4_vision_api.py` & `swarms-5.0.3/swarms/models/gpt4_vision_api.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/huggingface.py` & `swarms-5.0.3/swarms/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/huggingface_pipeline.py` & `swarms-5.0.3/swarms/models/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/idefics.py` & `swarms-5.0.3/swarms/models/idefics.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/kosmos_two.py` & `swarms-5.0.3/swarms/models/kosmos_two.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/layoutlm_document_qa.py` & `swarms-5.0.3/swarms/models/layoutlm_document_qa.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/llama_function_caller.py` & `swarms-5.0.3/swarms/models/llama_function_caller.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/llava.py` & `swarms-5.0.3/swarms/models/llava.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/mistral.py` & `swarms-5.0.3/swarms/models/mistral.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/mixtral.py` & `swarms-5.0.3/swarms/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/moondream_mm.py` & `swarms-5.0.3/swarms/models/moondream_mm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/nougat.py` & `swarms-5.0.3/swarms/models/nougat.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,26 +56,28 @@
         """Get an image from a path"""
         img = Image.open(img)
 
         if img.mode == "L":
             img = img.convert("RGB")
         return img
 
-    def __call__(self, img: str):
+    def __call__(self, img: str, *args, **kwargs):
         """Call the model with an image_path str as an input"""
         image = Image.open(img)
         pixel_values = self.processor(
             image, return_tensors="pt"
         ).pixel_values
 
         # Generate transcriptions, here we only generate 30 tokens
         outputs = self.model.generate(
             pixel_values.to(self.device),
             min_length=self.min_length,
             max_new_tokens=self.max_new_tokens,
+            *args,
+            **kwargs,
         )
 
         sequence = self.processor.batch_decode(
             outputs, skip_special_tokens=True
         )[0]
         sequence = self.processor.post_process_generation(
             sequence, fix_markdown=False
```

### Comparing `swarms-5.0.1/swarms/models/open_dalle.py` & `swarms-5.0.3/swarms/models/open_dalle.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/open_router.py` & `swarms-5.0.3/swarms/models/open_router.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/openai_tts.py` & `swarms-5.0.3/swarms/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/popular_llms.py` & `swarms-5.0.3/swarms/models/popular_llms.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/qwen.py` & `swarms-5.0.3/swarms/models/qwen.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/sam.py` & `swarms-5.0.3/swarms/models/sam.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         self.model = SamModel.from_pretrained(
             model_name, *args, **kwargs
         ).to(device)
 
         self.processor = SamProcessor.from_pretrained(model_name)
 
-    def run(self, task=None, img=None, *args, **kwargs):
+    def run(self, task: str = None, img: str = None, *args, **kwargs):
         """
         Runs the SAM model on the given image and returns the segmentation scores and masks.
 
         Args:
             task: The task to perform. Not used in this method.
             img: The input image to segment.
             *args: Additional positional arguments.
```

### Comparing `swarms-5.0.1/swarms/models/sampling_params.py` & `swarms-5.0.3/swarms/models/sampling_params.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/speecht5.py` & `swarms-5.0.3/swarms/models/speecht5.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/ssd_1b.py` & `swarms-5.0.3/swarms/models/ssd_1b.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/together.py` & `swarms-5.0.3/swarms/models/together.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/types.py` & `swarms-5.0.3/swarms/models/types.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/vilt.py` & `swarms-5.0.3/swarms/models/vilt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/vip_llava.py` & `swarms-5.0.3/swarms/models/vip_llava.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/models/zeroscope.py` & `swarms-5.0.3/swarms/models/zeroscope.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,15 @@
         self.dim = dim
         self.num_inference_steps = num_inference_steps
         self.height = height
         self.width = width
         self.num_frames = num_frames
 
         self.pipe = DiffusionPipeline.from_pretrained(
-            model_name,
-            torch_dtype=torch_dtype,
-            *args,
+            model_name, torch_dtype=torch_dtype, *args, **kwargs
         )
         self.pipe.scheduler = DPMSolverMultistepScheduler(
             self.pipe.scheduler.config,
         )
         self.pipe_enable_model_cpu_offload()
         self.pipe.enable_vae_slicing()
         self.pipe.unet.enable_forward_chunking(
```

### Comparing `swarms-5.0.1/swarms/prompts/__init__.py` & `swarms-5.0.3/swarms/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/accountant_swarm_prompts.py` & `swarms-5.0.3/swarms/prompts/accountant_swarm_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/aga.py` & `swarms-5.0.3/swarms/prompts/aga.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/agent_output_parser.py` & `swarms-5.0.3/swarms/prompts/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/agent_prompt.py` & `swarms-5.0.3/swarms/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/agent_prompts.py` & `swarms-5.0.3/swarms/prompts/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/agent_system_prompts.py` & `swarms-5.0.3/swarms/prompts/agent_system_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/ai_research_team.py` & `swarms-5.0.3/swarms/prompts/ai_research_team.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/aot_prompt.py` & `swarms-5.0.3/swarms/prompts/aot_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/autobloggen.py` & `swarms-5.0.3/swarms/prompts/autobloggen.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/autoswarm.py` & `swarms-5.0.3/swarms/prompts/autoswarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/base.py` & `swarms-5.0.3/swarms/prompts/base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/chat_prompt.py` & `swarms-5.0.3/swarms/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/code_interpreter.py` & `swarms-5.0.3/swarms/prompts/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/code_spawner.py` & `swarms-5.0.3/swarms/prompts/code_spawner.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/debate.py` & `swarms-5.0.3/swarms/prompts/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/documentation.py` & `swarms-5.0.3/swarms/prompts/documentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     put the arguments and methods in a table in markdown to make it visually seamless
 
     Now make the professional documentation for this code, provide the architecture and how the class works and why it works that way,
     it's purpose, provide args, their types, 3 ways of usage examples, in examples show all the code like imports main example etc
 
     BE VERY EXPLICIT AND THOROUGH, MAKE IT DEEP AND USEFUL
 
-    ########
+    ######## INSTRUCTIONS ########
     Step 1: Understand the purpose and functionality of the module or framework
 
     Read and analyze the description provided in the documentation to understand the purpose and functionality of the module or framework.
     Identify the key features, parameters, and operations performed by the module or framework.
     Step 2: Provide an overview and introduction
 
     Start the documentation by providing a brief overview and introduction to the module or framework.
@@ -39,14 +39,15 @@
     Address any common issues or challenges that developers may encounter and provide recommendations or workarounds.
     Step 6: Include references and resources
 
     Include references to any external resources or research papers that provide further information or background on the module or framework.
     Provide links to relevant documentation or websites for further exploration.
     Example Template for the given documentation:
 
+    ################################### EXAMPLE #####################################
     # Module/Function Name: MultiheadAttention
 
     class torch.nn.MultiheadAttention(embed_dim, num_heads, dropout=0.0, bias=True, add_bias_kv=False, add_zero_attn=False, kdim=None, vdim=None, batch_first=False, device=None, dtype=None):
         ```
         Creates a multi-head attention module for joint information representation from the different subspaces.
 
         Parameters:
```

### Comparing `swarms-5.0.1/swarms/prompts/education.py` & `swarms-5.0.3/swarms/prompts/education.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/finance_agent_prompt.py` & `swarms-5.0.3/swarms/prompts/finance_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/growth_agent_prompt.py` & `swarms-5.0.3/swarms/prompts/growth_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/idea2img.py` & `swarms-5.0.3/swarms/prompts/idea2img.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/legal_agent_prompt.py` & `swarms-5.0.3/swarms/prompts/legal_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/logistics.py` & `swarms-5.0.3/swarms/prompts/logistics.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/meta_system_prompt.py` & `swarms-5.0.3/swarms/prompts/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/multi_modal_autonomous_instruction_prompt.py` & `swarms-5.0.3/swarms/prompts/multi_modal_autonomous_instruction_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/multi_modal_prompts.py` & `swarms-5.0.3/swarms/prompts/multi_modal_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/multi_modal_visual_prompts.py` & `swarms-5.0.3/swarms/prompts/multi_modal_visual_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/operations_agent_prompt.py` & `swarms-5.0.3/swarms/prompts/operations_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/personal_stylist.py` & `swarms-5.0.3/swarms/prompts/personal_stylist.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/product_agent_prompt.py` & `swarms-5.0.3/swarms/prompts/product_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/programming.py` & `swarms-5.0.3/swarms/prompts/programming.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/project_manager.py` & `swarms-5.0.3/swarms/prompts/project_manager.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/python.py` & `swarms-5.0.3/swarms/prompts/python.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/react.py` & `swarms-5.0.3/swarms/prompts/react.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/sales.py` & `swarms-5.0.3/swarms/prompts/sales.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/sales_prompts.py` & `swarms-5.0.3/swarms/prompts/sales_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/security_team.py` & `swarms-5.0.3/swarms/prompts/security_team.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/self_operating_prompt.py` & `swarms-5.0.3/swarms/prompts/self_operating_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/sop_generator_agent_prompt.py` & `swarms-5.0.3/swarms/prompts/sop_generator_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/summaries_prompts.py` & `swarms-5.0.3/swarms/prompts/summaries_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/support_agent_prompt.py` & `swarms-5.0.3/swarms/prompts/support_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/swarm_manager_agent.py` & `swarms-5.0.3/swarms/prompts/swarm_manager_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/task_assignment_prompt.py` & `swarms-5.0.3/swarms/prompts/task_assignment_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/tests.py` & `swarms-5.0.3/swarms/prompts/tests.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/tools.py` & `swarms-5.0.3/swarms/prompts/tools.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/urban_planning.py` & `swarms-5.0.3/swarms/prompts/urban_planning.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/visual_cot.py` & `swarms-5.0.3/swarms/prompts/visual_cot.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/prompts/worker_prompt.py` & `swarms-5.0.3/swarms/prompts/worker_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
+from typing import List
+
 from pydantic import BaseModel, Field
+
 from swarms.tools.base_tool import BaseTool
 from swarms.tools.tool_utils import scrape_tool_func_docs
-from typing import List
-from swarms.tools.base_tool import BaseTool
 
 time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
 
 class Thoughts(BaseModel):
     text: str = Field(..., title="Thoughts")
     reasoning: str = Field(..., title="Reasoning")
```

### Comparing `swarms-5.0.1/swarms/prompts/xray_swarm_prompt.py` & `swarms-5.0.3/swarms/prompts/xray_swarm_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/__init__.py` & `swarms-5.0.3/swarms/structs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     get_type_name,
     create_yaml_schema_from_dict,
     pydantic_type_to_yaml_schema,
     YamlModel,
 )
 from swarms.structs.message_pool import MessagePool
 from swarms.structs.round_robin import RoundRobinSwarm
+from swarms.structs.hiearchical_swarm import HiearchicalSwarm
 
 __all__ = [
     "Agent",
     "AgentJob",
     "AgentProcess",
     "AgentProcessQueue",
     "AutoSwarm",
@@ -154,8 +155,9 @@
     "get_type_name",
     "create_yaml_schema_from_dict",
     "pydantic_type_to_yaml_schema",
     "YamlModel",
     "MessagePool",
     "rearrange",
     "RoundRobinSwarm",
+    "HiearchicalSwarm"
 ]
```

### Comparing `swarms-5.0.1/swarms/structs/agent.py` & `swarms-5.0.3/swarms/structs/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,14 +235,15 @@
         algorithm_of_thoughts: bool = False,
         tree_of_thoughts: bool = False,
         tool_choice: str = "auto",
         execute_tool: bool = False,
         rules: str = None,
         planning: Optional[str] = False,
         planning_prompt: Optional[str] = None,
+        device: str = None,
         *args,
         **kwargs,
     ):
         self.id = id
         self.llm = llm
         self.template = template
         self.max_loops = max_loops
@@ -310,14 +311,15 @@
         self.chain_of_thoughts = chain_of_thoughts
         self.algorithm_of_thoughts = algorithm_of_thoughts
         self.tree_of_thoughts = tree_of_thoughts
         self.tool_choice = tool_choice
         self.execute_tool = execute_tool
         self.planning = planning
         self.planning_prompt = planning_prompt
+        self.device = device
 
         # Name
         self.name = agent_name
         self.description = agent_description
         # Agentic stuff
         self.reply = ""
         self.question = None
```

### Comparing `swarms-5.0.1/swarms/structs/agent_job.py` & `swarms-5.0.3/swarms/structs/agent_job.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/agent_process.py` & `swarms-5.0.3/swarms/structs/agent_process.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/async_workflow.py` & `swarms-5.0.3/swarms/structs/async_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/auto_swarm.py` & `swarms-5.0.3/swarms/structs/auto_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/base_structure.py` & `swarms-5.0.3/swarms/structs/base_structure.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/base_swarm.py` & `swarms-5.0.3/swarms/structs/base_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/base_workflow.py` & `swarms-5.0.3/swarms/structs/base_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/block_wrapper.py` & `swarms-5.0.3/swarms/structs/block_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/blocks_dict.py` & `swarms-5.0.3/swarms/structs/blocks_dict.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/blocks_list.py` & `swarms-5.0.3/swarms/structs/blocks_list.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/company.py` & `swarms-5.0.3/swarms/structs/company.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/concurrent_workflow.py` & `swarms-5.0.3/swarms/structs/concurrent_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/conversation.py` & `swarms-5.0.3/swarms/structs/conversation.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/debate.py` & `swarms-5.0.3/swarms/structs/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/document.py` & `swarms-5.0.3/swarms/structs/document.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/groupchat.py` & `swarms-5.0.3/swarms/structs/groupchat.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/long_swarm.py` & `swarms-5.0.3/swarms/structs/long_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/majority_voting.py` & `swarms-5.0.3/swarms/structs/majority_voting.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/message.py` & `swarms-5.0.3/swarms/structs/message.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/message_pool.py` & `swarms-5.0.3/swarms/structs/message_pool.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/meta_system_prompt.py` & `swarms-5.0.3/swarms/structs/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/model_parallizer.py` & `swarms-5.0.3/swarms/structs/model_parallizer.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/multi_agent_collab.py` & `swarms-5.0.3/swarms/structs/multi_agent_collab.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/multi_process_workflow.py` & `swarms-5.0.3/swarms/structs/multi_process_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/multi_threaded_workflow.py` & `swarms-5.0.3/swarms/structs/multi_threaded_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/recursive_workflow.py` & `swarms-5.0.3/swarms/structs/recursive_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/round_robin.py` & `swarms-5.0.3/swarms/structs/round_robin.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/schemas.py` & `swarms-5.0.3/swarms/structs/schemas.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/sequential_workflow.py` & `swarms-5.0.3/swarms/structs/sequential_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/sermon_swarm.py` & `swarms-5.0.3/swarms/structs/sermon_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/step.py` & `swarms-5.0.3/swarms/structs/step.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/swarm_net.py` & `swarms-5.0.3/swarms/structs/swarm_net.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/swarming_architectures.py` & `swarms-5.0.3/swarms/structs/swarming_architectures.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/task.py` & `swarms-5.0.3/swarms/structs/task.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/task_queue_base.py` & `swarms-5.0.3/swarms/structs/task_queue_base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/utils.py` & `swarms-5.0.3/swarms/structs/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/structs/yaml_model.py` & `swarms-5.0.3/swarms/structs/yaml_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/telemetry/__init__.py` & `swarms-5.0.3/swarms/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/telemetry/auto_upgrade_swarms.py` & `swarms-5.0.3/swarms/telemetry/auto_upgrade_swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/telemetry/check_update.py` & `swarms-5.0.3/swarms/telemetry/check_update.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/telemetry/log_all.py` & `swarms-5.0.3/swarms/telemetry/log_all.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/telemetry/sys_info.py` & `swarms-5.0.3/swarms/telemetry/sys_info.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/telemetry/user_utils.py` & `swarms-5.0.3/swarms/telemetry/user_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/__init__.py` & `swarms-5.0.3/swarms/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/base_tool.py` & `swarms-5.0.3/swarms/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/code_interpreter.py` & `swarms-5.0.3/swarms/tools/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/exec_tool.py` & `swarms-5.0.3/swarms/tools/exec_tool.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/function_util.py` & `swarms-5.0.3/swarms/tools/function_util.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/json_former.py` & `swarms-5.0.3/swarms/tools/json_former.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/json_utils.py` & `swarms-5.0.3/swarms/tools/json_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/logits_processor.py` & `swarms-5.0.3/swarms/tools/logits_processor.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/math_eval.py` & `swarms-5.0.3/swarms/tools/math_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/openai_func_calling_schema.py` & `swarms-5.0.3/swarms/tools/openai_func_calling_schema.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/openai_tool_creator_decorator.py` & `swarms-5.0.3/swarms/tools/openai_tool_creator_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/py_func_to_openai_func_str.py` & `swarms-5.0.3/swarms/tools/py_func_to_openai_func_str.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/pydantic_to_json.py` & `swarms-5.0.3/swarms/tools/pydantic_to_json.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/tools/tool_utils.py` & `swarms-5.0.3/swarms/tools/tool_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/README.md` & `swarms-5.0.3/swarms/utils/README.md`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/__init__.py` & `swarms-5.0.3/swarms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/apa.py` & `swarms-5.0.3/swarms/utils/apa.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/check_function_result.py` & `swarms-5.0.3/swarms/utils/check_function_result.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/class_args_wrapper.py` & `swarms-5.0.3/swarms/utils/class_args_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/concurrent_utils.py` & `swarms-5.0.3/swarms/utils/concurrent_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/data_to_text.py` & `swarms-5.0.3/swarms/utils/data_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/decorators.py` & `swarms-5.0.3/swarms/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/disable_logging.py` & `swarms-5.0.3/swarms/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/download_img.py` & `swarms-5.0.3/swarms/utils/download_img.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/execute_futures.py` & `swarms-5.0.3/swarms/utils/execute_futures.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/exponential_backoff.py` & `swarms-5.0.3/swarms/utils/exponential_backoff.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/fetch_init_params.py` & `swarms-5.0.3/swarms/utils/fetch_init_params.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/file_processing.py` & `swarms-5.0.3/swarms/utils/file_processing.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/find_img_path.py` & `swarms-5.0.3/swarms/utils/find_img_path.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/get_logger.py` & `swarms-5.0.3/swarms/utils/get_logger.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/json_output_parser.py` & `swarms-5.0.3/swarms/utils/json_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/jsonl_utils.py` & `swarms-5.0.3/swarms/utils/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/llm_metrics_decorator.py` & `swarms-5.0.3/swarms/utils/llm_metrics_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/logger.py` & `swarms-5.0.3/swarms/utils/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/loggers.py` & `swarms-5.0.3/swarms/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/markdown_message.py` & `swarms-5.0.3/swarms/utils/markdown_message.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/parse_code.py` & `swarms-5.0.3/swarms/utils/parse_code.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/pdf_to_text.py` & `swarms-5.0.3/swarms/utils/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/remove_json_whitespace.py` & `swarms-5.0.3/swarms/utils/remove_json_whitespace.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/save_logs.py` & `swarms-5.0.3/swarms/utils/save_logs.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/serializable.py` & `swarms-5.0.3/swarms/utils/serializable.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/try_except_wrapper.py` & `swarms-5.0.3/swarms/utils/try_except_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/swarms/utils/yaml_output_parser.py` & `swarms-5.0.3/swarms/utils/yaml_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.1/setup.py` & `swarms-5.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,38 +16,37 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Pillow==10.3.0',
  'PyYAML',
- 'accelerate==0.28.0',
  'asyncio>=3.4.3,<4.0',
  'backoff==2.2.1',
  'docstring_parser==0.16',
  'langchain-community==0.0.29',
  'langchain-experimental==0.0.55',
  'loguru==0.7.2',
- 'opencv-python>=4.9.0.80,<5.0.0.0',
+ 'opencv-python-headless',
  'psutil',
  'pydantic==2.7.1',
  'pypdf==4.1.0',
  'python-dotenv',
  'ratelimit==2.2.1',
  'sentry-sdk',
  'tenacity==8.2.3',
  'toml',
  'torch>=2.1.1,<3.0',
  'transformers>=4.39.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'swarms',
-    'version': '5.0.1',
+    'version': '5.0.3',
     'description': 'Swarms - Pytorch',
-    'long_description': '![Swarming banner icon](images/swarmslogobanner.png)\n\n<div align="center">\n\nOrchestrate swarms of agents for production-grade applications.\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)\n\n[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)\n\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)\n\n</div>\n\nIndividual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups.\n----\n\n## Install\n`$ pip3 install -U swarms==4.9.7`\n\n---\n\n## Usage\n\n\nRun example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">\n<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\n### `Agent`\nA fully plug-and-play autonomous agent powered by an LLM extended by a long-term memory database, and equipped with function calling for tool usage! By passing in an LLM, you can create a fully autonomous agent with extreme customization and reliability, ready for real-world task automation!\n\nFeatures:\n\n✅ Any LLM / Any framework\n\n✅ Extremely customize-able with max loops, autosaving, import docs (PDFS, TXT, CSVs, etc), tool usage, etc etc\n\n✅ Long term memory database with RAG (ChromaDB, Pinecone, Qdrant)\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, autosave=True, dashboard=True)\n\n# Run the workflow on a task\nagent.run("Generate a 10,000 word blog on health and wellness.")\n```\n\n\n# `Agent` with Long Term Memory\n`Agent` equipped with quasi-infinite long term memory. Great for long document understanding, analysis, and retrieval.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n# `Agent` with Long Term Memory ++ Tools!\nAn LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat, tool\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initialize a tool\n@tool\ndef search_api(query: str):\n    # Add your logic here\n    return query\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n    tools=[search_api],\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n### Simple Conversational Agent\nA Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models\n\n- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking\n- Reliable, this simple system will always provide responses you want.\n\n```python\nfrom swarms import Agent, Anthropic\n\n\n## Initialize the workflow\nagent = Agent(\n    agent_name="Transcript Generator",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True, # Set to True\n)\n\n# Run the workflow on a task\nagent("Generate a transcript for a youtube video on what swarms are!")\n```\n\n## Devin\nImplementation of Devil in less than 90 lines of code with several tools:\nterminal, browser, and edit files!\n\n```python\nfrom swarms import Agent, Anthropic, tool\nimport subprocess\n\n# Model\nllm = Anthropic(\n    temperature=0.1,\n)\n\n# Tools\n@tool\ndef terminal(\n    code: str,\n):\n    """\n    Run code in the terminal.\n\n    Args:\n        code (str): The code to run in the terminal.\n\n    Returns:\n        str: The output of the code.\n    """\n    out = subprocess.run(\n        code, shell=True, capture_output=True, text=True\n    ).stdout\n    return str(out)\n\n\n@tool\ndef browser(query: str):\n    """\n    Search the query in the browser with the `browser` tool.\n\n    Args:\n        query (str): The query to search in the browser.\n\n    Returns:\n        str: The search results.\n    """\n    import webbrowser\n\n    url = f"https://www.google.com/search?q={query}"\n    webbrowser.open(url)\n    return f"Searching for {query} in the browser."\n\n@tool\ndef create_file(file_path: str, content: str):\n    """\n    Create a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file creation operation.\n    """\n    with open(file_path, "w") as file:\n        file.write(content)\n    return f"File {file_path} created successfully."\n\n@tool\ndef file_editor(file_path: str, mode: str, content: str):\n    """\n    Edit a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        mode (str): The mode to open the file in.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file editing operation.\n    """\n    with open(file_path, mode) as file:\n        file.write(content)\n    return f"File {file_path} edited successfully."\n\n\n# Agent\nagent = Agent(\n    agent_name="Devin",\n    system_prompt=(\n        "Autonomous agent that can interact with humans and other"\n        " agents. Be Helpful and Kind. Use the tools provided to"\n        " assist the user. Return all code in markdown format."\n    ),\n    llm=llm,\n    max_loops="auto",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True,\n    tools=[terminal, browser, file_editor, create_file],\n    code_interpreter=True,\n    # streaming=True,\n)\n\n# Run the agent\nout = agent("Create a new file for a plan to take over the world.")\nprint(out)\n```\n\n\n## `Agent`with Pydantic BaseModel as Output Type\nThe following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:\n\n```python\nfrom pydantic import BaseModel, Field\nfrom swarms import Anthropic, Agent\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(..., title="Whether the person is a student")\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = Schema(\n    name="Tool Name",\n    agent=1,\n    is_student=True,\n    courses=["Course1", "Course2"],\n)\n\n# Define the task to generate a person\'s information\ntask = "Generate a person\'s information based on the following schema:"\n\n# Initialize the agent\nagent = Agent(\n    agent_name="Person Information Generator",\n    system_prompt=(\n        "Generate a person\'s information based on the following schema:"\n    ),\n    # Set the tool schema to the JSON string -- this is the key difference\n    tool_schema=tool_schema,\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    interactive=True,\n    # Set the output type to the tool schema which is a BaseModel\n    output_type=tool_schema,  # or dict, or str\n    metadata_output_type="json",\n    # List of schemas that the agent can handle\n    list_tool_schemas=[tool_schema],\n    function_calling_format_type="OpenAI",\n    function_calling_type="json",  # or soon yaml\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n\n```\n\n\n### `ToolAgent`\nToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.\n\n\n```python\nfrom pydantic import BaseModel, Field\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom swarms import ToolAgent\nfrom swarms.utils.json_utils import base_model_to_json\n\n# Load the pre-trained model and tokenizer\nmodel = AutoModelForCausalLM.from_pretrained(\n    "databricks/dolly-v2-12b",\n    load_in_4bit=True,\n    device_map="auto",\n)\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = base_model_to_json(Schema)\n\n# Define the task to generate a person\'s information\ntask = (\n    "Generate a person\'s information based on the following schema:"\n)\n\n# Create an instance of the ToolAgent class\nagent = ToolAgent(\n    name="dolly-function-agent",\n    description="Ana gent to create a child data",\n    model=model,\n    tokenizer=tokenizer,\n    json_schema=tool_schema,\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n```\n\n\n### `Worker`\nThe `Worker` is a simple all-in-one agent equipped with an LLM, tools, and RAG for low level tasks.\n\n✅ Plug in and Play LLM. Utilize any LLM from anywhere and any framework\n\n✅ Reliable RAG: Utilizes FAISS for efficient RAG but it\'s modular so you can use any DB.\n\n✅ Multi-Step Parallel Function Calling: Use any tool\n\n```python\n# Importing necessary modules\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import OpenAIChat, Worker, tool\n\n# Loading environment variables from .env file\nload_dotenv()\n\n# Retrieving the OpenAI API key from environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Create a tool\n@tool\ndef search_api(query: str):\n    pass\n\n\n# Creating a Worker instance\nworker = Worker(\n    name="My Worker",\n    role="Worker",\n    human_in_the_loop=False,\n    tools=[search_api],\n    temperature=0.5,\n    llm=OpenAIChat(openai_api_key=api_key),\n)\n\n# Running the worker with a prompt\nout = worker.run("Hello, how are you? Create an image of how your are doing!")\n\n# Printing the output\nprint(out)\n```\n\n------\n\n\n\n\n\n\n\n----\n\n### `SequentialWorkflow`\nSequential Workflow enables you to sequentially execute tasks with `Agent` and then pass the output into the next agent and onwards until you have specified your max loops. `SequentialWorkflow` is wonderful for real-world business tasks like sending emails, summarizing documents, and analyzing data.\n\n\n✅  Save and Restore Workflow states!\n\n✅  Multi-Modal Support for Visual Chaining\n\n✅  Utilizes Agent class\n\n```python\nfrom swarms import Agent, SequentialWorkflow, Anthropic\n\n\n# Initialize the language model agent (e.g., GPT-3)\nllm = Anthropic()\n\n# Initialize agents for individual tasks\nagent1 = Agent(\n    agent_name="Blog generator",\n    system_prompt="Generate a blog post like stephen king",\n    llm=llm,\n    max_loops=1,\n    dashboard=False,\n    tools=[],\n)\nagent2 = Agent(\n    agent_name="summarizer",\n    system_prompt="Sumamrize the blog post",\n    llm=llm,\n    max_loops=1,\n    dashboard=False,\n    tools=[],\n)\n\n# Create the Sequential workflow\nworkflow = SequentialWorkflow(\n    agents=[agent1, agent2], max_loops=1, verbose=False\n)\n\n# Run the workflow\nworkflow.run(\n    "Generate a blog post on how swarms of agents can help businesses grow."\n)\n\n```\n\n\n\n### `ConcurrentWorkflow`\n`ConcurrentWorkflow` runs all the tasks all at the same time with the inputs you give it!\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, ConcurrentWorkflow, OpenAIChat, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = ConcurrentWorkflow(max_workers=5)\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(tasks=[task1, task2, task3])\n\n# Run the workflow\nworkflow.run()\n```\n\n### `RecursiveWorkflow`\n`RecursiveWorkflow` will keep executing the tasks until a specific token like <DONE> is located inside the text!\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, RecursiveWorkflow, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = RecursiveWorkflow(stop_token="<DONE>")\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(task1)\nworkflow.add(task2)\nworkflow.add(task3)\n\n# Run the workflow\nworkflow.run()\n```\n\n\n\n### `ModelParallelizer`\nThe ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.\n\nPlug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat\n\nload_dotenv()\n\n# API Keys\nanthropic_api_key = os.getenv("ANTHROPIC_API_KEY")\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Initialize the models\nllm = OpenAIChat(openai_api_key=openai_api_key)\nanthropic = Anthropic(anthropic_api_key=anthropic_api_key)\nmixtral = Mixtral()\ngemini = Gemini(gemini_api_key=gemini_api_key)\n\n# Initialize the parallelizer\nllms = [llm, anthropic, mixtral, gemini]\nparallelizer = ModelParallelizer(llms)\n\n# Set the task\ntask = "Generate a 10,000 word blog on health and wellness."\n\n# Run the task\nout = parallelizer.run(task)\n\n# Print the responses 1 by 1\nfor i in range(len(out)):\n    print(f"Response from LLM {i}: {out[i]}")\n```\n\n\n\n\n### `SwarmNetwork`\n`SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.\n\n✅ Efficient Task Management: SwarmNetwork\'s intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.\n\n✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.\n\n✅ Versatile Deployment Options: With SwarmNetwork, each agent can be run on its own thread, process, container, machine, or even cluster. This provides a high degree of flexibility and allows for deployment that best suits the user\'s needs and infrastructure.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat, SwarmNetwork\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5,\n    openai_api_key=api_key,\n)\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, agent_name="Social Media Manager")\nagent2 = Agent(llm=llm, max_loops=1, agent_name=" Product Manager")\nagent3 = Agent(llm=llm, max_loops=1, agent_name="SEO Manager")\n\n\n# Load the swarmnet with the agents\nswarmnet = SwarmNetwork(\n    agents=[agent, agent2, agent3],\n)\n\n# List the agents in the swarm network\nout = swarmnet.list_agents()\nprint(out)\n\n# Run the workflow on a task\nout = swarmnet.run_single_agent(\n    agent2.id, "Generate a 10,000 word blog on health and wellness."\n)\nprint(out)\n\n\n# Run all the agents in the swarm network on a task\nout = swarmnet.run_many_agents("Generate a 10,000 word blog on health and wellness.")\nprint(out)\n```\n\n\n### `Task`\n`Task` is a simple structure for task execution with the `Agent`. Imagine zapier for LLM-based workflow automation\n\n✅ Task is a structure for task execution with the Agent. \n\n✅ Tasks can have descriptions, scheduling, triggers, actions, conditions, dependencies, priority, and a history. \n\n✅ The Task structure allows for efficient workflow automation with LLM-based agents.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.structs import Agent, OpenAIChat, Task\n\n# Load the environment variables\nload_dotenv()\n\n\n# Define a function to be used as the action\ndef my_action():\n    print("Action executed")\n\n\n# Define a function to be used as the condition\ndef my_condition():\n    print("Condition checked")\n    return True\n\n\n# Create an agent\nagent = Agent(\n    llm=OpenAIChat(openai_api_key=os.environ["OPENAI_API_KEY"]),\n    max_loops=1,\n    dashboard=False,\n)\n\n# Create a task\ntask = Task(\n    description=(\n        "Generate a report on the top 3 biggest expenses for small"\n        " businesses and how businesses can save 20%"\n    ),\n    agent=agent,\n)\n\n# Set the action and condition\ntask.set_action(my_action)\ntask.set_condition(my_condition)\n\n# Execute the task\nprint("Executing task...")\ntask.run()\n\n# Check if the task is completed\nif task.is_completed():\n    print("Task completed")\nelse:\n    print("Task not completed")\n\n# Output the result of the task\nprint(f"Task result: {task.result}")\n```\n\n---\n\n\n\n### `BlockList`\n- Modularity and Flexibility: BlocksList allows users to create custom swarms by adding or removing different classes or functions as blocks. This means users can easily tailor the functionality of their swarm to suit their specific needs.\n\n- Ease of Management: With methods to add, remove, update, and retrieve blocks, BlocksList provides a straightforward way to manage the components of a swarm. This makes it easier to maintain and update the swarm over time.\n\n- Enhanced Searchability: BlocksList offers methods to get blocks by various attributes such as name, type, ID, and parent-related properties. This makes it easier for users to find and work with specific blocks in a large and complex swarm.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\nfrom pydantic import BaseModel\nfrom swarms import BlocksList, Gemini, GPT4VisionAPI, Mixtral, OpenAI, ToolAgent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the environment variables\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Tool Agent\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n# Convert the schema to a JSON string\njson_schema = base_model_to_json(Schema)\n\n\ntoolagent = ToolAgent(model=model, tokenizer=tokenizer, json_schema=json_schema)\n\n# Blocks List which enables you to build custom swarms by adding classes or functions\nswarm = BlocksList(\n    "SocialMediaSwarm",\n    "A swarm of social media agents",\n    [\n        OpenAI(openai_api_key=openai_api_key),\n        Mixtral(),\n        GPT4VisionAPI(openai_api_key=openai_api_key),\n        Gemini(gemini_api_key=gemini_api_key),\n    ],\n)\n\n\n# Add the new block to the swarm\nswarm.add(toolagent)\n\n# Remove a block from the swarm\nswarm.remove(toolagent)\n\n# Update a block in the swarm\nswarm.update(toolagent)\n\n# Get a block at a specific index\nblock_at_index = swarm.get(0)\n\n# Get all blocks in the swarm\nall_blocks = swarm.get_all()\n\n# Get blocks by name\nopenai_blocks = swarm.get_by_name("OpenAI")\n\n# Get blocks by type\ngpt4_blocks = swarm.get_by_type("GPT4VisionAPI")\n\n# Get blocks by ID\nblock_by_id = swarm.get_by_id(toolagent.id)\n\n# Get blocks by parent\nblocks_by_parent = swarm.get_by_parent(swarm)\n\n# Get blocks by parent ID\nblocks_by_parent_id = swarm.get_by_parent_id(swarm.id)\n\n# Get blocks by parent name\nblocks_by_parent_name = swarm.get_by_parent_name(swarm.name)\n\n# Get blocks by parent type\nblocks_by_parent_type = swarm.get_by_parent_type(type(swarm).__name__)\n\n# Get blocks by parent description\nblocks_by_parent_description = swarm.get_by_parent_description(swarm.description)\n\n# Run the block in the swarm\ninference = swarm.run_block(toolagent, "Hello World")\nprint(inference)\n```\n\n\n## Majority Voting\nMultiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)\n\n```python\nfrom swarms import Agent, MajorityVoting, ChromaDB, Anthropic\n\n# Initialize the llm\nllm = Anthropic()\n\n# Agents\nagent1 = Agent(\n    llm = llm,\n    system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",\n    agent_name="Progressive Leader",\n    agent_description="Leader of the Progressive Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent2 = Agent(\n    llm=llm,\n    agent_name="Conservative Leader",\n    agent_description="Leader of the Conservative Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent3 = Agent(\n    llm=llm,\n    agent_name="Libertarian Leader",\n    agent_description="Leader of the Libertarian Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\n# Initialize the majority voting\nmv = MajorityVoting(\n    agents=[agent1, agent2, agent3],\n    output_parser=llm.majority_voting,\n    autosave=False,\n    verbose=True,\n)\n\n\n# Start the majority voting\nmv.run("What is your stance on healthcare?")\n```\n\n## Real-World Deployment\n\n### Multi-Agent Swarm for Logistics\nHere\'s a production grade swarm ready for real-world deployment in a factory and logistics settings like warehouses. This swarm can automate 3 costly and inefficient workflows, safety checks, productivity checks, and warehouse security.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models import GPT4VisionAPI\nfrom swarms.prompts.logistics import (\n    Efficiency_Agent_Prompt,\n    Health_Security_Agent_Prompt,\n    Productivity_Agent_Prompt,\n    Quality_Control_Agent_Prompt,\n    Safety_Agent_Prompt,\n    Security_Agent_Prompt,\n    Sustainability_Agent_Prompt,\n)\nfrom swarms.structs import Agent\n\n# Load ENV\nload_dotenv()\napi_key = os.getenv("OPENAI_API_KEY")\n\n# GPT4VisionAPI\nllm = GPT4VisionAPI(openai_api_key=api_key)\n\n# Image for analysis\nfactory_image = "factory_image1.jpg"\n\n# Initialize agents with respective prompts\nhealth_security_agent = Agent(\n    llm=llm,\n    sop=Health_Security_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Quality control agent\nquality_control_agent = Agent(\n    llm=llm,\n    sop=Quality_Control_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Productivity Agent\nproductivity_agent = Agent(\n    llm=llm,\n    sop=Productivity_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Initiailize safety agent\nsafety_agent = Agent(llm=llm, sop=Safety_Agent_Prompt, max_loops=1, multi_modal=True)\n\n# Init the security agent\nsecurity_agent = Agent(\n    llm=llm, sop=Security_Agent_Prompt, max_loops=1, multi_modal=True\n)\n\n\n# Initialize sustainability agent\nsustainability_agent = Agent(\n    llm=llm,\n    sop=Sustainability_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Initialize efficincy agent\nefficiency_agent = Agent(\n    llm=llm,\n    sop=Efficiency_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Run agents with respective tasks on the same image\nhealth_analysis = health_security_agent.run(\n    "Analyze the safety of this factory", factory_image\n)\nquality_analysis = quality_control_agent.run(\n    "Examine product quality in the factory", factory_image\n)\nproductivity_analysis = productivity_agent.run(\n    "Evaluate factory productivity", factory_image\n)\nsafety_analysis = safety_agent.run(\n    "Inspect the factory\'s adherence to safety standards",\n    factory_image,\n)\nsecurity_analysis = security_agent.run(\n    "Assess the factory\'s security measures and systems",\n    factory_image,\n)\nsustainability_analysis = sustainability_agent.run(\n    "Examine the factory\'s sustainability practices", factory_image\n)\nefficiency_analysis = efficiency_agent.run(\n    "Analyze the efficiency of the factory\'s manufacturing process",\n    factory_image,\n)\n```\n---\n\n\n## `Multi Modal Autonomous Agents`\nRun the agent with multiple modalities useful for various real-world tasks in manufacturing, logistics, and health.\n\n```python\n# Description: This is an example of how to use the Agent class to run a multi-modal workflow\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models.gpt4_vision_api import GPT4VisionAPI\nfrom swarms.structs import Agent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = GPT4VisionAPI(\n    openai_api_key=api_key,\n    max_tokens=500,\n)\n\n# Initialize the task\ntask = (\n    "Analyze this image of an assembly line and identify any issues such as"\n    " misaligned parts, defects, or deviations from the standard assembly"\n    " process. IF there is anything unsafe in the image, explain why it is"\n    " unsafe and how it could be improved."\n)\nimg = "assembly_line.jpg"\n\n## Initialize the workflow\nagent = Agent(\n    llm=llm, max_loops="auto", autosave=True, dashboard=True, multi_modal=True\n)\n\n# Run the workflow on a task\nagent.run(task=task, img=img)\n```\n----\n\n\n## Build your own LLMs, Agents, and Swarms!\n\n### Swarms Compliant Model Interface\n```python\nfrom swarms import BaseLLM\n\nclass vLLMLM(BaseLLM):\n    def __init__(self, model_name=\'default_model\', tensor_parallel_size=1, *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.model_name = model_name\n        self.tensor_parallel_size = tensor_parallel_size\n        # Add any additional initialization here\n    \n    def run(self, task: str):\n        pass\n\n# Example\nmodel = vLLMLM("mistral")\n\n# Run the model\nout = model("Analyze these financial documents and summarize of them")\nprint(out)\n\n```\n\n\n### Swarms Compliant Agent Interface\n\n```python\nfrom swarms import Agent\n\n\nclass MyCustomAgent(Agent):\n\n\xa0 \xa0 def __init__(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 super().__init__(*args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Custom initialization logic\n\n\xa0 \xa0 def custom_method(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Implement custom logic here\n\n\xa0 \xa0 \xa0 \xa0 pass\n\n\xa0 \xa0 def run(self, task, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Customize the run method\n\n\xa0 \xa0 \xa0 \xa0 response = super().run(task, *args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Additional custom logic\n\n\xa0 \xa0 \xa0 \xa0 return response`\n\n# Model\nagent = MyCustomAgent()\n\n# Run the agent\nout = agent("Analyze and summarize these financial documents: ")\nprint(out)\n\n```\n\n\n### Compliant Interface for Multi-Agent Collaboration\n\n```python\nfrom swarms import AutoSwarm, AutoSwarmRouter, BaseSwarm\n\n\n# Build your own Swarm\nclass MySwarm(BaseSwarm):\n    def __init__(self, name="kyegomez/myswarm", *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.name = name\n\n    def run(self, task: str, *args, **kwargs):\n        # Add your multi-agent logic here\n        # agent 1\n        # agent 2\n        # agent 3\n        return "output of the swarm"\n\n\n# Add your custom swarm to the AutoSwarmRouter\nrouter = AutoSwarmRouter(\n    swarms=[MySwarm]\n)\n\n\n# Create an AutoSwarm instance\nautoswarm = AutoSwarm(\n    name="kyegomez/myswarm",\n    description="A simple API to build and run swarms",\n    verbose=True,\n    router=router,\n)\n\n\n# Run the AutoSwarm\nautoswarm.run("Analyze these financial data and give me a summary")\n\n\n```\n\n## `AgentRearrange`\nInspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships\n\n```python\nfrom swarms import Agent, AgentRearrange, rearrange, Anthropic\n\n\n# Initialize the director agent\n\ndirector = Agent(\n    agent_name="Director",\n    system_prompt="Directs the tasks for the workers",\n    llm=Anthropic(),\n    max_loops=1,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    state_save_file_type="json",\n    saved_state_path="director.json",\n)\n\n\n# Initialize worker 1\n\nworker1 = Agent(\n    agent_name="Worker1",\n    system_prompt="Generates a transcript for a youtube video on what swarms are",\n    llm=Anthropic(),\n    max_loops=1,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    state_save_file_type="json",\n    saved_state_path="worker1.json",\n)\n\n\n# Initialize worker 2\nworker2 = Agent(\n    agent_name="Worker2",\n    system_prompt="Summarizes the transcript generated by Worker1",\n    llm=Anthropic(),\n    max_loops=1,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    state_save_file_type="json",\n    saved_state_path="worker2.json",\n)\n\n\n# Create a list of agents\nagents = [director, worker1, worker2]\n\n# Define the flow pattern\nflow = "Director -> Worker1 -> Worker2"\n\n# Using AgentRearrange class\nagent_system = AgentRearrange(agents=agents, flow=flow)\noutput = agent_system.run(\n    "Create a format to express and communicate swarms of llms in a structured manner for youtube"\n)\nprint(output)\n\n\n# Using rearrange function\noutput = rearrange(\n    agents,\n    flow,\n    "Create a format to express and communicate swarms of llms in a structured manner for youtube",\n)\n\nprint(output)\n\n```\n\n\n---\n\n## Documentation\nDocumentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)\n\n----\n\n## 🫶 Contributions:\n\nThe easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)\n\nSwarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!\n\n<a href="https://github.com/kyegomez/swarms/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=kyegomez/swarms" />\n</a>\n\n----\n\n## Community\n\nJoin our growing community around the world, for real-time support, ideas, and discussions on Swarms 😊 \n\n- View our official [Blog](https://swarms.apac.ai)\n- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)\n- Follow us on [Twitter](https://twitter.com/kyegomez)\n- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)\n- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)\n- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)\n- Join our Swarms Community Gathering every Thursday at 1pm NYC Time to unlock the potential of autonomous agents in automating your daily tasks [Sign up here](https://lu.ma/5p2jnc2v)\n\n---\n\n## Discovery Call\nBook a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)\n\n\n\n## Accelerate Backlog\nHelp us accelerate our backlog by supporting us financially! Note, we\'re an open source corporation and so all the revenue we generate is through donations at the moment ;)\n\n<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>\n\n\n## File Structure\nThe swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs`\xa0that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.\n\n```sh\n├── __init__.py\n├── agents\n├── artifacts\n├── chunkers\n├── cli\n├── loaders\n├── memory\n├── models\n├── prompts\n├── structs\n├── telemetry\n├── tokenizers\n├── tools\n├── utils\n└── workers\n```\n\n## Docker Instructions\n\nThis application uses Docker with CUDA support. To build and run the Docker container, follow these steps:\n\n### Prerequisites\n\n- Make sure you have [Docker installed](https://docs.docker.com/get-docker/) on your machine.\n- Ensure your machine has an NVIDIA GPU and [NVIDIA Docker support](https://github.com/NVIDIA/nvidia-docker) installed.\n\n### Building the Docker Image\n\nTo build the Docker image, navigate to the root directory containing the `Dockerfile` and run the following command:\n\n```bash\ndocker build --gpus all -t swarms\n``` \n### Running the Docker Container\nTo run the Docker container, use the following command:\n\n`docker run --gpus all -p 4000:80 swarms`\n\nReplace swarms with the name of your Docker image, and replace 4000:80 with your actual port mapping. The format is hostPort:containerPort.\n\nNow, your application should be running with CUDA support!\n\n\n## Swarm Newsletter 🤖 🤖 🤖 📧 \nSign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊\n\n\n[CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)\n\n# License\nApache License\n\n\n\n',
+    'long_description': '![Swarming banner icon](images/swarmslogobanner.png)\n\n<div align="center">\n\nOrchestrate swarms of agents for production-grade applications.\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)\n\n[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)\n\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)\n\n</div>\n\nIndividual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups.\n----\n\n## Install\n`$ pip3 install -U swarms==4.9.7`\n\n---\n\n## Usage\n\n\nRun example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">\n<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\n### `Agent`\nA fully plug-and-play autonomous agent powered by an LLM extended by a long-term memory database, and equipped with function calling for tool usage! By passing in an LLM, you can create a fully autonomous agent with extreme customization and reliability, ready for real-world task automation!\n\nFeatures:\n\n✅ Any LLM / Any framework\n\n✅ Extremely customize-able with max loops, autosaving, import docs (PDFS, TXT, CSVs, etc), tool usage, etc etc\n\n✅ Long term memory database with RAG (ChromaDB, Pinecone, Qdrant)\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, autosave=True, dashboard=True)\n\n# Run the workflow on a task\nagent.run("Generate a 10,000 word blog on health and wellness.")\n```\n\n\n# `Agent` with Long Term Memory\n`Agent` equipped with quasi-infinite long term memory. Great for long document understanding, analysis, and retrieval.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n# `Agent` with Long Term Memory ++ Tools!\nAn LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat, tool\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initialize a tool\n@tool\ndef search_api(query: str):\n    # Add your logic here\n    return query\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n    tools=[search_api],\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n### Simple Conversational Agent\nA Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models\n\n- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking\n- Reliable, this simple system will always provide responses you want.\n\n```python\nfrom swarms import Agent, Anthropic\n\n\n## Initialize the workflow\nagent = Agent(\n    agent_name="Transcript Generator",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True, # Set to True\n)\n\n# Run the workflow on a task\nagent("Generate a transcript for a youtube video on what swarms are!")\n```\n\n## Devin\nImplementation of Devil in less than 90 lines of code with several tools:\nterminal, browser, and edit files!\n\n```python\nfrom swarms import Agent, Anthropic, tool\nimport subprocess\n\n# Model\nllm = Anthropic(\n    temperature=0.1,\n)\n\n# Tools\n@tool\ndef terminal(\n    code: str,\n):\n    """\n    Run code in the terminal.\n\n    Args:\n        code (str): The code to run in the terminal.\n\n    Returns:\n        str: The output of the code.\n    """\n    out = subprocess.run(\n        code, shell=True, capture_output=True, text=True\n    ).stdout\n    return str(out)\n\n\n@tool\ndef browser(query: str):\n    """\n    Search the query in the browser with the `browser` tool.\n\n    Args:\n        query (str): The query to search in the browser.\n\n    Returns:\n        str: The search results.\n    """\n    import webbrowser\n\n    url = f"https://www.google.com/search?q={query}"\n    webbrowser.open(url)\n    return f"Searching for {query} in the browser."\n\n@tool\ndef create_file(file_path: str, content: str):\n    """\n    Create a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file creation operation.\n    """\n    with open(file_path, "w") as file:\n        file.write(content)\n    return f"File {file_path} created successfully."\n\n@tool\ndef file_editor(file_path: str, mode: str, content: str):\n    """\n    Edit a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        mode (str): The mode to open the file in.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file editing operation.\n    """\n    with open(file_path, mode) as file:\n        file.write(content)\n    return f"File {file_path} edited successfully."\n\n\n# Agent\nagent = Agent(\n    agent_name="Devin",\n    system_prompt=(\n        "Autonomous agent that can interact with humans and other"\n        " agents. Be Helpful and Kind. Use the tools provided to"\n        " assist the user. Return all code in markdown format."\n    ),\n    llm=llm,\n    max_loops="auto",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True,\n    tools=[terminal, browser, file_editor, create_file],\n    code_interpreter=True,\n    # streaming=True,\n)\n\n# Run the agent\nout = agent("Create a new file for a plan to take over the world.")\nprint(out)\n```\n\n\n## `Agent`with Pydantic BaseModel as Output Type\nThe following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:\n\n```python\nfrom pydantic import BaseModel, Field\nfrom swarms import Anthropic, Agent\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(..., title="Whether the person is a student")\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = Schema(\n    name="Tool Name",\n    agent=1,\n    is_student=True,\n    courses=["Course1", "Course2"],\n)\n\n# Define the task to generate a person\'s information\ntask = "Generate a person\'s information based on the following schema:"\n\n# Initialize the agent\nagent = Agent(\n    agent_name="Person Information Generator",\n    system_prompt=(\n        "Generate a person\'s information based on the following schema:"\n    ),\n    # Set the tool schema to the JSON string -- this is the key difference\n    tool_schema=tool_schema,\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    interactive=True,\n    # Set the output type to the tool schema which is a BaseModel\n    output_type=tool_schema,  # or dict, or str\n    metadata_output_type="json",\n    # List of schemas that the agent can handle\n    list_tool_schemas=[tool_schema],\n    function_calling_format_type="OpenAI",\n    function_calling_type="json",  # or soon yaml\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n\n```\n\n\n### `ToolAgent`\nToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.\n\n\n```python\nfrom pydantic import BaseModel, Field\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom swarms import ToolAgent\nfrom swarms.utils.json_utils import base_model_to_json\n\n# Load the pre-trained model and tokenizer\nmodel = AutoModelForCausalLM.from_pretrained(\n    "databricks/dolly-v2-12b",\n    load_in_4bit=True,\n    device_map="auto",\n)\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = base_model_to_json(Schema)\n\n# Define the task to generate a person\'s information\ntask = (\n    "Generate a person\'s information based on the following schema:"\n)\n\n# Create an instance of the ToolAgent class\nagent = ToolAgent(\n    name="dolly-function-agent",\n    description="Ana gent to create a child data",\n    model=model,\n    tokenizer=tokenizer,\n    json_schema=tool_schema,\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n```\n\n\n### `Worker`\nThe `Worker` is a simple all-in-one agent equipped with an LLM, tools, and RAG for low level tasks.\n\n✅ Plug in and Play LLM. Utilize any LLM from anywhere and any framework\n\n✅ Reliable RAG: Utilizes FAISS for efficient RAG but it\'s modular so you can use any DB.\n\n✅ Multi-Step Parallel Function Calling: Use any tool\n\n```python\n# Importing necessary modules\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import OpenAIChat, Worker, tool\n\n# Loading environment variables from .env file\nload_dotenv()\n\n# Retrieving the OpenAI API key from environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Create a tool\n@tool\ndef search_api(query: str):\n    pass\n\n\n# Creating a Worker instance\nworker = Worker(\n    name="My Worker",\n    role="Worker",\n    human_in_the_loop=False,\n    tools=[search_api],\n    temperature=0.5,\n    llm=OpenAIChat(openai_api_key=api_key),\n)\n\n# Running the worker with a prompt\nout = worker.run("Hello, how are you? Create an image of how your are doing!")\n\n# Printing the output\nprint(out)\n```\n\n------\n\n\n\n\n\n\n\n----\n\n### `SequentialWorkflow`\nSequential Workflow enables you to sequentially execute tasks with `Agent` and then pass the output into the next agent and onwards until you have specified your max loops. `SequentialWorkflow` is wonderful for real-world business tasks like sending emails, summarizing documents, and analyzing data.\n\n\n✅  Save and Restore Workflow states!\n\n✅  Multi-Modal Support for Visual Chaining\n\n✅  Utilizes Agent class\n\n```python\nfrom swarms import Agent, SequentialWorkflow, Anthropic\n\n\n# Initialize the language model agent (e.g., GPT-3)\nllm = Anthropic()\n\n# Initialize agents for individual tasks\nagent1 = Agent(\n    agent_name="Blog generator",\n    system_prompt="Generate a blog post like stephen king",\n    llm=llm,\n    max_loops=1,\n    dashboard=False,\n    tools=[],\n)\nagent2 = Agent(\n    agent_name="summarizer",\n    system_prompt="Sumamrize the blog post",\n    llm=llm,\n    max_loops=1,\n    dashboard=False,\n    tools=[],\n)\n\n# Create the Sequential workflow\nworkflow = SequentialWorkflow(\n    agents=[agent1, agent2], max_loops=1, verbose=False\n)\n\n# Run the workflow\nworkflow.run(\n    "Generate a blog post on how swarms of agents can help businesses grow."\n)\n\n```\n\n\n\n### `ConcurrentWorkflow`\n`ConcurrentWorkflow` runs all the tasks all at the same time with the inputs you give it!\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, ConcurrentWorkflow, OpenAIChat, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = ConcurrentWorkflow(max_workers=5)\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(tasks=[task1, task2, task3])\n\n# Run the workflow\nworkflow.run()\n```\n\n### `RecursiveWorkflow`\n`RecursiveWorkflow` will keep executing the tasks until a specific token like <DONE> is located inside the text!\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, RecursiveWorkflow, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = RecursiveWorkflow(stop_token="<DONE>")\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(task1)\nworkflow.add(task2)\nworkflow.add(task3)\n\n# Run the workflow\nworkflow.run()\n```\n\n\n\n### `ModelParallelizer`\nThe ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.\n\nPlug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat\n\nload_dotenv()\n\n# API Keys\nanthropic_api_key = os.getenv("ANTHROPIC_API_KEY")\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Initialize the models\nllm = OpenAIChat(openai_api_key=openai_api_key)\nanthropic = Anthropic(anthropic_api_key=anthropic_api_key)\nmixtral = Mixtral()\ngemini = Gemini(gemini_api_key=gemini_api_key)\n\n# Initialize the parallelizer\nllms = [llm, anthropic, mixtral, gemini]\nparallelizer = ModelParallelizer(llms)\n\n# Set the task\ntask = "Generate a 10,000 word blog on health and wellness."\n\n# Run the task\nout = parallelizer.run(task)\n\n# Print the responses 1 by 1\nfor i in range(len(out)):\n    print(f"Response from LLM {i}: {out[i]}")\n```\n\n\n\n\n### `SwarmNetwork`\n`SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.\n\n✅ Efficient Task Management: SwarmNetwork\'s intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.\n\n✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.\n\n✅ Versatile Deployment Options: With SwarmNetwork, each agent can be run on its own thread, process, container, machine, or even cluster. This provides a high degree of flexibility and allows for deployment that best suits the user\'s needs and infrastructure.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat, SwarmNetwork\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5,\n    openai_api_key=api_key,\n)\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, agent_name="Social Media Manager")\nagent2 = Agent(llm=llm, max_loops=1, agent_name=" Product Manager")\nagent3 = Agent(llm=llm, max_loops=1, agent_name="SEO Manager")\n\n\n# Load the swarmnet with the agents\nswarmnet = SwarmNetwork(\n    agents=[agent, agent2, agent3],\n)\n\n# List the agents in the swarm network\nout = swarmnet.list_agents()\nprint(out)\n\n# Run the workflow on a task\nout = swarmnet.run_single_agent(\n    agent2.id, "Generate a 10,000 word blog on health and wellness."\n)\nprint(out)\n\n\n# Run all the agents in the swarm network on a task\nout = swarmnet.run_many_agents("Generate a 10,000 word blog on health and wellness.")\nprint(out)\n```\n\n\n### `Task`\n`Task` is a simple structure for task execution with the `Agent`. Imagine zapier for LLM-based workflow automation\n\n✅ Task is a structure for task execution with the Agent. \n\n✅ Tasks can have descriptions, scheduling, triggers, actions, conditions, dependencies, priority, and a history. \n\n✅ The Task structure allows for efficient workflow automation with LLM-based agents.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.structs import Agent, OpenAIChat, Task\n\n# Load the environment variables\nload_dotenv()\n\n\n# Define a function to be used as the action\ndef my_action():\n    print("Action executed")\n\n\n# Define a function to be used as the condition\ndef my_condition():\n    print("Condition checked")\n    return True\n\n\n# Create an agent\nagent = Agent(\n    llm=OpenAIChat(openai_api_key=os.environ["OPENAI_API_KEY"]),\n    max_loops=1,\n    dashboard=False,\n)\n\n# Create a task\ntask = Task(\n    description=(\n        "Generate a report on the top 3 biggest expenses for small"\n        " businesses and how businesses can save 20%"\n    ),\n    agent=agent,\n)\n\n# Set the action and condition\ntask.set_action(my_action)\ntask.set_condition(my_condition)\n\n# Execute the task\nprint("Executing task...")\ntask.run()\n\n# Check if the task is completed\nif task.is_completed():\n    print("Task completed")\nelse:\n    print("Task not completed")\n\n# Output the result of the task\nprint(f"Task result: {task.result}")\n```\n\n---\n\n\n\n### `BlockList`\n- Modularity and Flexibility: BlocksList allows users to create custom swarms by adding or removing different classes or functions as blocks. This means users can easily tailor the functionality of their swarm to suit their specific needs.\n\n- Ease of Management: With methods to add, remove, update, and retrieve blocks, BlocksList provides a straightforward way to manage the components of a swarm. This makes it easier to maintain and update the swarm over time.\n\n- Enhanced Searchability: BlocksList offers methods to get blocks by various attributes such as name, type, ID, and parent-related properties. This makes it easier for users to find and work with specific blocks in a large and complex swarm.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\nfrom pydantic import BaseModel\nfrom swarms import BlocksList, Gemini, GPT4VisionAPI, Mixtral, OpenAI, ToolAgent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the environment variables\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Tool Agent\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n# Convert the schema to a JSON string\njson_schema = base_model_to_json(Schema)\n\n\ntoolagent = ToolAgent(model=model, tokenizer=tokenizer, json_schema=json_schema)\n\n# Blocks List which enables you to build custom swarms by adding classes or functions\nswarm = BlocksList(\n    "SocialMediaSwarm",\n    "A swarm of social media agents",\n    [\n        OpenAI(openai_api_key=openai_api_key),\n        Mixtral(),\n        GPT4VisionAPI(openai_api_key=openai_api_key),\n        Gemini(gemini_api_key=gemini_api_key),\n    ],\n)\n\n\n# Add the new block to the swarm\nswarm.add(toolagent)\n\n# Remove a block from the swarm\nswarm.remove(toolagent)\n\n# Update a block in the swarm\nswarm.update(toolagent)\n\n# Get a block at a specific index\nblock_at_index = swarm.get(0)\n\n# Get all blocks in the swarm\nall_blocks = swarm.get_all()\n\n# Get blocks by name\nopenai_blocks = swarm.get_by_name("OpenAI")\n\n# Get blocks by type\ngpt4_blocks = swarm.get_by_type("GPT4VisionAPI")\n\n# Get blocks by ID\nblock_by_id = swarm.get_by_id(toolagent.id)\n\n# Get blocks by parent\nblocks_by_parent = swarm.get_by_parent(swarm)\n\n# Get blocks by parent ID\nblocks_by_parent_id = swarm.get_by_parent_id(swarm.id)\n\n# Get blocks by parent name\nblocks_by_parent_name = swarm.get_by_parent_name(swarm.name)\n\n# Get blocks by parent type\nblocks_by_parent_type = swarm.get_by_parent_type(type(swarm).__name__)\n\n# Get blocks by parent description\nblocks_by_parent_description = swarm.get_by_parent_description(swarm.description)\n\n# Run the block in the swarm\ninference = swarm.run_block(toolagent, "Hello World")\nprint(inference)\n```\n\n\n## Majority Voting\nMultiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)\n\n```python\nfrom swarms import Agent, MajorityVoting, ChromaDB, Anthropic\n\n# Initialize the llm\nllm = Anthropic()\n\n# Agents\nagent1 = Agent(\n    llm = llm,\n    system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",\n    agent_name="Progressive Leader",\n    agent_description="Leader of the Progressive Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent2 = Agent(\n    llm=llm,\n    agent_name="Conservative Leader",\n    agent_description="Leader of the Conservative Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent3 = Agent(\n    llm=llm,\n    agent_name="Libertarian Leader",\n    agent_description="Leader of the Libertarian Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\n# Initialize the majority voting\nmv = MajorityVoting(\n    agents=[agent1, agent2, agent3],\n    output_parser=llm.majority_voting,\n    autosave=False,\n    verbose=True,\n)\n\n\n# Start the majority voting\nmv.run("What is your stance on healthcare?")\n```\n\n## Real-World Deployment\n\n### Multi-Agent Swarm for Logistics\nHere\'s a production grade swarm ready for real-world deployment in a factory and logistics settings like warehouses. This swarm can automate 3 costly and inefficient workflows, safety checks, productivity checks, and warehouse security.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models import GPT4VisionAPI\nfrom swarms.prompts.logistics import (\n    Efficiency_Agent_Prompt,\n    Health_Security_Agent_Prompt,\n    Productivity_Agent_Prompt,\n    Quality_Control_Agent_Prompt,\n    Safety_Agent_Prompt,\n    Security_Agent_Prompt,\n    Sustainability_Agent_Prompt,\n)\nfrom swarms.structs import Agent\n\n# Load ENV\nload_dotenv()\napi_key = os.getenv("OPENAI_API_KEY")\n\n# GPT4VisionAPI\nllm = GPT4VisionAPI(openai_api_key=api_key)\n\n# Image for analysis\nfactory_image = "factory_image1.jpg"\n\n# Initialize agents with respective prompts\nhealth_security_agent = Agent(\n    llm=llm,\n    sop=Health_Security_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Quality control agent\nquality_control_agent = Agent(\n    llm=llm,\n    sop=Quality_Control_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Productivity Agent\nproductivity_agent = Agent(\n    llm=llm,\n    sop=Productivity_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Initiailize safety agent\nsafety_agent = Agent(llm=llm, sop=Safety_Agent_Prompt, max_loops=1, multi_modal=True)\n\n# Init the security agent\nsecurity_agent = Agent(\n    llm=llm, sop=Security_Agent_Prompt, max_loops=1, multi_modal=True\n)\n\n\n# Initialize sustainability agent\nsustainability_agent = Agent(\n    llm=llm,\n    sop=Sustainability_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Initialize efficincy agent\nefficiency_agent = Agent(\n    llm=llm,\n    sop=Efficiency_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Run agents with respective tasks on the same image\nhealth_analysis = health_security_agent.run(\n    "Analyze the safety of this factory", factory_image\n)\nquality_analysis = quality_control_agent.run(\n    "Examine product quality in the factory", factory_image\n)\nproductivity_analysis = productivity_agent.run(\n    "Evaluate factory productivity", factory_image\n)\nsafety_analysis = safety_agent.run(\n    "Inspect the factory\'s adherence to safety standards",\n    factory_image,\n)\nsecurity_analysis = security_agent.run(\n    "Assess the factory\'s security measures and systems",\n    factory_image,\n)\nsustainability_analysis = sustainability_agent.run(\n    "Examine the factory\'s sustainability practices", factory_image\n)\nefficiency_analysis = efficiency_agent.run(\n    "Analyze the efficiency of the factory\'s manufacturing process",\n    factory_image,\n)\n```\n---\n\n\n## `Multi Modal Autonomous Agents`\nRun the agent with multiple modalities useful for various real-world tasks in manufacturing, logistics, and health.\n\n```python\n# Description: This is an example of how to use the Agent class to run a multi-modal workflow\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models.gpt4_vision_api import GPT4VisionAPI\nfrom swarms.structs import Agent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = GPT4VisionAPI(\n    openai_api_key=api_key,\n    max_tokens=500,\n)\n\n# Initialize the task\ntask = (\n    "Analyze this image of an assembly line and identify any issues such as"\n    " misaligned parts, defects, or deviations from the standard assembly"\n    " process. IF there is anything unsafe in the image, explain why it is"\n    " unsafe and how it could be improved."\n)\nimg = "assembly_line.jpg"\n\n## Initialize the workflow\nagent = Agent(\n    llm=llm, max_loops="auto", autosave=True, dashboard=True, multi_modal=True\n)\n\n# Run the workflow on a task\nagent.run(task=task, img=img)\n```\n----\n\n\n## Build your own LLMs, Agents, and Swarms!\n\n### Swarms Compliant Model Interface\n```python\nfrom swarms import BaseLLM\n\nclass vLLMLM(BaseLLM):\n    def __init__(self, model_name=\'default_model\', tensor_parallel_size=1, *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.model_name = model_name\n        self.tensor_parallel_size = tensor_parallel_size\n        # Add any additional initialization here\n    \n    def run(self, task: str):\n        pass\n\n# Example\nmodel = vLLMLM("mistral")\n\n# Run the model\nout = model("Analyze these financial documents and summarize of them")\nprint(out)\n\n```\n\n\n### Swarms Compliant Agent Interface\n\n```python\nfrom swarms import Agent\n\n\nclass MyCustomAgent(Agent):\n\n\xa0 \xa0 def __init__(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 super().__init__(*args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Custom initialization logic\n\n\xa0 \xa0 def custom_method(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Implement custom logic here\n\n\xa0 \xa0 \xa0 \xa0 pass\n\n\xa0 \xa0 def run(self, task, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Customize the run method\n\n\xa0 \xa0 \xa0 \xa0 response = super().run(task, *args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Additional custom logic\n\n\xa0 \xa0 \xa0 \xa0 return response`\n\n# Model\nagent = MyCustomAgent()\n\n# Run the agent\nout = agent("Analyze and summarize these financial documents: ")\nprint(out)\n\n```\n\n\n### Compliant Interface for Multi-Agent Collaboration\n\n```python\nfrom swarms import AutoSwarm, AutoSwarmRouter, BaseSwarm\n\n\n# Build your own Swarm\nclass MySwarm(BaseSwarm):\n    def __init__(self, name="kyegomez/myswarm", *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.name = name\n\n    def run(self, task: str, *args, **kwargs):\n        # Add your multi-agent logic here\n        # agent 1\n        # agent 2\n        # agent 3\n        return "output of the swarm"\n\n\n# Add your custom swarm to the AutoSwarmRouter\nrouter = AutoSwarmRouter(\n    swarms=[MySwarm]\n)\n\n\n# Create an AutoSwarm instance\nautoswarm = AutoSwarm(\n    name="kyegomez/myswarm",\n    description="A simple API to build and run swarms",\n    verbose=True,\n    router=router,\n)\n\n\n# Run the AutoSwarm\nautoswarm.run("Analyze these financial data and give me a summary")\n\n\n```\n\n## `AgentRearrange`\nInspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships. [Docs Available:](https://swarms.apac.ai/en/latest/swarms/structs/agent_rearrange/)\n\n```python\nfrom swarms import Agent, AgentRearrange, rearrange, Anthropic\n\n\n# Initialize the director agent\n\ndirector = Agent(\n    agent_name="Director",\n    system_prompt="Directs the tasks for the workers",\n    llm=Anthropic(),\n    max_loops=1,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    state_save_file_type="json",\n    saved_state_path="director.json",\n)\n\n\n# Initialize worker 1\n\nworker1 = Agent(\n    agent_name="Worker1",\n    system_prompt="Generates a transcript for a youtube video on what swarms are",\n    llm=Anthropic(),\n    max_loops=1,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    state_save_file_type="json",\n    saved_state_path="worker1.json",\n)\n\n\n# Initialize worker 2\nworker2 = Agent(\n    agent_name="Worker2",\n    system_prompt="Summarizes the transcript generated by Worker1",\n    llm=Anthropic(),\n    max_loops=1,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    state_save_file_type="json",\n    saved_state_path="worker2.json",\n)\n\n\n# Create a list of agents\nagents = [director, worker1, worker2]\n\n# Define the flow pattern\nflow = "Director -> Worker1 -> Worker2"\n\n# Using AgentRearrange class\nagent_system = AgentRearrange(agents=agents, flow=flow)\noutput = agent_system.run(\n    "Create a format to express and communicate swarms of llms in a structured manner for youtube"\n)\nprint(output)\n\n\n# Using rearrange function\noutput = rearrange(\n    agents,\n    flow,\n    "Create a format to express and communicate swarms of llms in a structured manner for youtube",\n)\n\nprint(output)\n\n```\n\n\n---\n\n## Documentation\nDocumentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)\n\n----\n\n## File Structure\nThe swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs`\xa0that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.\n\n```sh\n├── __init__.py\n├── agents\n├── artifacts\n├── memory\n├── models\n├── prompts\n├── structs\n├── telemetry\n├── tools\n├── utils\n└── workers\n```\n\n----\n\n## 🫶 Contributions:\n\nThe easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)\n\nSwarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!\n\n<a href="https://github.com/kyegomez/swarms/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=kyegomez/swarms" />\n</a>\n\n----\n\n## Community\n\nJoin our growing community around the world, for real-time support, ideas, and discussions on Swarms 😊 \n\n- View our official [Blog](https://swarms.apac.ai)\n- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)\n- Follow us on [Twitter](https://twitter.com/kyegomez)\n- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)\n- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)\n- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)\n- Join our Swarms Community Gathering every Thursday at 1pm NYC Time to unlock the potential of autonomous agents in automating your daily tasks [Sign up here](https://lu.ma/5p2jnc2v)\n\n---\n\n## Discovery Call\nBook a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)\n\n\n## Accelerate Backlog\nAccelerate Bugs, Features, and Demos to implement by supporting us here:\n\n<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>\n\n\n## Docker Instructions\n- [Learn More Here About Deployments In Docker]()\n\n\n## Swarm Newsletter 🤖 🤖 🤖 📧 \nSign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊\n\n\n[CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)\n\n# License\nApache License\n\n\n\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/swarms',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `swarms-5.0.1/PKG-INFO` & `swarms-5.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 5.0.1
+Version: 5.0.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering,swarms,agents
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
@@ -14,22 +14,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: Pillow (==10.3.0)
 Requires-Dist: PyYAML
-Requires-Dist: accelerate (==0.28.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0)
 Requires-Dist: backoff (==2.2.1)
 Requires-Dist: docstring_parser (==0.16)
 Requires-Dist: langchain-community (==0.0.29)
 Requires-Dist: langchain-experimental (==0.0.55)
 Requires-Dist: loguru (==0.7.2)
-Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
+Requires-Dist: opencv-python-headless
 Requires-Dist: psutil
 Requires-Dist: pydantic (==2.7.1)
 Requires-Dist: pypdf (==4.1.0)
 Requires-Dist: python-dotenv
 Requires-Dist: ratelimit (==2.2.1)
 Requires-Dist: sentry-sdk
 Requires-Dist: tenacity (==8.2.3)
@@ -1208,15 +1207,15 @@
 # Run the AutoSwarm
 autoswarm.run("Analyze these financial data and give me a summary")
 
 
 ```
 
 ## `AgentRearrange`
-Inspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships
+Inspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships. [Docs Available:](https://swarms.apac.ai/en/latest/swarms/structs/agent_rearrange/)
 
 ```python
 from swarms import Agent, AgentRearrange, rearrange, Anthropic
 
 
 # Initialize the director agent
 
@@ -1294,14 +1293,33 @@
 ---
 
 ## Documentation
 Documentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)
 
 ----
 
+## File Structure
+The swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs` that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.
+
+```sh
+├── __init__.py
+├── agents
+├── artifacts
+├── memory
+├── models
+├── prompts
+├── structs
+├── telemetry
+├── tools
+├── utils
+└── workers
+```
+
+----
+
 ## 🫶 Contributions:
 
 The easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)
 
 Swarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!
 
 <a href="https://github.com/kyegomez/swarms/graphs/contributors">
@@ -1324,66 +1342,22 @@
 
 ---
 
 ## Discovery Call
 Book a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)
 
 
-
 ## Accelerate Backlog
-Help us accelerate our backlog by supporting us financially! Note, we're an open source corporation and so all the revenue we generate is through donations at the moment ;)
+Accelerate Bugs, Features, and Demos to implement by supporting us here:
 
 <a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>
 
 
-## File Structure
-The swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs` that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.
-
-```sh
-├── __init__.py
-├── agents
-├── artifacts
-├── chunkers
-├── cli
-├── loaders
-├── memory
-├── models
-├── prompts
-├── structs
-├── telemetry
-├── tokenizers
-├── tools
-├── utils
-└── workers
-```
-
 ## Docker Instructions
-
-This application uses Docker with CUDA support. To build and run the Docker container, follow these steps:
-
-### Prerequisites
-
-- Make sure you have [Docker installed](https://docs.docker.com/get-docker/) on your machine.
-- Ensure your machine has an NVIDIA GPU and [NVIDIA Docker support](https://github.com/NVIDIA/nvidia-docker) installed.
-
-### Building the Docker Image
-
-To build the Docker image, navigate to the root directory containing the `Dockerfile` and run the following command:
-
-```bash
-docker build --gpus all -t swarms
-``` 
-### Running the Docker Container
-To run the Docker container, use the following command:
-
-`docker run --gpus all -p 4000:80 swarms`
-
-Replace swarms with the name of your Docker image, and replace 4000:80 with your actual port mapping. The format is hostPort:containerPort.
-
-Now, your application should be running with CUDA support!
+- [Learn More Here About Deployments In Docker]()
 
 
 ## Swarm Newsletter 🤖 🤖 🤖 📧 
 Sign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊
 
 
 [CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)
```

