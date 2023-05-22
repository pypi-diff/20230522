# Comparing `tmp/soniox-1.6.2.tar.gz` & `tmp/soniox-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soniox-1.6.2.tar", last modified: Wed Mar 29 10:57:58 2023, max compression
+gzip compressed data, was "soniox-1.7.0.tar", last modified: Mon May 22 11:58:55 2023, max compression
```

## Comparing `soniox-1.6.2.tar` & `soniox-1.7.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-03-29 10:57:58.929152 soniox-1.6.2/
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1053 2022-06-20 18:06:39.000000 soniox-1.6.2/LICENSE
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1168 2023-03-29 10:57:58.929152 soniox-1.6.2/PKG-INFO
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      745 2023-03-29 10:56:40.000000 soniox-1.6.2/README.md
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)       38 2023-03-29 10:57:58.929152 soniox-1.6.2/setup.cfg
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      740 2023-03-29 10:57:18.000000 soniox-1.6.2/setup.py
-drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-03-29 10:57:58.929152 soniox-1.6.2/soniox/
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        0 2022-06-20 18:06:39.000000 soniox-1.6.2/soniox/__init__.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     3815 2022-06-21 13:02:17.000000 soniox-1.6.2/soniox/capture_device.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      304 2022-09-01 10:40:05.000000 soniox-1.6.2/soniox/conversion.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     6512 2022-08-31 07:52:52.000000 soniox-1.6.2/soniox/manage_speakers.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     5586 2022-08-31 07:53:02.000000 soniox-1.6.2/soniox/manage_speech_contexts.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     3808 2022-06-21 13:02:45.000000 soniox-1.6.2/soniox/multi_channel_utils.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    12860 2023-03-29 10:48:22.000000 soniox-1.6.2/soniox/speech_service.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    16985 2023-03-29 10:49:41.000000 soniox-1.6.2/soniox/speech_service_pb2.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    34287 2023-03-29 10:49:41.000000 soniox-1.6.2/soniox/speech_service_pb2_grpc.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    15276 2023-03-29 10:49:07.000000 soniox-1.6.2/soniox/transcribe_file.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     8284 2023-03-29 10:49:29.000000 soniox-1.6.2/soniox/transcribe_live.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      283 2023-03-28 15:25:04.000000 soniox-1.6.2/soniox/utils.py
-drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-03-29 10:57:58.929152 soniox-1.6.2/soniox.egg-info/
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1168 2023-03-29 10:57:58.000000 soniox-1.6.2/soniox.egg-info/PKG-INFO
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      485 2023-03-29 10:57:58.000000 soniox-1.6.2/soniox.egg-info/SOURCES.txt
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        1 2023-03-29 10:57:58.000000 soniox-1.6.2/soniox.egg-info/dependency_links.txt
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)       48 2023-03-29 10:57:58.000000 soniox-1.6.2/soniox.egg-info/requires.txt
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        7 2023-03-29 10:57:58.000000 soniox-1.6.2/soniox.egg-info/top_level.txt
+drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-05-22 11:58:55.018943 soniox-1.7.0/
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1053 2022-06-20 18:06:39.000000 soniox-1.7.0/LICENSE
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1168 2023-05-22 11:58:55.018943 soniox-1.7.0/PKG-INFO
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      745 2023-03-29 10:56:40.000000 soniox-1.7.0/README.md
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)       38 2023-05-22 11:58:55.018943 soniox-1.7.0/setup.cfg
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      740 2023-05-22 11:58:01.000000 soniox-1.7.0/setup.py
+drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-05-22 11:58:55.018943 soniox-1.7.0/soniox/
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        0 2022-06-20 18:06:39.000000 soniox-1.7.0/soniox/__init__.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     3815 2023-05-17 12:09:38.000000 soniox-1.7.0/soniox/capture_device.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      304 2022-09-01 10:40:05.000000 soniox-1.7.0/soniox/conversion.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     6512 2022-08-31 07:52:52.000000 soniox-1.7.0/soniox/manage_speakers.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     5586 2022-08-31 07:53:02.000000 soniox-1.7.0/soniox/manage_speech_contexts.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     3808 2022-06-21 13:02:45.000000 soniox-1.7.0/soniox/multi_channel_utils.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    12909 2023-03-31 09:29:12.000000 soniox-1.7.0/soniox/speech_service.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    25842 2023-05-22 11:58:22.000000 soniox-1.7.0/soniox/speech_service_pb2.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    42523 2023-05-22 11:58:22.000000 soniox-1.7.0/soniox/speech_service_pb2_grpc.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     5885 2023-04-25 11:52:59.000000 soniox-1.7.0/soniox/storage.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    16186 2023-03-31 09:29:12.000000 soniox-1.7.0/soniox/transcribe_file.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     8821 2023-05-17 12:09:43.000000 soniox-1.7.0/soniox/transcribe_live.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      283 2023-03-28 15:25:04.000000 soniox-1.7.0/soniox/utils.py
+drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-05-22 11:58:55.018943 soniox-1.7.0/soniox.egg-info/
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1168 2023-05-22 11:58:55.000000 soniox-1.7.0/soniox.egg-info/PKG-INFO
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      503 2023-05-22 11:58:55.000000 soniox-1.7.0/soniox.egg-info/SOURCES.txt
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        1 2023-05-22 11:58:55.000000 soniox-1.7.0/soniox.egg-info/dependency_links.txt
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)       48 2023-05-22 11:58:55.000000 soniox-1.7.0/soniox.egg-info/requires.txt
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        7 2023-05-22 11:58:55.000000 soniox-1.7.0/soniox.egg-info/top_level.txt
```

### Comparing `soniox-1.6.2/LICENSE` & `soniox-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `soniox-1.6.2/PKG-INFO` & `soniox-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soniox
-Version: 1.6.2
+Version: 1.7.0
 Summary: Soniox speech recognition service client library
 Home-page: https://soniox.com/
 Author: Soniox Inc
 Author-email: support@soniox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soniox-1.6.2/README.md` & `soniox-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `soniox-1.6.2/setup.py` & `soniox-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="soniox",
-    version="1.6.2",
+    version="1.7.0",
     author="Soniox Inc",
     author_email="support@soniox.com",
     description="Soniox speech recognition service client library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://soniox.com/",
     packages=setuptools.find_packages(),
```

### Comparing `soniox-1.6.2/soniox/capture_device.py` & `soniox-1.7.0/soniox/capture_device.py`

 * *Files identical despite different names*

### Comparing `soniox-1.6.2/soniox/manage_speakers.py` & `soniox-1.7.0/soniox/manage_speakers.py`

 * *Files identical despite different names*

### Comparing `soniox-1.6.2/soniox/manage_speech_contexts.py` & `soniox-1.7.0/soniox/manage_speech_contexts.py`

 * *Files identical despite different names*

### Comparing `soniox-1.6.2/soniox/multi_channel_utils.py` & `soniox-1.7.0/soniox/multi_channel_utils.py`

 * *Files identical despite different names*

### Comparing `soniox-1.6.2/soniox/speech_service.py` & `soniox-1.7.0/soniox/speech_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 SpeechContextEntry = speech_service_pb2.SpeechContextEntry
 Result = speech_service_pb2.Result
 Word = speech_service_pb2.Word
 TranscriptionConfig = speech_service_pb2.TranscriptionConfig
 TranscribeMeetingRequest = speech_service_pb2.TranscribeMeetingRequest
 TranscribeMeetingResponse = speech_service_pb2.TranscribeMeetingResponse
 TranscribeAsyncFileStatus = speech_service_pb2.TranscribeAsyncFileStatus
+StorageConfig = speech_service_pb2.StorageConfig
 
 SpeechServiceStub = speech_service_pb2_grpc.SpeechServiceStub
 
 _API_HOST = ""
 _API_KEY = ""
 _DEFAULT_API_HOST = "https://api.soniox.com:443"
 _GRPC_MAX_MESSAGE_LENGTH = 6291456
```

### Comparing `soniox-1.6.2/soniox/speech_service_pb2.py` & `soniox-1.7.0/soniox/speech_service_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,21 +10,29 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bsoniox/speech_service.proto\x12\x15soniox.speech_service\x1a\x1fgoogle/protobuf/timestamp.proto\"o\n\x11TranscribeRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\x04 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\r\n\x05\x61udio\x18\x03 \x01(\x0c\"\xbb\x01\n\x12TranscribeResponse\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12\x36\n\x0f\x63hannel_results\x18\x02 \x03(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x03 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"u\n\x17TranscribeStreamRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\x04 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\r\n\x05\x61udio\x18\x03 \x01(\x0c\"\x89\x01\n\x18TranscribeStreamResponse\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x02 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"\xcc\x01\n\x18TranscribeMeetingRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\n \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\x0f\n\x07seq_num\x18\x03 \x01(\x05\x12\x11\n\tstream_id\x18\x04 \x01(\x05\x12\x18\n\x10start_of_segment\x18\x05 \x01(\x08\x12\r\n\x05\x61udio\x18\x06 \x01(\x0c\x12\x16\n\x0e\x65nd_of_segment\x18\x07 \x01(\x08\"\xef\x01\n\x19TranscribeMeetingResponse\x12\x0f\n\x07seq_num\x18\x01 \x01(\x05\x12\x11\n\tstream_id\x18\x02 \x01(\x05\x12\x18\n\x10start_of_segment\x18\x03 \x01(\x08\x12\x16\n\x0e\x65nd_of_segment\x18\x04 \x01(\x08\x12-\n\x06result\x18\x05 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12\r\n\x05\x65rror\x18\x06 \x01(\t\x12>\n\x08metadata\x18\x07 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"\xad\x01\n\x16TranscribeAsyncRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x16\n\x0ereference_name\x18\x03 \x01(\t\x12:\n\x06\x63onfig\x18\x05 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\x12\n\nenable_eof\x18\x06 \x01(\x08\x12\x0b\n\x03\x65of\x18\x07 \x01(\x08\x12\r\n\x05\x61udio\x18\x04 \x01(\x0c\"*\n\x17TranscribeAsyncResponse\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\"C\n\x1fGetTranscribeAsyncStatusRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"c\n GetTranscribeAsyncStatusResponse\x12?\n\x05\x66iles\x18\x01 \x03(\x0b\x32\x30.soniox.speech_service.TranscribeAsyncFileStatus\"\x9d\x01\n\x19TranscribeAsyncFileStatus\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x16\n\x0ereference_name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x30\n\x0c\x63reated_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rerror_message\x18\x05 \x01(\t\"C\n\x1fGetTranscribeAsyncResultRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"\xbb\x01\n GetTranscribeAsyncResultResponse\x12(\n separate_recognition_per_channel\x18\x02 \x01(\x08\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x03 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"D\n DeleteTranscribeAsyncFileRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"#\n!DeleteTranscribeAsyncFileResponse\"\xee\x04\n\x13TranscriptionConfig\x12 \n\x18\x63lient_request_reference\x18\x13 \x01(\t\x12\x14\n\x0c\x61udio_format\x18\x01 \x01(\t\x12\x19\n\x11sample_rate_hertz\x18\x02 \x01(\x05\x12\x1a\n\x12num_audio_channels\x18\x03 \x01(\x05\x12\x18\n\x10include_nonfinal\x18\x04 \x01(\x08\x12/\n\'enable_separate_recognition_per_channel\x18\x10 \x01(\x08\x12!\n\x19\x65nable_endpoint_detection\x18\x12 \x01(\x08\x12<\n\x0espeech_context\x18\x05 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\x12\x1f\n\x17\x65nable_profanity_filter\x18\x06 \x01(\x08\x12\"\n\x1a\x63ontent_moderation_phrases\x18\x07 \x03(\t\x12,\n$enable_streaming_speaker_diarization\x18\x08 \x01(\x08\x12)\n!enable_global_speaker_diarization\x18\t \x01(\x08\x12\x18\n\x10min_num_speakers\x18\n \x01(\x05\x12\x18\n\x10max_num_speakers\x18\x0b \x01(\x05\x12%\n\x1d\x65nable_speaker_identification\x18\x0c \x01(\x08\x12\x1a\n\x12\x63\x61nd_speaker_names\x18\r \x03(\t\x12\r\n\x05model\x18\x0e \x01(\t\x12\x18\n\x10\x65nable_dictation\x18\x0f \x01(\x08\"0\n\x15TranscriptionMetadata\x12\x17\n\x0fpackage_version\x18\x01 \x01(\t\"\xb5\x01\n\x06Result\x12*\n\x05words\x18\x01 \x03(\x0b\x32\x1b.soniox.speech_service.Word\x12\x1a\n\x12\x66inal_proc_time_ms\x18\x02 \x01(\x05\x12\x1a\n\x12total_proc_time_ms\x18\x03 \x01(\x05\x12\x36\n\x08speakers\x18\x06 \x03(\x0b\x32$.soniox.speech_service.ResultSpeaker\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\x05\"\x85\x01\n\x04Word\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x10\n\x08start_ms\x18\x02 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x03 \x01(\x05\x12\x10\n\x08is_final\x18\x04 \x01(\x08\x12\x0f\n\x07speaker\x18\x05 \x01(\x05\x12\x11\n\torig_text\x18\x08 \x01(\t\x12\x12\n\nconfidence\x18\t \x01(\x01\".\n\rResultSpeaker\x12\x0f\n\x07speaker\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"Y\n\rSpeechContext\x12:\n\x07\x65ntries\x18\x01 \x03(\x0b\x32).soniox.speech_service.SpeechContextEntry\x12\x0c\n\x04name\x18\x02 \x01(\t\"4\n\x12SpeechContextEntry\x12\x0f\n\x07phrases\x18\x01 \x03(\t\x12\r\n\x05\x62oost\x18\x02 \x01(\x01\"k\n\x1a\x43reateSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12<\n\x0espeech_context\x18\x02 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"\x1d\n\x1b\x43reateSpeechContextResponse\";\n\x1a\x44\x65leteSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x1d\n\x1b\x44\x65leteSpeechContextResponse\"0\n\x1dListSpeechContextNamesRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\"/\n\x1eListSpeechContextNamesResponse\x12\r\n\x05names\x18\x01 \x03(\t\"8\n\x17GetSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"X\n\x18GetSpeechContextResponse\x12<\n\x0espeech_context\x18\x01 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"k\n\x1aUpdateSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12<\n\x0espeech_context\x18\x02 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"\x1d\n\x1bUpdateSpeechContextResponse\"2\n\x11\x41\x64\x64SpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"O\n\x12\x41\x64\x64SpeakerResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"2\n\x11GetSpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x8f\x01\n\x12GetSpeakerResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x06\x61udios\x18\x03 \x03(\x0b\x32..soniox.speech_service.GetSpeakerResponseAudio\"o\n\x17GetSpeakerResponseAudio\x12\x12\n\naudio_name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x03 \x01(\x05\"5\n\x14RemoveSpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x17\n\x15RemoveSpeakerResponse\"&\n\x13ListSpeakersRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\"\\\n\x14ListSpeakersResponse\x12\x44\n\x08speakers\x18\x01 \x03(\x0b\x32\x32.soniox.speech_service.ListSpeakersResponseSpeaker\"l\n\x1bListSpeakersResponseSpeaker\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nnum_audios\x18\x03 \x01(\x05\"b\n\x16\x41\x64\x64SpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\x12\r\n\x05\x61udio\x18\x04 \x01(\x0c\"\x85\x01\n\x17\x41\x64\x64SpeakerAudioResponse\x12\x14\n\x0cspeaker_name\x18\x01 \x01(\t\x12\x12\n\naudio_name\x18\x02 \x01(\t\x12+\n\x07\x63reated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x04 \x01(\x05\"S\n\x16GetSpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\"\x94\x01\n\x17GetSpeakerAudioResponse\x12\x14\n\x0cspeaker_name\x18\x01 \x01(\t\x12\x12\n\naudio_name\x18\x02 \x01(\t\x12+\n\x07\x63reated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x04 \x01(\x05\x12\r\n\x05\x61udio\x18\x05 \x01(\x0c\"V\n\x19RemoveSpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\"\x1c\n\x1aRemoveSpeakerAudioResponse2\xa1\x12\n\rSpeechService\x12\x63\n\nTranscribe\x12(.soniox.speech_service.TranscribeRequest\x1a).soniox.speech_service.TranscribeResponse\"\x00\x12y\n\x10TranscribeStream\x12..soniox.speech_service.TranscribeStreamRequest\x1a/.soniox.speech_service.TranscribeStreamResponse\"\x00(\x01\x30\x01\x12|\n\x11TranscribeMeeting\x12/.soniox.speech_service.TranscribeMeetingRequest\x1a\x30.soniox.speech_service.TranscribeMeetingResponse\"\x00(\x01\x30\x01\x12t\n\x0fTranscribeAsync\x12-.soniox.speech_service.TranscribeAsyncRequest\x1a..soniox.speech_service.TranscribeAsyncResponse\"\x00(\x01\x12\x8d\x01\n\x18GetTranscribeAsyncStatus\x12\x36.soniox.speech_service.GetTranscribeAsyncStatusRequest\x1a\x37.soniox.speech_service.GetTranscribeAsyncStatusResponse\"\x00\x12\x8f\x01\n\x18GetTranscribeAsyncResult\x12\x36.soniox.speech_service.GetTranscribeAsyncResultRequest\x1a\x37.soniox.speech_service.GetTranscribeAsyncResultResponse\"\x00\x30\x01\x12\x90\x01\n\x19\x44\x65leteTranscribeAsyncFile\x12\x37.soniox.speech_service.DeleteTranscribeAsyncFileRequest\x1a\x38.soniox.speech_service.DeleteTranscribeAsyncFileResponse\"\x00\x12~\n\x13\x43reateSpeechContext\x12\x31.soniox.speech_service.CreateSpeechContextRequest\x1a\x32.soniox.speech_service.CreateSpeechContextResponse\"\x00\x12~\n\x13\x44\x65leteSpeechContext\x12\x31.soniox.speech_service.DeleteSpeechContextRequest\x1a\x32.soniox.speech_service.DeleteSpeechContextResponse\"\x00\x12\x87\x01\n\x16ListSpeechContextNames\x12\x34.soniox.speech_service.ListSpeechContextNamesRequest\x1a\x35.soniox.speech_service.ListSpeechContextNamesResponse\"\x00\x12u\n\x10GetSpeechContext\x12..soniox.speech_service.GetSpeechContextRequest\x1a/.soniox.speech_service.GetSpeechContextResponse\"\x00\x12~\n\x13UpdateSpeechContext\x12\x31.soniox.speech_service.UpdateSpeechContextRequest\x1a\x32.soniox.speech_service.UpdateSpeechContextResponse\"\x00\x12\x63\n\nAddSpeaker\x12(.soniox.speech_service.AddSpeakerRequest\x1a).soniox.speech_service.AddSpeakerResponse\"\x00\x12\x63\n\nGetSpeaker\x12(.soniox.speech_service.GetSpeakerRequest\x1a).soniox.speech_service.GetSpeakerResponse\"\x00\x12l\n\rRemoveSpeaker\x12+.soniox.speech_service.RemoveSpeakerRequest\x1a,.soniox.speech_service.RemoveSpeakerResponse\"\x00\x12i\n\x0cListSpeakers\x12*.soniox.speech_service.ListSpeakersRequest\x1a+.soniox.speech_service.ListSpeakersResponse\"\x00\x12r\n\x0f\x41\x64\x64SpeakerAudio\x12-.soniox.speech_service.AddSpeakerAudioRequest\x1a..soniox.speech_service.AddSpeakerAudioResponse\"\x00\x12r\n\x0fGetSpeakerAudio\x12-.soniox.speech_service.GetSpeakerAudioRequest\x1a..soniox.speech_service.GetSpeakerAudioResponse\"\x00\x12{\n\x12RemoveSpeakerAudio\x12\x30.soniox.speech_service.RemoveSpeakerAudioRequest\x1a\x31.soniox.speech_service.RemoveSpeakerAudioResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bsoniox/speech_service.proto\x12\x15soniox.speech_service\x1a\x1fgoogle/protobuf/timestamp.proto\"o\n\x11TranscribeRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\x04 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\r\n\x05\x61udio\x18\x03 \x01(\x0c\"\xbb\x01\n\x12TranscribeResponse\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12\x36\n\x0f\x63hannel_results\x18\x02 \x03(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x03 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"u\n\x17TranscribeStreamRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\x04 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\r\n\x05\x61udio\x18\x03 \x01(\x0c\"\x89\x01\n\x18TranscribeStreamResponse\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x02 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"\xcc\x01\n\x18TranscribeMeetingRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\n \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\x0f\n\x07seq_num\x18\x03 \x01(\x05\x12\x11\n\tstream_id\x18\x04 \x01(\x05\x12\x18\n\x10start_of_segment\x18\x05 \x01(\x08\x12\r\n\x05\x61udio\x18\x06 \x01(\x0c\x12\x16\n\x0e\x65nd_of_segment\x18\x07 \x01(\x08\"\xef\x01\n\x19TranscribeMeetingResponse\x12\x0f\n\x07seq_num\x18\x01 \x01(\x05\x12\x11\n\tstream_id\x18\x02 \x01(\x05\x12\x18\n\x10start_of_segment\x18\x03 \x01(\x08\x12\x16\n\x0e\x65nd_of_segment\x18\x04 \x01(\x08\x12-\n\x06result\x18\x05 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12\r\n\x05\x65rror\x18\x06 \x01(\t\x12>\n\x08metadata\x18\x07 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"\xad\x01\n\x16TranscribeAsyncRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x16\n\x0ereference_name\x18\x03 \x01(\t\x12:\n\x06\x63onfig\x18\x05 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\x12\n\nenable_eof\x18\x06 \x01(\x08\x12\x0b\n\x03\x65of\x18\x07 \x01(\x08\x12\r\n\x05\x61udio\x18\x04 \x01(\x0c\"*\n\x17TranscribeAsyncResponse\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\"C\n\x1fGetTranscribeAsyncStatusRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"c\n GetTranscribeAsyncStatusResponse\x12?\n\x05\x66iles\x18\x01 \x03(\x0b\x32\x30.soniox.speech_service.TranscribeAsyncFileStatus\"\x9d\x01\n\x19TranscribeAsyncFileStatus\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x16\n\x0ereference_name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x30\n\x0c\x63reated_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rerror_message\x18\x05 \x01(\t\"C\n\x1fGetTranscribeAsyncResultRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"\xbb\x01\n GetTranscribeAsyncResultResponse\x12(\n separate_recognition_per_channel\x18\x02 \x01(\x08\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x03 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"D\n DeleteTranscribeAsyncFileRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"#\n!DeleteTranscribeAsyncFileResponse\"\xad\x05\n\x13TranscriptionConfig\x12 \n\x18\x63lient_request_reference\x18\x13 \x01(\t\x12\x14\n\x0c\x61udio_format\x18\x01 \x01(\t\x12\x19\n\x11sample_rate_hertz\x18\x02 \x01(\x05\x12\x1a\n\x12num_audio_channels\x18\x03 \x01(\x05\x12\x18\n\x10include_nonfinal\x18\x04 \x01(\x08\x12/\n\'enable_separate_recognition_per_channel\x18\x10 \x01(\x08\x12!\n\x19\x65nable_endpoint_detection\x18\x12 \x01(\x08\x12<\n\x0espeech_context\x18\x05 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\x12\x1f\n\x17\x65nable_profanity_filter\x18\x06 \x01(\x08\x12\"\n\x1a\x63ontent_moderation_phrases\x18\x07 \x03(\t\x12,\n$enable_streaming_speaker_diarization\x18\x08 \x01(\x08\x12)\n!enable_global_speaker_diarization\x18\t \x01(\x08\x12\x18\n\x10min_num_speakers\x18\n \x01(\x05\x12\x18\n\x10max_num_speakers\x18\x0b \x01(\x05\x12%\n\x1d\x65nable_speaker_identification\x18\x0c \x01(\x08\x12\x1a\n\x12\x63\x61nd_speaker_names\x18\r \x03(\t\x12\r\n\x05model\x18\x0e \x01(\t\x12\x18\n\x10\x65nable_dictation\x18\x0f \x01(\x08\x12=\n\x0estorage_config\x18\xee\x07 \x01(\x0b\x32$.soniox.speech_service.StorageConfig\"0\n\x15TranscriptionMetadata\x12\x17\n\x0fpackage_version\x18\x01 \x01(\t\"\xb5\x01\n\x06Result\x12*\n\x05words\x18\x01 \x03(\x0b\x32\x1b.soniox.speech_service.Word\x12\x1a\n\x12\x66inal_proc_time_ms\x18\x02 \x01(\x05\x12\x1a\n\x12total_proc_time_ms\x18\x03 \x01(\x05\x12\x36\n\x08speakers\x18\x06 \x03(\x0b\x32$.soniox.speech_service.ResultSpeaker\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\x05\"\x85\x01\n\x04Word\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x10\n\x08start_ms\x18\x02 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x03 \x01(\x05\x12\x10\n\x08is_final\x18\x04 \x01(\x08\x12\x0f\n\x07speaker\x18\x05 \x01(\x05\x12\x11\n\torig_text\x18\x08 \x01(\t\x12\x12\n\nconfidence\x18\t \x01(\x01\".\n\rResultSpeaker\x12\x0f\n\x07speaker\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"Y\n\rSpeechContext\x12:\n\x07\x65ntries\x18\x01 \x03(\x0b\x32).soniox.speech_service.SpeechContextEntry\x12\x0c\n\x04name\x18\x02 \x01(\t\"4\n\x12SpeechContextEntry\x12\x0f\n\x07phrases\x18\x01 \x03(\t\x12\r\n\x05\x62oost\x18\x02 \x01(\x01\"k\n\x1a\x43reateSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12<\n\x0espeech_context\x18\x02 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"\x1d\n\x1b\x43reateSpeechContextResponse\";\n\x1a\x44\x65leteSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x1d\n\x1b\x44\x65leteSpeechContextResponse\"0\n\x1dListSpeechContextNamesRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\"/\n\x1eListSpeechContextNamesResponse\x12\r\n\x05names\x18\x01 \x03(\t\"8\n\x17GetSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"X\n\x18GetSpeechContextResponse\x12<\n\x0espeech_context\x18\x01 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"k\n\x1aUpdateSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12<\n\x0espeech_context\x18\x02 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"\x1d\n\x1bUpdateSpeechContextResponse\"2\n\x11\x41\x64\x64SpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"O\n\x12\x41\x64\x64SpeakerResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"2\n\x11GetSpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x8f\x01\n\x12GetSpeakerResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x06\x61udios\x18\x03 \x03(\x0b\x32..soniox.speech_service.GetSpeakerResponseAudio\"o\n\x17GetSpeakerResponseAudio\x12\x12\n\naudio_name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x03 \x01(\x05\"5\n\x14RemoveSpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x17\n\x15RemoveSpeakerResponse\"&\n\x13ListSpeakersRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\"\\\n\x14ListSpeakersResponse\x12\x44\n\x08speakers\x18\x01 \x03(\x0b\x32\x32.soniox.speech_service.ListSpeakersResponseSpeaker\"l\n\x1bListSpeakersResponseSpeaker\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nnum_audios\x18\x03 \x01(\x05\"b\n\x16\x41\x64\x64SpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\x12\r\n\x05\x61udio\x18\x04 \x01(\x0c\"\x85\x01\n\x17\x41\x64\x64SpeakerAudioResponse\x12\x14\n\x0cspeaker_name\x18\x01 \x01(\t\x12\x12\n\naudio_name\x18\x02 \x01(\t\x12+\n\x07\x63reated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x04 \x01(\x05\"S\n\x16GetSpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\"\x94\x01\n\x17GetSpeakerAudioResponse\x12\x14\n\x0cspeaker_name\x18\x01 \x01(\t\x12\x12\n\naudio_name\x18\x02 \x01(\t\x12+\n\x07\x63reated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x04 \x01(\x05\x12\r\n\x05\x61udio\x18\x05 \x01(\x0c\"V\n\x19RemoveSpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\"\x1c\n\x1aRemoveSpeakerAudioResponse\"\x95\x02\n\rStorageConfig\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x44\n\x08metadata\x18\x02 \x03(\x0b\x32\x32.soniox.speech_service.StorageConfig.MetadataEntry\x12\r\n\x05title\x18\x03 \x01(\t\x12,\n\x08\x64\x61tetime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13\x64isable_store_audio\x18\x05 \x01(\x08\x12 \n\x18\x64isable_store_transcript\x18\x06 \x01(\x08\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa8\x01\n\x05Token\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x12\n\ntext_start\x18\x02 \x01(\x05\x12\x10\n\x08text_end\x18\x03 \x01(\x05\x12\x0c\n\x04text\x18\x04 \x01(\t\x12\x10\n\x08start_ms\x18\x05 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x06 \x01(\x05\x12\x12\n\nconfidence\x18\x07 \x01(\x01\x12\x12\n\nspeaker_id\x18\x08 \x01(\x05\x12\x0f\n\x07profane\x18\t \x01(\x08\"2\n\x08Sentence\x12\x13\n\x0btoken_start\x18\x01 \x01(\x05\x12\x11\n\ttoken_end\x18\x02 \x01(\x05\"9\n\tParagraph\x12\x16\n\x0esentence_start\x18\x01 \x01(\x05\x12\x14\n\x0csentence_end\x18\x02 \x01(\x05\"C\n\x07Keyterm\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x01\x12\x1b\n\x13token_start_indexes\x18\x03 \x03(\x05\"\xe5\x02\n\nTranscript\x12\x0c\n\x04text\x18\x01 \x01(\t\x12,\n\x06tokens\x18\x02 \x03(\x0b\x32\x1c.soniox.speech_service.Token\x12\x32\n\tsentences\x18\x03 \x03(\x0b\x32\x1f.soniox.speech_service.Sentence\x12\x34\n\nparagraphs\x18\x04 \x03(\x0b\x32 .soniox.speech_service.Paragraph\x12\x30\n\x08keyterms\x18\x06 \x03(\x0b\x32\x1e.soniox.speech_service.Keyterm\x12J\n\rspeaker_names\x18\x07 \x03(\x0b\x32\x33.soniox.speech_service.Transcript.SpeakerNamesEntry\x1a\x33\n\x11SpeakerNamesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x87\x03\n\x0cStoredObject\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x43\n\x08metadata\x18\x02 \x03(\x0b\x32\x31.soniox.speech_service.StoredObject.MetadataEntry\x12\r\n\x05title\x18\x03 \x01(\t\x12,\n\x08\x64\x61tetime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0fstored_datetime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x06 \x01(\x05\x12\x1a\n\x12num_audio_channels\x18\n \x01(\x05\x12\x14\n\x0c\x61udio_stored\x18\x0b \x01(\x08\x12\x35\n\ntranscript\x18\x07 \x01(\x0b\x32!.soniox.speech_service.Transcript\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xdf\x01\n\rSearchRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\x12\x16\n\x0emetadata_query\x18\x03 \x01(\t\x12\x31\n\rdatetime_from\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x64\x61tetime_to\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ntext_query\x18\x06 \x01(\t\x12\r\n\x05start\x18\x07 \x01(\x05\x12\x0b\n\x03num\x18\x08 \x01(\x05\"\xfa\x01\n\x0cSearchResult\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x43\n\x08metadata\x18\x02 \x03(\x0b\x32\x31.soniox.speech_service.SearchResult.MetadataEntry\x12\r\n\x05title\x18\x03 \x01(\t\x12,\n\x08\x64\x61tetime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x05 \x01(\x05\x12\x0f\n\x07preview\x18\x06 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"h\n\x0eSearchResponse\x12\x11\n\tnum_found\x18\x01 \x01(\x05\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x34\n\x07results\x18\x03 \x03(\x0b\x32#.soniox.speech_service.SearchResult\"6\n\x10GetObjectRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\"H\n\x11GetObjectResponse\x12\x33\n\x06object\x18\x01 \x01(\x0b\x32#.soniox.speech_service.StoredObject\"\xb3\x01\n\x12ListObjectsRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x38\n\x14stored_datetime_from\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12stored_datetime_to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05start\x18\x04 \x01(\x03\x12\x0b\n\x03num\x18\x05 \x01(\x03\"g\n\x13ListObjectsResponse\x12\r\n\x05start\x18\x01 \x01(\x03\x12\x41\n\x07objects\x18\x02 \x03(\x0b\x32\x30.soniox.speech_service.ListObjectsResponseObject\"\xc8\x01\n\x19ListObjectsResponseObject\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x33\n\x0fstored_datetime\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x61udio_stored\x18\x03 \x01(\x08\x12\x19\n\x11transcript_stored\x18\x04 \x01(\x08\x12\x19\n\x11\x61udio_duration_ms\x18\x05 \x01(\x05\x12\x17\n\x0fstored_audio_ms\x18\x06 \x01(\x05\"9\n\x13\x44\x65leteObjectRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\"\x16\n\x14\x44\x65leteObjectResponse\"\xea\x02\n\x0fGetAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\x12J\n\x0ctime_segment\x18\x03 \x01(\x0b\x32\x32.soniox.speech_service.GetAudioRequest.TimeSegmentH\x00\x12L\n\rtoken_segment\x18\x04 \x01(\x0b\x32\x33.soniox.speech_service.GetAudioRequest.TokenSegmentH\x00\x12\x1a\n\x12\x61udio_bytes_format\x18\x05 \x01(\t\x1a\x34\n\x0bTimeSegment\x12\x10\n\x08start_ms\x18\x01 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x02 \x01(\x05\x1a\x36\n\x0cTokenSegment\x12\x13\n\x0btoken_start\x18\x01 \x01(\x05\x12\x11\n\ttoken_end\x18\x02 \x01(\x05\x42\x0f\n\roneof_segment\"\x91\x01\n\x10GetAudioResponse\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x10\n\x08start_ms\x18\x02 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x03 \x01(\x05\x12\x19\n\x11total_duration_ms\x18\x04 \x01(\x05\x12\x1a\n\x12num_audio_channels\x18\x06 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\x32\x90\x16\n\rSpeechService\x12\x63\n\nTranscribe\x12(.soniox.speech_service.TranscribeRequest\x1a).soniox.speech_service.TranscribeResponse\"\x00\x12y\n\x10TranscribeStream\x12..soniox.speech_service.TranscribeStreamRequest\x1a/.soniox.speech_service.TranscribeStreamResponse\"\x00(\x01\x30\x01\x12|\n\x11TranscribeMeeting\x12/.soniox.speech_service.TranscribeMeetingRequest\x1a\x30.soniox.speech_service.TranscribeMeetingResponse\"\x00(\x01\x30\x01\x12t\n\x0fTranscribeAsync\x12-.soniox.speech_service.TranscribeAsyncRequest\x1a..soniox.speech_service.TranscribeAsyncResponse\"\x00(\x01\x12\x8d\x01\n\x18GetTranscribeAsyncStatus\x12\x36.soniox.speech_service.GetTranscribeAsyncStatusRequest\x1a\x37.soniox.speech_service.GetTranscribeAsyncStatusResponse\"\x00\x12\x8f\x01\n\x18GetTranscribeAsyncResult\x12\x36.soniox.speech_service.GetTranscribeAsyncResultRequest\x1a\x37.soniox.speech_service.GetTranscribeAsyncResultResponse\"\x00\x30\x01\x12\x90\x01\n\x19\x44\x65leteTranscribeAsyncFile\x12\x37.soniox.speech_service.DeleteTranscribeAsyncFileRequest\x1a\x38.soniox.speech_service.DeleteTranscribeAsyncFileResponse\"\x00\x12~\n\x13\x43reateSpeechContext\x12\x31.soniox.speech_service.CreateSpeechContextRequest\x1a\x32.soniox.speech_service.CreateSpeechContextResponse\"\x00\x12~\n\x13\x44\x65leteSpeechContext\x12\x31.soniox.speech_service.DeleteSpeechContextRequest\x1a\x32.soniox.speech_service.DeleteSpeechContextResponse\"\x00\x12\x87\x01\n\x16ListSpeechContextNames\x12\x34.soniox.speech_service.ListSpeechContextNamesRequest\x1a\x35.soniox.speech_service.ListSpeechContextNamesResponse\"\x00\x12u\n\x10GetSpeechContext\x12..soniox.speech_service.GetSpeechContextRequest\x1a/.soniox.speech_service.GetSpeechContextResponse\"\x00\x12~\n\x13UpdateSpeechContext\x12\x31.soniox.speech_service.UpdateSpeechContextRequest\x1a\x32.soniox.speech_service.UpdateSpeechContextResponse\"\x00\x12\x63\n\nAddSpeaker\x12(.soniox.speech_service.AddSpeakerRequest\x1a).soniox.speech_service.AddSpeakerResponse\"\x00\x12\x63\n\nGetSpeaker\x12(.soniox.speech_service.GetSpeakerRequest\x1a).soniox.speech_service.GetSpeakerResponse\"\x00\x12l\n\rRemoveSpeaker\x12+.soniox.speech_service.RemoveSpeakerRequest\x1a,.soniox.speech_service.RemoveSpeakerResponse\"\x00\x12i\n\x0cListSpeakers\x12*.soniox.speech_service.ListSpeakersRequest\x1a+.soniox.speech_service.ListSpeakersResponse\"\x00\x12r\n\x0f\x41\x64\x64SpeakerAudio\x12-.soniox.speech_service.AddSpeakerAudioRequest\x1a..soniox.speech_service.AddSpeakerAudioResponse\"\x00\x12r\n\x0fGetSpeakerAudio\x12-.soniox.speech_service.GetSpeakerAudioRequest\x1a..soniox.speech_service.GetSpeakerAudioResponse\"\x00\x12{\n\x12RemoveSpeakerAudio\x12\x30.soniox.speech_service.RemoveSpeakerAudioRequest\x1a\x31.soniox.speech_service.RemoveSpeakerAudioResponse\"\x00\x12W\n\x06Search\x12$.soniox.speech_service.SearchRequest\x1a%.soniox.speech_service.SearchResponse\"\x00\x12`\n\tGetObject\x12\'.soniox.speech_service.GetObjectRequest\x1a(.soniox.speech_service.GetObjectResponse\"\x00\x12\x66\n\x0bListObjects\x12).soniox.speech_service.ListObjectsRequest\x1a*.soniox.speech_service.ListObjectsResponse\"\x00\x12i\n\x0c\x44\x65leteObject\x12*.soniox.speech_service.DeleteObjectRequest\x1a+.soniox.speech_service.DeleteObjectResponse\"\x00\x12_\n\x08GetAudio\x12&.soniox.speech_service.GetAudioRequest\x1a\'.soniox.speech_service.GetAudioResponse\"\x00\x30\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'soniox.speech_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
+  _STORAGECONFIG_METADATAENTRY._options = None
+  _STORAGECONFIG_METADATAENTRY._serialized_options = b'8\001'
+  _TRANSCRIPT_SPEAKERNAMESENTRY._options = None
+  _TRANSCRIPT_SPEAKERNAMESENTRY._serialized_options = b'8\001'
+  _STOREDOBJECT_METADATAENTRY._options = None
+  _STOREDOBJECT_METADATAENTRY._serialized_options = b'8\001'
+  _SEARCHRESULT_METADATAENTRY._options = None
+  _SEARCHRESULT_METADATAENTRY._serialized_options = b'8\001'
   _TRANSCRIBEREQUEST._serialized_start=87
   _TRANSCRIBEREQUEST._serialized_end=198
   _TRANSCRIBERESPONSE._serialized_start=201
   _TRANSCRIBERESPONSE._serialized_end=388
   _TRANSCRIBESTREAMREQUEST._serialized_start=390
   _TRANSCRIBESTREAMREQUEST._serialized_end=507
   _TRANSCRIBESTREAMRESPONSE._serialized_start=510
@@ -48,75 +56,125 @@
   _GETTRANSCRIBEASYNCRESULTRESPONSE._serialized_start=1718
   _GETTRANSCRIBEASYNCRESULTRESPONSE._serialized_end=1905
   _DELETETRANSCRIBEASYNCFILEREQUEST._serialized_start=1907
   _DELETETRANSCRIBEASYNCFILEREQUEST._serialized_end=1975
   _DELETETRANSCRIBEASYNCFILERESPONSE._serialized_start=1977
   _DELETETRANSCRIBEASYNCFILERESPONSE._serialized_end=2012
   _TRANSCRIPTIONCONFIG._serialized_start=2015
-  _TRANSCRIPTIONCONFIG._serialized_end=2637
-  _TRANSCRIPTIONMETADATA._serialized_start=2639
-  _TRANSCRIPTIONMETADATA._serialized_end=2687
-  _RESULT._serialized_start=2690
-  _RESULT._serialized_end=2871
-  _WORD._serialized_start=2874
-  _WORD._serialized_end=3007
-  _RESULTSPEAKER._serialized_start=3009
-  _RESULTSPEAKER._serialized_end=3055
-  _SPEECHCONTEXT._serialized_start=3057
-  _SPEECHCONTEXT._serialized_end=3146
-  _SPEECHCONTEXTENTRY._serialized_start=3148
-  _SPEECHCONTEXTENTRY._serialized_end=3200
-  _CREATESPEECHCONTEXTREQUEST._serialized_start=3202
-  _CREATESPEECHCONTEXTREQUEST._serialized_end=3309
-  _CREATESPEECHCONTEXTRESPONSE._serialized_start=3311
-  _CREATESPEECHCONTEXTRESPONSE._serialized_end=3340
-  _DELETESPEECHCONTEXTREQUEST._serialized_start=3342
-  _DELETESPEECHCONTEXTREQUEST._serialized_end=3401
-  _DELETESPEECHCONTEXTRESPONSE._serialized_start=3403
-  _DELETESPEECHCONTEXTRESPONSE._serialized_end=3432
-  _LISTSPEECHCONTEXTNAMESREQUEST._serialized_start=3434
-  _LISTSPEECHCONTEXTNAMESREQUEST._serialized_end=3482
-  _LISTSPEECHCONTEXTNAMESRESPONSE._serialized_start=3484
-  _LISTSPEECHCONTEXTNAMESRESPONSE._serialized_end=3531
-  _GETSPEECHCONTEXTREQUEST._serialized_start=3533
-  _GETSPEECHCONTEXTREQUEST._serialized_end=3589
-  _GETSPEECHCONTEXTRESPONSE._serialized_start=3591
-  _GETSPEECHCONTEXTRESPONSE._serialized_end=3679
-  _UPDATESPEECHCONTEXTREQUEST._serialized_start=3681
-  _UPDATESPEECHCONTEXTREQUEST._serialized_end=3788
-  _UPDATESPEECHCONTEXTRESPONSE._serialized_start=3790
-  _UPDATESPEECHCONTEXTRESPONSE._serialized_end=3819
-  _ADDSPEAKERREQUEST._serialized_start=3821
-  _ADDSPEAKERREQUEST._serialized_end=3871
-  _ADDSPEAKERRESPONSE._serialized_start=3873
-  _ADDSPEAKERRESPONSE._serialized_end=3952
-  _GETSPEAKERREQUEST._serialized_start=3954
-  _GETSPEAKERREQUEST._serialized_end=4004
-  _GETSPEAKERRESPONSE._serialized_start=4007
-  _GETSPEAKERRESPONSE._serialized_end=4150
-  _GETSPEAKERRESPONSEAUDIO._serialized_start=4152
-  _GETSPEAKERRESPONSEAUDIO._serialized_end=4263
-  _REMOVESPEAKERREQUEST._serialized_start=4265
-  _REMOVESPEAKERREQUEST._serialized_end=4318
-  _REMOVESPEAKERRESPONSE._serialized_start=4320
-  _REMOVESPEAKERRESPONSE._serialized_end=4343
-  _LISTSPEAKERSREQUEST._serialized_start=4345
-  _LISTSPEAKERSREQUEST._serialized_end=4383
-  _LISTSPEAKERSRESPONSE._serialized_start=4385
-  _LISTSPEAKERSRESPONSE._serialized_end=4477
-  _LISTSPEAKERSRESPONSESPEAKER._serialized_start=4479
-  _LISTSPEAKERSRESPONSESPEAKER._serialized_end=4587
-  _ADDSPEAKERAUDIOREQUEST._serialized_start=4589
-  _ADDSPEAKERAUDIOREQUEST._serialized_end=4687
-  _ADDSPEAKERAUDIORESPONSE._serialized_start=4690
-  _ADDSPEAKERAUDIORESPONSE._serialized_end=4823
-  _GETSPEAKERAUDIOREQUEST._serialized_start=4825
-  _GETSPEAKERAUDIOREQUEST._serialized_end=4908
-  _GETSPEAKERAUDIORESPONSE._serialized_start=4911
-  _GETSPEAKERAUDIORESPONSE._serialized_end=5059
-  _REMOVESPEAKERAUDIOREQUEST._serialized_start=5061
-  _REMOVESPEAKERAUDIOREQUEST._serialized_end=5147
-  _REMOVESPEAKERAUDIORESPONSE._serialized_start=5149
-  _REMOVESPEAKERAUDIORESPONSE._serialized_end=5177
-  _SPEECHSERVICE._serialized_start=5180
-  _SPEECHSERVICE._serialized_end=7517
+  _TRANSCRIPTIONCONFIG._serialized_end=2700
+  _TRANSCRIPTIONMETADATA._serialized_start=2702
+  _TRANSCRIPTIONMETADATA._serialized_end=2750
+  _RESULT._serialized_start=2753
+  _RESULT._serialized_end=2934
+  _WORD._serialized_start=2937
+  _WORD._serialized_end=3070
+  _RESULTSPEAKER._serialized_start=3072
+  _RESULTSPEAKER._serialized_end=3118
+  _SPEECHCONTEXT._serialized_start=3120
+  _SPEECHCONTEXT._serialized_end=3209
+  _SPEECHCONTEXTENTRY._serialized_start=3211
+  _SPEECHCONTEXTENTRY._serialized_end=3263
+  _CREATESPEECHCONTEXTREQUEST._serialized_start=3265
+  _CREATESPEECHCONTEXTREQUEST._serialized_end=3372
+  _CREATESPEECHCONTEXTRESPONSE._serialized_start=3374
+  _CREATESPEECHCONTEXTRESPONSE._serialized_end=3403
+  _DELETESPEECHCONTEXTREQUEST._serialized_start=3405
+  _DELETESPEECHCONTEXTREQUEST._serialized_end=3464
+  _DELETESPEECHCONTEXTRESPONSE._serialized_start=3466
+  _DELETESPEECHCONTEXTRESPONSE._serialized_end=3495
+  _LISTSPEECHCONTEXTNAMESREQUEST._serialized_start=3497
+  _LISTSPEECHCONTEXTNAMESREQUEST._serialized_end=3545
+  _LISTSPEECHCONTEXTNAMESRESPONSE._serialized_start=3547
+  _LISTSPEECHCONTEXTNAMESRESPONSE._serialized_end=3594
+  _GETSPEECHCONTEXTREQUEST._serialized_start=3596
+  _GETSPEECHCONTEXTREQUEST._serialized_end=3652
+  _GETSPEECHCONTEXTRESPONSE._serialized_start=3654
+  _GETSPEECHCONTEXTRESPONSE._serialized_end=3742
+  _UPDATESPEECHCONTEXTREQUEST._serialized_start=3744
+  _UPDATESPEECHCONTEXTREQUEST._serialized_end=3851
+  _UPDATESPEECHCONTEXTRESPONSE._serialized_start=3853
+  _UPDATESPEECHCONTEXTRESPONSE._serialized_end=3882
+  _ADDSPEAKERREQUEST._serialized_start=3884
+  _ADDSPEAKERREQUEST._serialized_end=3934
+  _ADDSPEAKERRESPONSE._serialized_start=3936
+  _ADDSPEAKERRESPONSE._serialized_end=4015
+  _GETSPEAKERREQUEST._serialized_start=4017
+  _GETSPEAKERREQUEST._serialized_end=4067
+  _GETSPEAKERRESPONSE._serialized_start=4070
+  _GETSPEAKERRESPONSE._serialized_end=4213
+  _GETSPEAKERRESPONSEAUDIO._serialized_start=4215
+  _GETSPEAKERRESPONSEAUDIO._serialized_end=4326
+  _REMOVESPEAKERREQUEST._serialized_start=4328
+  _REMOVESPEAKERREQUEST._serialized_end=4381
+  _REMOVESPEAKERRESPONSE._serialized_start=4383
+  _REMOVESPEAKERRESPONSE._serialized_end=4406
+  _LISTSPEAKERSREQUEST._serialized_start=4408
+  _LISTSPEAKERSREQUEST._serialized_end=4446
+  _LISTSPEAKERSRESPONSE._serialized_start=4448
+  _LISTSPEAKERSRESPONSE._serialized_end=4540
+  _LISTSPEAKERSRESPONSESPEAKER._serialized_start=4542
+  _LISTSPEAKERSRESPONSESPEAKER._serialized_end=4650
+  _ADDSPEAKERAUDIOREQUEST._serialized_start=4652
+  _ADDSPEAKERAUDIOREQUEST._serialized_end=4750
+  _ADDSPEAKERAUDIORESPONSE._serialized_start=4753
+  _ADDSPEAKERAUDIORESPONSE._serialized_end=4886
+  _GETSPEAKERAUDIOREQUEST._serialized_start=4888
+  _GETSPEAKERAUDIOREQUEST._serialized_end=4971
+  _GETSPEAKERAUDIORESPONSE._serialized_start=4974
+  _GETSPEAKERAUDIORESPONSE._serialized_end=5122
+  _REMOVESPEAKERAUDIOREQUEST._serialized_start=5124
+  _REMOVESPEAKERAUDIOREQUEST._serialized_end=5210
+  _REMOVESPEAKERAUDIORESPONSE._serialized_start=5212
+  _REMOVESPEAKERAUDIORESPONSE._serialized_end=5240
+  _STORAGECONFIG._serialized_start=5243
+  _STORAGECONFIG._serialized_end=5520
+  _STORAGECONFIG_METADATAENTRY._serialized_start=5473
+  _STORAGECONFIG_METADATAENTRY._serialized_end=5520
+  _TOKEN._serialized_start=5523
+  _TOKEN._serialized_end=5691
+  _SENTENCE._serialized_start=5693
+  _SENTENCE._serialized_end=5743
+  _PARAGRAPH._serialized_start=5745
+  _PARAGRAPH._serialized_end=5802
+  _KEYTERM._serialized_start=5804
+  _KEYTERM._serialized_end=5871
+  _TRANSCRIPT._serialized_start=5874
+  _TRANSCRIPT._serialized_end=6231
+  _TRANSCRIPT_SPEAKERNAMESENTRY._serialized_start=6180
+  _TRANSCRIPT_SPEAKERNAMESENTRY._serialized_end=6231
+  _STOREDOBJECT._serialized_start=6234
+  _STOREDOBJECT._serialized_end=6625
+  _STOREDOBJECT_METADATAENTRY._serialized_start=5473
+  _STOREDOBJECT_METADATAENTRY._serialized_end=5520
+  _SEARCHREQUEST._serialized_start=6628
+  _SEARCHREQUEST._serialized_end=6851
+  _SEARCHRESULT._serialized_start=6854
+  _SEARCHRESULT._serialized_end=7104
+  _SEARCHRESULT_METADATAENTRY._serialized_start=5473
+  _SEARCHRESULT_METADATAENTRY._serialized_end=5520
+  _SEARCHRESPONSE._serialized_start=7106
+  _SEARCHRESPONSE._serialized_end=7210
+  _GETOBJECTREQUEST._serialized_start=7212
+  _GETOBJECTREQUEST._serialized_end=7266
+  _GETOBJECTRESPONSE._serialized_start=7268
+  _GETOBJECTRESPONSE._serialized_end=7340
+  _LISTOBJECTSREQUEST._serialized_start=7343
+  _LISTOBJECTSREQUEST._serialized_end=7522
+  _LISTOBJECTSRESPONSE._serialized_start=7524
+  _LISTOBJECTSRESPONSE._serialized_end=7627
+  _LISTOBJECTSRESPONSEOBJECT._serialized_start=7630
+  _LISTOBJECTSRESPONSEOBJECT._serialized_end=7830
+  _DELETEOBJECTREQUEST._serialized_start=7832
+  _DELETEOBJECTREQUEST._serialized_end=7889
+  _DELETEOBJECTRESPONSE._serialized_start=7891
+  _DELETEOBJECTRESPONSE._serialized_end=7913
+  _GETAUDIOREQUEST._serialized_start=7916
+  _GETAUDIOREQUEST._serialized_end=8278
+  _GETAUDIOREQUEST_TIMESEGMENT._serialized_start=8153
+  _GETAUDIOREQUEST_TIMESEGMENT._serialized_end=8205
+  _GETAUDIOREQUEST_TOKENSEGMENT._serialized_start=8207
+  _GETAUDIOREQUEST_TOKENSEGMENT._serialized_end=8261
+  _GETAUDIORESPONSE._serialized_start=8281
+  _GETAUDIORESPONSE._serialized_end=8426
+  _SPEECHSERVICE._serialized_start=8429
+  _SPEECHSERVICE._serialized_end=11261
 # @@protoc_insertion_point(module_scope)
```

### Comparing `soniox-1.6.2/soniox/speech_service_pb2_grpc.py` & `soniox-1.7.0/soniox/speech_service_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,14 +105,39 @@
                 response_deserializer=soniox_dot_speech__service__pb2.GetSpeakerAudioResponse.FromString,
                 )
         self.RemoveSpeakerAudio = channel.unary_unary(
                 '/soniox.speech_service.SpeechService/RemoveSpeakerAudio',
                 request_serializer=soniox_dot_speech__service__pb2.RemoveSpeakerAudioRequest.SerializeToString,
                 response_deserializer=soniox_dot_speech__service__pb2.RemoveSpeakerAudioResponse.FromString,
                 )
+        self.Search = channel.unary_unary(
+                '/soniox.speech_service.SpeechService/Search',
+                request_serializer=soniox_dot_speech__service__pb2.SearchRequest.SerializeToString,
+                response_deserializer=soniox_dot_speech__service__pb2.SearchResponse.FromString,
+                )
+        self.GetObject = channel.unary_unary(
+                '/soniox.speech_service.SpeechService/GetObject',
+                request_serializer=soniox_dot_speech__service__pb2.GetObjectRequest.SerializeToString,
+                response_deserializer=soniox_dot_speech__service__pb2.GetObjectResponse.FromString,
+                )
+        self.ListObjects = channel.unary_unary(
+                '/soniox.speech_service.SpeechService/ListObjects',
+                request_serializer=soniox_dot_speech__service__pb2.ListObjectsRequest.SerializeToString,
+                response_deserializer=soniox_dot_speech__service__pb2.ListObjectsResponse.FromString,
+                )
+        self.DeleteObject = channel.unary_unary(
+                '/soniox.speech_service.SpeechService/DeleteObject',
+                request_serializer=soniox_dot_speech__service__pb2.DeleteObjectRequest.SerializeToString,
+                response_deserializer=soniox_dot_speech__service__pb2.DeleteObjectResponse.FromString,
+                )
+        self.GetAudio = channel.unary_stream(
+                '/soniox.speech_service.SpeechService/GetAudio',
+                request_serializer=soniox_dot_speech__service__pb2.GetAudioRequest.SerializeToString,
+                response_deserializer=soniox_dot_speech__service__pb2.GetAudioResponse.FromString,
+                )
 
 
 class SpeechServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Transcribe(self, request, context):
         """Synchronous transcription
@@ -228,14 +253,45 @@
 
     def RemoveSpeakerAudio(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def Search(self, request, context):
+        """Storage
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetObject(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ListObjects(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteObject(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetAudio(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_SpeechServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Transcribe': grpc.unary_unary_rpc_method_handler(
                     servicer.Transcribe,
                     request_deserializer=soniox_dot_speech__service__pb2.TranscribeRequest.FromString,
                     response_serializer=soniox_dot_speech__service__pb2.TranscribeResponse.SerializeToString,
@@ -326,14 +382,39 @@
                     response_serializer=soniox_dot_speech__service__pb2.GetSpeakerAudioResponse.SerializeToString,
             ),
             'RemoveSpeakerAudio': grpc.unary_unary_rpc_method_handler(
                     servicer.RemoveSpeakerAudio,
                     request_deserializer=soniox_dot_speech__service__pb2.RemoveSpeakerAudioRequest.FromString,
                     response_serializer=soniox_dot_speech__service__pb2.RemoveSpeakerAudioResponse.SerializeToString,
             ),
+            'Search': grpc.unary_unary_rpc_method_handler(
+                    servicer.Search,
+                    request_deserializer=soniox_dot_speech__service__pb2.SearchRequest.FromString,
+                    response_serializer=soniox_dot_speech__service__pb2.SearchResponse.SerializeToString,
+            ),
+            'GetObject': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetObject,
+                    request_deserializer=soniox_dot_speech__service__pb2.GetObjectRequest.FromString,
+                    response_serializer=soniox_dot_speech__service__pb2.GetObjectResponse.SerializeToString,
+            ),
+            'ListObjects': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListObjects,
+                    request_deserializer=soniox_dot_speech__service__pb2.ListObjectsRequest.FromString,
+                    response_serializer=soniox_dot_speech__service__pb2.ListObjectsResponse.SerializeToString,
+            ),
+            'DeleteObject': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteObject,
+                    request_deserializer=soniox_dot_speech__service__pb2.DeleteObjectRequest.FromString,
+                    response_serializer=soniox_dot_speech__service__pb2.DeleteObjectResponse.SerializeToString,
+            ),
+            'GetAudio': grpc.unary_stream_rpc_method_handler(
+                    servicer.GetAudio,
+                    request_deserializer=soniox_dot_speech__service__pb2.GetAudioRequest.FromString,
+                    response_serializer=soniox_dot_speech__service__pb2.GetAudioResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'soniox.speech_service.SpeechService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -658,7 +739,92 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/soniox.speech_service.SpeechService/RemoveSpeakerAudio',
             soniox_dot_speech__service__pb2.RemoveSpeakerAudioRequest.SerializeToString,
             soniox_dot_speech__service__pb2.RemoveSpeakerAudioResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Search(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/soniox.speech_service.SpeechService/Search',
+            soniox_dot_speech__service__pb2.SearchRequest.SerializeToString,
+            soniox_dot_speech__service__pb2.SearchResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetObject(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/soniox.speech_service.SpeechService/GetObject',
+            soniox_dot_speech__service__pb2.GetObjectRequest.SerializeToString,
+            soniox_dot_speech__service__pb2.GetObjectResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListObjects(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/soniox.speech_service.SpeechService/ListObjects',
+            soniox_dot_speech__service__pb2.ListObjectsRequest.SerializeToString,
+            soniox_dot_speech__service__pb2.ListObjectsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteObject(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/soniox.speech_service.SpeechService/DeleteObject',
+            soniox_dot_speech__service__pb2.DeleteObjectRequest.SerializeToString,
+            soniox_dot_speech__service__pb2.DeleteObjectResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetAudio(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/soniox.speech_service.SpeechService/GetAudio',
+            soniox_dot_speech__service__pb2.GetAudioRequest.SerializeToString,
+            soniox_dot_speech__service__pb2.GetAudioResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `soniox-1.6.2/soniox/transcribe_file.py` & `soniox-1.7.0/soniox/transcribe_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional, Iterable, List, Union
 from soniox.speech_service import (
     SpeechClient,
     Result,
     TranscriptionConfig,
     SpeechContext,
+    StorageConfig,
 )
 
 READ_CHUNK_SIZE = 131072
 
 
 def iter_file_chunks(file_path: str, chunk_size: int = READ_CHUNK_SIZE) -> Iterable[bytes]:
     assert isinstance(file_path, str)
@@ -47,14 +48,15 @@
     max_num_speakers: int = 0,
     enable_speaker_identification: bool = False,
     cand_speaker_names: Optional[List[str]] = None,
     enable_separate_recognition_per_channel: bool = False,
     model: str = "",
     enable_dictation: bool = False,
     enable_endpoint_detection: bool = False,
+    storage_config: Optional[StorageConfig] = None,
     client_request_reference: str = "",
 ) -> Union[Result, List[Result]]:
     assert isinstance(file_path, str)
 
     with open(file_path, "rb") as fh:
         audio = fh.read()
 
@@ -73,14 +75,15 @@
         max_num_speakers,
         enable_speaker_identification,
         cand_speaker_names,
         enable_separate_recognition_per_channel,
         model,
         enable_dictation,
         enable_endpoint_detection,
+        storage_config,
         client_request_reference,
     )
 
 
 def transcribe_bytes_short(
     audio: bytes,
     client: SpeechClient,
@@ -96,14 +99,15 @@
     max_num_speakers: int = 0,
     enable_speaker_identification: bool = False,
     cand_speaker_names: Optional[List[str]] = None,
     enable_separate_recognition_per_channel: bool = False,
     model: str = "",
     enable_dictation: bool = False,
     enable_endpoint_detection: bool = False,
+    storage_config: Optional[StorageConfig] = None,
     client_request_reference: str = "",
 ) -> Union[Result, List[Result]]:
     assert isinstance(audio, bytes)
     assert isinstance(client, SpeechClient)
     assert isinstance(sample_rate_hertz, int)
     assert isinstance(num_audio_channels, int)
     assert speech_context is None or isinstance(speech_context, SpeechContext)
@@ -119,14 +123,15 @@
     if cand_speaker_names is not None:
         assert isinstance(cand_speaker_names, list)
         assert all(isinstance(name, str) for name in cand_speaker_names)
     assert isinstance(enable_separate_recognition_per_channel, bool)
     assert isinstance(model, str)
     assert isinstance(enable_dictation, bool)
     assert isinstance(enable_endpoint_detection, bool)
+    assert storage_config is None or isinstance(storage_config, StorageConfig)
     assert isinstance(client_request_reference, str)
 
     config = TranscriptionConfig()
     config.audio_format = audio_format
     config.sample_rate_hertz = sample_rate_hertz
     config.num_audio_channels = num_audio_channels
     if speech_context is not None:
@@ -141,14 +146,16 @@
     config.enable_speaker_identification = enable_speaker_identification
     if cand_speaker_names is not None:
         config.cand_speaker_names.extend(cand_speaker_names)
     config.enable_separate_recognition_per_channel = enable_separate_recognition_per_channel
     config.model = model
     config.enable_dictation = enable_dictation
     config.enable_endpoint_detection = enable_endpoint_detection
+    if storage_config is not None:
+        config.storage_config.CopyFrom(storage_config)
     config.client_request_reference = client_request_reference
 
     return client.Transcribe(config, audio)
 
 
 def transcribe_file_stream(
     file_path: str,
@@ -165,14 +172,15 @@
     max_num_speakers: int = 0,
     enable_speaker_identification: bool = False,
     cand_speaker_names: Optional[List[str]] = None,
     enable_separate_recognition_per_channel: bool = False,
     model: str = "",
     enable_dictation: bool = False,
     enable_endpoint_detection: bool = False,
+    storage_config: Optional[StorageConfig] = None,
     client_request_reference: str = "",
     chunk_size: int = READ_CHUNK_SIZE,
 ) -> Union[Result, List[Result]]:
     return transcribe_iter_bytes_stream(
         iter_file_chunks(file_path, chunk_size),
         client,
         audio_format,
@@ -187,14 +195,15 @@
         max_num_speakers,
         enable_speaker_identification,
         cand_speaker_names,
         enable_separate_recognition_per_channel,
         model,
         enable_dictation,
         enable_endpoint_detection,
+        storage_config,
         client_request_reference,
     )
 
 
 def transcribe_bytes_stream(
     audio: bytes,
     client: SpeechClient,
@@ -210,14 +219,15 @@
     max_num_speakers: int = 0,
     enable_speaker_identification: bool = False,
     cand_speaker_names: Optional[List[str]] = None,
     enable_separate_recognition_per_channel: bool = False,
     model: str = "",
     enable_dictation: bool = False,
     enable_endpoint_detection: bool = False,
+    storage_config: Optional[StorageConfig] = None,
     client_request_reference: str = "",
     chunk_size: int = READ_CHUNK_SIZE,
 ) -> Union[Result, List[Result]]:
     return transcribe_iter_bytes_stream(
         iter_bytes_chunks(audio, chunk_size),
         client,
         audio_format,
@@ -232,14 +242,15 @@
         max_num_speakers,
         enable_speaker_identification,
         cand_speaker_names,
         enable_separate_recognition_per_channel,
         model,
         enable_dictation,
         enable_endpoint_detection,
+        storage_config,
         client_request_reference,
     )
 
 
 def transcribe_iter_bytes_stream(
     iter_audio: Iterable[bytes],
     client: SpeechClient,
@@ -255,14 +266,15 @@
     max_num_speakers: int = 0,
     enable_speaker_identification: bool = False,
     cand_speaker_names: Optional[List[str]] = None,
     enable_separate_recognition_per_channel: bool = False,
     model: str = "",
     enable_dictation: bool = False,
     enable_endpoint_detection: bool = False,
+    storage_config: Optional[StorageConfig] = None,
     client_request_reference: str = "",
 ) -> Union[Result, List[Result]]:
     assert isinstance(client, SpeechClient)
     assert isinstance(sample_rate_hertz, int)
     assert isinstance(num_audio_channels, int)
     assert speech_context is None or isinstance(speech_context, SpeechContext)
     assert isinstance(enable_profanity_filter, bool)
@@ -277,14 +289,15 @@
     if cand_speaker_names is not None:
         assert isinstance(cand_speaker_names, list)
         assert all(isinstance(name, str) for name in cand_speaker_names)
     assert isinstance(enable_separate_recognition_per_channel, bool)
     assert isinstance(model, str)
     assert isinstance(enable_dictation, bool)
     assert isinstance(enable_endpoint_detection, bool)
+    assert storage_config is None or isinstance(storage_config, StorageConfig)
     assert isinstance(client_request_reference, str)
 
     config = TranscriptionConfig()
     config.audio_format = audio_format
     config.sample_rate_hertz = sample_rate_hertz
     config.num_audio_channels = num_audio_channels
     if speech_context is not None:
@@ -299,14 +312,16 @@
     config.enable_speaker_identification = enable_speaker_identification
     if cand_speaker_names is not None:
         config.cand_speaker_names.extend(cand_speaker_names)
     config.enable_separate_recognition_per_channel = enable_separate_recognition_per_channel
     config.model = model
     config.enable_dictation = enable_dictation
     config.enable_endpoint_detection = enable_endpoint_detection
+    if storage_config is not None:
+        config.storage_config.CopyFrom(storage_config)
     config.client_request_reference = client_request_reference
 
     return client.TranscribeCompleteStream(config, iter_audio)
 
 
 def transcribe_file_async(
     file_path: str,
@@ -324,14 +339,15 @@
     enable_speaker_identification: bool = False,
     cand_speaker_names: Optional[List[str]] = None,
     enable_separate_recognition_per_channel: bool = False,
     model: str = "",
     enable_dictation: bool = False,
     enable_endpoint_detection: bool = False,
     reference_name: str = "",
+    storage_config: Optional[StorageConfig] = None,
     client_request_reference: str = "",
     chunk_size: int = READ_CHUNK_SIZE,
 ) -> str:
     assert isinstance(client, SpeechClient)
     assert isinstance(sample_rate_hertz, int)
     assert isinstance(num_audio_channels, int)
     assert speech_context is None or isinstance(speech_context, SpeechContext)
@@ -347,14 +363,15 @@
     if cand_speaker_names is not None:
         assert isinstance(cand_speaker_names, list)
         assert all(isinstance(name, str) for name in cand_speaker_names)
     assert isinstance(enable_separate_recognition_per_channel, bool)
     assert isinstance(model, str)
     assert isinstance(enable_dictation, bool)
     assert isinstance(enable_endpoint_detection, bool)
+    assert storage_config is None or isinstance(storage_config, StorageConfig)
     assert isinstance(reference_name, str)
     assert isinstance(client_request_reference, str)
 
     config = TranscriptionConfig()
     config.audio_format = audio_format
     config.sample_rate_hertz = sample_rate_hertz
     config.num_audio_channels = num_audio_channels
@@ -370,10 +387,12 @@
     config.enable_speaker_identification = enable_speaker_identification
     if cand_speaker_names is not None:
         config.cand_speaker_names.extend(cand_speaker_names)
     config.enable_separate_recognition_per_channel = enable_separate_recognition_per_channel
     config.model = model
     config.enable_dictation = enable_dictation
     config.enable_endpoint_detection = enable_endpoint_detection
+    if storage_config is not None:
+        config.storage_config.CopyFrom(storage_config)
     config.client_request_reference = client_request_reference
 
     return client.TranscribeAsync(reference_name, iter_file_chunks(file_path, chunk_size), config)
```

### Comparing `soniox-1.6.2/soniox/transcribe_live.py` & `soniox-1.7.0/soniox/transcribe_live.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     SAMPLE_RATE,
 )
 from soniox.speech_service import (
     SpeechClient,
     TranscriptionConfig,
     Result,
     SpeechContext,
+    StorageConfig,
 )
 
 
 def transcribe_capture(
     capture_device: AbstractCaptureDevice,
     client: SpeechClient,
     include_nonfinal: bool = True,
@@ -27,14 +28,15 @@
     min_num_speakers: int = 0,
     max_num_speakers: int = 0,
     enable_speaker_identification: bool = False,
     cand_speaker_names: Optional[List[str]] = None,
     model: str = "",
     enable_dictation: bool = False,
     enable_endpoint_detection: bool = False,
+    storage_config: Optional[StorageConfig] = None,
     client_request_reference: str = "",
 ) -> Iterable[Result]:
     assert isinstance(capture_device, AbstractCaptureDevice)
     assert isinstance(client, SpeechClient)
     assert isinstance(include_nonfinal, bool)
     assert speech_context is None or isinstance(speech_context, SpeechContext)
     assert isinstance(enable_profanity_filter, bool)
@@ -48,14 +50,15 @@
     assert isinstance(enable_speaker_identification, bool)
     if cand_speaker_names is not None:
         assert isinstance(cand_speaker_names, list)
         assert all(isinstance(name, str) for name in cand_speaker_names)
     assert isinstance(model, str)
     assert isinstance(enable_dictation, bool)
     assert isinstance(enable_endpoint_detection, bool)
+    assert storage_config is None or isinstance(storage_config, StorageConfig)
     assert isinstance(client_request_reference, str)
 
     config = TranscriptionConfig()
     config.audio_format = "pcm_s16le"
     config.sample_rate_hertz = SAMPLE_RATE
     config.num_audio_channels = NUM_CHANNELS
     config.include_nonfinal = include_nonfinal
@@ -70,14 +73,16 @@
     config.max_num_speakers = max_num_speakers
     config.enable_speaker_identification = enable_speaker_identification
     if cand_speaker_names is not None:
         config.cand_speaker_names.extend(cand_speaker_names)
     config.model = model
     config.enable_dictation = enable_dictation
     config.enable_endpoint_detection = enable_endpoint_detection
+    if storage_config is not None:
+        config.storage_config.CopyFrom(storage_config)
     config.client_request_reference = client_request_reference
 
     if stop_event is None:
         stop_event = threading.Event()
 
     with capture_device:
 
@@ -103,14 +108,15 @@
     min_num_speakers: int = 0,
     max_num_speakers: int = 0,
     enable_speaker_identification: bool = False,
     cand_speaker_names: Optional[List[str]] = None,
     model: str = "",
     enable_dictation: bool = False,
     enable_endpoint_detection: bool = False,
+    storage_config: Optional[StorageConfig] = None,
     client_request_reference: str = "",
 ):
     return transcribe_capture(
         MicrophoneCaptureDevice(),
         client,
         include_nonfinal,
         speech_context,
@@ -122,14 +128,15 @@
         min_num_speakers,
         max_num_speakers,
         enable_speaker_identification,
         cand_speaker_names,
         model,
         enable_dictation,
         enable_endpoint_detection,
+        storage_config,
         client_request_reference,
     )
 
 
 def transcribe_stream(
     iter_audio: Iterable[bytes],
     client: SpeechClient,
@@ -146,14 +153,15 @@
     enable_speaker_identification: bool = False,
     cand_speaker_names: Optional[List[str]] = None,
     enable_separate_recognition_per_channel: bool = False,
     model: str = "",
     enable_dictation: bool = False,
     enable_endpoint_detection: bool = False,
     include_nonfinal: bool = True,
+    storage_config: Optional[StorageConfig] = None,
     client_request_reference: str = "",
 ) -> Iterable[Result]:
     assert isinstance(client, SpeechClient)
     assert isinstance(sample_rate_hertz, int)
     assert isinstance(num_audio_channels, int)
     assert speech_context is None or isinstance(speech_context, SpeechContext)
     assert isinstance(enable_profanity_filter, bool)
@@ -169,14 +177,15 @@
         assert isinstance(cand_speaker_names, list)
         assert all(isinstance(name, str) for name in cand_speaker_names)
     assert isinstance(enable_separate_recognition_per_channel, bool)
     assert isinstance(model, str)
     assert isinstance(enable_dictation, bool)
     assert isinstance(enable_endpoint_detection, bool)
     assert isinstance(include_nonfinal, bool)
+    assert storage_config is None or isinstance(storage_config, StorageConfig)
     assert isinstance(client_request_reference, str)
 
     config = TranscriptionConfig()
     config.audio_format = audio_format
     config.sample_rate_hertz = sample_rate_hertz
     config.num_audio_channels = num_audio_channels
     config.include_nonfinal = include_nonfinal
@@ -192,10 +201,12 @@
     config.enable_speaker_identification = enable_speaker_identification
     if cand_speaker_names is not None:
         config.cand_speaker_names.extend(cand_speaker_names)
     config.enable_separate_recognition_per_channel = enable_separate_recognition_per_channel
     config.model = model
     config.enable_dictation = enable_dictation
     config.enable_endpoint_detection = enable_endpoint_detection
+    if storage_config is not None:
+        config.storage_config.CopyFrom(storage_config)
     config.client_request_reference = client_request_reference
 
     yield from client.TranscribeStream(config, iter_audio)
```

### Comparing `soniox-1.6.2/soniox.egg-info/PKG-INFO` & `soniox-1.7.0/soniox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soniox
-Version: 1.6.2
+Version: 1.7.0
 Summary: Soniox speech recognition service client library
 Home-page: https://soniox.com/
 Author: Soniox Inc
 Author-email: support@soniox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

