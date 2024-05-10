# Comparing `tmp/MLLPStreamingClient-1.0.0.tar.gz` & `tmp/mllpstreamingclient-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLLPStreamingClient-1.0.0.tar", last modified: Fri Jan  5 00:31:21 2024, max compression
+gzip compressed data, was "mllpstreamingclient-1.0.1.tar", last modified: Fri May 10 11:35:32 2024, max compression
```

## Comparing `MLLPStreamingClient-1.0.0.tar` & `mllpstreamingclient-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-01-05 00:31:21.010697 MLLPStreamingClient-1.0.0/
-drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-01-05 00:31:21.010697 MLLPStreamingClient-1.0.0/MLLPStreamingClient/
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)    40375 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/MLLPStreamingClient/MLLPStreamingClient.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)      106 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/MLLPStreamingClient/__init__.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)    10032 2024-01-05 00:31:20.000000 MLLPStreamingClient-1.0.0/MLLPStreamingClient/mllp_streaming_pb2.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)    35341 2024-01-05 00:31:20.000000 MLLPStreamingClient-1.0.0/MLLPStreamingClient/mllp_streaming_pb2_grpc.py
-drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-01-05 00:31:21.010697 MLLPStreamingClient-1.0.0/MLLPStreamingClient.egg-info/
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)    14629 2024-01-05 00:31:20.000000 MLLPStreamingClient-1.0.0/MLLPStreamingClient.egg-info/PKG-INFO
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)      765 2024-01-05 00:31:20.000000 MLLPStreamingClient-1.0.0/MLLPStreamingClient.egg-info/SOURCES.txt
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)        1 2024-01-05 00:31:20.000000 MLLPStreamingClient-1.0.0/MLLPStreamingClient.egg-info/dependency_links.txt
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       83 2024-01-05 00:31:20.000000 MLLPStreamingClient-1.0.0/MLLPStreamingClient.egg-info/requires.txt
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       20 2024-01-05 00:31:20.000000 MLLPStreamingClient-1.0.0/MLLPStreamingClient.egg-info/top_level.txt
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)    14629 2024-01-05 00:31:21.010697 MLLPStreamingClient-1.0.0/PKG-INFO
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     1535 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/README.md
-drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-01-05 00:31:21.010697 MLLPStreamingClient-1.0.0/scripts/
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2816 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/scripts/mllp-speech-dubbing_file.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     4449 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/scripts/mllp-speech-dubbing_mic.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2305 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/scripts/mllp-speech-to-text_file.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2579 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/scripts/mllp-speech-to-text_mic.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2424 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/scripts/mllp-speech-translation_file.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2708 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/scripts/mllp-speech-translation_mic.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2526 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/scripts/mllp-text-to-speech_file.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2539 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/scripts/mllp-text-to-speech_terminal.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     1821 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/scripts/mllp-text-to-text_file.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     1823 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/scripts/mllp-text-to-text_terminal.py
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       38 2024-01-05 00:31:21.010697 MLLPStreamingClient-1.0.0/setup.cfg
--rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     1473 2024-01-05 00:21:34.000000 MLLPStreamingClient-1.0.0/setup.py
+drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-05-10 11:35:32.862713 mllpstreamingclient-1.0.1/
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)      600 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/LICENSE
+drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-05-10 11:35:32.862713 mllpstreamingclient-1.0.1/MLLPStreamingClient/
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)    40375 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/MLLPStreamingClient/MLLPStreamingClient.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)      106 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/MLLPStreamingClient/__init__.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)    10756 2024-05-10 11:35:32.000000 mllpstreamingclient-1.0.1/MLLPStreamingClient/mllp_streaming_pb2.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)    35341 2024-05-10 11:35:32.000000 mllpstreamingclient-1.0.1/MLLPStreamingClient/mllp_streaming_pb2_grpc.py
+drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-05-10 11:35:32.862713 mllpstreamingclient-1.0.1/MLLPStreamingClient.egg-info/
+-rw-r--r--   0 jsilvestre  (1000) jsilvestre  (1000)    12392 2024-05-10 11:35:32.000000 mllpstreamingclient-1.0.1/MLLPStreamingClient.egg-info/PKG-INFO
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)      773 2024-05-10 11:35:32.000000 mllpstreamingclient-1.0.1/MLLPStreamingClient.egg-info/SOURCES.txt
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)        1 2024-05-10 11:35:32.000000 mllpstreamingclient-1.0.1/MLLPStreamingClient.egg-info/dependency_links.txt
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       83 2024-05-10 11:35:32.000000 mllpstreamingclient-1.0.1/MLLPStreamingClient.egg-info/requires.txt
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       20 2024-05-10 11:35:32.000000 mllpstreamingclient-1.0.1/MLLPStreamingClient.egg-info/top_level.txt
+-rw-r--r--   0 jsilvestre  (1000) jsilvestre  (1000)    12392 2024-05-10 11:35:32.862713 mllpstreamingclient-1.0.1/PKG-INFO
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     1609 2024-05-10 11:32:11.000000 mllpstreamingclient-1.0.1/README.md
+drwxrwxr-x   0 jsilvestre  (1000) jsilvestre  (1000)        0 2024-05-10 11:35:32.862713 mllpstreamingclient-1.0.1/scripts/
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2816 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/scripts/mllp-speech-dubbing_file.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     4449 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/scripts/mllp-speech-dubbing_mic.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2305 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/scripts/mllp-speech-to-text_file.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2579 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/scripts/mllp-speech-to-text_mic.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2424 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/scripts/mllp-speech-translation_file.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2708 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/scripts/mllp-speech-translation_mic.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2526 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/scripts/mllp-text-to-speech_file.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     2539 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/scripts/mllp-text-to-speech_terminal.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     1821 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/scripts/mllp-text-to-text_file.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     1823 2024-05-10 11:05:27.000000 mllpstreamingclient-1.0.1/scripts/mllp-text-to-text_terminal.py
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)       38 2024-05-10 11:35:32.862713 mllpstreamingclient-1.0.1/setup.cfg
+-rw-rw-r--   0 jsilvestre  (1000) jsilvestre  (1000)     1473 2024-05-10 11:25:34.000000 mllpstreamingclient-1.0.1/setup.py
```

### Comparing `MLLPStreamingClient-1.0.0/MLLPStreamingClient/MLLPStreamingClient.py` & `mllpstreamingclient-1.0.1/MLLPStreamingClient/MLLPStreamingClient.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/MLLPStreamingClient/mllp_streaming_pb2.py` & `mllpstreamingclient-1.0.1/MLLPStreamingClient/mllp_streaming_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,81 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: MLLPStreamingClient/mllp_streaming.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(MLLPStreamingClient/mllp_streaming.proto\x1a\x1bgoogle/protobuf/empty.proto\"2\n\x10\x41uthTokenRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"W\n\x11\x41uthTokenResponse\x12\x19\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0b.ReturnCode\x12\x12\n\nauth_token\x18\x02 \x01(\t\x12\x13\n\x0b\x65xpiry_date\x18\x03 \x01(\x05\"\"\n\x04Lang\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\"0\n\x04\x44\x61te\x12\x0b\n\x03\x64\x61y\x18\x01 \x01(\x05\x12\r\n\x05month\x18\x02 \x01(\x05\x12\x0c\n\x04year\x18\x03 \x01(\x05\"D\n\x0fS2TInfoResponse\x12\x16\n\x04info\x18\x01 \x01(\x0b\x32\x08.S2TInfo\x12\n\n\x02id\x18\x02 \x01(\x05\x12\r\n\x05slots\x18\x03 \x01(\x05\"@\n\x07S2TInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x14\n\x05langs\x18\x02 \x03(\x0b\x32\x05.Lang\x12\x13\n\x04\x64\x61te\x18\x03 \x01(\x0b\x32\x05.Date\"G\n\nS2TRequest\x12\x13\n\tsystem_id\x18\x01 \x01(\x05H\x00\x12\x0e\n\x04\x64\x61ta\x18\x02 \x01(\x0cH\x00\x12\x0f\n\x05token\x18\x03 \x01(\tH\x00\x42\x03\n\x01v\"\xad\x01\n\x0eResponseStatus\x12\"\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x14.ResponseStatus.Code\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"f\n\x04\x43ode\x12\x06\n\x02OK\x10\x00\x12\x1a\n\x16\x45RR_NO_SLOTS_AVAILABLE\x10\x01\x12\x16\n\x12\x45RR_UNKNOWN_SYSTEM\x10\x02\x12\x0c\n\x08\x45RR_PROC\x10\x03\x12\x14\n\x10\x45RR_WRONG_FORMAT\x10\x04\"e\n\x0bS2TResponse\x12\x1f\n\x06status\x18\x01 \x01(\x0b\x32\x0f.ResponseStatus\x12\x12\n\nfinal_text\x18\x02 \x01(\t\x12\x14\n\x0congoing_text\x18\x03 \x01(\t\x12\x0b\n\x03\x65os\x18\x04 \x01(\x08\"D\n\x0fT2TInfoResponse\x12\x16\n\x04info\x18\x01 \x01(\x0b\x32\x08.T2TInfo\x12\n\n\x02id\x18\x02 \x01(\x05\x12\r\n\x05slots\x18\x03 \x01(\x05\"d\n\x07T2TInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1b\n\x0csource_langs\x18\x02 \x03(\x0b\x32\x05.Lang\x12\x1b\n\x0ctarget_langs\x18\x03 \x03(\x0b\x32\x05.Lang\x12\x13\n\x04\x64\x61te\x18\x04 \x01(\x0b\x32\x05.Date\"H\n\x0fT2TInputPackage\x12\x14\n\x0congoing_text\x18\x01 \x01(\t\x12\x12\n\nfinal_text\x18\x02 \x01(\t\x12\x0b\n\x03\x65os\x18\x03 \x01(\x08\"H\n\nT2TRequest\x12\x13\n\tsystem_id\x18\x01 \x01(\x05H\x00\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x10.T2TInputPackageH\x00\x42\x03\n\x01v\"e\n\x0bT2TResponse\x12\x1f\n\x06status\x18\x01 \x01(\x0b\x32\x0f.ResponseStatus\x12\x12\n\nfinal_text\x18\x02 \x01(\t\x12\x14\n\x0congoing_text\x18\x03 \x01(\t\x12\x0b\n\x03\x65os\x18\x04 \x01(\x08\"D\n\x0fT2SInfoResponse\x12\x16\n\x04info\x18\x01 \x01(\x0b\x32\x08.T2SInfo\x12\n\n\x02id\x18\x02 \x01(\x05\x12\r\n\x05slots\x18\x03 \x01(\x05\"\x92\x02\n\x07T2SInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x14\n\x05langs\x18\x02 \x03(\x0b\x32\x05.Lang\x12\x10\n\x08speakers\x18\x03 \x03(\t\x12\x0e\n\x06styles\x18\x04 \x03(\t\x12\x15\n\raudio_formats\x18\x05 \x03(\t\x12\x1c\n\x14\x64\x65\x66\x61ult_audio_format\x18\x06 \x01(\t\x12\x13\n\x0bsample_rate\x18\x07 \x01(\r\x12!\n\x19\x66\x65\x61tures_voice_adaptation\x18\x08 \x01(\x08\x12\x0f\n\x07symbols\x18\t \x03(\t\x12\x1a\n\x12pitch_manipulation\x18\n \x01(\x08\x12\x14\n\x0c\x66rame_length\x18\x0b \x01(\r\x12\x13\n\x04\x64\x61te\x18\x0c \x01(\x0b\x32\x05.Date\"\xf0\x03\n\x0fT2SInputPackage\x12\x0e\n\x04text\x18\x01 \x01(\tH\x00\x12\x11\n\x07symbols\x18\x02 \x01(\tH\x00\x12\x11\n\tlang_code\x18\x03 \x01(\t\x12\x17\n\nspeaker_id\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x12\n\x05style\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x12\n\x05tempo\x18\x06 \x01(\x02H\x03\x88\x01\x01\x12\x12\n\x05pitch\x18\x07 \x01(\x02H\x04\x88\x01\x01\x12\x1b\n\x0e\x65xpressiveness\x18\x08 \x01(\x02H\x05\x88\x01\x01\x12\x19\n\x11symbols_durations\x18\t \x03(\r\x12\x17\n\x0fsymbols_pitches\x18\n \x03(\x02\x12\x1c\n\x0freference_audio\x18\x0b \x01(\x0cH\x06\x88\x01\x01\x12\x1c\n\x0f\x66orced_duration\x18\x0c \x01(\x02H\x07\x88\x01\x01\x12\x18\n\x0bsample_rate\x18\x0e \x01(\rH\x08\x88\x01\x01\x12\x19\n\x0c\x61udio_format\x18\x0f \x01(\tH\t\x88\x01\x01\x42\x07\n\x05inputB\r\n\x0b_speaker_idB\x08\n\x06_styleB\x08\n\x06_tempoB\x08\n\x06_pitchB\x11\n\x0f_expressivenessB\x12\n\x10_reference_audioB\x12\n\x10_forced_durationB\x0e\n\x0c_sample_rateB\x0f\n\r_audio_format\"?\n\nT2SRequest\x12\x11\n\tsystem_id\x18\x01 \x01(\x05\x12\x1e\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x10.T2SInputPackage\"x\n\x0bT2SResponse\x12\x1f\n\x06status\x18\x01 \x01(\x0b\x32\x0f.ResponseStatus\x12(\n\x08metadata\x18\x02 \x01(\x0b\x32\x14.T2SResponseMetadataH\x00\x12\x14\n\naudio_data\x18\x03 \x01(\x0cH\x00\x42\x08\n\x06T2Sret\"\xd5\x01\n\x13T2SResponseMetadata\x12\x12\n\nerror_code\x18\x01 \x01(\r\x12\x11\n\terror_msg\x18\x02 \x01(\t\x12\x15\n\rrequest_index\x18\x03 \x01(\r\x12\x14\n\x0c\x61udio_format\x18\x04 \x01(\t\x12\x13\n\x0bsample_rate\x18\x05 \x01(\r\x12\x10\n\x08\x64uration\x18\x06 \x01(\x02\x12\x0f\n\x07symbols\x18\x07 \x03(\t\x12\x19\n\x11symbols_durations\x18\x08 \x03(\x02\x12\x17\n\x0fsymbols_pitches\x18\t \x03(\x02\",\n\x0e\x41\x64\x64NodeRequest\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"=\n\x0f\x41\x64\x64NodeResponse\x12\x19\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0b.ReturnCode\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"/\n\x11ListNodesResponse\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"/\n\x11RemoveNodeRequest\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"@\n\x12RemoveNodeResponse\x12\x19\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0b.ReturnCode\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t*\x1d\n\nReturnCode\x12\x06\n\x02OK\x10\x00\x12\x07\n\x03\x45RR\x10\x01\x32\xce\x07\n\rMLLPStreaming\x12\x34\n\tAuthToken\x12\x11.AuthTokenRequest\x1a\x12.AuthTokenResponse\"\x00\x12?\n\x0fSpeech2TextInfo\x12\x16.google.protobuf.Empty\x1a\x10.S2TInfoResponse\"\x00\x30\x01\x12.\n\x0bSpeech2Text\x12\x0b.S2TRequest\x1a\x0c.S2TResponse\"\x00(\x01\x30\x01\x12=\n\rText2TextInfo\x12\x16.google.protobuf.Empty\x1a\x10.T2TInfoResponse\"\x00\x30\x01\x12,\n\tText2Text\x12\x0b.T2TRequest\x1a\x0c.T2TResponse\"\x00(\x01\x30\x01\x12?\n\x0fText2SpeechInfo\x12\x16.google.protobuf.Empty\x1a\x10.T2SInfoResponse\"\x00\x30\x01\x12.\n\x0bText2Speech\x12\x0b.T2SRequest\x1a\x0c.T2SResponse\"\x00(\x01\x30\x01\x12\x36\n\x0f\x41\x64minAddS2TNode\x12\x0f.AddNodeRequest\x1a\x10.AddNodeResponse\"\x00\x12\x43\n\x11\x41\x64minListS2TNodes\x12\x16.google.protobuf.Empty\x1a\x12.ListNodesResponse\"\x00\x30\x01\x12?\n\x12\x41\x64minRemoveS2TNode\x12\x12.RemoveNodeRequest\x1a\x13.RemoveNodeResponse\"\x00\x12\x36\n\x0f\x41\x64minAddT2TNode\x12\x0f.AddNodeRequest\x1a\x10.AddNodeResponse\"\x00\x12\x43\n\x11\x41\x64minListT2TNodes\x12\x16.google.protobuf.Empty\x1a\x12.ListNodesResponse\"\x00\x30\x01\x12?\n\x12\x41\x64minRemoveT2TNode\x12\x12.RemoveNodeRequest\x1a\x13.RemoveNodeResponse\"\x00\x12\x36\n\x0f\x41\x64minAddT2SNode\x12\x0f.AddNodeRequest\x1a\x10.AddNodeResponse\"\x00\x12\x43\n\x11\x41\x64minListT2SNodes\x12\x16.google.protobuf.Empty\x1a\x12.ListNodesResponse\"\x00\x30\x01\x12?\n\x12\x41\x64minRemoveT2SNode\x12\x12.RemoveNodeRequest\x1a\x13.RemoveNodeResponse\"\x00\x62\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'MLLPStreamingClient.mllp_streaming_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'MLLPStreamingClient.mllp_streaming_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
-  _RETURNCODE._serialized_start=2733
-  _RETURNCODE._serialized_end=2762
-  _AUTHTOKENREQUEST._serialized_start=73
-  _AUTHTOKENREQUEST._serialized_end=123
-  _AUTHTOKENRESPONSE._serialized_start=125
-  _AUTHTOKENRESPONSE._serialized_end=212
-  _LANG._serialized_start=214
-  _LANG._serialized_end=248
-  _DATE._serialized_start=250
-  _DATE._serialized_end=298
-  _S2TINFORESPONSE._serialized_start=300
-  _S2TINFORESPONSE._serialized_end=368
-  _S2TINFO._serialized_start=370
-  _S2TINFO._serialized_end=434
-  _S2TREQUEST._serialized_start=436
-  _S2TREQUEST._serialized_end=507
-  _RESPONSESTATUS._serialized_start=510
-  _RESPONSESTATUS._serialized_end=683
-  _RESPONSESTATUS_CODE._serialized_start=581
-  _RESPONSESTATUS_CODE._serialized_end=683
-  _S2TRESPONSE._serialized_start=685
-  _S2TRESPONSE._serialized_end=786
-  _T2TINFORESPONSE._serialized_start=788
-  _T2TINFORESPONSE._serialized_end=856
-  _T2TINFO._serialized_start=858
-  _T2TINFO._serialized_end=958
-  _T2TINPUTPACKAGE._serialized_start=960
-  _T2TINPUTPACKAGE._serialized_end=1032
-  _T2TREQUEST._serialized_start=1034
-  _T2TREQUEST._serialized_end=1106
-  _T2TRESPONSE._serialized_start=1108
-  _T2TRESPONSE._serialized_end=1209
-  _T2SINFORESPONSE._serialized_start=1211
-  _T2SINFORESPONSE._serialized_end=1279
-  _T2SINFO._serialized_start=1282
-  _T2SINFO._serialized_end=1556
-  _T2SINPUTPACKAGE._serialized_start=1559
-  _T2SINPUTPACKAGE._serialized_end=2055
-  _T2SREQUEST._serialized_start=2057
-  _T2SREQUEST._serialized_end=2120
-  _T2SRESPONSE._serialized_start=2122
-  _T2SRESPONSE._serialized_end=2242
-  _T2SRESPONSEMETADATA._serialized_start=2245
-  _T2SRESPONSEMETADATA._serialized_end=2458
-  _ADDNODEREQUEST._serialized_start=2460
-  _ADDNODEREQUEST._serialized_end=2504
-  _ADDNODERESPONSE._serialized_start=2506
-  _ADDNODERESPONSE._serialized_end=2567
-  _LISTNODESRESPONSE._serialized_start=2569
-  _LISTNODESRESPONSE._serialized_end=2616
-  _REMOVENODEREQUEST._serialized_start=2618
-  _REMOVENODEREQUEST._serialized_end=2665
-  _REMOVENODERESPONSE._serialized_start=2667
-  _REMOVENODERESPONSE._serialized_end=2731
-  _MLLPSTREAMING._serialized_start=2765
-  _MLLPSTREAMING._serialized_end=3739
+  _globals['_RETURNCODE']._serialized_start=2733
+  _globals['_RETURNCODE']._serialized_end=2762
+  _globals['_AUTHTOKENREQUEST']._serialized_start=73
+  _globals['_AUTHTOKENREQUEST']._serialized_end=123
+  _globals['_AUTHTOKENRESPONSE']._serialized_start=125
+  _globals['_AUTHTOKENRESPONSE']._serialized_end=212
+  _globals['_LANG']._serialized_start=214
+  _globals['_LANG']._serialized_end=248
+  _globals['_DATE']._serialized_start=250
+  _globals['_DATE']._serialized_end=298
+  _globals['_S2TINFORESPONSE']._serialized_start=300
+  _globals['_S2TINFORESPONSE']._serialized_end=368
+  _globals['_S2TINFO']._serialized_start=370
+  _globals['_S2TINFO']._serialized_end=434
+  _globals['_S2TREQUEST']._serialized_start=436
+  _globals['_S2TREQUEST']._serialized_end=507
+  _globals['_RESPONSESTATUS']._serialized_start=510
+  _globals['_RESPONSESTATUS']._serialized_end=683
+  _globals['_RESPONSESTATUS_CODE']._serialized_start=581
+  _globals['_RESPONSESTATUS_CODE']._serialized_end=683
+  _globals['_S2TRESPONSE']._serialized_start=685
+  _globals['_S2TRESPONSE']._serialized_end=786
+  _globals['_T2TINFORESPONSE']._serialized_start=788
+  _globals['_T2TINFORESPONSE']._serialized_end=856
+  _globals['_T2TINFO']._serialized_start=858
+  _globals['_T2TINFO']._serialized_end=958
+  _globals['_T2TINPUTPACKAGE']._serialized_start=960
+  _globals['_T2TINPUTPACKAGE']._serialized_end=1032
+  _globals['_T2TREQUEST']._serialized_start=1034
+  _globals['_T2TREQUEST']._serialized_end=1106
+  _globals['_T2TRESPONSE']._serialized_start=1108
+  _globals['_T2TRESPONSE']._serialized_end=1209
+  _globals['_T2SINFORESPONSE']._serialized_start=1211
+  _globals['_T2SINFORESPONSE']._serialized_end=1279
+  _globals['_T2SINFO']._serialized_start=1282
+  _globals['_T2SINFO']._serialized_end=1556
+  _globals['_T2SINPUTPACKAGE']._serialized_start=1559
+  _globals['_T2SINPUTPACKAGE']._serialized_end=2055
+  _globals['_T2SREQUEST']._serialized_start=2057
+  _globals['_T2SREQUEST']._serialized_end=2120
+  _globals['_T2SRESPONSE']._serialized_start=2122
+  _globals['_T2SRESPONSE']._serialized_end=2242
+  _globals['_T2SRESPONSEMETADATA']._serialized_start=2245
+  _globals['_T2SRESPONSEMETADATA']._serialized_end=2458
+  _globals['_ADDNODEREQUEST']._serialized_start=2460
+  _globals['_ADDNODEREQUEST']._serialized_end=2504
+  _globals['_ADDNODERESPONSE']._serialized_start=2506
+  _globals['_ADDNODERESPONSE']._serialized_end=2567
+  _globals['_LISTNODESRESPONSE']._serialized_start=2569
+  _globals['_LISTNODESRESPONSE']._serialized_end=2616
+  _globals['_REMOVENODEREQUEST']._serialized_start=2618
+  _globals['_REMOVENODEREQUEST']._serialized_end=2665
+  _globals['_REMOVENODERESPONSE']._serialized_start=2667
+  _globals['_REMOVENODERESPONSE']._serialized_end=2731
+  _globals['_MLLPSTREAMING']._serialized_start=2765
+  _globals['_MLLPSTREAMING']._serialized_end=3739
 # @@protoc_insertion_point(module_scope)
```

### Comparing `MLLPStreamingClient-1.0.0/MLLPStreamingClient/mllp_streaming_pb2_grpc.py` & `mllpstreamingclient-1.0.1/MLLPStreamingClient/mllp_streaming_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/MLLPStreamingClient.egg-info/SOURCES.txt` & `mllpstreamingclient-1.0.1/MLLPStreamingClient.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 MLLPStreamingClient/MLLPStreamingClient.py
 MLLPStreamingClient/__init__.py
 MLLPStreamingClient/mllp_streaming_pb2.py
 MLLPStreamingClient/mllp_streaming_pb2_grpc.py
 MLLPStreamingClient.egg-info/PKG-INFO
```

### Comparing `MLLPStreamingClient-1.0.0/README.md` & `mllpstreamingclient-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 the three primitive rpc methods/endpoints offered by the API, *Speech2Text*,
 *Text2Text* and *Text2Speech*, than can be directly called using this module.
 
 ## Changelog
 
 - 1.0.0 (2024-01-05):
   + First (independent and corrected) version, matching API version 1.0.
+- 1.0.1 (2024-05-10):
+  + Upgraded to newer grpcio and protobuf versions.
 
 ## Installation
 
 Via [Pypi.org](https://pypi.org/project/MLLPStreamingClient/): 
 
 ```bash
 pip3 install MLLPStreamingClient
```

### Comparing `MLLPStreamingClient-1.0.0/scripts/mllp-speech-dubbing_file.py` & `mllpstreamingclient-1.0.1/scripts/mllp-speech-dubbing_file.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/scripts/mllp-speech-dubbing_mic.py` & `mllpstreamingclient-1.0.1/scripts/mllp-speech-dubbing_mic.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/scripts/mllp-speech-to-text_file.py` & `mllpstreamingclient-1.0.1/scripts/mllp-speech-to-text_file.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/scripts/mllp-speech-to-text_mic.py` & `mllpstreamingclient-1.0.1/scripts/mllp-speech-to-text_mic.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/scripts/mllp-speech-translation_file.py` & `mllpstreamingclient-1.0.1/scripts/mllp-speech-translation_file.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/scripts/mllp-speech-translation_mic.py` & `mllpstreamingclient-1.0.1/scripts/mllp-speech-translation_mic.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/scripts/mllp-text-to-speech_file.py` & `mllpstreamingclient-1.0.1/scripts/mllp-text-to-speech_file.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/scripts/mllp-text-to-speech_terminal.py` & `mllpstreamingclient-1.0.1/scripts/mllp-text-to-speech_terminal.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/scripts/mllp-text-to-text_file.py` & `mllpstreamingclient-1.0.1/scripts/mllp-text-to-text_file.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/scripts/mllp-text-to-text_terminal.py` & `mllpstreamingclient-1.0.1/scripts/mllp-text-to-text_terminal.py`

 * *Files identical despite different names*

### Comparing `MLLPStreamingClient-1.0.0/setup.py` & `mllpstreamingclient-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent"
     ],
     python_requires='>=3.5',
-    install_requires=['protobuf==4.22.0',
-                      'grpcio==1.51.3', 
-                      'grpcio-tools==1.51.3',
+    install_requires=['protobuf==4.25.3',
+                      'grpcio==1.62.0', 
+                      'grpcio-tools==1.62.0',
                       'pyaudio',
                       'soundfile',
                       'sounddevice'],
     scripts=glob.glob("scripts/mllp-*.py"),
 )
```

