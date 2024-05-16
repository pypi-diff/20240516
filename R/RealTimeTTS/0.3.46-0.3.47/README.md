# Comparing `tmp/RealTimeTTS-0.3.46.tar.gz` & `tmp/RealTimeTTS-0.3.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RealTimeTTS-0.3.46.tar", last modified: Mon May  6 13:47:38 2024, max compression
+gzip compressed data, was "RealTimeTTS-0.3.47.tar", last modified: Thu May 16 20:10:25 2024, max compression
```

## Comparing `RealTimeTTS-0.3.46.tar` & `RealTimeTTS-0.3.47.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:47:38.257563 RealTimeTTS-0.3.46/
--rw-rw-rw-   0        0        0    19946 2024-05-06 13:47:38.256563 RealTimeTTS-0.3.46/PKG-INFO
--rw-rw-rw-   0        0        0    18827 2024-05-06 13:46:11.000000 RealTimeTTS-0.3.46/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 13:47:38.255562 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/
--rw-rw-rw-   0        0        0    19946 2024-05-06 13:47:37.000000 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2024-05-06 13:47:37.000000 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:47:37.000000 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2024-05-06 13:47:37.000000 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-06 13:47:37.000000 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 13:47:37.600018 RealTimeTTS-0.3.46/RealtimeTTS/
--rw-rw-rw-   0        0        0      422 2023-12-28 10:50:12.000000 RealTimeTTS-0.3.46/RealtimeTTS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:47:38.251558 RealTimeTTS-0.3.46/RealtimeTTS/engines/
--rw-rw-rw-   0        0        0      397 2023-12-28 10:50:55.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/__init__.py
--rw-rw-rw-   0        0        0     9455 2024-04-12 11:47:00.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/azure_engine.py
--rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/base_engine.py
--rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/chinese.json
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/coqui_default_voice.json
--rw-rw-rw-   0        0        0    47582 2024-04-22 12:17:29.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/coqui_engine.py
--rw-rw-rw-   0        0        0    10595 2024-04-28 18:45:00.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/elevenlabs_engine.py
--rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/female.json
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/male.json
--rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/openai_engine.py
--rw-rw-rw-   0        0        0     5340 2024-04-11 20:41:30.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/system_engine.py
--rw-rw-rw-   0        0        0    10657 2024-05-06 13:40:39.000000 RealTimeTTS-0.3.46/RealtimeTTS/stream_player.py
--rw-rw-rw-   0        0        0    30141 2024-05-06 13:37:11.000000 RealTimeTTS-0.3.46/RealtimeTTS/text_to_stream.py
--rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.46/RealtimeTTS/threadsafe_generators.py
--rw-rw-rw-   0        0        0       42 2024-05-06 13:47:38.257563 RealTimeTTS-0.3.46/setup.cfg
--rw-rw-rw-   0        0        0     1295 2024-05-06 13:47:32.000000 RealTimeTTS-0.3.46/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:47:38.253560 RealTimeTTS-0.3.46/tests/
--rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.3.46/tests/test_callbacks.py
--rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.3.46/tests/test_on_audio_chunk_callback.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:10:25.013092 RealTimeTTS-0.3.47/
+-rw-rw-rw-   0        0        0    19978 2024-05-16 20:10:25.012091 RealTimeTTS-0.3.47/PKG-INFO
+-rw-rw-rw-   0        0        0    18860 2024-05-16 20:10:20.000000 RealTimeTTS-0.3.47/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 20:10:25.011089 RealTimeTTS-0.3.47/RealTimeTTS.egg-info/
+-rw-rw-rw-   0        0        0    19978 2024-05-16 20:10:24.000000 RealTimeTTS-0.3.47/RealTimeTTS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2024-05-16 20:10:24.000000 RealTimeTTS-0.3.47/RealTimeTTS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 20:10:24.000000 RealTimeTTS-0.3.47/RealTimeTTS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2024-05-16 20:10:24.000000 RealTimeTTS-0.3.47/RealTimeTTS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 20:10:24.000000 RealTimeTTS-0.3.47/RealTimeTTS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 20:10:24.995075 RealTimeTTS-0.3.47/RealtimeTTS/
+-rw-rw-rw-   0        0        0      422 2023-12-28 10:50:12.000000 RealTimeTTS-0.3.47/RealtimeTTS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:10:25.008086 RealTimeTTS-0.3.47/RealtimeTTS/engines/
+-rw-rw-rw-   0        0        0      397 2023-12-28 10:50:55.000000 RealTimeTTS-0.3.47/RealtimeTTS/engines/__init__.py
+-rw-rw-rw-   0        0        0     9413 2024-05-16 19:46:11.000000 RealTimeTTS-0.3.47/RealtimeTTS/engines/azure_engine.py
+-rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.47/RealtimeTTS/engines/base_engine.py
+-rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.47/RealtimeTTS/engines/chinese.json
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.47/RealtimeTTS/engines/coqui_default_voice.json
+-rw-rw-rw-   0        0        0    38627 2024-05-16 19:46:15.000000 RealTimeTTS-0.3.47/RealtimeTTS/engines/coqui_engine.py
+-rw-rw-rw-   0        0        0    10661 2024-05-16 20:09:01.000000 RealTimeTTS-0.3.47/RealtimeTTS/engines/elevenlabs_engine.py
+-rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.3.47/RealtimeTTS/engines/female.json
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.47/RealtimeTTS/engines/male.json
+-rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.3.47/RealtimeTTS/engines/openai_engine.py
+-rw-rw-rw-   0        0        0     4834 2024-05-16 19:46:19.000000 RealTimeTTS-0.3.47/RealtimeTTS/engines/system_engine.py
+-rw-rw-rw-   0        0        0    10657 2024-05-06 13:40:39.000000 RealTimeTTS-0.3.47/RealtimeTTS/stream_player.py
+-rw-rw-rw-   0        0        0    30141 2024-05-06 13:37:11.000000 RealTimeTTS-0.3.47/RealtimeTTS/text_to_stream.py
+-rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.47/RealtimeTTS/threadsafe_generators.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 20:10:25.013092 RealTimeTTS-0.3.47/setup.cfg
+-rw-rw-rw-   0        0        0     1295 2024-05-16 20:01:52.000000 RealTimeTTS-0.3.47/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:10:25.010088 RealTimeTTS-0.3.47/tests/
+-rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.3.47/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.3.47/tests/test_on_audio_chunk_callback.py
```

### Comparing `RealTimeTTS-0.3.46/PKG-INFO` & `RealTimeTTS-0.3.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.3.46
+Version: 0.3.47
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: PyAudio==0.2.14
 Requires-Dist: pyttsx3==2.90
 Requires-Dist: stream2sentence==0.2.3
 Requires-Dist: azure-cognitiveservices-speech==1.36.0
-Requires-Dist: elevenlabs==0.2.27
+Requires-Dist: elevenlabs==1.2.2
 Requires-Dist: TTS==0.22.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: pydub==0.25.1
 Requires-Dist: openai==1.13.3
 
 # RealtimeTTS
 
@@ -52,15 +52,15 @@
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.3.46
+Latest Version: v0.3.47 (switched to new elevenlabs api)
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
```

### Comparing `RealTimeTTS-0.3.46/README.md` & `RealTimeTTS-0.3.47/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.3.46
+Latest Version: v0.3.47 (switched to new elevenlabs api)
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
```

### Comparing `RealTimeTTS-0.3.46/RealTimeTTS.egg-info/PKG-INFO` & `RealTimeTTS-0.3.47/RealTimeTTS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.3.46
+Version: 0.3.47
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: PyAudio==0.2.14
 Requires-Dist: pyttsx3==2.90
 Requires-Dist: stream2sentence==0.2.3
 Requires-Dist: azure-cognitiveservices-speech==1.36.0
-Requires-Dist: elevenlabs==0.2.27
+Requires-Dist: elevenlabs==1.2.2
 Requires-Dist: TTS==0.22.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: pydub==0.25.1
 Requires-Dist: openai==1.13.3
 
 # RealtimeTTS
 
@@ -52,15 +52,15 @@
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.3.46
+Latest Version: v0.3.47 (switched to new elevenlabs api)
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
```

### Comparing `RealTimeTTS-0.3.46/RealTimeTTS.egg-info/SOURCES.txt` & `RealTimeTTS-0.3.47/RealTimeTTS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/engines/azure_engine.py` & `RealTimeTTS-0.3.47/RealtimeTTS/engines/azure_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,14 @@
     def set_voice(self, voice: Union[str, AzureVoice]):
         """
         Sets the voice to be used for speech synthesis.
 
         Args:
             voice (Union[str, AzureVoice]): The voice to be used for speech synthesis.
         """
-        print(f"Setting voice: {voice}")
         if isinstance(voice, AzureVoice):
             self.voice_name = voice.full_name
             self.language = self.voice_name[:5]
         else:
             installed_voices = self.get_voices()
             for installed_voice in installed_voices:
                 if voice in installed_voice.full_name:
```

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/engines/base_engine.py` & `RealTimeTTS-0.3.47/RealtimeTTS/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/engines/chinese.json` & `RealTimeTTS-0.3.47/RealtimeTTS/engines/chinese.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/engines/coqui_default_voice.json` & `RealTimeTTS-0.3.47/RealtimeTTS/engines/coqui_default_voice.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/engines/coqui_engine.py` & `RealTimeTTS-0.3.47/RealtimeTTS/engines/coqui_engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,16 +71,15 @@
                  use_mps=False,
                  use_deepspeed=False,
                  prepare_text_for_synthesis_callback=None,
                  add_sentence_filter=False,
                  pretrained=False,
                  comma_silence_duration=0.3,
                  sentence_silence_duration=0.6,
-                 default_silence_duration=0.3,
-                 delay_per_character=0,
+                 default_silence_duration=0.3
                  ):
         """
         Initializes a coqui voice realtime text to speech engine object.
 
         Args:
             model_name (str):
               Name of the coqui model to use.
@@ -156,15 +155,14 @@
         self.full_sentences = full_sentences
         self.use_mps = use_mps
         self.use_deepspeed = use_deepspeed
         self.add_sentence_filter = add_sentence_filter
         self.comma_silence_duration = comma_silence_duration
         self.sentence_silence_duration = sentence_silence_duration
         self.default_silence_duration = default_silence_duration
-        self.delay_per_character = delay_per_character
 
         self.cloning_reference_wav = voice
         self.speed = speed
         self.specific_model = specific_model
         if not local_models_path:
             local_models_path = os.environ.get("COQUI_MODEL_PATH")
             if local_models_path and len(local_models_path) > 0:
@@ -220,15 +218,14 @@
         self.output_worker_thread.start()
 
         self.main_synthesize_ready_event = mp.Event()
         self.parent_synthesize_pipe, child_synthesize_pipe = mp.Pipe()
         self.voices_list = []
         self.retrieve_coqui_voices()
 
-        log_level = logging.getLogger().getEffectiveLevel()
         self.synthesize_process = mp.Process(
             target=CoquiEngine._synthesize_worker, args=(
                 self.output_queue,
                 child_synthesize_pipe,
                 self.model_name,
                 self.cloning_reference_wav,
                 self.language,
@@ -249,17 +246,15 @@
                 self.model_path,
                 self.use_deepspeed,
                 self.voices_path,
                 self.voices_list,
                 self.pretrained,
                 self.comma_silence_duration,
                 self.sentence_silence_duration,
-                self.default_silence_duration,
-                self.delay_per_character,
-                log_level
+                self.default_silence_duration
             ))
         self.synthesize_process.start()
 
         logging.debug('Waiting for coqui model start')
         self.main_synthesize_ready_event.wait()
         logging.info('Coqui synthesis model ready')
 
@@ -290,31 +285,28 @@
             local_model_path,
             use_deepspeed,
             voices_path,
             predefined_voices,
             pretrained,
             comma_silence_duration,
             sentence_silence_duration,
-            default_silence_duration,
-            delay_per_character,
-            log_level):
+            default_silence_duration):
         """
         Worker process for the coqui text to speech synthesis model.
 
         Args:
             conn (multiprocessing.Connection):
               Connection to the parent process.
             model_name (str): Name of the coqui model to use.
             cloning_reference_wav (str):
               Name to the file containing the voice to clone.
             language (str): Language to use for the coqui model.
             ready_event (multiprocessing.Event):
               Event to signal when the model is ready.
         """
-        logging.basicConfig(level=log_level)
         sys.stdout = QueueWriter(output_queue)
 
         from TTS.utils.generic_utils import get_user_data_dir
         from TTS.config import load_config
         from TTS.tts.models import setup_model as setup_tts_model
         from TTS.tts.layers.xtts.xtts_manager import SpeakerManager
 
@@ -516,63 +508,36 @@
 
         ready_event.set()
 
         logging.info('Coqui text to speech synthesize model initialized successfully')
 
         try:
             while True:
-                try:
-                    message = conn.recv()
-                except EOFError:
-                    logging.error("EOFError caught, likely the parent process has closed the pipe", exc_info=True)
-                    break
-
+                message = conn.recv()  
                 command = message['command']
                 data = message['data']
 
                 if command == 'update_reference':
                     new_wav_path = data['cloning_reference_wav']
-                    logging.info(f'Updating reference WAV to {new_wav_path}')
+                    logging.info(f'Updating reference WAV to {new_wav_path}')                    
                     gpt_cond_latent, speaker_embedding = get_conditioning_latents(new_wav_path, tts)
-                    logging.debug("Sending message from worker process.")
                     conn.send(('success', 'Reference updated successfully'))
 
-                elif command == 'get_embeddings':
-                    new_wav_path = data['reference_wav']
-                    logging.info(f'Retrieving embedding for {new_wav_path}')
-                    try:
-                        gpt_cond_latent, speaker_embedding = tts.get_conditioning_latents(audio_path=new_wav_path, gpt_cond_len=30, max_ref_length=60)
-                        speaker_embedding = speaker_embedding.cpu().squeeze().half().tolist()
-                        logging.debug("Sending message from worker process.")
-                        conn.send(('success', speaker_embedding))
-                    except Exception as e:
-                        logging.debug("Sending message from worker process.")
-                        conn.send(('error', f'Could not retrieve embeddings, error: {e}'))
-
                 elif command == 'set_speed':
                     speed = data['speed']
-                    logging.debug("Sending message from worker process.")
                     conn.send(('success', 'Speed updated successfully'))
 
                 elif command == 'set_model':
                     checkpoint = data['checkpoint']
-                    try:
-                        logging.info(f'Updating model checkpoint to {checkpoint}')
-                        tts = load_model(checkpoint, tts)
-                    except Exception as e:
-                        logging.error("Error loading model", exc_info=True)
-                        logging.debug("Sending message from worker process.")
-                        conn.send(('error', f'Error updating model: {e}'))
-                    else:
-                        logging.debug("Sending message from worker process.")
-                        conn.send(('success', 'Model updated successfully'))
+                    logging.info(f'Updating model checkpoint to {checkpoint}')
+                    tts = load_model(checkpoint, tts)
+                    conn.send(('success', 'Model updated successfully'))
 
                 elif command == 'shutdown':
                     logging.info('Shutdown command received. Exiting worker process.')
-                    logging.debug("Sending message from worker process.")
                     conn.send(('shutdown', 'shutdown'))
                     break  # This exits the loop, effectively stopping the worker process.
 
                 elif command == 'synthesize':
 
                     text = data['text']
                     language = data['language']
@@ -582,228 +547,133 @@
                     print(f"XTTS Synthesizing: {text}")
                     time_start = time.time()
                     seconds_to_first_chunk = 0.0
                     full_generated_seconds = 0.0
                     raw_inference_start = 0.0
                     first_chunk_length_seconds = 0.0
 
-                    try:
-                        chunks = tts.inference_stream(
-                            text,
-                            language,
-                            gpt_cond_latent,
-                            speaker_embedding,
-                            stream_chunk_size=stream_chunk_size,
-                            overlap_wav_len=overlap_wav_len,
-                            temperature=temperature,
-                            length_penalty=length_penalty,
-                            repetition_penalty=repetition_penalty,
-                            top_k=top_k,
-                            top_p=top_p,
-                            speed=speed,
-                            enable_text_splitting=enable_text_splitting
-                        )
-                    except Exception as e:
-                        logging.error("Error perforing synthesis in tts.inference_stream", exc_info=True)
-                        logging.debug("Sending message from worker process.")
-                        conn.send(('error', f'Error during synthesis: {e}'))
-
-                    try:
-                        if full_sentences:
-                            chunklist = []
-
-                            for i, chunk in enumerate(chunks):
-                                chunk = postprocess_wave(chunk)
-                                chunk_bytes = chunk.tobytes()
-                                chunklist.append(chunk_bytes)
-                                chunk_duration = len(chunk_bytes) / (4 * 24000)
-                                full_generated_seconds += chunk_duration
-                                if i == 0:
-                                    first_chunk_length_seconds = chunk_duration
-                                    raw_inference_start = time.time()
-                                    seconds_to_first_chunk = raw_inference_start - time_start
-
-                            for chunk in chunklist:
-                                logging.debug("Sending message from worker process.")
-                                conn.send(('success', chunk))
-
-                        elif delay_per_character is not None and delay_per_character > 0:
-                            delayed_sent = False
-                            delay_time = delay_per_character * len(text)
-                            delay_time_end = time_start + delay_time
-
-                            chunklist = []
-
-                            print(f"Start time: {time_start}, delay_time: {delay_time}, delay_time_end: {delay_time_end}")
-
-                            for i, chunk in enumerate(chunks):
-                                
-                                delay_time_passed = time.time() > delay_time_end
-                                chunk = postprocess_wave(chunk)
-                                chunk_bytes = chunk.tobytes()
-                                chunk_duration = len(chunk_bytes) / (4 * 24000)
-                                full_generated_seconds += chunk_duration
-
-                                if i == 0:
-                                    first_chunk_length_seconds = chunk_duration
-                                    raw_inference_start = time.time()
-                                    seconds_to_first_chunk = raw_inference_start - time_start
-
-                                if delayed_sent:
-                                    logging.debug("Sending message from worker process.")
-                                    conn.send(('success', chunk_bytes))
-                                    continue
-
-                                chunklist.append(chunk_bytes)
-                                if delay_time_passed and not delayed_sent:
-                                    print(f"Delayed sending of {len(chunklist)} chunks")
-                                    delayed_sent = True
-                                    for chunk in chunklist:
-                                        logging.debug("Sending message from worker process.")
-                                        conn.send(('success', chunk))
-                                    chunklist = []
-
-                            if not delayed_sent:
-                                for chunk in chunklist:
-                                    logging.debug("Sending message from worker process.")
-                                    conn.send(('success', chunk))
+                    chunks = tts.inference_stream(
+                        text,
+                        language,
+                        gpt_cond_latent,
+                        speaker_embedding,
+                        stream_chunk_size=stream_chunk_size,
+                        overlap_wav_len=overlap_wav_len,
+                        temperature=temperature,
+                        length_penalty=length_penalty,
+                        repetition_penalty=repetition_penalty,
+                        top_k=top_k,
+                        top_p=top_p,
+                        speed=speed,
+                        enable_text_splitting=enable_text_splitting
+                    )
+
+                    if full_sentences:
+                        chunklist = []
+
+                        for i, chunk in enumerate(chunks):
+                            chunk = postprocess_wave(chunk)
+                            chunk_bytes = chunk.tobytes()
+                            chunklist.append(chunk_bytes)
+                            chunk_duration = len(chunk_bytes) / (4 * 24000)
+                            full_generated_seconds += chunk_duration
+                            if i == 0:
+                                first_chunk_length_seconds = chunk_duration
+                                raw_inference_start = time.time()
+                                seconds_to_first_chunk = raw_inference_start - time_start
+
+                        for i, chunk in enumerate(chunks):
+                            chunk = postprocess_wave(chunk)
+                            chunklist.append(chunk.tobytes())
 
-                        else:
-                            for i, chunk in enumerate(chunks):
-                                chunk = postprocess_wave(chunk)
-                                chunk_bytes = chunk.tobytes()
-                                logging.debug("Sending message from worker process.")
-                                conn.send(('success', chunk_bytes))
-                                chunk_duration = len(chunk_bytes) / (4 * 24000)  # 4 bytes per sample, 24000 Hz
-                                full_generated_seconds += chunk_duration
-                                if i == 0:
-                                    first_chunk_length_seconds = chunk_duration
-                                    raw_inference_start = time.time()
-                                    seconds_to_first_chunk = raw_inference_start - time_start
-                    except Exception as e:
-                        logging.error("Error processing and sending chunks during synthesis process ", exc_info=True)
-                        logging.debug("Sending message from worker process.")
-                        conn.send(('error', f'Error during synthesis: {e}'))
-
-                    try:
-
-                        time_end = time.time()
-                        seconds = time_end - time_start
-
-                        if full_generated_seconds > 0 and (full_generated_seconds - first_chunk_length_seconds) > 0:
-
-                            realtime_factor = seconds / full_generated_seconds
-                            raw_inference_time = seconds - seconds_to_first_chunk
-                            raw_inference_factor = raw_inference_time / (full_generated_seconds - first_chunk_length_seconds) 
-
-                            if realtime_factor > 1.0:
-                                desired_delay_seconds = seconds - full_generated_seconds
-                                desired_ratio = desired_delay_seconds / full_generated_seconds
-                                desired_delay_chars = desired_ratio * len(text)
-                                delay_per_character = desired_delay_seconds / desired_delay_chars
-
-                                print(f"desired_delay_seconds = {desired_delay_seconds} "
-                                    f"desired_ratio = {desired_ratio} "
-                                    f"desired_delay_chars = {desired_delay_chars} "
-                                    f"delay_per_character = {delay_per_character}")
-
-                                # len(text) in seconds synthesized
-                                # hat to be faster for (seconds - full_generated_seconds) seconds => this is our delay
-                                # delay = seconds - full_generated_seconds
-                                # wieviel characters entspricht das?
-                                # 
-                                # len_text = len(text)
-                                # duration = 
-
-                                print(f"Realtime factor: {realtime_factor:.2f}x, suggested delay_per_character: {delay_per_character:.2f}")
-                            # print(f"full_generated_seconds: {full_generated_seconds}, first_chunk_length_seconds: {first_chunk_length_seconds}")
-                            # print(f"raw_inferece_time: {raw_inference_time}")
-
-                            logging.info(
-                                f"XTTS synthesized {full_generated_seconds:.2f}s"
-                                f" audio in {seconds:.2f}s"
-                                f" realtime factor: {realtime_factor:.2f}x"
-                                f" seconds to first chunk: {seconds_to_first_chunk:.2f}s"
-                                f" raw_inference_factor: {raw_inference_factor:.2f}x"
-                            )
-                    except Exception as e:
-                        logging.error("Error calculating realtime factor", exc_info=True)
-
-                    try:
-
-                        # Send silent audio
-                        sample_rate = config.audio.sample_rate
-
-                        end_sentence_delimeters = ".!?…。¡¿"
-                        mid_sentence_delimeters = ";:,\n()[]{}-“”„”—/|《》"
-
-                        if text[-1] in end_sentence_delimeters:
-                            silence_duration = sentence_silence_duration
-                        elif text[-1] in mid_sentence_delimeters:
-                            silence_duration = comma_silence_duration
-                        else:
-                            silence_duration = default_silence_duration
+                        for chunk in chunklist:
+                            conn.send(('success', chunk))
+                    else:
+                        for i, chunk in enumerate(chunks):
+                            chunk = postprocess_wave(chunk)
+                            chunk_bytes = chunk.tobytes()
+                            conn.send(('success', chunk_bytes))
+                            chunk_duration = len(chunk_bytes) / (4 * 24000)  # 4 bytes per sample, 24000 Hz
+                            full_generated_seconds += chunk_duration
+                            if i == 0:
+                                first_chunk_length_seconds = chunk_duration
+                                raw_inference_start = time.time()
+                                seconds_to_first_chunk = raw_inference_start - time_start
+
+                    time_end = time.time()
+                    seconds = time_end - time_start
+
+                    if full_generated_seconds > 0 and (full_generated_seconds - first_chunk_length_seconds) > 0:
+
+                        realtime_factor = seconds / full_generated_seconds
+                        raw_inference_time = seconds - seconds_to_first_chunk
+                        raw_inference_factor = raw_inference_time / (full_generated_seconds - first_chunk_length_seconds) 
+
+                        # print(
+                        #     f"XTTS synthesized {full_generated_seconds:.2f}s"
+                        #     f" audio in {seconds:.2f}s"
+                        #     f" realtime factor: {realtime_factor:.2f}x"
+                        # )
+                        # print(
+                        #     f"seconds to first chunk: {seconds_to_first_chunk:.2f}s"
+                        #     f" raw_inference_factor: {raw_inference_factor:.2f}x"
+                        # )
+
+                    # Send silent audio
+                    sample_rate = config.audio.sample_rate
+
+                    end_sentence_delimeters = ".!?…。¡¿"
+                    mid_sentence_delimeters = ";:,\n()[]{}-“”„”—/|《》"
+
+                    if text[-1] in end_sentence_delimeters:
+                        silence_duration = sentence_silence_duration
+                    elif text[-1] in mid_sentence_delimeters:
+                        silence_duration = comma_silence_duration
+                    else:
+                        silence_duration = default_silence_duration
 
-                        silent_samples = int(sample_rate * silence_duration)
-                        silent_chunk = np.zeros(silent_samples, dtype=np.float32)
+                    silent_samples = int(sample_rate * silence_duration)
+                    silent_chunk = np.zeros(silent_samples, dtype=np.float32)
+                    conn.send(('success', silent_chunk.tobytes()))
 
-                        logging.debug("Sending message from worker process.")
-                        conn.send(('success', silent_chunk.tobytes()))
-                        logging.debug("Sending message from worker process.")
-                        conn.send(('finished', ''))
-
-                    except Exception as e:
-                        logging.error("Error sending silent chunk", exc_info=True)
-                        logging.debug("Sending message from worker process.")
-                        conn.send(('error', f'Error sending silent chunk: {e}'))
+                    conn.send(('finished', ''))
 
         except KeyboardInterrupt:
             logging.info("Keyboard interrupt received. "
                          "Exiting worker process.")
-            logging.debug("Sending message from worker process.")
             conn.send(('shutdown', 'shutdown'))
 
         except Exception as e:
-            logging.error("Caught an exception in _synthesize_worker", exc_info=True)
-            traceback_str = traceback.format_exc()
-            print(f"Traceback in _synthesize_worker: {traceback_str}")
-            try:
-                logging.debug("Sending message from worker process.")
-                conn.send(('error', str(e)))
-            except Exception as send_error:
-                logging.error("Failed to send error message to parent process", exc_info=True)
+            logging.error(f"General synthesis error: {e} occured in "
+                          "synthesize worker thread of coqui engine.")
+
+            tb_str = traceback.format_exc()
+            print(f"Traceback: {tb_str}")
+            print(f"Error: {e}")
+
+            conn.send(('error', str(e)))
 
         sys.stdout = sys.__stdout__
 
     def send_command(self, command, data):
         """
-        Send a command to the worker process, handling closed pipes.
+        Send a command to the worker process.
         """
-        try:
-            message = {'command': command, 'data': data}
-            logging.debug("Sending message to worker process.")
-            self.parent_synthesize_pipe.send(message)
-            return True
-        except BrokenPipeError:
-            logging.error("Failed to send command: pipe is closed.")
-            return False
-        except Exception as e:
-            logging.error(f"Failed to send command due to: {e}")
-            return False
+        message = {'command': command, 'data': data}
+        self.parent_synthesize_pipe.send(message)            
 
     def set_cloning_reference(self, cloning_reference_wav: str):
         """
         Send an 'update_reference' command and wait for a response.
         """
         if not isinstance(cloning_reference_wav, list):
             cloning_reference_wav = [cloning_reference_wav]        
         self.send_command('update_reference', {'cloning_reference_wav': cloning_reference_wav})
 
         # Wait for the response from the worker process
-        logging.debug("Receiving message from worker process.")
         status, result = self.parent_synthesize_pipe.recv()
         if status == 'success':
             logging.info('Reference WAV updated successfully')
         else:
             logging.error(f'Error updating reference WAV: {cloning_reference_wav}')
 
         return status, result
@@ -811,15 +681,14 @@
     def set_speed(self, speed: float):
         """
         Sets the speed of the speech synthesis.
         """
         self.send_command('set_speed', {'speed': speed})
 
         # Wait for the response from the worker process
-        logging.debug("Receiving message from worker process.")
         status, result = self.parent_synthesize_pipe.recv()
         if status == 'success':
             logging.info('Speed updated successfully')
         else:
             logging.error('Error updating speed')
 
         return status, result
@@ -917,25 +786,23 @@
 
             if len(text) < 1:
                 return
 
             data = {'text': text, 'language': self.language}
             self.send_command('synthesize', data)
 
-            logging.debug("Receiving message from worker process.")
             status, result = self.parent_synthesize_pipe.recv()
 
             while not 'finished' in status:
                 if 'shutdown' in status or 'error' in status:
-                    logging.error(f'Error synthesizing text: {text}')
-                    logging.error(f'Error: {result}')
+                    if 'error' in status:
+                        logging.error(f'Error synthesizing text: {text}')
+                        logging.error(f'Error: {result}')
                     return False
                 self.queue.put(result)
-                
-                logging.debug("Receiving message from worker process.")
                 status, result = self.parent_synthesize_pipe.recv()
 
             return True
 
     @staticmethod
     def download_file(url, destination):
         response = requests.get(url, stream=True)
@@ -978,30 +845,14 @@
                 CoquiEngine.download_file(url, file_path)
                 logging.info(f"{file_name} downloaded successfully.")
             else:
                 logging.info(f"{file_name} exists in {file_path} (no download).")
 
         return model_folder
 
-    def get_embeddings(self, path_to_wave):
-        """
-        Gets speaker embeddings for the given wave file.        
-        """
-        self.send_command('get_embeddings', {'reference_wav': path_to_wave})
-
-        # Wait for the response from the worker process
-        logging.debug("Receiving message from worker process.")
-        status, result = self.parent_synthesize_pipe.recv()
-        if status == 'success':
-            logging.info('Retrieved embedding successfully')
-        else:
-            logging.error(f'Error retrieving embedding for: {path_to_wave}')
-
-        return result
-
     def get_voices(self):
         """
         Retrieves the installed voices available for the Coqui TTS engine.
         """
 
         voice_objects = []
         voices_appended = []
@@ -1061,15 +912,14 @@
         self.send_command('shutdown', {})
 
         self.output_queue.put("STOP")
         self.output_worker_thread.join()
 
         # Wait for the worker process to acknowledge the shutdown
         try:
-            logging.debug("Receiving message from worker process.")
             status, _ = self.parent_synthesize_pipe.recv()
             if 'shutdown' in status:
                 logging.info('Worker process acknowledged shutdown')
         except EOFError:
             # Pipe was closed, meaning the process is already down
             logging.warning('Worker process pipe was closed before shutdown acknowledgement')
```

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/engines/elevenlabs_engine.py` & `RealTimeTTS-0.3.47/RealtimeTTS/engines/elevenlabs_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from elevenlabs import voices, generate, stream
-from elevenlabs.api import Voice, VoiceSettings
-from typing import Iterator, Union, Optional
+from elevenlabs.client import ElevenLabs
+from elevenlabs import Voice, VoiceSettings, play
+from typing import Iterator, Union
 from .base_engine import BaseEngine
-import elevenlabs
 import subprocess
 import threading
 import logging
 import pyaudio
-import shutil
 
 class ElevenlabsVoice:
     def __init__(self, name, voice_id, category, description, labels):
         self.name = name
         self.voice_id = voice_id
         self.category = category
         self.description = description
@@ -56,16 +54,18 @@
         self.model = model
         self.pause_event = threading.Event()
         self.immediate_stop = threading.Event()
         self.on_audio_chunk = None
         self.muted = False
         self.on_playback_started = False
 
-        self.set_api_key(api_key)
-        
+        self.client = ElevenLabs(
+            api_key=api_key
+        )
+
     def post_init(self):
         """ Information that this engine can handle generators directly """ 
         self.can_consume_generators = True
         self.engine_name = "elevenlabs"
 
     def get_stream_info(self):
         """
@@ -104,25 +104,27 @@
         Args:
             text (str): Text to synthesize.
         """
         
         self.on_playback_started = False
         self.immediate_stop.clear()
 
-        voice_object = Voice.from_id(self.id)
-        voice_object.settings = VoiceSettings(
-            stability=self.stability / 100,
-            similarity_boost=self.clarity / 100,
-            style=self.style_exxageration / 100,
-            use_speaker_boost=True
+        voice = Voice(
+            voice_id=self.id,
+            settings=VoiceSettings(
+                stability=self.stability / 100,
+                similarity_boost=self.clarity / 100,
+                style=self.style_exxageration / 100,
+                use_speaker_boost=True
+            )
         )
 
-        self.audio_stream = generate(
+        self.audio_stream = self.client.generate(
             text=generator,
-            voice=voice_object,
+            voice=voice,
             model=self.model,
             stream=True
         )
 
         self.stream(self.audio_stream)
 
         return True
@@ -131,17 +133,18 @@
         """
         Sets the elevenlabs api key. 
 
         Args:
             api_key (str): Elevenlabs API key. (TTS API key)
         """
         self.api_key = api_key
-        if api_key: 
-            elevenlabs.set_api_key(api_key)
-
+        if api_key:
+            self.client = ElevenLabs(
+               api_key=api_key
+            )
 
     def stream(self, audio_stream: Iterator[bytes]) -> bytes:
         """
         Stream the audio data using the 'mpv' player.
 
         This method takes the audio_stream iterator, which contains bytes of audio data,
         and plays them using the 'mpv' player. The function will continuously feed the
@@ -213,16 +216,16 @@
             list[ElevenlabsVoice]: A list containing ElevenlabsVoice objects representing each available voice. 
                                 Each ElevenlabsVoice object encapsulates information such as the voice's name, 
                                 ID, category, description, and associated labels.
 
         Note:
             This method relies on the `voices()` function to obtain the raw voice data. Ensure that the 
             `voices()` function is accessible and functional before calling this method.
-        """        
-        fetched_voices = voices()
+        """
+        fetched_voices = self.client.voices.get_all()
 
         voice_objects = []
         for voice in fetched_voices:
             voice_object = ElevenlabsVoice(voice.name, voice.voice_id, voice.category, voice.description, voice.labels)
             voice_objects.append(voice_object)
         return voice_objects
```

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/engines/female.json` & `RealTimeTTS-0.3.47/RealtimeTTS/engines/female.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/engines/male.json` & `RealTimeTTS-0.3.47/RealtimeTTS/engines/male.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/engines/openai_engine.py` & `RealTimeTTS-0.3.47/RealtimeTTS/engines/openai_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/engines/system_engine.py` & `RealTimeTTS-0.3.47/RealtimeTTS/engines/system_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 from .base_engine import BaseEngine
 from pydub.utils import mediainfo
 from pydub import AudioSegment
 from typing import Union
-import subprocess
-import platform
 import tempfile
 import pyaudio
 import pyttsx3
 import wave
 import os
 
-IS_MAC = platform.system() == "Darwin"
-
-if IS_MAC:
-    SYNTHESIS_FILE = "system_speech_synthesis.aiff"
-    DEFAULT_VOICE = "Alex"
-else:
-    SYNTHESIS_FILE = "system_speech_synthesis.wav"
-    DEFAULT_VOICE = "Zira"
+SYNTHESIS_FILE = 'system_speech_synthesis.wav' 
 
 
 class SystemVoice:
     def __init__(self, name, id):
         self.name = name
         self.id = id
 
     def __repr__(self):
         return self.name
+        #return f"<Voice(name={self.name})>"
 
 
 class SystemEngine(BaseEngine):
 
     def __init__(self, 
-                 voice: str = DEFAULT_VOICE,
+                 voice: str = "Zira",
                  print_installed_voices: bool = False):
         """
         Initializes a system realtime text to speech engine object.
 
         Args:
             voice (str, optional): Voice name. Defaults to "Zira".
             print_installed_voices (bool, optional): Indicates if the list of installed voices should be printed. Defaults to False.
@@ -69,24 +61,16 @@
         """
         Synthesizes text to audio stream.
 
         Args:
             text (str): Text to synthesize.
         """
 
-        if IS_MAC:
-            # Output file path
-            output_file = SYNTHESIS_FILE
-
-            # Synthesize speech and save to file
-            subprocess.call(['say', '-v', self.voice, '-o', output_file, text])
-
-        else:
-            self.engine.save_to_file(text, self.file_path)
-            self.engine.runAndWait()
+        self.engine.save_to_file(text, self.file_path)
+        self.engine.runAndWait()
 
         # Get media info of the file
         info = mediainfo(self.file_path)
 
         # Check if the file format is AIFF and convert to WAV if necessary
         if info['format_name'] == 'aiff':
             audio = AudioSegment.from_file(self.file_path, format="aiff")
@@ -126,24 +110,22 @@
     def set_voice(self, voice: Union[str, SystemVoice]):
         """
         Sets the voice to be used for speech synthesis.
 
         Args:
             voice (Union[str, SystemVoice]): The voice to be used for speech synthesis.
         """
-        if not IS_MAC:
-            if isinstance(voice, SystemVoice):
-                self.engine.setProperty('voice', voice.id)            
-            else:
-                installed_voices = self.engine.getProperty('voices')
-                if not voice is None:
-                    for installed_voice in installed_voices:
-                        if voice in installed_voice.name:
-                            self.engine.setProperty('voice', installed_voice.id)
-        self.voice = voice
+        if isinstance(voice, SystemVoice):
+            self.engine.setProperty('voice', voice.id)            
+        else:
+            installed_voices = self.engine.getProperty('voices')
+            if not voice is None:
+                for installed_voice in installed_voices:
+                    if voice in installed_voice.name:
+                        self.engine.setProperty('voice', installed_voice.id)
 
     def set_voice_parameters(self, **voice_parameters):
         """
         Sets the voice parameters to be used for speech synthesis.
 
         Args:
             **voice_parameters: The voice parameters to be used for speech synthesis.
```

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/stream_player.py` & `RealTimeTTS-0.3.47/RealtimeTTS/stream_player.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/text_to_stream.py` & `RealTimeTTS-0.3.47/RealtimeTTS/text_to_stream.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.46/RealtimeTTS/threadsafe_generators.py` & `RealTimeTTS-0.3.47/RealtimeTTS/threadsafe_generators.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.46/setup.py` & `RealTimeTTS-0.3.47/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Read requirements.txt
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="RealTimeTTS",
-    version="0.3.46",
+    version="0.3.47",
     author="Kolja Beigel",
     author_email="kolja.beigel@web.de",
     description="*Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KoljaB/RealTimeTTS",
     packages=setuptools.find_packages(),
```

### Comparing `RealTimeTTS-0.3.46/tests/test_callbacks.py` & `RealTimeTTS-0.3.47/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.46/tests/test_on_audio_chunk_callback.py` & `RealTimeTTS-0.3.47/tests/test_on_audio_chunk_callback.py`

 * *Files identical despite different names*

