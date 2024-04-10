# Comparing `tmp/g4f-0.2.9.0.tar.gz` & `tmp/g4f-0.2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.2.9.0.tar", last modified: Tue Apr  9 17:42:42 2024, max compression
+gzip compressed data, was "g4f-0.2.9.1.tar", last modified: Tue Apr  9 18:21:16 2024, max compression
```

## Comparing `g4f-0.2.9.0.tar` & `g4f-0.2.9.1.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.863630 g4f-0.2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-09 17:42:39.000000 g4f-0.2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 17:42:39.000000 g4f-0.2.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49105 2024-04-09 17:42:42.863630 g4f-0.2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    45989 2024-04-09 17:42:39.000000 g4f-0.2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.823629 g4f-0.2.9.0/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.831630 g4f-0.2.9.0/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    20732 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.831630 g4f-0.2.9.0/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.839630 g4f-0.2.9.0/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.839630 g4f-0.2.9.0/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.839630 g4f-0.2.9.0/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    31605 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.843629 g4f-0.2.9.0/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.843629 g4f-0.2.9.0/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.843629 g4f-0.2.9.0/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.843629 g4f-0.2.9.0/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.843629 g4f-0.2.9.0/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/openai/har_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.847630 g4f-0.2.9.0/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.847630 g4f-0.2.9.0/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.847630 g4f-0.2.9.0/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.847630 g4f-0.2.9.0/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.847630 g4f-0.2.9.0/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.851630 g4f-0.2.9.0/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.851630 g4f-0.2.9.0/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.819630 g4f-0.2.9.0/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.851630 g4f-0.2.9.0/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22127 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.851630 g4f-0.2.9.0/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.851630 g4f-0.2.9.0/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    43839 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.855630 g4f-0.2.9.0/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.855630 g4f-0.2.9.0/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.855630 g4f-0.2.9.0/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.855630 g4f-0.2.9.0/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.855630 g4f-0.2.9.0/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.859629 g4f-0.2.9.0/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.859629 g4f-0.2.9.0/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49105 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:42:42.863630 g4f-0.2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-09 17:42:39.000000 g4f-0.2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.235005 g4f-0.2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-09 18:21:12.000000 g4f-0.2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 18:21:12.000000 g4f-0.2.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49099 2024-04-09 18:21:16.235005 g4f-0.2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    45983 2024-04-09 18:21:12.000000 g4f-0.2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.199005 g4f-0.2.9.1/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.207005 g4f-0.2.9.1/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20732 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/Llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.207005 g4f-0.2.9.1/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.215005 g4f-0.2.9.1/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.215005 g4f-0.2.9.1/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.215005 g4f-0.2.9.1/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31605 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.219005 g4f-0.2.9.1/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.219005 g4f-0.2.9.1/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.219005 g4f-0.2.9.1/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.219005 g4f-0.2.9.1/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.219005 g4f-0.2.9.1/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/openai/har_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.219005 g4f-0.2.9.1/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.223005 g4f-0.2.9.1/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.223005 g4f-0.2.9.1/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.223005 g4f-0.2.9.1/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.223005 g4f-0.2.9.1/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.223005 g4f-0.2.9.1/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.223005 g4f-0.2.9.1/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.199005 g4f-0.2.9.1/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.223005 g4f-0.2.9.1/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22275 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.227005 g4f-0.2.9.1/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.227005 g4f-0.2.9.1/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    43946 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.227005 g4f-0.2.9.1/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.231005 g4f-0.2.9.1/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.231005 g4f-0.2.9.1/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.231005 g4f-0.2.9.1/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.231005 g4f-0.2.9.1/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.231005 g4f-0.2.9.1/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-09 18:21:12.000000 g4f-0.2.9.1/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:16.231005 g4f-0.2.9.1/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49099 2024-04-09 18:21:16.000000 g4f-0.2.9.1/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-09 18:21:16.000000 g4f-0.2.9.1/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:21:16.000000 g4f-0.2.9.1/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 18:21:16.000000 g4f-0.2.9.1/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 18:21:16.000000 g4f-0.2.9.1/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 18:21:16.000000 g4f-0.2.9.1/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:21:16.239006 g4f-0.2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-09 18:21:12.000000 g4f-0.2.9.1/setup.py
```

### Comparing `g4f-0.2.9.0/LICENSE` & `g4f-0.2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/PKG-INFO` & `g4f-0.2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.9.0
+Version: 0.2.9.1
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -261,15 +261,15 @@
 
 
 [![Image with cat](/docs/cat.jpeg)](/docs/client.md)
 
 **Full Documentation for Python API**
 
 - New AsyncClient API from G4F: [/docs/async_client](/docs/async_client.md)
-- Client API like the OpenAI Python library: [/docs/client](/docs/async_client.md)
+- Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
 - Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
 
 #### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.9.0 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.2.9.1 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -144,15 +144,15 @@
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
 client.md) **Full Documentation for Python API** - New AsyncClient API from
 G4F: [/docs/async_client](/docs/async_client.md) - Client API like the OpenAI
-Python library: [/docs/client](/docs/async_client.md) - Legacy API with python
+Python library: [/docs/client](/docs/client.md) - Legacy API with python
 modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
 interface, type the following codes in python: ```python from g4f.gui import
 run_gui run_gui() ``` or execute the following command: ```bash python -
 m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
 Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
 interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
 Configuration #### Cookies You need cookies for BingCreateImages and the Gemini
```

### Comparing `g4f-0.2.9.0/README.md` & `g4f-0.2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
 
 [![Image with cat](/docs/cat.jpeg)](/docs/client.md)
 
 **Full Documentation for Python API**
 
 - New AsyncClient API from G4F: [/docs/async_client](/docs/async_client.md)
-- Client API like the OpenAI Python library: [/docs/client](/docs/async_client.md)
+- Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
 - Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
 
 #### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
```

#### html2text {}

```diff
@@ -103,15 +103,15 @@
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
 client.md) **Full Documentation for Python API** - New AsyncClient API from
 G4F: [/docs/async_client](/docs/async_client.md) - Client API like the OpenAI
-Python library: [/docs/client](/docs/async_client.md) - Legacy API with python
+Python library: [/docs/client](/docs/client.md) - Legacy API with python
 modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
 interface, type the following codes in python: ```python from g4f.gui import
 run_gui run_gui() ``` or execute the following command: ```bash python -
 m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
 Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
 interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
 Configuration #### Cookies You need cookies for BingCreateImages and the Gemini
```

### Comparing `g4f-0.2.9.0/g4f/Provider/Aura.py` & `g4f-0.2.9.1/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/Bing.py` & `g4f-0.2.9.1/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/BingCreateImages.py` & `g4f-0.2.9.1/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/ChatForAi.py` & `g4f-0.2.9.1/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/Chatgpt4Online.py` & `g4f-0.2.9.1/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/ChatgptAi.py` & `g4f-0.2.9.1/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/ChatgptFree.py` & `g4f-0.2.9.1/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/ChatgptNext.py` & `g4f-0.2.9.1/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/ChatgptX.py` & `g4f-0.2.9.1/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/DeepInfra.py` & `g4f-0.2.9.1/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/DuckDuckGo.py` & `g4f-0.2.9.1/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/FlowGpt.py` & `g4f-0.2.9.1/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/FreeChatgpt.py` & `g4f-0.2.9.1/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/FreeGpt.py` & `g4f-0.2.9.1/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/GeminiPro.py` & `g4f-0.2.9.1/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/GeminiProChat.py` & `g4f-0.2.9.1/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/GigaChat.py` & `g4f-0.2.9.1/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/GptTalkRu.py` & `g4f-0.2.9.1/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/HuggingChat.py` & `g4f-0.2.9.1/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/HuggingFace.py` & `g4f-0.2.9.1/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/Koala.py` & `g4f-0.2.9.1/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/Liaobots.py` & `g4f-0.2.9.1/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/Llama2.py` & `g4f-0.2.9.1/g4f/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/Local.py` & `g4f-0.2.9.1/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/PerplexityLabs.py` & `g4f-0.2.9.1/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/Pi.py` & `g4f-0.2.9.1/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/Vercel.py` & `g4f-0.2.9.1/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.2.9.1/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/You.py` & `g4f-0.2.9.1/g4f/Provider/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/__init__.py` & `g4f-0.2.9.1/g4f/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/bing/conversation.py` & `g4f-0.2.9.1/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/bing/create_images.py` & `g4f-0.2.9.1/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/bing/upload_image.py` & `g4f-0.2.9.1/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/AiService.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Aibn.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Aichat.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Ails.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Berlin.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Equing.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Forefront.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/H2o.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Myshell.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Phind.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/V50.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Vercel.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/deprecated/__init__.py` & `g4f-0.2.9.1/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.2.9.1/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.2.9.1/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/needs_auth/Groq.py` & `g4f-0.2.9.1/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/needs_auth/Openai.py` & `g4f-0.2.9.1/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.2.9.1/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/needs_auth/Poe.py` & `g4f-0.2.9.1/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.2.9.1/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/needs_auth/Theb.py` & `g4f-0.2.9.1/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.2.9.1/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/AItianhu.py` & `g4f-0.2.9.1/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/Bestim.py` & `g4f-0.2.9.1/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/ChatBase.py` & `g4f-0.2.9.1/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.2.9.1/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.2.9.1/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.2.9.1/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.2.9.1/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/Gpt6.py` & `g4f-0.2.9.1/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/GptChatly.py` & `g4f-0.2.9.1/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/GptForLove.py` & `g4f-0.2.9.1/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/GptGo.py` & `g4f-0.2.9.1/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/GptGod.py` & `g4f-0.2.9.1/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.2.9.1/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.2.9.1/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.2.9.1/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/npm/package-lock.json` & `g4f-0.2.9.1/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/openai/crypt.py` & `g4f-0.2.9.1/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/openai/har_file.py` & `g4f-0.2.9.1/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.2.9.1/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/selenium/Bard.py` & `g4f-0.2.9.1/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/selenium/MyShell.py` & `g4f-0.2.9.1/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.2.9.1/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/selenium/Phind.py` & `g4f-0.2.9.1/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/selenium/TalkAi.py` & `g4f-0.2.9.1/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.2.9.1/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.2.9.1/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/unfinished/Komo.py` & `g4f-0.2.9.1/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.2.9.1/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/Provider/you/har_file.py` & `g4f-0.2.9.1/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/__init__.py` & `g4f-0.2.9.1/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/api/__init__.py` & `g4f-0.2.9.1/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/api/_logging.py` & `g4f-0.2.9.1/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/cli.py` & `g4f-0.2.9.1/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/client/async_client.py` & `g4f-0.2.9.1/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/client/client.py` & `g4f-0.2.9.1/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/client/helper.py` & `g4f-0.2.9.1/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/client/image_models.py` & `g4f-0.2.9.1/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/client/service.py` & `g4f-0.2.9.1/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/client/stubs.py` & `g4f-0.2.9.1/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/client/types.py` & `g4f-0.2.9.1/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/cookies.py` & `g4f-0.2.9.1/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/errors.py` & `g4f-0.2.9.1/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/__init__.py` & `g4f-0.2.9.1/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/index.html` & `g4f-0.2.9.1/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/css/style.css` & `g4f-0.2.9.1/g4f/gui/client/static/css/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,15 @@
     font-size: 10px;
 }
 
 .message {
     width: 100%;
     overflow-wrap: break-word;
     display: flex;
+    flex-direction: column;
     gap: var(--section-gap);
     padding: var(--inner-gap) var(--section-gap);
     padding-bottom: 0;
 }
 
 .message.regenerate {
     opacity: 0.75;
@@ -585,15 +586,15 @@
 
 .buttons input:checked+label,
 .settings input:checked+label {
     background: var(--accent);
 }
 
 .settings .bottom_buttons {
-    flex-direction: row;
+    flex-direction: column;
 }
 
 .settings .bottom_buttons button {
     display: inline-block;
     max-width: 210px;
     width: 100%;
 }
@@ -648,14 +649,20 @@
 @media only screen and (min-width: 40em) {
     select {
         width: 200px;
     }
     .field {
         padding-right: 15px
     }
+    .message {
+        flex-direction: row;
+    }
+    .settings .bottom_buttons {
+        flex-direction: row;
+    }
 }
 
 .input-box {
     display: flex;
     align-items: center;
     cursor: pointer;
 }
@@ -1066,22 +1073,22 @@
     outline: none;
     padding: var(--inner-gap) var(--section-gap);
     resize: vertical;
 }
 
 .settings {
     width: 100%;
-    min-width: 700px;
     display: flex;
     flex-direction: column;
 }
 
 .settings .paper {
     overflow: auto;
     flex-direction: column;
+    min-width: 400px;
 }
 
 .settings .field {
     margin: var(--inner-gap) 0;
 }
 
 .settings textarea {
@@ -1131,15 +1138,15 @@
     background: #28293629;
     border-radius: var(--border-radius-1);
     border: 1px solid var(--blur-border);
     font-size: 15px;
 }
 
 #message-input {
-    height: 82px;
+    height: 90px;
     margin-left: 20px;
     max-height: 200px;
 }
 
 #message-input::-webkit-scrollbar {
     width: 5px;
 }
```

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.2.9.1/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.2.9.1/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.2.9.1/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.2.9.1/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/img/gpt.png` & `g4f-0.2.9.1/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/img/user.png` & `g4f-0.2.9.1/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.2.9.1/g4f/gui/client/static/js/chat.v1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -92,18 +92,20 @@
         }
     });
     document.querySelectorAll(".message .fa-volume-high").forEach(async (el) => {
         if (!("click" in el.dataset)) {
             el.dataset.click = "true";
             el.addEventListener("click", async () => {
                 if ("active" in el.classList || window.doSpeech) {
+                    el.classList.add("blink")
                     stopped = true;
                     return;
                 }
                 if (stopped) {
+                    el.classList.remove("blink")
                     stopped = false;
                     return;
                 }
                 el.classList.add("blink")
                 el.classList.add("active")
                 const message_el = el.parentElement.parentElement.parentElement;
                 const content_el = el.parentElement.parentElement;
@@ -121,15 +123,15 @@
                 window.onSpeechResponse = (url) => {
                     el.classList.remove("blink")
                     if (url) {
                         var sound = document.createElement('audio');
                         sound.controls = 'controls';
                         sound.src = url;
                         sound.type = 'audio/wav';
-                        if (ended) {
+                        if (ended && !stopped) {
                             sound.autoplay = true;
                         }
                         sound.onended = function() {
                             ended = true;
                         };
                         sound.onplay = function() {
                             ended = false;
```

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.2.9.1/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.2.9.1/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/js/icons.js` & `g4f-0.2.9.1/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.2.9.1/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.2.9.1/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.2.9.1/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/server/android_gallery.py` & `g4f-0.2.9.1/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/server/api.py` & `g4f-0.2.9.1/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/server/backend.py` & `g4f-0.2.9.1/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/server/config.py` & `g4f-0.2.9.1/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/server/internet.py` & `g4f-0.2.9.1/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/server/js_api.py` & `g4f-0.2.9.1/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/server/website.py` & `g4f-0.2.9.1/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/gui/webview.py` & `g4f-0.2.9.1/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/image.py` & `g4f-0.2.9.1/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/local/__init__.py` & `g4f-0.2.9.1/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/locals/models.py` & `g4f-0.2.9.1/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/locals/provider.py` & `g4f-0.2.9.1/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/models.py` & `g4f-0.2.9.1/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/providers/base_provider.py` & `g4f-0.2.9.1/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/providers/create_images.py` & `g4f-0.2.9.1/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/providers/helper.py` & `g4f-0.2.9.1/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/providers/retry_provider.py` & `g4f-0.2.9.1/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/providers/types.py` & `g4f-0.2.9.1/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/requests/__init__.py` & `g4f-0.2.9.1/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/requests/aiohttp.py` & `g4f-0.2.9.1/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/requests/curl_cffi.py` & `g4f-0.2.9.1/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/requests/defaults.py` & `g4f-0.2.9.1/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/requests/raise_for_status.py` & `g4f-0.2.9.1/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/stubs.py` & `g4f-0.2.9.1/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/typing.py` & `g4f-0.2.9.1/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/version.py` & `g4f-0.2.9.1/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f/webdriver.py` & `g4f-0.2.9.1/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f.egg-info/PKG-INFO` & `g4f-0.2.9.1/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.9.0
+Version: 0.2.9.1
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -261,15 +261,15 @@
 
 
 [![Image with cat](/docs/cat.jpeg)](/docs/client.md)
 
 **Full Documentation for Python API**
 
 - New AsyncClient API from G4F: [/docs/async_client](/docs/async_client.md)
-- Client API like the OpenAI Python library: [/docs/client](/docs/async_client.md)
+- Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
 - Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
 
 #### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.9.0 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.2.9.1 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -144,15 +144,15 @@
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
 client.md) **Full Documentation for Python API** - New AsyncClient API from
 G4F: [/docs/async_client](/docs/async_client.md) - Client API like the OpenAI
-Python library: [/docs/client](/docs/async_client.md) - Legacy API with python
+Python library: [/docs/client](/docs/client.md) - Legacy API with python
 modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
 interface, type the following codes in python: ```python from g4f.gui import
 run_gui run_gui() ``` or execute the following command: ```bash python -
 m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
 Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
 interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
 Configuration #### Cookies You need cookies for BingCreateImages and the Gemini
```

### Comparing `g4f-0.2.9.0/g4f.egg-info/SOURCES.txt` & `g4f-0.2.9.1/g4f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/g4f.egg-info/requires.txt` & `g4f-0.2.9.1/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.0/setup.py` & `g4f-0.2.9.1/setup.py`

 * *Files identical despite different names*

