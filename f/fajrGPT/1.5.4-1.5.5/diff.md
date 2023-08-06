# Comparing `tmp/fajrGPT-1.5.4.tar.gz` & `tmp/fajrGPT-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.5.4.tar", last modified: Tue Aug  1 11:10:09 2023, max compression
+gzip compressed data, was "fajrGPT-1.5.5.tar", last modified: Sun Aug  6 21:26:25 2023, max compression
```

## Comparing `fajrGPT-1.5.4.tar` & `fajrGPT-1.5.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 11:10:09.794444 fajrGPT-1.5.4/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.5.4/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-08-01 11:10:09.794285 fajrGPT-1.5.4/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.5.4/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 11:10:09.791799 fajrGPT-1.5.4/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.5.4/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     4095 2023-07-31 02:16:34.000000 fajrGPT-1.5.4/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    22151 2023-08-01 11:08:56.000000 fajrGPT-1.5.4/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 11:10:09.794091 fajrGPT-1.5.4/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       68 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-08-01 11:10:09.794480 fajrGPT-1.5.4/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1165 2023-08-01 11:09:06.000000 fajrGPT-1.5.4/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-06 21:26:25.101393 fajrGPT-1.5.5/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.5.5/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-08-06 21:26:25.101218 fajrGPT-1.5.5/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.5.5/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-06 21:26:25.099649 fajrGPT-1.5.5/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.5.5/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     4095 2023-07-31 02:16:34.000000 fajrGPT-1.5.5/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    26175 2023-08-06 21:20:55.000000 fajrGPT-1.5.5/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-06 21:26:25.101015 fajrGPT-1.5.5/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-08-06 21:26:25.000000 fajrGPT-1.5.5/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-08-06 21:26:25.000000 fajrGPT-1.5.5/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-08-06 21:26:25.000000 fajrGPT-1.5.5/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-08-06 21:26:25.000000 fajrGPT-1.5.5/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       68 2023-08-06 21:26:25.000000 fajrGPT-1.5.5/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-08-06 21:26:25.000000 fajrGPT-1.5.5/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-08-06 21:26:25.101436 fajrGPT-1.5.5/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1165 2023-08-06 21:24:47.000000 fajrGPT-1.5.5/setup.py
```

### Comparing `fajrGPT-1.5.4/LICENSE` & `fajrGPT-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5.4/PKG-INFO` & `fajrGPT-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.5.4
+Version: 1.5.5
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.5.4/README.md` & `fajrGPT-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5.4/fajrGPT/quran_metadata.py` & `fajrGPT-1.5.5/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5.4/fajrGPT/wake.py` & `fajrGPT-1.5.5/fajrGPT/wake.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,94 +6,149 @@
 import numpy as np
 import time
 import subprocess
 import requests
 import openai
 import random
 import tempfile
+import queue
 import mutagen.mp3 as mp3
 from tqdm import tqdm
 from Quran_Module import Project_Quran
 from scipy.signal import butter, lfilter
 from pydub import AudioSegment
 from threading import Thread
 from fajrGPT.quran_metadata import quran_chapter_to_verse, surah_number_to_name_tag
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
-COMPLETIONS_MODEL = "gpt-3.5-turbo"
 
 @click.command()
-@click.option('--url', required=True, help='YouTube URL containing desired audio data.')
-@click.option('--time', required=True, help='Countdown time in format [number][h/m/s], i.e. 1h would create a 1 hour timer.')
-@click.option('--output', required=True, help='Name of the output file.')
+@click.option('--countdown-time', required=True, help='Countdown time in format [number][h/m/s], i.e. 1h would create a 1 hour timer.')
+@click.option('--surah', required=False, help='Specific Surah from the Quran to play for the alarm audio (int between 1 and 114). Default is the first chapter (Surah Al-Fatihah).', default=1)
 @click.option('--names-flag', required=False, help='Whether or not to include a randomly selected name of Allah in the preamble.', default=True)
-@click.option('--transition-time', required=False, help='Time in seconds for the transition between the output audio and the Quran verses.', default=600)
-@click.option('--surah', required=False, help='Specific Surah from the Quran. Should be given as integer.')
-@click.option('--english', required=False, help='Whether or not to play audio with the english translation of the Quran verses. Note this option only applies if the --surah option is not None.', default=False)
+@click.option('--english', required=False, help='Whether or not to play audio with the english translation of the Quran verses.', default=False)
 @click.option('--low-pass', required=False, help='Amount of low-pass to apply to the audio (float (KHz) or None). Default is 10 (KHz).', default=10)
+@click.option('--gpt-model-type', required=False, help='Which GPT model to use for the prompt responses from OpenAI.', default="gpt-4-0314")
 
-def main(url, time, output, names_flag, transition_time=600, surah=None, english=False, low_pass=10):
-    # Check surah option
-    if surah:
-        # make the output file name the same as the surah
-        output = 'quran-' + '{:03d}'.format(int(surah))
-        if not english:
-            flag = download_surah(surah, output)
-        else:
-            output += '-english'
-            flag = download_surah_with_english(surah, output)
-    else:
-        # Download video
-        flag = download_video(url, output)
-
-    # test audio
-    test_audio(f'{output}.mp3',output,flag)
-
-    # apply low pass filter to the audio
-    if low_pass:
-        cutoff_filter = float(low_pass) * 1000
-        apply_low_pass_filter(f'{output}.mp3', cutoff_filter)
+def main(countdown_time, surah=1, names_flag=True, english=False, low_pass=10, gpt_model_type="gpt-4-0314"):
+    # initialize the result queues
+    allah_queue = queue.Queue() if names_flag else None
+    selected_verses_queue = queue.Queue()
+    verses_explanations_queue = queue.Queue()
+    quran_audio_queue = queue.Queue()
+    alarm_out_queue = queue.Queue()
 
     # convert time to seconds
-    countdown_seconds = convert_to_seconds(time)
+    countdown_seconds = convert_to_seconds(countdown_time)
+
+    # Create threads for audio processing and countdown
+    prepare_alarm_audio_thread = Thread(target=alarm_audio_processing, args=(surah, english, low_pass, alarm_out_queue))
+    countdown_thread = Thread(target=countdown, args=(countdown_seconds,))
+
+    # create threads for obtaining quran verse and Allah name explanations
+    selected_verses_thread = Thread(target=select_quran_verse,args=(selected_verses_queue,))
+    get_name_of_allah_thread = Thread(target=get_name_of_allah_and_explanation, args=(gpt_model_type,allah_queue)) if names_flag else None
+
+    # Start the threads
+    countdown_thread.start()
+    selected_verses_thread.start()
+
+    # wait for the selected verse thread to finish
+    selected_verses_thread.join()
+
+    # fetch the results from the queue
+    verses_Quran_Module, selected_verses = selected_verses_queue.get()
+
+    # for the selected verses, get the explanations and corresponding audio on a separate thread
+    get_explanations_thread = Thread(target=get_explanations, args=(verses_Quran_Module,selected_verses,countdown_seconds,gpt_model_type,verses_explanations_queue,))
+    prepare_selected_verse_audio_thread = Thread(target=download_quran_verses_audio,args=(selected_verses,quran_audio_queue,))
+
+    # wait a second before starting the explanations and audio downloading threads
+    time.sleep(1)
+    get_name_of_allah_thread.start() if names_flag else None
+    get_explanations_thread.start()
+    prepare_alarm_audio_thread.start()
+    prepare_selected_verse_audio_thread.start()
+
+    # wait for the explanations threads to finish
+    get_name_of_allah_thread.join() if names_flag else None
+    get_explanations_thread.join()
+    prepare_alarm_audio_thread.join()
+
+    # fetch the results from the queue
+    name_of_allah_arabic, name_of_allah_transliteration, name_of_allah_english, explanation = allah_queue.get() if names_flag else None
+    verse_texts, explanations, verses = verses_explanations_queue.get()
+    selected_quran_audio_file = quran_audio_queue.get()[0]
+    alarm_output_file = alarm_out_queue.get()[0] + '.mp3'
+
+    # process the selected quran audio file on a separate thread
+    # filter_selected_audio_thread = Thread(target=apply_low_pass_filter,args=(selected_quran_audio_file,low_pass))
+    # filter_selected_audio_thread.start()
+    # filter_selected_audio_thread.join()
 
-    # Start countdown
-    countdown(countdown_seconds)
+    # Wait for both threads to finish
+    countdown_thread.join()
 
-    # Play audio with fade-in effect on a separate thread
-    play_audio_thread = Thread(target=play_audio, args=(f'{output}.mp3',transition_time))
+    # Play alarm audio with fade-in effect on a separate thread
+    play_audio_thread = Thread(target=play_audio, args=(alarm_output_file,))
     play_audio_thread.start()
 
-    # display a name of Allah
-    get_name_of_allah_and_explanation(names_flag)
+    # display the name of Allah and explanation
+    display_allah_name_and_explanation(name_of_allah_arabic, name_of_allah_transliteration, name_of_allah_english, explanation) if names_flag else None
 
-    # stop the misharay audio once the user has finished reading the name of Allah on a separate thread
-    stop_audio(5)
+    print(f'When you are ready to see the selected Quran verses, press ENTER.')
+    input()
 
-    # select the quran verses
-    versesQM, verses = select_quran_verse()
+    # print the selected verses
+    print_selected_verses(verses)
 
-    # print the verses selected
-    print(f'\n\nQuran Verses Selected:\n')
-    for verse in verses:
-        print(f'{verse}')
-    
-    # play the audio of the quran verses
-    play_audio_thread = Thread(target=play_quran_verses_audio, args=(verses,0.5))
+    # stop the misharay audio once the user has finished reading the name of Allah
+    stop_audio(5,)
+
+    # play the audio of the quran verses with 5 second fade in
+    play_audio_thread = Thread(target=play_audio, args=(selected_quran_audio_file,))
     play_audio_thread.start()
 
-    # get the explanations of the quran verses
-    get_explanations(versesQM, verses, countdown_seconds)
+    # display the explanations
+    display_quran_verse_explanations(verse_texts,explanations,verses)
 
     # stop the audio once the user has completed reading the verses
     stop_audio()
 
     # return back to the main thread
     play_audio_thread.join()
 
+def print_selected_verses(verses:list):
+    # print the verses selected
+    print(f'\n\nQuran Verses Selected:\n')
+    for verse in verses:
+        print(f'{verse}')
+
+def alarm_audio_processing(surah, english, low_pass, out_queue=None):
+    # make the output file name the same as the surah
+    output = 'quran-' + '{:03d}'.format(int(surah))
+    if not english:
+        flag = download_surah(surah, output)
+    else:
+        output += '-english'
+        flag = download_surah_with_english(surah, output)
+
+    # test audio
+    test_audio(f'{output}.mp3', output, flag)
+
+    # apply low pass filter to the audio
+    if low_pass:
+        cutoff_filter = float(low_pass) * 1000
+        apply_low_pass_filter(f'{output}.mp3', cutoff_filter)
+    
+    if out_queue:
+        out_queue.put([output])
+    else:
+        return True
+
 def download_surah_with_english(surah, output):
     # check if the output file already exists
     if os.path.exists(f'{output}.mp3'):
         # if the output file exists, then return True
         return True
     else:        
         # get the url directly from thechosenone.info
@@ -137,30 +192,29 @@
 
         # delete the temporary files
         for file_path in file_paths:
             os.remove(file_path)
 
     return True    
 
-def play_quran_verses_audio(verses,transition_time=0.5):
+def download_quran_verses_audio(verses, quran_audio_queue):
     # convert verses to urls
     urls = [quran_verse_to_mp3_url(verse) for verse in verses]
 
     # download the verse audio
     file_paths = [download_file_and_sleep(url,0.5) for url in urls]
 
     # concatenate the audio files into one
     combined_audio_file_name = combine_audio_from_files(file_paths)
 
     # delete the temporary files
     for file_path in file_paths:
         os.remove(file_path)
-
-    # play the audio of the combined quaran verses
-    play_audio(combined_audio_file_name, transition_time)
+    
+    quran_audio_queue.put([combined_audio_file_name])
 
 def combine_audio_from_files(file_paths):
     # combine the audio files
     combined_audio = AudioSegment.empty()
     for file_path in file_paths:
         combined_audio += AudioSegment.from_mp3(file_path)
 
@@ -244,70 +298,74 @@
             audio = AudioSegment.from_file(file_path, format="mp3")
         except:
             print("Error: Audio file could not be loaded.")
     else:
         print(f'{output}.mp3 has already been downloaded and converted.')
 
 def countdown(countdown_seconds):
+    # specify a global variable to store if the countdown has finished or not
+    global countdown_finished
+    countdown_finished = False
+
     # use tqdm to display the countdown progress
     print('\n\n\n\n ---------------- BEGINNING COUNTDOWN ---------------- \n\n\n\n')
     # print the current time in HH:MM format
     print(f'\n\nSTART TIME: {time.strftime("%H:%M", time.localtime())}\n\n')
     for i in tqdm(range(int(countdown_seconds))):
         time.sleep(1)
+    countdown_finished = True
     print('\n\n\n\n ---------------- COUNTDOWN COMPLETE ----------------')
     # print the current time in HH:MM format
     print(f'\n\nEND TIME: {time.strftime("%H:%M", time.localtime())}\n\n')
 
-def get_name_of_allah_and_explanation(names_flag):
-    if not names_flag:
-        return None
-    else:
-        # Get the names of Allah
-        names_of_allah = Project_Quran().Get_Names_of_Allah_English()
+def get_name_of_allah_and_explanation(gpt_model_type, allah_queue):
+    # Get the names of Allah
+    names_of_allah = Project_Quran().Get_Names_of_Allah_English()
 
-        # get the arabic names of Allah
-        names_of_allah_arabic = Project_Quran().Get_Names_of_Allah_Arabic()
+    # get the arabic names of Allah
+    names_of_allah_arabic = Project_Quran().Get_Names_of_Allah_Arabic()
 
-        # Get the transliterated names of Allah
-        allah_transliterations = Project_Quran().Get_Names_of_Allah_Transliteration()
+    # Get the transliterated names of Allah
+    allah_transliterations = Project_Quran().Get_Names_of_Allah_Transliteration()
 
-        # Select a index in the range of the number of names of Allah
-        index = random.randint(0, len(names_of_allah) - 1)
+    # Select a index in the range of the number of names of Allah
+    index = random.randint(0, len(names_of_allah) - 1)
 
-        # Get the name of Allah in English
-        name_of_allah_english = names_of_allah[index]
+    # Get the name of Allah in English
+    name_of_allah_english = names_of_allah[index]
 
-        # Get the name of Allah in Arabic
-        name_of_allah_arabic = names_of_allah_arabic[index]
+    # Get the name of Allah in Arabic
+    name_of_allah_arabic = names_of_allah_arabic[index]
 
-        # Get the transliteration of the name of Allah
-        name_of_allah_transliteration = allah_transliterations[index]
+    # Get the transliteration of the name of Allah
+    name_of_allah_transliteration = allah_transliterations[index]
 
-        # Get the explanation of the name of Allah using a GPT-3 model prompt
-        prompt = f"""
+    # Get the explanation of the name of Allah using a GPT-3 model prompt
+    prompt = f"""
 
-        For the name of Allah below, please do the following: First break down the word into its root letters and also identify the corresponding Arabic letter for each phonetic sound, giving their approximate equivalent in the english language.
-        Then, using the root letters, try to guess the meaning of the name. Finally, give a brief explanation of the significane of this particular name of Allah as it relates to the Quran.
-        
-        Name of Allah: {name_of_allah_arabic}\nExplanation: 
-        
-        """
+    For the name of Allah below, please do the following: First break down the word into its individual letters (remember that Arabic reads from right to left), giving their approximate equivalent in the english language.
+    Then, using the letters identified, give a few example sentences that use a word with similar letters, and then try to guess the meaning of the name. Finally, give a brief explanation of the significane of this particular name of Allah as it relates to the Quran.
+    
+    Name of Allah: {name_of_allah_arabic}\nExplanation: 
+    
+    """
 
-        # Get the explanation of the name of Allah
-        explanation = query_gpt(prompt)
+    # Get the explanation of the name of Allah
+    explanation = query_gpt(prompt, gpt_model_type)
 
-        # print the name of the Allah and the explanation in a nice format
-        print(f'\n\n\n\n ---------------- NAME OF ALLAH ---------------- \n')
-        print(f'---------------- {name_of_allah_arabic}: {name_of_allah_transliteration} - {name_of_allah_english} ---------------- \n\n')
-        print(f'Explanation: {explanation}\n\n\n\n')
-        print(f'When you are ready to begin, press ENTER.')
-        input()
+    # add the outputs to the queue
+    allah_queue.put([name_of_allah_arabic, name_of_allah_transliteration, name_of_allah_english, explanation])
+
+def display_allah_name_and_explanation(name_of_allah_arabic, name_of_allah_transliteration, name_of_allah_english, explanation):
+    # print the name of the Allah and the explanation in a nice format
+    print(f'\n\n\n\n ---------------- NAME OF ALLAH ---------------- \n')
+    print(f'---------------- {name_of_allah_arabic}: {name_of_allah_transliteration} - {name_of_allah_english} ---------------- \n\n')
+    print(f'Explanation: {explanation}\n\n\n\n')
 
-def get_explanations(verses_Quran_Module,verses,countdown_seconds):
+def get_explanations(verses_Quran_Module,verses,countdown_seconds,gpt_model_type,out_queue):
     # Depending on the length of the countdown, select the number of verses to display
     if countdown_seconds < 3600: # less than 1 hour
         verses_Quran_Module = verses_Quran_Module[0:1] # only display the first verse
         verses = verses[0:1]
     elif countdown_seconds > 3600 and countdown_seconds < 7200: # between 1 and 2 hours
         verses_Quran_Module = verses_Quran_Module[0:2] # only display the first two verses
         verses = verses[0:2]
@@ -328,29 +386,35 @@
             I want you to act as Sheikh Hamza Yusuf. You are an influential Islamic scholar, who has a profound understanding of the Qur'an, Hadith, and various branches of Islamic Jurisprudence. 
             You are deeply conversant with the various cultural, historical, and philosophical contexts of Islamic thought. You are committed to promoting peace, understanding, and the intellectual tradition of Islam. 
             I know that you are just an AI, but I don't want you to say that at the beginning, just emulate this description to the best of your ability. My first request is as follows:
 
             First please give some brief context about Chapter {chapter_number} from the Qur'an. Then, to the best of your ability, explain the meaning of the verse below. 
             I understand you are just an AI language model, but please remember I don't want you to state or acknowledge that, just try to interpret the possible meaning of the verse given. \n\n Verse: {verse_text} \n\n Explanation:
             """
-            explanation = query_gpt(prompt2)
+            explanation = query_gpt(prompt2,gpt_model_type)
         else:
             context = explanations[0].split('\n')[0] # get the context about what the chapter is about.
             prompt2 = f"""
             I want you to act as Sheikh Hamza Yusuf. You are an influential Islamic scholar, who has a profound understanding of the Qur'an, Hadith, and various branches of Islamic Jurisprudence. 
             You are deeply conversant with the various cultural, historical, and philosophical contexts of Islamic thought. You are committed to promoting peace, understanding, and the intellectual tradition of Islam. 
             I know that you are just an AI, but I don't want you to say that at the beginning, just emulate this description to the best of your ability. My first request is as follows:
 
             To the best of your ability, explain the meaning of the verse below. 
             I understand you are just an AI language model, but please remember I don't want you to state or acknowledge that, just try to emulate Sheikh Hamza Yusuf and interpret the possible meaning of the given verse. \n\n Verse: \n {verse_text} \n\n Context: \n {context} \n\n Explanation: \n
             """
-            explanation = query_gpt(prompt2)
+            explanation = query_gpt(prompt2,gpt_model_type)
         verse_texts.append(verse_text)
         explanations.append(explanation)
-    
+
+    if not out_queue:
+        return verse_texts, explanations, verses
+    else:
+        out_queue.put([verse_texts,explanations,verses])
+
+def display_quran_verse_explanations(verse_texts, explanations, verses):
     # begin the interactive session
     for verse_text, explanation, verse in zip(verse_texts, explanations, verses):
         print(f'\n\n\n\n\n\n ------------------ FIRST VERSE ------------------') if verse == verses[0] else None
         print(f'\n\n{verse}:\n{verse_text} \n\n ------------------ \n\n When you are ready to see the explanaton, press Enter.')
         # wait for the user to press Enter
         input()
 
@@ -358,23 +422,26 @@
         if verse != verses[-1]:
             print(f'{explanation} \n\n ------------------ \n\n When you are ready to proceed to the next verse, press Enter (20 second timer).')
         else:
             print(f'{explanation} \n\n ------------------ \n\n When you are ready to stop the alarm, press Enter (20 second timer).')
         time.sleep(20) # Wait for the user to press Enter, but not before 20 seconds have passed
         input() # wait for the user to press Enter
 
-def get_verses_and_explanations(countdown_seconds):
+def get_verses_and_explanations(countdown_seconds,gpt_model_type,verses_queue):
     # Get the verses
     verses_Quran_Module, verses  = select_quran_verse()
     # print(f"Verse 1:\n{verses}")
 
     # Get the explanations
-    get_explanations(verses_Quran_Module,verses,countdown_seconds)
+    verse_texts, explanations, verses = get_explanations(verses_Quran_Module,verses,countdown_seconds,gpt_model_type)
+
+    # put the results into the queue
+    verses_queue.put([verse_texts, explanations, verses])
 
-def select_quran_verse():
+def select_quran_verse(output_queue=None):
     # List of surah numbers
     surahs = list(quran_chapter_to_verse.keys())
 
     # Number of verses in each surah, this is just a placeholder
     # Please replace this with the actual number of verses in each surah
     verses_in_surah = list(quran_chapter_to_verse.values())
 
@@ -389,33 +456,41 @@
         # raise an error saying there are not enough verses in the Surah
         raise Exception(f'There are not enough verses in Surah {surah}.')
 
     # Select a verse such that there are at least 2 verses that follow after the verse
     verse = random.randint(1, num_verses - 2)
 
     # Return the verses
-    return (f'59,{surah},{verse}', f'59,{surah},{verse + 1}', f'59,{surah},{verse + 2}'), (f'{surah}:{verse}',f'{surah}:{verse+1}' ,f'{surah}:{verse+2}') # 59 corresponds to english Quran verse
+    if not output_queue:
+        return (f'59,{surah},{verse}', f'59,{surah},{verse + 1}', f'59,{surah},{verse + 2}'), (f'{surah}:{verse}',f'{surah}:{verse+1}' ,f'{surah}:{verse+2}') # 59 corresponds to english Quran verse
+    else:
+        verses_Quran_Module, verses = (f'59,{surah},{verse}', f'59,{surah},{verse + 1}', f'59,{surah},{verse + 2}'), (f'{surah}:{verse}',f'{surah}:{verse+1}' ,f'{surah}:{verse+2}') # 59 corresponds to english Quran verse
+        output_queue.put([verses_Quran_Module, verses])
 
-def query_gpt(prompt):
+def query_gpt(prompt,gpt_model_type):
     # GPT-3 API parameters
     COMPLETIONS_API_PARAMS = {
     # We use temperature of 0.4 because it gives the most predictable, factual answer with some variation.
     "temperature": 0.4,
     "max_tokens": 1000,
-    "model": COMPLETIONS_MODEL,
+    "model": gpt_model_type,
     }
     
     response = openai.ChatCompletion.create(
                 messages = [{"role": "user", "content": prompt}],
                 **COMPLETIONS_API_PARAMS
             )
 
     return response['choices'][0]['message']['content']
 
 def gradually_change_volume(start_volume, end_volume, duration):
+    # specify a global variable to indicate whether or not the audio has finished changing volume
+    global finished_changing_volume
+    finished_changing_volume = False
+
     # Compute the number of steps and the change in volume per step
     steps = int(duration * 100)  # Multiply by 100 to allow for hundredths of seconds
     delay = 0.01  # Delay for each step
 
     max_steps = 10000  # Maximum number of steps
 
     # If steps are more than maximum, adjust steps and delay
@@ -439,14 +514,18 @@
 
         # If the stop_audio function has been called, break the loop
         if stop_audio_called:
             print("Stopping volume change due to stop_audio being called")
             break
 
 def play_audio(file_path_or_url, transition_time=900):
+    # wait for the countdown to finish
+    while not countdown_finished:
+        time.sleep(1)
+
     global stop_audio_called
     stop_audio_called = False
     file_path = ''
 
     # Check if file_path_or_url is URL
     if file_path_or_url.startswith('http'):
         # Download the file and get the path
@@ -460,17 +539,17 @@
     # Load the audio file
     pygame.mixer.music.load(file_path)
 
     # Start playing the audio with volume 0
     pygame.mixer.music.set_volume(0.0)
     pygame.mixer.music.play()
 
-    # if the transition time is longer than the audio, set it to the audio length
+    # if the transition time is longer than half of the audio, set it to half of the audio length
     length_in_seconds = mp3.MP3(file_path).info.length
-    if transition_time > length_in_seconds:
+    if transition_time > 0.5 * length_in_seconds:
         transition_time = length_in_seconds * 0.5
 
     # Gradually increase the volume over 15 minutes in a separate thread
     gradually_change_volume(0.0, 1.0, transition_time)
 
     # Loop the audio until the stop_audio function is called
     while not stop_audio_called:
```

### Comparing `fajrGPT-1.5.4/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.5.5/fajrGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.5.4
+Version: 1.5.5
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.5.4/setup.py` & `fajrGPT-1.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.5.4",
+    version="1.5.5",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

