# Comparing `tmp/napari-chatgpt-2023.6.2.tar.gz` & `tmp/napari-chatgpt-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-chatgpt-2023.6.2.tar", last modified: Fri Jun  2 19:20:53 2023, max compression
+gzip compressed data, was "napari-chatgpt-2023.6.3.tar", last modified: Sun Jun  4 04:04:01 2023, max compression
```

## Comparing `napari-chatgpt-2023.6.2.tar` & `napari-chatgpt-2023.6.3.tar`

### file list

```diff
@@ -1,238 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.005091 napari-chatgpt-2023.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.969090 napari-chatgpt-2023.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.973090 napari-chatgpt-2023.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.github/workflows/just_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.973090 napari-chatgpt-2023.6.2/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-06-02 19:20:53.005091 napari-chatgpt-2023.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-02 19:20:53.005091 napari-chatgpt-2023.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.973090 napari-chatgpt-2023.6.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.973090 napari-chatgpt-2023.6.2/src/napari_chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/bard_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/conv_agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/enumerate_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/enumerate_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/gpt4all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/gtts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/lanchain_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/openai_list_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/playwright_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/tts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/whisper_cpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/chat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/chat_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.981090 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/
--rw-r--r--   0 runner    (1001) docker     (123)  3642321 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/_tailwind.css
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/chat.js
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/marked-highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/prism.css
--rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/prism.js
--rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/sunlight-min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/sunlight.dark.css
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/sunlight.python-min.js
--rw-r--r--   0 runner    (1001) docker     (123)  3897394 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/tailwind.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/llms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/test/.pytest_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/test/.pytest_cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/test/bard_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/memory/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/napari_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/agent_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/async_base_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/demo/tools_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.989091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/file_open_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari_base_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari_plugin_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/web_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/file_download_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/functions_info_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/human_input_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/tests/web_search_tool_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/async_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/async_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/async_utils/run_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/download_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/gpt4all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.993091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/test/download_files_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/test/summarizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/demo/open_zarr_in_napari_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/open_in_napari.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/dynamic_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/exception_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/exception_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/installed_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/missing_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/python_lang_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/required_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.997091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/dynamic_import_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/exception_description_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/exception_guard_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/installed_packages_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/missing_libraries_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/required_imports_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/qt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/qt/download_file_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/qt/qt_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/segmentation/cellpose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/camel_case_to_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/extract_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/extract_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/filter_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/find_function_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/python_code_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/extract_code_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/extract_url_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/filter_lines_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/find_function_name_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/find_integer_in_parenthesis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/system/folders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.001091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/metasearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/scrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:53.005091 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/duckduckgo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/google_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/metasearch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/scrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/wikipedia_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:20:52.977090 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 19:20:52.000000 napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 19:20:34.000000 napari-chatgpt-2023.6.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.545266 napari-chatgpt-2023.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.github/workflows/just_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/src/napari_chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/bard_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/conv_agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/enumerate_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/enumerate_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/gpt4all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/gtts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/lanchain_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/openai_list_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/playwright_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/tts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/whisper_cpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/chat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/chat_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.573267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  3642321 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/_tailwind.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/chat.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/marked-highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.css
+-rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.python-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3897394 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/tailwind.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/llms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/.pytest_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/.pytest_cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/bard_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/napari_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/async_base_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/tools_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/cellpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/file_open_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari_base_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari_plugin_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/file_download_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/functions_info_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/human_input_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/web_search_tool_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/run_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/gpt4all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/download_files_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/summarizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/demo/open_zarr_in_napari_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/napari_viewer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/open_in_napari.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/dynamic_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/fix_code_given_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/installed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/missing_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/python_lang_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/required_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/dynamic_import_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/exception_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/exception_guard_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/installed_packages_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/missing_libraries_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/required_imports_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/download_file_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/qt_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/camel_case_to_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/extract_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/extract_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/filter_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/find_function_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/python_code_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/extract_code_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/extract_url_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/filter_lines_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/find_function_name_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/find_integer_in_parenthesis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/system/folders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/metasearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/scrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/duckduckgo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/google_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/metasearch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/scrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/wikipedia_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.565267 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/tox.ini
```

### Comparing `napari-chatgpt-2023.6.2/.github/workflows/just_deploy.yml` & `napari-chatgpt-2023.6.3/.github/workflows/just_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/.github/workflows/test_and_deploy.yml` & `napari-chatgpt-2023.6.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/.gitignore` & `napari-chatgpt-2023.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/.napari-hub/config.yml` & `napari-chatgpt-2023.6.3/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/.pre-commit-config.yaml` & `napari-chatgpt-2023.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/LICENSE` & `napari-chatgpt-2023.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/PKG-INFO` & `napari-chatgpt-2023.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-chatgpt
-Version: 2023.6.2
+Version: 2023.6.3
 Summary: A napari plugin to process and analyse images with chatGPT.
 Home-page: https://github.com/royerlab/napari-chatgpt
 Author: Loic A. Royer
 Author-email: royerloic@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
 Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
```

### Comparing `napari-chatgpt-2023.6.2/README.md` & `napari-chatgpt-2023.6.3/README.md`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/setup.cfg` & `napari-chatgpt-2023.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/conv_agent_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/conv_agent_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/enumerate_functions.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/enumerate_functions.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/gpt4all_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/gpt4all_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/lanchain_openai.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/lanchain_openai.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/playwright_sandbox.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/playwright_sandbox.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/speech_recognition_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/speech_recognition_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/terminal.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/terminal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/tts_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/tts_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_sandbox/whisper_cpp.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/whisper_cpp.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_tests/test_widget.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/_widget.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/chat_server.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/chat_server.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/_tailwind.css` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/_tailwind.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/chat.js` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/chat.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/marked-highlight.js` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/marked-highlight.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/prism.css` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/prism.js` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/sunlight-min.js` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight-min.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/sunlight.dark.css` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.dark.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/sunlight.python-min.js` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.python-min.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/static/tailwind.min.css` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/tailwind.min.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/chat_server/templates/index.html` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/bard.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/bard.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/gpt4all.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/gpt4all.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/llm/llms.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/llms.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/memory/memory.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/memory.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/napari_bridge.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/napari_bridge.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/agent.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/prompts.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/omega_init.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_init.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/async_base_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/async_base_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/demo/tools_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/tools_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,16 @@
     diameter: Optional[float]
             Estimated size of cells.
             if diameter is set to None, the size of the cells is estimated on a per image basis
             you can set the average cell `diameter` in pixels yourself (recommended)
             diameter can be a list or a single number for all images
 
 This function returns the segmented image as a labels array.
-To use function cellpose_segmentation() simply import it:
+Use function cellpose_segmentation() directly without importing it:
 
-from napari_chatgpt.omega.tools.segmentation.cellpose import cellpose_segmentation
 
 **IMPORTANT INSTRUCTIONS:**
 - DO NOT include code for the function 'cellpose_segmentation()' in your answer.
 - INSTEAD, DIRECTLY call the segmentation function 'cellpose_segmentation()' provided above after import.
 - Assume that the function 'cellpose_segmentation()' is available and within scope of your code.
 - DO NOT add the segmentation to the napari viewer.
 - DO NOT directly use the Cellpose API: models.cellpose(...
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/file_open_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/file_open_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 """A tool for controlling a napari instance."""
+import traceback
 from contextlib import redirect_stdout
 from io import StringIO
 
 from arbol import asection, aprint
 from napari import Viewer
 
 from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
+from napari_chatgpt.utils.python.exception_description import \
+    exception_description
+from napari_chatgpt.utils.python.fix_code_given_error import \
+    fix_code_given_error_message
 
 _napari_viewer_control_prompt = """
 "
 **Task:**
 
 Your task is to write Python code to control an already instantiated napari viewer instance based on a plain text request. The viewer instance is accessible using the variable `viewer`, so you can directly use methods like `viewer.add_image(np.zeros((10,10)))` without any preamble.
 
-**Please note the following instructions for your code:**
-- Do not create a new instance of `napari.Viewer()`. Use the existing instance provided in the variable `viewer`.
-- Ensure that your calls to the viewer's methods are correct.
+**Request:**
+{input}
 
 **Please keep the following notes in mind:**
 - If you need to add images, labels, points, shapes, surfaces, tracks, vectors, or any other type of layer that is not stored as an array, you may need additional code to read files from disk or download from a URL.
 - Unless explicitly stated in the request, the result of operations on layers should be a new layer in napari and not modify the existing layers.
 - Convert arrays to the float type before processing. Intermediate or local arrays should be of type float. Constants like `np.full()`, `np.ones()`, `np.zeros()`, etc., should be floats (e.g., 1.0).
 - If the request mentions "this," "that," or "the image/layer," it most likely refers to the last added image/layer.
 - If you are unsure about the layer being referred to, assume it is the last layer of the type most appropriate for the request.
 - If the request mentions the 'selected image', it most likely refers to the active or selected image layer.
 - To get the selected layer use: viewer.layers.selection.active
 - Important: At the end of your code add a print statement that states clearly and concisely what has been, or not, achieved. 
 
+**Please note the following instructions for your code:**
+- Do not create a new instance of `napari.Viewer()`. Use the existing instance provided in the variable `viewer`.
+- Ensure that your calls to the viewer's methods are correct.
+
 {generic_codegen_instructions}
 
 {last_generated_code}
 
-**Request:**
-{input}
+Make sure that the code is correct!
 
 **Answer in markdown:**
 """
 
 """
 **Use the existing methods of the `napari` viewer, which are as follows:**
 - `viewer.add_layer(layer: Layer)`
@@ -75,26 +82,49 @@
     def _run_code(self, request: str, code: str, viewer: Viewer) -> str:
 
         with asection(f"NapariViewerControlTool: request= {request} "):
 
             # Prepare code:
             code = super()._prepare_code(code, do_fix_bad_calls=True)
 
-            # Redirect output:
-            f = StringIO()
-            with redirect_stdout(f):
-                # Running code:
-                exec(code, globals(), {**locals(), 'viewer': viewer})
-
-            # Get captured stdout:
-            captured_output = f.getvalue().strip()
+            captured_output = _run_code_catch_errors_fix_and_try_again(code, viewer)
 
             # Message:
             if len(captured_output) > 0:
                 message = f"Tool completed task successfully: {captured_output}"
             else:
                 message = f"Tool completed task successfully"
 
             with asection(f"Message:"):
                 aprint(message)
 
             return message
+
+def _run_code_catch_errors_fix_and_try_again(code, viewer, error:str = '', nb_tries: int = 3) -> str:
+
+    try:
+        # Redirect output:
+        f = StringIO()
+        with redirect_stdout(f):
+            # Running code:
+            exec(code, globals(), {**locals(), 'viewer': viewer})
+
+        # Get captured stdout:
+        captured_output = f.getvalue().strip()
+    except Exception as e:
+        if nb_tries >= 1:
+            traceback.print_exc()
+            description = error+'\n\n'+exception_description(e)
+            description = description.strip()
+            fixed_code = fix_code_given_error_message(code,
+                                                      description,
+                                                      viewer)
+            # We try again:
+            return _run_code_catch_errors_fix_and_try_again(fixed_code, viewer,
+                                                            error=error,
+                                                            nb_tries = nb_tries-1)
+        else:
+            # No more tries available, we give up!
+            raise e
+
+
+    return captured_output
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 _napari_viewer_query_prompt = """
 "
 **Task:**
 Your task is to write Python code that can query an already instantiated napari viewer instance based on a plain text request. The code should be able to perform various operations such as returning information about the state of the viewer, the layers present, the dtype or shape of an image, and analyzing the content of different layers. For example, you can count the number of segments in a labels layer using the np.unique function, retrieve characteristics of individual segments like centroid coordinates, area/volume, or return statistics about the shape, area/volume, and positions of segments. You may also collect diverse measurements and statistics about segments in a labels layer.
 
 To answer the request, you need to implement a Python function called `query(viewer)` which takes the napari viewer as a parameter and returns a string. This string will be the answer to the request.
 
+**Request:**
+{input}
+
 **Here are some additional notes to help you determine which layer is referred to:**
 - If the request mentions 'this/that/the image (or layer)', it most likely refers to the last added layer.
 - If you are unsure about the layer being referred to, assume it is the last layer of the type most appropriate for the request.
 - If the request mentions the 'selected image', it most likely refers to the active or selected image layer.
 - To get the selected layer use: viewer.layers.selection.active
 
 **Instructions for using the napari viewer:**
@@ -27,21 +30,19 @@
 - Therefore, DO NOT use 'napari.Viewer()' or 'gui_qt():' in your code.
 - It is important NOT to create a new instance of a napari viewer. Use the one provided in the variable 'viewer'.
 - Ensure that your calls to the viewer are correct.
 
 {generic_codegen_instructions}
 - DO NOT call the 'query(viewer)' function yourself.
 - Please provide your answer in Markdown format.
-- Write the `query(viewer) -> str` function that takes the viewer as a parameter and returns the response.
 
 {last_generated_code}
 
-**Request:**
-{input}
-
+Make sure we have the right answer!
+Write the `query(viewer) -> str` function that takes the viewer as a parameter and returns the response.
 **Answer in markdown:**
 """
 
 
 class NapariViewerQueryTool(NapariBaseTool):
     """A tool for running python code in a REPL."""
 
@@ -74,13 +75,16 @@
                 # Run query code:
                 response = query(viewer)
 
             # Get captured stdout:
             captured_output = f.getvalue()
 
             # Message:
-            message = f"Tool completed query successfully, here is the response:\n\n{response}\n\nand the captured standard output:\n\n{captured_output}\n\n"
+            if len(captured_output) > 0:
+                message = f"Tool completed query successfully, here is the response:\n\n{response}\n\nand the captured standard output:\n\n{captured_output}\n\n"
+            else:
+                message = f"Tool completed query successfully, here is the response:\n\n{response}\n\n"
 
             with asection(f"Message:"):
                 aprint(message)
 
             return message
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 {generic_codegen_instructions}
 
 {last_generated_code}
 
 **Request:**
 {input}
 
+Make sure that the code is correct!
+
 **Answer in markdown:**
 """
 #
 # Important: all import statements must be inside of the function except for those needed for magicgui and for type hints.
 # All import statements required by function calls within the function must be within the function.
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/napari_base_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari_base_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/web_search_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_search_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A tool for opening ome-zarr files in napari"""
 import queue
 import sys
+import traceback
 
 from arbol import aprint, asection
 
 from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
 from napari_chatgpt.utils.python.exception_description import \
     exception_description
 
@@ -12,19 +13,20 @@
 exception_queue = queue.Queue()
 
 # existing exception handler:
 _original_exception_handler = sys.excepthook
 
 
 # New handler:
-def _uncaught_exception_handler(exctype, value, traceback):
+def _uncaught_exception_handler(exctype, value, _traceback):
     # Store the exception information in the queue
 
     enqueue_exception(value)
     aprint(value)
+    traceback.print_exc()
 
     # if _original_exception_handler != sys.__excepthook__:
     #     # Call the existing uncaught exception handler
     #     _original_exception_handler(exctype, value, traceback)
 
 
 def enqueue_exception(exception):
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/file_download_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/file_download_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/functions_info_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/functions_info_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/omega/tools/special/human_input_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/human_input_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/async_utils/run_async.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/run_async.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/download_files.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/download_files.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/gpt4all.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/gpt4all.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/download/test/download_files_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/download_files_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/summarizer.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/summarizer.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/llm/test/summarizer_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/summarizer_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/napari/open_in_napari.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/open_in_napari.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/dynamic_import.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/exception_description.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_description.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/exception_guard.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_guard.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,27 +100,30 @@
             traceback.print_exc()
             aprint(f"Encoutered exception: {str(e)} while trying to fix code! Returning code unchanged!")
             # TOODOO: if code does not compile maybe use LLM to fix it?
             return code, False
 
 
 _fix_bad_fun_calls_prompt = f"""
-**Task:**
+**Context:**
+You are an expert Python coder with extensive knowledge of all python libraries and their different versions.
+
 This function call: '{'{call}'}' refers to a non-existent function '{'{fully_qual_fun_name}'}'.
 The current environment is based on Python version {sys.version.split()[0]} and has the following packages/libraries installed:
 {'{package_list}'}. It is very likely that the function call exists but for a different version of the library! 
 
+**Task:**
 Please propose the most likely fix for the function call. 
 For example: if I tell you that this function call: 'transform.line' refers to a non existent function: 'skimage.transform.line',
 you should return the fully qualified corrected function call: 'skimage.draw.line' as this is the correct call for recent version of scikit-image. 
 In any case you should check the list above of packages and their version to return the correct function call.
 Important: just return the function call as a single line with no comments before or after!
 please enclose the returned fixed function call using apostrophes: '<fully_qualified_fixed_function_call>'.
 
-**FIXED CALL:**
+**Fixed Call:**
 """
 
 def fix_function_call(original_function_call:str,
                       fully_qual_fun_name: str,
                       llm: BaseLLM = None,
                       verbose: bool = False
                       ):
@@ -136,15 +139,15 @@
 
     # Instantiate chain:
     chain = LLMChain(
         prompt=prompt_template,
         llm=llm,
         verbose=verbose,
         callback_manager=CallbackManager(
-            [ArbolCallbackHandler('Required imports')])
+            [ArbolCallbackHandler('fix_all_bad_function_calls')])
     )
 
     # List of installed packages with their versions:
     package_list = installed_package_list()
 
     # turn it into a string:
     package_list_str = '\n'.join(package_list)
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/installed_packages.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/installed_packages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import traceback
+from functools import lru_cache
 
 _image_processing_analysis_packages = \
     ['OpenCV', 'Pillow', 'PyWavelets', 'scipy', 'networkx', 'tifffile',
      'scikit-image', 'napari', 'psygnal', 'numpy', 'imagecodecs', 'dask',
      'dask-core',
      'brotlipy', 'vispy', 'tqdm', 'openai', 'zarr', 'numcodecs', 'blosc',
      'imagecodecs', 'imageio', 'imagesize', 'scikit-image', 'cupy', 'cucim',
      'tensorflow', 'pytorch', 'mahotas', 'SimpleITK', 'matplotlib', 'pgmagick',
      'xarray', 'image', 'magicgui', 'arbol', 'tqdm']
 
-
+@lru_cache
 def installed_package_list(clean_up: bool = True,
                            version: bool = True,
                            filter=_image_processing_analysis_packages):
     package_list = pip_list(version=version) + conda_list(version=version)
 
     if clean_up:
         package_list = [pkg for pkg in package_list if not 'aws-' in pkg]
@@ -68,10 +69,15 @@
 
     except Exception as e:
         print(traceback.format_exc())
         return []
 
 
 def is_package_installed(package_name: str):
-    from pkgutil import find_loader
-    loader = find_loader(package_name)
-    return loader is not None
+    try:
+        from pkgutil import find_loader
+        loader = find_loader(package_name)
+        return loader is not None
+    except Exception as e:
+        traceback.print_exc()
+        # If for whatever reason the above fails, we just return false:
+        return False
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/missing_packages.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/missing_packages.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,27 +12,32 @@
 from langchain.llms import BaseLLM
 
 from napari_chatgpt.chat_server.callbacks.callbacks_stdout import \
     ArbolCallbackHandler
 from napari_chatgpt.utils.python.installed_packages import is_package_installed
 
 _required_packages_prompt = f"""
-Task:
-Find the list of "pip installable" packages (packages that can be installed using the 'pip install' command) required to run the provided Python code. The code is written against Python version {sys.version.split()[0]}.
+**Context:**
+You are an expert Python coder with extensive knowledge of all python libraries, and their different versions.
 
-CODE:
+**Task:**
+Find the list of "pip installable" packages (packages that can be installed using the 'pip install' command) required to run the Python code provided below. The code is written against Python version {sys.version.split()[0]}.
+Please only include packages that are absolutely necessary for running the code. Do not include any other packages. Exclude any dependencies that are already included in the listed packages.
+The answer should be a space-delimited list of packages (<list_of_packages>), without any additional text or explanations before or after.
+If no additional packages are required to run this code, just return an empty string.
+Make sure we have the right answer.
 
-Please replace '{input}' with the actual code you want to check.
-{'{input}'}
+**Code:**
 
-Please only include packages that are absolutely necessary for running the code. Do not include any other packages. Exclude any dependencies that are already included in the listed packages.
+```python
+{'{code}'}
+```python
 
-The answer should be a space-delimited list of packages (<list_of_packages>), without any additional text or explanations before or after.
 
-ANSWER:
+**Answer:**
 """
 
 
 def required_packages(code: str,
                       llm: BaseLLM = None,
                       verbose: bool = False):
     with(asection(
@@ -48,44 +53,53 @@
 
         # Instantiates LLM if needed:
         llm = llm or ChatOpenAI(model_name='gpt-3.5-turbo',
                                 temperature=0)
 
         # Make prompt template:
         prompt_template = PromptTemplate(template=_required_packages_prompt,
-                                         input_variables=["input"])
+                                         input_variables=["code"])
 
         # Instantiate chain:
         chain = LLMChain(
             prompt=prompt_template,
             llm=llm,
             verbose=verbose,
             callback_manager=CallbackManager(
                 [ArbolCallbackHandler('Required libraries')])
         )
 
         # Variable for prompt:
-        variables = {"input": code}
+        variables = {"code": code}
 
         # call LLM:
         list_of_packages_str = chain(variables)['text']
 
-        # Parse the list:
-        list_of_packages = list_of_packages_str.split()
+        # Cleanup:
+        list_of_packages_str = list_of_packages_str.strip()
 
-        aprint(f'List of required packages:\n{list_of_packages}')
+        if len(list_of_packages_str)>0:
+
+            # Parse the list:
+            list_of_packages = list_of_packages_str.split()
+
+            aprint(f'List of required packages:\n{list_of_packages}')
+
+        else:
+            aprint(f'No packages to run this code!')
+            return []
 
     return list_of_packages
 
 
 def pip_install(packages: List[str],
                 ignore_obvious: bool = True,
                 special_rules: bool = True) -> bool:
     if ignore_obvious:
-        obvious_packages = ['numpy', 'napari', 'magicgui', 'scikit-image']
+        obvious_packages = ['numpy', 'napari', 'magicgui', 'scikit-image', 'scipy']
         aprint(
             f"Removing 'obvious' packages that should be already installed with Omega: {', '.join(obvious_packages)}")
         packages = [p for p in packages if
                     not p in obvious_packages]
         aprint(f'Packages left: {packages}')
 
     # Ensure it is a list:
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/python_lang_utils.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/python_lang_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,86 @@
 import ast
 import importlib
 import inspect
 import re
+import traceback
 from functools import lru_cache
 from typing import get_type_hints, Any, List
 
+import inspect
+
+from arbol import aprint
+
+
+@lru_cache
+def get_function_signature(function_name: str,
+                           include_docstring: bool = False) -> str:
+    try:
+        module_name, function_name = function_name.rsplit('.', 1)
+        module = __import__(module_name, fromlist=[function_name])
+        function = getattr(module, function_name)
+        signature = inspect.signature(function)
+
+        # Get function parameters
+        parameters = []
+        for name, param in signature.parameters.items():
+            if param.annotation != inspect.Parameter.empty:
+                if param.default != inspect.Parameter.empty:
+                    default_value = str(param.default)
+                    parameters.append(f"{name}: {param.annotation.__name__} = {default_value}")
+                else:
+                    parameters.append(f"{name}: {param.annotation.__name__}")
+            else:
+                parameters.append(name)
+
+        # get the return type:
+        if signature.return_annotation != inspect.Signature.empty:
+            return_type = f" -> {str(signature.return_annotation.__name__)}"
+        else:
+            return_type = f""
+
+        # Get function name and signature
+        function_signature = f"def {function_name}({', '.join(parameters)}){return_type}:"
+
+        # Include docstring if flag is True
+        if include_docstring:
+            docstring = inspect.getdoc(function)
+            if docstring:
+                lines = docstring.strip().split('\n')
+                sections = {'Description':''}
+                current_section = 'Description'
+                for i, line in enumerate(lines):
+                    try:
+                        line_stripped = line.strip()
+                        if line_stripped.startswith('----'):
+                            current_section = lines[i-1].strip()
+                            sections[current_section] = ''
+                        else:
+                            if current_section and i+1 < len(lines) and not lines[i+1].startswith('----'):
+                                sections[current_section] += line + '\n'
+                    except Exception:
+                       traceback.print_exc()
+                       aprint(f'Issue while parsing docstring line {i}: {line} ')
+
+
+                desc_section = sections.get('Description', '')
+                param_section = sections.get('Parameters', '')
+                return_section = sections.get('Returns', '')
+
+                if desc_section:
+                    function_signature += f"\n\nDescription\n---------\n{desc_section}"
+                if param_section:
+                    function_signature += f"\n\nParameters\n---------\n{param_section}"
+                if return_section:
+                    function_signature += f"\n\nReturns\n------\n{return_section}"
+
+        return function_signature
+
+    except (ImportError, AttributeError):
+        return None
 
 @lru_cache
 def object_info_str(obj: Any,
                     add_docstrings: bool = True,
                     show_hidden: bool = False) -> str:
     methods = enumerate_methods(obj,
                                 add_docstrings=add_docstrings,
@@ -82,14 +154,15 @@
     signature = f"{method_name}({', '.join(signature_parts)})"
     return signature
 
 
 @lru_cache
 def get_function_info(function_path: str,
                       add_docstrings: bool = False):
+
     splitted_function_path = function_path.split('.')
 
     function_name = splitted_function_path[-1]
     pkg_name = '.'.join(splitted_function_path[0:-2])
 
     info = find_function_info_in_package(pkg_name=pkg_name,
                                          function_name=function_name,
@@ -155,53 +228,60 @@
         return package_name
     else:
         return None
 
 
 @lru_cache
 def extract_fully_qualified_function_names(code: str,
-                                           unzip_result: bool = False) -> List[
-    str]:
-    function_calls = []
-    import_statements = {}
-
-    tree = ast.parse(code)
-    for node in ast.walk(tree):
-        if isinstance(node, ast.Import):
-            for alias in node.names:
-                module_name = alias.name
-                import_statements[alias.asname or module_name] = module_name
-
-        elif isinstance(node, ast.ImportFrom):
-            module_name = node.module
-            for item in node.names:
-                import_statements[
-                    item.asname or item.name] = module_name + '.' + item.name
-
-        elif isinstance(node, ast.Call) and isinstance(node.func,
-                                                       ast.Attribute):
-            module_name = ""
-            if isinstance(node.func.value, ast.Name):
-                module_name = node.func.value.id
-            elif isinstance(node.func.value, ast.Attribute):
-                module_name = node.func.value.value.id + "." + node.func.value.attr
-
-            function_name = node.func.attr
-            if module_name and function_name:
-                if module_name in import_statements:
-                    fully_qualified_module_name = import_statements[module_name]
-                    fully_qualified_function_name = fully_qualified_module_name + '.' + function_name
-                    original_function_call = module_name + '.' + function_name
-                    function_calls.append(
-                        (fully_qualified_function_name, original_function_call))
+                                           unzip_result: bool = False) -> List[str]:
+
+
+    try:
+        function_calls = []
+        import_statements = {}
+
+        tree = ast.parse(code)
+        for node in ast.walk(tree):
+            if isinstance(node, ast.Import):
+                for alias in node.names:
+                    module_name = alias.name
+                    import_statements[alias.asname or module_name] = module_name
+
+            elif isinstance(node, ast.ImportFrom):
+                module_name = node.module
+                for item in node.names:
+                    import_statements[
+                        item.asname or item.name] = module_name + '.' + item.name
+
+            elif isinstance(node, ast.Call) and isinstance(node.func,
+                                                           ast.Attribute):
+                module_name = ""
+                if isinstance(node.func.value, ast.Name):
+                    module_name = node.func.value.id
+                elif isinstance(node.func.value, ast.Attribute):
+                    module_name = node.func.value.value.id + "." + node.func.value.attr
+
+                function_name = node.func.attr
+                if module_name and function_name:
+                    if module_name in import_statements:
+                        fully_qualified_module_name = import_statements[module_name]
+                        fully_qualified_function_name = fully_qualified_module_name + '.' + function_name
+                        original_function_call = module_name + '.' + function_name
+                        function_calls.append(
+                            (fully_qualified_function_name, original_function_call))
+
+        if unzip_result:
+            function_calls = unzip(function_calls)
+
+        return function_calls
+    except:
+        traceback.print_exc()
+        return None
 
-    if unzip_result:
-        function_calls = unzip(function_calls)
 
-    return function_calls
 
 
 def unzip(list_of_tuples):
     unzipped = zip(*list_of_tuples)
     return [list(items) for items in unzipped]
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/exception_description_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/exception_description_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,30 +64,30 @@
 
     return labels
 """
 
 
 @pytest.mark.skipif(not is_api_key_available('OpenAI'),
                     reason="requires OpenAI key to run")
-def test_ix_code_imports_1():
+def test_fix_bad_call_1():
     fixed_code, did_something = fix_all_bad_function_calls(_code_snippet_1)
     aprint(fixed_code)
 
     assert not did_something
 
 
 @pytest.mark.skipif(not is_api_key_available('OpenAI'),
                     reason="requires OpenAI key to run")
-def test_fix_code_imports_2():
+def test_fix_bad_call_2():
     fixed_code, did_something  = fix_all_bad_function_calls(_code_snippet_2)
     aprint(fixed_code)
 
     assert not did_something
 
 @pytest.mark.skipif(not is_api_key_available('OpenAI'),
                     reason="requires OpenAI key to run")
-def test_fix_code_imports_3():
+def test_fix_bad_call_3():
     fixed_code, did_something  = fix_all_bad_function_calls(_code_snippet_3)
     aprint(fixed_code)
 
     assert did_something
     assert 'skimage.draw.line' in fixed_code
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/missing_libraries_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/missing_libraries_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pprint import pprint
 
+from arbol import aprint
+
 from napari_chatgpt.utils.python.python_lang_utils import enumerate_methods, \
     find_function_info_in_package, \
     get_function_info, object_info_str, extract_fully_qualified_function_names, \
-    function_exists, get_imported_modules
+    function_exists, get_imported_modules, get_function_signature
 
 
 def test_object_info():
     string = 'string'
     info = object_info_str(string)
     pprint(info)
     assert "Class <class 'str'>" in info
@@ -110,7 +112,43 @@
 #     print('\n')
 #     modules = get_imported_modules(code)
 #
 #     functions = find_functions_with_name(modules, 'probabilistic_hough_line')
 #
 #     print('\n\n')
 #     pprint(functions)
+
+def test_get_function_signature():
+
+    print('\n')
+
+    signature = get_function_signature('napari_chatgpt.utils.python.python_lang_utils.get_function_signature')
+    aprint(signature)
+    assert 'get_function_signature(function_name: str, include_docstring: bool = False) -> str' in signature
+
+    print('\n\n')
+
+    signature = get_function_signature('numpy.zeros_like', include_docstring=True)
+    aprint(signature)
+    assert 'zeros_like(a, dtype, order, subok, shape)' in signature
+    assert 'shape : int or sequence of ints, optional.' in signature
+
+    print('\n\n')
+
+    signature = get_function_signature('skimage.draw.line', include_docstring=True)
+    aprint(signature)
+    assert 'line(r0, c0, r1, c1)' in signature
+
+    print('\n\n')
+
+    signature = get_function_signature('skimage.transform.probabilistic_hough_line', include_docstring=True)
+    aprint(signature)
+    assert 'probabilistic_hough_line(image, threshold, line_length, line_gap, theta, seed)' in signature
+
+    print('\n\n')
+
+
+
+
+
+
+
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/python/test/required_imports_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/required_imports_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 from arbol import aprint
 
 from napari_chatgpt.utils.api_keys.api_key import is_api_key_available
-from napari_chatgpt.utils.python.required_imports import required_imports
+from napari_chatgpt.utils.python.required_imports import required_imports, \
+    check_import_statement
 
 _code_snippet_1 = \
     """
     import numpy as np
     
     data = pd.read_csv("data.csv")
     result = np.mean(data["value"])
@@ -37,14 +38,22 @@
         Iyy = Iy*Iy
         Ixy = Ix*Iy
         
         trace = Ixx + Iyy 
         return trace
     """
 
+_code_snipper_3 = \
+"""
+def query(viewer) -> str:
+    layers = viewer.layers
+    layer_names = [layer.name for layer in layers]
+    return str(layer_names)
+"""
+
 
 @pytest.mark.skipif(not is_api_key_available('OpenAI'),
                     reason="requires OpenAI key to run")
 def test_required_imports_1():
     imports = required_imports(_code_snippet_1)
     aprint(imports)
 
@@ -55,7 +64,29 @@
 @pytest.mark.skipif(not is_api_key_available('OpenAI'),
                     reason="requires OpenAI key to run")
 def test_required_imports_2():
     imports = required_imports(_code_snippet_2)
     aprint(imports)
 
     assert 'import scipy.signal' in imports
+
+
+@pytest.mark.skipif(not is_api_key_available('OpenAI'),
+                    reason="requires OpenAI key to run")
+def test_required_imports_3():
+    imports = required_imports(_code_snipper_3)
+    aprint(imports)
+
+    assert len(imports)==0
+
+
+@pytest.mark.skipif(not is_api_key_available('OpenAI'),
+                    reason="requires OpenAI key to run")
+def test_check_import_statement():
+
+    assert not check_import_statement('from napari.layers import LayerList')
+
+    assert check_import_statement('import napari')
+
+    assert check_import_statement('from arbol import aprint')
+
+    assert check_import_statement('from arbol import aprint as funny_print')
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/qt/download_file_qt.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/download_file_qt.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/segmentation/cellpose.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/cellpose.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/camel_case_to_normal.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/camel_case_to_normal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/extract_urls.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/extract_urls.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/filter_lines.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/filter_lines.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/python_code_cleanup.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/python_code_cleanup.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/extract_code_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/extract_code_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/strings/test/filter_lines_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/filter_lines_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/duckduckgo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/duckduckgo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/google.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/google.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/headers.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/headers.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/metasearch.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/metasearch.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/scrapper.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/scrapper.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/duckduckgo_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/duckduckgo_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/metasearch_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/metasearch_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/test/wikipedia_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/wikipedia_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt/utils/web/wikipedia.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/wikipedia.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/PKG-INFO` & `napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-chatgpt
-Version: 2023.6.2
+Version: 2023.6.3
 Summary: A napari plugin to process and analyse images with chatGPT.
 Home-page: https://github.com/royerlab/napari-chatgpt
 Author: Loic A. Royer
 Author-email: royerloic@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
 Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
```

### Comparing `napari-chatgpt-2023.6.2/src/napari_chatgpt.egg-info/SOURCES.txt` & `napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 src/napari_chatgpt/omega/tools/napari_plugin_tool.py
 src/napari_chatgpt/omega/tools/demo/__init__.py
 src/napari_chatgpt/omega/tools/demo/tools_demo.py
 src/napari_chatgpt/omega/tools/examples/__init__.py
 src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
 src/napari_chatgpt/omega/tools/napari/__init__.py
 src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py
+src/napari_chatgpt/omega/tools/napari/cellpose.py
 src/napari_chatgpt/omega/tools/napari/file_open_tool.py
 src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py
 src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py
 src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py
 src/napari_chatgpt/omega/tools/search/__init__.py
 src/napari_chatgpt/omega/tools/search/web_image_search_tool.py
 src/napari_chatgpt/omega/tools/search/web_search_tool.py
@@ -123,44 +124,47 @@
 src/napari_chatgpt/utils/download/test/__init__.py
 src/napari_chatgpt/utils/download/test/download_files_test.py
 src/napari_chatgpt/utils/llm/__init__.py
 src/napari_chatgpt/utils/llm/summarizer.py
 src/napari_chatgpt/utils/llm/test/__init__.py
 src/napari_chatgpt/utils/llm/test/summarizer_test.py
 src/napari_chatgpt/utils/napari/__init__.py
+src/napari_chatgpt/utils/napari/napari_viewer_info.py
 src/napari_chatgpt/utils/napari/open_in_napari.py
 src/napari_chatgpt/utils/napari/demo/__init__.py
 src/napari_chatgpt/utils/napari/demo/open_zarr_in_napari_demo.py
+src/napari_chatgpt/utils/napari/test/__init__.py
+src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py
 src/napari_chatgpt/utils/omega_plugins/__init__.py
 src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
 src/napari_chatgpt/utils/omega_plugins/test/__init__.py
 src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
 src/napari_chatgpt/utils/python/__init__.py
 src/napari_chatgpt/utils/python/dynamic_import.py
 src/napari_chatgpt/utils/python/exception_description.py
 src/napari_chatgpt/utils/python/exception_guard.py
 src/napari_chatgpt/utils/python/fix_bad_fun_calls.py
+src/napari_chatgpt/utils/python/fix_code_given_error.py
 src/napari_chatgpt/utils/python/installed_packages.py
 src/napari_chatgpt/utils/python/missing_packages.py
 src/napari_chatgpt/utils/python/python_lang_utils.py
 src/napari_chatgpt/utils/python/required_imports.py
 src/napari_chatgpt/utils/python/test/__init__.py
 src/napari_chatgpt/utils/python/test/dynamic_import_test.py
 src/napari_chatgpt/utils/python/test/exception_description_test.py
 src/napari_chatgpt/utils/python/test/exception_guard_test.py
 src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py
+src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py
 src/napari_chatgpt/utils/python/test/installed_packages_test.py
 src/napari_chatgpt/utils/python/test/missing_libraries_test.py
 src/napari_chatgpt/utils/python/test/python_lang_utils_test.py
 src/napari_chatgpt/utils/python/test/required_imports_test.py
 src/napari_chatgpt/utils/qt/__init__.py
 src/napari_chatgpt/utils/qt/download_file_qt.py
 src/napari_chatgpt/utils/qt/qt_app.py
-src/napari_chatgpt/utils/segmentation/__init__.py
-src/napari_chatgpt/utils/segmentation/cellpose.py
 src/napari_chatgpt/utils/strings/__init__.py
 src/napari_chatgpt/utils/strings/camel_case_to_normal.py
 src/napari_chatgpt/utils/strings/extract_code.py
 src/napari_chatgpt/utils/strings/extract_urls.py
 src/napari_chatgpt/utils/strings/filter_lines.py
 src/napari_chatgpt/utils/strings/find_function_name.py
 src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py
```

### Comparing `napari-chatgpt-2023.6.2/tox.ini` & `napari-chatgpt-2023.6.3/tox.ini`

 * *Files identical despite different names*

