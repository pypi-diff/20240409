# Comparing `tmp/g4f-0.2.8.2.tar.gz` & `tmp/g4f-0.2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.2.8.2.tar", last modified: Sun Apr  7 18:05:19 2024, max compression
+gzip compressed data, was "g4f-0.2.9.0.tar", last modified: Tue Apr  9 17:42:42 2024, max compression
```

## Comparing `g4f-0.2.8.2.tar` & `g4f-0.2.9.0.tar`

### file list

```diff
@@ -1,226 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.853846 g4f-0.2.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-07 18:05:10.000000 g4f-0.2.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-07 18:05:10.000000 g4f-0.2.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49027 2024-04-07 18:05:19.853846 g4f-0.2.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    45911 2024-04-07 18:05:10.000000 g4f-0.2.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.821846 g4f-0.2.8.2/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.825846 g4f-0.2.8.2/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    20635 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/Llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.829846 g4f-0.2.8.2/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.833846 g4f-0.2.8.2/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.833846 g4f-0.2.8.2/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.833846 g4f-0.2.8.2/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    31605 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.837846 g4f-0.2.8.2/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.837846 g4f-0.2.8.2/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.837846 g4f-0.2.8.2/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.837846 g4f-0.2.8.2/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.837846 g4f-0.2.8.2/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/openai/har_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.841846 g4f-0.2.8.2/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.841846 g4f-0.2.8.2/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.841846 g4f-0.2.8.2/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.841846 g4f-0.2.8.2/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.841846 g4f-0.2.8.2/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.841846 g4f-0.2.8.2/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.841846 g4f-0.2.8.2/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.817846 g4f-0.2.8.2/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.845846 g4f-0.2.8.2/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.845846 g4f-0.2.8.2/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.845846 g4f-0.2.8.2/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    34997 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/client/static/js/icons.js
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.845846 g4f-0.2.8.2/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.845846 g4f-0.2.8.2/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.849846 g4f-0.2.8.2/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.849846 g4f-0.2.8.2/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.849846 g4f-0.2.8.2/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-07 18:05:10.000000 g4f-0.2.8.2/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:05:19.849846 g4f-0.2.8.2/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49027 2024-04-07 18:05:19.000000 g4f-0.2.8.2/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-07 18:05:19.000000 g4f-0.2.8.2/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:05:19.000000 g4f-0.2.8.2/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 18:05:19.000000 g4f-0.2.8.2/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-07 18:05:19.000000 g4f-0.2.8.2/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-07 18:05:19.000000 g4f-0.2.8.2/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:05:19.853846 g4f-0.2.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-07 18:05:10.000000 g4f-0.2.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.863630 g4f-0.2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-09 17:42:39.000000 g4f-0.2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 17:42:39.000000 g4f-0.2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49105 2024-04-09 17:42:42.863630 g4f-0.2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    45989 2024-04-09 17:42:39.000000 g4f-0.2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.823629 g4f-0.2.9.0/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.831630 g4f-0.2.9.0/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20732 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.831630 g4f-0.2.9.0/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.839630 g4f-0.2.9.0/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.839630 g4f-0.2.9.0/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.839630 g4f-0.2.9.0/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31605 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.843629 g4f-0.2.9.0/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.843629 g4f-0.2.9.0/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.843629 g4f-0.2.9.0/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.843629 g4f-0.2.9.0/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.843629 g4f-0.2.9.0/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/openai/har_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.847630 g4f-0.2.9.0/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.847630 g4f-0.2.9.0/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.847630 g4f-0.2.9.0/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.847630 g4f-0.2.9.0/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.847630 g4f-0.2.9.0/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.851630 g4f-0.2.9.0/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.851630 g4f-0.2.9.0/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.819630 g4f-0.2.9.0/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.851630 g4f-0.2.9.0/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22127 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.851630 g4f-0.2.9.0/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.851630 g4f-0.2.9.0/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    43839 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.855630 g4f-0.2.9.0/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.855630 g4f-0.2.9.0/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.855630 g4f-0.2.9.0/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.855630 g4f-0.2.9.0/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.855630 g4f-0.2.9.0/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.859629 g4f-0.2.9.0/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-09 17:42:39.000000 g4f-0.2.9.0/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:42.859629 g4f-0.2.9.0/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49105 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 17:42:42.000000 g4f-0.2.9.0/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:42:42.863630 g4f-0.2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-09 17:42:39.000000 g4f-0.2.9.0/setup.py
```

### Comparing `g4f-0.2.8.2/LICENSE` & `g4f-0.2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/PKG-INFO` & `g4f-0.2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.8.2
+Version: 0.2.9.0
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -260,15 +260,16 @@
 ```
 
 
 [![Image with cat](/docs/cat.jpeg)](/docs/client.md)
 
 **Full Documentation for Python API**
 
-- New Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
+- New AsyncClient API from G4F: [/docs/async_client](/docs/async_client.md)
+- Client API like the OpenAI Python library: [/docs/client](/docs/async_client.md)
 - Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
 
 #### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.8.2 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.2.9.0 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -142,16 +142,17 @@
 g4f.client import Client client = Client() response =
 client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
-client.md) **Full Documentation for Python API** - New Client API like the
-OpenAI Python library: [/docs/client](/docs/client.md) - Legacy API with python
+client.md) **Full Documentation for Python API** - New AsyncClient API from
+G4F: [/docs/async_client](/docs/async_client.md) - Client API like the OpenAI
+Python library: [/docs/client](/docs/async_client.md) - Legacy API with python
 modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
 interface, type the following codes in python: ```python from g4f.gui import
 run_gui run_gui() ``` or execute the following command: ```bash python -
 m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
 Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
 interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
 Configuration #### Cookies You need cookies for BingCreateImages and the Gemini
```

### Comparing `g4f-0.2.8.2/README.md` & `g4f-0.2.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,16 @@
 ```
 
 
 [![Image with cat](/docs/cat.jpeg)](/docs/client.md)
 
 **Full Documentation for Python API**
 
-- New Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
+- New AsyncClient API from G4F: [/docs/async_client](/docs/async_client.md)
+- Client API like the OpenAI Python library: [/docs/client](/docs/async_client.md)
 - Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
 
 #### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
```

#### html2text {}

```diff
@@ -101,16 +101,17 @@
 g4f.client import Client client = Client() response =
 client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
-client.md) **Full Documentation for Python API** - New Client API like the
-OpenAI Python library: [/docs/client](/docs/client.md) - Legacy API with python
+client.md) **Full Documentation for Python API** - New AsyncClient API from
+G4F: [/docs/async_client](/docs/async_client.md) - Client API like the OpenAI
+Python library: [/docs/client](/docs/async_client.md) - Legacy API with python
 modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
 interface, type the following codes in python: ```python from g4f.gui import
 run_gui run_gui() ``` or execute the following command: ```bash python -
 m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
 Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
 interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
 Configuration #### Cookies You need cookies for BingCreateImages and the Gemini
```

### Comparing `g4f-0.2.8.2/g4f/Provider/Aura.py` & `g4f-0.2.9.0/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/Bing.py` & `g4f-0.2.9.0/g4f/Provider/Bing.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     @classmethod
     def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
         timeout: int = 900,
+        api_key: str = None,
         cookies: Cookies = None,
         connector: BaseConnector = None,
         tone: str = None,
         image: ImageType = None,
         web_search: bool = False,
         context: str = None,
         **kwargs
@@ -64,14 +65,16 @@
         :param cookies: Cookies for the session.
         :param tone: The tone of the response.
         :param image: The image type to be used.
         :param web_search: Flag to enable or disable web search.
         :return: An asynchronous result object.
         """
         prompt = messages[-1]["content"]
+        if api_key is not None:
+            cookies["_U"] = api_key
         if context is None:
             context = create_context(messages[:-1]) if len(messages) > 1 else None
         if tone is None:
             tone = tone if model.startswith("gpt-4") else model
         tone = cls.get_model("" if tone is None else tone)
         gpt4_turbo = True if model.startswith("gpt-4-turbo") else False
```

### Comparing `g4f-0.2.8.2/g4f/Provider/BingCreateImages.py` & `g4f-0.2.9.0/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/ChatForAi.py` & `g4f-0.2.9.0/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/Chatgpt4Online.py` & `g4f-0.2.9.0/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/ChatgptAi.py` & `g4f-0.2.9.0/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/ChatgptFree.py` & `g4f-0.2.9.0/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/ChatgptNext.py` & `g4f-0.2.9.0/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/ChatgptX.py` & `g4f-0.2.9.0/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/DeepInfra.py` & `g4f-0.2.9.0/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/FlowGpt.py` & `g4f-0.2.9.0/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/FreeChatgpt.py` & `g4f-0.2.9.0/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/FreeGpt.py` & `g4f-0.2.9.0/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/GeminiPro.py` & `g4f-0.2.9.0/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/GeminiProChat.py` & `g4f-0.2.9.0/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/GigaChat.py` & `g4f-0.2.9.0/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/GptTalkRu.py` & `g4f-0.2.9.0/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/HuggingChat.py` & `g4f-0.2.9.0/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/HuggingFace.py` & `g4f-0.2.9.0/g4f/Provider/HuggingFace.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from ..errors import RateLimitError, ModelNotFoundError
 from ..requests.raise_for_status import raise_for_status
 
 class HuggingFace(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://huggingface.co/chat"
     working = True
     supports_message_history = True
+    models = [
+        "mistralai/Mixtral-8x7B-Instruct-v0.1",
+        "mistralai/Mistral-7B-Instruct-v0.2"
+    ]
     default_model = "mistralai/Mixtral-8x7B-Instruct-v0.1"
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
@@ -25,15 +29,15 @@
         connector: BaseConnector = None,
         api_base: str = "https://api-inference.huggingface.co",
         api_key: str = None,
         max_new_tokens: int = 1024,
         temperature: float = 0.7,
         **kwargs
     ) -> AsyncResult:
-        model = cls.get_model(model)
+        model = cls.get_model(model) if not model else model
         headers = {}
         if api_key is not None:
             headers["Authorization"] = f"Bearer {api_key}"
         params = {
             "return_full_text": False,
             "max_new_tokens": max_new_tokens,
             "temperature": temperature,
```

### Comparing `g4f-0.2.8.2/g4f/Provider/Koala.py` & `g4f-0.2.9.0/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/Liaobots.py` & `g4f-0.2.9.0/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/Llama2.py` & `g4f-0.2.9.0/g4f/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/Local.py` & `g4f-0.2.9.0/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/PerplexityLabs.py` & `g4f-0.2.9.0/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/Pi.py` & `g4f-0.2.9.0/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/Vercel.py` & `g4f-0.2.9.0/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/You.py` & `g4f-0.2.9.0/g4f/Provider/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/__init__.py` & `g4f-0.2.9.0/g4f/Provider/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .ChatForAi        import ChatForAi
 from .Chatgpt4Online   import Chatgpt4Online
 from .ChatgptAi        import ChatgptAi
 from .ChatgptFree      import ChatgptFree
 from .ChatgptNext      import ChatgptNext
 from .ChatgptX         import ChatgptX
 from .DeepInfra        import DeepInfra
+from .DuckDuckGo       import DuckDuckGo
 from .FlowGpt          import FlowGpt
 from .FreeChatgpt      import FreeChatgpt
 from .FreeGpt          import FreeGpt
 from .GigaChat         import GigaChat
 from .GeminiPro        import GeminiPro
 from .GeminiProChat    import GeminiProChat
 from .GptTalkRu        import GptTalkRu
@@ -33,14 +34,15 @@
 from .Koala            import Koala
 from .Liaobots         import Liaobots
 from .Llama2           import Llama2
 from .Local            import Local
 from .PerplexityLabs   import PerplexityLabs
 from .Pi               import Pi
 from .Vercel           import Vercel
+from .WhiteRabbitNeo   import WhiteRabbitNeo
 from .You              import You
 
 import sys
 
 __modules__: list = [
     getattr(sys.modules[__name__], provider) for provider in dir()
     if not provider.startswith("__")
```

### Comparing `g4f-0.2.8.2/g4f/Provider/bing/conversation.py` & `g4f-0.2.9.0/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/bing/create_images.py` & `g4f-0.2.9.0/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/bing/upload_image.py` & `g4f-0.2.9.0/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/AiService.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Aibn.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Aichat.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Ails.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Berlin.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Equing.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Forefront.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/H2o.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Myshell.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Phind.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/V50.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Vercel.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/deprecated/__init__.py` & `g4f-0.2.9.0/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.2.9.0/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.2.9.0/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/needs_auth/Groq.py` & `g4f-0.2.9.0/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/needs_auth/Openai.py` & `g4f-0.2.9.0/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.2.9.0/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/needs_auth/Poe.py` & `g4f-0.2.9.0/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.2.9.0/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/needs_auth/Theb.py` & `g4f-0.2.9.0/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.2.9.0/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/AItianhu.py` & `g4f-0.2.9.0/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/Bestim.py` & `g4f-0.2.9.0/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/ChatBase.py` & `g4f-0.2.9.0/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.2.9.0/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.2.9.0/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.2.9.0/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.2.9.0/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/Gpt6.py` & `g4f-0.2.9.0/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/GptChatly.py` & `g4f-0.2.9.0/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/GptForLove.py` & `g4f-0.2.9.0/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/GptGo.py` & `g4f-0.2.9.0/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/GptGod.py` & `g4f-0.2.9.0/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.2.9.0/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.2.9.0/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.2.9.0/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/npm/package-lock.json` & `g4f-0.2.9.0/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/openai/crypt.py` & `g4f-0.2.9.0/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/openai/har_file.py` & `g4f-0.2.9.0/g4f/Provider/openai/har_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,18 @@
             except json.JSONDecodeError:
                 # Error: not a HAR file!
                 continue
             for v in harFile['log']['entries']:
                 if arkPreURL in v['request']['url']:
                     chatArks.append(parseHAREntry(v))
                 elif v['request']['url'] == sessionUrl:
-                    accessToken = json.loads(v["response"]["content"]["text"]).get("accessToken")
+                    try:
+                        accessToken = json.loads(v["response"]["content"]["text"]).get("accessToken")
+                    except KeyError:
+                        continue
                     cookies = {c['name']: c['value'] for c in v['request']['cookies']}
     if not accessToken:
         raise NoValidHarFileError("No accessToken found in .har files")
     if not chatArks:
         return None, accessToken, cookies
     return chatArks.pop(), accessToken, cookies
 
@@ -123,8 +126,8 @@
 async def getArkoseAndAccessToken(proxy: str):
     global chatArk, accessToken, cookies
     if chatArk is None or accessToken is None:
         chatArk, accessToken, cookies = readHAR()
     if chatArk is None:
         return None, accessToken, cookies
     newReq = genArkReq(chatArk)
-    return await sendRequest(newReq, proxy), accessToken, cookies
+    return await sendRequest(newReq, proxy), accessToken, cookies
```

### Comparing `g4f-0.2.8.2/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.2.9.0/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/selenium/Bard.py` & `g4f-0.2.9.0/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/selenium/MyShell.py` & `g4f-0.2.9.0/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.2.9.0/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/selenium/Phind.py` & `g4f-0.2.9.0/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/selenium/TalkAi.py` & `g4f-0.2.9.0/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.2.9.0/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.2.9.0/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/unfinished/Komo.py` & `g4f-0.2.9.0/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.2.9.0/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/Provider/you/har_file.py` & `g4f-0.2.9.0/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/__init__.py` & `g4f-0.2.9.0/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/api/__init__.py` & `g4f-0.2.9.0/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/api/_logging.py` & `g4f-0.2.9.0/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/cli.py` & `g4f-0.2.9.0/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/client/async_client.py` & `g4f-0.2.9.0/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/client/client.py` & `g4f-0.2.9.0/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/client/helper.py` & `g4f-0.2.9.0/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/client/image_models.py` & `g4f-0.2.9.0/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/client/service.py` & `g4f-0.2.9.0/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/client/stubs.py` & `g4f-0.2.9.0/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/client/types.py` & `g4f-0.2.9.0/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/cookies.py` & `g4f-0.2.9.0/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/errors.py` & `g4f-0.2.9.0/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/__init__.py` & `g4f-0.2.9.0/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/client/index.html` & `g4f-0.2.9.0/g4f/gui/client/index.html`

 * *Files 11% similar despite different names*

```diff
@@ -33,83 +33,124 @@
     <script type="module" src="https://cdn.jsdelivr.net/npm/mistral-tokenizer-js" async>
         import mistralTokenizer from "mistral-tokenizer-js"
     </script>
     <script type="module" src="https://belladoreai.github.io/llama-tokenizer-js/llama-tokenizer.js" async>
         import llamaTokenizer from "llama-tokenizer-js"
     </script>
     <script src="https://unpkg.com/gpt-tokenizer/dist/cl100k_base.js" async></script>
+    <script src="/static/js/text_to_speech/index.js" async></script>
     <script>
         const user_image = '<img src="/static/img/user.png" alt="your avatar">';
         const gpt_image = '<img src="/static/img/gpt.png" alt="your avatar">';
     </script>
     <script src="/static/js/highlight.min.js"></script>
     <script>window.conversation_id = "{{chat_id}}"</script>
     <title>g4f - gui</title>
 </head>
 
 <body>
     <div class="gradient"></div>
     <div class="row">
-        <div class="box conversations hidden">
+        <div class="box conversations">
             <div class="top">
                 <button class="new_convo" onclick="new_conversation()">
                     <i class="fa-regular fa-plus"></i>
                     <span>New Conversation</span>
                 </button>
             </div>
             <div class="bottom_buttons">
-                <button onclick="delete_conversations()">
-                    <i class="fa-regular fa-trash"></i>
-                    <span>Clear Conversations</span>
-                </button>
-                <button onclick="save_storage()">
-                    <i class="fa-solid fa-download"></i>
-                    <a href="" onclick="return false;">Export Conversations</a>
+                <button onclick="open_settings();">
+                    <i class="fa-solid fa-toolbox"></i>
+                    <span>Open Settings</span>
                 </button>
                 <div class="info">
+                    <i class="fa-brands fa-discord"></i>
+                    <span class="convo-title">discord ~ <a href="https://discord.gg/XfybzPXPH5">discord.gg/XfybzPXPH5</a>
+                    </span>
+                </div>
+                <div class="info">
                     <i class="fa-brands fa-github"></i>
-                    <span class="convo-title">github ~ <a href="https://github.com/xtekky/gpt4free">@gpt4free</a>
+                    <span class="convo-title">github ~ <a href="https://github.com/xtekky/gpt4free">@xtekky/gpt4free</a>
                     </span>
                 </div>
                 <div class="info">
                     <i class="fa-solid fa-star"></i>
                     <span id="version_text" class="convo-title"></span>
                 </div>
             </div>
         </div>
-        <div class="settings">
-            <div class="field box">
-                <label for="OpenaiChat-api_key" class="label" title="">OpenaiChat: access_token</label>
-                <textarea id="OpenaiChat-api_key" name="OpenaiChat[api_key]" placeholder="..."></textarea>
+        <div class="settings hidden">
+            <div class="paper">
+            <div class="field">
+                <span class="label">Web Access</span>
+                <input type="checkbox" id="switch" />
+                <label for="switch" class="toogle" title="Add the pages of the first 5 search results to the query."></label>
+            </div>
+            <div class="field">
+                <span class="label">Disable History</span>
+                <input type="checkbox" id="history" />
+                <label for="history" class="toogle" title="To improve the reaction time or if you have trouble with large conversations."></label>
             </div>
             <div class="field">
-                <span class="label">OpenaiChat: Auto continue</span>
-                <input id="OpenaiChat-auto_continue" type="checkbox" name="OpenaiChat[auto_continue]" checked/>
-                <label for="OpenaiChat-auto_continue" class="toogle" title=""></label>
+                <span class="label">Hide System prompt</span>
+                <input type="checkbox" id="hide-systemPrompt" />
+                <label for="hide-systemPrompt" class="toogle" title="For more space on phones"></label>
+            </div>
+            <div class="field">
+                <span class="label">Auto continue</span>
+                <input id="auto_continue" type="checkbox" name="auto_continue" checked/>
+                <label for="auto_continue" class="toogle" title="Continue large responses in OpenaiChat"></label>
+            </div>
+            <div class="field box">
+                <label for="message-input-height" class="label" title="">Input max. grow height</label>
+                <input type="number" id="message-input-height" value="200"/>
+            </div>
+            <div class="field box">
+                <label for="recognition-language" class="label" title="">Speech recognition lang</label>
+                <input type="text" id="recognition-language" value="" placeholder="navigator.language"/>
+            </div>
+            <div class="field box">
+                <label for="OpenaiChat-api_key" class="label" title="">OpenaiChat: api_key</label>
+                <textarea id="OpenaiChat-api_key" name="OpenaiChat[api_key]" placeholder="..."></textarea>
             </div>
             <div class="field box">
                 <label for="Bing-api_key" class="label" title="">Bing: "_U" cookie</label>
                 <textarea id="Bing-api_key" name="Bing[api_key]" placeholder="..."></textarea>
             </div>
             <div class="field box">
-                <label for="Gemini-api_key" class="label" title="">Gemini: Auth cookies</label>
+                <label for="Gemini-api_key" class="label" title="">Gemini: Cookies</label>
                 <textarea id="Gemini-api_key" name="Gemini[api_key]" placeholder="..."></textarea>
             </div>
             <div class="field box">
                 <label for="Openai-api_key" class="label" title="">Openai: api_key</label>
                 <textarea id="Openai-api_key" name="Openai[api_key]" placeholder="..."></textarea>
             </div>
             <div class="field box">
+                <label for="Groq-api_key" class="label" title="">Groq: api_key</label>
+                <textarea id="Groq-api_key" name="Groq[api_key]" placeholder="..."></textarea>
+            </div>
+            <div class="field box">
                 <label for="GeminiPro-api_key" class="label" title="">GeminiPro: api_key</label>
                 <textarea id="GeminiPro-api_key" name="GeminiPro[api_key]" placeholder="..."></textarea>
             </div>
             <div class="field box">
                 <label for="HuggingFace-api_key" class="label" title="">HuggingFace: api_key</label>
                 <textarea id="HuggingFace-api_key" name="HuggingFace[api_key]" placeholder="..."></textarea>
             </div>
+            </div>
+            <div class="bottom_buttons">
+                <button onclick="delete_conversations()">
+                    <i class="fa-regular fa-trash"></i>
+                    <span>Clear Conversations</span>
+                </button>
+                <button onclick="save_storage()">
+                    <i class="fa-solid fa-download"></i>
+                    <a href="" onclick="return false;">Export Conversations</a>
+                </button>
+            </div>
         </div>
         <div class="conversation">
             <textarea id="systemPrompt" class="box" placeholder="System prompt"></textarea>    
             <div id="messages" class="box"></div>
             <div class="toolbar">
                 <div id="input-count" class="">
                     &nbsp;
@@ -139,14 +180,17 @@
                         <input type="file" id="camera" name="camera" accept="image/*" capture="camera" required/>
                         <i class="fa-solid fa-camera"></i>
                     </label>
                     <label class="file-label" for="file">
                         <input type="file" id="file" name="file" accept="text/plain, text/html, text/xml, application/json, text/javascript, .sh, .py, .php, .css, .yaml, .sql, .log, .csv, .twig, .md" required/>
                         <i class="fa-solid fa-paperclip"></i>
                     </label>
+                    <label class="micro-label" for="micro">
+                        <i class="fa-solid fa-microphone-slash"></i>
+                    </label>
                     <div id="send-button">
                         <i class="fa-solid fa-paper-plane-top"></i>
                     </div>
                 </div>
             </div>
             <div class="buttons">
                 <div class="field">
@@ -157,51 +201,23 @@
                         <option value="llama2-70b">llama2-70b</option>
                         <option value="gemini-pro">gemini-pro</option>
                         <option value="">----</option>
                     </select>
                     <select name="model2" id="model2" class="hidden"></select>
                 </div>
                 <div class="field">
-                    <select name="jailbreak" id="jailbreak" style="display: none;">
-                        <option value="default" selected>Set Jailbreak</option>
-                        <option value="gpt-math-1.0">math 1.0</option>
-                        <option value="gpt-dude-1.0">dude 1.0</option>
-                        <option value="gpt-dan-1.0">dan 1.0</option>
-                        <option value="gpt-dan-2.0">dan 2.0</option>
-                        <option value="gpt-dev-2.0">dev 2.0</option>
-                        <option value="gpt-evil-1.0">evil 1.0</option>
+                    <select name="provider" id="provider">
+                        <option value="">Provider: Auto</option>
+                        <option value="Bing">Bing</option>
+                        <option value="OpenaiChat">OpenaiChat</option>
+                        <option value="Gemini">Gemini</option>
+                        <option value="Liaobots">Liaobots</option>
+                        <option value="You">You</option>
+                        <option value="">----</option>
                     </select>
-                    <div class="field">
-                        <select name="provider" id="provider">
-                            <option value="">Provider: Auto</option>
-                            <option value="Bing">Bing</option>
-                            <option value="OpenaiChat">OpenaiChat</option>
-                            <option value="Gemini">Gemini</option>
-                            <option value="Liaobots">Liaobots</option>
-                            <option value="You">You</option>
-                            <option value="">----</option>
-                        </select>
-                    </div>
-                </div>
-                <div class="field">
-                    <input type="checkbox" id="switch" />
-                    <label for="switch" title="Add the pages of the first 5 search results to the query."></label>
-                    <span class="about">Web Access</span>
-                </div>
-                <!--
-                <div class="field">
-                    <input type="checkbox" id="patch" />
-                    <label for="patch" title="Enable create images with Bing."></label>
-                    <span class="about">Image Generator</span>
-                </div>
-                -->
-                <div class="field">
-                    <input type="checkbox" id="history" />
-                    <label for="history" title="To improve the reaction time or if you have trouble with large conversations."></label>
-                    <span class="about">Disable History</span>
                 </div>
             </div>
         </div>
     </div>
     <div class="mobile-sidebar">
         <i class="fa-solid fa-bars"></i>
     </div>
```

#### html2text {}

```diff
@@ -1,12 +1,16 @@
 New Conversation
+Open Settings
+discord ~ _d_i_s_c_o_r_d_._g_g_/_X_f_y_b_z_P_X_P_H_5
+github ~ _@_x_t_e_k_k_y_/_g_p_t_4_f_r_e_e
+Web Access??
+Disable History??
+Hide System prompt??
+Auto continue
+Input max. grow height[Unknown INPUT type]
+Speech recognition lang[                    ]
 Clear Conversations Export Conversations
-github ~ _@_g_p_t_4_f_r_e_e
-OpenaiChat: Auto continue
  
 Stop Generating
 Regenerate
 [File][File][File]
-[One of: Set Jailbreak/math 1.0/dude 1.0/dan 1.0/dan 2.0/dev 2.0/evil 1.0]
 [One of: Provider: Auto/Bing/OpenaiChat/Gemini/Liaobots/You/----]
-??Web Access
-??Disable History
```

### Comparing `g4f-0.2.8.2/g4f/gui/client/static/css/style.css` & `g4f-0.2.9.0/g4f/gui/client/static/css/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -80,42 +80,40 @@
 html,
 body {
     scroll-behavior: smooth;
     overflow: hidden;
 }
 
 body {
-    padding: var(--section-gap);
+    padding: 10px;
     background: var(--colour-1);
     color: var(--colour-3);
     height: 100vh;
+    max-width: 1600px;
+    margin: auto;
 }
 
 .row {
     display: flex;
-    gap: var(--section-gap);
+    gap: 10px;
     height: 100%;
 }
 
 .box {
     backdrop-filter: blur(20px);
     -webkit-backdrop-filter: blur(20px);
     background-color: var(--blur-bg);
     height: 100%;
     width: 100%;
     border-radius: var(--border-radius-1);
     border: 1px solid var(--blur-border);
 }
 
-.hidden {
-    display: none;
-}
-
 .conversations {
-    max-width: 260px;
+    max-width: 280px;
     padding: var(--section-gap);
     overflow: auto;
     flex-shrink: 0;
     display: flex;
     flex-direction: column;
     justify-content: space-between;
 }
@@ -134,16 +132,15 @@
     flex-direction: column;
     overflow: auto;
     overflow-wrap: break-word;
     padding-bottom: 10px;
 }
 
 .conversation .user-input {
-    max-height: 200px;
-    margin-bottom: 10px;
+    margin-bottom: 4px;
 }
 
 .conversation .user-input input {
     font-size: 15px;
     width: 100%;
     height: 100%;
     padding: 12px 15px;
@@ -179,16 +176,16 @@
     transform: translateY(-50%);
     filter: blur(calc(0.5 * 70vw)) opacity(var(--opacity));
 }
 
 .conversations {
     display: flex;
     flex-direction: column;
-    gap: var(--inner-gap);
-    padding: var(--inner-gap);
+    gap: 10px;
+    padding: 10px;
 }
 
 .conversations .title {
     font-size: 14px;
     font-weight: 500;
 }
 
@@ -203,36 +200,45 @@
     border-radius: var(--border-radius-1);
 }
 
 .conversations .convo .left {
     cursor: pointer;
     display: flex;
     align-items: center;
-    gap: 10px;
+    gap: 4px;
+}
+
+.conversations .convo .fa-trash {
+    position: absolute;
+    right: 8px;
 }
 
 .conversations .convo .choise {
     position: absolute;
     right: 8px;
     background-color: var(--blur-bg);
 }
 
-.conversations i {
+.conversations i, .bottom_buttons i {
     color: var(--conversations);
     cursor: pointer;
 }
 
 .convo-title {
     color: var(--colour-3);
     font-size: 14px;
     text-overflow: ellipsis;
     overflow: hidden; 
     white-space: nowrap;
 }
 
+.convo-title .datetime {
+    font-size: 10px;
+}
+
 .message {
     width: 100%;
     overflow-wrap: break-word;
     display: flex;
     gap: var(--section-gap);
     padding: var(--inner-gap) var(--section-gap);
     padding-bottom: 0;
@@ -305,14 +311,15 @@
     z-index: 10000;
 }
 
 .message .content {
     display: flex;
     flex-direction: column;
     gap: 10px;
+    flex-wrap: wrap;
 }
 
 .message .content,
 .message .content a:link,
 .message .content a:visited{
     font-size: 15px;
     line-height: 1.3;
@@ -322,14 +329,18 @@
     white-space: pre-wrap;
 }
 
 .message .content img{
     max-width: 400px;
 }
 
+.message .content .audio{
+    display: flex;
+}
+
 .message .user i {
     position: absolute;
     bottom: -6px;
     right: -6px;
     z-index: 1000;
 }
 
@@ -347,18 +358,36 @@
     top: -2px;
     left: 0px;
     z-index: 1000;
     display: none;
     cursor: pointer;
 }
 
+.message .count .fa-clipboard,
+.message .count .fa-volume-high {
+    z-index: 1000;
+    cursor: pointer;
+}
+
 .message .user .fa-xmark {
     color: var(--colour-1);
 }
 
+.message .count .fa-clipboard {
+    color: var(--colour-3);
+}
+
+.message .count .fa-clipboard.clicked {
+    color: var(--accent);
+}
+
+.message .count .fa-volume-high.active {
+    color: var(--accent);
+}
+
 .message .assistant:hover .fa-xmark,
 .message .user:hover .fa-xmark {
     display: block;
 }
 
 .message .content .provider a,
 .message .content .provider {
@@ -478,35 +507,38 @@
     display: none;
 }
 
 #image, #file, #camera {
     display: none;
 }
 
-.file-label {
+.file-label,
+.micro-label {
     cursor: pointer;
     position: absolute;
     top: 10px;
     left: 10px;
 }
 
 .file-label:has(> input:valid),
-.file-label.selected {
+.file-label.selected,
+.micro-label.recognition {
     color: var(--accent);
 }
 
 label[for="image"] {
     top: 32px;
 }
 
-label[for="camera"] {
+label[for="micro"] {
     top: 54px;
 }
 
 label[for="camera"] {
+    top: 74px;
     display: none;
 }
 
 @media (pointer:none), (pointer:coarse) {
     label[for="camera"] {
         display: block;
     }
@@ -552,23 +584,34 @@
 }
 
 .buttons input:checked+label,
 .settings input:checked+label {
     background: var(--accent);
 }
 
+.settings .bottom_buttons {
+    flex-direction: row;
+}
+
+.settings .bottom_buttons button {
+    display: inline-block;
+    max-width: 210px;
+    width: 100%;
+}
+
 .buttons input:checked+label:after {
     left: calc(100% - 5px - 20px);
 }
 
 .buttons {
     display: flex;
     align-items: center;
     justify-content: left;
     width: 100%;
+    margin-bottom: 4px;
 }
 
 .field {
     height: fit-content;
     display: flex;
     align-items: center;
     gap: var(--inner-gap);
@@ -631,14 +674,15 @@
 }
 
 .bottom_buttons {
     width: 100%;
     display: flex;
     flex-direction: column;
     gap: 10px;
+    margin: 4px 0;
 }
 
 .bottom_buttons button {
     padding: 8px 12px;
     display: flex;
     gap: 18px;
     align-items: center;
@@ -803,15 +847,15 @@
     padding: 12px var(--inner-gap);
     background: none;
     border: none;
     outline: none;
     color: var(--colour-3);
 
     resize: vertical;
-    max-height: 150px;
+    max-height: 200px;
     min-height: 80px;
 }
 
 /* style for hljs copy */
 .hljs-copy-wrapper {
     position: relative;
     overflow: hidden
@@ -1022,27 +1066,47 @@
     outline: none;
     padding: var(--inner-gap) var(--section-gap);
     resize: vertical;
 }
 
 .settings {
     width: 100%;
-    display: none;
+    min-width: 700px;
+    display: flex;
+    flex-direction: column;
+}
+
+.settings .paper {
+    overflow: auto;
+    flex-direction: column;
 }
 
 .settings .field {
     margin: var(--inner-gap) 0;
 }
 
 .settings textarea {
     background-color: transparent;
     border: none;
     padding: var(--inner-gap) 0;
 }
 
+.settings input {
+    background-color: transparent;
+    padding: 2px;
+    border: none;
+    font-size: 15px;
+    width: 100%;
+    color: var(--colour-3);
+}
+
+.settings input:focus {
+    outline: none;
+}
+
 .settings .label {
     font-size: 15px;
     padding: var(--inner-gap) 0;
     width: fit-content;
     min-width: 190px;
     margin-left: var(--section-gap);
     white-space:nowrap;
@@ -1055,26 +1119,41 @@
     background: var(--colour-3);
 }
 ::-webkit-scrollbar-thumb {
     background: var(--blur-bg);
     border-radius: 5px;
 }
 ::-webkit-scrollbar-thumb:hover {
-    background: var(--accent)
+    background: var(--accent);
 }
 
 .hljs {
     color: #e9e9f4;
     background: #28293629;
     border-radius: var(--border-radius-1);
     border: 1px solid var(--blur-border);
     font-size: 15px;
 }
 
 #message-input {
     height: 82px;
     margin-left: 20px;
+    max-height: 200px;
 }
 
 #message-input::-webkit-scrollbar {
     width: 5px;
+}
+
+.hidden {
+    display: none;
+}
+
+.blink {
+    animation: blinker 1s step-start infinite;
+}
+
+@keyframes blinker {
+    50% {
+        opacity: 0;
+    }
 }
```

### Comparing `g4f-0.2.8.2/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.2.9.0/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.2.9.0/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.2.9.0/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.2.9.0/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/client/static/img/gpt.png` & `g4f-0.2.9.0/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/client/static/img/user.png` & `g4f-0.2.9.0/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.2.9.0/g4f/gui/client/static/js/chat.v1.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -6,26 +6,27 @@
 const regenerate = document.querySelector(`.regenerate`);
 const sidebar = document.querySelector(".conversations");
 const sidebar_button = document.querySelector(".mobile-sidebar");
 const sendButton = document.getElementById("send-button");
 const imageInput = document.getElementById("image");
 const cameraInput = document.getElementById("camera");
 const fileInput = document.getElementById("file");
+const microLabel = document.querySelector(".micro-label")
 const inputCount = document.getElementById("input-count")
 const providerSelect = document.getElementById("provider");
 const modelSelect = document.getElementById("model");
 const modelProvider = document.getElementById("model2");
 const systemPrompt = document.getElementById("systemPrompt")
-const jailbreak = document.getElementById("jailbreak");
+const settings = document.querySelector(".settings")
 
 let prompt_lock = false;
 
 let content, content_inner, content_count = null;
 
-const options = ["switch", "model", "model2", "jailbreak", "patch", "provider", "history"];
+const optionElements = document.querySelectorAll(".settings input, .settings textarea, #model, #model2, #provider")
 
 messageInput.addEventListener("blur", () => {
     window.scrollTo(0, 0);
 });
 
 messageInput.addEventListener("focus", () => {
     document.documentElement.scrollTop = document.documentElement.scrollHeight;
@@ -59,28 +60,109 @@
     typesetPromise = typesetPromise.then(
         () => MathJax.typesetPromise([container])
     ).catch(
         (err) => console.log('Typeset failed: ' + err.message)
     );
 }
 
-const register_remove_message = async () => {
+let stopped = false;
+const register_message_buttons = async () => {
     document.querySelectorAll(".message .fa-xmark").forEach(async (el) => {
         if (!("click" in el.dataset)) {
             el.dataset.click = "true";
             el.addEventListener("click", async () => {
                 if (prompt_lock) {
                     return;
                 }
                 const message_el = el.parentElement.parentElement;
                 await remove_message(window.conversation_id, message_el.dataset.index);
                 await load_conversation(window.conversation_id, false);
             })
         }
     });
+    document.querySelectorAll(".message .fa-clipboard").forEach(async (el) => {
+        if (!("click" in el.dataset)) {
+            el.dataset.click = "true";
+            el.addEventListener("click", async () => {
+                const message_el = el.parentElement.parentElement.parentElement;
+                const copyText = await get_message(window.conversation_id, message_el.dataset.index);
+                navigator.clipboard.writeText(copyText);
+                el.classList.add("clicked");
+                setTimeout(() => el.classList.remove("clicked"), 1000);
+            })
+        }
+    });
+    document.querySelectorAll(".message .fa-volume-high").forEach(async (el) => {
+        if (!("click" in el.dataset)) {
+            el.dataset.click = "true";
+            el.addEventListener("click", async () => {
+                if ("active" in el.classList || window.doSpeech) {
+                    stopped = true;
+                    return;
+                }
+                if (stopped) {
+                    stopped = false;
+                    return;
+                }
+                el.classList.add("blink")
+                el.classList.add("active")
+                const message_el = el.parentElement.parentElement.parentElement;
+                const content_el = el.parentElement.parentElement;
+                let speechText = await get_message(window.conversation_id, message_el.dataset.index);
+
+                speechText = speechText.replaceAll(/\[(.+)\]\(.+\)/gm, "($1)");
+                speechText = speechText.replaceAll("`", "").replaceAll("#", "")
+                speechText = speechText.replaceAll(
+                    /<!-- generated images start -->[\s\S]+<!-- generated images end -->/gm,
+                    ""
+                )
+
+                const lines = speechText.trim().split(/\n|\.|;/);
+                let ended = true;
+                window.onSpeechResponse = (url) => {
+                    el.classList.remove("blink")
+                    if (url) {
+                        var sound = document.createElement('audio');
+                        sound.controls = 'controls';
+                        sound.src = url;
+                        sound.type = 'audio/wav';
+                        if (ended) {
+                            sound.autoplay = true;
+                        }
+                        sound.onended = function() {
+                            ended = true;
+                        };
+                        sound.onplay = function() {
+                            ended = false;
+                        };
+                        var container = document.createElement('div');
+                        container.classList.add("audio");
+                        container.appendChild(sound);
+                        content_el.appendChild(container);
+                    }
+                    if (lines.length < 1 || stopped) {
+                        el.classList.remove("active");
+                        return;
+                    }
+                    while (lines.length > 0) {
+                        let line = lines.shift();
+                        var reg = new RegExp('^[0-9]$');
+                        if (line && !reg.test(line)) {
+                            return handleGenerateSpeech(line);
+                        }
+                    }
+                    if (!line) {
+                        el.classList.remove("active")
+                    }
+                }
+                let line = lines.shift();
+                return handleGenerateSpeech(line);
+            });
+        }
+    });
 }
 
 const delete_conversations = async () => {
     for (let i = 0; i < appStorage.length; i++) {
         let key = appStorage.key(i);
         if (key.startsWith("conversation:")) {
             appStorage.removeItem(key);
@@ -128,15 +210,19 @@
                 <div class="content_inner">
                 ${markdown_render(message)}
                 ${imageInput.dataset.src
                     ? '<img src="' + imageInput.dataset.src + '" alt="Image upload">'
                     : ''
                 }
                 </div>
-                <div class="count">${count_words_and_tokens(message, get_selected_model())}</div>
+                <div class="count">
+                    ${count_words_and_tokens(message, get_selected_model())}
+                    <i class="fa-solid fa-volume-high"></i>
+                    <i class="fa-regular fa-clipboard"></i>
+                </div>
             </div>
         </div>
     `;
     highlight(message_box);
     await ask_gpt();
 };
 
@@ -304,23 +390,30 @@
     content_count = content.querySelector('.count');
 
     message_box.scrollTop = message_box.scrollHeight;
     window.scrollTo(0, 0);
     try {
         const input = imageInput && imageInput.files.length > 0 ? imageInput : cameraInput;
         const file = input && input.files.length > 0 ? input.files[0] : null;
+        const provider = providerSelect.options[providerSelect.selectedIndex].value;
+        const auto_continue = document.getElementById("auto_continue")?.checked;
+        if (file && !provider)
+            provider = "Bing";
+        let api_key = null;
+        if (provider)
+            api_key = document.getElementById(`${provider}-api_key`)?.value;
         await api("conversation", {
             id: window.token,
             conversation_id: window.conversation_id,
             model: get_selected_model(),
-            jailbreak: jailbreak?.options[jailbreak.selectedIndex].value,
             web_search: document.getElementById("switch").checked,
-            provider: providerSelect.options[providerSelect.selectedIndex].value,
-            patch_provider: document.getElementById("patch")?.checked,
-            messages: messages
+            provider: provider,
+            messages: messages,
+            auto_continue: auto_continue,
+            api_key: api_key
         }, file);
         if (!error) {
             html = markdown_render(text);
             content_inner.innerHTML = html;
             highlight(content_inner);
 
             if (imageInput) imageInput.value = "";
@@ -340,15 +433,15 @@
     } else {
         let cursorDiv = document.getElementById("cursor");
         if (cursorDiv) cursorDiv.parentNode.removeChild(cursorDiv);
     }
     window.scrollTo(0, 0);
     message_box.scrollTop = message_box.scrollHeight;
     await remove_cancel_button();
-    await register_remove_message();
+    await register_message_buttons();
     prompt_lock = false;
     await load_conversations();
     regenerate.classList.remove("regenerate-hidden");
 };
 
 const clear_conversations = async () => {
     const elements = box_conversations.childNodes;
@@ -458,15 +551,19 @@
                         ? `<i class="fa-regular fa-phone-arrow-down-left"></i>`
                         : `<i class="fa-regular fa-phone-arrow-up-right"></i>`
                     }
                 </div>
                 <div class="content">
                     ${provider}
                     <div class="content_inner">${markdown_render(item.content)}</div>
-                    <div class="count">${count_words_and_tokens(item.content, next_provider?.model)}</div>
+                    <div class="count">
+                        ${count_words_and_tokens(item.content, next_provider?.model)}
+                        <i class="fa-solid fa-volume-high"></i>
+                        <i class="fa-regular fa-clipboard"></i>
+                    </div>
                 </div>
             </div>
         `;
     }
 
     const filtered = prepare_messages(messages, false);
     if (filtered.length > 0) {
@@ -474,16 +571,17 @@
         let count_total = GPTTokenizer_cl100k_base?.encodeChat(filtered, last_model).length
         if (count_total > 0) {
             elements += `<div class="count_total">(${count_total} tokens used)</div>`;
         }
     }
 
     message_box.innerHTML = elements;
-    register_remove_message();
+    register_message_buttons();
     highlight(message_box);
+    regenerate.classList.remove("regenerate-hidden");
 
     if (scroll) {
         message_box.scrollTo({
             top: message_box.scrollHeight,
             behavior: "smooth"
         });
 
@@ -497,14 +595,15 @@
     let conversation = await JSON.parse(
         appStorage.getItem(`conversation:${conversation_id}`)
     );
     return conversation;
 }
 
 async function save_conversation(conversation_id, conversation) {
+    conversation.updated = Date.now();
     appStorage.setItem(
         `conversation:${conversation_id}`,
         JSON.stringify(conversation)
     );
 }
 
 async function get_messages(conversation_id) {
@@ -519,29 +618,32 @@
         title = content + '&nbsp;'.repeat(19 - content.length)
     }
 
     if (appStorage.getItem(`conversation:${conversation_id}`) == null) {
         await save_conversation(conversation_id, {
             id: conversation_id,
             title: title,
+            added: Date.now(),
             system: systemPrompt?.value,
             items: [],
         });
     }
 
     history.pushState({}, null, `/chat/${conversation_id}`);
 }
 
 async function save_system_message() {
     if (!window.conversation_id) {
         return;
     }
     const conversation = await get_conversation(window.conversation_id);
-    conversation.system = systemPrompt?.value;
-    await save_conversation(window.conversation_id, conversation);
+    if (conversation) {
+        conversation.system = systemPrompt?.value;
+        await save_conversation(window.conversation_id, conversation);
+    }
 }
 
 const hide_last_message = async (conversation_id) => {
     const conversation = await get_conversation(conversation_id)
     const last_message = conversation.items.pop();
     if (last_message !== null) {
         if (last_message["role"] == "assistant") {
@@ -565,14 +667,20 @@
             new_items.push(conversation.items[i])
         }
     }
     conversation.items = new_items;
     await save_conversation(conversation_id, conversation);
 };
 
+const get_message = async (conversation_id, index) => {
+    const messages = await get_messages(conversation_id);
+    if (index in messages)
+        return messages[index]["content"];
+};
+
 const add_message = async (conversation_id, role, content, provider) => {
     const conversation = await get_conversation(conversation_id);
     conversation.items.push({
         role: role,
         content: content,
         provider: provider
     });
@@ -588,19 +696,29 @@
             conversations.push(JSON.parse(conversation));
         }
     }
 
     await clear_conversations();
 
     for (conversation of conversations) {
+        let updated = "";
+        if (conversation.updated) {
+            const date = new Date(conversation.updated);
+            updated = date.toLocaleString('en-GB', {
+                dateStyle: 'short',
+                timeStyle: 'short',
+                monthStyle: 'short'
+            });
+            updated = updated.replace("/" + date.getFullYear(), "")
+        }
         box_conversations.innerHTML += `
             <div class="convo" id="convo-${conversation.id}">
                 <div class="left" onclick="set_conversation('${conversation.id}')">
                     <i class="fa-regular fa-comments"></i>
-                    <span class="convo-title">${conversation.title}</span>
+                    <span class="convo-title"><span class="datetime">${updated}</span> ${conversation.title}</span>
                 </div>
                 <i onclick="show_option('${conversation.id}')" class="fa-regular fa-trash" id="conv-${conversation.id}"></i>
                 <div id="cho-${conversation.id}" class="choise" style="display:none;">
                     <i onclick="delete_conversation('${conversation.id}')" class="fa-regular fa-check"></i>
                     <i onclick="hide_option('${conversation.id}')" class="fa-regular fa-x"></i>
                 </div>
             </div>
@@ -644,67 +762,87 @@
 
     return BigInt(`0b${unix}${random_bytes}`).toString();
 };
 
 async function hide_sidebar() {
     sidebar.classList.remove("shown");
     sidebar_button.classList.remove("rotated");
-    if (window.location.pathname == "/menu/") {
+    settings.classList.add("hidden");
+    if (window.location.pathname == "/menu/" || window.location.pathname == "/settings/") {
         history.back();
     }
 }
 
 window.addEventListener('popstate', hide_sidebar, false);
 
 sidebar_button.addEventListener("click", (event) => {
+    settings.classList.add("hidden");
     if (sidebar.classList.contains("shown")) {
         hide_sidebar();
     } else {
         sidebar.classList.add("shown");
         sidebar_button.classList.add("rotated");
         history.pushState({}, null, "/menu/");
     }
     window.scrollTo(0, 0);
 });
 
+function open_settings() {
+    if (settings.classList.contains("hidden")) {
+        sidebar.classList.remove("shown");
+        settings.classList.remove("hidden");
+        history.pushState({}, null, "/settings/");
+    } else {
+        settings.classList.add("hidden");
+    }
+}
+
 const register_settings_storage = async () => {
-    options.forEach((id) => {
-        element = document.getElementById(id);
-        if (!element) {
-            return;
+    optionElements.forEach((element) => {
+        if (element.type == "textarea") {
+            element.addEventListener('input', async (event) => {
+                appStorage.setItem(element.id, element.value);
+            });
+        } else {
+            element.addEventListener('change', async (event) => {
+                switch (element.type) {
+                    case "checkbox":
+                        appStorage.setItem(element.id, element.checked);
+                        break;
+                    case "select-one":
+                        appStorage.setItem(element.id, element.selectedIndex);
+                        break;
+                    case "text":
+                        appStorage.setItem(element.id, element.value);
+                        break;
+                    default:
+                        console.warn("Unresolved element type");
+                }
+            });
         }
-        element.addEventListener('change', async (event) => {
-            switch (event.target.type) {
-                case "checkbox":
-                    appStorage.setItem(id, event.target.checked);
-                    break;
-                case "select-one":
-                    appStorage.setItem(id, event.target.selectedIndex);
-                    break;
-                default:
-                    console.warn("Unresolved element type");
-            }
-        });
     });
 }
 
 const load_settings_storage = async () => {
-    options.forEach((id) => {
-        element = document.getElementById(id);
-        if (!element || !(value = appStorage.getItem(id))) {
+    optionElements.forEach((element) => {
+        if (!(value = appStorage.getItem(element.id))) {
             return;
         }
         if (value) {
             switch (element.type) {
                 case "checkbox":
                     element.checked = value === "true";
                     break;
                 case "select-one":
                     element.selectedIndex = parseInt(value);
                     break;
+                case "text":
+                case "textarea":
+                    element.value = value;
+                    break;
                 default:
                     console.warn("Unresolved element type");
             }
         }
     });
 }
 
@@ -793,15 +931,15 @@
 };
 messageInput.addEventListener("keyup", count_input);
 systemPrompt.addEventListener("keyup", count_input);
 systemPrompt.addEventListener("focus", function() {
     countFocus = systemPrompt;
     count_input();
 });
-systemPrompt.addEventListener("blur", function() {
+systemPrompt.addEventListener("input", function() {
     countFocus = messageInput;
     count_input();
 });
 
 window.addEventListener('load', async function() {
     await on_load();
     if (window.conversation_id == "{{chat_id}}") {
@@ -861,14 +999,35 @@
         let option = document.createElement("option");
         option.value = option.text = provider;
         providerSelect.appendChild(option);
     })
 
     await load_provider_models(appStorage.getItem("provider"));
     await load_settings_storage()
+
+    const hide_systemPrompt = document.getElementById("hide-systemPrompt")
+    if (hide_systemPrompt.checked) {
+        systemPrompt.classList.add("hidden");
+    }
+    hide_systemPrompt.addEventListener('change', async (event) => {
+        if (event.target.checked) {
+            systemPrompt.classList.add("hidden");
+        } else {
+            systemPrompt.classList.remove("hidden");
+        }
+    });
+    const messageInputHeight = document.getElementById("message-input-height");
+    if (messageInputHeight) {
+        if (messageInputHeight.value) {
+            messageInput.style.maxHeight = `${messageInputHeight.value}px`;
+        }
+        messageInputHeight.addEventListener('change', async () => {
+            messageInput.style.maxHeight = `${messageInputHeight.value}px`;
+        });
+    }
 }
 
 async function load_version() {
     const versions = await api("version");
     document.title = 'g4f - ' + versions["version"];
     let text = "version ~ "
     if (versions["version"] != versions["latest_version"]) {
@@ -877,15 +1036,15 @@
         text += `<a href="${release_url}" target="_blank" title="${title}">${versions["version"]}</a> `;
         text += `<i class="fa-solid fa-rotate"></i>`
     } else {
         text += versions["version"];
     }
     document.getElementById("version_text").innerHTML = text
 }
-setTimeout(load_version, 5000);
+setTimeout(load_version, 2000);
 
 for (const el of [imageInput, cameraInput]) {
     el.addEventListener('click', async () => {
         el.value = '';
         if (imageInput.dataset.src) {
             URL.revokeObjectURL(imageInput.dataset.src);
             delete imageInput.dataset.src
@@ -930,15 +1089,15 @@
         });
         reader.readAsText(fileInput.files[0]);
     } else {
         delete fileInput.dataset.text;
     }
 });
 
-systemPrompt?.addEventListener("blur", async () => {
+systemPrompt?.addEventListener("input", async () => {
     await save_system_message();
 });
 
 function get_selected_model() {
     if (modelProvider.selectedIndex >= 0) {
         return modelProvider.options[modelProvider.selectedIndex].value;
     } else if (modelSelect.selectedIndex >= 0) {
@@ -1044,26 +1203,90 @@
         }
     };
     for (let i = 0; i < appStorage.length; i++) {
         let key = appStorage.key(i);
         let item = appStorage.getItem(key);
         if (key.startsWith("conversation:")) {
             data[key] = JSON.parse(item);
-        } else {
+        } else if (!key.includes("api_key")) {
             data["options"][key] = item;
         }
     }
     data = JSON.stringify(data, null, 4);
     const blob = new Blob([data], {
-        type: 'text/csv'
+        type: 'application/json'
     });
     if (window.navigator.msSaveOrOpenBlob) {
         window.navigator.msSaveBlob(blob, filename);
     } else {
         const elem = window.document.createElement('a');
         elem.href = window.URL.createObjectURL(blob);
         elem.download = filename;
         document.body.appendChild(elem);
         elem.click();
         document.body.removeChild(elem);
     }
+}
+
+const SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;
+if (SpeechRecognition) {
+    const mircoIcon = microLabel.querySelector("i");
+    mircoIcon.classList.add("fa-microphone");
+    mircoIcon.classList.remove("fa-microphone-slash");
+
+    const recognition = new SpeechRecognition();
+    recognition.continuous = true;
+    recognition.interimResults = true;
+    recognition.maxAlternatives = 1;
+
+    function may_stop() {
+        if (microLabel.classList.contains("recognition")) {
+            recognition.stop();
+        }
+    }
+
+    let startValue;
+    let lastValue;
+    let timeoutHandle;
+    recognition.onstart = function() {
+        microLabel.classList.add("recognition");
+        startValue = messageInput.value;
+        lastValue = "";
+        timeoutHandle = window.setTimeout(may_stop, 8000);
+    };
+    recognition.onend = function() {
+        microLabel.classList.remove("recognition");
+    };
+    recognition.onresult = function(event) {
+        if (!event.results) {
+            return;
+        }
+        window.clearTimeout(timeoutHandle);
+        let newText;
+        Array.from(event.results).forEach((result) => {
+            newText = result[0].transcript;
+            if (newText && newText != lastValue) {
+                messageInput.value = `${startValue ? startValue+"\n" : ""}${newText.trim()}`;
+                if (result.isFinal) {
+                    lastValue = newText;
+                    startValue = messageInput.value;
+                    messageInput.focus();
+                }
+                messageInput.style.height = messageInput.scrollHeight + "px";
+                messageInput.scrollTop = messageInput.scrollHeight;
+            }
+        });
+        window.clearTimeout(timeoutHandle);
+        timeoutHandle = window.setTimeout(may_stop, newText ? 8000 : 5000);
+    };
+
+    microLabel.addEventListener("click", () => {
+        if (microLabel.classList.contains("recognition")) {
+            window.clearTimeout(timeoutHandle);
+            recognition.stop();
+        } else {
+            const lang = document.getElementById("recognition-language")?.value;
+            recognition.lang = lang || navigator.language;
+            recognition.start();
+        }
+    });
 }
```

### Comparing `g4f-0.2.8.2/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.2.9.0/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.2.9.0/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/client/static/js/icons.js` & `g4f-0.2.9.0/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/server/android_gallery.py` & `g4f-0.2.9.0/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/server/api.py` & `g4f-0.2.9.0/g4f/gui/server/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,34 +76,31 @@
 
         Reads the request and prepares the necessary arguments for handling 
         a chat completion request.
 
         Returns:
             dict: Arguments prepared for chat completion.
         """ 
-        provider = json_data.get('provider', None)
-        if "image" in kwargs and provider is None:
-            provider = "Bing"
-        if provider == 'OpenaiChat':
-            kwargs['auto_continue'] = True
-
+        model = json_data.get('model') or models.default
+        provider = json_data.get('provider')
         messages = json_data['messages']
+        api_key = json_data.get("api_key")
+        if api_key is not None:
+            kwargs["api_key"] = api_key
         if json_data.get('web_search'):
             if provider == "Bing":
                 kwargs['web_search'] = True
             else:
                 from .internet import get_search_message
                 messages[-1]["content"] = get_search_message(messages[-1]["content"])
 
         conversation_id = json_data.get("conversation_id")
         if conversation_id and provider in conversations and conversation_id in conversations[provider]:
             kwargs["conversation"] = conversations[provider][conversation_id]
 
-        model = json_data.get('model') or models.default
-
         return {
             "model": model,
             "provider": provider,
             "messages": messages,
             "stream": True,
             "ignore_stream": True,
             "return_conversation": True,
```

### Comparing `g4f-0.2.8.2/g4f/gui/server/backend.py` & `g4f-0.2.9.0/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/server/config.py` & `g4f-0.2.9.0/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/server/internet.py` & `g4f-0.2.9.0/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/gui/server/js_api.py` & `g4f-0.2.9.0/g4f/gui/server/js_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import logging
 import json
 import os.path
 from typing import Iterator
 from uuid import uuid4
 from functools import partial
 
 import webview
```

### Comparing `g4f-0.2.8.2/g4f/gui/webview.py` & `g4f-0.2.9.0/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/image.py` & `g4f-0.2.9.0/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/local/__init__.py` & `g4f-0.2.9.0/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/locals/models.py` & `g4f-0.2.9.0/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/locals/provider.py` & `g4f-0.2.9.0/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/models.py` & `g4f-0.2.9.0/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/providers/base_provider.py` & `g4f-0.2.9.0/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/providers/create_images.py` & `g4f-0.2.9.0/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/providers/helper.py` & `g4f-0.2.9.0/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/providers/retry_provider.py` & `g4f-0.2.9.0/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/providers/types.py` & `g4f-0.2.9.0/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/requests/__init__.py` & `g4f-0.2.9.0/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/requests/aiohttp.py` & `g4f-0.2.9.0/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/requests/curl_cffi.py` & `g4f-0.2.9.0/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/requests/defaults.py` & `g4f-0.2.9.0/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/requests/raise_for_status.py` & `g4f-0.2.9.0/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/stubs.py` & `g4f-0.2.9.0/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/typing.py` & `g4f-0.2.9.0/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/version.py` & `g4f-0.2.9.0/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f/webdriver.py` & `g4f-0.2.9.0/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/g4f.egg-info/PKG-INFO` & `g4f-0.2.9.0/g4f.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.8.2
+Version: 0.2.9.0
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -260,15 +260,16 @@
 ```
 
 
 [![Image with cat](/docs/cat.jpeg)](/docs/client.md)
 
 **Full Documentation for Python API**
 
-- New Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
+- New AsyncClient API from G4F: [/docs/async_client](/docs/async_client.md)
+- Client API like the OpenAI Python library: [/docs/client](/docs/async_client.md)
 - Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
 
 #### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.8.2 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.2.9.0 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -142,16 +142,17 @@
 g4f.client import Client client = Client() response =
 client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
-client.md) **Full Documentation for Python API** - New Client API like the
-OpenAI Python library: [/docs/client](/docs/client.md) - Legacy API with python
+client.md) **Full Documentation for Python API** - New AsyncClient API from
+G4F: [/docs/async_client](/docs/async_client.md) - Client API like the OpenAI
+Python library: [/docs/client](/docs/async_client.md) - Legacy API with python
 modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
 interface, type the following codes in python: ```python from g4f.gui import
 run_gui run_gui() ``` or execute the following command: ```bash python -
 m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
 Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
 interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
 Configuration #### Cookies You need cookies for BingCreateImages and the Gemini
```

### Comparing `g4f-0.2.8.2/g4f.egg-info/SOURCES.txt` & `g4f-0.2.9.0/g4f.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 g4f/Provider/ChatForAi.py
 g4f/Provider/Chatgpt4Online.py
 g4f/Provider/ChatgptAi.py
 g4f/Provider/ChatgptFree.py
 g4f/Provider/ChatgptNext.py
 g4f/Provider/ChatgptX.py
 g4f/Provider/DeepInfra.py
+g4f/Provider/DuckDuckGo.py
 g4f/Provider/FlowGpt.py
 g4f/Provider/FreeChatgpt.py
 g4f/Provider/FreeGpt.py
 g4f/Provider/GeminiPro.py
 g4f/Provider/GeminiProChat.py
 g4f/Provider/GigaChat.py
 g4f/Provider/GptTalkRu.py
@@ -41,14 +42,15 @@
 g4f/Provider/Koala.py
 g4f/Provider/Liaobots.py
 g4f/Provider/Llama2.py
 g4f/Provider/Local.py
 g4f/Provider/PerplexityLabs.py
 g4f/Provider/Pi.py
 g4f/Provider/Vercel.py
+g4f/Provider/WhiteRabbitNeo.py
 g4f/Provider/You.py
 g4f/Provider/__init__.py
 g4f/Provider/base_provider.py
 g4f/Provider/helper.py
 g4f/Provider/bing/__init__.py
 g4f/Provider/bing/conversation.py
 g4f/Provider/bing/create_images.py
@@ -164,14 +166,17 @@
 g4f/gui/client/static/img/gpt.png
 g4f/gui/client/static/img/site.webmanifest
 g4f/gui/client/static/img/user.png
 g4f/gui/client/static/js/chat.v1.js
 g4f/gui/client/static/js/highlight.min.js
 g4f/gui/client/static/js/highlightjs-copy.min.js
 g4f/gui/client/static/js/icons.js
+g4f/gui/client/static/js/text_to_speech/630.index.js
+g4f/gui/client/static/js/text_to_speech/900.index.js
+g4f/gui/client/static/js/text_to_speech/index.js
 g4f/gui/server/__init__.py
 g4f/gui/server/android_gallery.py
 g4f/gui/server/api.py
 g4f/gui/server/app.py
 g4f/gui/server/backend.py
 g4f/gui/server/config.py
 g4f/gui/server/internet.py
```

### Comparing `g4f-0.2.8.2/g4f.egg-info/requires.txt` & `g4f-0.2.9.0/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.2/setup.py` & `g4f-0.2.9.0/setup.py`

 * *Files identical despite different names*

