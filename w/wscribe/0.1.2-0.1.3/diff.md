# Comparing `tmp/wscribe-0.1.2.tar.gz` & `tmp/wscribe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wscribe-0.1.2.tar", max compression
+gzip compressed data, was "wscribe-0.1.3.tar", max compression
```

## Comparing `wscribe-0.1.2.tar` & `wscribe-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2023-07-21 09:28:16.650987 wscribe-0.1.2/LICENSE
--rw-r--r--   0        0        0     5908 2023-08-05 16:00:55.334063 wscribe-0.1.2/docs/README.md
--rw-r--r--   0        0        0     1132 2023-08-05 16:02:05.787534 wscribe-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1786 2023-07-25 13:58:47.564422 wscribe-0.1.2/src/wscribe/__init__.py
--rw-r--r--   0        0        0     2576 2023-08-05 07:06:03.013196 wscribe-0.1.2/src/wscribe/backends/fasterwhisper.py
--rw-r--r--   0        0        0     2253 2023-08-05 15:47:09.721778 wscribe-0.1.2/src/wscribe/cli/main.py
--rw-r--r--   0        0        0     2157 2023-08-05 07:10:37.672683 wscribe-0.1.2/src/wscribe/core.py
--rw-r--r--   0        0        0      378 2023-07-25 13:58:47.514422 wscribe-0.1.2/src/wscribe/sources/local.py
--rw-r--r--   0        0        0     3298 2023-08-05 07:17:56.081761 wscribe-0.1.2/src/wscribe/writers.py
--rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 wscribe-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-21 09:28:16.650987 wscribe-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5908 2023-08-05 20:05:11.292595 wscribe-0.1.3/docs/README.md
+-rw-r--r--   0        0        0     1132 2023-08-05 20:05:46.808394 wscribe-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1778 2023-08-05 20:05:11.312595 wscribe-0.1.3/src/wscribe/__init__.py
+-rw-r--r--   0        0        0     2569 2023-08-05 20:05:11.312595 wscribe-0.1.3/src/wscribe/backends/fasterwhisper.py
+-rw-r--r--   0        0        0     3321 2023-08-05 20:05:11.312595 wscribe-0.1.3/src/wscribe/cli/main.py
+-rw-r--r--   0        0        0     2277 2023-08-05 20:05:11.312595 wscribe-0.1.3/src/wscribe/core.py
+-rw-r--r--   0        0        0      378 2023-07-25 13:58:47.514422 wscribe-0.1.3/src/wscribe/sources/local.py
+-rw-r--r--   0        0        0     3298 2023-08-05 07:17:56.081761 wscribe-0.1.3/src/wscribe/writers.py
+-rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 wscribe-0.1.3/PKG-INFO
```

### Comparing `wscribe-0.1.2/LICENSE` & `wscribe-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wscribe-0.1.2/docs/README.md` & `wscribe-0.1.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `wscribe-0.1.2/pyproject.toml` & `wscribe-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wscribe"
-version = "0.1.2"
+version = "0.1.3"
 description = "ez audio transcription tool with flexible processing and post-processing options"
 authors = ["Hrishikesh Barman <oss@geekodour.org>"]
 homepage = "https://github.com/geekodour/wscribe"
 license = "MIT"
 readme = "docs/README.md"
 packages = [{include = "wscribe", from = "src"}]
```

### Comparing `wscribe-0.1.2/src/wscribe/__init__.py` & `wscribe-0.1.3/src/wscribe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def setup_stdlogger():
     DATEFMT = "%d-%m-%Y %I:%M:%S %p"
     FORMAT = "%(message)s"
     logging.basicConfig(
         format=FORMAT,
         stream=sys.stdout,  # https://12factor.net/logs
-        level=logging.INFO,
+        level=None,
         datefmt=DATEFMT,
     )
 
 
 def get_structlog_processors() -> Iterable[Processor]:
     processors: Iterable[Processor] = [
         structlog.stdlib.add_logger_name,
```

### Comparing `wscribe-0.1.2/src/wscribe/backends/fasterwhisper.py` & `wscribe-0.1.3/src/wscribe/backends/fasterwhisper.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,26 +9,22 @@
 from tqdm import tqdm  # type: ignore
 
 from ..core import Backend, TranscribedData
 from ..writers import format_timestamp
 
 DEFAULT_BEAM = 5
 LOGGER = structlog.get_logger()
-SUPPORTED_MODELS = ["tiny", "small", "medium", "large-v2"]
 
 
 @dataclass(kw_only=True)
 class FasterWhisperBackend(Backend):
     device: str = "cpu"  # cpu, cuda
     quantization: str = "int8"  # int8, float16
     model: WhisperModel | None = None
 
-    def supported_model_sizes(self) -> list[str]:
-        return SUPPORTED_MODELS
-
     def model_path(self) -> str:
         local_model_path = os.path.join(
             os.environ["WSCRIBE_MODELS_DIR"], f"faster-whisper-{self.model_size}"
         )
 
         if os.path.exists(local_model_path):
             return local_model_path
@@ -36,27 +32,32 @@
             raise RuntimeError(f"model not found in {local_model_path}")
 
     def load(self) -> None:
         self.model = WhisperModel(
             self.model_path(), device=self.device, compute_type=self.quantization
         )
 
-    def transcribe(self, input: np.ndarray) -> list[TranscribedData]:
+    def transcribe(
+        self, input: np.ndarray, silent: bool = False
+    ) -> list[TranscribedData]:
         """
         Return word level transcription data.
         World level probabities are calculated by ctranslate2.models.Whisper.align
         """
         result: list[TranscribedData] = []
         assert self.model is not None
         segments, info = self.model.transcribe(
             input,
             beam_size=DEFAULT_BEAM,
             word_timestamps=True,
         )
-        with tqdm(total=info.duration, unit_scale=True, unit="playback") as pbar:
+        # ps = playback seconds
+        with tqdm(
+            total=info.duration, unit_scale=True, unit="ps", disable=silent
+        ) as pbar:
             for segment in segments:
                 if segment.words is None:
                     continue
                 segment_extract: TranscribedData = {
                     "text": segment.text,
                     "start": segment.start,
                     "end": segment.end,
@@ -68,9 +69,10 @@
                             "text": w.word,
                             "score": round(w.probability, 2),
                         }
                         for w in segment.words
                     ],
                 }
                 result.append(segment_extract)
-                pbar.update(segment.end - pbar.last_print_n)
+                if not silent:
+                    pbar.update(segment.end - pbar.last_print_n)
         return result
```

### Comparing `wscribe-0.1.2/src/wscribe/cli/main.py` & `wscribe-0.1.3/src/wscribe/cli/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
 import logging
 import os
+import time
 
 import click
 import structlog
 
 from wscribe.backends.fasterwhisper import FasterWhisperBackend
 from wscribe.sources.local import LocalAudio
 
+from ..core import SUPPORTED_MODELS
 from ..writers import WRITERS
 
 LOGGER = structlog.get_logger(ui="cli")
 
 
 @click.group()
 def cli():
@@ -38,42 +40,69 @@
     default="json",
     show_default=True,
 )
 @click.option(
     "-m",
     "--model",
     help="model should already be downloaded",
-    type=click.Choice(["small", "medium", "large-v2"], case_sensitive=True),
+    type=click.Choice(SUPPORTED_MODELS, case_sensitive=True),
     default="medium",
     show_default=True,
 )
 @click.option(
     "-g", "--gpu", help="enable gpu, disabled by default", default=False, is_flag=True
 )
 @click.option("-d", "--debug", help="show debug logs", default=False, is_flag=True)
-def transcribe(source, destination, format, model, gpu, debug):
+@click.option("-s", "--stats", help="print stats", default=False, is_flag=True)
+@click.option("-q", "--quiet", help="no progress bar", default=False, is_flag=True)
+def transcribe(source, destination, format, model, gpu, debug, stats, quiet):
     """
     Transcribes SOURCE to DESTINATION. Where SOURCE can be local path to an audio/video file and
     DESTINATION needs to be a local path to a non-existing file.
     """
     if debug:
         logging.basicConfig(level=logging.DEBUG, force=True)
     log = LOGGER.bind(
         source=source, destination=destination, format=format, model=model, gpu=gpu
     )
 
     device, quantization = ("cuda", "float16") if gpu else ("cpu", "int8")
     m = FasterWhisperBackend(model_size=model, device=device, quantization=quantization)
     m.load()
     log.debug(f"model loaded with {device}-{quantization}")
+
+    audio_start_time = time.perf_counter()
     audio = LocalAudio(source=source).convert_audio()
-    result = m.transcribe(input=audio)
+    audio_end_time = time.perf_counter()
+
+    ts_start_time = time.perf_counter()
+    result = m.transcribe(input=audio, silent=quiet)
+    ts_end_time = time.perf_counter()
+
     writer = WRITERS[format](result=result, destination=destination)
     writer.write()
 
+    if stats:
+        original_audio_time = audio.shape[0] / LocalAudio.sampling_rate
+        transcription_time = ts_end_time - ts_start_time
+        audio_conversion_time = audio_end_time - audio_start_time
+        click.echo(
+            " | ".join(
+                [
+                    device,
+                    quantization,
+                    model,
+                    str(round(audio_conversion_time, 1)) + "s",
+                    str(round(original_audio_time / 60, 1)) + "m",
+                    str(round(transcription_time / 60, 1)) + "m",
+                    str(int(original_audio_time / transcription_time)) + "x",
+                ]
+            )
+        )
+
 
 @cli.command()
 def info():
     """Information about related files and directories"""
     click.echo(f"WSCRIBE_MODELS_DIR: {os.environ['WSCRIBE_MODELS_DIR']}")
```

### Comparing `wscribe-0.1.2/src/wscribe/core.py` & `wscribe-0.1.3/src/wscribe/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Mapping, TypedDict
 
 import numpy as np
 import structlog
 from faster_whisper.audio import decode_audio  # type: ignore
 
 LOGGER = structlog.get_logger()
+SUPPORTED_MODELS = ["tiny", "small", "medium", "large-v2"]
 
 WordData = TypedDict(
     "WordData", {"text": str, "start": float | str, "end": float | str, "score": float}
 )
 TranscribedData = TypedDict(
     "TranscribedData",
     {
@@ -42,15 +43,15 @@
     def model_path(self) -> str:
         """
         Returns the local path to the model, error-out if unavailable
         """
         raise NotImplementedError()
 
     def supported_model_sizes(self) -> list[str]:
-        raise NotImplementedError()
+        return SUPPORTED_MODELS
 
     def load(self):
         raise NotImplementedError()
 
     def transcribe(self, input: np.ndarray) -> list[TranscribedData]:
         """
         This should return word level transcription data.
@@ -58,14 +59,15 @@
         raise NotImplementedError()
 
 
 @dataclass(kw_only=True)
 class Audio:
     source: str
     local_source_path: str = ""
+    sampling_rate: int = 16000
 
     def fetch_audio(self):
         """
         Fetches audio and sets local_source_path
         Should be implemented by inherited class
         """
         raise NotImplementedError()
@@ -75,8 +77,8 @@
         """
         regex match
         User is supposed to initialte appropriate class based on this
         """
         raise NotImplementedError()
 
     def convert_audio(self) -> np.ndarray:
-        return decode_audio(self.local_source_path, split_stereo=False)  # type: ignore
+        return decode_audio(self.local_source_path, split_stereo=False, sampling_rate=self.sampling_rate)  # type: ignore
```

### Comparing `wscribe-0.1.2/src/wscribe/writers.py` & `wscribe-0.1.3/src/wscribe/writers.py`

 * *Files identical despite different names*

### Comparing `wscribe-0.1.2/PKG-INFO` & `wscribe-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wscribe
-Version: 0.1.2
+Version: 0.1.3
 Summary: ez audio transcription tool with flexible processing and post-processing options
 Home-page: https://github.com/geekodour/wscribe
 License: MIT
 Author: Hrishikesh Barman
 Author-email: oss@geekodour.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

