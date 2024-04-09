# Comparing `tmp/webscout-1.2.6.tar.gz` & `tmp/webscout-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.2.6.tar", last modified: Sun Apr  7 08:19:59 2024, max compression
+gzip compressed data, was "webscout-1.2.8.tar", last modified: Tue Apr  9 09:28:37 2024, max compression
```

## Comparing `webscout-1.2.6.tar` & `webscout-1.2.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 08:19:59.081478 webscout-1.2.6/
-drwxrwxrwx   0        0        0        0 2024-04-07 08:19:57.976422 webscout-1.2.6/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 08:19:58.019423 webscout-1.2.6/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-04-07 08:19:58.231903 webscout-1.2.6/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3846 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-04-07 08:19:58.303830 webscout-1.2.6/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     1754 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-04-02 10:54:23.000000 webscout-1.2.6/LICENSE.md
--rw-rw-rw-   0        0        0    24247 2024-04-07 08:19:59.063517 webscout-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    22072 2024-04-07 08:14:49.000000 webscout-1.2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 08:19:59.082479 webscout-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     2790 2024-04-07 06:24:18.000000 webscout-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 08:19:58.966784 webscout-1.2.6/webscout/
--rw-rw-rw-   0        0        0    57985 2024-04-06 15:11:56.000000 webscout-1.2.6/webscout/AI.py
--rw-rw-rw-   0        0        0     2343 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/AIbase.py
--rw-rw-rw-   0        0        0    24123 2024-04-03 10:06:49.000000 webscout-1.2.6/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     8103 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/HelpingAI.py
--rw-rw-rw-   0        0        0     3309 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/LLM.py
--rw-rw-rw-   0        0        0      547 2024-04-07 06:11:57.000000 webscout-1.2.6/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-03 10:30:01.000000 webscout-1.2.6/webscout/__main__.py
--rw-rw-rw-   0        0        0    17059 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/cli.py
--rw-rw-rw-   0        0        0      276 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/exceptions.py
--rw-rw-rw-   0        0        0      692 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/models.py
--rw-rw-rw-   0        0        0    20232 2024-04-07 08:02:09.000000 webscout-1.2.6/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2605 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-04-07 07:49:31.000000 webscout-1.2.6/webscout/version.py
--rw-rw-rw-   0        0        0     3085 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-04-07 08:19:59.056465 webscout-1.2.6/webscout.egg-info/
--rw-rw-rw-   0        0        0    24247 2024-04-07 08:19:56.000000 webscout-1.2.6/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      965 2024-04-07 08:19:57.000000 webscout-1.2.6/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 08:19:56.000000 webscout-1.2.6/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-04-07 08:19:56.000000 webscout-1.2.6/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      334 2024-04-07 08:19:56.000000 webscout-1.2.6/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-07 08:19:56.000000 webscout-1.2.6/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.824119 webscout-1.2.8/
+drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.213994 webscout-1.2.8/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.257495 webscout-1.2.8/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.309498 webscout-1.2.8/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3846 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.349494 webscout-1.2.8/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     1754 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-02 10:54:23.000000 webscout-1.2.8/LICENSE.md
+-rw-rw-rw-   0        0        0    24645 2024-04-09 09:28:37.824119 webscout-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    22470 2024-04-09 09:23:09.000000 webscout-1.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 09:28:37.824119 webscout-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     2817 2024-04-09 09:25:42.000000 webscout-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.665109 webscout-1.2.8/webscout/
+-rw-rw-rw-   0        0        0    57985 2024-04-06 15:11:56.000000 webscout-1.2.8/webscout/AI.py
+-rw-rw-rw-   0        0        0     2343 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    24123 2024-04-03 10:06:49.000000 webscout-1.2.8/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     8103 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/HelpingAI.py
+-rw-rw-rw-   0        0        0     3309 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/LLM.py
+-rw-rw-rw-   0        0        0      547 2024-04-07 06:11:57.000000 webscout-1.2.8/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-03 10:30:01.000000 webscout-1.2.8/webscout/__main__.py
+-rw-rw-rw-   0        0        0    17059 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/cli.py
+-rw-rw-rw-   0        0        0      276 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/exceptions.py
+-rw-rw-rw-   0        0        0      692 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/models.py
+-rw-rw-rw-   0        0        0    20140 2024-04-09 09:21:35.000000 webscout-1.2.8/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2605 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-04-09 09:19:36.000000 webscout-1.2.8/webscout/version.py
+-rw-rw-rw-   0        0        0     3085 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.801562 webscout-1.2.8/webscout.egg-info/
+-rw-rw-rw-   0        0        0    24645 2024-04-09 09:28:35.000000 webscout-1.2.8/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      965 2024-04-09 09:28:36.000000 webscout-1.2.8/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 09:28:35.000000 webscout-1.2.8/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-04-09 09:28:35.000000 webscout-1.2.8/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      334 2024-04-09 09:28:35.000000 webscout-1.2.8/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-09 09:28:35.000000 webscout-1.2.8/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.2.6/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.2.8/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.2.8/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/DeepWEBS/networks/filepath_converter.py` & `webscout-1.2.8/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/DeepWEBS/networks/google_searcher.py` & `webscout-1.2.8/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/DeepWEBS/networks/network_configs.py` & `webscout-1.2.8/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.2.8/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/DeepWEBS/utilsdw/enver.py` & `webscout-1.2.8/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/DeepWEBS/utilsdw/logger.py` & `webscout-1.2.8/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/LICENSE.md` & `webscout-1.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/PKG-INFO` & `webscout-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.2.6
+Version: 1.2.8
 Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -225,25 +225,31 @@
 from webscout import transcriber
 
 def extract_transcript(video_id):
     """Extracts the transcript from a YouTube video."""
     try:
         transcript_list = transcriber.list_transcripts(video_id)
         for transcript in transcript_list:
-            transcript_text_list = transcript.fetch()
+            transcript_data_list = transcript.fetch()
             lang = transcript.language
             transcript_text = ""
             if transcript.language_code == 'en':
-                for line in transcript_text_list:
-                    transcript_text += " " + line["text"]
+                for line in transcript_data_list:
+                    start_time = line['start']
+                    end_time = start_time + line['duration']
+                    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+                    transcript_text += formatted_line
                 return transcript_text
             elif transcript.is_translatable:
                 english_transcript_list = transcript.translate('en').fetch()
                 for line in english_transcript_list:
-                    transcript_text += " " + line["text"]
+                    start_time = line['start']
+                    end_time = start_time + line['duration']
+                    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+                    transcript_text += formatted_line
                 return transcript_text
         print("Transcript extraction failed. Please check the video URL.")
     except Exception as e:
         print(f"Error: {e}")
 
 def main():
     video_url = input("Enter the video link: ")
@@ -681,10 +687,10 @@
 from webscout.LLM import LLM
 
 def chat(model_name, system_message="You are Jarvis"):# system prompt
     AI = LLM(model_name, system_message)
     AI.chat()
 
 if __name__ == "__main__":
-    model_name = "mistralai/Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL text generation models on deepinfra.com.
+    model_name = "mistralai/Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL text generation models on deepinfra.com.
     chat(model_name)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.6 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.2.8 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and
 now can transcribe yt videos Author: OEvortex Author-email:
 helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
 URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
 Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
 github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
@@ -116,20 +116,24 @@
  for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
  States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
  To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
 tool that transcribes YouTube videos. Here's an example code demonstrating its
        usage: ```python import sys from webscout import transcriber def
     extract_transcript(video_id): """Extracts the transcript from a YouTube
   video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
-transcript in transcript_list: transcript_text_list = transcript.fetch() lang =
+transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
-for line in transcript_text_list: transcript_text += " " + line["text"] return
+    for line in transcript_data_list: start_time = line['start'] end_time =
+     start_time + line['duration'] formatted_line = f"{start_time:.2f} -
+  {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
-transcript_text += " " + line["text"] return transcript_text print("Transcript
+      start_time = line['start'] end_time = start_time + line['duration']
+    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+  transcript_text += formatted_line return transcript_text print("Transcript
  extraction failed. Please check the video URL.") except Exception as e: print
   (f"Error: {e}") def main(): video_url = input("Enter the video link: ") if
  video_url: video_id = video_url.split("=")[1] print("Video URL:", video_url)
 submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
         if submit == '': print("Extracting Transcript...") transcript =
    extract_transcript(video_id) print('Transcript:') print(transcript) print
 ("__________________________________________________________________________________")
@@ -271,9 +275,9 @@
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
  (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
        `LLM` ```python from webscout.LLM import LLM def chat(model_name,
      system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
  system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
- Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL
+ Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL
          text generation models on deepinfra.com. chat(model_name) ```
```

### Comparing `webscout-1.2.6/README.md` & `webscout-1.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -173,25 +173,31 @@
 from webscout import transcriber
 
 def extract_transcript(video_id):
     """Extracts the transcript from a YouTube video."""
     try:
         transcript_list = transcriber.list_transcripts(video_id)
         for transcript in transcript_list:
-            transcript_text_list = transcript.fetch()
+            transcript_data_list = transcript.fetch()
             lang = transcript.language
             transcript_text = ""
             if transcript.language_code == 'en':
-                for line in transcript_text_list:
-                    transcript_text += " " + line["text"]
+                for line in transcript_data_list:
+                    start_time = line['start']
+                    end_time = start_time + line['duration']
+                    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+                    transcript_text += formatted_line
                 return transcript_text
             elif transcript.is_translatable:
                 english_transcript_list = transcript.translate('en').fetch()
                 for line in english_transcript_list:
-                    transcript_text += " " + line["text"]
+                    start_time = line['start']
+                    end_time = start_time + line['duration']
+                    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+                    transcript_text += formatted_line
                 return transcript_text
         print("Transcript extraction failed. Please check the video URL.")
     except Exception as e:
         print(f"Error: {e}")
 
 def main():
     video_url = input("Enter the video link: ")
@@ -629,10 +635,10 @@
 from webscout.LLM import LLM
 
 def chat(model_name, system_message="You are Jarvis"):# system prompt
     AI = LLM(model_name, system_message)
     AI.chat()
 
 if __name__ == "__main__":
-    model_name = "mistralai/Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL text generation models on deepinfra.com.
+    model_name = "mistralai/Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL text generation models on deepinfra.com.
     chat(model_name)
 ```
```

#### html2text {}

```diff
@@ -88,20 +88,24 @@
  for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
  States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
  To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
 tool that transcribes YouTube videos. Here's an example code demonstrating its
        usage: ```python import sys from webscout import transcriber def
     extract_transcript(video_id): """Extracts the transcript from a YouTube
   video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
-transcript in transcript_list: transcript_text_list = transcript.fetch() lang =
+transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
-for line in transcript_text_list: transcript_text += " " + line["text"] return
+    for line in transcript_data_list: start_time = line['start'] end_time =
+     start_time + line['duration'] formatted_line = f"{start_time:.2f} -
+  {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
-transcript_text += " " + line["text"] return transcript_text print("Transcript
+      start_time = line['start'] end_time = start_time + line['duration']
+    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+  transcript_text += formatted_line return transcript_text print("Transcript
  extraction failed. Please check the video URL.") except Exception as e: print
   (f"Error: {e}") def main(): video_url = input("Enter the video link: ") if
  video_url: video_id = video_url.split("=")[1] print("Video URL:", video_url)
 submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
         if submit == '': print("Extracting Transcript...") transcript =
    extract_transcript(video_id) print('Transcript:') print(transcript) print
 ("__________________________________________________________________________________")
@@ -243,9 +247,9 @@
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
  (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
        `LLM` ```python from webscout.LLM import LLM def chat(model_name,
      system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
  system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
- Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL
+ Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL
          text generation models on deepinfra.com. chat(model_name) ```
```

### Comparing `webscout-1.2.6/setup.py` & `webscout-1.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
-version = None
-with open("webscout/version.py") as version_file:
-    exec(version_file.read())
+# version = None
+# with open("webscout/version.py") as version_file:
+#     exec(version_file.read())
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.2.6", 
+    version="1.2.8", 
     description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
@@ -50,14 +50,15 @@
         "pydantic",
         "requests",
         "sse_starlette",
         "termcolor",
         "tiktoken",
         "tldextract",
         "orjson",
+        # "appdirs"
     ],
     entry_points={
         "console_scripts": [
             "WEBS = webscout.cli:cli",
             "webscout-ai-phindsearch = webscout.AI:phindsearch",
             "webscout-ai-yepchat = webscout.AI:yepchat",
             "webscout-ai = webscout.AI:cli",
```

### Comparing `webscout-1.2.6/webscout/AI.py` & `webscout-1.2.8/webscout/AI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout/AIbase.py` & `webscout-1.2.8/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout/AIutel.py` & `webscout-1.2.8/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout/DWEBS.py` & `webscout-1.2.8/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout/HelpingAI.py` & `webscout-1.2.8/webscout/HelpingAI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout/LLM.py` & `webscout-1.2.8/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout/__init__.py` & `webscout-1.2.8/webscout/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout/cli.py` & `webscout-1.2.8/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout/models.py` & `webscout-1.2.8/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout/transcriber.py` & `webscout-1.2.8/webscout/transcriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     CAUSE_MESSAGE = ''
     GITHUB_REFERRAL = (
         '\n\nIf you are sure that the described cause is not responsible for this error '
         'and that a transcript should be retrievable, please create an issue at '
         'https://github.com/OE-LUCIFER/Webscout/issues. '
         'Please add which version of youtube_transcript_api you are using '
         'and provide the information needed to replicate the error. '
-        'Also make sure that there are no open issues which already describe your problem!'
     )
 
     def __init__(self, video_id):
         self.video_id = video_id
         super(TranscriptRetrievalError, self).__init__(self._build_error_message())
 
     def _build_error_message(self):
```

### Comparing `webscout-1.2.6/webscout/utils.py` & `webscout-1.2.8/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout/webscout_search.py` & `webscout-1.2.8/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout/webscout_search_async.py` & `webscout-1.2.8/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.6/webscout.egg-info/PKG-INFO` & `webscout-1.2.8/webscout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.2.6
+Version: 1.2.8
 Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -225,25 +225,31 @@
 from webscout import transcriber
 
 def extract_transcript(video_id):
     """Extracts the transcript from a YouTube video."""
     try:
         transcript_list = transcriber.list_transcripts(video_id)
         for transcript in transcript_list:
-            transcript_text_list = transcript.fetch()
+            transcript_data_list = transcript.fetch()
             lang = transcript.language
             transcript_text = ""
             if transcript.language_code == 'en':
-                for line in transcript_text_list:
-                    transcript_text += " " + line["text"]
+                for line in transcript_data_list:
+                    start_time = line['start']
+                    end_time = start_time + line['duration']
+                    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+                    transcript_text += formatted_line
                 return transcript_text
             elif transcript.is_translatable:
                 english_transcript_list = transcript.translate('en').fetch()
                 for line in english_transcript_list:
-                    transcript_text += " " + line["text"]
+                    start_time = line['start']
+                    end_time = start_time + line['duration']
+                    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+                    transcript_text += formatted_line
                 return transcript_text
         print("Transcript extraction failed. Please check the video URL.")
     except Exception as e:
         print(f"Error: {e}")
 
 def main():
     video_url = input("Enter the video link: ")
@@ -681,10 +687,10 @@
 from webscout.LLM import LLM
 
 def chat(model_name, system_message="You are Jarvis"):# system prompt
     AI = LLM(model_name, system_message)
     AI.chat()
 
 if __name__ == "__main__":
-    model_name = "mistralai/Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL text generation models on deepinfra.com.
+    model_name = "mistralai/Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL text generation models on deepinfra.com.
     chat(model_name)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.6 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.2.8 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and
 now can transcribe yt videos Author: OEvortex Author-email:
 helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
 URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
 Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
 github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
@@ -116,20 +116,24 @@
  for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
  States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
  To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
 tool that transcribes YouTube videos. Here's an example code demonstrating its
        usage: ```python import sys from webscout import transcriber def
     extract_transcript(video_id): """Extracts the transcript from a YouTube
   video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
-transcript in transcript_list: transcript_text_list = transcript.fetch() lang =
+transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
-for line in transcript_text_list: transcript_text += " " + line["text"] return
+    for line in transcript_data_list: start_time = line['start'] end_time =
+     start_time + line['duration'] formatted_line = f"{start_time:.2f} -
+  {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
-transcript_text += " " + line["text"] return transcript_text print("Transcript
+      start_time = line['start'] end_time = start_time + line['duration']
+    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+  transcript_text += formatted_line return transcript_text print("Transcript
  extraction failed. Please check the video URL.") except Exception as e: print
   (f"Error: {e}") def main(): video_url = input("Enter the video link: ") if
  video_url: video_id = video_url.split("=")[1] print("Video URL:", video_url)
 submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
         if submit == '': print("Extracting Transcript...") transcript =
    extract_transcript(video_id) print('Transcript:') print(transcript) print
 ("__________________________________________________________________________________")
@@ -271,9 +275,9 @@
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
  (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
        `LLM` ```python from webscout.LLM import LLM def chat(model_name,
      system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
  system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
- Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL
+ Mistral-7B-Instruct-v0.2" # name of the model you wish to use It supports ALL
          text generation models on deepinfra.com. chat(model_name) ```
```

### Comparing `webscout-1.2.6/webscout.egg-info/SOURCES.txt` & `webscout-1.2.8/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

