# Comparing `tmp/g4f-0.3.1.4.tar.gz` & `tmp/g4f-0.3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.1.4.tar", last modified: Sat May 18 14:55:18 2024, max compression
+gzip compressed data, was "g4f-0.3.1.5.tar", last modified: Sat May 18 21:36:48 2024, max compression
```

## Comparing `g4f-0.3.1.4.tar` & `g4f-0.3.1.5.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.084169 g4f-0.3.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-18 14:55:14.000000 g4f-0.3.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-18 14:55:14.000000 g4f-0.3.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-18 14:55:18.084169 g4f-0.3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    52480 2024-05-18 14:55:14.000000 g4f-0.3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.040169 g4f-0.3.1.4/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.052169 g4f-0.3.1.4/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/MetaAIAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Reka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.052169 g4f-0.3.1.4/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.060169 g4f-0.3.1.4/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.060169 g4f-0.3.1.4/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.060169 g4f-0.3.1.4/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    34879 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/PerplexityApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/openai/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/openai/proofofwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.036169 g4f-0.3.1.4/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.072169 g4f-0.3.1.4/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/css/dracula.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    22924 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.072169 g4f-0.3.1.4/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.072169 g4f-0.3.1.4/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    48500 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.072169 g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.076170 g4f-0.3.1.4/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.076170 g4f-0.3.1.4/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.076170 g4f-0.3.1.4/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.076170 g4f-0.3.1.4/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.080170 g4f-0.3.1.4/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.080170 g4f-0.3.1.4/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:55:18.084169 g4f-0.3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-18 14:55:14.000000 g4f-0.3.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.272410 g4f-0.3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-18 21:36:38.000000 g4f-0.3.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-18 21:36:38.000000 g4f-0.3.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    56222 2024-05-18 21:36:48.272410 g4f-0.3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    53026 2024-05-18 21:36:38.000000 g4f-0.3.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.236409 g4f-0.3.1.5/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.244409 g4f-0.3.1.5/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Reka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.244409 g4f-0.3.1.5/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.248409 g4f-0.3.1.5/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.248409 g4f-0.3.1.5/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.252409 g4f-0.3.1.5/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33245 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/PerplexityApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.252409 g4f-0.3.1.5/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/openai/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/openai/proofofwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.232409 g4f-0.3.1.5/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/css/dracula.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    23077 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.264409 g4f-0.3.1.5/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    49163 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.264409 g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.264409 g4f-0.3.1.5/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.264409 g4f-0.3.1.5/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.268410 g4f-0.3.1.5/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.268410 g4f-0.3.1.5/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.268410 g4f-0.3.1.5/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.268410 g4f-0.3.1.5/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    56222 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 21:36:48.272410 g4f-0.3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-18 21:36:38.000000 g4f-0.3.1.5/setup.py
```

### Comparing `g4f-0.3.1.4/LICENSE` & `g4f-0.3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/PKG-INFO` & `g4f-0.3.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.4
+Version: 0.3.1.5
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -310,27 +310,47 @@
 })
 
 set_cookies(".google.com", {
   "__Secure-1PSID": "cookie value"
 })
 ```
 
-Alternatively, you can place your .har and cookie files in the `/har_and_cookies` directory. To export a cookie file, use the EditThisCookie extension available on the Chrome Web Store: [EditThisCookie Extension](https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg).
+#### Using .har and Cookie Files
 
-You can also create .har files to capture cookies. If you need further assistance, refer to the next section.
+You can place `.har` and cookie files in the default `./har_and_cookies` directory. To export a cookie file, use the [EditThisCookie Extension](https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg) available on the Chrome Web Store.
 
-```bash
-python -m g4f.cli api --debug
+#### Creating .har Files to Capture Cookies
+
+To capture cookies, you can also create `.har` files. For more details, refer to the next section.
+
+#### Changing the Cookies Directory and Loading Cookie Files in Python
+
+You can change the cookies directory and load cookie files in your Python environment. To set the cookies directory relative to your Python file, use the following code:
+
+```python
+import os.path
+from g4f.cookies import set_cookies_dir, read_cookie_files
+
+import g4f.debug
+g4f.debug.logging = True
+
+cookies_dir = os.path.join(os.path.dirname(__file__), "har_and_cookies")
+set_cookies_dir(cookies_dir)
+read_cookie_files(cookies_dir)
 ```
+
+### Debug Mode
+
+If you enable debug mode, you will see logs similar to the following:
+
 ```
 Read .har file: ./har_and_cookies/you.com.har
 Cookies added: 10 from .you.com
 Read cookie file: ./har_and_cookies/google.json
 Cookies added: 16 from .google.com
-Starting server... [g4f v-0.0.0] (debug)
 ```
 
 #### .HAR File for OpenaiChat Provider
 
 ##### Generating a .HAR File
 
 To utilize the OpenaiChat provider, a .har file is required from https://chat.openai.com/. Follow the steps below to create a valid .har file:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.4 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.5 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -167,90 +167,97 @@
 Cookies Cookies are essential for using Meta AI and Microsoft Designer to
 create images. Additionally, cookies are required for the Google Gemini and
 WhiteRabbitNeo Provider. From Bing, ensure you have the "_U" cookie, and from
 Google, all cookies starting with "__Secure-1PSID" are needed. You can pass
 these cookies directly to the create function or set them using the
 `set_cookies` method before running G4F: ```python from g4f.cookies import
 set_cookies set_cookies(".bing.com", { "_U": "cookie value" }) set_cookies
-(".google.com", { "__Secure-1PSID": "cookie value" }) ``` Alternatively, you
-can place your .har and cookie files in the `/har_and_cookies` directory. To
-export a cookie file, use the EditThisCookie extension available on the Chrome
-Web Store: [EditThisCookie Extension](https://chromewebstore.google.com/detail/
-editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg). You can also create .har
-files to capture cookies. If you need further assistance, refer to the next
-section. ```bash python -m g4f.cli api --debug ``` ``` Read .har file: ./
-har_and_cookies/you.com.har Cookies added: 10 from .you.com Read cookie file:
-./har_and_cookies/google.json Cookies added: 16 from .google.com Starting
-server... [g4f v-0.0.0] (debug) ``` #### .HAR File for OpenaiChat Provider
-##### Generating a .HAR File To utilize the OpenaiChat provider, a .har file is
-required from https://chat.openai.com/. Follow the steps below to create a
-valid .har file: 1. Navigate to https://chat.openai.com/ using your preferred
-web browser and log in with your credentials. 2. Access the Developer Tools in
-your browser. This can typically be done by right-clicking the page and
-selecting "Inspect," or by pressing F12 or Ctrl+Shift+I (Cmd+Option+I on a
-Mac). 3. With the Developer Tools open, switch to the "Network" tab. 4. Reload
-the website to capture the loading process within the Network tab. 5. Initiate
-an action in the chat which can be captured in the .har file. 6. Right-click
-any of the network activities listed and select "Save all as HAR with content"
-to export the .har file. ##### Storing the .HAR File - Place the exported .har
-file in the `./har_and_cookies` directory if you are using Docker.
-Alternatively, you can store it in any preferred location within your current
-working directory. Note: Ensure that your .har file is stored securely, as it
-may contain sensitive information. #### Using Proxy If you want to hide or
-change your IP address for the providers, you can set a proxy globally via an
-environment variable: - On macOS and Linux: ```bash export G4F_PROXY="http://
-host:port" ``` - On Windows: ```bash set G4F_PROXY=http://host:port ``` ## ð
-Providers and Models ### GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream
-| Status | Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---
-- | | [bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ |
-âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
-[chatgpt.ai](https://chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ |
-âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[liaobots.site](https://liaobots.site) | `g4f.Provider.Liaobots` | âï¸ |
-âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â |
-| [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` |
-âï¸ | âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-
-brightgreen) | â+âï¸ | | [raycast.com](https://raycast.com) |
-`g4f.Provider.Raycast` | âï¸ | âï¸ | âï¸ | ![Unknown](https://
-img.shields.io/badge/Unknown-grey) | âï¸ | | [beta.theb.ai](https://
-beta.theb.ai) | `g4f.Provider.Theb` | âï¸ | âï¸ | âï¸ | ![Unknown]
-(https://img.shields.io/badge/Unknown-grey) | â | | [you.com](https://
-you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸ | ![Active](https://
-img.shields.io/badge/Active-brightgreen) | â | ## Best OpenSource Models
-While we wait for gpt-5, here is a list of new models that are at least better
-than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow. |
-Website | Provider | parameters | better than | | ------ | ------- | ------ | -
------ | | [claude-3-opus](https://anthropic.com/) | `g4f.Provider.You` | ?B |
-gpt-4-0125-preview | | [command-r+](https://txt.cohere.com/command-r-plus-
-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0314 | | [llama-
-3-70b](https://meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-
-0314 | | [claude-3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B |
-gpt-4-0314 | | [reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B |
-gpt-4-vision | | [dbrx-instruct](https://www.databricks.com/blog/introducing-
-dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active|
-gpt-3.5-turbo | | [mixtral-8x22b](https://huggingface.co/mistral-community/
-Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-
-turbo | ### GPT-3.5 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status |
-Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---- | |
-[chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace`
-| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
-| â | | [chat10.aichatos.xyz](https://chat10.aichatos.xyz) |
-`g4f.Provider.Aichatos` | âï¸ | â | âï¸ | ![Active](https://
-img.shields.io/badge/Active-brightgreen) | â | | [chatforai.store](https://
-chatforai.store) | `g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | !
+(".google.com", { "__Secure-1PSID": "cookie value" }) ``` #### Using .har and
+Cookie Files You can place `.har` and cookie files in the default `./
+har_and_cookies` directory. To export a cookie file, use the [EditThisCookie
+Extension](https://chromewebstore.google.com/detail/editthiscookie/
+fngmhnnpilhplaeedifhccceomclgfbg) available on the Chrome Web Store. ####
+Creating .har Files to Capture Cookies To capture cookies, you can also create
+`.har` files. For more details, refer to the next section. #### Changing the
+Cookies Directory and Loading Cookie Files in Python You can change the cookies
+directory and load cookie files in your Python environment. To set the cookies
+directory relative to your Python file, use the following code: ```python
+import os.path from g4f.cookies import set_cookies_dir, read_cookie_files
+import g4f.debug g4f.debug.logging = True cookies_dir = os.path.join
+(os.path.dirname(__file__), "har_and_cookies") set_cookies_dir(cookies_dir)
+read_cookie_files(cookies_dir) ``` ### Debug Mode If you enable debug mode, you
+will see logs similar to the following: ``` Read .har file: ./har_and_cookies/
+you.com.har Cookies added: 10 from .you.com Read cookie file: ./
+har_and_cookies/google.json Cookies added: 16 from .google.com ``` #### .HAR
+File for OpenaiChat Provider ##### Generating a .HAR File To utilize the
+OpenaiChat provider, a .har file is required from https://chat.openai.com/.
+Follow the steps below to create a valid .har file: 1. Navigate to https://
+chat.openai.com/ using your preferred web browser and log in with your
+credentials. 2. Access the Developer Tools in your browser. This can typically
+be done by right-clicking the page and selecting "Inspect," or by pressing F12
+or Ctrl+Shift+I (Cmd+Option+I on a Mac). 3. With the Developer Tools open,
+switch to the "Network" tab. 4. Reload the website to capture the loading
+process within the Network tab. 5. Initiate an action in the chat which can be
+captured in the .har file. 6. Right-click any of the network activities listed
+and select "Save all as HAR with content" to export the .har file. #####
+Storing the .HAR File - Place the exported .har file in the `./har_and_cookies`
+directory if you are using Docker. Alternatively, you can store it in any
+preferred location within your current working directory. Note: Ensure that
+your .har file is stored securely, as it may contain sensitive information.
+#### Using Proxy If you want to hide or change your IP address for the
+providers, you can set a proxy globally via an environment variable: - On macOS
+and Linux: ```bash export G4F_PROXY="http://host:port" ``` - On Windows:
+```bash set G4F_PROXY=http://host:port ``` ## ð Providers and Models ###
+GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | -----
+- | ------- | ------- | ----- | ------ | ------ | ---- | | [bing.com](https://
+bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ | âï¸ | ![Active](https:
+//img.shields.io/badge/Active-brightgreen) | â | | [chatgpt.ai](https://
+chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ | âï¸ | ![Unknown]
+(https://img.shields.io/badge/Unknown-grey) | â | | [liaobots.site](https://
+liaobots.site) | `g4f.Provider.Liaobots` | âï¸ | âï¸ | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | âï¸
+| âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen)
+| â+âï¸ | | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` |
+âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
+grey) | âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` |
+âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
+grey) | â | | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ |
+âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
+â | ## Best OpenSource Models While we wait for gpt-5, here is a list of new
+models that are at least better than gpt-3.5-turbo. **Some are better than gpt-
+4**. Expect this list to grow. | Website | Provider | parameters | better than
+| | ------ | ------- | ------ | ------ | | [claude-3-opus](https://
+anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0125-preview | | [command-r+]
+(https://txt.cohere.com/command-r-plus-microsoft-azure/) |
+`g4f.Provider.HuggingChat` | 104B | gpt-4-0314 | | [llama-3-70b](https://
+meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-0314 | | [claude-
+3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0314 | |
+[reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B | gpt-4-vision |
+| [dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-
+art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo | |
+[mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) |
+`g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo | ### GPT-3.5 |
+Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ----
+--- | ------- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
+chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
 [Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[chatgpt4online.org](https://chatgpt4online.org) |
-`g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | ![Unknown](https://
-img.shields.io/badge/Unknown-grey) | â | | [chatgpt-free.cc](https://
-www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ | â | âï¸ | !
-[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgptx.de]
-(https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â | âï¸ | !
-[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [f1.cnote.top]
-(https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â | âï¸ | !
-[Active](https://img.shields.io/badge/Active-brightgreen) | â | |
+[chat10.aichatos.xyz](https://chat10.aichatos.xyz) | `g4f.Provider.Aichatos` |
+âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
+brightgreen) | â | | [chatforai.store](https://chatforai.store) |
+`g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | ![Unknown](https://
+img.shields.io/badge/Unknown-grey) | â | | [chatgpt4online.org](https://
+chatgpt4online.org) | `g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt-
+free.cc](https://www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ |
+â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[chatgptx.de](https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â |
+âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[f1.cnote.top](https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â |
+âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [duckduckgo.com](https://duckduckgo.com/duckchat) | `g4f.Provider.DuckDuckGo` |
 âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
 brightgreen) | â | | [ecosia.org](https://www.ecosia.org) |
 `g4f.Provider.Ecosia` | âï¸ | â | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | | [feedough.com](https://
 www.feedough.com) | `g4f.Provider.Feedough` | âï¸ | â | âï¸ | ![Active]
 (https://img.shields.io/badge/Active-brightgreen) | â | | [flowgpt.com]
```

### Comparing `g4f-0.3.1.4/README.md` & `g4f-0.3.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -232,27 +232,47 @@
 })
 
 set_cookies(".google.com", {
   "__Secure-1PSID": "cookie value"
 })
 ```
 
-Alternatively, you can place your .har and cookie files in the `/har_and_cookies` directory. To export a cookie file, use the EditThisCookie extension available on the Chrome Web Store: [EditThisCookie Extension](https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg).
+#### Using .har and Cookie Files
 
-You can also create .har files to capture cookies. If you need further assistance, refer to the next section.
+You can place `.har` and cookie files in the default `./har_and_cookies` directory. To export a cookie file, use the [EditThisCookie Extension](https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg) available on the Chrome Web Store.
 
-```bash
-python -m g4f.cli api --debug
+#### Creating .har Files to Capture Cookies
+
+To capture cookies, you can also create `.har` files. For more details, refer to the next section.
+
+#### Changing the Cookies Directory and Loading Cookie Files in Python
+
+You can change the cookies directory and load cookie files in your Python environment. To set the cookies directory relative to your Python file, use the following code:
+
+```python
+import os.path
+from g4f.cookies import set_cookies_dir, read_cookie_files
+
+import g4f.debug
+g4f.debug.logging = True
+
+cookies_dir = os.path.join(os.path.dirname(__file__), "har_and_cookies")
+set_cookies_dir(cookies_dir)
+read_cookie_files(cookies_dir)
 ```
+
+### Debug Mode
+
+If you enable debug mode, you will see logs similar to the following:
+
 ```
 Read .har file: ./har_and_cookies/you.com.har
 Cookies added: 10 from .you.com
 Read cookie file: ./har_and_cookies/google.json
 Cookies added: 16 from .google.com
-Starting server... [g4f v-0.0.0] (debug)
 ```
 
 #### .HAR File for OpenaiChat Provider
 
 ##### Generating a .HAR File
 
 To utilize the OpenaiChat provider, a .har file is required from https://chat.openai.com/. Follow the steps below to create a valid .har file:
```

#### html2text {}

```diff
@@ -125,90 +125,97 @@
 Cookies Cookies are essential for using Meta AI and Microsoft Designer to
 create images. Additionally, cookies are required for the Google Gemini and
 WhiteRabbitNeo Provider. From Bing, ensure you have the "_U" cookie, and from
 Google, all cookies starting with "__Secure-1PSID" are needed. You can pass
 these cookies directly to the create function or set them using the
 `set_cookies` method before running G4F: ```python from g4f.cookies import
 set_cookies set_cookies(".bing.com", { "_U": "cookie value" }) set_cookies
-(".google.com", { "__Secure-1PSID": "cookie value" }) ``` Alternatively, you
-can place your .har and cookie files in the `/har_and_cookies` directory. To
-export a cookie file, use the EditThisCookie extension available on the Chrome
-Web Store: [EditThisCookie Extension](https://chromewebstore.google.com/detail/
-editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg). You can also create .har
-files to capture cookies. If you need further assistance, refer to the next
-section. ```bash python -m g4f.cli api --debug ``` ``` Read .har file: ./
-har_and_cookies/you.com.har Cookies added: 10 from .you.com Read cookie file:
-./har_and_cookies/google.json Cookies added: 16 from .google.com Starting
-server... [g4f v-0.0.0] (debug) ``` #### .HAR File for OpenaiChat Provider
-##### Generating a .HAR File To utilize the OpenaiChat provider, a .har file is
-required from https://chat.openai.com/. Follow the steps below to create a
-valid .har file: 1. Navigate to https://chat.openai.com/ using your preferred
-web browser and log in with your credentials. 2. Access the Developer Tools in
-your browser. This can typically be done by right-clicking the page and
-selecting "Inspect," or by pressing F12 or Ctrl+Shift+I (Cmd+Option+I on a
-Mac). 3. With the Developer Tools open, switch to the "Network" tab. 4. Reload
-the website to capture the loading process within the Network tab. 5. Initiate
-an action in the chat which can be captured in the .har file. 6. Right-click
-any of the network activities listed and select "Save all as HAR with content"
-to export the .har file. ##### Storing the .HAR File - Place the exported .har
-file in the `./har_and_cookies` directory if you are using Docker.
-Alternatively, you can store it in any preferred location within your current
-working directory. Note: Ensure that your .har file is stored securely, as it
-may contain sensitive information. #### Using Proxy If you want to hide or
-change your IP address for the providers, you can set a proxy globally via an
-environment variable: - On macOS and Linux: ```bash export G4F_PROXY="http://
-host:port" ``` - On Windows: ```bash set G4F_PROXY=http://host:port ``` ## ð
-Providers and Models ### GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream
-| Status | Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---
-- | | [bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ |
-âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
-[chatgpt.ai](https://chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ |
-âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[liaobots.site](https://liaobots.site) | `g4f.Provider.Liaobots` | âï¸ |
-âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â |
-| [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` |
-âï¸ | âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-
-brightgreen) | â+âï¸ | | [raycast.com](https://raycast.com) |
-`g4f.Provider.Raycast` | âï¸ | âï¸ | âï¸ | ![Unknown](https://
-img.shields.io/badge/Unknown-grey) | âï¸ | | [beta.theb.ai](https://
-beta.theb.ai) | `g4f.Provider.Theb` | âï¸ | âï¸ | âï¸ | ![Unknown]
-(https://img.shields.io/badge/Unknown-grey) | â | | [you.com](https://
-you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸ | ![Active](https://
-img.shields.io/badge/Active-brightgreen) | â | ## Best OpenSource Models
-While we wait for gpt-5, here is a list of new models that are at least better
-than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow. |
-Website | Provider | parameters | better than | | ------ | ------- | ------ | -
------ | | [claude-3-opus](https://anthropic.com/) | `g4f.Provider.You` | ?B |
-gpt-4-0125-preview | | [command-r+](https://txt.cohere.com/command-r-plus-
-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0314 | | [llama-
-3-70b](https://meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-
-0314 | | [claude-3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B |
-gpt-4-0314 | | [reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B |
-gpt-4-vision | | [dbrx-instruct](https://www.databricks.com/blog/introducing-
-dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active|
-gpt-3.5-turbo | | [mixtral-8x22b](https://huggingface.co/mistral-community/
-Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-
-turbo | ### GPT-3.5 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status |
-Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---- | |
-[chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace`
-| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
-| â | | [chat10.aichatos.xyz](https://chat10.aichatos.xyz) |
-`g4f.Provider.Aichatos` | âï¸ | â | âï¸ | ![Active](https://
-img.shields.io/badge/Active-brightgreen) | â | | [chatforai.store](https://
-chatforai.store) | `g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | !
+(".google.com", { "__Secure-1PSID": "cookie value" }) ``` #### Using .har and
+Cookie Files You can place `.har` and cookie files in the default `./
+har_and_cookies` directory. To export a cookie file, use the [EditThisCookie
+Extension](https://chromewebstore.google.com/detail/editthiscookie/
+fngmhnnpilhplaeedifhccceomclgfbg) available on the Chrome Web Store. ####
+Creating .har Files to Capture Cookies To capture cookies, you can also create
+`.har` files. For more details, refer to the next section. #### Changing the
+Cookies Directory and Loading Cookie Files in Python You can change the cookies
+directory and load cookie files in your Python environment. To set the cookies
+directory relative to your Python file, use the following code: ```python
+import os.path from g4f.cookies import set_cookies_dir, read_cookie_files
+import g4f.debug g4f.debug.logging = True cookies_dir = os.path.join
+(os.path.dirname(__file__), "har_and_cookies") set_cookies_dir(cookies_dir)
+read_cookie_files(cookies_dir) ``` ### Debug Mode If you enable debug mode, you
+will see logs similar to the following: ``` Read .har file: ./har_and_cookies/
+you.com.har Cookies added: 10 from .you.com Read cookie file: ./
+har_and_cookies/google.json Cookies added: 16 from .google.com ``` #### .HAR
+File for OpenaiChat Provider ##### Generating a .HAR File To utilize the
+OpenaiChat provider, a .har file is required from https://chat.openai.com/.
+Follow the steps below to create a valid .har file: 1. Navigate to https://
+chat.openai.com/ using your preferred web browser and log in with your
+credentials. 2. Access the Developer Tools in your browser. This can typically
+be done by right-clicking the page and selecting "Inspect," or by pressing F12
+or Ctrl+Shift+I (Cmd+Option+I on a Mac). 3. With the Developer Tools open,
+switch to the "Network" tab. 4. Reload the website to capture the loading
+process within the Network tab. 5. Initiate an action in the chat which can be
+captured in the .har file. 6. Right-click any of the network activities listed
+and select "Save all as HAR with content" to export the .har file. #####
+Storing the .HAR File - Place the exported .har file in the `./har_and_cookies`
+directory if you are using Docker. Alternatively, you can store it in any
+preferred location within your current working directory. Note: Ensure that
+your .har file is stored securely, as it may contain sensitive information.
+#### Using Proxy If you want to hide or change your IP address for the
+providers, you can set a proxy globally via an environment variable: - On macOS
+and Linux: ```bash export G4F_PROXY="http://host:port" ``` - On Windows:
+```bash set G4F_PROXY=http://host:port ``` ## ð Providers and Models ###
+GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | -----
+- | ------- | ------- | ----- | ------ | ------ | ---- | | [bing.com](https://
+bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ | âï¸ | ![Active](https:
+//img.shields.io/badge/Active-brightgreen) | â | | [chatgpt.ai](https://
+chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ | âï¸ | ![Unknown]
+(https://img.shields.io/badge/Unknown-grey) | â | | [liaobots.site](https://
+liaobots.site) | `g4f.Provider.Liaobots` | âï¸ | âï¸ | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | âï¸
+| âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen)
+| â+âï¸ | | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` |
+âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
+grey) | âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` |
+âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
+grey) | â | | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ |
+âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
+â | ## Best OpenSource Models While we wait for gpt-5, here is a list of new
+models that are at least better than gpt-3.5-turbo. **Some are better than gpt-
+4**. Expect this list to grow. | Website | Provider | parameters | better than
+| | ------ | ------- | ------ | ------ | | [claude-3-opus](https://
+anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0125-preview | | [command-r+]
+(https://txt.cohere.com/command-r-plus-microsoft-azure/) |
+`g4f.Provider.HuggingChat` | 104B | gpt-4-0314 | | [llama-3-70b](https://
+meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-0314 | | [claude-
+3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0314 | |
+[reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B | gpt-4-vision |
+| [dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-
+art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo | |
+[mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) |
+`g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo | ### GPT-3.5 |
+Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ----
+--- | ------- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
+chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
 [Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[chatgpt4online.org](https://chatgpt4online.org) |
-`g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | ![Unknown](https://
-img.shields.io/badge/Unknown-grey) | â | | [chatgpt-free.cc](https://
-www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ | â | âï¸ | !
-[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgptx.de]
-(https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â | âï¸ | !
-[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [f1.cnote.top]
-(https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â | âï¸ | !
-[Active](https://img.shields.io/badge/Active-brightgreen) | â | |
+[chat10.aichatos.xyz](https://chat10.aichatos.xyz) | `g4f.Provider.Aichatos` |
+âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
+brightgreen) | â | | [chatforai.store](https://chatforai.store) |
+`g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | ![Unknown](https://
+img.shields.io/badge/Unknown-grey) | â | | [chatgpt4online.org](https://
+chatgpt4online.org) | `g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt-
+free.cc](https://www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ |
+â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[chatgptx.de](https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â |
+âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[f1.cnote.top](https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â |
+âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [duckduckgo.com](https://duckduckgo.com/duckchat) | `g4f.Provider.DuckDuckGo` |
 âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
 brightgreen) | â | | [ecosia.org](https://www.ecosia.org) |
 `g4f.Provider.Ecosia` | âï¸ | â | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | | [feedough.com](https://
 www.feedough.com) | `g4f.Provider.Feedough` | âï¸ | â | âï¸ | ![Active]
 (https://img.shields.io/badge/Active-brightgreen) | â | | [flowgpt.com]
```

### Comparing `g4f-0.3.1.4/g4f/Provider/Aichatos.py` & `g4f-0.3.1.5/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Aura.py` & `g4f-0.3.1.5/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Bing.py` & `g4f-0.3.1.5/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Blackbox.py` & `g4f-0.3.1.5/g4f/Provider/Blackbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from __future__ import annotations
 
 import uuid
 import secrets
 from aiohttp import ClientSession
 
-from ..typing import AsyncResult, Messages
+from ..typing import AsyncResult, Messages, ImageType
+from ..image import to_data_uri
 from .base_provider import AsyncGeneratorProvider
 
 class Blackbox(AsyncGeneratorProvider):
     url = "https://www.blackbox.ai"
     working = True
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
+        image: ImageType = None,
+        image_name: str = None,
         **kwargs
     ) -> AsyncResult:
+        if image is not None:
+            messages[-1]["data"] = {
+                "fileText":	image_name,
+                "imageBase64": to_data_uri(image)
+            }
         headers = {
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
             "Accept": "*/*",
             "Accept-Language": "en-US,en;q=0.5",
             "Accept-Encoding": "gzip, deflate, br",
             "Referer": cls.url,
             "Content-Type": "application/json",
```

### Comparing `g4f-0.3.1.4/g4f/Provider/ChatForAi.py` & `g4f-0.3.1.5/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.1.5/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/ChatgptAi.py` & `g4f-0.3.1.5/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/ChatgptFree.py` & `g4f-0.3.1.5/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/ChatgptNext.py` & `g4f-0.3.1.5/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/ChatgptX.py` & `g4f-0.3.1.5/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Cnote.py` & `g4f-0.3.1.5/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Cohere.py` & `g4f-0.3.1.5/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/DeepInfra.py` & `g4f-0.3.1.5/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.1.5/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.1.5/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Ecosia.py` & `g4f-0.3.1.5/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Feedough.py` & `g4f-0.3.1.5/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/FlowGpt.py` & `g4f-0.3.1.5/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.1.5/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/FreeGpt.py` & `g4f-0.3.1.5/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/GeminiPro.py` & `g4f-0.3.1.5/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/GeminiProChat.py` & `g4f-0.3.1.5/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/GigaChat.py` & `g4f-0.3.1.5/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/GptTalkRu.py` & `g4f-0.3.1.5/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/HuggingChat.py` & `g4f-0.3.1.5/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/HuggingFace.py` & `g4f-0.3.1.5/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Koala.py` & `g4f-0.3.1.5/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Liaobots.py` & `g4f-0.3.1.5/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Llama.py` & `g4f-0.3.1.5/g4f/Provider/Llama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Local.py` & `g4f-0.3.1.5/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/MetaAI.py` & `g4f-0.3.1.5/g4f/Provider/MetaAI.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/MetaAIAccount.py` & `g4f-0.3.1.5/g4f/Provider/MetaAIAccount.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Ollama.py` & `g4f-0.3.1.5/g4f/Provider/Ollama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.1.5/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Pi.py` & `g4f-0.3.1.5/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Reka.py` & `g4f-0.3.1.5/g4f/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Replicate.py` & `g4f-0.3.1.5/g4f/Provider/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/ReplicateImage.py` & `g4f-0.3.1.5/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/Vercel.py` & `g4f-0.3.1.5/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.1.5/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/You.py` & `g4f-0.3.1.5/g4f/Provider/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/__init__.py` & `g4f-0.3.1.5/g4f/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/bing/conversation.py` & `g4f-0.3.1.5/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/bing/create_images.py` & `g4f-0.3.1.5/g4f/Provider/bing/create_images.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""
-This module provides functionalities for creating and managing images using Bing's service.
-It includes functions for user login, session creation, image creation, and processing.
-"""
 from __future__ import annotations
 
 import asyncio
 import time
 import json
 from aiohttp import ClientSession, BaseConnector
 from urllib.parse import quote
@@ -13,17 +9,15 @@
 
 try:
     from bs4 import BeautifulSoup
     has_requirements = True
 except ImportError:
     has_requirements = False
 
-from ...providers.create_images import CreateImagesProvider
 from ..helper import get_connector
-from ...providers.types import ProviderType
 from ...errors import MissingRequirementsError, RateLimitError
 from ...webdriver import WebDriver, get_driver_cookies, get_browser
 
 BING_URL = "https://www.bing.com"
 TIMEOUT_LOGIN = 1200
 TIMEOUT_IMAGE_CREATION = 300
 ERRORS = [
@@ -97,15 +91,15 @@
         "sec-fetch-user": "?1",
         "upgrade-insecure-requests": "1",
     }
     if cookies:
         headers["Cookie"] = "; ".join(f"{k}={v}" for k, v in cookies.items())
     return ClientSession(headers=headers, connector=get_connector(connector, proxy))
 
-async def create_images(session: ClientSession, prompt: str, proxy: str = None, timeout: int = TIMEOUT_IMAGE_CREATION) -> List[str]:
+async def create_images(session: ClientSession, prompt: str, timeout: int = TIMEOUT_IMAGE_CREATION) -> List[str]:
     """
     Creates images based on a given prompt using Bing's service.
 
     Args:
         session (ClientSession): Active client session.
         prompt (str): Prompt to generate images.
         proxy (str, optional): Proxy configuration.
@@ -128,15 +122,15 @@
         if "0 coins available" in text:
             raise RateLimitError("No coins left. Log in with a different account or wait a while")
         for error in ERRORS:
             if error in text:
                 raise RuntimeError(f"Create images failed: {error}")
     if response.status != 302:
         url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=3&FORM=GENCRE"
-        async with session.post(url, allow_redirects=False, proxy=proxy, timeout=timeout) as response:
+        async with session.post(url, allow_redirects=False, timeout=timeout) as response:
             if response.status != 302:
                 raise RuntimeError(f"Create images failed. Code: {response.status}")
 
     redirect_url = response.headers["Location"].replace("&nfy=1", "")
     redirect_url = f"{BING_URL}{redirect_url}"
     request_id = redirect_url.split("id=")[1]
     async with session.get(redirect_url) as response:
@@ -181,26 +175,8 @@
     if not tags:
         tags = soup.find_all("img", class_="gir_mmimg")
     images = [img["src"].split("?w=")[0] for img in tags]
     if any(im in BAD_IMAGES for im in images):
         raise RuntimeError("Bad images found")
     if not images:
         raise RuntimeError("No images found")
-    return images
-
-def patch_provider(provider: ProviderType) -> CreateImagesProvider:
-    """
-    Patches a provider to include image creation capabilities.
-
-    Args:
-        provider (ProviderType): The provider to be patched.
-
-    Returns:
-        CreateImagesProvider: The patched provider with image creation capabilities.
-    """
-    from ..BingCreateImages import BingCreateImages
-    service = BingCreateImages()
-    return CreateImagesProvider(
-        provider,
-        service.create,
-        service.create_async
-    )
+    return images
```

### Comparing `g4f-0.3.1.4/g4f/Provider/bing/upload_image.py` & `g4f-0.3.1.5/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/V50.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.1.5/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.1.5/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.1.5/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.1.5/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.1.5/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.1.5/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.1.5/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     pass
 
 from ..base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from ...webdriver import get_browser
 from ...typing import AsyncResult, Messages, Cookies, ImageType, AsyncIterator
 from ...requests import get_args_from_browser, raise_for_status
 from ...requests.aiohttp import StreamSession
-from ...image import to_image, to_bytes, ImageResponse, ImageRequest
+from ...image import ImageResponse, ImageRequest, to_image, to_bytes, is_accepted_format
 from ...errors import MissingAuthError, ResponseError
 from ...providers.conversation import BaseConversation
 from ..helper import format_cookies
 from ..openai.har_file import getArkoseAndAccessToken, NoValidHarFileError
 from ..openai.proofofwork import generate_proof_token
 from ... import debug
 
@@ -134,31 +134,30 @@
             headers: The headers to include in the requests
             image: The image to upload, either a PIL Image object or a bytes object
         
         Returns:
             An ImageRequest object that contains the download URL, file name, and other data
         """
         # Convert the image to a PIL Image object and get the extension
-        image = to_image(image)
-        extension = image.format.lower()
-        # Convert the image to a bytes object and get the size
         data_bytes = to_bytes(image)
+        image = to_image(data_bytes)
+        extension = image.format.lower()
         data = {
-            "file_name": image_name if image_name else f"{image.width}x{image.height}.{extension}",
+            "file_name": "" if image_name is None else image_name,
             "file_size": len(data_bytes),
             "use_case":	"multimodal"
         }
         # Post the image data to the service and get the image data
         async with session.post(f"{cls.url}/backend-api/files", json=data, headers=headers) as response:
-            cls._update_request_args()
+            cls._update_request_args(session)
             await raise_for_status(response)
             image_data = {
                 **data,
                 **await response.json(),
-                "mime_type": f"image/{extension}",
+                "mime_type": is_accepted_format(data_bytes),
                 "extension": extension,
                 "height": image.height,
                 "width": image.width
             }
         # Put the image bytes to the upload URL and check the status
         async with session.put(
             image_data["upload_url"],
@@ -271,15 +270,15 @@
             RuntimeError: If there'san error in downloading the image, including issues with the HTTP request or response.
         """
         if "parts" not in line["message"]["content"]:
             return
         first_part = line["message"]["content"]["parts"][0]
         if "asset_pointer" not in first_part or "metadata" not in first_part:
             return
-        if first_part["metadata"] is None:
+        if first_part["metadata"] is None or first_part["metadata"]["dalle"] is None:
             return
         prompt = first_part["metadata"]["dalle"]["prompt"]
         file_id = first_part["asset_pointer"].split("file-service://", 1)[1]
         try:
             async with session.get(f"{cls.url}/backend-api/files/{file_id}/download", headers=headers) as response:
                 cls._update_request_args(session)
                 await raise_for_status(response)
@@ -361,57 +360,25 @@
         async with StreamSession(
             proxy=proxy,
             impersonate="chrome",
             timeout=timeout
         ) as session:
             if cls._expires is not None and cls._expires < time.time():
                 cls._headers = cls._api_key = None
-            if cls._headers is None or cookies is not None:
-                cls._create_request_args(cookies)
-            api_key = kwargs["access_token"] if "access_token" in kwargs else api_key
-            if api_key is not None:
-                cls._set_api_key(api_key)
-
-            if cls.default_model is None and (not cls.needs_auth or cls._api_key is not None):
-                if cls._api_key is None:
-                    cls._create_request_args(cookies)
-                    async with session.get(
-                        f"{cls.url}/",
-                        headers=DEFAULT_HEADERS
-                    ) as response:
-                        cls._update_request_args(session)
-                        await raise_for_status(response)
-                try:
-                    if not model:
-                        cls.default_model = cls.get_model(await cls.get_default_model(session, cls._headers))
-                    else:
-                        cls.default_model = cls.get_model(model)
-                except MissingAuthError:
-                    pass
-                except Exception as e:
-                    api_key = cls._api_key = None
-                    cls._create_request_args()
-                    if debug.logging:
-                        print("OpenaiChat: Load default model failed")
-                        print(f"{e.__class__.__name__}: {e}")
-
             arkose_token = None
             proofTokens = None
-            if cls.default_model is None:
-                error = None
-                try:
-                    arkose_token, api_key, cookies, headers, proofTokens = await getArkoseAndAccessToken(proxy)
-                    cls._create_request_args(cookies, headers)
-                    cls._set_api_key(api_key)
-                except NoValidHarFileError as e:
-                    error = e
-                if cls._api_key is None:
-                    await cls.nodriver_access_token(proxy)
+            try:
+                arkose_token, api_key, cookies, headers, proofTokens = await getArkoseAndAccessToken(proxy)
+                cls._create_request_args(cookies, headers)
+                cls._set_api_key(api_key)
+            except NoValidHarFileError as e:
                 if cls._api_key is None and cls.needs_auth:
-                    raise error
+                    raise e
+
+            if cls.default_model is None:
                 cls.default_model = cls.get_model(await cls.get_default_model(session, cls._headers))
 
             try:
                 image_request = await cls.upload_image(session, cls._headers, image, image_name) if image else None
             except Exception as e:
                 image_request = None
                 if debug.logging:
@@ -457,15 +424,15 @@
                 if debug.logging:
                     print(
                         'Arkose:', False if not need_arkose else arkose_token[:12]+"...",
                         'Proofofwork:', False if proofofwork is None else proofofwork[:12]+"...",
                     )
                 ws = None
                 if need_arkose:
-                    async with session.post("https://chatgpt.com/backend-api/register-websocket", headers=cls._headers) as response:
+                    async with session.post(f"{cls.url}/backend-api/register-websocket", headers=cls._headers) as response:
                         wss_url = (await response.json()).get("wss_url")
                     if wss_url:
                         ws = await session.ws_connect(wss_url)    
                 websocket_request_id = str(uuid.uuid4())
                 data = {
                     "action": action,
                     "conversation_mode": {"kind": "primary_assistant"},
@@ -486,15 +453,16 @@
                     **cls._headers
                 }
                 if need_arkose:
                     headers["Openai-Sentinel-Arkose-Token"] = arkose_token
                 if proofofwork is not None:
                     headers["Openai-Sentinel-Proof-Token"] = proofofwork
                 async with session.post(
-                    f"{cls.url}/backend-anon/conversation" if cls._api_key is None else
+                    f"{cls.url}/backend-anon/conversation"
+                    if cls._api_key is None else
                     f"{cls.url}/backend-api/conversation",
                     json=data,
                     headers=headers
                 ) as response:
                     cls._update_request_args(session)
                     if response.status == 403 and max_retries > 0:
                         max_retries -= 1
@@ -576,20 +544,17 @@
             return
         if "message" not in line:
             return
         if "error" in line and line["error"]:
             raise RuntimeError(line["error"])
         if "message_type" not in line["message"]["metadata"]:
             return
-        try:
-            image_response = await cls.get_generated_image(session, cls._headers, line)
-            if image_response is not None:
-                yield image_response
-        except Exception as e:
-            yield e
+        image_response = await cls.get_generated_image(session, cls._headers, line)
+        if image_response is not None:
+            yield image_response
         if line["message"]["author"]["role"] != "assistant":
             return
         if line["message"]["content"]["content_type"] != "text":
             return
         if line["message"]["metadata"]["message_type"] not in ("next", "continue", "variant"):
             return
         if line["message"]["recipient"] != "all":
```

### Comparing `g4f-0.3.1.4/g4f/Provider/needs_auth/PerplexityApi.py` & `g4f-0.3.1.5/g4f/Provider/needs_auth/PerplexityApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.1.5/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.1.5/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.1.5/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.1.5/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.1.5/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.1.5/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.1.5/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.1.5/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.1.5/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.1.5/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.1.5/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.1.5/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.1.5/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.1.5/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.1.5/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.1.5/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.1.5/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.1.5/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.1.5/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/npm/package-lock.json` & `g4f-0.3.1.5/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/openai/crypt.py` & `g4f-0.3.1.5/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/openai/har_file.py` & `g4f-0.3.1.5/g4f/Provider/openai/har_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import uuid
 import random
 from urllib.parse import unquote
 from copy import deepcopy
 
 from .crypt import decrypt, encrypt
 from ...requests import StreamSession
+from ...cookies import get_cookies_dir
 from ... import debug
 
 class NoValidHarFileError(Exception):
     ...
 
 class arkReq:
     def __init__(self, arkURL, arkBx, arkHeader, arkBody, arkCookies, userAgent):
@@ -32,25 +33,22 @@
 accessToken: str = None
 cookies: dict = None
 headers: dict = None
 proofTokens: list = []
 
 def readHAR():
     global proofTokens
-    dirPath = "./"
     harPath = []
     chatArks = []
     accessToken = None
     cookies = {}
-    for root, dirs, files in os.walk(dirPath):
+    for root, dirs, files in os.walk(get_cookies_dir()):
         for file in files:
             if file.endswith(".har"):
                 harPath.append(os.path.join(root, file))
-        if harPath:
-            break
     if not harPath:
         raise NoValidHarFileError("No .har file found")
     for path in harPath:
         with open(path, 'rb') as file:
             try:
                 harFile = json.loads(file.read())
             except json.JSONDecodeError:
```

### Comparing `g4f-0.3.1.4/g4f/Provider/openai/proofofwork.py` & `g4f-0.3.1.5/g4f/Provider/openai/proofofwork.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.1.5/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/selenium/Bard.py` & `g4f-0.3.1.5/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.1.5/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.1.5/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/selenium/Phind.py` & `g4f-0.3.1.5/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.1.5/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.1.5/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.1.5/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.1.5/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.1.5/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/Provider/you/har_file.py` & `g4f-0.3.1.5/g4f/Provider/you/har_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import os
 import os.path
 import random
 import logging
 
 from ...requests import StreamSession, raise_for_status
+from ...cookies import get_cookies_dir
 from ...errors import MissingRequirementsError
 from ... import debug
 
 logging.basicConfig(level=logging.ERROR)
 
 class NoValidHarFileError(Exception):
     ...
@@ -24,18 +25,17 @@
         self.userAgent = userAgent
 
 telemetry_url = "https://telemetry.stytch.com/submit"
 public_token = "public-token-live-507a52ad-7e69-496b-aee0-1c9863c7c819"
 chatArks: list = None
 
 def readHAR():
-    dirPath = "./"
     harPath = []
     chatArks = []
-    for root, dirs, files in os.walk(dirPath):
+    for root, dirs, files in os.walk(get_cookies_dir()):
         for file in files:
             if file.endswith(".har"):
                 harPath.append(os.path.join(root, file))
         if harPath:
             break
     if not harPath:
         raise NoValidHarFileError("No .har file found")
@@ -61,24 +61,18 @@
         arkCookies={c['name']: c['value'] for c in entry['request']['cookies']},
         userAgent=""
     )
     tmpArk.userAgent = tmpArk.arkHeaders.get('user-agent', '')
     return tmpArk
 
 async def sendRequest(tmpArk: arkReq, proxy: str = None):
-    try:
-        async with StreamSession(headers=tmpArk.arkHeaders, cookies=tmpArk.arkCookies, proxy=proxy) as session:
-            async with session.post(tmpArk.arkURL, data=tmpArk.arkBody) as response:
-                await raise_for_status(response)
-                return await response.text()
-    except RuntimeError as e:
-        if str(e) == "Event loop is closed":
-            print("Event loop is closed error occurred in sendRequest.")
-        else:
-            raise
+    async with StreamSession(headers=tmpArk.arkHeaders, cookies=tmpArk.arkCookies, proxy=proxy) as session:
+        async with session.post(tmpArk.arkURL, data=tmpArk.arkBody) as response:
+            await raise_for_status(response)
+            return await response.text()
 
 async def create_telemetry_id(proxy: str = None):
     global chatArks
     if chatArks is None:
         chatArks = readHAR()
     return await sendRequest(random.choice(chatArks), proxy)
```

### Comparing `g4f-0.3.1.4/g4f/__init__.py` & `g4f-0.3.1.5/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/api/__init__.py` & `g4f-0.3.1.5/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/api/_logging.py` & `g4f-0.3.1.5/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/cli.py` & `g4f-0.3.1.5/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/client/async_client.py` & `g4f-0.3.1.5/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/client/client.py` & `g4f-0.3.1.5/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/client/helper.py` & `g4f-0.3.1.5/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/client/image_models.py` & `g4f-0.3.1.5/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/client/service.py` & `g4f-0.3.1.5/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/client/stubs.py` & `g4f-0.3.1.5/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/client/types.py` & `g4f-0.3.1.5/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/cookies.py` & `g4f-0.3.1.5/g4f/cookies.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 except ImportError:
     has_browser_cookie3 = False
 
 from .typing import Dict, Cookies
 from .errors import MissingRequirementsError
 from . import debug
 
-# Global variable to store cookies
-_cookies: Dict[str, Cookies] = {}
+class CookiesConfig():
+    cookies: Dict[str, Cookies] = {}
+    cookies_dir: str = "./har_and_cookies"
 
 DOMAINS = [
     ".bing.com",
     ".meta.ai",
     ".google.com",
     "www.whiterabbitneo.com",
     "huggingface.co",
@@ -44,28 +45,26 @@
 
     Args:
         domain_name (str): The domain for which to load cookies.
 
     Returns:
         Dict[str, str]: A dictionary of cookie names and values.
     """
-    global _cookies
-    if domain_name in _cookies:
-        return _cookies[domain_name]
+    if domain_name in CookiesConfig.cookies:
+        return CookiesConfig.cookies[domain_name]
 
     cookies = load_cookies_from_browsers(domain_name, raise_requirements_error, single_browser)
-    _cookies[domain_name] = cookies
+    CookiesConfig.cookies[domain_name] = cookies
     return cookies
 
 def set_cookies(domain_name: str, cookies: Cookies = None) -> None:
-    global _cookies
     if cookies:
-        _cookies[domain_name] = cookies
-    elif domain_name in _cookies:
-        _cookies.pop(domain_name)
+        CookiesConfig.cookies[domain_name] = cookies
+    elif domain_name in CookiesConfig.cookies:
+        CookiesConfig.cookies.pop(domain_name)
 
 def load_cookies_from_browsers(domain_name: str, raise_requirements_error: bool = True, single_browser: bool = False) -> Cookies:
     """
     Helper function to load cookies from various browsers.
 
     Args:
         domain_name (str): The domain for which to load cookies.
@@ -92,34 +91,40 @@
         except BrowserCookieError:
             pass
         except Exception as e:
             if debug.logging:
                 print(f"Error reading cookies from {cookie_fn.__name__} for {domain_name}: {e}")
     return cookies
 
-def read_cookie_files(dirPath: str = "./har_and_cookies"):
+def set_cookies_dir(dir: str) -> None:
+    CookiesConfig.cookies_dir = dir
+
+def get_cookies_dir() -> str:
+    return CookiesConfig.cookies_dir
+
+def read_cookie_files(dirPath: str = None):
     def get_domain(v: dict) -> str:
         host = [h["value"] for h in v['request']['headers'] if h["name"].lower() in ("host", ":authority")]
         if not host:
             return
         host = host.pop()
         for d in DOMAINS:
             if d in host:
                 return d
 
-    global _cookies
     harFiles = []
     cookieFiles = []
-    for root, dirs, files in os.walk(dirPath):
+    for root, dirs, files in os.walk(CookiesConfig.cookies_dir if dirPath is None else dirPath):
         for file in files:
             if file.endswith(".har"):
                 harFiles.append(os.path.join(root, file))
             elif file.endswith(".json"):
                 cookieFiles.append(os.path.join(root, file))
-    _cookies = {}
+
+    CookiesConfig.cookies = {}
     for path in harFiles:
         with open(path, 'rb') as file:
             try:
                 harFile = json.load(file)
             except json.JSONDecodeError:
                 # Error: not a HAR file!
                 continue
@@ -130,15 +135,15 @@
                 domain = get_domain(v)
                 if domain is None:
                     continue
                 v_cookies = {}
                 for c in v['request']['cookies']:
                     v_cookies[c['name']] = c['value']
                 if len(v_cookies) > 0:
-                    _cookies[domain] = v_cookies
+                    CookiesConfig.cookies[domain] = v_cookies
                     new_cookies[domain] = len(v_cookies)
             if debug.logging:
                 for domain, new_values in new_cookies.items():
                     print(f"Cookies added: {new_values} from {domain}")
     for path in cookieFiles:
         with open(path, 'rb') as file:
             try:
@@ -155,15 +160,15 @@
                 if isinstance(c, dict) and "domain" in c:
                     if c["domain"] not in new_cookies:
                         new_cookies[c["domain"]] = {}
                     new_cookies[c["domain"]][c["name"]] = c["value"]
             for domain, new_values in new_cookies.items():
                 if debug.logging:
                     print(f"Cookies added: {len(new_values)} from {domain}")
-                _cookies[domain] = new_values
+                CookiesConfig.cookies[domain] = new_values
 
 def _g4f(domain_name: str) -> list:
     """
     Load cookies from the 'g4f' browser (if exists).
 
     Args:
         domain_name (str): The domain for which to load cookies.
```

### Comparing `g4f-0.3.1.4/g4f/errors.py` & `g4f-0.3.1.5/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/__init__.py` & `g4f-0.3.1.5/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/index.html` & `g4f-0.3.1.5/g4f/gui/client/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -89,44 +89,44 @@
         <div class="images hidden">
             
         </div>
         <div class="settings hidden">
             <div class="paper">
             <h3>Settings</h3>
             <div class="field">
-                <span class="label">Web Access</span>
+                <span class="label">Web Access with DuckDuckGo</span>
                 <input type="checkbox" id="switch" />
                 <label for="switch" class="toogle" title="Add the pages of the first 5 search results to the query."></label>
             </div>
             <div class="field">
-                <span class="label">Disable History</span>
+                <span class="label">Disable Conversation History</span>
                 <input type="checkbox" id="history" />
                 <label for="history" class="toogle" title="To improve the reaction time or if you have trouble with large conversations."></label>
             </div>
             <div class="field">
-                <span class="label">Hide System prompt</span>
+                <span class="label">Hide System-prompt</span>
                 <input type="checkbox" id="hide-systemPrompt" />
                 <label for="hide-systemPrompt" class="toogle" title="For more space on phones"></label>
             </div>
             <div class="field">
-                <span class="label">Auto continue</span>
+                <span class="label">Auto continue in ChatGPT</span>
                 <input id="auto_continue" type="checkbox" name="auto_continue" checked/>
                 <label for="auto_continue" class="toogle" title="Continue large responses in OpenaiChat"></label>
             </div>
             <div class="field box">
                 <label for="message-input-height" class="label" title="">Input max. height</label>
                 <input type="number" id="message-input-height" value="200"/>
             </div>
             <div class="field box">
                 <label for="recognition-language" class="label" title="">Speech recognition lang</label>
                 <input type="text" id="recognition-language" value="" placeholder="navigator.language"/>
             </div>
             <div class="field box">
-                <label for="Bing-api_key" class="label" title="">Bing:</label>
-                <textarea id="Bing-api_key" name="Bing[api_key]" class="BingCreateImages-api_key" placeholder="&quot;_U&quot; cookie"></textarea>
+                <label for="BingCreateImages-api_key" class="label" title="">Microsoft Designer in Bing:</label>
+                <textarea id="BingCreateImages-api_key" name="BingCreateImages[api_key]" placeholder="&quot;_U&quot; cookie"></textarea>
             </div>
             <div class="field box">
                 <label for="DeepInfra-api_key" class="label" title="">DeepInfra:</label>
                 <textarea id="DeepInfra-api_key" name="DeepInfra[api_key]" class="DeepInfraImage-api_key" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
                 <label for="GeminiPro-api_key" class="label" title="">Gemini API:</label>
@@ -141,22 +141,22 @@
                 <textarea id="HuggingFace-api_key" name="HuggingFace[api_key]" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
                 <label for="Openai-api_key" class="label" title="">OpenAI API:</label>
                 <textarea id="Openai-api_key" name="Openai[api_key]" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
-                <label for="OpenaiAccount-api_key" class="label" title="">OpenAI ChatGPT:</label>
-                <textarea id="OpenaiAccount-api_key" name="OpenaiAccount[api_key]" class="OpenaiChat-api_key" placeholder="access_key"></textarea>
-            </div>
-            <div class="field box">
                 <label for="OpenRouter-api_key" class="label" title="">OpenRouter:</label>
                 <textarea id="OpenRouter-api_key" name="OpenRouter[api_key]" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
+                <label for="PerplexityApi-api_key" class="label" title="">Perplexity API:</label>
+                <textarea id="PerplexityApi-api_key" name="PerplexityApi[api_key]" placeholder="api_key"></textarea>
+            </div>
+            <div class="field box">
                 <label for="Replicate-api_key" class="label" title="">Replicate:</label>
                 <textarea id="Replicate-api_key" name="Replicate[api_key]" class="ReplicateImage-api_key" placeholder="api_key"></textarea>
             </div>
             </div>
             <div class="bottom_buttons">
                 <button onclick="delete_conversations()">
                     <i class="fa-regular fa-trash"></i>
@@ -169,15 +169,18 @@
             </div>
         </div>
         <div class="conversation">
             <textarea id="systemPrompt" class="box" placeholder="System prompt"></textarea>    
             <div id="messages" class="box"></div>
             <div class="toolbar">
                 <div id="input-count" class="">
-                    &nbsp;
+                    <button class="hide-input">
+                        <i class="fa-solid fa-angles-down"></i>
+                    </button>
+                    <span class="text"></span>
                 </div>
                 <div class="stop_generating stop_generating-hidden">
                     <button id="cancelButton">
                         <span>Stop Generating</span>
                         <i class="fa-regular fa-stop"></i>
                     </button>
                 </div>
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
 New Conversation
 Open Settings
 discord ~ _d_i_s_c_o_r_d_._g_g_/_X_f_y_b_z_P_X_P_H_5
 github ~ _@_x_t_e_k_k_y_/_g_p_t_4_f_r_e_e
 ******** SSeettttiinnggss ********
-Web Access??
-Disable History??
-Hide System prompt??
-Auto continue
+Web Access with DuckDuckGo??
+Disable Conversation History??
+Hide System-prompt??
+Auto continue in ChatGPT
 Input max. height[Unknown INPUT type]
 Speech recognition lang[                    ]
 Clear Conversations Export Conversations
- 
 Stop Generating
 Regenerate
 [File][File][File]
 [One of: Provider: Auto/Bing/OpenAI ChatGPT/Gemini/Liaobots/Meta AI/You/----]
```

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/css/dracula.min.css` & `g4f-0.3.1.5/g4f/gui/client/static/css/dracula.min.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/css/style.css` & `g4f-0.3.1.5/g4f/gui/client/static/css/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -453,15 +453,19 @@
 .toolbar {
     position: relative;
 }
 
 #input-count {
     width: fit-content;
     font-size: 12px;
-    padding: 6px var(--inner-gap);
+    padding: 6px 6px;
+}
+
+#input-count .text {
+    padding: 0 4px;
 }
 
 .stop_generating, .toolbar .regenerate {
     position: absolute;
     z-index: 1000000;
     top: 0;
     right: 0;
@@ -487,14 +491,21 @@
     justify-content: center;
     align-items: center;
     gap: 12px;
     cursor: pointer;
     animation: show_popup 0.4s;
 }
 
+.toolbar .hide-input {
+    background: transparent;
+    border: none;
+    color: var(--colour-3);
+    cursor: pointer;
+}
+
 @keyframes show_popup {
     from {
         opacity: 0;
         transform: translateY(10px);
     }
 }
```

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.1.5/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.1.5/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.1.5/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.1.5/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.1.5/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/img/user.png` & `g4f-0.3.1.5/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.1.5/g4f/gui/client/static/js/chat.v1.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
 const sidebar = document.querySelector(".conversations");
 const sidebar_button = document.querySelector(".mobile-sidebar");
 const sendButton = document.getElementById("send-button");
 const imageInput = document.getElementById("image");
 const cameraInput = document.getElementById("camera");
 const fileInput = document.getElementById("file");
 const microLabel = document.querySelector(".micro-label");
-const inputCount = document.getElementById("input-count");
+const inputCount = document.getElementById("input-count").querySelector(".text");
 const providerSelect = document.getElementById("provider");
 const modelSelect = document.getElementById("model");
 const modelProvider = document.getElementById("model2");
 const systemPrompt = document.getElementById("systemPrompt");
 const settings = document.querySelector(".settings");
 const chat = document.querySelector(".conversation");
 const album = document.querySelector(".images");
@@ -37,17 +37,15 @@
 appStorage = window.localStorage || {
     setItem: (key, value) => self[key] = value,
     getItem: (key) => self[key],
     removeItem: (key) => delete self[key],
     length: 0
 }
 
-const markdown = window.markdownit({
-    html: true,
-});
+const markdown = window.markdownit();
 const markdown_render = (content) => {
     return markdown.render(content
             .replaceAll(/<!-- generated images start -->|<!-- generated images end -->/gm, "")
             .replaceAll(/<img data-prompt="[^>]+">/gm, "")
         )
         .replaceAll("<a href=", '<a target="_blank" href=')
         .replaceAll('<code>', '<code class="language-plaintext">')
@@ -820,14 +818,25 @@
 document.getElementById("regenerateButton").addEventListener("click", async () => {
     prompt_lock = true;
     await hide_message(window.conversation_id);
     window.token = message_id();
     await ask_gpt();
 });
 
+const hide_input = document.querySelector(".toolbar .hide-input");
+hide_input.addEventListener("click", async (e) => {
+    const icon = hide_input.querySelector("i");
+    const func = icon.classList.contains("fa-angles-down") ? "add" : "remove";
+    const remv = icon.classList.contains("fa-angles-down") ? "remove" : "add";
+    icon.classList[func]("fa-angles-up");
+    icon.classList[remv]("fa-angles-down");
+    document.querySelector(".conversation .user-input").classList[func]("hidden");
+    document.querySelector(".conversation .buttons").classList[func]("hidden");
+});
+
 const uuid = () => {
     return `xxxxxxxx-xxxx-4xxx-yxxx-${Date.now().toString(16)}`.replace(
         /[xy]/g,
         function(c) {
             var r = (Math.random() * 16) | 0,
                 v = c == "x" ? r : (r & 0x3) | 0x8;
             return v.toString(16);
@@ -1023,15 +1032,15 @@
 let timeoutId;
 const count_input = async () => {
     if (timeoutId) clearTimeout(timeoutId);
     timeoutId = setTimeout(() => {
         if (countFocus.value) {
             inputCount.innerText = count_words_and_tokens(countFocus.value, get_selected_model());
         } else {
-            inputCount.innerHTML = "&nbsp;"
+            inputCount.innerText = "";
         }
     }, 100);
 };
 messageInput.addEventListener("keyup", count_input);
 systemPrompt.addEventListener("keyup", count_input);
 systemPrompt.addEventListener("focus", function() {
     countFocus = systemPrompt;
@@ -1067,22 +1076,24 @@
     load_conversations();
 }
 
 async function on_api() {
     messageInput.addEventListener("keydown", async (evt) => {
         if (prompt_lock) return;
 
-        if (evt.keyCode === 13 && !evt.shiftKey) {
-            evt.preventDefault();
-            console.log("pressed enter");
-            await handle_ask();
-        } else {
-            messageInput.style.removeProperty("height");
-            messageInput.style.height = messageInput.scrollHeight + "px";
-        }
+        // If not mobile
+        if (!window.matchMedia("(pointer:coarse)").matches)
+            if (evt.keyCode === 13 && !evt.shiftKey) {
+                evt.preventDefault();
+                console.log("pressed enter");
+                await handle_ask();
+            } else {
+                messageInput.style.removeProperty("height");
+                messageInput.style.height = messageInput.scrollHeight + "px";
+            }
     });
     sendButton.addEventListener(`click`, async () => {
         console.log("clicked send");
         if (prompt_lock) return;
         await handle_ask();
     });
     messageInput.focus();
@@ -1272,22 +1283,22 @@
     }
 }
 
 async function load_provider_models(providerIndex = null) {
     if (!providerIndex) {
         providerIndex = providerSelect.selectedIndex;
     }
+    modelProvider.innerHTML = '';
     const provider = providerSelect.options[providerIndex].value;
     if (!provider) {
         modelProvider.classList.add("hidden");
         modelSelect.classList.remove("hidden");
         return;
     }
     const models = await api('models', provider);
-    modelProvider.innerHTML = '';
     if (models.length > 0) {
         modelSelect.classList.add("hidden");
         modelProvider.classList.remove("hidden");
         models.forEach((model) => {
             let option = document.createElement('option');
             option.value = option.text = model.model;
             option.selected = model.default;
```

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.1.5/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.1.5/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/js/icons.js` & `g4f-0.3.1.5/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/server/android_gallery.py` & `g4f-0.3.1.5/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/server/api.py` & `g4f-0.3.1.5/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/server/backend.py` & `g4f-0.3.1.5/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/server/config.py` & `g4f-0.3.1.5/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/server/internet.py` & `g4f-0.3.1.5/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/server/js_api.py` & `g4f-0.3.1.5/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/server/website.py` & `g4f-0.3.1.5/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/gui/webview.py` & `g4f-0.3.1.5/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/image.py` & `g4f-0.3.1.5/g4f/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,16 +206,16 @@
     """
     if isinstance(images, str):
         result = f"[![{alt}]({preview.replace('{image}', images) if preview else images})]({images})"
     else:
         if not isinstance(preview, list):
             preview = [preview.replace('{image}', image) if preview else image for image in images]
         result = "\n".join(
-            #f"[![#{idx+1} {alt}]({preview[idx]})]({image})"
-            f'[<img src="{preview[idx]}" width="200" alt="#{idx+1} {alt}">]({image})'
+            f"[![#{idx+1} {alt}]({preview[idx]})]({image})"
+            #f'[<img src="{preview[idx]}" width="200" alt="#{idx+1} {alt}">]({image})'
             for idx, image in enumerate(images)
         )
     start_flag = "<!-- generated images start -->\n"
     end_flag = "<!-- generated images end -->\n"
     return f"\n{start_flag}{result}\n{end_flag}\n"
 
 def to_bytes(image: ImageType) -> bytes:
```

### Comparing `g4f-0.3.1.4/g4f/local/__init__.py` & `g4f-0.3.1.5/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/locals/models.py` & `g4f-0.3.1.5/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/locals/provider.py` & `g4f-0.3.1.5/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/models.py` & `g4f-0.3.1.5/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/providers/base_provider.py` & `g4f-0.3.1.5/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/providers/create_images.py` & `g4f-0.3.1.5/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/providers/helper.py` & `g4f-0.3.1.5/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/providers/retry_provider.py` & `g4f-0.3.1.5/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/providers/types.py` & `g4f-0.3.1.5/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/requests/__init__.py` & `g4f-0.3.1.5/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/requests/aiohttp.py` & `g4f-0.3.1.5/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/requests/curl_cffi.py` & `g4f-0.3.1.5/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/requests/defaults.py` & `g4f-0.3.1.5/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/requests/raise_for_status.py` & `g4f-0.3.1.5/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/stubs.py` & `g4f-0.3.1.5/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/typing.py` & `g4f-0.3.1.5/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/version.py` & `g4f-0.3.1.5/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f/webdriver.py` & `g4f-0.3.1.5/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f.egg-info/PKG-INFO` & `g4f-0.3.1.5/g4f.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.4
+Version: 0.3.1.5
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -310,27 +310,47 @@
 })
 
 set_cookies(".google.com", {
   "__Secure-1PSID": "cookie value"
 })
 ```
 
-Alternatively, you can place your .har and cookie files in the `/har_and_cookies` directory. To export a cookie file, use the EditThisCookie extension available on the Chrome Web Store: [EditThisCookie Extension](https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg).
+#### Using .har and Cookie Files
 
-You can also create .har files to capture cookies. If you need further assistance, refer to the next section.
+You can place `.har` and cookie files in the default `./har_and_cookies` directory. To export a cookie file, use the [EditThisCookie Extension](https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg) available on the Chrome Web Store.
 
-```bash
-python -m g4f.cli api --debug
+#### Creating .har Files to Capture Cookies
+
+To capture cookies, you can also create `.har` files. For more details, refer to the next section.
+
+#### Changing the Cookies Directory and Loading Cookie Files in Python
+
+You can change the cookies directory and load cookie files in your Python environment. To set the cookies directory relative to your Python file, use the following code:
+
+```python
+import os.path
+from g4f.cookies import set_cookies_dir, read_cookie_files
+
+import g4f.debug
+g4f.debug.logging = True
+
+cookies_dir = os.path.join(os.path.dirname(__file__), "har_and_cookies")
+set_cookies_dir(cookies_dir)
+read_cookie_files(cookies_dir)
 ```
+
+### Debug Mode
+
+If you enable debug mode, you will see logs similar to the following:
+
 ```
 Read .har file: ./har_and_cookies/you.com.har
 Cookies added: 10 from .you.com
 Read cookie file: ./har_and_cookies/google.json
 Cookies added: 16 from .google.com
-Starting server... [g4f v-0.0.0] (debug)
 ```
 
 #### .HAR File for OpenaiChat Provider
 
 ##### Generating a .HAR File
 
 To utilize the OpenaiChat provider, a .har file is required from https://chat.openai.com/. Follow the steps below to create a valid .har file:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.4 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.5 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -167,90 +167,97 @@
 Cookies Cookies are essential for using Meta AI and Microsoft Designer to
 create images. Additionally, cookies are required for the Google Gemini and
 WhiteRabbitNeo Provider. From Bing, ensure you have the "_U" cookie, and from
 Google, all cookies starting with "__Secure-1PSID" are needed. You can pass
 these cookies directly to the create function or set them using the
 `set_cookies` method before running G4F: ```python from g4f.cookies import
 set_cookies set_cookies(".bing.com", { "_U": "cookie value" }) set_cookies
-(".google.com", { "__Secure-1PSID": "cookie value" }) ``` Alternatively, you
-can place your .har and cookie files in the `/har_and_cookies` directory. To
-export a cookie file, use the EditThisCookie extension available on the Chrome
-Web Store: [EditThisCookie Extension](https://chromewebstore.google.com/detail/
-editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg). You can also create .har
-files to capture cookies. If you need further assistance, refer to the next
-section. ```bash python -m g4f.cli api --debug ``` ``` Read .har file: ./
-har_and_cookies/you.com.har Cookies added: 10 from .you.com Read cookie file:
-./har_and_cookies/google.json Cookies added: 16 from .google.com Starting
-server... [g4f v-0.0.0] (debug) ``` #### .HAR File for OpenaiChat Provider
-##### Generating a .HAR File To utilize the OpenaiChat provider, a .har file is
-required from https://chat.openai.com/. Follow the steps below to create a
-valid .har file: 1. Navigate to https://chat.openai.com/ using your preferred
-web browser and log in with your credentials. 2. Access the Developer Tools in
-your browser. This can typically be done by right-clicking the page and
-selecting "Inspect," or by pressing F12 or Ctrl+Shift+I (Cmd+Option+I on a
-Mac). 3. With the Developer Tools open, switch to the "Network" tab. 4. Reload
-the website to capture the loading process within the Network tab. 5. Initiate
-an action in the chat which can be captured in the .har file. 6. Right-click
-any of the network activities listed and select "Save all as HAR with content"
-to export the .har file. ##### Storing the .HAR File - Place the exported .har
-file in the `./har_and_cookies` directory if you are using Docker.
-Alternatively, you can store it in any preferred location within your current
-working directory. Note: Ensure that your .har file is stored securely, as it
-may contain sensitive information. #### Using Proxy If you want to hide or
-change your IP address for the providers, you can set a proxy globally via an
-environment variable: - On macOS and Linux: ```bash export G4F_PROXY="http://
-host:port" ``` - On Windows: ```bash set G4F_PROXY=http://host:port ``` ## ð
-Providers and Models ### GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream
-| Status | Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---
-- | | [bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ |
-âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
-[chatgpt.ai](https://chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ |
-âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[liaobots.site](https://liaobots.site) | `g4f.Provider.Liaobots` | âï¸ |
-âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â |
-| [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` |
-âï¸ | âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-
-brightgreen) | â+âï¸ | | [raycast.com](https://raycast.com) |
-`g4f.Provider.Raycast` | âï¸ | âï¸ | âï¸ | ![Unknown](https://
-img.shields.io/badge/Unknown-grey) | âï¸ | | [beta.theb.ai](https://
-beta.theb.ai) | `g4f.Provider.Theb` | âï¸ | âï¸ | âï¸ | ![Unknown]
-(https://img.shields.io/badge/Unknown-grey) | â | | [you.com](https://
-you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸ | ![Active](https://
-img.shields.io/badge/Active-brightgreen) | â | ## Best OpenSource Models
-While we wait for gpt-5, here is a list of new models that are at least better
-than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow. |
-Website | Provider | parameters | better than | | ------ | ------- | ------ | -
------ | | [claude-3-opus](https://anthropic.com/) | `g4f.Provider.You` | ?B |
-gpt-4-0125-preview | | [command-r+](https://txt.cohere.com/command-r-plus-
-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0314 | | [llama-
-3-70b](https://meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-
-0314 | | [claude-3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B |
-gpt-4-0314 | | [reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B |
-gpt-4-vision | | [dbrx-instruct](https://www.databricks.com/blog/introducing-
-dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active|
-gpt-3.5-turbo | | [mixtral-8x22b](https://huggingface.co/mistral-community/
-Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-
-turbo | ### GPT-3.5 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status |
-Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---- | |
-[chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace`
-| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
-| â | | [chat10.aichatos.xyz](https://chat10.aichatos.xyz) |
-`g4f.Provider.Aichatos` | âï¸ | â | âï¸ | ![Active](https://
-img.shields.io/badge/Active-brightgreen) | â | | [chatforai.store](https://
-chatforai.store) | `g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | !
+(".google.com", { "__Secure-1PSID": "cookie value" }) ``` #### Using .har and
+Cookie Files You can place `.har` and cookie files in the default `./
+har_and_cookies` directory. To export a cookie file, use the [EditThisCookie
+Extension](https://chromewebstore.google.com/detail/editthiscookie/
+fngmhnnpilhplaeedifhccceomclgfbg) available on the Chrome Web Store. ####
+Creating .har Files to Capture Cookies To capture cookies, you can also create
+`.har` files. For more details, refer to the next section. #### Changing the
+Cookies Directory and Loading Cookie Files in Python You can change the cookies
+directory and load cookie files in your Python environment. To set the cookies
+directory relative to your Python file, use the following code: ```python
+import os.path from g4f.cookies import set_cookies_dir, read_cookie_files
+import g4f.debug g4f.debug.logging = True cookies_dir = os.path.join
+(os.path.dirname(__file__), "har_and_cookies") set_cookies_dir(cookies_dir)
+read_cookie_files(cookies_dir) ``` ### Debug Mode If you enable debug mode, you
+will see logs similar to the following: ``` Read .har file: ./har_and_cookies/
+you.com.har Cookies added: 10 from .you.com Read cookie file: ./
+har_and_cookies/google.json Cookies added: 16 from .google.com ``` #### .HAR
+File for OpenaiChat Provider ##### Generating a .HAR File To utilize the
+OpenaiChat provider, a .har file is required from https://chat.openai.com/.
+Follow the steps below to create a valid .har file: 1. Navigate to https://
+chat.openai.com/ using your preferred web browser and log in with your
+credentials. 2. Access the Developer Tools in your browser. This can typically
+be done by right-clicking the page and selecting "Inspect," or by pressing F12
+or Ctrl+Shift+I (Cmd+Option+I on a Mac). 3. With the Developer Tools open,
+switch to the "Network" tab. 4. Reload the website to capture the loading
+process within the Network tab. 5. Initiate an action in the chat which can be
+captured in the .har file. 6. Right-click any of the network activities listed
+and select "Save all as HAR with content" to export the .har file. #####
+Storing the .HAR File - Place the exported .har file in the `./har_and_cookies`
+directory if you are using Docker. Alternatively, you can store it in any
+preferred location within your current working directory. Note: Ensure that
+your .har file is stored securely, as it may contain sensitive information.
+#### Using Proxy If you want to hide or change your IP address for the
+providers, you can set a proxy globally via an environment variable: - On macOS
+and Linux: ```bash export G4F_PROXY="http://host:port" ``` - On Windows:
+```bash set G4F_PROXY=http://host:port ``` ## ð Providers and Models ###
+GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | -----
+- | ------- | ------- | ----- | ------ | ------ | ---- | | [bing.com](https://
+bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ | âï¸ | ![Active](https:
+//img.shields.io/badge/Active-brightgreen) | â | | [chatgpt.ai](https://
+chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ | âï¸ | ![Unknown]
+(https://img.shields.io/badge/Unknown-grey) | â | | [liaobots.site](https://
+liaobots.site) | `g4f.Provider.Liaobots` | âï¸ | âï¸ | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | âï¸
+| âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen)
+| â+âï¸ | | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` |
+âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
+grey) | âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` |
+âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
+grey) | â | | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ |
+âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
+â | ## Best OpenSource Models While we wait for gpt-5, here is a list of new
+models that are at least better than gpt-3.5-turbo. **Some are better than gpt-
+4**. Expect this list to grow. | Website | Provider | parameters | better than
+| | ------ | ------- | ------ | ------ | | [claude-3-opus](https://
+anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0125-preview | | [command-r+]
+(https://txt.cohere.com/command-r-plus-microsoft-azure/) |
+`g4f.Provider.HuggingChat` | 104B | gpt-4-0314 | | [llama-3-70b](https://
+meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-0314 | | [claude-
+3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0314 | |
+[reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B | gpt-4-vision |
+| [dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-
+art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo | |
+[mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) |
+`g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo | ### GPT-3.5 |
+Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ----
+--- | ------- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
+chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
 [Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[chatgpt4online.org](https://chatgpt4online.org) |
-`g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | ![Unknown](https://
-img.shields.io/badge/Unknown-grey) | â | | [chatgpt-free.cc](https://
-www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ | â | âï¸ | !
-[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgptx.de]
-(https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â | âï¸ | !
-[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [f1.cnote.top]
-(https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â | âï¸ | !
-[Active](https://img.shields.io/badge/Active-brightgreen) | â | |
+[chat10.aichatos.xyz](https://chat10.aichatos.xyz) | `g4f.Provider.Aichatos` |
+âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
+brightgreen) | â | | [chatforai.store](https://chatforai.store) |
+`g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | ![Unknown](https://
+img.shields.io/badge/Unknown-grey) | â | | [chatgpt4online.org](https://
+chatgpt4online.org) | `g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt-
+free.cc](https://www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ |
+â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[chatgptx.de](https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â |
+âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[f1.cnote.top](https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â |
+âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [duckduckgo.com](https://duckduckgo.com/duckchat) | `g4f.Provider.DuckDuckGo` |
 âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
 brightgreen) | â | | [ecosia.org](https://www.ecosia.org) |
 `g4f.Provider.Ecosia` | âï¸ | â | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | | [feedough.com](https://
 www.feedough.com) | `g4f.Provider.Feedough` | âï¸ | â | âï¸ | ![Active]
 (https://img.shields.io/badge/Active-brightgreen) | â | | [flowgpt.com]
```

### Comparing `g4f-0.3.1.4/g4f.egg-info/SOURCES.txt` & `g4f-0.3.1.5/g4f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/g4f.egg-info/requires.txt` & `g4f-0.3.1.5/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.4/setup.py` & `g4f-0.3.1.5/setup.py`

 * *Files identical despite different names*

