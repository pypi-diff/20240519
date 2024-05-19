# Comparing `tmp/teams_ai-1.1.0.tar.gz` & `tmp/teams_ai-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teams_ai-1.1.0.tar", max compression
+gzip compressed data, was "teams_ai-1.2.0.tar", max compression
```

## Comparing `teams_ai-1.1.0.tar` & `teams_ai-1.2.0.tar`

### file list

```diff
@@ -1,191 +1,202 @@
--rw-r--r--   0        0        0     1093 2024-02-28 17:27:33.896122 teams_ai-1.1.0/LICENSE
--rw-r--r--   0        0        0     1913 2024-05-09 21:14:19.181479 teams_ai-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1303 2024-04-22 18:27:52.693426 teams_ai-1.1.0/README.md
--rw-r--r--   0        0        0      644 2024-02-28 17:27:33.921639 teams_ai-1.1.0/teams/__init__.py
--rw-r--r--   0        0        0      963 2024-02-28 17:27:33.922639 teams_ai-1.1.0/teams/activity_type.py
--rw-r--r--   0        0        0      386 2024-04-01 15:45:21.915342 teams_ai-1.1.0/teams/adaptive_cards/__init__.py
--rw-r--r--   0        0        0    10816 2024-05-09 16:06:14.138234 teams_ai-1.1.0/teams/adaptive_cards/adaptive_cards.py
--rw-r--r--   0        0        0      471 2024-02-28 17:27:33.941901 teams_ai-1.1.0/teams/adaptive_cards/adaptive_cards_options.py
--rw-r--r--   0        0        0      252 2024-02-28 17:27:33.941901 teams_ai-1.1.0/teams/adaptive_cards/adaptive_cards_search_params.py
--rw-r--r--   0        0        0      344 2024-03-26 18:27:31.042285 teams_ai-1.1.0/teams/adaptive_cards/adaptive_cards_search_result.py
--rw-r--r--   0        0        0      183 2024-02-28 17:27:33.942826 teams_ai-1.1.0/teams/ai/__init__.py
--rw-r--r--   0        0        0      321 2024-02-28 17:27:33.943872 teams_ai-1.1.0/teams/ai/actions/__init__.py
--rw-r--r--   0        0        0     1001 2024-02-28 17:27:33.950724 teams_ai-1.1.0/teams/ai/actions/action_entry.py
--rw-r--r--   0        0        0      641 2024-02-28 17:27:33.950724 teams_ai-1.1.0/teams/ai/actions/action_turn_context.py
--rw-r--r--   0        0        0      502 2024-04-01 15:45:21.927348 teams_ai-1.1.0/teams/ai/actions/action_types.py
--rw-r--r--   0        0        0     9031 2024-05-09 16:06:14.144681 teams_ai-1.1.0/teams/ai/ai.py
--rw-r--r--   0        0        0      903 2024-04-01 15:45:21.942863 teams_ai-1.1.0/teams/ai/ai_options.py
--rw-r--r--   0        0        0      425 2024-02-28 17:27:33.959629 teams_ai-1.1.0/teams/ai/augmentations/__init__.py
--rw-r--r--   0        0        0     1635 2024-03-04 19:10:38.243854 teams_ai-1.1.0/teams/ai/augmentations/augmentation.py
--rw-r--r--   0        0        0     2554 2024-03-04 19:10:38.249089 teams_ai-1.1.0/teams/ai/augmentations/default_augmentation.py
--rw-r--r--   0        0        0    10072 2024-05-09 16:06:14.153198 teams_ai-1.1.0/teams/ai/augmentations/monologue_augmentation.py
--rw-r--r--   0        0        0     7071 2024-03-04 19:10:38.262051 teams_ai-1.1.0/teams/ai/augmentations/sequence_augmentation.py
--rw-r--r--   0        0        0      196 2024-02-28 17:27:33.962205 teams_ai-1.1.0/teams/ai/clients/__init__.py
--rw-r--r--   0        0        0     7231 2024-04-22 18:27:52.706612 teams_ai-1.1.0/teams/ai/clients/llm_client.py
--rw-r--r--   0        0        0      224 2024-02-28 17:27:33.962205 teams_ai-1.1.0/teams/ai/data_sources/__init__.py
--rw-r--r--   0        0        0     1360 2024-03-04 19:10:38.273303 teams_ai-1.1.0/teams/ai/data_sources/data_source.py
--rw-r--r--   0        0        0     2500 2024-03-04 19:10:38.279346 teams_ai-1.1.0/teams/ai/data_sources/text_data_source.py
--rw-r--r--   0        0        0      625 2024-04-01 15:45:21.948864 teams_ai-1.1.0/teams/ai/embeddings/__init__.py
--rw-r--r--   0        0        0     4379 2024-05-09 16:06:14.161855 teams_ai-1.1.0/teams/ai/embeddings/azure_openai_embeddings.py
--rw-r--r--   0        0        0     1048 2024-02-28 17:27:33.962205 teams_ai-1.1.0/teams/ai/embeddings/azure_openai_embeddings_options.py
--rw-r--r--   0        0        0      894 2024-02-28 17:27:33.962205 teams_ai-1.1.0/teams/ai/embeddings/embeddings_model.py
--rw-r--r--   0        0        0      802 2024-02-28 17:27:33.962205 teams_ai-1.1.0/teams/ai/embeddings/embeddings_response.py
--rw-r--r--   0        0        0     3803 2024-02-28 17:27:33.968740 teams_ai-1.1.0/teams/ai/embeddings/openai_embeddings.py
--rw-r--r--   0        0        0      991 2024-02-28 17:27:33.968740 teams_ai-1.1.0/teams/ai/embeddings/openai_embeddings_options.py
--rw-r--r--   0        0        0      562 2024-02-28 17:27:33.968740 teams_ai-1.1.0/teams/ai/models/__init__.py
--rw-r--r--   0        0        0      729 2024-02-28 17:27:33.969778 teams_ai-1.1.0/teams/ai/models/chat_completion_action.py
--rw-r--r--   0        0        0     7173 2024-04-22 18:27:52.713613 teams_ai-1.1.0/teams/ai/models/openai_model.py
--rw-r--r--   0        0        0     1302 2024-03-04 19:10:38.291151 teams_ai-1.1.0/teams/ai/models/prompt_completion_model.py
--rw-r--r--   0        0        0      909 2024-02-28 17:27:33.969778 teams_ai-1.1.0/teams/ai/models/prompt_response.py
--rw-r--r--   0        0        0      557 2024-03-05 21:42:08.164469 teams_ai-1.1.0/teams/ai/moderators/__init__.py
--rw-r--r--   0        0        0     7695 2024-03-26 18:27:31.059067 teams_ai-1.1.0/teams/ai/moderators/azure_content_safety_moderator.py
--rw-r--r--   0        0        0      656 2024-02-28 17:27:33.969778 teams_ai-1.1.0/teams/ai/moderators/default_moderator.py
--rw-r--r--   0        0        0     1589 2024-03-04 19:10:38.297196 teams_ai-1.1.0/teams/ai/moderators/moderator.py
--rw-r--r--   0        0        0     4332 2024-03-05 21:41:32.156765 teams_ai-1.1.0/teams/ai/moderators/openai_moderator.py
--rw-r--r--   0        0        0      735 2024-05-09 15:32:43.716003 teams_ai-1.1.0/teams/ai/planners/__init__.py
--rw-r--r--   0        0        0     6127 2024-04-01 15:45:21.959862 teams_ai-1.1.0/teams/ai/planners/action_planner.py
--rw-r--r--   0        0        0    16702 2024-05-09 15:32:43.716003 teams_ai-1.1.0/teams/ai/planners/assistants_planner.py
--rw-r--r--   0        0        0     2085 2024-02-29 18:07:09.525392 teams_ai-1.1.0/teams/ai/planners/plan.py
--rw-r--r--   0        0        0     1065 2024-04-01 15:45:21.968867 teams_ai-1.1.0/teams/ai/planners/planner.py
--rw-r--r--   0        0        0     1476 2024-02-28 17:27:33.969778 teams_ai-1.1.0/teams/ai/prompts/__init__.py
--rw-r--r--   0        0        0      846 2024-02-28 17:27:33.975341 teams_ai-1.1.0/teams/ai/prompts/assistant_message.py
--rw-r--r--   0        0        0     1066 2024-02-28 17:27:33.975782 teams_ai-1.1.0/teams/ai/prompts/augmentation_config.py
--rw-r--r--   0        0        0     3285 2024-02-28 17:27:33.976301 teams_ai-1.1.0/teams/ai/prompts/completion_config.py
--rw-r--r--   0        0        0      428 2024-02-28 17:27:33.976301 teams_ai-1.1.0/teams/ai/prompts/function_call.py
--rw-r--r--   0        0        0     2992 2024-03-04 19:10:38.315390 teams_ai-1.1.0/teams/ai/prompts/function_call_message.py
--rw-r--r--   0        0        0     3137 2024-03-04 19:10:38.321390 teams_ai-1.1.0/teams/ai/prompts/function_response_message.py
--rw-r--r--   0        0        0     1511 2024-02-28 17:27:33.977950 teams_ai-1.1.0/teams/ai/prompts/message.py
--rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.978714 teams_ai-1.1.0/teams/ai/prompts/prompt.py
--rw-r--r--   0        0        0     2493 2024-03-04 19:10:38.326426 teams_ai-1.1.0/teams/ai/prompts/prompt_functions.py
--rw-r--r--   0        0        0    14509 2024-05-09 16:06:14.171453 teams_ai-1.1.0/teams/ai/prompts/prompt_manager.py
--rw-r--r--   0        0        0     1571 2024-02-28 17:27:33.986946 teams_ai-1.1.0/teams/ai/prompts/prompt_manager_options.py
--rw-r--r--   0        0        0      478 2024-02-28 17:27:33.986946 teams_ai-1.1.0/teams/ai/prompts/prompt_section_layout.py
--rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.988031 teams_ai-1.1.0/teams/ai/prompts/prompt_template.py
--rw-r--r--   0        0        0     2116 2024-02-28 17:27:33.988538 teams_ai-1.1.0/teams/ai/prompts/prompt_template_config.py
--rw-r--r--   0        0        0      614 2024-02-28 17:27:33.988538 teams_ai-1.1.0/teams/ai/prompts/rendered_prompt_section.py
--rw-r--r--   0        0        0      800 2024-02-28 17:27:33.989546 teams_ai-1.1.0/teams/ai/prompts/sections/__init__.py
--rw-r--r--   0        0        0     4104 2024-03-27 21:04:22.804466 teams_ai-1.1.0/teams/ai/prompts/sections/action_augmentation_section.py
--rw-r--r--   0        0        0     6894 2024-03-04 19:10:38.345727 teams_ai-1.1.0/teams/ai/prompts/sections/conversation_history_section.py
--rw-r--r--   0        0        0     2451 2024-03-04 19:10:38.351007 teams_ai-1.1.0/teams/ai/prompts/sections/data_source_section.py
--rw-r--r--   0        0        0     3361 2024-03-04 19:10:38.357972 teams_ai-1.1.0/teams/ai/prompts/sections/group_section.py
--rw-r--r--   0        0        0     9245 2024-03-04 19:10:38.363971 teams_ai-1.1.0/teams/ai/prompts/sections/layout_engine_section.py
--rw-r--r--   0        0        0     2941 2024-03-04 19:10:38.370157 teams_ai-1.1.0/teams/ai/prompts/sections/prompt_section.py
--rw-r--r--   0        0        0     7305 2024-03-04 19:10:38.376193 teams_ai-1.1.0/teams/ai/prompts/sections/prompt_section_base.py
--rw-r--r--   0        0        0     9006 2024-03-04 19:10:38.382234 teams_ai-1.1.0/teams/ai/prompts/sections/template_section.py
--rw-r--r--   0        0        0     3124 2024-03-04 19:10:38.388234 teams_ai-1.1.0/teams/ai/prompts/sections/text_section.py
--rw-r--r--   0        0        0      635 2024-02-28 17:27:33.994231 teams_ai-1.1.0/teams/ai/prompts/system_message.py
--rw-r--r--   0        0        0     4028 2024-03-04 19:10:38.394784 teams_ai-1.1.0/teams/ai/prompts/user_input_message.py
--rw-r--r--   0        0        0      800 2024-02-28 17:27:33.996243 teams_ai-1.1.0/teams/ai/prompts/user_message.py
--rw-r--r--   0        0        0      213 2024-02-28 17:27:33.997052 teams_ai-1.1.0/teams/ai/tokenizers/__init__.py
--rw-r--r--   0        0        0     1071 2024-02-28 17:27:33.998562 teams_ai-1.1.0/teams/ai/tokenizers/gpt_tokenizer.py
--rw-r--r--   0        0        0      993 2024-02-28 17:27:33.999575 teams_ai-1.1.0/teams/ai/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     1436 2024-03-04 19:10:38.399820 teams_ai-1.1.0/teams/ai/utilities.py
--rw-r--r--   0        0        0      621 2024-02-28 17:27:34.000614 teams_ai-1.1.0/teams/ai/validators/__init__.py
--rw-r--r--   0        0        0     4415 2024-05-09 16:06:14.178969 teams_ai-1.1.0/teams/ai/validators/action_response_validator.py
--rw-r--r--   0        0        0      777 2024-03-04 19:10:38.411023 teams_ai-1.1.0/teams/ai/validators/default_response_validator.py
--rw-r--r--   0        0        0     3045 2024-03-26 20:05:45.109561 teams_ai-1.1.0/teams/ai/validators/json_response_validator.py
--rw-r--r--   0        0        0     1286 2024-03-04 19:10:38.423061 teams_ai-1.1.0/teams/ai/validators/prompt_response_validator.py
--rw-r--r--   0        0        0      648 2024-02-28 17:27:34.002010 teams_ai-1.1.0/teams/ai/validators/validation.py
--rw-r--r--   0        0        0    28277 2024-05-09 16:06:14.179970 teams_ai-1.1.0/teams/app.py
--rw-r--r--   0        0        0      296 2024-02-28 17:27:34.013515 teams_ai-1.1.0/teams/app_error.py
--rw-r--r--   0        0        0     2753 2024-05-09 16:06:14.187482 teams_ai-1.1.0/teams/app_options.py
--rw-r--r--   0        0        0      508 2024-05-09 16:06:14.188482 teams_ai-1.1.0/teams/auth/__init__.py
--rw-r--r--   0        0        0     4037 2024-05-09 16:06:14.196032 teams_ai-1.1.0/teams/auth/auth.py
--rw-r--r--   0        0        0     1987 2024-05-09 16:06:14.202995 teams_ai-1.1.0/teams/auth/auth_component.py
--rw-r--r--   0        0        0     4763 2024-05-09 16:06:14.213113 teams_ai-1.1.0/teams/auth/auth_manager.py
--rw-r--r--   0        0        0      702 2024-05-09 16:06:14.214126 teams_ai-1.1.0/teams/auth/auth_options.py
--rw-r--r--   0        0        0      433 2024-05-09 16:06:14.227073 teams_ai-1.1.0/teams/auth/oauth/__init__.py
--rw-r--r--   0        0        0     4090 2024-05-09 16:06:14.238600 teams_ai-1.1.0/teams/auth/oauth/oauth.py
--rw-r--r--   0        0        0     4739 2024-05-09 16:06:14.247705 teams_ai-1.1.0/teams/auth/oauth/oauth_adaptive_card.py
--rw-r--r--   0        0        0     3447 2024-05-09 16:06:14.254248 teams_ai-1.1.0/teams/auth/oauth/oauth_dialog.py
--rw-r--r--   0        0        0     4432 2024-05-09 16:06:14.265765 teams_ai-1.1.0/teams/auth/oauth/oauth_message_extension.py
--rw-r--r--   0        0        0     1303 2024-05-09 16:06:14.278305 teams_ai-1.1.0/teams/auth/oauth/oauth_options.py
--rw-r--r--   0        0        0      448 2024-05-09 16:06:14.285836 teams_ai-1.1.0/teams/auth/sign_in_response.py
--rw-r--r--   0        0        0      148 2024-05-09 16:06:14.299410 teams_ai-1.1.0/teams/dialogs/__init__.py
--rw-r--r--   0        0        0     1810 2024-05-09 16:06:14.300410 teams_ai-1.1.0/teams/dialogs/dialog.py
--rw-r--r--   0        0        0     1137 2024-04-09 18:41:37.993611 teams_ai-1.1.0/teams/input_file.py
--rw-r--r--   0        0        0      154 2024-02-28 17:27:34.020845 teams_ai-1.1.0/teams/meetings/__init__.py
--rw-r--r--   0        0        0     3655 2024-05-09 16:06:14.309928 teams_ai-1.1.0/teams/meetings/meetings.py
--rw-r--r--   0        0        0      228 2024-02-28 17:27:34.029400 teams_ai-1.1.0/teams/message_extensions/__init__.py
--rw-r--r--   0        0        0    24325 2024-05-09 16:06:14.334577 teams_ai-1.1.0/teams/message_extensions/message_extensions.py
--rw-r--r--   0        0        0      241 2024-02-28 17:27:34.039795 teams_ai-1.1.0/teams/message_reaction_types.py
--rw-r--r--   0        0        0        0 2024-02-28 17:27:34.039795 teams_ai-1.1.0/teams/py.typed
--rw-r--r--   0        0        0      328 2024-02-28 17:27:34.041095 teams_ai-1.1.0/teams/query.py
--rw-r--r--   0        0        0      762 2024-02-28 17:27:34.049441 teams_ai-1.1.0/teams/route.py
--rw-r--r--   0        0        0      564 2024-05-09 16:06:14.350682 teams_ai-1.1.0/teams/state/__init__.py
--rw-r--r--   0        0        0     1365 2024-05-09 16:06:14.364841 teams_ai-1.1.0/teams/state/conversation_state.py
--rw-r--r--   0        0        0     3481 2024-03-04 19:10:38.447269 teams_ai-1.1.0/teams/state/memory.py
--rw-r--r--   0        0        0     4884 2024-05-09 16:06:14.379408 teams_ai-1.1.0/teams/state/state.py
--rw-r--r--   0        0        0     1216 2024-05-09 16:06:14.386924 teams_ai-1.1.0/teams/state/temp_state.py
--rw-r--r--   0        0        0      603 2024-05-09 16:06:14.400866 teams_ai-1.1.0/teams/state/todict.py
--rw-r--r--   0        0        0     2466 2024-05-09 16:06:14.423060 teams_ai-1.1.0/teams/state/turn_state.py
--rw-r--r--   0        0        0     1306 2024-05-09 16:06:14.448917 teams_ai-1.1.0/teams/state/user_state.py
--rw-r--r--   0        0        0      239 2024-02-28 17:27:34.059743 teams_ai-1.1.0/teams/task_modules/__init__.py
--rw-r--r--   0        0        0     6431 2024-05-09 16:06:14.474558 teams_ai-1.1.0/teams/task_modules/task_modules.py
--rw-r--r--   0        0        0      488 2024-02-28 17:27:34.071531 teams_ai-1.1.0/teams/task_modules/task_modules_options.py
--rw-r--r--   0        0        0     5793 2024-04-17 20:51:17.950656 teams_ai-1.1.0/teams/teams_adapter.py
--rw-r--r--   0        0        0      325 2024-04-09 18:41:38.006774 teams_ai-1.1.0/teams/teams_attachment_downloader/__init__.py
--rw-r--r--   0        0        0     5533 2024-04-30 21:35:02.331772 teams_ai-1.1.0/teams/teams_attachment_downloader/teams_attachment_downloader.py
--rw-r--r--   0        0        0      463 2024-04-09 18:41:38.022774 teams_ai-1.1.0/teams/teams_attachment_downloader/teams_attachment_downloader_options.py
--rw-r--r--   0        0        0     1190 2024-02-28 17:27:34.072531 teams_ai-1.1.0/teams/typing.py
--rw-r--r--   0        0        0      292 2024-02-28 17:27:34.072531 teams_ai-1.1.0/teams/user_agent.py
--rw-r--r--   0        0        0      200 2024-02-28 17:27:34.073532 teams_ai-1.1.0/teams/utils/json/__init__.py
--rw-r--r--   0        0        0      637 2024-03-27 21:04:22.850998 teams_ai-1.1.0/teams/utils/json/parse.py
--rw-r--r--   0        0        0     1747 2024-02-28 17:27:34.074530 teams_ai-1.1.0/teams/utils/json/parse_object.py
--rw-r--r--   0        0        0     4966 2024-04-01 15:45:22.007862 teams_ai-1.1.0/tests/adaptive_cards/test_adaptive_cards.py
--rw-r--r--   0        0        0     2746 2024-02-28 17:27:34.075531 teams_ai-1.1.0/tests/ai/augmentations/test_default_augmentation.py
--rw-r--r--   0        0        0     6562 2024-03-27 21:04:22.882484 teams_ai-1.1.0/tests/ai/augmentations/test_monologue_augmentation.py
--rw-r--r--   0        0        0     7587 2024-03-04 19:10:38.474809 teams_ai-1.1.0/tests/ai/augmentations/test_sequence_augmentation.py
--rw-r--r--   0        0        0     8034 2024-05-09 16:06:14.498221 teams_ai-1.1.0/tests/ai/clients/test_llm_client.py
--rw-r--r--   0        0        0     1502 2024-02-28 17:27:34.077308 teams_ai-1.1.0/tests/ai/data_sources/test_text_data_source.py
--rw-r--r--   0        0        0     6111 2024-04-01 15:45:22.009865 teams_ai-1.1.0/tests/ai/embeddings/test_azure_openai_embeddings.py
--rw-r--r--   0        0        0     5222 2024-04-01 15:45:22.009865 teams_ai-1.1.0/tests/ai/embeddings/test_openai_embeddings.py
--rw-r--r--   0        0        0     5006 2024-02-28 17:27:34.078742 teams_ai-1.1.0/tests/ai/models/test_openai_model.py
--rw-r--r--   0        0        0     6927 2024-03-26 18:27:31.075685 teams_ai-1.1.0/tests/ai/moderators/test_azure_content_safety_moderator.py
--rw-r--r--   0        0        0      828 2024-02-28 17:27:34.079758 teams_ai-1.1.0/tests/ai/moderators/test_default_moderator.py
--rw-r--r--   0        0        0     9480 2024-03-04 19:10:38.486811 teams_ai-1.1.0/tests/ai/moderators/test_openai_moderator.py
--rw-r--r--   0        0        0    32822 2024-05-09 16:06:14.508755 teams_ai-1.1.0/tests/ai/planners/test_assistants_planner.py
--rw-r--r--   0        0        0      692 2024-02-28 17:27:34.081309 teams_ai-1.1.0/tests/ai/prompts/test_assets/happy_path/actions.json
--rw-r--r--   0        0        0      587 2024-02-28 17:27:34.081309 teams_ai-1.1.0/tests/ai/prompts/test_assets/happy_path/config.json
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.1.0/tests/ai/prompts/test_assets/happy_path/skprompt.txt
--rw-r--r--   0        0        0      614 2024-02-28 17:27:34.082314 teams_ai-1.1.0/tests/ai/prompts/test_assets/include_images/config.json
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.1.0/tests/ai/prompts/test_assets/include_images/skprompt.txt
--rw-r--r--   0        0        0      366 2024-02-28 17:27:34.083314 teams_ai-1.1.0/tests/ai/prompts/test_assets/migrate_old_schema/config.json
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.083314 teams_ai-1.1.0/tests/ai/prompts/test_assets/migrate_old_schema/skprompt.txt
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.084313 teams_ai-1.1.0/tests/ai/prompts/test_assets/no_config/skprompt.txt
--rw-r--r--   0        0        0      582 2024-02-28 17:27:34.084313 teams_ai-1.1.0/tests/ai/prompts/test_assets/no_prompt/config.json
--rw-r--r--   0        0        0     1164 2024-02-28 17:27:34.085314 teams_ai-1.1.0/tests/ai/prompts/test_assistant_message.py
--rw-r--r--   0        0        0     7157 2024-03-04 19:10:38.492599 teams_ai-1.1.0/tests/ai/prompts/test_conversation_history.py
--rw-r--r--   0        0        0     1560 2024-02-28 17:27:34.085423 teams_ai-1.1.0/tests/ai/prompts/test_data_source_section.py
--rw-r--r--   0        0        0     2175 2024-02-28 17:27:34.085423 teams_ai-1.1.0/tests/ai/prompts/test_function_call_message.py
--rw-r--r--   0        0        0     2221 2024-02-28 17:27:34.086488 teams_ai-1.1.0/tests/ai/prompts/test_function_response_message.py
--rw-r--r--   0        0        0     2807 2024-02-28 17:27:34.086488 teams_ai-1.1.0/tests/ai/prompts/test_group_section.py
--rw-r--r--   0        0        0     6968 2024-02-28 17:27:34.086488 teams_ai-1.1.0/tests/ai/prompts/test_layout_engine.py
--rw-r--r--   0        0        0     9534 2024-05-09 16:06:14.528136 teams_ai-1.1.0/tests/ai/prompts/test_prompt_manager_v2.py
--rw-r--r--   0        0        0     8405 2024-02-28 17:27:34.087490 teams_ai-1.1.0/tests/ai/prompts/test_prompt_section_base.py
--rw-r--r--   0        0        0     1056 2024-02-28 17:27:34.087490 teams_ai-1.1.0/tests/ai/prompts/test_system_message.py
--rw-r--r--   0        0        0     9290 2024-03-04 19:10:38.503635 teams_ai-1.1.0/tests/ai/prompts/test_template_section.py
--rw-r--r--   0        0        0     2319 2024-02-28 17:27:34.088994 teams_ai-1.1.0/tests/ai/prompts/test_text_section.py
--rw-r--r--   0        0        0     7349 2024-03-04 19:10:38.509640 teams_ai-1.1.0/tests/ai/prompts/test_user_input_message.py
--rw-r--r--   0        0        0     1048 2024-02-28 17:27:34.089504 teams_ai-1.1.0/tests/ai/prompts/test_user_message.py
--rw-r--r--   0        0        0     1457 2024-02-28 17:27:34.089504 teams_ai-1.1.0/tests/ai/test_utilities.py
--rw-r--r--   0        0        0      853 2024-02-28 17:27:34.089504 teams_ai-1.1.0/tests/ai/tokenizers/test_gpt_tokenizer.py
--rw-r--r--   0        0        0     6169 2024-02-28 17:27:34.090510 teams_ai-1.1.0/tests/ai/validators/test_action_response_validator.py
--rw-r--r--   0        0        0      822 2024-02-28 17:27:34.090510 teams_ai-1.1.0/tests/ai/validators/test_default_response_validator.py
--rw-r--r--   0        0        0     5196 2024-02-28 17:27:34.091510 teams_ai-1.1.0/tests/ai/validators/test_json_response_validator.py
--rw-r--r--   0        0        0     2643 2024-05-09 16:06:14.538656 teams_ai-1.1.0/tests/auth/test_auth_manager.py
--rw-r--r--   0        0        0     4144 2024-03-26 18:27:31.075685 teams_ai-1.1.0/tests/state/test_conversation_state.py
--rw-r--r--   0        0        0     6282 2024-05-09 16:06:14.552991 teams_ai-1.1.0/tests/state/test_custom_turn_state.py
--rw-r--r--   0        0        0      818 2024-05-09 16:06:14.565573 teams_ai-1.1.0/tests/state/test_state.py
--rw-r--r--   0        0        0     1797 2024-04-10 20:07:23.487380 teams_ai-1.1.0/tests/state/test_temp_state.py
--rw-r--r--   0        0        0     6677 2024-05-09 16:06:14.583128 teams_ai-1.1.0/tests/state/test_turn_state.py
--rw-r--r--   0        0        0     3692 2024-03-26 18:27:31.099741 teams_ai-1.1.0/tests/state/test_user_state.py
--rw-r--r--   0        0        0     2250 2024-04-01 15:45:22.019885 teams_ai-1.1.0/tests/task_modules/test_task_modules.py
--rw-r--r--   0        0        0    30053 2024-04-25 20:02:47.968168 teams_ai-1.1.0/tests/test_app.py
--rw-r--r--   0        0        0    11702 2024-02-28 17:27:34.096123 teams_ai-1.1.0/tests/test_meetings.py
--rw-r--r--   0        0        0    32052 2024-02-28 17:27:34.106581 teams_ai-1.1.0/tests/test_message_extensions.py
--rw-r--r--   0        0        0    14794 2024-05-06 18:56:24.275371 teams_ai-1.1.0/tests/test_teams_attachment_downloader.py
--rw-r--r--   0        0        0      146 2024-02-28 17:27:34.106581 teams_ai-1.1.0/tests/utils/__init__.py
--rw-r--r--   0        0        0      526 2024-02-28 17:27:34.107578 teams_ai-1.1.0/tests/utils/activity.py
--rw-r--r--   0        0        0     1055 2024-02-28 17:27:34.107578 teams_ai-1.1.0/tests/utils/adapter.py
--rw-r--r--   0        0        0     2774 1970-01-01 00:00:00.000000 teams_ai-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-02-28 17:27:33.896122 teams_ai-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1913 2024-05-19 16:24:12.447072 teams_ai-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1303 2024-04-22 18:27:52.693426 teams_ai-1.2.0/README.md
+-rw-r--r--   0        0        0      644 2024-02-28 17:27:33.921639 teams_ai-1.2.0/teams/__init__.py
+-rw-r--r--   0        0        0      963 2024-02-28 17:27:33.922639 teams_ai-1.2.0/teams/activity_type.py
+-rw-r--r--   0        0        0      386 2024-04-01 15:45:21.915342 teams_ai-1.2.0/teams/adaptive_cards/__init__.py
+-rw-r--r--   0        0        0    10816 2024-05-09 16:06:14.138234 teams_ai-1.2.0/teams/adaptive_cards/adaptive_cards.py
+-rw-r--r--   0        0        0      471 2024-02-28 17:27:33.941901 teams_ai-1.2.0/teams/adaptive_cards/adaptive_cards_options.py
+-rw-r--r--   0        0        0      252 2024-02-28 17:27:33.941901 teams_ai-1.2.0/teams/adaptive_cards/adaptive_cards_search_params.py
+-rw-r--r--   0        0        0      344 2024-03-26 18:27:31.042285 teams_ai-1.2.0/teams/adaptive_cards/adaptive_cards_search_result.py
+-rw-r--r--   0        0        0      183 2024-02-28 17:27:33.942826 teams_ai-1.2.0/teams/ai/__init__.py
+-rw-r--r--   0        0        0      321 2024-02-28 17:27:33.943872 teams_ai-1.2.0/teams/ai/actions/__init__.py
+-rw-r--r--   0        0        0     1001 2024-02-28 17:27:33.950724 teams_ai-1.2.0/teams/ai/actions/action_entry.py
+-rw-r--r--   0        0        0      641 2024-02-28 17:27:33.950724 teams_ai-1.2.0/teams/ai/actions/action_turn_context.py
+-rw-r--r--   0        0        0      502 2024-04-01 15:45:21.927348 teams_ai-1.2.0/teams/ai/actions/action_types.py
+-rw-r--r--   0        0        0    11573 2024-05-19 16:00:23.389691 teams_ai-1.2.0/teams/ai/ai.py
+-rw-r--r--   0        0        0     1098 2024-05-17 17:55:44.050297 teams_ai-1.2.0/teams/ai/ai_options.py
+-rw-r--r--   0        0        0      425 2024-02-28 17:27:33.959629 teams_ai-1.2.0/teams/ai/augmentations/__init__.py
+-rw-r--r--   0        0        0     1635 2024-03-04 19:10:38.243854 teams_ai-1.2.0/teams/ai/augmentations/augmentation.py
+-rw-r--r--   0        0        0     2498 2024-05-17 17:55:44.057323 teams_ai-1.2.0/teams/ai/augmentations/default_augmentation.py
+-rw-r--r--   0        0        0    10375 2024-05-17 17:55:44.063332 teams_ai-1.2.0/teams/ai/augmentations/monologue_augmentation.py
+-rw-r--r--   0        0        0     8367 2024-05-17 20:39:33.692426 teams_ai-1.2.0/teams/ai/augmentations/sequence_augmentation.py
+-rw-r--r--   0        0        0      259 2024-05-17 17:55:44.068694 teams_ai-1.2.0/teams/ai/citations/__init__.py
+-rw-r--r--   0        0        0     3262 2024-05-19 15:15:30.527486 teams_ai-1.2.0/teams/ai/citations/citations.py
+-rw-r--r--   0        0        0      196 2024-02-28 17:27:33.962205 teams_ai-1.2.0/teams/ai/clients/__init__.py
+-rw-r--r--   0        0        0     7231 2024-04-22 18:27:52.706612 teams_ai-1.2.0/teams/ai/clients/llm_client.py
+-rw-r--r--   0        0        0      224 2024-02-28 17:27:33.962205 teams_ai-1.2.0/teams/ai/data_sources/__init__.py
+-rw-r--r--   0        0        0     1360 2024-03-04 19:10:38.273303 teams_ai-1.2.0/teams/ai/data_sources/data_source.py
+-rw-r--r--   0        0        0     2500 2024-03-04 19:10:38.279346 teams_ai-1.2.0/teams/ai/data_sources/text_data_source.py
+-rw-r--r--   0        0        0      625 2024-04-01 15:45:21.948864 teams_ai-1.2.0/teams/ai/embeddings/__init__.py
+-rw-r--r--   0        0        0     4379 2024-05-09 16:06:14.161855 teams_ai-1.2.0/teams/ai/embeddings/azure_openai_embeddings.py
+-rw-r--r--   0        0        0     1048 2024-02-28 17:27:33.962205 teams_ai-1.2.0/teams/ai/embeddings/azure_openai_embeddings_options.py
+-rw-r--r--   0        0        0      894 2024-02-28 17:27:33.962205 teams_ai-1.2.0/teams/ai/embeddings/embeddings_model.py
+-rw-r--r--   0        0        0      802 2024-02-28 17:27:33.962205 teams_ai-1.2.0/teams/ai/embeddings/embeddings_response.py
+-rw-r--r--   0        0        0     3803 2024-02-28 17:27:33.968740 teams_ai-1.2.0/teams/ai/embeddings/openai_embeddings.py
+-rw-r--r--   0        0        0      991 2024-02-28 17:27:33.968740 teams_ai-1.2.0/teams/ai/embeddings/openai_embeddings_options.py
+-rw-r--r--   0        0        0      562 2024-02-28 17:27:33.968740 teams_ai-1.2.0/teams/ai/models/__init__.py
+-rw-r--r--   0        0        0      729 2024-02-28 17:27:33.969778 teams_ai-1.2.0/teams/ai/models/chat_completion_action.py
+-rw-r--r--   0        0        0     7171 2024-05-17 17:55:44.085383 teams_ai-1.2.0/teams/ai/models/openai_model.py
+-rw-r--r--   0        0        0     1302 2024-03-04 19:10:38.291151 teams_ai-1.2.0/teams/ai/models/prompt_completion_model.py
+-rw-r--r--   0        0        0      909 2024-02-28 17:27:33.969778 teams_ai-1.2.0/teams/ai/models/prompt_response.py
+-rw-r--r--   0        0        0      557 2024-03-05 21:42:08.164469 teams_ai-1.2.0/teams/ai/moderators/__init__.py
+-rw-r--r--   0        0        0     7891 2024-05-17 17:55:44.085383 teams_ai-1.2.0/teams/ai/moderators/azure_content_safety_moderator.py
+-rw-r--r--   0        0        0      656 2024-02-28 17:27:33.969778 teams_ai-1.2.0/teams/ai/moderators/default_moderator.py
+-rw-r--r--   0        0        0     1589 2024-03-04 19:10:38.297196 teams_ai-1.2.0/teams/ai/moderators/moderator.py
+-rw-r--r--   0        0        0     4414 2024-05-17 17:55:44.105897 teams_ai-1.2.0/teams/ai/moderators/openai_moderator.py
+-rw-r--r--   0        0        0      735 2024-05-09 15:32:43.716003 teams_ai-1.2.0/teams/ai/planners/__init__.py
+-rw-r--r--   0        0        0     6127 2024-04-01 15:45:21.959862 teams_ai-1.2.0/teams/ai/planners/action_planner.py
+-rw-r--r--   0        0        0    17927 2024-05-17 17:55:44.111974 teams_ai-1.2.0/teams/ai/planners/assistants_planner.py
+-rw-r--r--   0        0        0     2173 2024-05-17 17:55:44.117935 teams_ai-1.2.0/teams/ai/planners/plan.py
+-rw-r--r--   0        0        0     1065 2024-04-01 15:45:21.968867 teams_ai-1.2.0/teams/ai/planners/planner.py
+-rw-r--r--   0        0        0     1569 2024-05-17 17:55:44.125664 teams_ai-1.2.0/teams/ai/prompts/__init__.py
+-rw-r--r--   0        0        0      846 2024-02-28 17:27:33.975341 teams_ai-1.2.0/teams/ai/prompts/assistant_message.py
+-rw-r--r--   0        0        0     1066 2024-02-28 17:27:33.975782 teams_ai-1.2.0/teams/ai/prompts/augmentation_config.py
+-rw-r--r--   0        0        0     3285 2024-02-28 17:27:33.976301 teams_ai-1.2.0/teams/ai/prompts/completion_config.py
+-rw-r--r--   0        0        0      428 2024-02-28 17:27:33.976301 teams_ai-1.2.0/teams/ai/prompts/function_call.py
+-rw-r--r--   0        0        0     2992 2024-03-04 19:10:38.315390 teams_ai-1.2.0/teams/ai/prompts/function_call_message.py
+-rw-r--r--   0        0        0     3144 2024-05-17 17:55:44.132002 teams_ai-1.2.0/teams/ai/prompts/function_response_message.py
+-rw-r--r--   0        0        0     2310 2024-05-17 18:22:32.407079 teams_ai-1.2.0/teams/ai/prompts/message.py
+-rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.978714 teams_ai-1.2.0/teams/ai/prompts/prompt.py
+-rw-r--r--   0        0        0     2493 2024-03-04 19:10:38.326426 teams_ai-1.2.0/teams/ai/prompts/prompt_functions.py
+-rw-r--r--   0        0        0    14509 2024-05-09 16:06:14.171453 teams_ai-1.2.0/teams/ai/prompts/prompt_manager.py
+-rw-r--r--   0        0        0     1571 2024-02-28 17:27:33.986946 teams_ai-1.2.0/teams/ai/prompts/prompt_manager_options.py
+-rw-r--r--   0        0        0      478 2024-02-28 17:27:33.986946 teams_ai-1.2.0/teams/ai/prompts/prompt_section_layout.py
+-rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.988031 teams_ai-1.2.0/teams/ai/prompts/prompt_template.py
+-rw-r--r--   0        0        0     2116 2024-02-28 17:27:33.988538 teams_ai-1.2.0/teams/ai/prompts/prompt_template_config.py
+-rw-r--r--   0        0        0      614 2024-02-28 17:27:33.988538 teams_ai-1.2.0/teams/ai/prompts/rendered_prompt_section.py
+-rw-r--r--   0        0        0      800 2024-02-28 17:27:33.989546 teams_ai-1.2.0/teams/ai/prompts/sections/__init__.py
+-rw-r--r--   0        0        0     4104 2024-03-27 21:04:22.804466 teams_ai-1.2.0/teams/ai/prompts/sections/action_augmentation_section.py
+-rw-r--r--   0        0        0     6901 2024-05-17 17:55:44.145986 teams_ai-1.2.0/teams/ai/prompts/sections/conversation_history_section.py
+-rw-r--r--   0        0        0     2451 2024-03-04 19:10:38.351007 teams_ai-1.2.0/teams/ai/prompts/sections/data_source_section.py
+-rw-r--r--   0        0        0     3361 2024-03-04 19:10:38.357972 teams_ai-1.2.0/teams/ai/prompts/sections/group_section.py
+-rw-r--r--   0        0        0     9245 2024-03-04 19:10:38.363971 teams_ai-1.2.0/teams/ai/prompts/sections/layout_engine_section.py
+-rw-r--r--   0        0        0     2941 2024-03-04 19:10:38.370157 teams_ai-1.2.0/teams/ai/prompts/sections/prompt_section.py
+-rw-r--r--   0        0        0     7305 2024-03-04 19:10:38.376193 teams_ai-1.2.0/teams/ai/prompts/sections/prompt_section_base.py
+-rw-r--r--   0        0        0     9013 2024-05-17 17:55:44.153293 teams_ai-1.2.0/teams/ai/prompts/sections/template_section.py
+-rw-r--r--   0        0        0     3124 2024-03-04 19:10:38.388234 teams_ai-1.2.0/teams/ai/prompts/sections/text_section.py
+-rw-r--r--   0        0        0      635 2024-02-28 17:27:33.994231 teams_ai-1.2.0/teams/ai/prompts/system_message.py
+-rw-r--r--   0        0        0     4028 2024-03-04 19:10:38.394784 teams_ai-1.2.0/teams/ai/prompts/user_input_message.py
+-rw-r--r--   0        0        0      800 2024-02-28 17:27:33.996243 teams_ai-1.2.0/teams/ai/prompts/user_message.py
+-rw-r--r--   0        0        0      213 2024-02-28 17:27:33.997052 teams_ai-1.2.0/teams/ai/tokenizers/__init__.py
+-rw-r--r--   0        0        0     1071 2024-02-28 17:27:33.998562 teams_ai-1.2.0/teams/ai/tokenizers/gpt_tokenizer.py
+-rw-r--r--   0        0        0      993 2024-02-28 17:27:33.999575 teams_ai-1.2.0/teams/ai/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0      621 2024-02-28 17:27:34.000614 teams_ai-1.2.0/teams/ai/validators/__init__.py
+-rw-r--r--   0        0        0     4415 2024-05-09 16:06:14.178969 teams_ai-1.2.0/teams/ai/validators/action_response_validator.py
+-rw-r--r--   0        0        0      777 2024-03-04 19:10:38.411023 teams_ai-1.2.0/teams/ai/validators/default_response_validator.py
+-rw-r--r--   0        0        0     3045 2024-03-26 20:05:45.109561 teams_ai-1.2.0/teams/ai/validators/json_response_validator.py
+-rw-r--r--   0        0        0     1286 2024-03-04 19:10:38.423061 teams_ai-1.2.0/teams/ai/validators/prompt_response_validator.py
+-rw-r--r--   0        0        0      648 2024-02-28 17:27:34.002010 teams_ai-1.2.0/teams/ai/validators/validation.py
+-rw-r--r--   0        0        0    28277 2024-05-09 16:06:14.179970 teams_ai-1.2.0/teams/app.py
+-rw-r--r--   0        0        0      296 2024-02-28 17:27:34.013515 teams_ai-1.2.0/teams/app_error.py
+-rw-r--r--   0        0        0     2753 2024-05-09 16:06:14.187482 teams_ai-1.2.0/teams/app_options.py
+-rw-r--r--   0        0        0      508 2024-05-09 16:06:14.188482 teams_ai-1.2.0/teams/auth/__init__.py
+-rw-r--r--   0        0        0     4037 2024-05-09 16:06:14.196032 teams_ai-1.2.0/teams/auth/auth.py
+-rw-r--r--   0        0        0     1987 2024-05-09 16:06:14.202995 teams_ai-1.2.0/teams/auth/auth_component.py
+-rw-r--r--   0        0        0     4763 2024-05-09 16:06:14.213113 teams_ai-1.2.0/teams/auth/auth_manager.py
+-rw-r--r--   0        0        0      702 2024-05-09 16:06:14.214126 teams_ai-1.2.0/teams/auth/auth_options.py
+-rw-r--r--   0        0        0      433 2024-05-09 16:06:14.227073 teams_ai-1.2.0/teams/auth/oauth/__init__.py
+-rw-r--r--   0        0        0     4090 2024-05-09 16:06:14.238600 teams_ai-1.2.0/teams/auth/oauth/oauth.py
+-rw-r--r--   0        0        0     4739 2024-05-09 16:06:14.247705 teams_ai-1.2.0/teams/auth/oauth/oauth_adaptive_card.py
+-rw-r--r--   0        0        0     3447 2024-05-09 16:06:14.254248 teams_ai-1.2.0/teams/auth/oauth/oauth_dialog.py
+-rw-r--r--   0        0        0     4432 2024-05-09 16:06:14.265765 teams_ai-1.2.0/teams/auth/oauth/oauth_message_extension.py
+-rw-r--r--   0        0        0     1303 2024-05-09 16:06:14.278305 teams_ai-1.2.0/teams/auth/oauth/oauth_options.py
+-rw-r--r--   0        0        0      448 2024-05-09 16:06:14.285836 teams_ai-1.2.0/teams/auth/sign_in_response.py
+-rw-r--r--   0        0        0      148 2024-05-09 16:06:14.299410 teams_ai-1.2.0/teams/dialogs/__init__.py
+-rw-r--r--   0        0        0     1810 2024-05-09 16:06:14.300410 teams_ai-1.2.0/teams/dialogs/dialog.py
+-rw-r--r--   0        0        0     1137 2024-04-09 18:41:37.993611 teams_ai-1.2.0/teams/input_file.py
+-rw-r--r--   0        0        0      154 2024-02-28 17:27:34.020845 teams_ai-1.2.0/teams/meetings/__init__.py
+-rw-r--r--   0        0        0     3655 2024-05-09 16:06:14.309928 teams_ai-1.2.0/teams/meetings/meetings.py
+-rw-r--r--   0        0        0      228 2024-02-28 17:27:34.029400 teams_ai-1.2.0/teams/message_extensions/__init__.py
+-rw-r--r--   0        0        0    24325 2024-05-09 16:06:14.334577 teams_ai-1.2.0/teams/message_extensions/message_extensions.py
+-rw-r--r--   0        0        0      241 2024-02-28 17:27:34.039795 teams_ai-1.2.0/teams/message_reaction_types.py
+-rw-r--r--   0        0        0        0 2024-02-28 17:27:34.039795 teams_ai-1.2.0/teams/py.typed
+-rw-r--r--   0        0        0      328 2024-02-28 17:27:34.041095 teams_ai-1.2.0/teams/query.py
+-rw-r--r--   0        0        0      762 2024-02-28 17:27:34.049441 teams_ai-1.2.0/teams/route.py
+-rw-r--r--   0        0        0      564 2024-05-09 16:06:14.350682 teams_ai-1.2.0/teams/state/__init__.py
+-rw-r--r--   0        0        0     1365 2024-05-09 16:06:14.364841 teams_ai-1.2.0/teams/state/conversation_state.py
+-rw-r--r--   0        0        0     3481 2024-03-04 19:10:38.447269 teams_ai-1.2.0/teams/state/memory.py
+-rw-r--r--   0        0        0     4830 2024-05-17 20:39:33.708046 teams_ai-1.2.0/teams/state/state.py
+-rw-r--r--   0        0        0     1216 2024-05-09 16:06:14.386924 teams_ai-1.2.0/teams/state/temp_state.py
+-rw-r--r--   0        0        0      691 2024-05-17 20:39:33.708046 teams_ai-1.2.0/teams/state/todict.py
+-rw-r--r--   0        0        0     2466 2024-05-09 16:06:14.423060 teams_ai-1.2.0/teams/state/turn_state.py
+-rw-r--r--   0        0        0     1306 2024-05-09 16:06:14.448917 teams_ai-1.2.0/teams/state/user_state.py
+-rw-r--r--   0        0        0      239 2024-02-28 17:27:34.059743 teams_ai-1.2.0/teams/task_modules/__init__.py
+-rw-r--r--   0        0        0     6431 2024-05-09 16:06:14.474558 teams_ai-1.2.0/teams/task_modules/task_modules.py
+-rw-r--r--   0        0        0      488 2024-02-28 17:27:34.071531 teams_ai-1.2.0/teams/task_modules/task_modules_options.py
+-rw-r--r--   0        0        0     5793 2024-04-17 20:51:17.950656 teams_ai-1.2.0/teams/teams_adapter.py
+-rw-r--r--   0        0        0      325 2024-04-09 18:41:38.006774 teams_ai-1.2.0/teams/teams_attachment_downloader/__init__.py
+-rw-r--r--   0        0        0     5533 2024-04-30 21:35:02.331772 teams_ai-1.2.0/teams/teams_attachment_downloader/teams_attachment_downloader.py
+-rw-r--r--   0        0        0      463 2024-04-09 18:41:38.022774 teams_ai-1.2.0/teams/teams_attachment_downloader/teams_attachment_downloader_options.py
+-rw-r--r--   0        0        0     1190 2024-02-28 17:27:34.072531 teams_ai-1.2.0/teams/typing.py
+-rw-r--r--   0        0        0      292 2024-02-28 17:27:34.072531 teams_ai-1.2.0/teams/user_agent.py
+-rw-r--r--   0        0        0      197 2024-05-17 17:55:44.171941 teams_ai-1.2.0/teams/utils/__init__.py
+-rw-r--r--   0        0        0      278 2024-05-17 17:55:44.177941 teams_ai-1.2.0/teams/utils/citations/__init__.py
+-rw-r--r--   0        0        0      409 2024-05-17 17:55:44.183908 teams_ai-1.2.0/teams/utils/citations/format_citations_response.py
+-rw-r--r--   0        0        0     1043 2024-05-17 17:55:44.190030 teams_ai-1.2.0/teams/utils/citations/get_used_citations.py
+-rw-r--r--   0        0        0      200 2024-02-28 17:27:34.073532 teams_ai-1.2.0/teams/utils/json/__init__.py
+-rw-r--r--   0        0        0      637 2024-03-27 21:04:22.850998 teams_ai-1.2.0/teams/utils/json/parse.py
+-rw-r--r--   0        0        0     1747 2024-02-28 17:27:34.074530 teams_ai-1.2.0/teams/utils/json/parse_object.py
+-rw-r--r--   0        0        0      631 2024-05-17 17:55:44.196030 teams_ai-1.2.0/teams/utils/snippet.py
+-rw-r--r--   0        0        0     1440 2024-05-17 17:55:44.234170 teams_ai-1.2.0/teams/utils/to_string.py
+-rw-r--r--   0        0        0     4966 2024-04-01 15:45:22.007862 teams_ai-1.2.0/tests/adaptive_cards/test_adaptive_cards.py
+-rw-r--r--   0        0        0     2907 2024-05-17 17:55:44.235304 teams_ai-1.2.0/tests/ai/augmentations/test_default_augmentation.py
+-rw-r--r--   0        0        0     6693 2024-05-17 17:55:44.252006 teams_ai-1.2.0/tests/ai/augmentations/test_monologue_augmentation.py
+-rw-r--r--   0        0        0     7935 2024-05-17 17:55:44.252006 teams_ai-1.2.0/tests/ai/augmentations/test_sequence_augmentation.py
+-rw-r--r--   0        0        0     8034 2024-05-09 16:06:14.498221 teams_ai-1.2.0/tests/ai/clients/test_llm_client.py
+-rw-r--r--   0        0        0     1502 2024-02-28 17:27:34.077308 teams_ai-1.2.0/tests/ai/data_sources/test_text_data_source.py
+-rw-r--r--   0        0        0     6111 2024-04-01 15:45:22.009865 teams_ai-1.2.0/tests/ai/embeddings/test_azure_openai_embeddings.py
+-rw-r--r--   0        0        0     5222 2024-04-01 15:45:22.009865 teams_ai-1.2.0/tests/ai/embeddings/test_openai_embeddings.py
+-rw-r--r--   0        0        0     5006 2024-02-28 17:27:34.078742 teams_ai-1.2.0/tests/ai/models/test_openai_model.py
+-rw-r--r--   0        0        0     7158 2024-05-17 17:55:44.270261 teams_ai-1.2.0/tests/ai/moderators/test_azure_content_safety_moderator.py
+-rw-r--r--   0        0        0      828 2024-02-28 17:27:34.079758 teams_ai-1.2.0/tests/ai/moderators/test_default_moderator.py
+-rw-r--r--   0        0        0     9711 2024-05-17 17:55:44.291261 teams_ai-1.2.0/tests/ai/moderators/test_openai_moderator.py
+-rw-r--r--   0        0        0    33818 2024-05-19 16:32:37.955319 teams_ai-1.2.0/tests/ai/planners/test_assistants_planner.py
+-rw-r--r--   0        0        0      692 2024-02-28 17:27:34.081309 teams_ai-1.2.0/tests/ai/prompts/test_assets/happy_path/actions.json
+-rw-r--r--   0        0        0      587 2024-02-28 17:27:34.081309 teams_ai-1.2.0/tests/ai/prompts/test_assets/happy_path/config.json
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.2.0/tests/ai/prompts/test_assets/happy_path/skprompt.txt
+-rw-r--r--   0        0        0      614 2024-02-28 17:27:34.082314 teams_ai-1.2.0/tests/ai/prompts/test_assets/include_images/config.json
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.2.0/tests/ai/prompts/test_assets/include_images/skprompt.txt
+-rw-r--r--   0        0        0      366 2024-02-28 17:27:34.083314 teams_ai-1.2.0/tests/ai/prompts/test_assets/migrate_old_schema/config.json
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.083314 teams_ai-1.2.0/tests/ai/prompts/test_assets/migrate_old_schema/skprompt.txt
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.084313 teams_ai-1.2.0/tests/ai/prompts/test_assets/no_config/skprompt.txt
+-rw-r--r--   0        0        0      582 2024-02-28 17:27:34.084313 teams_ai-1.2.0/tests/ai/prompts/test_assets/no_prompt/config.json
+-rw-r--r--   0        0        0     1164 2024-02-28 17:27:34.085314 teams_ai-1.2.0/tests/ai/prompts/test_assistant_message.py
+-rw-r--r--   0        0        0     7157 2024-03-04 19:10:38.492599 teams_ai-1.2.0/tests/ai/prompts/test_conversation_history.py
+-rw-r--r--   0        0        0     1560 2024-02-28 17:27:34.085423 teams_ai-1.2.0/tests/ai/prompts/test_data_source_section.py
+-rw-r--r--   0        0        0     2175 2024-02-28 17:27:34.085423 teams_ai-1.2.0/tests/ai/prompts/test_function_call_message.py
+-rw-r--r--   0        0        0     2221 2024-02-28 17:27:34.086488 teams_ai-1.2.0/tests/ai/prompts/test_function_response_message.py
+-rw-r--r--   0        0        0     2807 2024-02-28 17:27:34.086488 teams_ai-1.2.0/tests/ai/prompts/test_group_section.py
+-rw-r--r--   0        0        0     6968 2024-02-28 17:27:34.086488 teams_ai-1.2.0/tests/ai/prompts/test_layout_engine.py
+-rw-r--r--   0        0        0     9534 2024-05-09 16:06:14.528136 teams_ai-1.2.0/tests/ai/prompts/test_prompt_manager_v2.py
+-rw-r--r--   0        0        0     8405 2024-02-28 17:27:34.087490 teams_ai-1.2.0/tests/ai/prompts/test_prompt_section_base.py
+-rw-r--r--   0        0        0     1056 2024-02-28 17:27:34.087490 teams_ai-1.2.0/tests/ai/prompts/test_system_message.py
+-rw-r--r--   0        0        0     9290 2024-03-04 19:10:38.503635 teams_ai-1.2.0/tests/ai/prompts/test_template_section.py
+-rw-r--r--   0        0        0     2319 2024-02-28 17:27:34.088994 teams_ai-1.2.0/tests/ai/prompts/test_text_section.py
+-rw-r--r--   0        0        0     7349 2024-03-04 19:10:38.509640 teams_ai-1.2.0/tests/ai/prompts/test_user_input_message.py
+-rw-r--r--   0        0        0     1048 2024-02-28 17:27:34.089504 teams_ai-1.2.0/tests/ai/prompts/test_user_message.py
+-rw-r--r--   0        0        0      853 2024-02-28 17:27:34.089504 teams_ai-1.2.0/tests/ai/tokenizers/test_gpt_tokenizer.py
+-rw-r--r--   0        0        0     6169 2024-02-28 17:27:34.090510 teams_ai-1.2.0/tests/ai/validators/test_action_response_validator.py
+-rw-r--r--   0        0        0      822 2024-02-28 17:27:34.090510 teams_ai-1.2.0/tests/ai/validators/test_default_response_validator.py
+-rw-r--r--   0        0        0     5196 2024-02-28 17:27:34.091510 teams_ai-1.2.0/tests/ai/validators/test_json_response_validator.py
+-rw-r--r--   0        0        0     2643 2024-05-09 16:06:14.538656 teams_ai-1.2.0/tests/auth/test_auth_manager.py
+-rw-r--r--   0        0        0     4144 2024-03-26 18:27:31.075685 teams_ai-1.2.0/tests/state/test_conversation_state.py
+-rw-r--r--   0        0        0     6282 2024-05-09 16:06:14.552991 teams_ai-1.2.0/tests/state/test_custom_turn_state.py
+-rw-r--r--   0        0        0      818 2024-05-09 16:06:14.565573 teams_ai-1.2.0/tests/state/test_state.py
+-rw-r--r--   0        0        0     1797 2024-04-10 20:07:23.487380 teams_ai-1.2.0/tests/state/test_temp_state.py
+-rw-r--r--   0        0        0     6677 2024-05-09 16:06:14.583128 teams_ai-1.2.0/tests/state/test_turn_state.py
+-rw-r--r--   0        0        0     3692 2024-03-26 18:27:31.099741 teams_ai-1.2.0/tests/state/test_user_state.py
+-rw-r--r--   0        0        0     2250 2024-04-01 15:45:22.019885 teams_ai-1.2.0/tests/task_modules/test_task_modules.py
+-rw-r--r--   0        0        0    30053 2024-04-25 20:02:47.968168 teams_ai-1.2.0/tests/test_app.py
+-rw-r--r--   0        0        0    11702 2024-02-28 17:27:34.096123 teams_ai-1.2.0/tests/test_meetings.py
+-rw-r--r--   0        0        0    32052 2024-02-28 17:27:34.106581 teams_ai-1.2.0/tests/test_message_extensions.py
+-rw-r--r--   0        0        0    14794 2024-05-06 18:56:24.275371 teams_ai-1.2.0/tests/test_teams_attachment_downloader.py
+-rw-r--r--   0        0        0      204 2024-05-17 17:55:44.322882 teams_ai-1.2.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0      526 2024-02-28 17:27:34.107578 teams_ai-1.2.0/tests/utils/activity.py
+-rw-r--r--   0        0        0     1055 2024-02-28 17:27:34.107578 teams_ai-1.2.0/tests/utils/adapter.py
+-rw-r--r--   0        0        0        0 2024-05-17 17:55:44.323748 teams_ai-1.2.0/tests/utils/citations/__init__.py
+-rw-r--r--   0        0        0      570 2024-05-17 17:55:44.329833 teams_ai-1.2.0/tests/utils/citations/test_format_citations_response.py
+-rw-r--r--   0        0        0     1937 2024-05-17 17:55:44.337217 teams_ai-1.2.0/tests/utils/citations/test_get_used_citations.py
+-rw-r--r--   0        0        0      513 2024-05-17 17:55:44.345212 teams_ai-1.2.0/tests/utils/test_snippet.py
+-rw-r--r--   0        0        0     1449 2024-05-17 17:55:44.352254 teams_ai-1.2.0/tests/utils/test_to_string.py
+-rw-r--r--   0        0        0     2774 1970-01-01 00:00:00.000000 teams_ai-1.2.0/PKG-INFO
```

### Comparing `teams_ai-1.1.0/LICENSE` & `teams_ai-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/pyproject.toml` & `teams_ai-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "teams-ai"
-version = "1.1.0"
+version = "1.2.0"
 description = "SDK focused on building AI based applications for Microsoft Teams."
 authors = ["Microsoft <teams@microsoft.com>"]
 readme = "README.md"
 repository = "https://github.com/microsoft/teams-ai"
 documentation = "https://learn.microsoft.com/en-us/microsoftteams/platform/bots/how-to/teams%20conversational%20ai/teams-conversation-ai-overview"
 keywords = ["microsoft", "teams", "ai", "bot"]
 packages = [
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 botbuilder-core = "^4.15.0"
 botbuilder-integration-aiohttp = "^4.15.0"
 botframework-connector = "^4.15.0"
 python = ">=3.8,<4.0"
 tiktoken = "^0.4.0"
-aiohttp = "^3.8.5"
+aiohttp = "^3.9.3"
 jsonschema = "^4.21.1"
 types-pyyaml = "^6.0.12.12"
 pyyaml = "^6.0.1"
 dataclasses-json = "^0.6.4"
 azure-ai-contentsafety = "^1.0.0"
 msal = "^1.28.0"
 botbuilder-dialogs = "^4.14.8"
```

### Comparing `teams_ai-1.1.0/README.md` & `teams_ai-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/__init__.py` & `teams_ai-1.2.0/teams/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/activity_type.py` & `teams_ai-1.2.0/teams/activity_type.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/adaptive_cards/adaptive_cards.py` & `teams_ai-1.2.0/teams/adaptive_cards/adaptive_cards.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/actions/action_entry.py` & `teams_ai-1.2.0/teams/ai/actions/action_entry.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/actions/action_turn_context.py` & `teams_ai-1.2.0/teams/ai/actions/action_turn_context.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/ai.py` & `teams_ai-1.2.0/teams/ai/ai.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 from __future__ import annotations
 
 from datetime import datetime
 from logging import Logger
 from typing import Callable, Dict, Generic, Optional, TypeVar
 
 from botbuilder.core import TurnContext
+from botbuilder.schema import Activity, ActivityTypes
 from botframework.connector import Channels
 
 from ..app_error import ApplicationError
 from ..state import TurnState
+from ..utils import snippet
+from ..utils.citations import format_citations_response, get_used_citations
 from .actions import ActionEntry, ActionHandler, ActionTurnContext, ActionTypes
 from .ai_options import AIOptions
+from .citations.citations import Appearance, ClientCitation
 from .moderators.moderator import Moderator
 from .planners.plan import Plan, PredictedDoCommand, PredictedSayCommand
 from .planners.planner import Planner
 
 StateT = TypeVar("StateT", bound=TurnState)
 
 
@@ -107,15 +111,15 @@
             if not action_name:
                 action_name = func.__name__
 
             existing = self._actions.get(action_name)
 
             if existing and not existing.allow_overrides:
                 raise ApplicationError(f"""
-                    The AI.action() method was called with a previously 
+                    The AI.action() method was called with a previously
                     registered action named \"{action_name}\".
                     """)
 
             self._actions[action_name] = ActionEntry[StateT](action_name, allow_overrides, func)
             return func
 
         return __call__
@@ -251,23 +255,85 @@
         return await action.invoke(context, state, context.data.parameters, context.name)
 
     async def _on_say_command(
         self,
         context: ActionTurnContext[PredictedSayCommand],
         _state: StateT,
     ) -> str:
-        response = context.data.response
+        content = (
+            context.data.response.content
+            if context.data.response and context.data.response.content
+            else ""
+        )
+        msg_context = (
+            context.data.response.context
+            if context.data.response and context.data.response.context
+            else None
+        )
+        is_teams_channel = context.activity.channel_id == Channels.ms_teams
 
-        if not response:
+        if not content:
             return ""
 
-        if context.activity.channel_id == Channels.ms_teams:
-            await context.send_activity(response.replace("\n", "<br>"))
-        else:
-            await context.send_activity(response)
+        if is_teams_channel:
+            content = content.replace("\n", "<br>")
+
+        # If the response from AI includes citations,
+        # those citations will be parsed and added to the SAY command.
+        citations = []
+
+        if (
+            msg_context
+            and isinstance(msg_context, dict)
+            and "citations" in msg_context
+            and len(msg_context["citations"]) > 0
+        ):
+            for i, citation in enumerate(msg_context["citations"]):
+                citations.append(
+                    ClientCitation(
+                        position=f"[{i + 1}]",
+                        appearance=Appearance(
+                            name=citation["title"],
+                            abstract=snippet(citation["abstract"], 500),
+                        ),
+                    )
+                )
+
+        # If there are citations, modify the content so that the sources are numbers
+        # instead of [doc1], [doc2], etc.
+        content_text = content if not citations else format_citations_response(content)
+
+        # If there are citations, filter out the citations unused in content.
+        referenced_citations = get_used_citations(content_text, citations)
+        channel_data = {}
+
+        if is_teams_channel:
+            channel_data["feedbackLoopEnabled"] = self._options.enable_feedback_loop
+
+        await context.send_activity(
+            Activity(
+                type=ActivityTypes.message,
+                text=content_text,
+                channel_data=channel_data,
+                entities=[
+                    {
+                        "type": "https://schema.org/Message",
+                        "@type": "Message",
+                        "@context": "https://schema.org",
+                        "@id": "",
+                        "additionalType": ["AIGeneratedContent"],
+                        **(
+                            {"citation": [citation.__dict__ for citation in referenced_citations]}
+                            if referenced_citations
+                            else {}
+                        ),
+                    }
+                ],
+            )
+        )
 
         return ""
 
     async def _on_too_many_steps(
         self,
         _context: ActionTurnContext,
         _state: StateT,
```

### Comparing `teams_ai-1.1.0/teams/ai/ai_options.py` & `teams_ai-1.2.0/teams/ai/ai_options.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,16 +21,22 @@
     planner: Planner[StateT]
     """
     The planner to use for generating plans.
     """
 
     moderator: Moderator = field(default_factory=DefaultModerator)
     """
-    Optional. The moderator to use for moderating input passed to 
+    Optional. The moderator to use for moderating input passed to
     the model and the output return by the model.
     """
 
     allow_looping: bool = True
     """
     Optional. If true, the AI system will allow the planner to loop.
     Default `True`
     """
+
+    enable_feedback_loop: bool = False
+    """
+    Optional. If true, the AI system will enable the feedback loop in Teams that
+    allows a user to give thumbs up or down to a response.
+    """
```

### Comparing `teams_ai-1.1.0/teams/ai/augmentations/augmentation.py` & `teams_ai-1.2.0/teams/ai/augmentations/augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/augmentations/default_augmentation.py` & `teams_ai-1.2.0/teams/ai/augmentations/default_augmentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 Copyright (c) Microsoft Corporation. All rights reserved.
 Licensed under the MIT License.
 """
 
 from __future__ import annotations
 
-from typing import Union
+from typing import TypeVar, Union
 
 from botbuilder.core import TurnContext
 
 from ...state import MemoryBase
 from ..models.prompt_response import PromptResponse
 from ..planners.plan import Plan, PredictedSayCommand
 from ..prompts.sections.prompt_section import PromptSection
 from ..tokenizers.tokenizer import Tokenizer
 from ..validators.validation import Validation
 from .augmentation import Augmentation
 
+ContentT = TypeVar("ContentT")
+
 
 class DefaultAugmentation(Augmentation[str]):
     """
     The default 'none' augmentation.
 
     This augmentation does not add any additional functionality to the prompt. It always
     returns a `Plan` with a single `SAY` command containing the models response.
@@ -59,17 +61,15 @@
         self, turn_context: TurnContext, memory: MemoryBase, response: PromptResponse[str]
     ) -> Plan:
         """
         Creates a plan given validated response value.
 
         Args:
             turn_context (TurnContext): Context for the current turn of conversation.
-            memory (MemoryBase):  Interface for accessing state variables.
+            memory (MemoryBase): Interface for accessing state variables.
             response (PromptResponse[str]): The validated and transformed response for the prompt.
 
         Returns:
             Plan: The created plan.
         """
-        say_response = ""
-        if response.message and response.message.content:
-            say_response = response.message.content
+        say_response = response.message
         return Plan(commands=[PredictedSayCommand(response=say_response)])
```

### Comparing `teams_ai-1.1.0/teams/ai/augmentations/monologue_augmentation.py` & `teams_ai-1.2.0/teams/ai/augmentations/monologue_augmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,16 +119,16 @@
     The monologue helps the LLM to perform chain-of-thought reasoning
     across multiple turns of conversation.
     """
 
     _section: ActionAugmentationSection
     _monologue_validator = JSONResponseValidator(
         InnerMonologueSchema,
-        """No valid JSON objects were found in the response. Return a 
-        valid JSON object with your thoughts and the next 
+        """No valid JSON objects were found in the response. Return a
+        valid JSON object with your thoughts and the next
         action to perform.""",
     )
     _action_validator: ActionResponseValidator
 
     def __init__(self, actions: List[ChatCompletionAction]) -> None:
         """
         Creates a new 'MonologueAugmentation' instance.
@@ -254,16 +254,26 @@
         if response.message and response.message.content:
             command: PredictedCommand
             # Double encoding/decoding required for class
             monologue = InnerMonologue.from_dict(InnerMonologue.to_dict(response.message.content))
 
             if monologue.action.name == "SAY":
                 params = monologue.action.parameters
-                response_val = cast(str, params.get("text")) if params else ""
-                command = PredictedSayCommand(response=response_val)
+                response_val = PredictedSayCommand(
+                    response=(
+                        Message(
+                            role="assistant",
+                            context=response.message.context,
+                            content=params.get("text"),
+                        )
+                        if params
+                        else None
+                    )
+                )
+                command = response_val
             else:
                 command = PredictedDoCommand(
                     action=monologue.action.name,
                     parameters=monologue.action.parameters if monologue.action.parameters else {},
                 )
             return Plan(commands=[command])
         return Plan()
```

### Comparing `teams_ai-1.1.0/teams/ai/augmentations/sequence_augmentation.py` & `teams_ai-1.2.0/teams/ai/augmentations/sequence_augmentation.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 from typing import Any, Dict, List, Optional, Union, cast
 
 from botbuilder.core import TurnContext
 
 from ...state import MemoryBase
 from ..models.chat_completion_action import ChatCompletionAction
 from ..models.prompt_response import PromptResponse
-from ..planners.plan import Plan, PredictedDoCommand, PredictedSayCommand
+from ..planners.plan import (
+    Plan,
+    PredictedCommand,
+    PredictedDoCommand,
+    PredictedSayCommand,
+)
 from ..prompts.function_call import FunctionCall
 from ..prompts.message import Message
 from ..prompts.sections.action_augmentation_section import ActionAugmentationSection
 from ..prompts.sections.prompt_section import PromptSection
 from ..tokenizers import Tokenizer
 from ..validators.action_response_validator import ActionResponseValidator
 from ..validators.json_response_validator import JSONResponseValidator
@@ -32,15 +37,21 @@
             "type": "array",
             "items": {
                 "type": "object",
                 "properties": {
                     "type": {"type": "string", "enum": ["DO", "SAY"]},
                     "action": {"type": "string"},
                     "parameters": {"type": "object"},
-                    "response": {"type": "string"},
+                    "response": {
+                        "type": "object",
+                        "properties": {
+                            "role": {"type": "string", "enum": ["assistant"]},
+                            "content": {"type": "string"},
+                        },
+                    },
                 },
                 "required": ["type"],
             },
             "minItems": 1,
         },
     },
     "required": ["type", "commands"],
@@ -150,14 +161,17 @@
                     # Ensure that the model specified a response
                     if not command.response:
                         return Validation(
                             valid=False,
                             feedback='The plan JSON is missing the SAY "response" '
                             + f"for command[{index}]. Return the response to SAY.",
                         )
+
+                    if isinstance(command.response, dict):
+                        command.response = Message[str].from_dict(command.response)
                 else:
                     return Validation(
                         valid=False,
                         feedback="The plan JSON contains an unknown command"
                         + f"type of ${command.type}. Only use DO or SAY commands.",
                     )
 
@@ -174,10 +188,33 @@
             turn_context (TurnContext): Context for the current turn of conversation.
             memory (MemoryBase): Interface for accessing state variables.
             response (PromptResponse): Validated, transformed response for the prompt.
 
         Returns:
             Plan: The created plan
         """
+
         if response.message and response.message.content:
-            return response.message.content
+            plan = response.message.content
+            commands: List[PredictedCommand] = []
+
+            for command in plan.commands:
+                if command.type == "SAY":
+                    commands.append(
+                        PredictedSayCommand(
+                            response=Message[str](
+                                role="assistant",
+                                context=response.message.context,
+                                content=(
+                                    command.response.content
+                                    if command.response and command.response.content
+                                    else None
+                                ),
+                            )
+                        )
+                    )
+                else:
+                    commands.append(command)
+
+            plan.commands = commands
+            return plan
         return Plan()
```

### Comparing `teams_ai-1.1.0/teams/ai/clients/llm_client.py` & `teams_ai-1.2.0/teams/ai/clients/llm_client.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/data_sources/data_source.py` & `teams_ai-1.2.0/teams/ai/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/data_sources/text_data_source.py` & `teams_ai-1.2.0/teams/ai/data_sources/text_data_source.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/embeddings/__init__.py` & `teams_ai-1.2.0/teams/ai/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/embeddings/azure_openai_embeddings.py` & `teams_ai-1.2.0/teams/ai/embeddings/azure_openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/embeddings/azure_openai_embeddings_options.py` & `teams_ai-1.2.0/teams/ai/embeddings/azure_openai_embeddings_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/embeddings/embeddings_model.py` & `teams_ai-1.2.0/teams/ai/embeddings/embeddings_model.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/embeddings/embeddings_response.py` & `teams_ai-1.2.0/teams/ai/embeddings/embeddings_response.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/embeddings/openai_embeddings.py` & `teams_ai-1.2.0/teams/ai/embeddings/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/embeddings/openai_embeddings_options.py` & `teams_ai-1.2.0/teams/ai/embeddings/openai_embeddings_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/models/__init__.py` & `teams_ai-1.2.0/teams/ai/models/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/models/chat_completion_action.py` & `teams_ai-1.2.0/teams/ai/models/chat_completion_action.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/models/openai_model.py` & `teams_ai-1.2.0/teams/ai/models/openai_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             max_tokens=max_tokens,
         )
 
         if res.too_long:
             return PromptResponse[str](
                 status="too_long",
                 error=f"""
-                the generated chat completion prompt had a length of {res.length} tokens 
+                the generated chat completion prompt had a length of {res.length} tokens
                 which exceeded the max_input_tokens of {max_tokens}
                 """,
             )
 
         if self._options.logger is not None:
             self._options.logger.debug(f"PROMPT:\n{res.output}")
 
@@ -208,11 +208,11 @@
         except openai.APIError as err:
             if self._options.logger is not None:
                 self._options.logger.error("ERROR:\n%s", json.dumps(err.body))
 
             return PromptResponse[str](
                 status="error",
                 error=f"""
-                The chat completion API returned an error 
+                The chat completion API returned an error
                 status of {err.code}: {err.message}
                 """,
             )
```

### Comparing `teams_ai-1.1.0/teams/ai/models/prompt_completion_model.py` & `teams_ai-1.2.0/teams/ai/models/prompt_completion_model.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/models/prompt_response.py` & `teams_ai-1.2.0/teams/ai/models/prompt_response.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/moderators/__init__.py` & `teams_ai-1.2.0/teams/ai/moderators/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/moderators/azure_content_safety_moderator.py` & `teams_ai-1.2.0/teams/ai/moderators/azure_content_safety_moderator.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             models.TextCategory.VIOLENCE,
         ]
     )
     "Optional. Azure Content Safety Categories. Default: all"
 
     blocklist_names: Optional[List[str]] = None
     """
-    Text blocklist Name. Only support following characters: 0-9 A-Z a-z - . _ ~. 
+    Text blocklist Name. Only support following characters: 0-9 A-Z a-z - . _ ~.
     You could attach multiple lists name here.
     """
 
 
 class AzureContentSafetyModerator(Generic[StateT], Moderator[StateT]):
     """
     An Azure OpenAI moderator that uses OpenAI's moderation API
@@ -145,15 +145,19 @@
             return plan
 
         for cmd in plan.commands:
             if isinstance(cmd, PredictedSayCommand):
                 try:
                     res = self._client.analyze_text(
                         options=models.AnalyzeTextOptions(
-                            text=cmd.response,
+                            text=(
+                                cmd.response.content
+                                if cmd.response and cmd.response.content is not None
+                                else ""
+                            ),
                             categories=self._options.categories,
                             blocklist_names=self._options.blocklist_names,
                         )
                     )
 
                     flagged: bool = False
                     categories: Dict[str, bool] = {}
```

### Comparing `teams_ai-1.1.0/teams/ai/moderators/default_moderator.py` & `teams_ai-1.2.0/teams/ai/moderators/default_moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/moderators/moderator.py` & `teams_ai-1.2.0/teams/ai/moderators/moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/moderators/openai_moderator.py` & `teams_ai-1.2.0/teams/ai/moderators/openai_moderator.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,16 @@
         if self._options.moderate == "input":
             return plan
 
         for cmd in plan.commands:
             if isinstance(cmd, PredictedSayCommand):
                 try:
                     res = await self._client.moderations.create(
-                        input=cmd.response, model=self._options.model
+                        input=cmd.response.content if cmd.response and cmd.response.content else "",
+                        model=self._options.model,
                     )
 
                     for result in res.results:
                         if result.flagged:
                             return Plan(
                                 commands=[
                                     PredictedDoCommand(
```

### Comparing `teams_ai-1.1.0/teams/ai/planners/__init__.py` & `teams_ai-1.2.0/teams/ai/planners/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/planners/action_planner.py` & `teams_ai-1.2.0/teams/ai/planners/action_planner.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/planners/assistants_planner.py` & `teams_ai-1.2.0/teams/ai/planners/assistants_planner.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from openai.types.beta.threads.run import RequiredAction
 from openai.types.beta.threads.run_submit_tool_outputs_params import ToolOutput
 
 from ...app_error import ApplicationError
 from ...state import TurnState
 from ...user_agent import _UserAgent
 from ..actions.action_types import ActionTypes
+from ..prompts.message import Citation, Message, MessageContext
 from .plan import Plan, PredictedDoCommand, PredictedSayCommand
 from .planner import Planner
 
 DEFAULT_POLLING_INTERVAL = 1
 DEFAULT_ASSISTANTS_STATE_VARIABLE = "conversation.assistants_state"
 SUBMIT_TOOL_OUTPUTS_VARIABLE = "temp.submit_tool_outputs"
 SUBMIT_TOOL_OUTPUTS_MAP = "temp.submit_tool_map"
@@ -353,15 +354,39 @@
         new_messages.reverse()
 
         # Convert the messages to SAY commands
         plan = Plan()
         for message in new_messages:
             for content in message.content:
                 if content.type == "text":
-                    plan.commands.append(PredictedSayCommand(response=content.text.value))
+                    annotations = content.text.annotations if content.text.annotations else None
+                    plan.commands.append(
+                        PredictedSayCommand(
+                            response=Message(
+                                role="assistant",
+                                content=content.text.value,
+                                context=MessageContext(
+                                    intent="",
+                                    citations=(
+                                        [
+                                            Citation(
+                                                title="",
+                                                url="",
+                                                filepath="",
+                                                content=annotation.text,
+                                            )
+                                            for annotation in annotations
+                                        ]
+                                        if annotations
+                                        else []
+                                    ),
+                                ),
+                            )
+                        )
+                    )
 
         return plan
 
     async def _block_on_in_progress_runs(self, thread_id: str) -> None:
         # We loop until we're told the last run is completed
         while True:
             runs = await self._client.beta.threads.runs.list(thread_id, limit=1)
```

### Comparing `teams_ai-1.1.0/teams/ai/planners/plan.py` & `teams_ai-1.2.0/teams/ai/planners/plan.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 Copyright (c) Microsoft Corporation. All rights reserved.
 Licensed under the MIT License.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Literal, Union
+from typing import Any, Dict, List, Literal, Optional, Union
 
 from dataclasses_json import DataClassJsonMixin, dataclass_json
 
+from ..prompts.message import Message
+
 
 @dataclass_json
 @dataclass
 class PredictedDoCommand(DataClassJsonMixin):
     """
     A predicted DO command is an action that the AI system should perform.
     """
@@ -34,16 +36,16 @@
     """
     A predicted SAY command is a response that the AI system should say.
     """
 
     type: Literal["SAY"] = "SAY"
     "Type to indicate that a SAY command is being returned."
 
-    response: str = ""
-    "The response that the AI system should say."
+    response: Optional[Message[str]] = None
+    "The prompt response containing what the AI system should say."
 
 
 PredictedCommand = Union[PredictedDoCommand, PredictedSayCommand]
 "A predicted command is a command that the AI system should execute."
 
 
 @dataclass
```

### Comparing `teams_ai-1.1.0/teams/ai/planners/planner.py` & `teams_ai-1.2.0/teams/ai/planners/planner.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/__init__.py` & `teams_ai-1.2.0/teams/ai/prompts/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 
 from .assistant_message import AssistantMessage
 from .augmentation_config import AugmentationConfig
 from .completion_config import CompletionConfig
 from .function_call import FunctionCall
 from .function_call_message import FunctionCallMessage
 from .function_response_message import FunctionResponseMessage
-from .message import ImageContentPart, ImageUrl, Message, TextContentPart
+from .message import (
+    Citation,
+    ImageContentPart,
+    ImageUrl,
+    Message,
+    MessageContext,
+    TextContentPart,
+)
 from .prompt import Prompt
 from .prompt_functions import PromptFunction, PromptFunctions
 from .prompt_manager import PromptManager
 from .prompt_manager_options import PromptManagerOptions
 from .prompt_template import PromptTemplate
 from .prompt_template_config import PromptTemplateConfig
 from .rendered_prompt_section import RenderedPromptSection
@@ -22,20 +29,22 @@
 from .user_input_message import UserInputMessage
 from .user_message import UserMessage
 
 __all__ = [
     "AssistantMessage",
     "AugmentationConfig",
     "CompletionConfig",
+    "Citation",
     "FunctionCall",
     "FunctionCallMessage",
     "FunctionResponseMessage",
     "ImageContentPart",
     "ImageUrl",
     "Message",
+    "MessageContext",
     "TextContentPart",
     "Prompt",
     "PromptFunction",
     "PromptFunctions",
     "PromptManager",
     "PromptManagerOptions",
     "PromptTemplate",
```

### Comparing `teams_ai-1.1.0/teams/ai/prompts/assistant_message.py` & `teams_ai-1.2.0/teams/ai/prompts/assistant_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/augmentation_config.py` & `teams_ai-1.2.0/teams/ai/prompts/augmentation_config.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/completion_config.py` & `teams_ai-1.2.0/teams/ai/prompts/completion_config.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/function_call_message.py` & `teams_ai-1.2.0/teams/ai/prompts/function_call_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/function_response_message.py` & `teams_ai-1.2.0/teams/ai/prompts/function_response_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from __future__ import annotations
 
 from typing import Any, List
 
 from botbuilder.core import TurnContext
 
 from ...state import MemoryBase
+from ...utils.to_string import to_string
 from ..tokenizers import Tokenizer
-from ..utilities import to_string
 from .message import Message
 from .prompt_functions import PromptFunctions
 from .rendered_prompt_section import RenderedPromptSection
 from .sections.prompt_section_base import PromptSectionBase
 
 
 class FunctionResponseMessage(PromptSectionBase):
```

### Comparing `teams_ai-1.1.0/teams/ai/prompts/message.py` & `teams_ai-1.2.0/teams/ai/prompts/message.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,33 +4,37 @@
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Generic, Literal, Optional, TypeVar, Union
 
+from dataclasses_json import DataClassJsonMixin, dataclass_json
+
 from .function_call import FunctionCall
 
 T = TypeVar("T")
 
 
+@dataclass_json
 @dataclass
-class Message(Generic[T]):
+class Message(Generic[T], DataClassJsonMixin):
     """
     A message object sent to or received from an LLM.
 
     Attributes:
         role (str): The messages role. Typically 'system', 'user', 'assistant', 'function'.
         content (Optional[T]): Text of the message.
         function_call (Optional[FunctionCall]): A named function to call.
         name (Optional[str]): Name of the function that was called.
     """
 
     role: str
     content: Optional[T] = None
+    context: Optional[MessageContext] = None
     function_call: Optional[FunctionCall] = None
     name: Optional[str] = None
 
 
 @dataclass
 class ImageUrl:
     """
@@ -69,7 +73,39 @@
     image_url: Union[str, ImageUrl]
 
 
 MessageContentParts = Union[TextContentPart, ImageContentPart]
 """
 Represents part of the message's content
 """
+
+
+@dataclass
+class Citation:
+    """
+    Represents a citation returned by the model
+
+    Attributes:
+        content (str): The content of the citation
+        title (str): The title of the citation
+        url (str): The url of the citation
+        filepath (str): The filepath of the citation
+    """
+
+    content: str
+    title: str
+    url: str
+    filepath: str
+
+
+@dataclass
+class MessageContext:
+    """
+    Represents the message context containing a citation
+
+    Attributes:
+        citations (list[Citation]): The citations in the message
+        intent (str): The intent of the message
+    """
+
+    citations: list[Citation]
+    intent: str
```

### Comparing `teams_ai-1.1.0/teams/ai/prompts/prompt.py` & `teams_ai-1.2.0/teams/ai/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/prompt_functions.py` & `teams_ai-1.2.0/teams/ai/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/prompt_manager.py` & `teams_ai-1.2.0/teams/ai/prompts/prompt_manager.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/prompt_manager_options.py` & `teams_ai-1.2.0/teams/ai/prompts/prompt_manager_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/prompt_template.py` & `teams_ai-1.2.0/teams/ai/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/prompt_template_config.py` & `teams_ai-1.2.0/teams/ai/prompts/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/rendered_prompt_section.py` & `teams_ai-1.2.0/teams/ai/prompts/rendered_prompt_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/sections/__init__.py` & `teams_ai-1.2.0/teams/ai/prompts/sections/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/sections/action_augmentation_section.py` & `teams_ai-1.2.0/teams/ai/prompts/sections/action_augmentation_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/sections/conversation_history_section.py` & `teams_ai-1.2.0/teams/ai/prompts/sections/conversation_history_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 from copy import deepcopy
 from typing import List
 
 from botbuilder.core import TurnContext
 
 from ....state import MemoryBase
+from ....utils.to_string import to_string
 from ...tokenizers import Tokenizer
-from ...utilities import to_string
 from ..message import Message
 from ..prompt_functions import PromptFunctions
 from ..rendered_prompt_section import RenderedPromptSection
 from .prompt_section_base import PromptSectionBase
 
 
 class ConversationHistorySection(PromptSectionBase):
```

### Comparing `teams_ai-1.1.0/teams/ai/prompts/sections/data_source_section.py` & `teams_ai-1.2.0/teams/ai/prompts/sections/data_source_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/sections/group_section.py` & `teams_ai-1.2.0/teams/ai/prompts/sections/group_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/sections/layout_engine_section.py` & `teams_ai-1.2.0/teams/ai/prompts/sections/layout_engine_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/sections/prompt_section.py` & `teams_ai-1.2.0/teams/ai/prompts/sections/prompt_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/sections/prompt_section_base.py` & `teams_ai-1.2.0/teams/ai/prompts/sections/prompt_section_base.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/sections/template_section.py` & `teams_ai-1.2.0/teams/ai/prompts/sections/template_section.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from enum import Enum
 from typing import Awaitable, Callable, List
 
 from botbuilder.core import TurnContext
 
 from ....app_error import ApplicationError
 from ....state import MemoryBase
+from ....utils.to_string import to_string
 from ...tokenizers import Tokenizer
-from ...utilities import to_string
 from ..message import Message
 from ..prompt_functions import PromptFunctions
 from ..rendered_prompt_section import RenderedPromptSection
 from .prompt_section_base import PromptSectionBase
 
 
 # private
```

### Comparing `teams_ai-1.1.0/teams/ai/prompts/sections/text_section.py` & `teams_ai-1.2.0/teams/ai/prompts/sections/text_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/system_message.py` & `teams_ai-1.2.0/teams/ai/prompts/system_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/user_input_message.py` & `teams_ai-1.2.0/teams/ai/prompts/user_input_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/prompts/user_message.py` & `teams_ai-1.2.0/teams/ai/prompts/user_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/tokenizers/gpt_tokenizer.py` & `teams_ai-1.2.0/teams/ai/tokenizers/gpt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/tokenizers/tokenizer.py` & `teams_ai-1.2.0/teams/ai/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/utilities.py` & `teams_ai-1.2.0/teams/utils/to_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from __future__ import annotations
 
 import json
 from typing import Any
 
 import yaml
 
-from .tokenizers import Tokenizer
+from ..ai.tokenizers import Tokenizer
 
 
 def to_string(tokenizer: Tokenizer, value: Any, as_json: bool = False) -> str:
     """
     Converts a value to a string representation.
     Dates are converted to ISO strings and Objects are converted to JSON or YAML,
     whichever is shorter.
```

### Comparing `teams_ai-1.1.0/teams/ai/validators/__init__.py` & `teams_ai-1.2.0/teams/ai/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/validators/action_response_validator.py` & `teams_ai-1.2.0/teams/ai/validators/action_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/validators/default_response_validator.py` & `teams_ai-1.2.0/teams/ai/validators/default_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/validators/json_response_validator.py` & `teams_ai-1.2.0/teams/ai/validators/json_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/validators/prompt_response_validator.py` & `teams_ai-1.2.0/teams/ai/validators/prompt_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/ai/validators/validation.py` & `teams_ai-1.2.0/teams/ai/validators/validation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/app.py` & `teams_ai-1.2.0/teams/app.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/app_options.py` & `teams_ai-1.2.0/teams/app_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/auth/auth.py` & `teams_ai-1.2.0/teams/auth/auth.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/auth/auth_component.py` & `teams_ai-1.2.0/teams/auth/auth_component.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/auth/auth_manager.py` & `teams_ai-1.2.0/teams/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/auth/auth_options.py` & `teams_ai-1.2.0/teams/auth/auth_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/auth/oauth/oauth.py` & `teams_ai-1.2.0/teams/auth/oauth/oauth.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/auth/oauth/oauth_adaptive_card.py` & `teams_ai-1.2.0/teams/auth/oauth/oauth_adaptive_card.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/auth/oauth/oauth_dialog.py` & `teams_ai-1.2.0/teams/auth/oauth/oauth_dialog.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/auth/oauth/oauth_message_extension.py` & `teams_ai-1.2.0/teams/auth/oauth/oauth_message_extension.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/auth/oauth/oauth_options.py` & `teams_ai-1.2.0/teams/auth/oauth/oauth_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/dialogs/dialog.py` & `teams_ai-1.2.0/teams/dialogs/dialog.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/input_file.py` & `teams_ai-1.2.0/teams/input_file.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/meetings/meetings.py` & `teams_ai-1.2.0/teams/meetings/meetings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/message_extensions/message_extensions.py` & `teams_ai-1.2.0/teams/message_extensions/message_extensions.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/route.py` & `teams_ai-1.2.0/teams/route.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/state/__init__.py` & `teams_ai-1.2.0/teams/state/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/state/conversation_state.py` & `teams_ai-1.2.0/teams/state/conversation_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/state/memory.py` & `teams_ai-1.2.0/teams/state/memory.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/state/state.py` & `teams_ai-1.2.0/teams/state/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,43 +68,46 @@
     __deleted__: List[str]
     """
     Deleted Keys
     """
 
     def __init__(self, *args, **kwargs) -> None:  # pylint: disable=unused-argument
         super().__init__()
-        self.__key__ = kwargs["__key__"] if "__key__" in kwargs else ""
+        self.__key__ = ""
         self.__deleted__ = []
 
         # copy public attributes that are not functions
         for name in dir(self):
             value = object.__getattribute__(self, name)
 
             if not name.startswith("_") and not callable(value):
                 self[name] = deepcopy(value)
 
         for key, value in kwargs.items():
-            if not key in ("__key__", "__deleted__"):
-                self[key] = value
+            self[key] = value
 
     async def save(self, _context: TurnContext, storage: Optional[Storage] = None) -> None:
         """
         Saves The State to Storage
 
         Args:
             context (TurnContext): the turn context.
             storage (Optional[Storage]): storage to save to.
         """
+
         if not storage or self.__key__ == "":
             return
 
+        data = self.copy()
+        del data["__key__"]
+
         await storage.delete(self.__deleted__)
         await storage.write(
             {
-                self.__key__: self.copy(),
+                self.__key__: data,
             }
         )
 
         self.__deleted__ = []
 
     @classmethod
     @abstractmethod
```

### Comparing `teams_ai-1.1.0/teams/state/temp_state.py` & `teams_ai-1.2.0/teams/state/temp_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/state/todict.py` & `teams_ai-1.2.0/teams/state/todict.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     Converts a value to a
     dictionary recursively
     """
 
     if isinstance(value, dict):
         data = {}
         for key, val in value.items():
+            if isinstance(key, str) and key.startswith("__"):
+                continue
+
             data[key] = todict(val)
         return data
 
     if isinstance(value, list):
         return [todict(v) for v in value]
 
     if isinstance(value, object) and hasattr(value, "__dict__"):
```

### Comparing `teams_ai-1.1.0/teams/state/turn_state.py` & `teams_ai-1.2.0/teams/state/turn_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/state/user_state.py` & `teams_ai-1.2.0/teams/state/user_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/task_modules/task_modules.py` & `teams_ai-1.2.0/teams/task_modules/task_modules.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/teams_adapter.py` & `teams_ai-1.2.0/teams/teams_adapter.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/teams_attachment_downloader/teams_attachment_downloader.py` & `teams_ai-1.2.0/teams/teams_attachment_downloader/teams_attachment_downloader.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/typing.py` & `teams_ai-1.2.0/teams/typing.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/utils/json/parse.py` & `teams_ai-1.2.0/teams/utils/json/parse.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/teams/utils/json/parse_object.py` & `teams_ai-1.2.0/teams/utils/json/parse_object.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/adaptive_cards/test_adaptive_cards.py` & `teams_ai-1.2.0/tests/adaptive_cards/test_adaptive_cards.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/augmentations/test_default_augmentation.py` & `teams_ai-1.2.0/tests/ai/augmentations/test_default_augmentation.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         state = TurnState()
 
         # Validate response
         say_response = PromptResponse(
             message=Message(
                 role="assistant",
                 content='{ "type": "plan", '
-                + '"commands": [{ "type": "SAY", "response": "hello world"}]}',
+                + '"commands": [{ "type": "SAY", "response": { "role": "assistant", "content":'
+                ' "hello world"}}]}',
             )
         )
         validation = await self.default_augmentation.validate_response(
             cast(TurnContext, {}),
             memory=state,
             tokenizer=self.tokenizer,
             response=say_response,
@@ -64,14 +65,17 @@
         self.assertEqual(validation.valid, True)
 
         # Create plan from validated response
         plan = await self.default_augmentation.create_plan_from_response(
             cast(TurnContext, {}),
             memory=state,
             response=PromptResponse[str](
-                message=Message(role="assistant", content=validation.value)
+                message=Message(role="assistant", content=validation.value or "")
             ),
         )
         self.assertEqual(len(plan.commands), 1)
         self.assertEqual(plan.commands[0].type, "SAY")
         assert isinstance(plan.commands[0], PredictedSayCommand)
-        self.assertEqual(plan.commands[0].response, "")
+        self.assertEqual(
+            plan.commands[0].response,
+            Message(role="assistant", content="", function_call=None, name=None),
+        )
```

### Comparing `teams_ai-1.1.0/tests/ai/augmentations/test_monologue_augmentation.py` & `teams_ai-1.2.0/tests/ai/augmentations/test_monologue_augmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,17 @@
                     ),
                 )
             ),
         )
         self.assertEqual(len(plan.commands), 1)
         self.assertEqual(plan.commands[0].type, "SAY")
         assert isinstance(plan.commands[0], PredictedSayCommand)
-        self.assertEqual(plan.commands[0].response, "hello world")
+        assert plan.commands[0].response is not None
+        self.assertEqual(plan.commands[0].response.role, "assistant")
+        self.assertEqual(plan.commands[0].response.content, "hello world")
 
     async def test_create_plan_with_do_command(self):
         state = TurnState()
         plan = await self.monologue_augmentation.create_plan_from_response(
             cast(TurnContext, {}),
             state,
             PromptResponse[InnerMonologue](
```

### Comparing `teams_ai-1.1.0/tests/ai/augmentations/test_sequence_augmentation.py` & `teams_ai-1.2.0/tests/ai/augmentations/test_sequence_augmentation.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from unittest import IsolatedAsyncioTestCase
 
 from botbuilder.core import TurnContext
 
 from teams.ai.augmentations.sequence_augmentation import SequenceAugmentation
 from teams.ai.models.chat_completion_action import ChatCompletionAction
 from teams.ai.models.prompt_response import PromptResponse
-from teams.ai.planners import Plan
+from teams.ai.planners.plan import PredictedDoCommand, PredictedSayCommand
 from teams.ai.prompts.message import Message
 from teams.ai.prompts.prompt_functions import PromptFunctions
 from teams.ai.tokenizers.gpt_tokenizer import GPTTokenizer
 from teams.state.turn_state import TurnState
 
 
 class TestSequenceAugmentation(IsolatedAsyncioTestCase):
@@ -117,16 +117,15 @@
         response = await self.sequence_augmentation.validate_response(
             cast(TurnContext, {}),
             state,
             self.tokenizer,
             PromptResponse[str](
                 message=Message[str](
                     role="assistant",
-                    content='{ "type": "plan", '
-                    + '"commands": [{ "type": "SAY", "response": ""}]}',
+                    content='{ "type": "plan", ' + '"commands": [{ "type": "SAY"' + "}]}",
                 )
             ),
             3,
         )
         self.assertEqual(response.valid, False)
         self.assertEqual(
             response.feedback,
@@ -160,50 +159,52 @@
             state,
             self.tokenizer,
             PromptResponse[str](
                 message=Message[str](
                     role="assistant",
                     content='{"type":"plan","commands":[{"type":"DO",'
                     + '"action":"test1","parameters": { "foo": "bar" }}'
-                    + ',{"type":"SAY","response":"hello world"}]}',
+                    + ',{"type":"SAY","response": { "role": "assistant", "content": "hello'
+                    ' world"}}]}',
                 )
             ),
             3,
         )
+        self.assertEqual(response.feedback, None)
         self.assertEqual(response.valid, True)
 
     async def test_create_plan_from_response(self):
         state = TurnState()
         # Validate response
         validation = await self.sequence_augmentation.validate_response(
             cast(TurnContext, {}),
             state,
             self.tokenizer,
             PromptResponse[str](
                 message=Message[str](
                     role="assistant",
                     content='{"type":"plan","commands":[{"type":"DO",'
                     + '"action":"test1","parameters": { "foo": "bar" }},'
-                    + '{"type":"SAY","response":"hello world"}]}',
+                    + '{"type":"SAY","response": { "role": "assistant", "content": "hello'
+                    ' world"}}]}',
                 )
             ),
             3,
         )
-
         # Create plan from response
         plan = await self.sequence_augmentation.create_plan_from_response(
             cast(TurnContext, {}),
             state,
             PromptResponse(message=Message(role="assistant", content=validation.value)),
         )
-        self.assertEqual(
-            plan,
-            Plan.from_dict(
-                {
-                    "type": "plan",
-                    "commands": [
-                        {"type": "DO", "action": "test1", "parameters": {"foo": "bar"}},
-                        {"type": "SAY", "response": "hello world"},
-                    ],
-                }
-            ),
-        )
+        command0 = cast(PredictedDoCommand, plan.commands[0])
+        command1 = cast(PredictedSayCommand, plan.commands[1])
+
+        self.assertEqual(len(plan.commands), 2)
+        self.assertEqual(command0.type, "DO")
+        self.assertEqual(command0.action, "test1")
+        self.assertEqual(command0.parameters, {"foo": "bar"})
+
+        self.assertEqual(command1.type, "SAY")
+        assert command1.response is not None
+        self.assertEqual(command1.response.role, "assistant")
+        self.assertEqual(command1.response.content, "hello world")
```

### Comparing `teams_ai-1.1.0/tests/ai/clients/test_llm_client.py` & `teams_ai-1.2.0/tests/ai/clients/test_llm_client.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/data_sources/test_text_data_source.py` & `teams_ai-1.2.0/tests/ai/data_sources/test_text_data_source.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/embeddings/test_azure_openai_embeddings.py` & `teams_ai-1.2.0/tests/ai/embeddings/test_azure_openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/embeddings/test_openai_embeddings.py` & `teams_ai-1.2.0/tests/ai/embeddings/test_openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/models/test_openai_model.py` & `teams_ai-1.2.0/tests/ai/models/test_openai_model.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/moderators/test_azure_content_safety_moderator.py` & `teams_ai-1.2.0/tests/ai/moderators/test_azure_content_safety_moderator.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from teams import ApplicationError
 from teams.ai.actions import ActionTypes
 from teams.ai.moderators import (
     AzureContentSafetyModerator,
     AzureContentSafetyModeratorOptions,
 )
 from teams.ai.planners import Plan, PredictedDoCommand, PredictedSayCommand
+from teams.ai.prompts.message import Message
 from teams.state import ConversationState, TempState, TurnState, UserState
 
 
 class MockContentSafetyClient:
     def analyze_text(self, *_args, **_kwargs: Any):
         return {}
 
@@ -107,15 +108,17 @@
     @mock.patch(
         "azure.ai.contentsafety.ContentSafetyClient", return_value=MockContentSafetyClient()
     )
     async def test_should_not_review_output(self, mock_async_openai):
         moderator = AzureContentSafetyModerator(
             options=AzureContentSafetyModeratorOptions(api_key="", moderate="input", endpoint="")
         )
-        plan = Plan(commands=[PredictedSayCommand(response="test")])
+        plan = Plan(
+            commands=[PredictedSayCommand(response=Message[str](role="assistant", content="test"))]
+        )
         output = await moderator.review_output(
             context=cast(TurnContext, {}), state=TurnState(), plan=plan
         )
         self.assertTrue(mock_async_openai.called)
         self.assertEqual(plan, output)
 
     @mock.patch(
@@ -124,15 +127,17 @@
     )
     async def test_should_review_output_and_flag(self, mock_async_openai):
         moderator = AzureContentSafetyModerator(
             options=AzureContentSafetyModeratorOptions(api_key="", moderate="output", endpoint="")
         )
         context = self.create_mock_context()
         state = await TurnState[ConversationState, UserState, TempState].load(context)
-        plan = Plan(commands=[PredictedSayCommand(response="test")])
+        plan = Plan(
+            commands=[PredictedSayCommand(response=Message[str](role="assistant", content="test"))]
+        )
         output = await moderator.review_output(context=context, state=state, plan=plan)
         self.assertTrue(mock_async_openai.called)
         assert output is not None
         self.assertEqual(len(output.commands), 1)
         self.assertEqual(output.commands[0].type, "DO")
         assert isinstance(output.commands[0], PredictedDoCommand)
         self.assertEqual(output.commands[0].action, ActionTypes.FLAGGED_OUTPUT)
@@ -143,15 +148,17 @@
     )
     async def test_should_review_output_and_error(self, mock_async_openai):
         moderator = AzureContentSafetyModerator(
             options=AzureContentSafetyModeratorOptions(api_key="", moderate="both", endpoint="")
         )
         context = self.create_mock_context()
         state = await TurnState[ConversationState, UserState, TempState].load(context)
-        plan = Plan(commands=[PredictedSayCommand(response="test")])
+        plan = Plan(
+            commands=[PredictedSayCommand(response=Message[str](role="assistant", content="test"))]
+        )
         output = await moderator.review_output(context=context, state=state, plan=plan)
         self.assertTrue(mock_async_openai.called)
         assert output is not None
         self.assertEqual(len(output.commands), 1)
         self.assertEqual(output.commands[0].type, "DO")
         assert isinstance(output.commands[0], PredictedDoCommand)
         self.assertEqual(output.commands[0].action, ActionTypes.HTTP_ERROR)
```

### Comparing `teams_ai-1.1.0/tests/ai/moderators/test_default_moderator.py` & `teams_ai-1.2.0/tests/ai/moderators/test_default_moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/moderators/test_openai_moderator.py` & `teams_ai-1.2.0/tests/ai/moderators/test_openai_moderator.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import httpx
 import openai
 from botbuilder.core import TurnContext
 
 from teams.ai.actions import ActionTypes
 from teams.ai.moderators import OpenAIModerator, OpenAIModeratorOptions
 from teams.ai.planners import Plan, PredictedDoCommand, PredictedSayCommand
+from teams.ai.prompts.message import Message
 from teams.state import ConversationState, TempState, TurnState, UserState
 
 
 class MockAsyncModerations:
     async def create(
         self,
         *,
@@ -174,41 +175,47 @@
         self.assertEqual(plan.commands[0].type, "DO")
         assert isinstance(plan.commands[0], PredictedDoCommand)
         self.assertEqual(plan.commands[0].action, ActionTypes.HTTP_ERROR)
 
     @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAI)
     async def test_should_not_review_output(self, mock_async_openai):
         moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="input"))
-        plan = Plan(commands=[PredictedSayCommand(response="test")])
+        plan = Plan(
+            commands=[PredictedSayCommand(response=Message[str](role="assistant", content="test"))]
+        )
         output = await moderator.review_output(
             context=cast(TurnContext, {}), state=TurnState(), plan=plan
         )
         self.assertTrue(mock_async_openai.called)
         self.assertEqual(plan, output)
 
     @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAIWithResults)
     async def test_should_review_output_and_flag(self, mock_async_openai):
         moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="output"))
         context = self.create_mock_context()
         state = await TurnState[ConversationState, UserState, TempState].load(context)
-        plan = Plan(commands=[PredictedSayCommand(response="test")])
+        plan = Plan(
+            commands=[PredictedSayCommand(response=Message[str](role="assistant", content="test"))]
+        )
         output = await moderator.review_output(context=context, state=state, plan=plan)
         self.assertTrue(mock_async_openai.called)
         assert output is not None
         self.assertEqual(len(output.commands), 1)
         self.assertEqual(output.commands[0].type, "DO")
         assert isinstance(output.commands[0], PredictedDoCommand)
         self.assertEqual(output.commands[0].action, ActionTypes.FLAGGED_OUTPUT)
 
     @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAIRateLimited)
     async def test_should_review_output_and_error(self, mock_async_openai):
         moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="both"))
         context = self.create_mock_context()
         state = await TurnState[ConversationState, UserState, TempState].load(context)
-        plan = Plan(commands=[PredictedSayCommand(response="test")])
+        plan = Plan(
+            commands=[PredictedSayCommand(response=Message[str](role="assistant", content="test"))]
+        )
         output = await moderator.review_output(context=context, state=state, plan=plan)
         self.assertTrue(mock_async_openai.called)
         assert output is not None
         self.assertEqual(len(output.commands), 1)
         self.assertEqual(output.commands[0].type, "DO")
         assert isinstance(output.commands[0], PredictedDoCommand)
         self.assertEqual(output.commands[0].action, ActionTypes.HTTP_ERROR)
```

### Comparing `teams_ai-1.1.0/tests/ai/planners/test_assistants_planner.py` & `teams_ai-1.2.0/tests/ai/planners/test_assistants_planner.py`

 * *Files 5% similar despite different names*

```diff
@@ -436,15 +436,16 @@
                     id=str(datetime.now()),
                     status="completed",
                     created_at=23123,
                     thread_id=new_thread.id,
                     assistant_id=ASSISTANT_ID,
                     content=[
                         TextContentBlock(
-                            type="text", text=Text(annotations=[], value=message["content"])
+                            type="text",
+                            text=Text(annotations=[], value=cast(str, message["content"])),
                         )
                     ],
                     object="thread.message",
                 )
                 new_messages.append(new_message)
 
         self._messages[new_thread.id] = new_messages
@@ -601,15 +602,19 @@
 
         plan = await assistants_planner.begin_task(context, state)
 
         self.assertTrue(mock_async_openai.called)
         self.assertNotEqual(plan, None)
         self.assertEqual(len(plan.commands), 1)
         self.assertEqual(plan.commands[0].type, "SAY")
-        self.assertEqual("welcome", cast(PredictedSayCommand, plan.commands[0]).response)
+        commands = cast(List[PredictedSayCommand], plan.commands)
+        if commands[0].response is not None:
+            self.assertEqual("welcome", commands[0].response.content)
+        else:
+            self.fail("commands[0].response is None")
 
     @mock.patch(
         "openai.AsyncOpenAI",
         return_value=MockAsyncOpenAI(
             remaining_run_status=["in_progress", "completed"], remaining_messages=["welcome"]
         ),
     )
@@ -627,15 +632,17 @@
 
         plan = await assistants_planner.begin_task(context, state)
 
         self.assertTrue(mock_async_openai.called)
         self.assertNotEqual(plan, None)
         self.assertEqual(len(plan.commands), 1)
         self.assertEqual(plan.commands[0].type, "SAY")
-        self.assertEqual("welcome", cast(PredictedSayCommand, plan.commands[0]).response)
+        commands = cast(List[PredictedSayCommand], plan.commands)
+        assert commands[0].response is not None
+        self.assertEqual("welcome", commands[0].response.content)
 
     @mock.patch(
         "openai.AsyncOpenAI",
         return_value=MockAsyncOpenAI(
             shared_messages={"123": []},
             shared_threads=[Thread(id="123", created_at=12323, object="thread")],
             shared_runs={
@@ -674,15 +681,17 @@
 
         plan = await assistants_planner.begin_task(context, state)
 
         self.assertTrue(mock_async_openai.called)
         self.assertNotEqual(plan, None)
         self.assertEqual(len(plan.commands), 1)
         self.assertEqual(plan.commands[0].type, "SAY")
-        self.assertEqual("welcome", cast(PredictedSayCommand, plan.commands[0]).response)
+        commands = cast(List[PredictedSayCommand], plan.commands)
+        assert commands[0].response is not None
+        self.assertEqual("welcome", commands[0].response.content)
 
     @mock.patch(
         "openai.AsyncOpenAI",
         return_value=MockAsyncOpenAI(
             remaining_run_status=["cancelled"], remaining_messages=["welcome"]
         ),
     )
@@ -789,25 +798,33 @@
                 assistant_id=ASSISTANT_ID,
             )
         )
 
         plan1 = await assistants_planner.continue_task(context, state)
         state.temp.action_outputs["test-action"] = "test-output"
         plan2 = await assistants_planner.continue_task(context, state)
+        commands1 = cast(List[PredictedDoCommand], plan1.commands)
+        commands2 = cast(List[PredictedSayCommand], plan2.commands)
 
         self.assertTrue(mock_async_openai.called)
         self.assertNotEqual(plan1, None)
         self.assertEqual(len(plan1.commands), 1)
         self.assertEqual(plan1.commands[0].type, "DO")
-        self.assertEqual("test-action", cast(PredictedDoCommand, plan1.commands[0]).action)
+        if commands1[0].action is not None:
+            self.assertEqual("test-action", commands1[0].action)
+        else:
+            self.fail("commands1[0].action is None")
 
         self.assertNotEqual(plan2, None)
         self.assertEqual(len(plan2.commands), 1)
         self.assertEqual(plan2.commands[0].type, "SAY")
-        self.assertEqual("welcome", cast(PredictedSayCommand, plan2.commands[0]).response)
+        if commands2[0].response is not None:
+            self.assertEqual("welcome", commands2[0].response.content)
+        else:
+            self.fail("commands2[0].response is None")
 
         tool_map = state.get("temp.submit_tool_map")
         if tool_map:
             self.assertTrue("test-action" in tool_map)
             self.assertEqual(tool_map["test-action"], "test-tool-id")
 
     @mock.patch(
@@ -855,15 +872,17 @@
         self.assertEqual(len(plan1.commands), 1)
         self.assertEqual(plan1.commands[0].type, "DO")
         self.assertEqual("test-action", cast(PredictedDoCommand, plan1.commands[0]).action)
 
         self.assertNotEqual(plan2, None)
         self.assertEqual(len(plan2.commands), 1)
         self.assertEqual(plan2.commands[0].type, "SAY")
-        self.assertEqual("welcome", cast(PredictedSayCommand, plan2.commands[0]).response)
+        commands = cast(List[PredictedSayCommand], plan2.commands)
+        assert commands[0].response is not None
+        self.assertEqual("welcome", commands[0].response.content)
 
         tool_map = state.get("temp.submit_tool_map")
         if tool_map:
             self.assertTrue("test-action" in tool_map)
             self.assertEqual(tool_map["test-action"], "test-tool-id")
 
     @mock.patch(
@@ -883,15 +902,24 @@
             OpenAIAssistantsOptions(
                 api_key="test-key",
                 assistant_id=ASSISTANT_ID,
             )
         )
 
         plan = await assistants_planner.continue_task(context, state)
+        commands = cast(List[PredictedSayCommand], plan.commands)
 
         self.assertTrue(mock_async_openai.called)
         self.assertNotEqual(plan, None)
-        self.assertEqual(len(plan.commands), 3)
-        self.assertEqual(plan.commands[0].type, "SAY")
-        self.assertEqual("message 2", cast(PredictedSayCommand, plan.commands[0]).response)
-        self.assertEqual("message 1", cast(PredictedSayCommand, plan.commands[1]).response)
-        self.assertEqual("welcome", cast(PredictedSayCommand, plan.commands[2]).response)
+        self.assertEqual(len(commands), 3)
+
+        self.assertEqual(commands[0].type, "SAY")
+        assert commands[0].response is not None
+        self.assertEqual("message 2", commands[0].response.content)
+
+        assert commands[1].type == "SAY"
+        assert commands[1].response is not None
+        self.assertEqual("message 1", commands[1].response.content)
+
+        assert commands[2].type == "SAY"
+        assert commands[2].response is not None
+        self.assertEqual("welcome", commands[2].response.content)
```

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_assets/happy_path/actions.json` & `teams_ai-1.2.0/tests/ai/prompts/test_assets/happy_path/actions.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_assets/happy_path/config.json` & `teams_ai-1.2.0/tests/ai/prompts/test_assets/happy_path/config.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_assets/include_images/config.json` & `teams_ai-1.2.0/tests/ai/prompts/test_assets/include_images/config.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_assets/no_prompt/config.json` & `teams_ai-1.2.0/tests/ai/prompts/test_assets/no_prompt/config.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_assistant_message.py` & `teams_ai-1.2.0/tests/ai/prompts/test_assistant_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_conversation_history.py` & `teams_ai-1.2.0/tests/ai/prompts/test_conversation_history.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_data_source_section.py` & `teams_ai-1.2.0/tests/ai/prompts/test_data_source_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_function_call_message.py` & `teams_ai-1.2.0/tests/ai/prompts/test_function_call_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_function_response_message.py` & `teams_ai-1.2.0/tests/ai/prompts/test_function_response_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_group_section.py` & `teams_ai-1.2.0/tests/ai/prompts/test_group_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_layout_engine.py` & `teams_ai-1.2.0/tests/ai/prompts/test_layout_engine.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_prompt_manager_v2.py` & `teams_ai-1.2.0/tests/ai/prompts/test_prompt_manager_v2.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_prompt_section_base.py` & `teams_ai-1.2.0/tests/ai/prompts/test_prompt_section_base.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_system_message.py` & `teams_ai-1.2.0/tests/ai/prompts/test_system_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_template_section.py` & `teams_ai-1.2.0/tests/ai/prompts/test_template_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_text_section.py` & `teams_ai-1.2.0/tests/ai/prompts/test_text_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_user_input_message.py` & `teams_ai-1.2.0/tests/ai/prompts/test_user_input_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/prompts/test_user_message.py` & `teams_ai-1.2.0/tests/ai/prompts/test_user_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/test_utilities.py` & `teams_ai-1.2.0/tests/utils/test_to_string.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import datetime
 import json
 from unittest import TestCase
 
 import yaml
 
 from teams.ai.tokenizers.gpt_tokenizer import GPTTokenizer
-from teams.ai.utilities import to_string
+from teams.utils import to_string
 
 
-class TestUtilities(TestCase):
+class TestToString(TestCase):
     def setUp(self):
         self.tokenizer = GPTTokenizer()
 
     def test_to_string_with_none(self):
         self.assertEqual(to_string(self.tokenizer, None), "")
 
     def test_to_string_with_string(self):
```

### Comparing `teams_ai-1.1.0/tests/ai/tokenizers/test_gpt_tokenizer.py` & `teams_ai-1.2.0/tests/ai/tokenizers/test_gpt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/validators/test_action_response_validator.py` & `teams_ai-1.2.0/tests/ai/validators/test_action_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/validators/test_default_response_validator.py` & `teams_ai-1.2.0/tests/ai/validators/test_default_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/ai/validators/test_json_response_validator.py` & `teams_ai-1.2.0/tests/ai/validators/test_json_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/auth/test_auth_manager.py` & `teams_ai-1.2.0/tests/auth/test_auth_manager.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/state/test_conversation_state.py` & `teams_ai-1.2.0/tests/state/test_conversation_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/state/test_custom_turn_state.py` & `teams_ai-1.2.0/tests/state/test_custom_turn_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/state/test_state.py` & `teams_ai-1.2.0/tests/state/test_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/state/test_temp_state.py` & `teams_ai-1.2.0/tests/state/test_temp_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/state/test_turn_state.py` & `teams_ai-1.2.0/tests/state/test_turn_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/state/test_user_state.py` & `teams_ai-1.2.0/tests/state/test_user_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/task_modules/test_task_modules.py` & `teams_ai-1.2.0/tests/task_modules/test_task_modules.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/test_app.py` & `teams_ai-1.2.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/test_meetings.py` & `teams_ai-1.2.0/tests/test_meetings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/test_message_extensions.py` & `teams_ai-1.2.0/tests/test_message_extensions.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/test_teams_attachment_downloader.py` & `teams_ai-1.2.0/tests/test_teams_attachment_downloader.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/utils/activity.py` & `teams_ai-1.2.0/tests/utils/activity.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/tests/utils/adapter.py` & `teams_ai-1.2.0/tests/utils/adapter.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.1.0/PKG-INFO` & `teams_ai-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: teams-ai
-Version: 1.1.0
+Version: 1.2.0
 Summary: SDK focused on building AI based applications for Microsoft Teams.
 Home-page: https://github.com/microsoft/teams-ai
 Keywords: microsoft,teams,ai,bot
 Author: Microsoft
 Author-email: teams@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
+Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: azure-ai-contentsafety (>=1.0.0,<2.0.0)
 Requires-Dist: botbuilder-core (>=4.15.0,<5.0.0)
 Requires-Dist: botbuilder-dialogs (>=4.14.8,<5.0.0)
 Requires-Dist: botbuilder-integration-aiohttp (>=4.15.0,<5.0.0)
 Requires-Dist: botframework-connector (>=4.15.0,<5.0.0)
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
 Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
```

