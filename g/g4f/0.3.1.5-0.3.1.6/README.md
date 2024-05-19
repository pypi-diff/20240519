# Comparing `tmp/g4f-0.3.1.5.tar.gz` & `tmp/g4f-0.3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.1.5.tar", last modified: Sat May 18 21:36:48 2024, max compression
+gzip compressed data, was "g4f-0.3.1.6.tar", last modified: Sun May 19 04:02:11 2024, max compression
```

## Comparing `g4f-0.3.1.5.tar` & `g4f-0.3.1.6.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.272410 g4f-0.3.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-18 21:36:38.000000 g4f-0.3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-18 21:36:38.000000 g4f-0.3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    56222 2024-05-18 21:36:48.272410 g4f-0.3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    53026 2024-05-18 21:36:38.000000 g4f-0.3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.236409 g4f-0.3.1.5/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.244409 g4f-0.3.1.5/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/MetaAIAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Reka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.244409 g4f-0.3.1.5/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.248409 g4f-0.3.1.5/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.248409 g4f-0.3.1.5/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.252409 g4f-0.3.1.5/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    33245 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/PerplexityApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.252409 g4f-0.3.1.5/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/openai/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/openai/proofofwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.256409 g4f-0.3.1.5/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.232409 g4f-0.3.1.5/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/css/dracula.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    23077 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.260409 g4f-0.3.1.5/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.264409 g4f-0.3.1.5/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    49163 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.264409 g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.264409 g4f-0.3.1.5/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.264409 g4f-0.3.1.5/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.268410 g4f-0.3.1.5/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.268410 g4f-0.3.1.5/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.268410 g4f-0.3.1.5/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-18 21:36:38.000000 g4f-0.3.1.5/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:36:48.268410 g4f-0.3.1.5/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    56222 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 21:36:48.000000 g4f-0.3.1.5/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 21:36:48.272410 g4f-0.3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-18 21:36:38.000000 g4f-0.3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.377868 g4f-0.3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-19 04:02:00.000000 g4f-0.3.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-19 04:02:00.000000 g4f-0.3.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    56222 2024-05-19 04:02:11.377868 g4f-0.3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    53026 2024-05-19 04:02:00.000000 g4f-0.3.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.337868 g4f-0.3.1.6/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.345868 g4f-0.3.1.6/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Reka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.345868 g4f-0.3.1.6/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.353868 g4f-0.3.1.6/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.353868 g4f-0.3.1.6/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.353868 g4f-0.3.1.6/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33277 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/PerplexityApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.357868 g4f-0.3.1.6/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.357868 g4f-0.3.1.6/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.357868 g4f-0.3.1.6/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.357868 g4f-0.3.1.6/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.357868 g4f-0.3.1.6/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/openai/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/openai/proofofwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.361868 g4f-0.3.1.6/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.361868 g4f-0.3.1.6/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.361868 g4f-0.3.1.6/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.361868 g4f-0.3.1.6/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.361868 g4f-0.3.1.6/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.365868 g4f-0.3.1.6/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.365868 g4f-0.3.1.6/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.333868 g4f-0.3.1.6/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.365868 g4f-0.3.1.6/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/css/dracula.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.365868 g4f-0.3.1.6/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.365868 g4f-0.3.1.6/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    50252 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.369868 g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.369868 g4f-0.3.1.6/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.369868 g4f-0.3.1.6/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.369868 g4f-0.3.1.6/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.373868 g4f-0.3.1.6/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.373868 g4f-0.3.1.6/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.373868 g4f-0.3.1.6/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    56222 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 04:02:11.377868 g4f-0.3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-19 04:02:00.000000 g4f-0.3.1.6/setup.py
```

### Comparing `g4f-0.3.1.5/LICENSE` & `g4f-0.3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/PKG-INFO` & `g4f-0.3.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.5
+Version: 0.3.1.6
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.5 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.6 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.1.5/README.md` & `g4f-0.3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Aichatos.py` & `g4f-0.3.1.6/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Aura.py` & `g4f-0.3.1.6/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Bing.py` & `g4f-0.3.1.6/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/BingCreateImages.py` & `g4f-0.3.1.6/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Blackbox.py` & `g4f-0.3.1.6/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/ChatForAi.py` & `g4f-0.3.1.6/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.1.6/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/ChatgptAi.py` & `g4f-0.3.1.6/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/ChatgptFree.py` & `g4f-0.3.1.6/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/ChatgptNext.py` & `g4f-0.3.1.6/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/ChatgptX.py` & `g4f-0.3.1.6/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Cnote.py` & `g4f-0.3.1.6/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Cohere.py` & `g4f-0.3.1.6/g4f/Provider/Cohere.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ..typing import CreateResult, Messages
 from .base_provider import AbstractProvider
 from .helper import format_prompt
 
 class Cohere(AbstractProvider):
     url                   = "https://cohereforai-c4ai-command-r-plus.hf.space"
-    working               = True
+    working               = False
     supports_gpt_35_turbo = False
     supports_gpt_4        = False
     supports_stream       = True
     
     @staticmethod
     def create_completion(
         model: str,
```

### Comparing `g4f-0.3.1.5/g4f/Provider/DeepInfra.py` & `g4f-0.3.1.6/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.1.6/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.1.6/g4f/Provider/DuckDuckGo.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,19 @@
 class DuckDuckGo(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://duckduckgo.com/duckchat"
     working = True
     supports_gpt_35_turbo = True
     supports_message_history = True
 
     default_model = "gpt-3.5-turbo-0125"
-    models = ["gpt-3.5-turbo-0125", "claude-instant-1.2"]
-    model_aliases = {"gpt-3.5-turbo": "gpt-3.5-turbo-0125"}
+    models = ["gpt-3.5-turbo-0125", "claude-3-haiku-20240307"]
+    model_aliases = {
+        "gpt-3.5-turbo": "gpt-3.5-turbo-0125",
+        "claude-3-haiku": "claude-3-haiku-20240307"
+    }
 
     status_url = "https://duckduckgo.com/duckchat/v1/status"
     chat_url = "https://duckduckgo.com/duckchat/v1/chat"
     user_agent = 'Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:123.0) Gecko/20100101 Firefox/123.0'
     headers = {
         'User-Agent': user_agent,
         'Accept': 'text/event-stream',
```

### Comparing `g4f-0.3.1.5/g4f/Provider/Ecosia.py` & `g4f-0.3.1.6/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Feedough.py` & `g4f-0.3.1.6/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/FlowGpt.py` & `g4f-0.3.1.6/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.1.6/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/FreeGpt.py` & `g4f-0.3.1.6/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/GeminiPro.py` & `g4f-0.3.1.6/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/GeminiProChat.py` & `g4f-0.3.1.6/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/GigaChat.py` & `g4f-0.3.1.6/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/GptTalkRu.py` & `g4f-0.3.1.6/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/HuggingChat.py` & `g4f-0.3.1.6/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/HuggingFace.py` & `g4f-0.3.1.6/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Koala.py` & `g4f-0.3.1.6/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Liaobots.py` & `g4f-0.3.1.6/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Llama.py` & `g4f-0.3.1.6/g4f/Provider/Llama.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..typing import AsyncResult, Messages
 from ..requests.raise_for_status import raise_for_status
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 
 
 class Llama(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://www.llama2.ai"
-    working = True
+    working = False
     supports_message_history = True
     default_model = "meta/meta-llama-3-70b-instruct"
     models = [
         "meta/llama-2-7b-chat",
         "meta/llama-2-13b-chat",
         "meta/llama-2-70b-chat",
         "meta/meta-llama-3-8b-instruct",
```

### Comparing `g4f-0.3.1.5/g4f/Provider/Local.py` & `g4f-0.3.1.6/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/MetaAI.py` & `g4f-0.3.1.6/g4f/Provider/MetaAI.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/MetaAIAccount.py` & `g4f-0.3.1.6/g4f/Provider/MetaAIAccount.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Ollama.py` & `g4f-0.3.1.6/g4f/Provider/Ollama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.1.6/g4f/Provider/PerplexityLabs.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,22 @@
     models = [
         "llama-3-sonar-large-32k-online", "llama-3-sonar-small-32k-online", "llama-3-sonar-large-32k-chat", "llama-3-sonar-small-32k-chat",
         "dbrx-instruct", "claude-3-haiku-20240307", "llama-3-8b-instruct", "llama-3-70b-instruct", "codellama-70b-instruct", "mistral-7b-instruct",
         "llava-v1.5-7b-wrapper", "llava-v1.6-34b", "mixtral-8x7b-instruct", "mixtral-8x22b-instruct", "mistral-medium", "gemma-2b-it", "gemma-7b-it",
         "related"
     ]
     model_aliases = {
-        "mistralai/Mistral-7B-Instruct-v0.1": "mistral-7b-instruct", 
+        "mistralai/Mistral-7B-Instruct-v0.1": "mistral-7b-instruct",
+        "mistralai/Mistral-7B-Instruct-v0.2": "mistral-7b-instruct",
         "mistralai/Mixtral-8x7B-Instruct-v0.1": "mixtral-8x7b-instruct",
         "codellama/CodeLlama-70b-Instruct-hf": "codellama-70b-instruct",
         "llava-v1.5-7b": "llava-v1.5-7b-wrapper",
-        'databricks/dbrx-instruct': "dbrx-instruct"
+        "databricks/dbrx-instruct": "dbrx-instruct",
+        "meta-llama/Meta-Llama-3-70B-Instruct": "llama-3-70b-instruct",
+        "meta-llama/Meta-Llama-3-8B-Instruct": "llama-3-8b-instruct"
     }
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
```

### Comparing `g4f-0.3.1.5/g4f/Provider/Pi.py` & `g4f-0.3.1.6/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Reka.py` & `g4f-0.3.1.6/g4f/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Replicate.py` & `g4f-0.3.1.6/g4f/Provider/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/ReplicateImage.py` & `g4f-0.3.1.6/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/Vercel.py` & `g4f-0.3.1.6/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.1.6/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/You.py` & `g4f-0.3.1.6/g4f/Provider/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/__init__.py` & `g4f-0.3.1.6/g4f/Provider/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from ..providers.types          import BaseProvider, ProviderType
-from ..providers.retry_provider import RetryProvider, IterProvider
+from ..providers.retry_provider import RetryProvider, IterListProvider
 from ..providers.base_provider  import AsyncProvider, AsyncGeneratorProvider
 from ..providers.create_images  import CreateImagesProvider
 
 from .deprecated      import *
 from .not_working     import *
 from .selenium        import *
 from .needs_auth      import *
```

### Comparing `g4f-0.3.1.5/g4f/Provider/bing/conversation.py` & `g4f-0.3.1.6/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/bing/create_images.py` & `g4f-0.3.1.6/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/bing/upload_image.py` & `g4f-0.3.1.6/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/V50.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.1.6/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.1.6/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.1.6/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.1.6/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.1.6/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.1.6/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.1.6/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,14 +369,15 @@
             try:
                 arkose_token, api_key, cookies, headers, proofTokens = await getArkoseAndAccessToken(proxy)
                 cls._create_request_args(cookies, headers)
                 cls._set_api_key(api_key)
             except NoValidHarFileError as e:
                 if cls._api_key is None and cls.needs_auth:
                     raise e
+                cls._create_request_args()
 
             if cls.default_model is None:
                 cls.default_model = cls.get_model(await cls.get_default_model(session, cls._headers))
 
             try:
                 image_request = await cls.upload_image(session, cls._headers, image, image_name) if image else None
             except Exception as e:
@@ -416,15 +417,15 @@
                         raise MissingAuthError("No arkose token found in .har file")
 
                 if "proofofwork" in requirements:
                     proofofwork = generate_proof_token(
                         **requirements["proofofwork"],
                         user_agent=cls._headers["user-agent"],
                         proofTokens=proofTokens
-                    )           
+                    )
                 if debug.logging:
                     print(
                         'Arkose:', False if not need_arkose else arkose_token[:12]+"...",
                         'Proofofwork:', False if proofofwork is None else proofofwork[:12]+"...",
                     )
                 ws = None
                 if need_arkose:
```

### Comparing `g4f-0.3.1.5/g4f/Provider/needs_auth/PerplexityApi.py` & `g4f-0.3.1.6/g4f/Provider/needs_auth/PerplexityApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.1.6/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.1.6/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.1.6/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.1.6/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.1.6/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.1.6/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.1.6/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.1.6/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.1.6/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.1.6/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.1.6/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.1.6/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.1.6/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.1.6/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.1.6/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.1.6/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.1.6/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.1.6/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.1.6/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/npm/package-lock.json` & `g4f-0.3.1.6/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/openai/crypt.py` & `g4f-0.3.1.6/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/openai/har_file.py` & `g4f-0.3.1.6/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/openai/proofofwork.py` & `g4f-0.3.1.6/g4f/Provider/openai/proofofwork.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.1.6/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/selenium/Bard.py` & `g4f-0.3.1.6/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.1.6/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.1.6/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/selenium/Phind.py` & `g4f-0.3.1.6/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.1.6/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.1.6/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.1.6/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.1.6/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.1.6/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/Provider/you/har_file.py` & `g4f-0.3.1.6/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/__init__.py` & `g4f-0.3.1.6/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/api/__init__.py` & `g4f-0.3.1.6/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/api/_logging.py` & `g4f-0.3.1.6/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/cli.py` & `g4f-0.3.1.6/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/client/async_client.py` & `g4f-0.3.1.6/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/client/client.py` & `g4f-0.3.1.6/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/client/helper.py` & `g4f-0.3.1.6/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/client/image_models.py` & `g4f-0.3.1.6/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/client/service.py` & `g4f-0.3.1.6/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/client/stubs.py` & `g4f-0.3.1.6/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/client/types.py` & `g4f-0.3.1.6/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/cookies.py` & `g4f-0.3.1.6/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/errors.py` & `g4f-0.3.1.6/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/__init__.py` & `g4f-0.3.1.6/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/index.html` & `g4f-0.3.1.6/g4f/gui/client/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,19 @@
         <div class="images hidden">
             
         </div>
         <div class="settings hidden">
             <div class="paper">
             <h3>Settings</h3>
             <div class="field">
+                <span class="label">Enable Dark Mode</span>
+                <input type="checkbox" id="darkMode" checked />
+                <label for="darkMode" class="toogle" title=""></label>
+            </div>
+            <div class="field">
                 <span class="label">Web Access with DuckDuckGo</span>
                 <input type="checkbox" id="switch" />
                 <label for="switch" class="toogle" title="Add the pages of the first 5 search results to the query."></label>
             </div>
             <div class="field">
                 <span class="label">Disable Conversation History</span>
                 <input type="checkbox" id="history" />
@@ -165,16 +170,19 @@
                 <button onclick="save_storage()">
                     <i class="fa-solid fa-download"></i>
                     <a href="" onclick="return false;">Export Conversations</a>
                 </button>
             </div>
         </div>
         <div class="conversation">
-            <textarea id="systemPrompt" class="box" placeholder="System prompt"></textarea>    
+            <textarea id="systemPrompt" class="box" placeholder="System prompt"></textarea>
             <div id="messages" class="box"></div>
+            <button class="slide-systemPrompt">
+                <i class="fa-solid fa-angles-up"></i>
+            </button>
             <div class="toolbar">
                 <div id="input-count" class="">
                     <button class="hide-input">
                         <i class="fa-solid fa-angles-down"></i>
                     </button>
                     <span class="text"></span>
                 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 New Conversation
 Open Settings
 discord ~ _d_i_s_c_o_r_d_._g_g_/_X_f_y_b_z_P_X_P_H_5
 github ~ _@_x_t_e_k_k_y_/_g_p_t_4_f_r_e_e
 ******** SSeettttiinnggss ********
+Enable Dark Mode
 Web Access with DuckDuckGo??
 Disable Conversation History??
 Hide System-prompt??
 Auto continue in ChatGPT
 Input max. height[Unknown INPUT type]
 Speech recognition lang[                    ]
 Clear Conversations Export Conversations
```

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/css/dracula.min.css` & `g4f-0.3.1.6/g4f/gui/client/static/css/dracula.min.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/css/style.css` & `g4f-0.3.1.6/g4f/gui/client/static/css/style.css`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     --colour-2: #ccc;
     --colour-3: #e4d4ff;
     --colour-4: #f0f0f0;
     --colour-5: #181818;
     --colour-6: #242424;
 
     --accent: #8b3dff;
+    --gradient: var(--accent);
     --blur-bg: #16101b66;
     --blur-border: #84719040;
     --user-input: #ac87bb;
     --conversations: #c7a2ff;
     --conversations-hover: #c7a2ff4d;
 }
 
@@ -164,15 +165,15 @@
 }
 
 .gradient {
     position: absolute;
     z-index: -1;
     border-radius: calc(0.5 * var(--size));
     background-color: var(--accent);
-    background: radial-gradient(circle at center, var(--accent), var(--accent));
+    background: radial-gradient(circle at center, var(--gradient), var(--gradient));
     width: 70vw;
     height: 70vw;
     top: 50%;
     right: 0;
     transform: translateY(-50%);
     filter: blur(calc(0.5 * 70vw)) opacity(var(--opacity));
 }
@@ -374,14 +375,15 @@
 .message .user .fa-xmark {
     position: absolute;
     top: -2px;
     left: 0px;
     z-index: 1000;
     display: none;
     cursor: pointer;
+    filter: grayscale(1) invert(1);
 }
 
 .message .count .fa-clipboard,
 .message .count .fa-volume-high,
 .message .count .fa-rotate {
     z-index: 1000;
     cursor: pointer;
@@ -683,16 +685,22 @@
     min-height: 49px;
     height: 59px;
     outline: none;
     padding: var(--inner-gap) var(--section-gap);
     resize: vertical;
 }
 
-#systemPrompt {
-    padding-left: 35px;
+.slide-systemPrompt {
+    position: absolute;
+    top: 0;
+    padding: var(--inner-gap) 10px;
+    border: none;
+    background: transparent;
+    cursor: pointer;
+    height: 49px;
 }
 
 @media only screen and (min-width: 40em) {
     select {
         width: 200px;
     }
     .field {
@@ -777,15 +785,15 @@
 
 @keyframes blink {
     0% {
         background: #ffffff00;
     }
 
     50% {
-        background: white;
+        background: var(--colour-3);
     }
 
     100% {
         background: #ffffff00;
     }
 }
 
@@ -984,128 +992,21 @@
     height: 1px;
     overflow: hidden;
     position: absolute;
     white-space: nowrap;
     width: 1px;
 }
 
-.color-picker>fieldset {
-    border: 0;
-    display: flex;
-    width: fit-content;
-    background: var(--colour-1);
-    margin-inline: auto;
-    border-radius: 8px;
-    -webkit-backdrop-filter: blur(20px);
-    backdrop-filter: blur(20px);
-    cursor: pointer;
-    background-color: var(--blur-bg);
-    border: 1px solid var(--blur-border);
-    color: var(--colour-3);
-    display: block;
-    position: relative;
-    overflow: hidden;
-    outline: none;
-    padding: 6px 16px;
-}
-
-.color-picker input[type="radio"]:checked {
-    background-color: var(--radio-color);
-}
-
-.color-picker input[type="radio"]#light {
-    --radio-color: gray;
-}
-
-.color-picker input[type="radio"]#pink {
-    --radio-color: white;
-}
-
-.color-picker input[type="radio"]#blue {
-    --radio-color: blue;
-}
-
-.color-picker input[type="radio"]#green {
-    --radio-color: green;
-}
-
-.color-picker input[type="radio"]#dark {
-    --radio-color: #232323;
-}
-
-.pink {
-    --colour-1: #ffffff;
-    --colour-2: #000000;
-    --colour-3: #000000;
-    --colour-4: #000000;
-    --colour-5: #000000;
-    --colour-6: #000000;
-
-    --accent: #ffffff;
-    --blur-bg: #98989866;
-    --blur-border: #00000040;
-    --user-input: #000000;
-    --conversations: #000000;
-}
-
-.blue {
-    --colour-1: hsl(209 50% 90%);
-    --clr-card-bg: hsl(209 50% 100%);
-    --colour-3: hsl(209 50% 15%);
-    --conversations: hsl(209 50% 25%);
-}
-
-.green {
-    --colour-1: hsl(109 50% 90%);
-    --clr-card-bg: hsl(109 50% 100%);
-    --colour-3: hsl(109 50% 15%);
-    --conversations: hsl(109 50% 25%);
-}
-
-.dark {
-    --colour-1: hsl(209 50% 10%);
-    --clr-card-bg: hsl(209 50% 5%);
-    --colour-3: hsl(209 50% 90%);
-    --conversations: hsl(209 50% 80%);
-}
-
-:root:has(#pink:checked) {
+.white {
+    --blur-bg: transparent;
+    --accent: #007bff;
+    --gradient: #ccc;
+    --conversations: #0062cc;
     --colour-1: #ffffff;
-    --colour-2: #000000;
-    --colour-3: #000000;
-    --colour-4: #000000;
-    --colour-5: #000000;
-    --colour-6: #000000;
-
-    --accent: #ffffff;
-    --blur-bg: #98989866;
-    --blur-border: #00000040;
-    --user-input: #000000;
-    --conversations: #000000;
-}
-
-:root:has(#blue:checked) {
-    --colour-1: hsl(209 50% 90%);
-    --clr-card-bg: hsl(209 50% 100%);
-    --colour-3: hsl(209 50% 15%);
-    --conversations: hsl(209 50% 25%);
-}
-
-:root:has(#green:checked) {
-    --colour-1: hsl(109 50% 90%);
-    --clr-card-bg: hsl(109 50% 100%);
-    --colour-3: hsl(109 50% 15%);
-    --conversations: hsl(109 50% 25%);
-}
-
-:root:has(#dark:checked) {
-    --colour-1: hsl(209 50% 10%);
-    --clr-card-bg: hsl(209 50% 5%);
-    --colour-3: hsl(209 50% 90%);
-    --conversations: hsl(209 50% 80%);
+    --colour-3: #212529;
 }
 
 #send-button {
     border: 1px dashed #e4d4ffa6;
     border-radius: 4px;
     cursor: pointer;
     padding-left: 8px;
```

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.1.6/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.1.6/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.1.6/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.1.6/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.1.6/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/img/user.png` & `g4f-0.3.1.6/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.1.6/g4f/gui/client/static/js/chat.v1.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -299,15 +299,15 @@
         new_messages.push({
             "role": "system",
             "content": systemPrompt.value
         });
     }
     messages.forEach((new_message) => {
         // Include only not regenerated messages
-        if (!new_message.regenerate) {
+        if (new_message && !new_message.regenerate) {
             // Remove generated images from history
             new_message.content = filter_message(new_message.content);
             delete new_message.provider;
             new_messages.push(new_message)
         }
     });
     return new_messages;
@@ -1115,33 +1115,56 @@
         providerSelect.appendChild(option);
     })
 
     await load_provider_models(appStorage.getItem("provider"));
     await load_settings_storage()
 
     const hide_systemPrompt = document.getElementById("hide-systemPrompt")
+    const slide_systemPrompt_icon = document.querySelector(".slide-systemPrompt i");
     if (hide_systemPrompt.checked) {
         systemPrompt.classList.add("hidden");
+        slide_systemPrompt_icon.classList.remove("fa-angles-up");
+        slide_systemPrompt_icon.classList.add("fa-angles-down");
     }
     hide_systemPrompt.addEventListener('change', async (event) => {
         if (event.target.checked) {
             systemPrompt.classList.add("hidden");
         } else {
             systemPrompt.classList.remove("hidden");
         }
     });
+    document.querySelector(".slide-systemPrompt")?.addEventListener("click", () => {
+        hide_systemPrompt.click();
+        let checked = hide_systemPrompt.checked;
+        systemPrompt.classList[checked ? "add" : "remove"]("hidden");
+        slide_systemPrompt_icon.classList[checked ? "remove" : "add"]("fa-angles-up");
+        slide_systemPrompt_icon.classList[checked ? "add" : "remove"]("fa-angles-down");
+    });
     const messageInputHeight = document.getElementById("message-input-height");
     if (messageInputHeight) {
         if (messageInputHeight.value) {
             messageInput.style.maxHeight = `${messageInputHeight.value}px`;
         }
         messageInputHeight.addEventListener('change', async () => {
             messageInput.style.maxHeight = `${messageInputHeight.value}px`;
         });
     }
+    const darkMode = document.getElementById("darkMode");
+    if (darkMode) {
+        if (!darkMode.checked) {
+            document.body.classList.add("white");
+        }
+        darkMode.addEventListener('change', async (event) => {
+            if (event.target.checked) {
+                document.body.classList.remove("white");
+            } else {
+                document.body.classList.add("white");
+            }
+        });
+    }
 }
 
 async function load_version() {
     const versions = await api("version");
     document.title = 'g4f - ' + versions["version"];
     let text = "version ~ "
     if (versions["version"] != versions["latest_version"]) {
```

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.1.6/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.1.6/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/js/icons.js` & `g4f-0.3.1.6/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/server/android_gallery.py` & `g4f-0.3.1.6/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/server/api.py` & `g4f-0.3.1.6/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/server/backend.py` & `g4f-0.3.1.6/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/server/config.py` & `g4f-0.3.1.6/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/server/internet.py` & `g4f-0.3.1.6/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/server/js_api.py` & `g4f-0.3.1.6/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/server/website.py` & `g4f-0.3.1.6/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/gui/webview.py` & `g4f-0.3.1.6/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/image.py` & `g4f-0.3.1.6/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/local/__init__.py` & `g4f-0.3.1.6/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/locals/models.py` & `g4f-0.3.1.6/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/locals/provider.py` & `g4f-0.3.1.6/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/models.py` & `g4f-0.3.1.6/g4f/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 from __future__  import annotations
 
 from dataclasses import dataclass
 
-from .Provider import RetryProvider, ProviderType
+from .Provider import IterListProvider, ProviderType
 from .Provider import (
     Aichatos,
     Bing,
     Blackbox,
-    Chatgpt4Online,
     ChatgptAi,
     ChatgptNext,
-    Cohere,
     Cnote,
     DeepInfra,
+    DuckDuckGo,
+    Ecosia,
     Feedough,
     FreeGpt,
     Gemini,
-    GeminiProChat,
+    GeminiPro,
     GigaChat,
     HuggingChat,
     HuggingFace,
     Koala,
     Liaobots,
-    Llama,
+    MetaAI,
     OpenaiChat,
     PerplexityLabs,
     Replicate,
     Pi,
     Vercel,
     You,
     Reka
 )
 
-
 @dataclass(unsafe_hash=True)
 class Model:
     """
     Represents a machine learning model configuration.
 
     Attributes:
         name (str): Name of the model.
@@ -51,64 +50,67 @@
     def __all__() -> list[str]:
         """Returns a list of all model names."""
         return _all_models
 
 default = Model(
     name          = "",
     base_provider = "",
-    best_provider = RetryProvider([
+    best_provider = IterListProvider([
         Bing,
         ChatgptAi,
         You,
-        Chatgpt4Online,
-        OpenaiChat
+        OpenaiChat,
+        Ecosia,
     ])
 )
 
 # GPT-3.5 too, but all providers supports long requests and responses
 gpt_35_long = Model(
     name          = 'gpt-3.5-turbo',
     base_provider = 'openai',
-    best_provider = RetryProvider([
+    best_provider = IterListProvider([
         FreeGpt,
         You,
         ChatgptNext,
         OpenaiChat,
+        Koala,
+        Ecosia,
+        DuckDuckGo,
     ])
 )
 
 # GPT-3.5 / GPT-4
 gpt_35_turbo = Model(
     name          = 'gpt-3.5-turbo',
     base_provider = 'openai',
-    best_provider = RetryProvider([
+    best_provider = IterListProvider([
         FreeGpt,
         You,
         ChatgptNext,
         Koala,
         OpenaiChat,
         Aichatos,
         Cnote,
         Feedough,
     ])
 )
 
 gpt_4 = Model(
     name          = 'gpt-4',
     base_provider = 'openai',
-    best_provider = RetryProvider([
+    best_provider = IterListProvider([
         Bing, Liaobots, 
     ])
 )
 
 gpt_4o = Model(
     name          = 'gpt-4o',
     base_provider = 'openai',
-    best_provider = RetryProvider([
-        You
+    best_provider = IterListProvider([
+        You, Liaobots
     ])
 )
 
 gpt_4_turbo = Model(
     name          = 'gpt-4-turbo',
     base_provider = 'openai',
     best_provider = Bing
@@ -116,143 +118,94 @@
 
 gigachat = Model(
     name          = 'GigaChat:latest',
     base_provider = 'gigachat',
     best_provider = GigaChat
 )
 
-gigachat_plus = Model(
-    name          = 'GigaChat-Plus',
-    base_provider = 'gigachat',
-    best_provider = GigaChat
-)
-
-gigachat_pro = Model(
-    name          = 'GigaChat-Pro',
-    base_provider = 'gigachat',
-    best_provider = GigaChat
-)
-
-llama2_7b = Model(
-    name          = "meta-llama/Llama-2-7b-chat-hf",
-    base_provider = 'meta',
-    best_provider = RetryProvider([Llama, DeepInfra])
-)
-
-llama2_13b = Model(
-    name          = "meta-llama/Llama-2-13b-chat-hf",
-    base_provider = 'meta',
-    best_provider = RetryProvider([Llama, DeepInfra])
-)
-
-llama2_70b = Model(
-    name          = "meta-llama/Llama-2-70b-chat-hf",
+meta = Model(
+    name          = "meta",
     base_provider = "meta",
-    best_provider = RetryProvider([Llama, DeepInfra])
+    best_provider = MetaAI
 )
 
 llama3_8b_instruct = Model(
     name          = "meta-llama/Meta-Llama-3-8B-Instruct",
     base_provider = "meta",
-    best_provider = RetryProvider([Llama, DeepInfra, Replicate])
+    best_provider = IterListProvider([DeepInfra, PerplexityLabs, Replicate])
 )
 
 llama3_70b_instruct = Model(
     name          = "meta-llama/Meta-Llama-3-70B-Instruct",
     base_provider = "meta",
-    best_provider = RetryProvider([Llama, DeepInfra])
+    best_provider = IterListProvider([DeepInfra, PerplexityLabs, Replicate])
 )
 
 codellama_34b_instruct = Model(
     name          = "codellama/CodeLlama-34b-Instruct-hf",
     base_provider = "meta",
     best_provider = HuggingChat
 )
 
 codellama_70b_instruct = Model(
     name          = "codellama/CodeLlama-70b-Instruct-hf",
     base_provider = "meta",
-    best_provider = RetryProvider([DeepInfra, PerplexityLabs])
+    best_provider = IterListProvider([DeepInfra, PerplexityLabs])
 )
 
 # Mistral
 mixtral_8x7b = Model(
     name          = "mistralai/Mixtral-8x7B-Instruct-v0.1",
     base_provider = "huggingface",
-    best_provider = RetryProvider([DeepInfra, HuggingFace, PerplexityLabs])
+    best_provider = IterListProvider([DeepInfra, HuggingFace, PerplexityLabs])
 )
 
 mistral_7b = Model(
     name          = "mistralai/Mistral-7B-Instruct-v0.1",
     base_provider = "huggingface",
-    best_provider = RetryProvider([HuggingChat, HuggingFace, PerplexityLabs])
+    best_provider = IterListProvider([HuggingChat, HuggingFace, PerplexityLabs])
 )
 
 mistral_7b_v02 = Model(
     name          = "mistralai/Mistral-7B-Instruct-v0.2",
     base_provider = "huggingface",
-    best_provider = DeepInfra
-)
-
-mixtral_8x22b = Model(
-    name          = "HuggingFaceH4/zephyr-orpo-141b-A35b-v0.1",
-    base_provider = "huggingface",
-    best_provider = DeepInfra
-)
-
-# Misc models
-dolphin_mixtral_8x7b = Model(
-    name          = "cognitivecomputations/dolphin-2.6-mixtral-8x7b",
-    base_provider = "huggingface",
-    best_provider = DeepInfra
-)
-
-lzlv_70b = Model(
-    name          = "lizpreciatior/lzlv_70b_fp16_hf",
-    base_provider = "huggingface",
-    best_provider = DeepInfra
-)
-
-airoboros_70b = Model(
-    name          = "deepinfra/airoboros-70b",
-    base_provider = "huggingface",
-    best_provider = DeepInfra
-)
-
-openchat_35 = Model(
-    name          = "openchat/openchat_3.5",
-    base_provider = "huggingface",
-    best_provider = DeepInfra
+    best_provider = IterListProvider([DeepInfra, HuggingFace, PerplexityLabs])
 )
 
 # Bard
-gemini = bard = palm = Model(
+gemini = Model(
     name          = 'gemini',
     base_provider = 'google',
     best_provider = Gemini
 )
 
 claude_v2 = Model(
     name          = 'claude-v2',
     base_provider = 'anthropic',
-    best_provider = RetryProvider([Vercel])
+    best_provider = IterListProvider([Vercel])
 )
 
 claude_3_opus = Model(
     name          = 'claude-3-opus',
     base_provider = 'anthropic',
     best_provider = You
 )
 
 claude_3_sonnet = Model(
     name          = 'claude-3-sonnet',
     base_provider = 'anthropic',
     best_provider = You
 )
 
+claude_3_haiku = Model(
+    name          = 'claude-3-haiku',
+    base_provider = 'anthropic',
+    best_provider = DuckDuckGo
+)
+
 gpt_35_turbo_16k = Model(
     name          = 'gpt-3.5-turbo-16k',
     base_provider = 'openai',
     best_provider = gpt_35_long.best_provider
 )
 
 gpt_35_turbo_16k_0613 = Model(
@@ -284,33 +237,33 @@
     base_provider = 'openai',
     best_provider = gpt_4.best_provider
 )
 
 gemini_pro = Model(
     name          = 'gemini-pro',
     base_provider = 'google',
-    best_provider = RetryProvider([GeminiProChat, You])
+    best_provider = IterListProvider([GeminiPro, You])
 )
 
 pi = Model(
     name = 'pi',
     base_provider = 'inflection',
     best_provider = Pi
 )
 
 dbrx_instruct = Model(
     name = 'databricks/dbrx-instruct',
     base_provider = 'mistral',
-    best_provider = RetryProvider([DeepInfra, PerplexityLabs])
+    best_provider = IterListProvider([DeepInfra, PerplexityLabs])
 )
 
 command_r_plus = Model(
     name = 'CohereForAI/c4ai-command-r-plus',
     base_provider = 'mistral',
-    best_provider = RetryProvider([HuggingChat, Cohere])
+    best_provider = IterListProvider([HuggingChat])
 )
 
 blackbox = Model(
     name = 'blackbox',
     base_provider = 'blackbox',
     best_provider = Blackbox
 )
@@ -330,68 +283,53 @@
     """
     convert: dict[str, Model] = {
         # gpt-3.5
         'gpt-3.5-turbo'          : gpt_35_turbo,
         'gpt-3.5-turbo-0613'     : gpt_35_turbo_0613,
         'gpt-3.5-turbo-16k'      : gpt_35_turbo_16k,
         'gpt-3.5-turbo-16k-0613' : gpt_35_turbo_16k_0613,
-        
         'gpt-3.5-long': gpt_35_long,
-        
+
         # gpt-4
         'gpt-4o'         : gpt_4o,
         'gpt-4'          : gpt_4,
         'gpt-4-0613'     : gpt_4_0613,
         'gpt-4-32k'      : gpt_4_32k,
         'gpt-4-32k-0613' : gpt_4_32k_0613,
         'gpt-4-turbo'    : gpt_4_turbo,
 
-        # Llama
-        'llama2-7b' : llama2_7b,
-        'llama2-13b': llama2_13b,
-        'llama2-70b': llama2_70b,
-        
-        'llama3-8b' : llama3_8b_instruct, # alias
+        "meta-ai": meta,
+        'llama3-8b': llama3_8b_instruct, # alias
         'llama3-70b': llama3_70b_instruct, # alias
         'llama3-8b-instruct' : llama3_8b_instruct,
         'llama3-70b-instruct': llama3_70b_instruct,
-        
+
         'codellama-34b-instruct': codellama_34b_instruct,
         'codellama-70b-instruct': codellama_70b_instruct,
 
-        # GigaChat
-        'gigachat'     : gigachat,
-        'gigachat_plus': gigachat_plus,
-        'gigachat_pro' : gigachat_pro,
-        
         # Mistral Opensource
         'mixtral-8x7b': mixtral_8x7b,
         'mistral-7b': mistral_7b,
         'mistral-7b-v02': mistral_7b_v02,
-        'mixtral-8x22b': mixtral_8x22b,
-        'dolphin-mixtral-8x7b': dolphin_mixtral_8x7b,
-        
+
         # google gemini
         'gemini': gemini,
         'gemini-pro': gemini_pro,
-        
+
         # anthropic
         'claude-v2': claude_v2,
         'claude-3-opus': claude_3_opus,
         'claude-3-sonnet': claude_3_sonnet,
-        
+        'claude-3-haiku': claude_3_haiku,
+
         # reka core
-        'reka-core': reka_core,
         'reka': reka_core,
-        'Reka Core': reka_core,
-        
+
         # other
         'blackbox': blackbox,
         'command-r+': command_r_plus,
         'dbrx-instruct': dbrx_instruct,
-        'lzlv-70b': lzlv_70b,
-        'airoboros-70b': airoboros_70b,
-        'openchat_3.5': openchat_35,
+        'gigachat': gigachat,
         'pi': pi
     }
 
 _all_models = list(ModelUtils.convert.keys())
```

### Comparing `g4f-0.3.1.5/g4f/providers/base_provider.py` & `g4f-0.3.1.6/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/providers/create_images.py` & `g4f-0.3.1.6/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/providers/helper.py` & `g4f-0.3.1.6/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/providers/retry_provider.py` & `g4f-0.3.1.6/g4f/providers/retry_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import asyncio
 import random
 
 from ..typing import Type, List, CreateResult, Messages, Iterator, AsyncResult
-from .types import BaseProvider, BaseRetryProvider
+from .types import BaseProvider, BaseRetryProvider, ProviderType
 from .. import debug
 from ..errors import RetryProviderError, RetryNoProviderError
 
-class NewBaseRetryProvider(BaseRetryProvider):
+class IterListProvider(BaseRetryProvider):
     def __init__(
         self,
         providers: List[Type[BaseProvider]],
         shuffle: bool = True
     ) -> None:
         """
         Initialize the BaseRetryProvider.
@@ -41,29 +41,25 @@
             messages (Messages): The messages to be used for generating completion.
             stream (bool, optional): Flag to indicate if the response should be streamed. Defaults to False.
         Yields:
             CreateResult: Tokens or results from the completion.
         Raises:
             Exception: Any exception encountered during the completion process.
         """
-        providers = [p for p in self.providers if stream and p.supports_stream] if stream else self.providers
-        if self.shuffle:
-            random.shuffle(providers)
-
         exceptions = {}
         started: bool = False
 
-        for provider in providers:
+        for provider in self.get_providers(stream):
             self.last_provider = provider
             try:
                 if debug.logging:
                     print(f"Using {provider.__name__} provider")
                 for token in provider.create_completion(model, messages, stream, **kwargs):
                     yield token
-                started = True
+                    started = True
                 if started:
                     return
             except Exception as e:
                 exceptions[provider.__name__] = e
                 if debug.logging:
                     print(f"{provider.__name__}: {e.__class__.__name__}: {e}")
                 if started:
@@ -83,21 +79,17 @@
             model (str): The model to be used for completion.
             messages (Messages): The messages to be used for generating completion.
         Returns:
             str: The result of the asynchronous completion.
         Raises:
             Exception: Any exception encountered during the asynchronous completion process.
         """
-        providers = self.providers
-        if self.shuffle:
-            random.shuffle(providers)
-
         exceptions = {}
 
-        for provider in providers:
+        for provider in self.get_providers(False):
             self.last_provider = provider
             try:
                 if debug.logging:
                     print(f"Using {provider.__name__} provider")
                 return await asyncio.wait_for(
                     provider.create_async(model, messages, **kwargs),
                     timeout=kwargs.get("timeout", 60),
@@ -105,16 +97,16 @@
             except Exception as e:
                 exceptions[provider.__name__] = e
                 if debug.logging:
                     print(f"{provider.__name__}: {e.__class__.__name__}: {e}")
 
         raise_exceptions(exceptions)
 
-    def get_providers(self, stream: bool):
-        providers = [p for p in self.providers if stream and p.supports_stream] if stream else self.providers
+    def get_providers(self, stream: bool) -> list[ProviderType]:
+        providers = [p for p in self.providers if p.supports_stream] if stream else self.providers
         if self.shuffle:
             random.shuffle(providers)
         return providers
 
     async def create_async_generator(
         self,
         model: str,
@@ -134,27 +126,27 @@
                     yield await provider.create_async(model, messages, **kwargs)
                 elif hasattr(provider, "create_async_generator"):
                     async for token in provider.create_async_generator(model, messages, stream=stream, **kwargs):
                         yield token
                 else:
                     for token in provider.create_completion(model, messages, stream, **kwargs):
                         yield token
-                started = True
+                        started = True
                 if started:
                     return
             except Exception as e:
                 exceptions[provider.__name__] = e
                 if debug.logging:
                     print(f"{provider.__name__}: {e.__class__.__name__}: {e}")
                 if started:
                     raise e
 
         raise_exceptions(exceptions)
 
-class RetryProvider(NewBaseRetryProvider):
+class RetryProvider(IterListProvider):
     def __init__(
         self,
         providers: List[Type[BaseProvider]],
         shuffle: bool = True,
         single_provider_retry: bool = False,
         max_retries: int = 3,
     ) -> None:
@@ -184,27 +176,26 @@
             messages (Messages): The messages to be used for generating completion.
             stream (bool, optional): Flag to indicate if the response should be streamed. Defaults to False.
         Yields:
             CreateResult: Tokens or results from the completion.
         Raises:
             Exception: Any exception encountered during the completion process.
         """
-        providers = self.get_providers(stream)
-        if self.single_provider_retry and len(providers) == 1:
+        if self.single_provider_retry:
             exceptions = {}
             started: bool = False
-            provider = providers[0]
+            provider = self.providers[0]
             self.last_provider = provider
             for attempt in range(self.max_retries):
                 try:
                     if debug.logging:
                         print(f"Using {provider.__name__} provider (attempt {attempt + 1})")
                     for token in provider.create_completion(model, messages, stream, **kwargs):
                         yield token
-                    started = True
+                        started = True
                     if started:
                         return
                 except Exception as e:
                     exceptions[provider.__name__] = e
                     if debug.logging:
                         print(f"{provider.__name__}: {e.__class__.__name__}: {e}")
                     if started:
@@ -225,22 +216,18 @@
             model (str): The model to be used for completion.
             messages (Messages): The messages to be used for generating completion.
         Returns:
             str: The result of the asynchronous completion.
         Raises:
             Exception: Any exception encountered during the asynchronous completion process.
         """
-        providers = self.providers
-        if self.shuffle:
-            random.shuffle(providers)
-
         exceptions = {}
 
-        if self.single_provider_retry and len(providers) == 1:
-            provider = providers[0]
+        if self.single_provider_retry:
+            provider = self.providers[0]
             self.last_provider = provider
             for attempt in range(self.max_retries):
                 try:
                     if debug.logging:
                         print(f"Using {provider.__name__} provider (attempt {attempt + 1})")
                     return await asyncio.wait_for(
                         provider.create_async(model, messages, **kwargs),
```

### Comparing `g4f-0.3.1.5/g4f/providers/types.py` & `g4f-0.3.1.6/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/requests/__init__.py` & `g4f-0.3.1.6/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/requests/aiohttp.py` & `g4f-0.3.1.6/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/requests/curl_cffi.py` & `g4f-0.3.1.6/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/requests/defaults.py` & `g4f-0.3.1.6/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/requests/raise_for_status.py` & `g4f-0.3.1.6/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/stubs.py` & `g4f-0.3.1.6/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/typing.py` & `g4f-0.3.1.6/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/version.py` & `g4f-0.3.1.6/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f/webdriver.py` & `g4f-0.3.1.6/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f.egg-info/PKG-INFO` & `g4f-0.3.1.6/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.5
+Version: 0.3.1.6
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.5 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.6 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.1.5/g4f.egg-info/SOURCES.txt` & `g4f-0.3.1.6/g4f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/g4f.egg-info/requires.txt` & `g4f-0.3.1.6/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.5/setup.py` & `g4f-0.3.1.6/setup.py`

 * *Files identical despite different names*

