# Comparing `tmp/vocode-0.1.98.tar.gz` & `tmp/vocode-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocode-0.1.98.tar", max compression
+gzip compressed data, was "vocode-0.1.99.tar", max compression
```

## Comparing `vocode-0.1.98.tar` & `vocode-0.1.99.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1065 2023-03-28 17:29:00.108721 vocode-0.1.98/LICENSE
--rw-r--r--   0        0        0     8266 2023-04-17 21:22:32.475929 vocode-0.1.98/README.md
--rw-r--r--   0        0        0     2065 2023-04-18 22:44:29.482157 vocode-0.1.98/pyproject.toml
--rw-r--r--   0        0        0      308 2023-03-28 17:30:02.280446 vocode-0.1.98/vocode/__init__.py
--rw-r--r--   0        0        0     2403 2023-04-17 21:22:32.477579 vocode-0.1.98/vocode/helpers.py
--rw-r--r--   0        0        0     1543 2023-04-17 21:22:32.477911 vocode-0.1.98/vocode/streaming/agent/base_agent.py
--rw-r--r--   0        0        0     2013 2023-04-17 21:22:32.478098 vocode-0.1.98/vocode/streaming/agent/bot_sentiment_analyser.py
--rw-r--r--   0        0        0     6666 2023-04-17 21:22:32.478308 vocode-0.1.98/vocode/streaming/agent/chat_gpt_agent.py
--rw-r--r--   0        0        0      598 2023-04-17 21:22:32.478479 vocode-0.1.98/vocode/streaming/agent/echo_agent.py
--rw-r--r--   0        0        0     1467 2023-04-11 21:06:59.691054 vocode-0.1.98/vocode/streaming/agent/factory.py
--rw-r--r--   0        0        0     1481 2023-03-28 17:30:02.281854 vocode-0.1.98/vocode/streaming/agent/information_retrieval_agent.py
--rw-r--r--   0        0        0     5731 2023-04-17 21:22:32.478651 vocode-0.1.98/vocode/streaming/agent/llm_agent.py
--rw-r--r--   0        0        0     2060 2023-04-17 21:22:32.478825 vocode-0.1.98/vocode/streaming/agent/restful_user_implemented_agent.py
--rw-r--r--   0        0        0      684 2023-03-28 17:30:02.282322 vocode-0.1.98/vocode/streaming/agent/utils.py
--rw-r--r--   0        0        0     3259 2023-04-04 06:04:39.618650 vocode-0.1.98/vocode/streaming/client_backend/conversation.py
--rw-r--r--   0        0        0       96 2023-03-28 17:30:02.282460 vocode-0.1.98/vocode/streaming/constants.py
--rw-r--r--   0        0        0     3724 2023-04-12 18:22:27.897471 vocode-0.1.98/vocode/streaming/hosted_streaming_conversation.py
--rw-r--r--   0        0        0      476 2023-03-28 07:12:57.812101 vocode-0.1.98/vocode/streaming/input_device/base_input_device.py
--rw-r--r--   0        0        0     1638 2023-04-17 21:22:32.479145 vocode-0.1.98/vocode/streaming/input_device/microphone_input.py
--rw-r--r--   0        0        0      334 2023-03-28 07:12:57.811970 vocode-0.1.98/vocode/streaming/input_device/telephone_input.py
--rw-r--r--   0        0        0     5320 2023-04-17 21:22:32.479341 vocode-0.1.98/vocode/streaming/models/agent.py
--rw-r--r--   0        0        0      102 2023-03-28 17:30:02.283498 vocode-0.1.98/vocode/streaming/models/audio_encoding.py
--rw-r--r--   0        0        0      856 2023-04-03 01:45:30.651534 vocode-0.1.98/vocode/streaming/models/events.py
--rw-r--r--   0        0        0      299 2023-03-28 07:12:57.772953 vocode-0.1.98/vocode/streaming/models/message.py
--rw-r--r--   0        0        0     1455 2023-03-28 17:30:02.283821 vocode-0.1.98/vocode/streaming/models/model.py
--rw-r--r--   0        0        0     3871 2023-04-18 20:09:17.887473 vocode-0.1.98/vocode/streaming/models/synthesizer.py
--rw-r--r--   0        0        0     1806 2023-03-28 17:30:02.284366 vocode-0.1.98/vocode/streaming/models/telephony.py
--rw-r--r--   0        0        0     3254 2023-04-17 21:22:32.479891 vocode-0.1.98/vocode/streaming/models/transcriber.py
--rw-r--r--   0        0        0     1765 2023-04-04 06:04:39.619062 vocode-0.1.98/vocode/streaming/models/websocket.py
--rw-r--r--   0        0        0      396 2023-03-28 17:30:02.285240 vocode-0.1.98/vocode/streaming/output_device/base_output_device.py
--rw-r--r--   0        0        0     1015 2023-03-28 07:12:57.807120 vocode-0.1.98/vocode/streaming/output_device/speaker_output.py
--rw-r--r--   0        0        0      262 2023-03-28 07:12:57.809162 vocode-0.1.98/vocode/streaming/output_device/telephone_output.py
--rw-r--r--   0        0        0     1148 2023-04-04 06:04:39.619476 vocode-0.1.98/vocode/streaming/output_device/twilio_output_device.py
--rw-r--r--   0        0        0      800 2023-04-04 06:04:39.619698 vocode-0.1.98/vocode/streaming/output_device/websocket_output_device.py
--rw-r--r--   0        0        0    21227 2023-04-17 21:22:32.480231 vocode-0.1.98/vocode/streaming/streaming_conversation.py
--rw-r--r--   0        0        0    10583 2023-04-17 21:22:32.480445 vocode-0.1.98/vocode/streaming/synthesizer/azure_synthesizer.py
--rw-r--r--   0        0        0     7708 2023-04-17 21:22:32.480719 vocode-0.1.98/vocode/streaming/synthesizer/base_synthesizer.py
--rw-r--r--   0        0        0     2355 2023-04-17 21:22:32.481003 vocode-0.1.98/vocode/streaming/synthesizer/eleven_labs_synthesizer.py
--rw-r--r--   0        0        0     1902 2023-04-18 22:40:23.788111 vocode-0.1.98/vocode/streaming/synthesizer/factory.py
--rw-r--r--   0        0        0  6548060 2023-03-28 17:30:02.328281 vocode-0.1.98/vocode/streaming/synthesizer/filler_audio/typing-noise.wav
--rw-r--r--   0        0        0     3396 2023-04-11 21:06:59.694063 vocode-0.1.98/vocode/streaming/synthesizer/google_synthesizer.py
--rw-r--r--   0        0        0     1252 2023-04-17 21:22:32.481260 vocode-0.1.98/vocode/streaming/synthesizer/gtts_synthesizer.py
--rw-r--r--   0        0        0     2527 2023-04-18 19:57:27.432344 vocode-0.1.98/vocode/streaming/synthesizer/play_ht_synthesizer.py
--rw-r--r--   0        0        0     1795 2023-04-12 06:50:30.491534 vocode-0.1.98/vocode/streaming/synthesizer/rime_synthesizer.py
--rw-r--r--   0        0        0     1453 2023-04-17 21:22:32.481598 vocode-0.1.98/vocode/streaming/synthesizer/stream_elements_synthesizer.py
--rw-r--r--   0        0        0        0 2023-03-28 17:30:02.329443 vocode-0.1.98/vocode/streaming/telephony/__init__.py
--rw-r--r--   0        0        0      438 2023-03-28 17:30:02.330427 vocode-0.1.98/vocode/streaming/telephony/config_manager/base_config_manager.py
--rw-r--r--   0        0        0      609 2023-03-28 23:14:27.148000 vocode-0.1.98/vocode/streaming/telephony/config_manager/in_memory_config_manager.py
--rw-r--r--   0        0        0     1248 2023-03-28 17:30:02.331245 vocode-0.1.98/vocode/streaming/telephony/config_manager/redis_config_manager.py
--rw-r--r--   0        0        0      170 2023-03-28 17:30:02.331397 vocode-0.1.98/vocode/streaming/telephony/constants.py
--rw-r--r--   0        0        0     6799 2023-04-11 21:06:59.694996 vocode-0.1.98/vocode/streaming/telephony/conversation/call.py
--rw-r--r--   0        0        0     4136 2023-04-11 17:15:11.315392 vocode-0.1.98/vocode/streaming/telephony/conversation/outbound_call.py
--rw-r--r--   0        0        0     2802 2023-03-28 17:30:02.332164 vocode-0.1.98/vocode/streaming/telephony/conversation/zoom_dial_in.py
--rw-r--r--   0        0        0      106 2023-04-03 01:45:30.652609 vocode-0.1.98/vocode/streaming/telephony/hosted/exceptions.py
--rw-r--r--   0        0        0     2264 2023-03-28 17:30:02.332438 vocode-0.1.98/vocode/streaming/telephony/hosted/inbound_call_server.py
--rw-r--r--   0        0        0     1697 2023-03-28 17:30:02.332777 vocode-0.1.98/vocode/streaming/telephony/hosted/inbound_call_user_agent_server.py
--rw-r--r--   0        0        0     3032 2023-04-03 01:45:30.652914 vocode-0.1.98/vocode/streaming/telephony/hosted/outbound_call.py
--rw-r--r--   0        0        0     2458 2023-04-03 01:45:30.653149 vocode-0.1.98/vocode/streaming/telephony/hosted/zoom_dial_in.py
--rw-r--r--   0        0        0     5851 2023-04-17 21:22:32.481997 vocode-0.1.98/vocode/streaming/telephony/server/base.py
--rw-r--r--   0        0        0     2439 2023-04-11 21:06:59.695619 vocode-0.1.98/vocode/streaming/telephony/server/router/calls.py
--rw-r--r--   0        0        0      865 2023-04-04 06:04:39.620616 vocode-0.1.98/vocode/streaming/telephony/server/router/twiml.py
--rw-r--r--   0        0        0      150 2023-03-28 17:30:02.333925 vocode-0.1.98/vocode/streaming/telephony/templates/connect_call.xml
--rw-r--r--   0        0        0      653 2023-03-28 17:30:02.333757 vocode-0.1.98/vocode/streaming/telephony/templates.py
--rw-r--r--   0        0        0      434 2023-04-11 21:06:59.695870 vocode-0.1.98/vocode/streaming/telephony/twilio.py
--rw-r--r--   0        0        0     2220 2023-03-21 03:19:41.096039 vocode-0.1.98/vocode/streaming/telephony/zoom_dial_in.py
--rw-r--r--   0        0        0     3452 2023-04-17 21:22:32.482561 vocode-0.1.98/vocode/streaming/transcriber/assembly_ai_transcriber.py
--rw-r--r--   0        0        0     1241 2023-04-11 21:06:59.696653 vocode-0.1.98/vocode/streaming/transcriber/base_transcriber.py
--rw-r--r--   0        0        0     7975 2023-04-17 21:22:32.482831 vocode-0.1.98/vocode/streaming/transcriber/deepgram_transcriber.py
--rw-r--r--   0        0        0     1249 2023-04-17 21:22:32.483062 vocode-0.1.98/vocode/streaming/transcriber/factory.py
--rw-r--r--   0        0        0     4377 2023-04-17 21:22:32.483265 vocode-0.1.98/vocode/streaming/transcriber/google_transcriber.py
--rw-r--r--   0        0        0     4800 2023-04-17 21:22:32.483579 vocode-0.1.98/vocode/streaming/transcriber/rev_ai_transcriber.py
--rw-r--r--   0        0        0     3353 2023-04-11 23:13:05.536070 vocode-0.1.98/vocode/streaming/transcriber/whisper_cpp_transcriber.py
--rw-r--r--   0        0        0      216 2023-03-28 07:12:57.762251 vocode-0.1.98/vocode/streaming/user_implemented_agent/base_agent.py
--rw-r--r--   0        0        0      697 2023-03-28 07:12:57.762593 vocode-0.1.98/vocode/streaming/user_implemented_agent/restful_agent.py
--rw-r--r--   0        0        0     2183 2023-03-28 07:12:57.762008 vocode-0.1.98/vocode/streaming/user_implemented_agent/websocket_agent.py
--rw-r--r--   0        0        0     1768 2023-03-28 17:30:02.335417 vocode-0.1.98/vocode/streaming/utils/__init__.py
--rw-r--r--   0        0        0      125 2023-04-04 06:04:39.620775 vocode-0.1.98/vocode/streaming/utils/base_router.py
--rw-r--r--   0        0        0        0 2023-03-28 17:30:02.335448 vocode-0.1.98/vocode/streaming/utils/goodbye_embeddings/.gitkeep
--rw-r--r--   0        0        0     2237 2023-03-29 06:27:49.549508 vocode-0.1.98/vocode/streaming/utils/goodbye_model.py
--rw-r--r--   0        0        0     7782 2023-03-28 17:30:02.335881 vocode-0.1.98/vocode/streaming/utils/sse_client.py
--rw-r--r--   0        0        0     1109 2023-04-17 21:22:32.483781 vocode-0.1.98/vocode/streaming/utils/transcript.py
--rw-r--r--   0        0        0      233 2023-03-28 07:12:57.813897 vocode-0.1.98/vocode/turn_based/agent/base_agent.py
--rw-r--r--   0        0        0     1758 2023-04-11 23:08:06.680994 vocode-0.1.98/vocode/turn_based/agent/chat_gpt_agent.py
--rw-r--r--   0        0        0      155 2023-03-28 07:12:57.813754 vocode-0.1.98/vocode/turn_based/agent/echo_agent.py
--rw-r--r--   0        0        0     2147 2023-04-18 19:56:18.226539 vocode-0.1.98/vocode/turn_based/agent/llama_cpp_agent.py
--rw-r--r--   0        0        0      201 2023-03-28 07:12:57.817990 vocode-0.1.98/vocode/turn_based/input_device/base_input_device.py
--rw-r--r--   0        0        0     2030 2023-04-17 21:22:32.484021 vocode-0.1.98/vocode/turn_based/input_device/microphone_input.py
--rw-r--r--   0        0        0      185 2023-03-28 07:12:57.817099 vocode-0.1.98/vocode/turn_based/output_device/base_output_device.py
--rw-r--r--   0        0        0     1244 2023-04-04 06:04:39.621216 vocode-0.1.98/vocode/turn_based/output_device/speaker_output.py
--rw-r--r--   0        0        0     3579 2023-04-17 21:22:32.484215 vocode-0.1.98/vocode/turn_based/synthesizer/azure_synthesizer.py
--rw-r--r--   0        0        0      138 2023-03-28 07:12:57.815598 vocode-0.1.98/vocode/turn_based/synthesizer/base_synthesizer.py
--rw-r--r--   0        0        0     1733 2023-04-04 06:04:39.621772 vocode-0.1.98/vocode/turn_based/synthesizer/eleven_labs_synthesizer.py
--rw-r--r--   0        0        0      409 2023-04-11 17:15:11.317870 vocode-0.1.98/vocode/turn_based/synthesizer/gtts_synthesizer.py
--rw-r--r--   0        0        0     1757 2023-04-17 21:22:32.484506 vocode-0.1.98/vocode/turn_based/synthesizer/play_ht_synthesizer.py
--rw-r--r--   0        0        0      973 2023-04-11 17:15:11.318340 vocode-0.1.98/vocode/turn_based/synthesizer/rime_synthesizer.py
--rw-r--r--   0        0        0      701 2023-04-17 21:22:32.484647 vocode-0.1.98/vocode/turn_based/synthesizer/stream_elements_synthesizer.py
--rw-r--r--   0        0        0      152 2023-03-28 07:12:57.812543 vocode-0.1.98/vocode/turn_based/transcriber/base_transcriber.py
--rw-r--r--   0        0        0     1532 2023-04-11 23:13:05.536284 vocode-0.1.98/vocode/turn_based/transcriber/whisper_cpp_transcriber.py
--rw-r--r--   0        0        0      770 2023-03-28 17:30:02.337446 vocode-0.1.98/vocode/turn_based/transcriber/whisper_transcriber.py
--rw-r--r--   0        0        0     1638 2023-03-28 07:12:57.817247 vocode-0.1.98/vocode/turn_based/turn_based_conversation.py
--rw-r--r--   0        0        0      872 2023-04-11 23:13:05.536499 vocode-0.1.98/vocode/utils/whisper_cpp/helpers.py
--rw-r--r--   0        0        0     2124 2023-04-11 23:13:05.536728 vocode-0.1.98/vocode/utils/whisper_cpp/whisper_params.py
--rw-r--r--   0        0        0    11547 1970-01-01 00:00:00.000000 vocode-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-28 17:29:00.108721 vocode-0.1.99/LICENSE
+-rw-r--r--   0        0        0     8266 2023-04-17 21:22:32.475929 vocode-0.1.99/README.md
+-rw-r--r--   0        0        0     2083 2023-04-21 18:17:14.681374 vocode-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0      308 2023-03-28 17:30:02.280446 vocode-0.1.99/vocode/__init__.py
+-rw-r--r--   0        0        0     2403 2023-04-17 21:22:32.477579 vocode-0.1.99/vocode/helpers.py
+-rw-r--r--   0        0        0     1543 2023-04-17 21:22:32.477911 vocode-0.1.99/vocode/streaming/agent/base_agent.py
+-rw-r--r--   0        0        0     2013 2023-04-17 21:22:32.478098 vocode-0.1.99/vocode/streaming/agent/bot_sentiment_analyser.py
+-rw-r--r--   0        0        0     6666 2023-04-21 18:13:25.412654 vocode-0.1.99/vocode/streaming/agent/chat_gpt_agent.py
+-rw-r--r--   0        0        0      598 2023-04-17 21:22:32.478479 vocode-0.1.99/vocode/streaming/agent/echo_agent.py
+-rw-r--r--   0        0        0     1467 2023-04-11 21:06:59.691054 vocode-0.1.99/vocode/streaming/agent/factory.py
+-rw-r--r--   0        0        0     1481 2023-03-28 17:30:02.281854 vocode-0.1.99/vocode/streaming/agent/information_retrieval_agent.py
+-rw-r--r--   0        0        0     5731 2023-04-17 21:22:32.478651 vocode-0.1.99/vocode/streaming/agent/llm_agent.py
+-rw-r--r--   0        0        0     2060 2023-04-17 21:22:32.478825 vocode-0.1.99/vocode/streaming/agent/restful_user_implemented_agent.py
+-rw-r--r--   0        0        0      684 2023-03-28 17:30:02.282322 vocode-0.1.99/vocode/streaming/agent/utils.py
+-rw-r--r--   0        0        0     3259 2023-04-04 06:04:39.618650 vocode-0.1.99/vocode/streaming/client_backend/conversation.py
+-rw-r--r--   0        0        0       96 2023-03-28 17:30:02.282460 vocode-0.1.99/vocode/streaming/constants.py
+-rw-r--r--   0        0        0     3724 2023-04-12 18:22:27.897471 vocode-0.1.99/vocode/streaming/hosted_streaming_conversation.py
+-rw-r--r--   0        0        0      476 2023-03-28 07:12:57.812101 vocode-0.1.99/vocode/streaming/input_device/base_input_device.py
+-rw-r--r--   0        0        0     1638 2023-04-17 21:22:32.479145 vocode-0.1.99/vocode/streaming/input_device/microphone_input.py
+-rw-r--r--   0        0        0      334 2023-03-28 07:12:57.811970 vocode-0.1.99/vocode/streaming/input_device/telephone_input.py
+-rw-r--r--   0        0        0     5320 2023-04-17 21:22:32.479341 vocode-0.1.99/vocode/streaming/models/agent.py
+-rw-r--r--   0        0        0      102 2023-03-28 17:30:02.283498 vocode-0.1.99/vocode/streaming/models/audio_encoding.py
+-rw-r--r--   0        0        0      856 2023-04-03 01:45:30.651534 vocode-0.1.99/vocode/streaming/models/events.py
+-rw-r--r--   0        0        0      299 2023-03-28 07:12:57.772953 vocode-0.1.99/vocode/streaming/models/message.py
+-rw-r--r--   0        0        0     1455 2023-03-28 17:30:02.283821 vocode-0.1.99/vocode/streaming/models/model.py
+-rw-r--r--   0        0        0     3871 2023-04-18 20:09:17.887473 vocode-0.1.99/vocode/streaming/models/synthesizer.py
+-rw-r--r--   0        0        0     1806 2023-03-28 17:30:02.284366 vocode-0.1.99/vocode/streaming/models/telephony.py
+-rw-r--r--   0        0        0     3254 2023-04-17 21:22:32.479891 vocode-0.1.99/vocode/streaming/models/transcriber.py
+-rw-r--r--   0        0        0     1765 2023-04-04 06:04:39.619062 vocode-0.1.99/vocode/streaming/models/websocket.py
+-rw-r--r--   0        0        0      396 2023-03-28 17:30:02.285240 vocode-0.1.99/vocode/streaming/output_device/base_output_device.py
+-rw-r--r--   0        0        0     1015 2023-03-28 07:12:57.807120 vocode-0.1.99/vocode/streaming/output_device/speaker_output.py
+-rw-r--r--   0        0        0      262 2023-03-28 07:12:57.809162 vocode-0.1.99/vocode/streaming/output_device/telephone_output.py
+-rw-r--r--   0        0        0     1148 2023-04-04 06:04:39.619476 vocode-0.1.99/vocode/streaming/output_device/twilio_output_device.py
+-rw-r--r--   0        0        0      800 2023-04-04 06:04:39.619698 vocode-0.1.99/vocode/streaming/output_device/websocket_output_device.py
+-rw-r--r--   0        0        0    21227 2023-04-17 21:22:32.480231 vocode-0.1.99/vocode/streaming/streaming_conversation.py
+-rw-r--r--   0        0        0    10583 2023-04-17 21:22:32.480445 vocode-0.1.99/vocode/streaming/synthesizer/azure_synthesizer.py
+-rw-r--r--   0        0        0     7708 2023-04-17 21:22:32.480719 vocode-0.1.99/vocode/streaming/synthesizer/base_synthesizer.py
+-rw-r--r--   0        0        0     2355 2023-04-17 21:22:32.481003 vocode-0.1.99/vocode/streaming/synthesizer/eleven_labs_synthesizer.py
+-rw-r--r--   0        0        0     1902 2023-04-18 22:40:23.788111 vocode-0.1.99/vocode/streaming/synthesizer/factory.py
+-rw-r--r--   0        0        0  6548060 2023-03-28 17:30:02.328281 vocode-0.1.99/vocode/streaming/synthesizer/filler_audio/typing-noise.wav
+-rw-r--r--   0        0        0     3396 2023-04-11 21:06:59.694063 vocode-0.1.99/vocode/streaming/synthesizer/google_synthesizer.py
+-rw-r--r--   0        0        0     1252 2023-04-17 21:22:32.481260 vocode-0.1.99/vocode/streaming/synthesizer/gtts_synthesizer.py
+-rw-r--r--   0        0        0     2527 2023-04-18 19:57:27.432344 vocode-0.1.99/vocode/streaming/synthesizer/play_ht_synthesizer.py
+-rw-r--r--   0        0        0     1795 2023-04-12 06:50:30.491534 vocode-0.1.99/vocode/streaming/synthesizer/rime_synthesizer.py
+-rw-r--r--   0        0        0     1453 2023-04-17 21:22:32.481598 vocode-0.1.99/vocode/streaming/synthesizer/stream_elements_synthesizer.py
+-rw-r--r--   0        0        0        0 2023-03-28 17:30:02.329443 vocode-0.1.99/vocode/streaming/telephony/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-28 17:30:02.330427 vocode-0.1.99/vocode/streaming/telephony/config_manager/base_config_manager.py
+-rw-r--r--   0        0        0      609 2023-03-28 23:14:27.148000 vocode-0.1.99/vocode/streaming/telephony/config_manager/in_memory_config_manager.py
+-rw-r--r--   0        0        0     1248 2023-03-28 17:30:02.331245 vocode-0.1.99/vocode/streaming/telephony/config_manager/redis_config_manager.py
+-rw-r--r--   0        0        0      170 2023-03-28 17:30:02.331397 vocode-0.1.99/vocode/streaming/telephony/constants.py
+-rw-r--r--   0        0        0     6799 2023-04-11 21:06:59.694996 vocode-0.1.99/vocode/streaming/telephony/conversation/call.py
+-rw-r--r--   0        0        0     4136 2023-04-11 17:15:11.315392 vocode-0.1.99/vocode/streaming/telephony/conversation/outbound_call.py
+-rw-r--r--   0        0        0     2802 2023-03-28 17:30:02.332164 vocode-0.1.99/vocode/streaming/telephony/conversation/zoom_dial_in.py
+-rw-r--r--   0        0        0      106 2023-04-03 01:45:30.652609 vocode-0.1.99/vocode/streaming/telephony/hosted/exceptions.py
+-rw-r--r--   0        0        0     2264 2023-03-28 17:30:02.332438 vocode-0.1.99/vocode/streaming/telephony/hosted/inbound_call_server.py
+-rw-r--r--   0        0        0     1697 2023-03-28 17:30:02.332777 vocode-0.1.99/vocode/streaming/telephony/hosted/inbound_call_user_agent_server.py
+-rw-r--r--   0        0        0     3032 2023-04-03 01:45:30.652914 vocode-0.1.99/vocode/streaming/telephony/hosted/outbound_call.py
+-rw-r--r--   0        0        0     2458 2023-04-03 01:45:30.653149 vocode-0.1.99/vocode/streaming/telephony/hosted/zoom_dial_in.py
+-rw-r--r--   0        0        0     5851 2023-04-17 21:22:32.481997 vocode-0.1.99/vocode/streaming/telephony/server/base.py
+-rw-r--r--   0        0        0     2439 2023-04-11 21:06:59.695619 vocode-0.1.99/vocode/streaming/telephony/server/router/calls.py
+-rw-r--r--   0        0        0      865 2023-04-04 06:04:39.620616 vocode-0.1.99/vocode/streaming/telephony/server/router/twiml.py
+-rw-r--r--   0        0        0      150 2023-03-28 17:30:02.333925 vocode-0.1.99/vocode/streaming/telephony/templates/connect_call.xml
+-rw-r--r--   0        0        0      653 2023-03-28 17:30:02.333757 vocode-0.1.99/vocode/streaming/telephony/templates.py
+-rw-r--r--   0        0        0      434 2023-04-11 21:06:59.695870 vocode-0.1.99/vocode/streaming/telephony/twilio.py
+-rw-r--r--   0        0        0     2220 2023-03-21 03:19:41.096039 vocode-0.1.99/vocode/streaming/telephony/zoom_dial_in.py
+-rw-r--r--   0        0        0     3452 2023-04-17 21:22:32.482561 vocode-0.1.99/vocode/streaming/transcriber/assembly_ai_transcriber.py
+-rw-r--r--   0        0        0     1241 2023-04-11 21:06:59.696653 vocode-0.1.99/vocode/streaming/transcriber/base_transcriber.py
+-rw-r--r--   0        0        0     7975 2023-04-17 21:22:32.482831 vocode-0.1.99/vocode/streaming/transcriber/deepgram_transcriber.py
+-rw-r--r--   0        0        0     1249 2023-04-17 21:22:32.483062 vocode-0.1.99/vocode/streaming/transcriber/factory.py
+-rw-r--r--   0        0        0     4377 2023-04-17 21:22:32.483265 vocode-0.1.99/vocode/streaming/transcriber/google_transcriber.py
+-rw-r--r--   0        0        0     4800 2023-04-17 21:22:32.483579 vocode-0.1.99/vocode/streaming/transcriber/rev_ai_transcriber.py
+-rw-r--r--   0        0        0     3353 2023-04-11 23:13:05.536070 vocode-0.1.99/vocode/streaming/transcriber/whisper_cpp_transcriber.py
+-rw-r--r--   0        0        0      216 2023-03-28 07:12:57.762251 vocode-0.1.99/vocode/streaming/user_implemented_agent/base_agent.py
+-rw-r--r--   0        0        0      697 2023-03-28 07:12:57.762593 vocode-0.1.99/vocode/streaming/user_implemented_agent/restful_agent.py
+-rw-r--r--   0        0        0     2183 2023-03-28 07:12:57.762008 vocode-0.1.99/vocode/streaming/user_implemented_agent/websocket_agent.py
+-rw-r--r--   0        0        0     1768 2023-03-28 17:30:02.335417 vocode-0.1.99/vocode/streaming/utils/__init__.py
+-rw-r--r--   0        0        0      125 2023-04-04 06:04:39.620775 vocode-0.1.99/vocode/streaming/utils/base_router.py
+-rw-r--r--   0        0        0        0 2023-03-28 17:30:02.335448 vocode-0.1.99/vocode/streaming/utils/goodbye_embeddings/.gitkeep
+-rw-r--r--   0        0        0     2237 2023-03-29 06:27:49.549508 vocode-0.1.99/vocode/streaming/utils/goodbye_model.py
+-rw-r--r--   0        0        0     7782 2023-03-28 17:30:02.335881 vocode-0.1.99/vocode/streaming/utils/sse_client.py
+-rw-r--r--   0        0        0     1109 2023-04-17 21:22:32.483781 vocode-0.1.99/vocode/streaming/utils/transcript.py
+-rw-r--r--   0        0        0      233 2023-03-28 07:12:57.813897 vocode-0.1.99/vocode/turn_based/agent/base_agent.py
+-rw-r--r--   0        0        0     1758 2023-04-11 23:08:06.680994 vocode-0.1.99/vocode/turn_based/agent/chat_gpt_agent.py
+-rw-r--r--   0        0        0      155 2023-03-28 07:12:57.813754 vocode-0.1.99/vocode/turn_based/agent/echo_agent.py
+-rw-r--r--   0        0        0     2147 2023-04-21 18:13:38.426144 vocode-0.1.99/vocode/turn_based/agent/llama_cpp_agent.py
+-rw-r--r--   0        0        0      201 2023-03-28 07:12:57.817990 vocode-0.1.99/vocode/turn_based/input_device/base_input_device.py
+-rw-r--r--   0        0        0     2030 2023-04-17 21:22:32.484021 vocode-0.1.99/vocode/turn_based/input_device/microphone_input.py
+-rw-r--r--   0        0        0      185 2023-03-28 07:12:57.817099 vocode-0.1.99/vocode/turn_based/output_device/base_output_device.py
+-rw-r--r--   0        0        0     1244 2023-04-04 06:04:39.621216 vocode-0.1.99/vocode/turn_based/output_device/speaker_output.py
+-rw-r--r--   0        0        0     3579 2023-04-17 21:22:32.484215 vocode-0.1.99/vocode/turn_based/synthesizer/azure_synthesizer.py
+-rw-r--r--   0        0        0      138 2023-03-28 07:12:57.815598 vocode-0.1.99/vocode/turn_based/synthesizer/base_synthesizer.py
+-rw-r--r--   0        0        0     1733 2023-04-04 06:04:39.621772 vocode-0.1.99/vocode/turn_based/synthesizer/eleven_labs_synthesizer.py
+-rw-r--r--   0        0        0      409 2023-04-11 17:15:11.317870 vocode-0.1.99/vocode/turn_based/synthesizer/gtts_synthesizer.py
+-rw-r--r--   0        0        0     1757 2023-04-17 21:22:32.484506 vocode-0.1.99/vocode/turn_based/synthesizer/play_ht_synthesizer.py
+-rw-r--r--   0        0        0      973 2023-04-11 17:15:11.318340 vocode-0.1.99/vocode/turn_based/synthesizer/rime_synthesizer.py
+-rw-r--r--   0        0        0      701 2023-04-17 21:22:32.484647 vocode-0.1.99/vocode/turn_based/synthesizer/stream_elements_synthesizer.py
+-rw-r--r--   0        0        0      152 2023-03-28 07:12:57.812543 vocode-0.1.99/vocode/turn_based/transcriber/base_transcriber.py
+-rw-r--r--   0        0        0     1532 2023-04-11 23:13:05.536284 vocode-0.1.99/vocode/turn_based/transcriber/whisper_cpp_transcriber.py
+-rw-r--r--   0        0        0      770 2023-03-28 17:30:02.337446 vocode-0.1.99/vocode/turn_based/transcriber/whisper_transcriber.py
+-rw-r--r--   0        0        0     1638 2023-03-28 07:12:57.817247 vocode-0.1.99/vocode/turn_based/turn_based_conversation.py
+-rw-r--r--   0        0        0      872 2023-04-11 23:13:05.536499 vocode-0.1.99/vocode/utils/whisper_cpp/helpers.py
+-rw-r--r--   0        0        0     2124 2023-04-11 23:13:05.536728 vocode-0.1.99/vocode/utils/whisper_cpp/whisper_params.py
+-rw-r--r--   0        0        0    11540 1970-01-01 00:00:00.000000 vocode-0.1.99/PKG-INFO
```

### Comparing `vocode-0.1.98/LICENSE` & `vocode-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/README.md` & `vocode-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/pyproject.toml` & `vocode-0.1.99/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "vocode"
-version = "0.1.98"
+version = "0.1.99"
 description = "The all-in-one voice SDK"
 authors = ["Ajay Raj <ajay@vocode.dev>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/vocodedev/vocode-python"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.8.1"
 pydantic = ">=1.9.0"
 python-dotenv = ">=0.21.1"
 typing-extensions = ">=3.10.0.2"
 websockets = "10.4"
 anyio = "3.6.2"
 certifi = "2022.12.7"
 cffi = "1.15.1"
@@ -47,15 +47,15 @@
 aiohttp = "3.8.4"
 aiosignal = "1.3.1"
 async-timeout = "4.0.2"
 attrs = "22.2.0"
 azure-cognitiveservices-speech = "1.25.0"
 dataclasses-json = "0.5.7"
 frozenlist = "1.3.3"
-langchain = "0.0.117"
+langchain = "^0.0.146"
 marshmallow = "3.19.0"
 marshmallow-enum = "1.5.1"
 multidict = "6.0.4"
 openai = "0.27.2"
 pydub = { version = "0.25.1", optional = true }
 pyyaml = "6.0"
 sqlalchemy = "1.4.47"
@@ -79,14 +79,15 @@
 protobuf = ">=3.20.3"
 pyasn1 = "0.4.8"
 pyasn1-modules = "0.2.8"
 redis = "4.5.3"
 regex = "2023.3.23"
 rsa = "4.9"
 twilio = "7.17.0"
+gtts = "2.3.1"
 
 [tool.poetry.extras]
 io = ["pyaudio", "sounddevice", "pydub"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `vocode-0.1.98/vocode/helpers.py` & `vocode-0.1.99/vocode/helpers.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/agent/base_agent.py` & `vocode-0.1.99/vocode/streaming/agent/base_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/agent/bot_sentiment_analyser.py` & `vocode-0.1.99/vocode/streaming/agent/bot_sentiment_analyser.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/agent/chat_gpt_agent.py` & `vocode-0.1.99/vocode/streaming/agent/chat_gpt_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/agent/echo_agent.py` & `vocode-0.1.99/vocode/streaming/agent/echo_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/agent/factory.py` & `vocode-0.1.99/vocode/streaming/agent/factory.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/agent/information_retrieval_agent.py` & `vocode-0.1.99/vocode/streaming/agent/information_retrieval_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/agent/llm_agent.py` & `vocode-0.1.99/vocode/streaming/agent/llm_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/agent/restful_user_implemented_agent.py` & `vocode-0.1.99/vocode/streaming/agent/restful_user_implemented_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/agent/utils.py` & `vocode-0.1.99/vocode/streaming/agent/utils.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/client_backend/conversation.py` & `vocode-0.1.99/vocode/streaming/client_backend/conversation.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/hosted_streaming_conversation.py` & `vocode-0.1.99/vocode/streaming/hosted_streaming_conversation.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/input_device/microphone_input.py` & `vocode-0.1.99/vocode/streaming/input_device/microphone_input.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/models/agent.py` & `vocode-0.1.99/vocode/streaming/models/agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/models/events.py` & `vocode-0.1.99/vocode/streaming/models/events.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/models/model.py` & `vocode-0.1.99/vocode/streaming/models/model.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/models/synthesizer.py` & `vocode-0.1.99/vocode/streaming/models/synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/models/telephony.py` & `vocode-0.1.99/vocode/streaming/models/telephony.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/models/transcriber.py` & `vocode-0.1.99/vocode/streaming/models/transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/models/websocket.py` & `vocode-0.1.99/vocode/streaming/models/websocket.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/output_device/speaker_output.py` & `vocode-0.1.99/vocode/streaming/output_device/speaker_output.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/output_device/twilio_output_device.py` & `vocode-0.1.99/vocode/streaming/output_device/twilio_output_device.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/output_device/websocket_output_device.py` & `vocode-0.1.99/vocode/streaming/output_device/websocket_output_device.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/streaming_conversation.py` & `vocode-0.1.99/vocode/streaming/streaming_conversation.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/synthesizer/azure_synthesizer.py` & `vocode-0.1.99/vocode/streaming/synthesizer/azure_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/synthesizer/base_synthesizer.py` & `vocode-0.1.99/vocode/streaming/synthesizer/base_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/synthesizer/eleven_labs_synthesizer.py` & `vocode-0.1.99/vocode/streaming/synthesizer/eleven_labs_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/synthesizer/factory.py` & `vocode-0.1.99/vocode/streaming/synthesizer/factory.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/synthesizer/filler_audio/typing-noise.wav` & `vocode-0.1.99/vocode/streaming/synthesizer/filler_audio/typing-noise.wav`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/synthesizer/google_synthesizer.py` & `vocode-0.1.99/vocode/streaming/synthesizer/google_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/synthesizer/gtts_synthesizer.py` & `vocode-0.1.99/vocode/streaming/synthesizer/gtts_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/synthesizer/play_ht_synthesizer.py` & `vocode-0.1.99/vocode/streaming/synthesizer/play_ht_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/synthesizer/rime_synthesizer.py` & `vocode-0.1.99/vocode/streaming/synthesizer/rime_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/synthesizer/stream_elements_synthesizer.py` & `vocode-0.1.99/vocode/streaming/synthesizer/stream_elements_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/config_manager/in_memory_config_manager.py` & `vocode-0.1.99/vocode/streaming/telephony/config_manager/in_memory_config_manager.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/config_manager/redis_config_manager.py` & `vocode-0.1.99/vocode/streaming/telephony/config_manager/redis_config_manager.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/conversation/call.py` & `vocode-0.1.99/vocode/streaming/telephony/conversation/call.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/conversation/outbound_call.py` & `vocode-0.1.99/vocode/streaming/telephony/conversation/outbound_call.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/conversation/zoom_dial_in.py` & `vocode-0.1.99/vocode/streaming/telephony/conversation/zoom_dial_in.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/hosted/inbound_call_server.py` & `vocode-0.1.99/vocode/streaming/telephony/hosted/inbound_call_server.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/hosted/inbound_call_user_agent_server.py` & `vocode-0.1.99/vocode/streaming/telephony/hosted/inbound_call_user_agent_server.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/hosted/outbound_call.py` & `vocode-0.1.99/vocode/streaming/telephony/hosted/outbound_call.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/hosted/zoom_dial_in.py` & `vocode-0.1.99/vocode/streaming/telephony/hosted/zoom_dial_in.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/server/base.py` & `vocode-0.1.99/vocode/streaming/telephony/server/base.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/server/router/calls.py` & `vocode-0.1.99/vocode/streaming/telephony/server/router/calls.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/server/router/twiml.py` & `vocode-0.1.99/vocode/streaming/telephony/server/router/twiml.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/templates.py` & `vocode-0.1.99/vocode/streaming/telephony/templates.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/telephony/zoom_dial_in.py` & `vocode-0.1.99/vocode/streaming/telephony/zoom_dial_in.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/transcriber/assembly_ai_transcriber.py` & `vocode-0.1.99/vocode/streaming/transcriber/assembly_ai_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/transcriber/base_transcriber.py` & `vocode-0.1.99/vocode/streaming/transcriber/base_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/transcriber/deepgram_transcriber.py` & `vocode-0.1.99/vocode/streaming/transcriber/deepgram_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/transcriber/factory.py` & `vocode-0.1.99/vocode/streaming/transcriber/factory.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/transcriber/google_transcriber.py` & `vocode-0.1.99/vocode/streaming/transcriber/google_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/transcriber/rev_ai_transcriber.py` & `vocode-0.1.99/vocode/streaming/transcriber/rev_ai_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/transcriber/whisper_cpp_transcriber.py` & `vocode-0.1.99/vocode/streaming/transcriber/whisper_cpp_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/user_implemented_agent/restful_agent.py` & `vocode-0.1.99/vocode/streaming/user_implemented_agent/restful_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/user_implemented_agent/websocket_agent.py` & `vocode-0.1.99/vocode/streaming/user_implemented_agent/websocket_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/utils/__init__.py` & `vocode-0.1.99/vocode/streaming/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/utils/goodbye_model.py` & `vocode-0.1.99/vocode/streaming/utils/goodbye_model.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/utils/sse_client.py` & `vocode-0.1.99/vocode/streaming/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/streaming/utils/transcript.py` & `vocode-0.1.99/vocode/streaming/utils/transcript.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/agent/chat_gpt_agent.py` & `vocode-0.1.99/vocode/turn_based/agent/chat_gpt_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/agent/llama_cpp_agent.py` & `vocode-0.1.99/vocode/turn_based/agent/llama_cpp_agent.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/input_device/microphone_input.py` & `vocode-0.1.99/vocode/turn_based/input_device/microphone_input.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/output_device/speaker_output.py` & `vocode-0.1.99/vocode/turn_based/output_device/speaker_output.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/synthesizer/azure_synthesizer.py` & `vocode-0.1.99/vocode/turn_based/synthesizer/azure_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/synthesizer/eleven_labs_synthesizer.py` & `vocode-0.1.99/vocode/turn_based/synthesizer/eleven_labs_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/synthesizer/play_ht_synthesizer.py` & `vocode-0.1.99/vocode/turn_based/synthesizer/play_ht_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/synthesizer/rime_synthesizer.py` & `vocode-0.1.99/vocode/turn_based/synthesizer/rime_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/synthesizer/stream_elements_synthesizer.py` & `vocode-0.1.99/vocode/turn_based/synthesizer/stream_elements_synthesizer.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/transcriber/whisper_cpp_transcriber.py` & `vocode-0.1.99/vocode/turn_based/transcriber/whisper_cpp_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/transcriber/whisper_transcriber.py` & `vocode-0.1.99/vocode/turn_based/transcriber/whisper_transcriber.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/turn_based/turn_based_conversation.py` & `vocode-0.1.99/vocode/turn_based/turn_based_conversation.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/utils/whisper_cpp/helpers.py` & `vocode-0.1.99/vocode/utils/whisper_cpp/helpers.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/vocode/utils/whisper_cpp/whisper_params.py` & `vocode-0.1.99/vocode/utils/whisper_cpp/whisper_params.py`

 * *Files identical despite different names*

### Comparing `vocode-0.1.98/PKG-INFO` & `vocode-0.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: vocode
-Version: 0.1.98
+Version: 0.1.99
 Summary: The all-in-one voice SDK
 Home-page: https://github.com/vocodedev/vocode-python
 License: MIT
 Author: Ajay Raj
 Author-email: ajay@vocode.dev
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: io
 Requires-Dist: aiohttp (==3.8.4)
 Requires-Dist: aiosignal (==1.3.1)
 Requires-Dist: anyio (==3.6.2)
@@ -32,19 +31,20 @@
 Requires-Dist: google-api-core (==2.11.0)
 Requires-Dist: google-auth (==2.16.3)
 Requires-Dist: google-cloud-speech (==2.17.3)
 Requires-Dist: google-cloud-texttospeech (==2.14.1)
 Requires-Dist: googleapis-common-protos (==1.59.0)
 Requires-Dist: grpcio (>=1.47.0)
 Requires-Dist: grpcio-status (>=1.47.0)
+Requires-Dist: gtts (==2.3.1)
 Requires-Dist: h11 (==0.14.0)
 Requires-Dist: idna (==3.4)
 Requires-Dist: jinja2 (==3.1.2)
 Requires-Dist: joblib (==1.2.0)
-Requires-Dist: langchain (==0.0.117)
+Requires-Dist: langchain (>=0.0.146,<0.0.147)
 Requires-Dist: markupsafe (==2.1.2)
 Requires-Dist: marshmallow (==3.19.0)
 Requires-Dist: marshmallow-enum (==1.5.1)
 Requires-Dist: mccabe (==0.7.0)
 Requires-Dist: multidict (==6.0.4)
 Requires-Dist: mypy-extensions (==1.0.0)
 Requires-Dist: nltk (==3.8.1)
```

