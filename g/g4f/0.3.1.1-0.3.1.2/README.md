# Comparing `tmp/g4f-0.3.1.1.tar.gz` & `tmp/g4f-0.3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.1.1.tar", last modified: Wed May 15 00:43:24 2024, max compression
+gzip compressed data, was "g4f-0.3.1.2.tar", last modified: Thu May 16 18:09:32 2024, max compression
```

## Comparing `g4f-0.3.1.1.tar` & `g4f-0.3.1.2.tar`

### file list

```diff
@@ -1,249 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.529514 g4f-0.3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-15 00:43:18.000000 g4f-0.3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 00:43:18.000000 g4f-0.3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55724 2024-05-15 00:43:24.529514 g4f-0.3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    52528 2024-05-15 00:43:18.000000 g4f-0.3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.489514 g4f-0.3.1.1/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.497514 g4f-0.3.1.1/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/MetaAIAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Reka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.497514 g4f-0.3.1.1/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.505514 g4f-0.3.1.1/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.505514 g4f-0.3.1.1/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.505514 g4f-0.3.1.1/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    33763 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.509514 g4f-0.3.1.1/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.509514 g4f-0.3.1.1/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.509514 g4f-0.3.1.1/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.509514 g4f-0.3.1.1/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.509514 g4f-0.3.1.1/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/openai/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/openai/proofofwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.513514 g4f-0.3.1.1/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.513514 g4f-0.3.1.1/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.513514 g4f-0.3.1.1/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.513514 g4f-0.3.1.1/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.513514 g4f-0.3.1.1/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.517514 g4f-0.3.1.1/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.517514 g4f-0.3.1.1/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.485514 g4f-0.3.1.1/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.517514 g4f-0.3.1.1/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/css/dracula.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    22924 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.517514 g4f-0.3.1.1/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.517514 g4f-0.3.1.1/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    48500 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.521514 g4f-0.3.1.1/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.521514 g4f-0.3.1.1/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.521514 g4f-0.3.1.1/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.521514 g4f-0.3.1.1/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.521514 g4f-0.3.1.1/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.525514 g4f-0.3.1.1/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-15 00:43:18.000000 g4f-0.3.1.1/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:24.525514 g4f-0.3.1.1/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55724 2024-05-15 00:43:24.000000 g4f-0.3.1.1/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-15 00:43:24.000000 g4f-0.3.1.1/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:43:24.000000 g4f-0.3.1.1/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 00:43:24.000000 g4f-0.3.1.1/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-15 00:43:24.000000 g4f-0.3.1.1/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 00:43:24.000000 g4f-0.3.1.1/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:43:24.529514 g4f-0.3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-15 00:43:18.000000 g4f-0.3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.112183 g4f-0.3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-16 18:09:21.000000 g4f-0.3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 18:09:21.000000 g4f-0.3.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-16 18:09:32.112183 g4f-0.3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    52480 2024-05-16 18:09:21.000000 g4f-0.3.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.072182 g4f-0.3.1.2/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.080182 g4f-0.3.1.2/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Reka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.080182 g4f-0.3.1.2/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.088182 g4f-0.3.1.2/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.088182 g4f-0.3.1.2/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.088182 g4f-0.3.1.2/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/PerplexityApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.092182 g4f-0.3.1.2/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.092182 g4f-0.3.1.2/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.092182 g4f-0.3.1.2/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.092182 g4f-0.3.1.2/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.092182 g4f-0.3.1.2/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/openai/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/openai/proofofwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.096182 g4f-0.3.1.2/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.096182 g4f-0.3.1.2/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.096182 g4f-0.3.1.2/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.096182 g4f-0.3.1.2/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.096182 g4f-0.3.1.2/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.100183 g4f-0.3.1.2/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.100183 g4f-0.3.1.2/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.068182 g4f-0.3.1.2/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.100183 g4f-0.3.1.2/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/css/dracula.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    22924 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.100183 g4f-0.3.1.2/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.100183 g4f-0.3.1.2/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    48500 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.104183 g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.104183 g4f-0.3.1.2/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.104183 g4f-0.3.1.2/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.104183 g4f-0.3.1.2/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.104183 g4f-0.3.1.2/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.108183 g4f-0.3.1.2/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.108183 g4f-0.3.1.2/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:09:32.112183 g4f-0.3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-16 18:09:21.000000 g4f-0.3.1.2/setup.py
```

### Comparing `g4f-0.3.1.1/LICENSE` & `g4f-0.3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/PKG-INFO` & `g4f-0.3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.1
+Version: 0.3.1.2
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -98,15 +98,15 @@
 ```
 ```sh
 docker pull hlohaus789/g4f
 ```
 
 ## 🆕 What's New
 
-- Added `gpt-4o`, simply use `gpt-4o` in `chat.completion.create`. !! NOT AVAILABLE ON PIP, DOWNLOAD REPOSITORY !!
+- Added `gpt-4o`, simply use `gpt-4o` in `chat.completion.create`.
 - Installation Guide for Windows (.exe): 💻 [#installation-guide-for-windows](#installation-guide-for-windows-exe)
 - Join our Telegram Channel: 📨 [telegram.me/g4f_channel](https://telegram.me/g4f_channel)
 - Join our Discord Group: 💬 [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5)
 - `g4f` now supports 100% local inference: 🧠 [local-docs](https://g4f.mintlify.app/docs/core/usage/local)
 
 ## 🔻 Site Takedown
 Is your site on this repository and you want to take it down? Send an email to takedown@g4f.ai with proof it is yours and it will be removed as fast as possible. To prevent reproduction please secure your API. 😉
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.1 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.2 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -57,66 +57,66 @@
 img.shields.io/pypi/v/g4f?color=blue)](https://pypi.org/project/g4f) [![Docker
 version](https://img.shields.io/docker/v/hlohaus789/
 g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/g4f) > SSttaattss::
 [![Downloads](https://static.pepy.tech/badge/g4f)](https://pepy.tech/project/
 g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)](https://
 pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
 hlohaus789/g4f ``` ## ð What's New - Added `gpt-4o`, simply use `gpt-4o` in
-`chat.completion.create`. !! NOT AVAILABLE ON PIP, DOWNLOAD REPOSITORY !! -
-Installation Guide for Windows (.exe): ð» [#installation-guide-for-windows]
-(#installation-guide-for-windows-exe) - Join our Telegram Channel: ð¨
-[telegram.me/g4f_channel](https://telegram.me/g4f_channel) - Join our Discord
-Group: ð¬ [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5) - `g4f` now
-supports 100% local inference: ð§  [local-docs](https://g4f.mintlify.app/docs/
-core/usage/local) ## ð» Site Takedown Is your site on this repository and you
-want to take it down? Send an email to takedown@g4f.ai with proof it is yours
-and it will be removed as fast as possible. To prevent reproduction please
-secure your API. ð ## ð Feedback and Todo You can always leave some
-feedback here: https://forms.gle/FeWV9RLEedfdkmFN6 As per the survey, here is a
-list of improvements to come - [x] Update the repository to include the new
-openai library syntax (ex: `Openai()` class) | completed, use
-`g4f.client.Client` - [ ] Golang implementation - [ ] ð§ Improve
-Documentation (in /docs & Guides, Howtos, & Do video tutorials) - [x] Improve
-the provider status list & updates - [ ] Tutorials on how to reverse sites to
-write your own wrapper (PoC only ofc) - [x] Improve the Bing wrapper. (Wait and
-Retry or reuse conversation) - [ ] ð§ Write a standard provider performance
-test to improve the stability - [ ] Potential support and development of local
-models - [ ] ð§ Improve compatibility and error handling ## ð Table of
-Contents - [ð What's New](#-whats-new) - [ð Table of Contents](#-table-
-of-contents) - [ð ï¸ Getting Started](#-getting-started) + [Docker Container
-Guide](#docker-container-guide) + [Installation Guide for Windows (.exe)]
-(#installation-guide-for-windows-exe) + [Use python](#use-python) -
-[Prerequisites](#prerequisites) - [Install using PyPI package:](#install-using-
-pypi-package) - [Install from source:](#install-from-source) - [Install using
-Docker:](#install-using-docker) - [ð¡ Usage](#-usage) * [Text Generation]
-(#text-generation) * [Image Generation](#image-generation) * [Web UI](#web-ui)
-* [Interference API](#interference-api) * [Configuration](#configuration) -
-[ð Providers and Models](#-providers-and-models) * [GPT-4](#gpt-4) * [GPT-
-3.5](#gpt-35) * [Other](#other) * [Models](#models) - [ð Powered by
-gpt4free](#-powered-by-gpt4free) - [ð¤ Contribute](#-contribute) + [How do i
-create a new Provider?](#guide-how-do-i-create-a-new-provider) + [How can AI
-help me with writing code?](#guide-how-can-ai-help-me-with-writing-code) -
-[ð Contributors](#-contributors) - [Â©ï¸ Copyright](#-copyright) - [â­
-Star History](#-star-history) - [ð License](#-license) ## ð ï¸ Getting
-Started #### Docker Container Guide ##### Getting Started Quickly: 1. **Install
-Docker:** Begin by [downloading and installing Docker](https://docs.docker.com/
-get-docker/). 2. **Set Up the Container:** Use the following commands to pull
-the latest image and start the container: ```sh docker pull hlohaus789/g4f
-docker run -p 8080:8080 -p 1337:1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/
-har_and_cookies:/app/har_and_cookies hlohaus789/g4f:latest ``` 3. **Access the
-Client:** - To use the included client, navigate to: [http://localhost:8080/
-chat/](http://localhost:8080/chat/) - Or set the API base for your client to:
-[http://localhost:1337/v1](http://localhost:1337/v1) 4. **(Optional) Provider
-Login:** If required, you can access the container's desktop here: http://
-localhost:7900/?autoconnect=1&resize=scale&password=secret for provider login
-purposes. #### Installation Guide for Windows (.exe) To ensure the seamless
-operation of our application, please follow the instructions below. These steps
-are designed to guide you through the installation process on Windows operating
-systems. ##### Prerequisites 1. **WebView2 Runtime**: Our application requires
-the *WebView2 Runtime* to be installed on your system. If you do not have it
+`chat.completion.create`. - Installation Guide for Windows (.exe): ð»
+[#installation-guide-for-windows](#installation-guide-for-windows-exe) - Join
+our Telegram Channel: ð¨ [telegram.me/g4f_channel](https://telegram.me/
+g4f_channel) - Join our Discord Group: ð¬ [discord.gg/XfybzPXPH5](https://
+discord.gg/XfybzPXPH5) - `g4f` now supports 100% local inference: ð§  [local-
+docs](https://g4f.mintlify.app/docs/core/usage/local) ## ð» Site Takedown Is
+your site on this repository and you want to take it down? Send an email to
+takedown@g4f.ai with proof it is yours and it will be removed as fast as
+possible. To prevent reproduction please secure your API. ð ## ð Feedback
+and Todo You can always leave some feedback here: https://forms.gle/
+FeWV9RLEedfdkmFN6 As per the survey, here is a list of improvements to come -
+[x] Update the repository to include the new openai library syntax (ex: `Openai
+()` class) | completed, use `g4f.client.Client` - [ ] Golang implementation -
+[ ] ð§ Improve Documentation (in /docs & Guides, Howtos, & Do video
+tutorials) - [x] Improve the provider status list & updates - [ ] Tutorials on
+how to reverse sites to write your own wrapper (PoC only ofc) - [x] Improve the
+Bing wrapper. (Wait and Retry or reuse conversation) - [ ] ð§ Write a
+standard provider performance test to improve the stability - [ ] Potential
+support and development of local models - [ ] ð§ Improve compatibility and
+error handling ## ð Table of Contents - [ð What's New](#-whats-new) -
+[ð Table of Contents](#-table-of-contents) - [ð ï¸ Getting Started](#-
+getting-started) + [Docker Container Guide](#docker-container-guide) +
+[Installation Guide for Windows (.exe)](#installation-guide-for-windows-exe) +
+[Use python](#use-python) - [Prerequisites](#prerequisites) - [Install using
+PyPI package:](#install-using-pypi-package) - [Install from source:](#install-
+from-source) - [Install using Docker:](#install-using-docker) - [ð¡ Usage](#-
+usage) * [Text Generation](#text-generation) * [Image Generation](#image-
+generation) * [Web UI](#web-ui) * [Interference API](#interference-api) *
+[Configuration](#configuration) - [ð Providers and Models](#-providers-and-
+models) * [GPT-4](#gpt-4) * [GPT-3.5](#gpt-35) * [Other](#other) * [Models]
+(#models) - [ð Powered by gpt4free](#-powered-by-gpt4free) - [ð¤
+Contribute](#-contribute) + [How do i create a new Provider?](#guide-how-do-i-
+create-a-new-provider) + [How can AI help me with writing code?](#guide-how-
+can-ai-help-me-with-writing-code) - [ð Contributors](#-contributors) -
+[Â©ï¸ Copyright](#-copyright) - [â­ Star History](#-star-history) - [ð
+License](#-license) ## ð ï¸ Getting Started #### Docker Container Guide
+##### Getting Started Quickly: 1. **Install Docker:** Begin by [downloading and
+installing Docker](https://docs.docker.com/get-docker/). 2. **Set Up the
+Container:** Use the following commands to pull the latest image and start the
+container: ```sh docker pull hlohaus789/g4f docker run -p 8080:8080 -p 1337:
+1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/har_and_cookies:/app/
+har_and_cookies hlohaus789/g4f:latest ``` 3. **Access the Client:** - To use
+the included client, navigate to: [http://localhost:8080/chat/](http://
+localhost:8080/chat/) - Or set the API base for your client to: [http://
+localhost:1337/v1](http://localhost:1337/v1) 4. **(Optional) Provider Login:**
+If required, you can access the container's desktop here: http://localhost:
+7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
+#### Installation Guide for Windows (.exe) To ensure the seamless operation of
+our application, please follow the instructions below. These steps are designed
+to guide you through the installation process on Windows operating systems.
+##### Prerequisites 1. **WebView2 Runtime**: Our application requires the
+*WebView2 Runtime* to be installed on your system. If you do not have it
 installed, please download and install it from the [Microsoft Developer
 Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If
 you already have *WebView2 Runtime* installed but are encountering issues,
 navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair
 option. ##### Installation Steps 2. **Download the Application**: Visit our
 [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and
 download the most recent version of the application, named `g4f.webview.*.exe`.
```

### Comparing `g4f-0.3.1.1/README.md` & `g4f-0.3.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ```
 ```sh
 docker pull hlohaus789/g4f
 ```
 
 ## 🆕 What's New
 
-- Added `gpt-4o`, simply use `gpt-4o` in `chat.completion.create`. !! NOT AVAILABLE ON PIP, DOWNLOAD REPOSITORY !!
+- Added `gpt-4o`, simply use `gpt-4o` in `chat.completion.create`.
 - Installation Guide for Windows (.exe): 💻 [#installation-guide-for-windows](#installation-guide-for-windows-exe)
 - Join our Telegram Channel: 📨 [telegram.me/g4f_channel](https://telegram.me/g4f_channel)
 - Join our Discord Group: 💬 [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5)
 - `g4f` now supports 100% local inference: 🧠 [local-docs](https://g4f.mintlify.app/docs/core/usage/local)
 
 ## 🔻 Site Takedown
 Is your site on this repository and you want to take it down? Send an email to takedown@g4f.ai with proof it is yours and it will be removed as fast as possible. To prevent reproduction please secure your API. 😉
```

#### html2text {}

```diff
@@ -15,66 +15,66 @@
 img.shields.io/pypi/v/g4f?color=blue)](https://pypi.org/project/g4f) [![Docker
 version](https://img.shields.io/docker/v/hlohaus789/
 g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/g4f) > SSttaattss::
 [![Downloads](https://static.pepy.tech/badge/g4f)](https://pepy.tech/project/
 g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)](https://
 pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
 hlohaus789/g4f ``` ## ð What's New - Added `gpt-4o`, simply use `gpt-4o` in
-`chat.completion.create`. !! NOT AVAILABLE ON PIP, DOWNLOAD REPOSITORY !! -
-Installation Guide for Windows (.exe): ð» [#installation-guide-for-windows]
-(#installation-guide-for-windows-exe) - Join our Telegram Channel: ð¨
-[telegram.me/g4f_channel](https://telegram.me/g4f_channel) - Join our Discord
-Group: ð¬ [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5) - `g4f` now
-supports 100% local inference: ð§  [local-docs](https://g4f.mintlify.app/docs/
-core/usage/local) ## ð» Site Takedown Is your site on this repository and you
-want to take it down? Send an email to takedown@g4f.ai with proof it is yours
-and it will be removed as fast as possible. To prevent reproduction please
-secure your API. ð ## ð Feedback and Todo You can always leave some
-feedback here: https://forms.gle/FeWV9RLEedfdkmFN6 As per the survey, here is a
-list of improvements to come - [x] Update the repository to include the new
-openai library syntax (ex: `Openai()` class) | completed, use
-`g4f.client.Client` - [ ] Golang implementation - [ ] ð§ Improve
-Documentation (in /docs & Guides, Howtos, & Do video tutorials) - [x] Improve
-the provider status list & updates - [ ] Tutorials on how to reverse sites to
-write your own wrapper (PoC only ofc) - [x] Improve the Bing wrapper. (Wait and
-Retry or reuse conversation) - [ ] ð§ Write a standard provider performance
-test to improve the stability - [ ] Potential support and development of local
-models - [ ] ð§ Improve compatibility and error handling ## ð Table of
-Contents - [ð What's New](#-whats-new) - [ð Table of Contents](#-table-
-of-contents) - [ð ï¸ Getting Started](#-getting-started) + [Docker Container
-Guide](#docker-container-guide) + [Installation Guide for Windows (.exe)]
-(#installation-guide-for-windows-exe) + [Use python](#use-python) -
-[Prerequisites](#prerequisites) - [Install using PyPI package:](#install-using-
-pypi-package) - [Install from source:](#install-from-source) - [Install using
-Docker:](#install-using-docker) - [ð¡ Usage](#-usage) * [Text Generation]
-(#text-generation) * [Image Generation](#image-generation) * [Web UI](#web-ui)
-* [Interference API](#interference-api) * [Configuration](#configuration) -
-[ð Providers and Models](#-providers-and-models) * [GPT-4](#gpt-4) * [GPT-
-3.5](#gpt-35) * [Other](#other) * [Models](#models) - [ð Powered by
-gpt4free](#-powered-by-gpt4free) - [ð¤ Contribute](#-contribute) + [How do i
-create a new Provider?](#guide-how-do-i-create-a-new-provider) + [How can AI
-help me with writing code?](#guide-how-can-ai-help-me-with-writing-code) -
-[ð Contributors](#-contributors) - [Â©ï¸ Copyright](#-copyright) - [â­
-Star History](#-star-history) - [ð License](#-license) ## ð ï¸ Getting
-Started #### Docker Container Guide ##### Getting Started Quickly: 1. **Install
-Docker:** Begin by [downloading and installing Docker](https://docs.docker.com/
-get-docker/). 2. **Set Up the Container:** Use the following commands to pull
-the latest image and start the container: ```sh docker pull hlohaus789/g4f
-docker run -p 8080:8080 -p 1337:1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/
-har_and_cookies:/app/har_and_cookies hlohaus789/g4f:latest ``` 3. **Access the
-Client:** - To use the included client, navigate to: [http://localhost:8080/
-chat/](http://localhost:8080/chat/) - Or set the API base for your client to:
-[http://localhost:1337/v1](http://localhost:1337/v1) 4. **(Optional) Provider
-Login:** If required, you can access the container's desktop here: http://
-localhost:7900/?autoconnect=1&resize=scale&password=secret for provider login
-purposes. #### Installation Guide for Windows (.exe) To ensure the seamless
-operation of our application, please follow the instructions below. These steps
-are designed to guide you through the installation process on Windows operating
-systems. ##### Prerequisites 1. **WebView2 Runtime**: Our application requires
-the *WebView2 Runtime* to be installed on your system. If you do not have it
+`chat.completion.create`. - Installation Guide for Windows (.exe): ð»
+[#installation-guide-for-windows](#installation-guide-for-windows-exe) - Join
+our Telegram Channel: ð¨ [telegram.me/g4f_channel](https://telegram.me/
+g4f_channel) - Join our Discord Group: ð¬ [discord.gg/XfybzPXPH5](https://
+discord.gg/XfybzPXPH5) - `g4f` now supports 100% local inference: ð§  [local-
+docs](https://g4f.mintlify.app/docs/core/usage/local) ## ð» Site Takedown Is
+your site on this repository and you want to take it down? Send an email to
+takedown@g4f.ai with proof it is yours and it will be removed as fast as
+possible. To prevent reproduction please secure your API. ð ## ð Feedback
+and Todo You can always leave some feedback here: https://forms.gle/
+FeWV9RLEedfdkmFN6 As per the survey, here is a list of improvements to come -
+[x] Update the repository to include the new openai library syntax (ex: `Openai
+()` class) | completed, use `g4f.client.Client` - [ ] Golang implementation -
+[ ] ð§ Improve Documentation (in /docs & Guides, Howtos, & Do video
+tutorials) - [x] Improve the provider status list & updates - [ ] Tutorials on
+how to reverse sites to write your own wrapper (PoC only ofc) - [x] Improve the
+Bing wrapper. (Wait and Retry or reuse conversation) - [ ] ð§ Write a
+standard provider performance test to improve the stability - [ ] Potential
+support and development of local models - [ ] ð§ Improve compatibility and
+error handling ## ð Table of Contents - [ð What's New](#-whats-new) -
+[ð Table of Contents](#-table-of-contents) - [ð ï¸ Getting Started](#-
+getting-started) + [Docker Container Guide](#docker-container-guide) +
+[Installation Guide for Windows (.exe)](#installation-guide-for-windows-exe) +
+[Use python](#use-python) - [Prerequisites](#prerequisites) - [Install using
+PyPI package:](#install-using-pypi-package) - [Install from source:](#install-
+from-source) - [Install using Docker:](#install-using-docker) - [ð¡ Usage](#-
+usage) * [Text Generation](#text-generation) * [Image Generation](#image-
+generation) * [Web UI](#web-ui) * [Interference API](#interference-api) *
+[Configuration](#configuration) - [ð Providers and Models](#-providers-and-
+models) * [GPT-4](#gpt-4) * [GPT-3.5](#gpt-35) * [Other](#other) * [Models]
+(#models) - [ð Powered by gpt4free](#-powered-by-gpt4free) - [ð¤
+Contribute](#-contribute) + [How do i create a new Provider?](#guide-how-do-i-
+create-a-new-provider) + [How can AI help me with writing code?](#guide-how-
+can-ai-help-me-with-writing-code) - [ð Contributors](#-contributors) -
+[Â©ï¸ Copyright](#-copyright) - [â­ Star History](#-star-history) - [ð
+License](#-license) ## ð ï¸ Getting Started #### Docker Container Guide
+##### Getting Started Quickly: 1. **Install Docker:** Begin by [downloading and
+installing Docker](https://docs.docker.com/get-docker/). 2. **Set Up the
+Container:** Use the following commands to pull the latest image and start the
+container: ```sh docker pull hlohaus789/g4f docker run -p 8080:8080 -p 1337:
+1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/har_and_cookies:/app/
+har_and_cookies hlohaus789/g4f:latest ``` 3. **Access the Client:** - To use
+the included client, navigate to: [http://localhost:8080/chat/](http://
+localhost:8080/chat/) - Or set the API base for your client to: [http://
+localhost:1337/v1](http://localhost:1337/v1) 4. **(Optional) Provider Login:**
+If required, you can access the container's desktop here: http://localhost:
+7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
+#### Installation Guide for Windows (.exe) To ensure the seamless operation of
+our application, please follow the instructions below. These steps are designed
+to guide you through the installation process on Windows operating systems.
+##### Prerequisites 1. **WebView2 Runtime**: Our application requires the
+*WebView2 Runtime* to be installed on your system. If you do not have it
 installed, please download and install it from the [Microsoft Developer
 Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If
 you already have *WebView2 Runtime* installed but are encountering issues,
 navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair
 option. ##### Installation Steps 2. **Download the Application**: Visit our
 [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and
 download the most recent version of the application, named `g4f.webview.*.exe`.
```

### Comparing `g4f-0.3.1.1/g4f/Provider/Aichatos.py` & `g4f-0.3.1.2/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Aura.py` & `g4f-0.3.1.2/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Bing.py` & `g4f-0.3.1.2/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/BingCreateImages.py` & `g4f-0.3.1.2/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Blackbox.py` & `g4f-0.3.1.2/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/ChatForAi.py` & `g4f-0.3.1.2/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.1.2/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/ChatgptAi.py` & `g4f-0.3.1.2/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/ChatgptFree.py` & `g4f-0.3.1.2/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/ChatgptNext.py` & `g4f-0.3.1.2/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/ChatgptX.py` & `g4f-0.3.1.2/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Cnote.py` & `g4f-0.3.1.2/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Cohere.py` & `g4f-0.3.1.2/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/DeepInfra.py` & `g4f-0.3.1.2/g4f/Provider/DeepInfra.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from ..typing import AsyncResult, Messages
 from .needs_auth.Openai import Openai
 
 class DeepInfra(Openai):
     label = "DeepInfra"
     url = "https://deepinfra.com"
     working = True
-    needs_auth = False
-    has_auth = True
+    needs_auth = True
     supports_stream = True
     supports_message_history = True
     default_model = "meta-llama/Meta-Llama-3-70b-instruct"
     default_vision_model = "llava-hf/llava-1.5-7b-hf"
     model_aliases = {
         'dbrx-instruct': 'databricks/dbrx-instruct',
     }
```

### Comparing `g4f-0.3.1.1/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.1.2/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.1.2/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Ecosia.py` & `g4f-0.3.1.2/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Feedough.py` & `g4f-0.3.1.2/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/FlowGpt.py` & `g4f-0.3.1.2/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.1.2/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/FreeGpt.py` & `g4f-0.3.1.2/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/GeminiPro.py` & `g4f-0.3.1.2/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/GeminiProChat.py` & `g4f-0.3.1.2/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/GigaChat.py` & `g4f-0.3.1.2/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/GptTalkRu.py` & `g4f-0.3.1.2/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/HuggingChat.py` & `g4f-0.3.1.2/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/HuggingFace.py` & `g4f-0.3.1.2/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Koala.py` & `g4f-0.3.1.2/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Liaobots.py` & `g4f-0.3.1.2/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Llama.py` & `g4f-0.3.1.2/g4f/Provider/Llama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Local.py` & `g4f-0.3.1.2/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/MetaAI.py` & `g4f-0.3.1.2/g4f/Provider/MetaAI.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/MetaAIAccount.py` & `g4f-0.3.1.2/g4f/Provider/MetaAIAccount.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Ollama.py` & `g4f-0.3.1.2/g4f/Provider/Ollama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.1.2/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Pi.py` & `g4f-0.3.1.2/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Reka.py` & `g4f-0.3.1.2/g4f/Provider/Reka.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,52 +5,52 @@
 from .base_provider import AbstractProvider
 from ..cookies      import get_cookies
 from ..image        import to_bytes
 
 class Reka(AbstractProvider):
     url             = "https://chat.reka.ai/"
     working         = True
+    needs_auth      = True
     supports_stream = True
     default_vision_model = "reka"
     cookies         = {}
 
     @classmethod
     def create_completion(
         cls,
         model: str,
         messages: Messages,
         stream: bool,
         proxy: str = None,
-        timeout: int = 180,
         api_key: str = None,
         image: ImageType = None,
         **kwargs
     ) -> CreateResult:
         cls.proxy = proxy
-        
+
         if not api_key:
             cls.cookies = get_cookies("chat.reka.ai")
             if not cls.cookies:
                 raise ValueError("No cookies found for chat.reka.ai")
             elif "appSession" not in cls.cookies:
                 raise ValueError("No appSession found in cookies for chat.reka.ai, log in or provide bearer_auth")
             api_key = cls.get_access_token(cls)
-            
+
         conversation = []
         for message in messages:
             conversation.append({
                 "type": "human",
                 "text": message["content"],
             })
-        
+
         if image:
             image_url = cls.upload_image(cls, api_key, image)
             conversation[-1]["image_url"] = image_url
             conversation[-1]["media_type"] = "image"
-        
+
         headers = {
             'accept': '*/*',
             'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
             'authorization': f'Bearer {api_key}',
             'cache-control': 'no-cache',
             'content-type': 'application/json',
             'origin': 'https://chat.reka.ai',
@@ -60,37 +60,37 @@
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"macOS"',
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-origin',
             'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36',
         }
-        
+
         json_data = {
             'conversation_history': conversation,
             'stream': True,
             'use_search_engine': False,
             'use_code_interpreter': False,
             'model_name': 'reka-core',
             'random_seed': int(time.time() * 1000),
         }
-        
+
         tokens = ''
 
         response = requests.post('https://chat.reka.ai/api/chat', 
                                 cookies=cls.cookies, headers=headers, json=json_data, proxies=cls.proxy, stream=True)
 
         for completion in response.iter_lines():
             if b'data' in completion:
                 token_data = json.loads(completion.decode('utf-8')[5:])['text']
-                
+
                 yield (token_data.replace(tokens, ''))
-                
+
                 tokens = token_data
-    
+
     def upload_image(cls, access_token, image: ImageType) -> str:
         boundary_token = os.urandom(8).hex()
 
         headers = {
             'accept': '*/*',
             'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
             'cache-control': 'no-cache',
@@ -116,15 +116,15 @@
         data += image_data.decode('latin-1')
         data += f'\r\n--{boundary}--\r\n'
 
         response = requests.post('https://chat.reka.ai/api/upload-image', 
                                     cookies=cls.cookies, headers=headers, proxies=cls.proxy, data=data.encode('latin-1'))
 
         return response.json()['media_url']
-    
+
     def get_access_token(cls):
         headers = {
             'accept': '*/*',
             'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
             'cache-control': 'no-cache',
             'pragma': 'no-cache',
             'priority': 'u=1, i',
@@ -137,12 +137,12 @@
             'sec-fetch-site': 'same-origin',
             'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36',
         }
 
         try:
             response = requests.get('https://chat.reka.ai/bff/auth/access_token', 
                                     cookies=cls.cookies, headers=headers, proxies=cls.proxy)
-            
+
             return response.json()['accessToken']
-        
+
         except Exception as e:
             raise ValueError(f"Failed to get access token: {e}, refresh your cookies / log in into chat.reka.ai")
```

### Comparing `g4f-0.3.1.1/g4f/Provider/Replicate.py` & `g4f-0.3.1.2/g4f/Provider/Replicate.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ..requests import raise_for_status
 from ..requests.aiohttp import StreamSession
 from ..errors import ResponseError, MissingAuthError
 
 class Replicate(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://replicate.com"
     working = True
+    needs_auth = True
     default_model = "meta/meta-llama-3-70b-instruct"
     model_aliases = {
         "meta-llama/Meta-Llama-3-70B-Instruct": default_model
     }
 
     @classmethod
     async def create_async_generator(
```

### Comparing `g4f-0.3.1.1/g4f/Provider/ReplicateImage.py` & `g4f-0.3.1.2/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/Vercel.py` & `g4f-0.3.1.2/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.1.2/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/You.py` & `g4f-0.3.1.2/g4f/Provider/You.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 import json
 import base64
 import uuid
 
 from ..typing import AsyncResult, Messages, ImageType, Cookies
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
@@ -38,15 +40,14 @@
         "llama3",
         "zephyr",
         default_vision_model,
         *image_models
     ]
     model_aliases = {
         "claude-v2": "claude-2",
-        "gpt-4o": "gpt-4o",
     }
     _cookies = None
     _cookies_used = 0
     _telemetry_ids = []
 
     @classmethod
     async def create_async_generator(
@@ -181,23 +182,15 @@
         auth_token = f"public-token-live-{auth_uuid}:public-token-live-{auth_uuid}"
         auth = base64.standard_b64encode(auth_token.encode()).decode()
         return f"Basic {auth}"
 
     @classmethod
     async def create_cookies(cls, client: StreamSession) -> Cookies:
         if not cls._telemetry_ids:
-            try:
-                cls._telemetry_ids = await get_telemetry_ids()
-            except RuntimeError as e:
-                if str(e) == "Event loop is closed":
-                    if debug.logging:
-                        print("Event loop is closed error occurred in create_cookies.")
-                else:
-                    raise
-                
+            cls._telemetry_ids = await get_telemetry_ids()
         user_uuid = str(uuid.uuid4())
         telemetry_id = cls._telemetry_ids.pop()
         if debug.logging:
             print(f"Use telemetry_id: {telemetry_id}")
         async with client.post(
             "https://web.stytch.com/sdk/v1/passwords",
             headers={
```

### Comparing `g4f-0.3.1.1/g4f/Provider/__init__.py` & `g4f-0.3.1.2/g4f/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/bing/conversation.py` & `g4f-0.3.1.2/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/bing/create_images.py` & `g4f-0.3.1.2/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/bing/upload_image.py` & `g4f-0.3.1.2/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/V50.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.1.2/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.1.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.1.2/g4f/Provider/needs_auth/Gemini.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,27 +55,30 @@
     needs_auth = True
     working = True
     image_models = ["gemini"]
     default_vision_model = "gemini"
     _cookies: Cookies = None
 
     @classmethod
-    async def nodriver_login(cls) -> AsyncIterator[str]:
+    async def nodriver_login(cls, proxy: str = None) -> AsyncIterator[str]:
         try:
             import nodriver as uc
         except ImportError:
             return
         try:
             from platformdirs import user_config_dir
             user_data_dir = user_config_dir("g4f-nodriver")
         except:
             user_data_dir = None
         if debug.logging:
             print(f"Open nodriver with user_dir: {user_data_dir}")
-        browser = await uc.start(user_data_dir=user_data_dir)
+        browser = await uc.start(
+            user_data_dir=user_data_dir,
+            browser_args=None if proxy is None else [f"--proxy-server={proxy}"],
+        )
         login_url = os.environ.get("G4F_LOGIN_URL")
         if login_url:
             yield f"Please login: [Google Gemini]({login_url})\n\n"
         page = await browser.get(f"{cls.url}/app")
         await page.select("div.ql-editor.textarea", 240)
         cookies = {}
         for c in await page.browser.cookies.get_all():
@@ -130,15 +133,15 @@
         base_connector = get_connector(connector, proxy)
         async with ClientSession(
             headers=REQUEST_HEADERS,
             connector=base_connector
         ) as session:
             snlm0e  = await cls.fetch_snlm0e(session, cls._cookies) if cls._cookies else None
             if not snlm0e:
-                async for chunk in cls.nodriver_login():
+                async for chunk in cls.nodriver_login(proxy):
                     yield chunk
                 if cls._cookies is None:
                     async for chunk in cls.webdriver_login(proxy):
                         yield chunk
 
             if not snlm0e:
                 if cls._cookies is None or "__Secure-1PSID" not in cls._cookies:
```

### Comparing `g4f-0.3.1.1/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.1.2/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.1.2/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.1.2/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.1.2/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,15 +399,15 @@
                 try:
                     arkose_token, api_key, cookies, headers = await getArkoseAndAccessToken(proxy)
                     cls._create_request_args(cookies, headers)
                     cls._set_api_key(api_key)
                 except NoValidHarFileError as e:
                     error = e
                 if cls._api_key is None:
-                    await cls.nodriver_access_token()
+                    await cls.nodriver_access_token(proxy)
                 if cls._api_key is None and cls.needs_auth:
                     raise error
                 cls.default_model = cls.get_model(await cls.get_default_model(session, cls._headers))
 
             async with session.post(
                 f"{cls.url}/backend-anon/sentinel/chat-requirements"
                 if cls._api_key is None else
@@ -621,27 +621,30 @@
         window.destroy()
         cls._cookies = dict([(name, cookie.value) for name, cookie in cookies])
         cls._headers = headers
         cls._expires = int(time.time()) + 60 * 60 * 4
         cls._update_cookie_header()
 
     @classmethod
-    async def nodriver_access_token(cls):
+    async def nodriver_access_token(cls, proxy: str = None):
         try:
             import nodriver as uc
         except ImportError:
             return
         try:
             from platformdirs import user_config_dir
             user_data_dir = user_config_dir("g4f-nodriver")
         except:
             user_data_dir = None
         if debug.logging:
             print(f"Open nodriver with user_dir: {user_data_dir}")
-        browser = await uc.start(user_data_dir=user_data_dir)
+        browser = await uc.start(
+            user_data_dir=user_data_dir,
+            browser_args=None if proxy is None else [f"--proxy-server={proxy}"],
+        )
         page = await browser.get("https://chatgpt.com/")
         await page.select("[id^=headlessui-menu-button-]", 240)
         api_key = await page.evaluate(
             "(async () => {"
             "let session = await fetch('/api/auth/session');"
             "let data = await session.json();"
             "let accessToken = data['accessToken'];"
```

### Comparing `g4f-0.3.1.1/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.1.2/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.1.2/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.1.2/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.1.2/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.1.2/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.1.2/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.1.2/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.1.2/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.1.2/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.1.2/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.1.2/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.1.2/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.1.2/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.1.2/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.1.2/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.1.2/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.1.2/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.1.2/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.1.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/npm/package-lock.json` & `g4f-0.3.1.2/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/openai/crypt.py` & `g4f-0.3.1.2/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/openai/har_file.py` & `g4f-0.3.1.2/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/openai/proofofwork.py` & `g4f-0.3.1.2/g4f/Provider/openai/proofofwork.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.1.2/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/selenium/Bard.py` & `g4f-0.3.1.2/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.1.2/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.1.2/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/selenium/Phind.py` & `g4f-0.3.1.2/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.1.2/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.1.2/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.1.2/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.1.2/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.1.2/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/Provider/you/har_file.py` & `g4f-0.3.1.2/g4f/Provider/you/har_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,40 +84,38 @@
 
 async def get_telemetry_ids(proxy: str = None) -> list:
     try:
         return [await create_telemetry_id(proxy)]
     except NoValidHarFileError as e:
         if debug.logging:
             logging.error(e)
-    if debug.logging:
-        logging.error('Getting telemetry_id for you.com with nodriver')
+
     try:
         from nodriver import start
     except ImportError:
         raise MissingRequirementsError('Add .har file from you.com or install "nodriver" package | pip install -U nodriver')
-    page = None
+    if debug.logging:
+        logging.error('Getting telemetry_id for you.com with nodriver')
+
+    browser = page = None
     try:
-        browser = await start()
+        browser = await start(
+            browser_args=None if proxy is None else [f"--proxy-server={proxy}"],
+        )
         page = await browser.get("https://you.com")
-
         while not await page.evaluate('"GetTelemetryID" in this'):
             await page.sleep(1)
-
         async def get_telemetry_id():
             return await page.evaluate(
                 f'this.GetTelemetryID("{public_token}", "{telemetry_url}");',
                 await_promise=True
             )
-
         return [await get_telemetry_id()]
-    
     finally:
         try:
             if page is not None:
                 await page.close()
-                
             if browser is not None:
                 await browser.close()
-        
         except Exception as e:
             if debug.logging:
                 logging.error(e)
```

### Comparing `g4f-0.3.1.1/g4f/__init__.py` & `g4f-0.3.1.2/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/api/__init__.py` & `g4f-0.3.1.2/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/api/_logging.py` & `g4f-0.3.1.2/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/cli.py` & `g4f-0.3.1.2/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/client/async_client.py` & `g4f-0.3.1.2/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/client/client.py` & `g4f-0.3.1.2/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/client/helper.py` & `g4f-0.3.1.2/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/client/image_models.py` & `g4f-0.3.1.2/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/client/service.py` & `g4f-0.3.1.2/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/client/stubs.py` & `g4f-0.3.1.2/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/client/types.py` & `g4f-0.3.1.2/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/cookies.py` & `g4f-0.3.1.2/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/errors.py` & `g4f-0.3.1.2/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/__init__.py` & `g4f-0.3.1.2/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/index.html` & `g4f-0.3.1.2/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/css/dracula.min.css` & `g4f-0.3.1.2/g4f/gui/client/static/css/dracula.min.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/css/style.css` & `g4f-0.3.1.2/g4f/gui/client/static/css/style.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.1.2/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.1.2/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.1.2/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.1.2/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.1.2/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/img/user.png` & `g4f-0.3.1.2/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.1.2/g4f/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.1.2/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.1.2/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/js/icons.js` & `g4f-0.3.1.2/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/server/android_gallery.py` & `g4f-0.3.1.2/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/server/api.py` & `g4f-0.3.1.2/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/server/backend.py` & `g4f-0.3.1.2/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/server/config.py` & `g4f-0.3.1.2/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/server/internet.py` & `g4f-0.3.1.2/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/server/js_api.py` & `g4f-0.3.1.2/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/server/website.py` & `g4f-0.3.1.2/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/gui/webview.py` & `g4f-0.3.1.2/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/image.py` & `g4f-0.3.1.2/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/local/__init__.py` & `g4f-0.3.1.2/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/locals/models.py` & `g4f-0.3.1.2/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/locals/provider.py` & `g4f-0.3.1.2/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/models.py` & `g4f-0.3.1.2/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/providers/base_provider.py` & `g4f-0.3.1.2/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/providers/create_images.py` & `g4f-0.3.1.2/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/providers/helper.py` & `g4f-0.3.1.2/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/providers/retry_provider.py` & `g4f-0.3.1.2/g4f/providers/retry_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             self.last_provider = provider
             try:
                 if debug.logging:
                     print(f"Using {provider.__name__} provider")
                 if not stream:
                     yield await provider.create_async(model, messages, **kwargs)
                 elif hasattr(provider, "create_async_generator"):
-                    async for token in provider.create_async_generator(model, messages, stream, **kwargs):
+                    async for token in provider.create_async_generator(model, messages, stream=stream, **kwargs):
                         yield token
                 else:
                     for token in provider.create_completion(model, messages, stream, **kwargs):
                         yield token
                 started = True
                 if started:
                     return
```

### Comparing `g4f-0.3.1.1/g4f/providers/types.py` & `g4f-0.3.1.2/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/requests/__init__.py` & `g4f-0.3.1.2/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/requests/aiohttp.py` & `g4f-0.3.1.2/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/requests/curl_cffi.py` & `g4f-0.3.1.2/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/requests/defaults.py` & `g4f-0.3.1.2/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/requests/raise_for_status.py` & `g4f-0.3.1.2/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/stubs.py` & `g4f-0.3.1.2/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/typing.py` & `g4f-0.3.1.2/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/version.py` & `g4f-0.3.1.2/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f/webdriver.py` & `g4f-0.3.1.2/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/g4f.egg-info/PKG-INFO` & `g4f-0.3.1.2/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.1
+Version: 0.3.1.2
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -98,15 +98,15 @@
 ```
 ```sh
 docker pull hlohaus789/g4f
 ```
 
 ## 🆕 What's New
 
-- Added `gpt-4o`, simply use `gpt-4o` in `chat.completion.create`. !! NOT AVAILABLE ON PIP, DOWNLOAD REPOSITORY !!
+- Added `gpt-4o`, simply use `gpt-4o` in `chat.completion.create`.
 - Installation Guide for Windows (.exe): 💻 [#installation-guide-for-windows](#installation-guide-for-windows-exe)
 - Join our Telegram Channel: 📨 [telegram.me/g4f_channel](https://telegram.me/g4f_channel)
 - Join our Discord Group: 💬 [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5)
 - `g4f` now supports 100% local inference: 🧠 [local-docs](https://g4f.mintlify.app/docs/core/usage/local)
 
 ## 🔻 Site Takedown
 Is your site on this repository and you want to take it down? Send an email to takedown@g4f.ai with proof it is yours and it will be removed as fast as possible. To prevent reproduction please secure your API. 😉
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.1 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.2 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -57,66 +57,66 @@
 img.shields.io/pypi/v/g4f?color=blue)](https://pypi.org/project/g4f) [![Docker
 version](https://img.shields.io/docker/v/hlohaus789/
 g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/g4f) > SSttaattss::
 [![Downloads](https://static.pepy.tech/badge/g4f)](https://pepy.tech/project/
 g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)](https://
 pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
 hlohaus789/g4f ``` ## ð What's New - Added `gpt-4o`, simply use `gpt-4o` in
-`chat.completion.create`. !! NOT AVAILABLE ON PIP, DOWNLOAD REPOSITORY !! -
-Installation Guide for Windows (.exe): ð» [#installation-guide-for-windows]
-(#installation-guide-for-windows-exe) - Join our Telegram Channel: ð¨
-[telegram.me/g4f_channel](https://telegram.me/g4f_channel) - Join our Discord
-Group: ð¬ [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5) - `g4f` now
-supports 100% local inference: ð§  [local-docs](https://g4f.mintlify.app/docs/
-core/usage/local) ## ð» Site Takedown Is your site on this repository and you
-want to take it down? Send an email to takedown@g4f.ai with proof it is yours
-and it will be removed as fast as possible. To prevent reproduction please
-secure your API. ð ## ð Feedback and Todo You can always leave some
-feedback here: https://forms.gle/FeWV9RLEedfdkmFN6 As per the survey, here is a
-list of improvements to come - [x] Update the repository to include the new
-openai library syntax (ex: `Openai()` class) | completed, use
-`g4f.client.Client` - [ ] Golang implementation - [ ] ð§ Improve
-Documentation (in /docs & Guides, Howtos, & Do video tutorials) - [x] Improve
-the provider status list & updates - [ ] Tutorials on how to reverse sites to
-write your own wrapper (PoC only ofc) - [x] Improve the Bing wrapper. (Wait and
-Retry or reuse conversation) - [ ] ð§ Write a standard provider performance
-test to improve the stability - [ ] Potential support and development of local
-models - [ ] ð§ Improve compatibility and error handling ## ð Table of
-Contents - [ð What's New](#-whats-new) - [ð Table of Contents](#-table-
-of-contents) - [ð ï¸ Getting Started](#-getting-started) + [Docker Container
-Guide](#docker-container-guide) + [Installation Guide for Windows (.exe)]
-(#installation-guide-for-windows-exe) + [Use python](#use-python) -
-[Prerequisites](#prerequisites) - [Install using PyPI package:](#install-using-
-pypi-package) - [Install from source:](#install-from-source) - [Install using
-Docker:](#install-using-docker) - [ð¡ Usage](#-usage) * [Text Generation]
-(#text-generation) * [Image Generation](#image-generation) * [Web UI](#web-ui)
-* [Interference API](#interference-api) * [Configuration](#configuration) -
-[ð Providers and Models](#-providers-and-models) * [GPT-4](#gpt-4) * [GPT-
-3.5](#gpt-35) * [Other](#other) * [Models](#models) - [ð Powered by
-gpt4free](#-powered-by-gpt4free) - [ð¤ Contribute](#-contribute) + [How do i
-create a new Provider?](#guide-how-do-i-create-a-new-provider) + [How can AI
-help me with writing code?](#guide-how-can-ai-help-me-with-writing-code) -
-[ð Contributors](#-contributors) - [Â©ï¸ Copyright](#-copyright) - [â­
-Star History](#-star-history) - [ð License](#-license) ## ð ï¸ Getting
-Started #### Docker Container Guide ##### Getting Started Quickly: 1. **Install
-Docker:** Begin by [downloading and installing Docker](https://docs.docker.com/
-get-docker/). 2. **Set Up the Container:** Use the following commands to pull
-the latest image and start the container: ```sh docker pull hlohaus789/g4f
-docker run -p 8080:8080 -p 1337:1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/
-har_and_cookies:/app/har_and_cookies hlohaus789/g4f:latest ``` 3. **Access the
-Client:** - To use the included client, navigate to: [http://localhost:8080/
-chat/](http://localhost:8080/chat/) - Or set the API base for your client to:
-[http://localhost:1337/v1](http://localhost:1337/v1) 4. **(Optional) Provider
-Login:** If required, you can access the container's desktop here: http://
-localhost:7900/?autoconnect=1&resize=scale&password=secret for provider login
-purposes. #### Installation Guide for Windows (.exe) To ensure the seamless
-operation of our application, please follow the instructions below. These steps
-are designed to guide you through the installation process on Windows operating
-systems. ##### Prerequisites 1. **WebView2 Runtime**: Our application requires
-the *WebView2 Runtime* to be installed on your system. If you do not have it
+`chat.completion.create`. - Installation Guide for Windows (.exe): ð»
+[#installation-guide-for-windows](#installation-guide-for-windows-exe) - Join
+our Telegram Channel: ð¨ [telegram.me/g4f_channel](https://telegram.me/
+g4f_channel) - Join our Discord Group: ð¬ [discord.gg/XfybzPXPH5](https://
+discord.gg/XfybzPXPH5) - `g4f` now supports 100% local inference: ð§  [local-
+docs](https://g4f.mintlify.app/docs/core/usage/local) ## ð» Site Takedown Is
+your site on this repository and you want to take it down? Send an email to
+takedown@g4f.ai with proof it is yours and it will be removed as fast as
+possible. To prevent reproduction please secure your API. ð ## ð Feedback
+and Todo You can always leave some feedback here: https://forms.gle/
+FeWV9RLEedfdkmFN6 As per the survey, here is a list of improvements to come -
+[x] Update the repository to include the new openai library syntax (ex: `Openai
+()` class) | completed, use `g4f.client.Client` - [ ] Golang implementation -
+[ ] ð§ Improve Documentation (in /docs & Guides, Howtos, & Do video
+tutorials) - [x] Improve the provider status list & updates - [ ] Tutorials on
+how to reverse sites to write your own wrapper (PoC only ofc) - [x] Improve the
+Bing wrapper. (Wait and Retry or reuse conversation) - [ ] ð§ Write a
+standard provider performance test to improve the stability - [ ] Potential
+support and development of local models - [ ] ð§ Improve compatibility and
+error handling ## ð Table of Contents - [ð What's New](#-whats-new) -
+[ð Table of Contents](#-table-of-contents) - [ð ï¸ Getting Started](#-
+getting-started) + [Docker Container Guide](#docker-container-guide) +
+[Installation Guide for Windows (.exe)](#installation-guide-for-windows-exe) +
+[Use python](#use-python) - [Prerequisites](#prerequisites) - [Install using
+PyPI package:](#install-using-pypi-package) - [Install from source:](#install-
+from-source) - [Install using Docker:](#install-using-docker) - [ð¡ Usage](#-
+usage) * [Text Generation](#text-generation) * [Image Generation](#image-
+generation) * [Web UI](#web-ui) * [Interference API](#interference-api) *
+[Configuration](#configuration) - [ð Providers and Models](#-providers-and-
+models) * [GPT-4](#gpt-4) * [GPT-3.5](#gpt-35) * [Other](#other) * [Models]
+(#models) - [ð Powered by gpt4free](#-powered-by-gpt4free) - [ð¤
+Contribute](#-contribute) + [How do i create a new Provider?](#guide-how-do-i-
+create-a-new-provider) + [How can AI help me with writing code?](#guide-how-
+can-ai-help-me-with-writing-code) - [ð Contributors](#-contributors) -
+[Â©ï¸ Copyright](#-copyright) - [â­ Star History](#-star-history) - [ð
+License](#-license) ## ð ï¸ Getting Started #### Docker Container Guide
+##### Getting Started Quickly: 1. **Install Docker:** Begin by [downloading and
+installing Docker](https://docs.docker.com/get-docker/). 2. **Set Up the
+Container:** Use the following commands to pull the latest image and start the
+container: ```sh docker pull hlohaus789/g4f docker run -p 8080:8080 -p 1337:
+1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/har_and_cookies:/app/
+har_and_cookies hlohaus789/g4f:latest ``` 3. **Access the Client:** - To use
+the included client, navigate to: [http://localhost:8080/chat/](http://
+localhost:8080/chat/) - Or set the API base for your client to: [http://
+localhost:1337/v1](http://localhost:1337/v1) 4. **(Optional) Provider Login:**
+If required, you can access the container's desktop here: http://localhost:
+7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
+#### Installation Guide for Windows (.exe) To ensure the seamless operation of
+our application, please follow the instructions below. These steps are designed
+to guide you through the installation process on Windows operating systems.
+##### Prerequisites 1. **WebView2 Runtime**: Our application requires the
+*WebView2 Runtime* to be installed on your system. If you do not have it
 installed, please download and install it from the [Microsoft Developer
 Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If
 you already have *WebView2 Runtime* installed but are encountering issues,
 navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair
 option. ##### Installation Steps 2. **Download the Application**: Visit our
 [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and
 download the most recent version of the application, named `g4f.webview.*.exe`.
```

### Comparing `g4f-0.3.1.1/g4f.egg-info/SOURCES.txt` & `g4f-0.3.1.2/g4f.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
 g4f/Provider/needs_auth/Gemini.py
 g4f/Provider/needs_auth/Groq.py
 g4f/Provider/needs_auth/OpenRouter.py
 g4f/Provider/needs_auth/Openai.py
 g4f/Provider/needs_auth/OpenaiAccount.py
 g4f/Provider/needs_auth/OpenaiChat.py
+g4f/Provider/needs_auth/PerplexityApi.py
 g4f/Provider/needs_auth/Poe.py
 g4f/Provider/needs_auth/Raycast.py
 g4f/Provider/needs_auth/Theb.py
 g4f/Provider/needs_auth/ThebApi.py
 g4f/Provider/needs_auth/__init__.py
 g4f/Provider/not_working/AItianhu.py
 g4f/Provider/not_working/Bestim.py
```

### Comparing `g4f-0.3.1.1/g4f.egg-info/requires.txt` & `g4f-0.3.1.2/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.1/setup.py` & `g4f-0.3.1.2/setup.py`

 * *Files identical despite different names*

