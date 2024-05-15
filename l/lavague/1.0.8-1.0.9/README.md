# Comparing `tmp/lavague-1.0.8.tar.gz` & `tmp/lavague-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague-1.0.8.tar", last modified: Tue Apr 23 09:46:39 2024, max compression
+gzip compressed data, was "lavague-1.0.9.tar", last modified: Fri May  3 11:05:05 2024, max compression
```

## Comparing `lavague-1.0.8.tar` & `lavague-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:39.490492 lavague-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 09:46:16.000000 lavague-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20739 2024-04-23 09:46:39.490492 lavague-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-23 09:46:16.000000 lavague-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-23 09:46:16.000000 lavague-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:46:39.490492 lavague-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:39.486492 lavague-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:39.486492 lavague-1.0.8/src/lavague/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/action_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:39.490492 lavague-1.0.8/src/lavague/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/command_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17087 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/version_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/vscode_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:39.490492 lavague-1.0.8/src/lavague.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20739 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:05:05.308676 lavague-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 11:04:55.000000 lavague-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20934 2024-05-03 11:05:05.308676 lavague-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-03 11:04:55.000000 lavague-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-03 11:04:55.000000 lavague-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:05:05.308676 lavague-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:05:05.304676 lavague-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:05:05.308676 lavague-1.0.9/src/lavague/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/action_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:05:05.308676 lavague-1.0.9/src/lavague/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/command_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16751 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/version_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-03 11:04:55.000000 lavague-1.0.9/src/lavague/vscode_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:05:05.308676 lavague-1.0.9/src/lavague.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20934 2024-05-03 11:05:05.000000 lavague-1.0.9/src/lavague.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-03 11:05:05.000000 lavague-1.0.9/src/lavague.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:05:05.000000 lavague-1.0.9/src/lavague.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 11:05:05.000000 lavague-1.0.9/src/lavague.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-03 11:05:05.000000 lavague-1.0.9/src/lavague.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 11:05:05.000000 lavague-1.0.9/src/lavague.egg-info/top_level.txt
```

### Comparing `lavague-1.0.8/LICENSE` & `lavague-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague-1.0.8/PKG-INFO` & `lavague-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague
-Version: 1.0.8
+Version: 1.0.9
 Summary: Selenium code generation from text instructions
 Author-email: Mithril Security <contact@mithrilsecurity.io>
 Maintainer-email: Mithril Security <contact@mithrilsecurity.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -230,28 +230,31 @@
 Requires-Dist: llama-index-embeddings-azure-openai==0.1.5
 Requires-Dist: llama-index-embeddings-openai==0.1.6
 Requires-Dist: llama-index-indices-managed-llama-cloud==0.1.4
 Requires-Dist: llama-index-legacy==0.9.48
 Requires-Dist: llama-index-llms-azure-openai==0.1.5
 Requires-Dist: llama-index-llms-litellm==0.1.4
 Requires-Dist: llama-index-llms-openai==0.1.9
+Requires-Dist: llama-index-llms-anthropic==0.1.8
+Requires-Dist: llama-index-llms-groq==0.1.3
 Requires-Dist: llama-index-multi-modal-llms-openai==0.1.4
 Requires-Dist: llama-index-program-openai==0.1.4
 Requires-Dist: llama-index-question-gen-openai==0.1.3
 Requires-Dist: llama-index-readers-file==0.1.9
 Requires-Dist: llama-index-readers-llama-parse==0.1.3
 Requires-Dist: llama-index-retrievers-bm25==0.1.3
 Requires-Dist: tree-sitter==0.21.0
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: nest_asyncio==1.6.0
 Requires-Dist: selenium==4.18.1
 Requires-Dist: google-search-results==2.4.2
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: gradio==4.21.0
 Requires-Dist: ipython
+Requires-Dist: langchain==0.1.10
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Provides-Extra: cuda
 Requires-Dist: accelerate==0.28.0; extra == "cuda"
 Requires-Dist: bitsandbytes==0.42.0; extra == "cuda"
 Provides-Extra: huggingface
@@ -261,41 +264,40 @@
 Requires-Dist: playwright==1.42.0; extra == "playwright"
 
 <p align="center">
   <a href="https://github.com/lavague-ai/LaVague/stargazers"><img src="https://img.shields.io/github/stars/lavague-ai/LaVague.svg?style=for-the-badge" alt="Stargazers"></a>
   <a href="https://github.com/lavague-ai/LaVague/issues"><img src="https://img.shields.io/github/issues/lavague-ai/LaVague.svg?style=for-the-badge" alt="Issues"></a>
   <a href="https://github.com/lavague-ai/LaVague/network/members"><img src="https://img.shields.io/github/forks/lavague-ai/LaVague.svg?style=for-the-badge" alt="Forks"></a>
   <a href="https://github.com/lavague-ai/LaVague/graphs/contributors"><img src="https://img.shields.io/github/contributors/lavague-ai/LaVague.svg?style=for-the-badge" alt="Contributors"></a>
-  <a href="https://github.com/lavague-ai/LaVague/blob/master/LICENSE.md"><img src="https://img.shields.io/github/license/lavague-ai/LaVague.svg?style=for-the-badge" alt="Apache License"></a>
 </p>
 </br>
 
 <div align="center">
   <img src="static/logo.png" width=140px: alt="LaVague Logo">
   <h1>Welcome to LaVague</h1>
 
 <h4 align="center">
  <a href="https://discord.gg/SDxn9KpqX9" target="_blank">
-    <img src="https://img.shields.io/badge/discord-000000?style=for-the-badge&colorB=555" height='35px' alt="Join our Discord server!">
+    <img src="https://dcbadge.vercel.app/api/server/SDxn9KpqX9?compact=true" height='35px' alt="Join our Discord server!">
   </a>
-  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/docs-000000?style=for-the-badge&colorB=07f" height='35px' alt="Docs"></a>
+  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/📄-docs-000000?style=for-the-badge&colorA=09c&colorB=555" height='35px' alt="Docs"></a>
 </h4>
-  <p>Copilot for devs to automate automation</p>
+  <p>The open-source community for Large Action Models</p>
 <h1></h1>
 </div>
 
 ## 🏄‍♀️  What is LaVague?
 
-LaVague is an **open-source** project designed to automate automation for devs! 
+LaVague is an **open-source Large Action Model framework** for turning **natural language** into **browser actions**.
 
-We use **advanced AI techniques** (RAG, Few-shot learning, Chain of Thought) to turn **natural language instructions** into Python code leveraging **Selenium**. LaVague is designed to make it easy for users to **automate web workflows** and execute them on a browser.
+At LaVague's core, we have an **Action Engine** which uses **advanced AI techniques** (RAG, Few-shot learning, Chain of Thought) to “compile” natural language instructions into browser automation code, by leveraging **Selenium** or **Playwright**.
 
 ### LaVague in Action
 
-Here's an example to show how LaVague can execute natural language instructions on a browser to automate interactions with a website:
+Here's an example of LaVague being used to execute natural language instructions on a browser to automate web interactions. This example uses the Gradio interface available with the `lavague launch` CLI command:
 
 <div>
   <figure>
     <img src="static/hf_lavague.gif" alt="LaVague Interaction Example" style="margin-right: 20px;">
     <figcaption><b>LaVague interacting with Hugging Face's website.</b></figcaption>
   </figure>
   <br><br>
@@ -306,38 +308,40 @@
 ### Running LaVague in your local env
 
 You can get started with `LaVague` in 2 steps:
 
 1. Install LaVague & dependencies
 ```
 wget https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh &&
-sudo bash setup.sh
+bash setup.sh
 ```
 
 2. Run your LaVague command!
 
-You can either `launch` an interactive demo, where LaVague will execute and show you the results of the automation code it generates for your instruction.
+You can either `launch` an interactive Gradio interface, where you will see both the automation code generated for each instruction but also a live preview of the results of executing the code with a debug tab:
 ```
-lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py launch
+lavague launch
 ```
 
-Or you can use the `build` command to directly get the Python code leveraging Selenium in a file, which you can then inspect & execute locally.
+Or you can use the `build` command to directly get the Python code leveraging Selenium in a file, which you can then inspect & execute locally:
 ```
-lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py build
+lavague build
 ```
 
-For a step-by-step guide or to run LaVague in a Google Colab, see our [quick-tour](https://docs.lavague.ai/en/latest/docs/get-started/quick-tour/) which will walk you through how to get set-up and launch LaVague with our CLI tool.
+> Note, you'll need an OpenAI API key for this default example and will need the `OPENAI_API_KEY` set in your environment. To use LaVague with a different API, see our [integrations section](https://docs.lavague.ai/en/latest/docs/integrations/home/).
+
+For an end-to-end example of LaVague in a Google Colab, see our [quick-tour notebook](https://colab.research.google.com/github/lavague-ai/lavague/blob/main/docs/docs/get-started/quick-tour-notebook/quick-tour.ipynb)
 
 ## 🎭 Playwright integration
 
 If you want to get started with LaVague build using Playwright as your underlying automation tool, see our [Playwright integration guide](./docs/docs/get-started/playwright.md)
 
 ## 🙋 Contributing
 
-We would love your help in making La Vague a reality. 
+We would love your help and support on our quest to build a robust and reliable Large Action Model for web automation.
 
 To avoid having multiple people working on the same things & being unable to merge your work, we have outlined the following contribution process:
 
 1) 📢 We outline tasks on our [`backlog`](https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-ai/LaVague/labels/good%20first%20issue) labels
 2) 🙋‍♀️ If you are interested in working on one of these tasks, comment on the issue! 
 3) 🤝 We will discuss with you and assign you the task with a [`community assigned`](https://github.com/lavague-ai/LaVague/labels/community-assigned) label 
 4) 💬 We will then be available to discuss this task with you
@@ -350,8 +354,8 @@
 
 ## 🗺️ Roadmap
 
 TO keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
 
 ### 🚨 Disclaimer
 
-This project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
+Note, this project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
```

### Comparing `lavague-1.0.8/README.md` & `lavague-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 <p align="center">
   <a href="https://github.com/lavague-ai/LaVague/stargazers"><img src="https://img.shields.io/github/stars/lavague-ai/LaVague.svg?style=for-the-badge" alt="Stargazers"></a>
   <a href="https://github.com/lavague-ai/LaVague/issues"><img src="https://img.shields.io/github/issues/lavague-ai/LaVague.svg?style=for-the-badge" alt="Issues"></a>
   <a href="https://github.com/lavague-ai/LaVague/network/members"><img src="https://img.shields.io/github/forks/lavague-ai/LaVague.svg?style=for-the-badge" alt="Forks"></a>
   <a href="https://github.com/lavague-ai/LaVague/graphs/contributors"><img src="https://img.shields.io/github/contributors/lavague-ai/LaVague.svg?style=for-the-badge" alt="Contributors"></a>
-  <a href="https://github.com/lavague-ai/LaVague/blob/master/LICENSE.md"><img src="https://img.shields.io/github/license/lavague-ai/LaVague.svg?style=for-the-badge" alt="Apache License"></a>
 </p>
 </br>
 
 <div align="center">
   <img src="static/logo.png" width=140px: alt="LaVague Logo">
   <h1>Welcome to LaVague</h1>
 
 <h4 align="center">
  <a href="https://discord.gg/SDxn9KpqX9" target="_blank">
-    <img src="https://img.shields.io/badge/discord-000000?style=for-the-badge&colorB=555" height='35px' alt="Join our Discord server!">
+    <img src="https://dcbadge.vercel.app/api/server/SDxn9KpqX9?compact=true" height='35px' alt="Join our Discord server!">
   </a>
-  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/docs-000000?style=for-the-badge&colorB=07f" height='35px' alt="Docs"></a>
+  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/📄-docs-000000?style=for-the-badge&colorA=09c&colorB=555" height='35px' alt="Docs"></a>
 </h4>
-  <p>Copilot for devs to automate automation</p>
+  <p>The open-source community for Large Action Models</p>
 <h1></h1>
 </div>
 
 ## 🏄‍♀️  What is LaVague?
 
-LaVague is an **open-source** project designed to automate automation for devs! 
+LaVague is an **open-source Large Action Model framework** for turning **natural language** into **browser actions**.
 
-We use **advanced AI techniques** (RAG, Few-shot learning, Chain of Thought) to turn **natural language instructions** into Python code leveraging **Selenium**. LaVague is designed to make it easy for users to **automate web workflows** and execute them on a browser.
+At LaVague's core, we have an **Action Engine** which uses **advanced AI techniques** (RAG, Few-shot learning, Chain of Thought) to “compile” natural language instructions into browser automation code, by leveraging **Selenium** or **Playwright**.
 
 ### LaVague in Action
 
-Here's an example to show how LaVague can execute natural language instructions on a browser to automate interactions with a website:
+Here's an example of LaVague being used to execute natural language instructions on a browser to automate web interactions. This example uses the Gradio interface available with the `lavague launch` CLI command:
 
 <div>
   <figure>
     <img src="static/hf_lavague.gif" alt="LaVague Interaction Example" style="margin-right: 20px;">
     <figcaption><b>LaVague interacting with Hugging Face's website.</b></figcaption>
   </figure>
   <br><br>
@@ -44,38 +43,40 @@
 ### Running LaVague in your local env
 
 You can get started with `LaVague` in 2 steps:
 
 1. Install LaVague & dependencies
 ```
 wget https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh &&
-sudo bash setup.sh
+bash setup.sh
 ```
 
 2. Run your LaVague command!
 
-You can either `launch` an interactive demo, where LaVague will execute and show you the results of the automation code it generates for your instruction.
+You can either `launch` an interactive Gradio interface, where you will see both the automation code generated for each instruction but also a live preview of the results of executing the code with a debug tab:
 ```
-lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py launch
+lavague launch
 ```
 
-Or you can use the `build` command to directly get the Python code leveraging Selenium in a file, which you can then inspect & execute locally.
+Or you can use the `build` command to directly get the Python code leveraging Selenium in a file, which you can then inspect & execute locally:
 ```
-lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py build
+lavague build
 ```
 
-For a step-by-step guide or to run LaVague in a Google Colab, see our [quick-tour](https://docs.lavague.ai/en/latest/docs/get-started/quick-tour/) which will walk you through how to get set-up and launch LaVague with our CLI tool.
+> Note, you'll need an OpenAI API key for this default example and will need the `OPENAI_API_KEY` set in your environment. To use LaVague with a different API, see our [integrations section](https://docs.lavague.ai/en/latest/docs/integrations/home/).
+
+For an end-to-end example of LaVague in a Google Colab, see our [quick-tour notebook](https://colab.research.google.com/github/lavague-ai/lavague/blob/main/docs/docs/get-started/quick-tour-notebook/quick-tour.ipynb)
 
 ## 🎭 Playwright integration
 
 If you want to get started with LaVague build using Playwright as your underlying automation tool, see our [Playwright integration guide](./docs/docs/get-started/playwright.md)
 
 ## 🙋 Contributing
 
-We would love your help in making La Vague a reality. 
+We would love your help and support on our quest to build a robust and reliable Large Action Model for web automation.
 
 To avoid having multiple people working on the same things & being unable to merge your work, we have outlined the following contribution process:
 
 1) 📢 We outline tasks on our [`backlog`](https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-ai/LaVague/labels/good%20first%20issue) labels
 2) 🙋‍♀️ If you are interested in working on one of these tasks, comment on the issue! 
 3) 🤝 We will discuss with you and assign you the task with a [`community assigned`](https://github.com/lavague-ai/LaVague/labels/community-assigned) label 
 4) 💬 We will then be available to discuss this task with you
@@ -88,8 +89,8 @@
 
 ## 🗺️ Roadmap
 
 TO keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
 
 ### 🚨 Disclaimer
 
-This project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
+Note, this project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
```

#### html2text {}

```diff
@@ -1,52 +1,56 @@
-           _[_S_t_a_r_g_a_z_e_r_s_]_[_I_s_s_u_e_s_]_[_F_o_r_k_s_]_[_C_o_n_t_r_i_b_u_t_o_r_s_]_[_A_p_a_c_h_e_ _L_i_c_e_n_s_e_]
+                   _[_S_t_a_r_g_a_z_e_r_s_]_[_I_s_s_u_e_s_]_[_F_o_r_k_s_]_[_C_o_n_t_r_i_b_u_t_o_r_s_]
                                 [LaVague Logo]
                        ************ WWeellccoommee ttoo LLaaVVaagguuee ************
                    ****** _[[_JJ_oo_ii_nn_ _oo_uu_rr_ _DD_ii_ss_cc_oo_rr_dd_ _ss_ee_rr_vv_ee_rr_!!_]]_[[_DD_oo_cc_ss_]] ******
-                    Copilot for devs to automate automation
-## ðââï¸ What is LaVague? LaVague is an **open-source** project
-designed to automate automation for devs! We use **advanced AI techniques**
-(RAG, Few-shot learning, Chain of Thought) to turn **natural language
-instructions** into Python code leveraging **Selenium**. LaVague is designed to
-make it easy for users to **automate web workflows** and execute them on a
-browser. ### LaVague in Action Here's an example to show how LaVague can
-execute natural language instructions on a browser to automate interactions
-with a website:
+               The open-source community for Large Action Models
+## ðââï¸ What is LaVague? LaVague is an **open-source Large Action
+Model framework** for turning **natural language** into **browser actions**. At
+LaVague's core, we have an **Action Engine** which uses **advanced AI
+techniques** (RAG, Few-shot learning, Chain of Thought) to âcompileâ
+natural language instructions into browser automation code, by leveraging
+**Selenium** or **Playwright**. ### LaVague in Action Here's an example of
+LaVague being used to execute natural language instructions on a browser to
+automate web interactions. This example uses the Gradio interface available
+with the `lavague launch` CLI command:
 [LaVague Interaction Example]LLaaVVaagguuee iinntteerraaccttiinngg wwiitthh HHuuggggiinngg FFaaccee''ss wweebbssiittee..
 
 ## ð Getting Started ### Running LaVague in your local env You can get
 started with `LaVague` in 2 steps: 1. Install LaVague & dependencies ``` wget
-https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh && sudo bash
+https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh && bash
 setup.sh ``` 2. Run your LaVague command! You can either `launch` an
-interactive demo, where LaVague will execute and show you the results of the
-automation code it generates for your instruction. ``` lavague --instructions
-examples/instructions/huggingface.yaml --config examples/configurations/api/
-openai_api.py launch ``` Or you can use the `build` command to directly get the
-Python code leveraging Selenium in a file, which you can then inspect & execute
-locally. ``` lavague --instructions examples/instructions/huggingface.yaml --
-config examples/configurations/api/openai_api.py build ``` For a step-by-step
-guide or to run LaVague in a Google Colab, see our [quick-tour](https://
-docs.lavague.ai/en/latest/docs/get-started/quick-tour/) which will walk you
-through how to get set-up and launch LaVague with our CLI tool. ## ð­
-Playwright integration If you want to get started with LaVague build using
-Playwright as your underlying automation tool, see our [Playwright integration
-guide](./docs/docs/get-started/playwright.md) ## ð Contributing We would
-love your help in making La Vague a reality. To avoid having multiple people
-working on the same things & being unable to merge your work, we have outlined
-the following contribution process: 1) ð¢ We outline tasks on our [`backlog`]
-(https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check
-out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/
-labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-
-ai/LaVague/labels/good%20first%20issue) labels 2) ðââï¸ If you are
-interested in working on one of these tasks, comment on the issue! 3) ð¤ We
-will discuss with you and assign you the task with a [`community assigned`]
-(https://github.com/lavague-ai/LaVague/labels/community-assigned) label 4) ð¬
-We will then be available to discuss this task with you 5) â¬ï¸ You should
-submit your work as a PR 6) â We will review & merge your code or request
-changes/give feedback Please check out our [`contributing guide`](./
-contributing.md) for a more detailed guide. If you want to ask questions,
-contribute, or have proposals, please come on our [`Discord`](https://
-discord.gg/SDxn9KpqX9) to chat! ## ðºï¸ Roadmap TO keep up to date with our
-project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
-### ð¨ Disclaimer This project executes LLM-generated code using `exec`. This
-is not considered a safe practice. We therefore recommend taking extra care
-when using LaVague (such as running LaVague in a sandboxed environment)!
+interactive Gradio interface, where you will see both the automation code
+generated for each instruction but also a live preview of the results of
+executing the code with a debug tab: ``` lavague launch ``` Or you can use the
+`build` command to directly get the Python code leveraging Selenium in a file,
+which you can then inspect & execute locally: ``` lavague build ``` > Note,
+you'll need an OpenAI API key for this default example and will need the
+`OPENAI_API_KEY` set in your environment. To use LaVague with a different API,
+see our [integrations section](https://docs.lavague.ai/en/latest/docs/
+integrations/home/). For an end-to-end example of LaVague in a Google Colab,
+see our [quick-tour notebook](https://colab.research.google.com/github/lavague-
+ai/lavague/blob/main/docs/docs/get-started/quick-tour-notebook/quick-
+tour.ipynb) ## ð­ Playwright integration If you want to get started with
+LaVague build using Playwright as your underlying automation tool, see our
+[Playwright integration guide](./docs/docs/get-started/playwright.md) ## ð
+Contributing We would love your help and support on our quest to build a robust
+and reliable Large Action Model for web automation. To avoid having multiple
+people working on the same things & being unable to merge your work, we have
+outlined the following contribution process: 1) ð¢ We outline tasks on our
+[`backlog`](https://github.com/orgs/lavague-ai/projects/1/views/3): we
+recommend you check out issues with the [`help-wanted`](https://github.com/
+lavague-ai/LaVague/labels/help%20wanted) labels & [`good first issue`](https://
+github.com/lavague-ai/LaVague/labels/good%20first%20issue) labels 2)
+ðââï¸ If you are interested in working on one of these tasks, comment
+on the issue! 3) ð¤ We will discuss with you and assign you the task with a
+[`community assigned`](https://github.com/lavague-ai/LaVague/labels/community-
+assigned) label 4) ð¬ We will then be available to discuss this task with you
+5) â¬ï¸ You should submit your work as a PR 6) â We will review & merge
+your code or request changes/give feedback Please check out our [`contributing
+guide`](./contributing.md) for a more detailed guide. If you want to ask
+questions, contribute, or have proposals, please come on our [`Discord`](https:
+//discord.gg/SDxn9KpqX9) to chat! ## ðºï¸ Roadmap TO keep up to date with
+our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/
+2). ### ð¨ Disclaimer Note, this project executes LLM-generated code using
+`exec`. This is not considered a safe practice. We therefore recommend taking
+extra care when using LaVague (such as running LaVague in a sandboxed
+environment)!
```

### Comparing `lavague-1.0.8/pyproject.toml` & `lavague-1.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["pip>=24", "setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lavague"
-version = "1.0.8"
+version = "1.0.9"
 description = "Selenium code generation from text instructions"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["IA", "AI", "selenium", "generation"]
 authors = [
   {name = "Mithril Security", email = "contact@mithrilsecurity.io" }
@@ -38,28 +38,31 @@
   "llama-index-embeddings-azure-openai==0.1.5",
   "llama-index-embeddings-openai==0.1.6",
   "llama-index-indices-managed-llama-cloud==0.1.4",
   "llama-index-legacy==0.9.48",
   "llama-index-llms-azure-openai==0.1.5",
   "llama-index-llms-litellm==0.1.4",
   "llama-index-llms-openai==0.1.9",
+  "llama-index-llms-anthropic==0.1.8",
+  "llama-index-llms-groq==0.1.3",
   "llama-index-multi-modal-llms-openai==0.1.4",
   "llama-index-program-openai==0.1.4",
   "llama-index-question-gen-openai==0.1.3",
   "llama-index-readers-file==0.1.9",
   "llama-index-readers-llama-parse==0.1.3",
   "llama-index-retrievers-bm25==0.1.3",
   "tree-sitter==0.21.0",
   "tree-sitter-languages==1.10.2",
   "nest_asyncio==1.6.0",
   "selenium==4.18.1",
   "google-search-results==2.4.2",
   "python-dotenv==1.0.1",
   "gradio==4.21.0",
   "ipython",
+  "langchain==0.1.10",
 ]
 
 [project.optional-dependencies]
 dev = ["ruff", "ipykernel"]
 cuda = ["accelerate==0.28.0", "bitsandbytes==0.42.0"]
 huggingface = ["llama-index-embeddings-huggingface==0.1.4", "llama-index-llms-huggingface==0.1.4"]
 playwright = ["playwright==1.42.0"]
```

### Comparing `lavague-1.0.8/src/lavague/cli/config.py` & `lavague-1.0.9/src/lavague/cli/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,70 +2,86 @@
 from typing import List, Callable, Optional
 from pydantic import BaseModel
 import yaml
 import importlib.util
 from pathlib import Path
 from llama_index.core.base.llms.base import BaseLLM
 from llama_index.core.base.embeddings.base import BaseEmbedding
+from lavague.evaluator import Evaluator
 from ..defaults import (
     default_get_selenium_driver,
     DefaultLLM,
     DefaultEmbedder,
     default_python_code_extractor,
 )
 from ..prompts import SELENIUM_PROMPT
 from ..driver import AbstractDriver
 from ..action_engine import ActionEngine
+from ..retrievers import OpsmSplitRetriever, BaseHtmlRetriever
 
 
 class Config:
     def __init__(
         self,
         llm: BaseLLM,
-        embedder: BaseEmbedding,
+        retriever: BaseHtmlRetriever,
         get_driver: Callable[[], AbstractDriver],
         prompt_template: str,
         cleaning_function: Callable[[str], Optional[str]],
     ):
         self.llm = llm
-        self.embedder = embedder
+        self.retriever = retriever
         self.get_driver = get_driver
         self.prompt_template = prompt_template
         self.cleaning_function = cleaning_function
 
-    def from_path(path: str) -> Config:
-        # Convert the path to a Python module path
-        module_name = Path(path).stem
-        spec = importlib.util.spec_from_file_location(module_name, path)
-        module = importlib.util.module_from_spec(spec)
-        spec.loader.exec_module(module)
+    def from_path(path: str | None) -> Config:
+        if path is not None:
+            # Convert the path to a Python module path
+            module_name = Path(path).stem
+            spec = importlib.util.spec_from_file_location(module_name, path)
+            module = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(module)
+        else:
+            module = None
         llm = getattr(module, "LLM", DefaultLLM)()
         embedder = getattr(module, "Embedder", DefaultEmbedder)()
+        retriever = getattr(module, "retriever", OpsmSplitRetriever(embedder))
         get_driver = getattr(module, "get_driver", default_get_selenium_driver)
         prompt_template = getattr(module, "prompt_template", SELENIUM_PROMPT)
         cleaning_function = getattr(
             module, "cleaning_function", default_python_code_extractor
         )
-        return Config(llm, embedder, get_driver, prompt_template, cleaning_function)
+        return Config(llm, retriever, get_driver, prompt_template, cleaning_function)
 
     def make_default_action_engine() -> ActionEngine:
         return ActionEngine(
             DefaultLLM(),
-            DefaultEmbedder(),
+            OpsmSplitRetriever(DefaultEmbedder()),
             SELENIUM_PROMPT,
             default_python_code_extractor,
         )
 
     def make_action_engine(self) -> ActionEngine:
         return ActionEngine(
-            self.llm, self.embedder, self.prompt_template, self.cleaning_function
+            self.llm, self.retriever, self.prompt_template, self.cleaning_function
+        )
+    
+    def make_evaluator(self) -> Evaluator:
+        return Evaluator(
+            self.make_action_engine(), self.get_driver
         )
 
 
 class Instructions(BaseModel):
     url: str
     instructions: List[str]
 
+    def from_default() -> Instructions:
+        url = "https://huggingface.co/"
+        instructions = ["Click on the datasets button, in the menu", "Click on the search bar 'Search models, datasets, users...', type 'lavague-ai', import time to sleep 1 second and press enter", "Scroll by 500 pixels"]
+        return Instructions(url=url, instructions=instructions)
+
     def from_yaml(path: Path) -> Instructions:
         with open(path, "r") as file:
             loaded = yaml.safe_load(file)
         return Instructions(**loaded)
```

### Comparing `lavague-1.0.8/src/lavague/cli/main.py` & `lavague-1.0.9/src/lavague/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,28 +39,30 @@
 
 
 @click.group(
     cls=LazyGroup,
     lazy_subcommands={
         "launch": "lavague.cli.commands.launch",
         "build": "lavague.cli.commands.build",
+        "eval": "lavague.cli.commands.evaluation",
         "test": "lavague.cli.commands.test",
     },
 )
 @click.option(
     "--instructions",
     "-i",
     type=click.Path(exists=True),
-    required=True,
+    required=False,
 )
 @click.option(
     "--config",
     "-c",
     type=click.Path(exists=True),
-    required=True,
+    required=False,
 )
+
 @click.pass_context
 def cli(ctx, instructions, config):
     """Copilot for devs to automate automation"""
     ctx.ensure_object(dict)
     ctx.obj["instructions"] = instructions
     ctx.obj["config"] = config
```

### Comparing `lavague-1.0.8/src/lavague/command_center.py` & `lavague-1.0.9/src/lavague/command_center.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import gradio as gr
 from selenium.webdriver.common.by import By  # import used by generated selenium code
 from selenium.webdriver.common.keys import (
     Keys,
 )
 
 from .telemetry import send_telemetry
-from .action_engine import BaseActionEngine
+from .action_engine import ActionEngine
 from .driver import AbstractDriver
 import base64
 
 
 class CommandCenter(ABC):
     @abstractmethod
     def init_driver():
@@ -36,19 +36,20 @@
     title = """
     <div align="center">
     <h1>🌊 Welcome to LaVague</h1>
     <p>Redefining internet surfing by transforming natural language instructions into seamless browser interactions.</p>
     </div>
     """
 
-    def __init__(self, actionEngine: BaseActionEngine, driver: AbstractDriver):
+    def __init__(self, actionEngine: ActionEngine, driver: AbstractDriver):
         self.actionEngine = actionEngine
         self.driver = driver
         self.base_url = ""
         self.success = False
+        self.error = ""
 
     def init_driver(self):
         def init_driver_impl(url):
             self.driver.goTo(url)
             self.driver.getScreenshot("screenshot.png")
             # This function is supposed to fetch and return the image from the URL.
             # Placeholder function: replace with actual image fetching logic.
@@ -73,42 +74,49 @@
         def telemetry(query, code, html):
             screenshot = b""
             try:
                 scr = open("screenshot.png", "rb")
                 screenshot = base64.b64encode(scr.read())
             except:
                 pass
+            source_nodes = self.actionEngine.get_nodes(query, html)
+            retrieved_context = "\n".join(source_nodes)
             send_telemetry(
                 self.actionEngine.llm.metadata.model_name,
                 code,
                 screenshot,
                 html,
                 query,
                 self.driver.getUrl(),
                 "Lavague-Launch",
                 self.success,
+                False,
+                self.error,
+                retrieved_context
             )
 
         return telemetry
 
     def __exec_code(self):
         def exec_code(code, full_code):
+            self.error = ""
             code = self.actionEngine.cleaning_function(code)
             html = self.driver.getHtml()
             _, driver = self.driver.getDriver()  # define driver for exec
             try:
                 exec(code)
                 output = "Successful code execution"
                 status = """<p style="color: green; font-size: 20px; font-weight: bold;">Success!</p>"""
                 self.success = True
                 full_code += code
             except Exception as e:
                 output = f"Error in code execution: {str(e)}"
                 status = """<p style="color: red; font-size: 20px; font-weight: bold;">Failure! Open the Debug tab for more information</p>"""
                 self.success = False
+                self.error = repr(e)
             return output, code, html, status, full_code
 
         return exec_code
 
     def __update_image_display(self):
         def update_image_display():
             self.driver.getScreenshot("screenshot.png")
```

### Comparing `lavague-1.0.8/src/lavague/driver.py` & `lavague-1.0.9/src/lavague/driver.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.8/src/lavague/format_utils.py` & `lavague-1.0.9/src/lavague/format_utils.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.8/src/lavague/prompts.py` & `lavague-1.0.9/src/lavague/prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -422,14 +422,18 @@
 
 PLAYWRIGHT_PROMPT = '''
 Your goal is to write Playwright Python code to answer queries.
 
 Your answer must be a Python markdown only.
 You can have access to external websites and libraries.
 
+In your playwright code, you should only use the page.locator() or page.get_by_text() methods to uniquely locate and interact with the elements on the page. 
+For page.locator(), you must use XPath selectors to uniquely locate elements.
+you must always interact with the first matching element by calling .first and performing an action on it (e.g., click, fill, type, etc.).
+
 You can assume the following code has been executed:
 ```python
 from playwright.sync_api import sync_playwright
 p = playwright().__enter__()
 browser = p.chromium.launch()
 page = browser.new_page()
 ```
@@ -442,40 +446,34 @@
 <head>
     <title>Mock Search Page</title>
 </head>
 <body>
     <h1>Search Page Example</h1>
     <input id="searchBar" type="text" placeholder="Type here to search...">
     <button id="searchButton">Search</button>
-    <script>
-        document.getElementById('searchButton').onclick = function() {{
-            var searchText = document.getElementById('searchBar').value;
-            alert("Searching for: " + searchText);
-        }};
-    </script>
 </body>
 </html>
 
 Query: Click on the search bar 'Type here to search...', type 'playwright', and press the 'Enter' key
 
 Completion:
 ```python
 # Let's proceed step by step.
 # First we need to identify the component first, then we can click on it.
 
 # Based on the HTML, the link can be uniquely identified using the ID "searchBar"
-# Click on the search bar
-search_bar = page.locator('#searchBar')
-search_bar.click()
+# Get the first matching element and click on it
+search_bar_button = page.locator("//input[@id='searchBar']").first
+search_bar_button.click()
 
 # Type 'playwright' into the search bar
-page.type('#searchBar', 'playwright')
+search_bar_button.fill('playwright')
 
 # Press the 'Enter' key
-page.keyboard.press('Enter')
+search_bar_button.press('Enter')
 
 ```
 
 ---
 
 HTML:
 <!DOCTYPE html>
@@ -498,24 +496,24 @@
 Query: Click on the title Link 1 and then click on the title Link 2
 
 Completion:
 ```python
 # Let's proceed step by step.
 # First we need to identify the first component, then we can click on it. Then we can identify the second component and click on it.
 
-# Based on the HTML, the first link the link can be uniquely identified using the ID "link1"
-# Let's use this ID with playwright to identify the link
-link1 = page.locator('#link1')
+# Based on the HTML, the first link the link can be uniquely identified using the text "Link 1"
+# Let's use get_by_text to identify the link and get the first matching element
+link1 = page.get_by_text('Link 1').first
 
 # Then we click on the link
 link1.click()
 
-# The other link can be uniquely identified using the class "link"
-# Let's use this class to identify the link
-link2 = page.locator('.link')
+# The other link can be uniquely identified using the text Link 2
+# Let's use get_by_text to identify the link and get the first matching element
+link2 = page.get_by_text('Link 2').first
 
 # Click on the element found
 link2.click()
 ```
 
 ---
 
@@ -535,36 +533,19 @@
 
 Query: Select the text inside the third paragraph
 
 Completion:
 ```python
 # Let's proceed step by step.
 
-# To select a paragraph, we can execute a JS script to select the text using the DOM
-# In the provided HTML, the third paragraph can be identified using the ID "para3"
-# We need to use getElementById to select the paragraph precisely
-js_script = """
-    // This part depends on the specific HTML, here is the identified ID "para3"
-    var para = document.getElementById('para3');
-    // The rest is standard
-    if (document.body.createTextRange) {{
-        var range = document.body.createTextRange();
-        range.moveToElementText(para);
-        range.select();
-    }} else if (window.getSelection) {{
-        var selection = window.getSelection();
-        var range = document.createRange();
-        range.selectNodeContents(para);
-        selection.removeAllRanges();
-        selection.addRange(range);
-    }}
-"""
+# Locate the third paragraph using the ID "para3" and get the first matching element
+third_paragraph = page.locator("//p[@id='para3']").first
 
-# Then we execute JavaScript
-page.evaluate(js_script)
+# Select the text inside the third paragraph
+third_paragraph.select_text()
 ```
 
 ---
 
 HTML:
 
 Query: Scroll up a bit
@@ -607,20 +588,20 @@
 Query: Click on the Button 'Action Button'
 
 Completion:
 ```python
 # Let's proceed step by step.
 # First we need to identify the button first, then we can click on it.
 
-# Based on the HTML provided, we need to devise the best strategy to select the button.
-# The action button can be identified using the class name "action-btn"
-action_button = page.locator('.action-btn')
+# Based on the HTML provided, we need to devise the best strategy to select the button and get the first matching element.
+# The action button can be identified using the text "Action Button"
+action_button = page.get_by_text("Action Button").first
 
 # Then we can click on it
-await action_button.click()
+action_button.click()
 ```
 
 ---
 
 HTML:
 {context_str}
 Query: {query_str}
```

#### html2text {}

```diff
@@ -125,64 +125,64 @@
 on it. # Based on the HTML provided, we need to devise the best strategy to
 select the button. # The action button can be identified using the class name
 "action-btn" action_button = driver.find_element(By.XPATH, "//*[@class='action-
 btn']") # Then we can click on it action_button.click() ``` --- HTML:
 {context_str} Query: {query_str} Completion: ```python # Let's proceed step by
 step. ''' PLAYWRIGHT_PROMPT = ''' Your goal is to write Playwright Python code
 to answer queries. Your answer must be a Python markdown only. You can have
-access to external websites and libraries. You can assume the following code
-has been executed: ```python from playwright.sync_api import sync_playwright p
-= playwright().__enter__() browser = p.chromium.launch() page =
-browser.new_page() ``` --- HTML:
+access to external websites and libraries. In your playwright code, you should
+only use the page.locator() or page.get_by_text() methods to uniquely locate
+and interact with the elements on the page. For page.locator(), you must use
+XPath selectors to uniquely locate elements. you must always interact with the
+first matching element by calling .first and performing an action on it (e.g.,
+click, fill, type, etc.). You can assume the following code has been executed:
+```python from playwright.sync_api import sync_playwright p = playwright
+().__enter__() browser = p.chromium.launch() page = browser.new_page() ``` --
+- HTML:
 ************ SSeeaarrcchh PPaaggee EExxaammppllee ************
 [                    ]Search
 Query: Click on the search bar 'Type here to search...', type 'playwright', and
 press the 'Enter' key Completion: ```python # Let's proceed step by step. #
 First we need to identify the component first, then we can click on it. # Based
-on the HTML, the link can be uniquely identified using the ID "searchBar" #
-Click on the search bar search_bar = page.locator('#searchBar')
-search_bar.click() # Type 'playwright' into the search bar page.type
-('#searchBar', 'playwright') # Press the 'Enter' key page.keyboard.press
-('Enter') ``` --- HTML:
+on the HTML, the link can be uniquely identified using the ID "searchBar" # Get
+the first matching element and click on it search_bar_button = page.locator("//
+input[@id='searchBar']").first search_bar_button.click() # Type 'playwright'
+into the search bar search_bar_button.fill('playwright') # Press the 'Enter'
+key search_bar_button.press('Enter') ``` --- HTML:
 ************ WWeellccoommee ttoo tthhee MMoocckk PPaaggee ************
 _L_i_n_k_ _1
 _L_i_n_k_ _2
 Query: Click on the title Link 1 and then click on the title Link 2 Completion:
 ```python # Let's proceed step by step. # First we need to identify the first
 component, then we can click on it. Then we can identify the second component
 and click on it. # Based on the HTML, the first link the link can be uniquely
-identified using the ID "link1" # Let's use this ID with playwright to identify
-the link link1 = page.locator('#link1') # Then we click on the link link1.click
-() # The other link can be uniquely identified using the class "link" # Let's
-use this class to identify the link link2 = page.locator('.link') # Click on
-the element found link2.click() ``` --- HTML:
+identified using the text "Link 1" # Let's use get_by_text to identify the link
+and get the first matching element link1 = page.get_by_text('Link 1').first #
+Then we click on the link link1.click() # The other link can be uniquely
+identified using the text Link 2 # Let's use get_by_text to identify the link
+and get the first matching element link2 = page.get_by_text('Link 2').first #
+Click on the element found link2.click() ``` --- HTML:
 This is the first paragraph.
 This is the second paragraph.
 This is the third paragraph, which we will select and copy.
 This is the fourth paragraph.
 Query: Select the text inside the third paragraph Completion: ```python # Let's
-proceed step by step. # To select a paragraph, we can execute a JS script to
-select the text using the DOM # In the provided HTML, the third paragraph can
-be identified using the ID "para3" # We need to use getElementById to select
-the paragraph precisely js_script = """ // This part depends on the specific
-HTML, here is the identified ID "para3" var para = document.getElementById
-('para3'); // The rest is standard if (document.body.createTextRange) {{ var
-range = document.body.createTextRange(); range.moveToElementText(para);
-range.select(); }} else if (window.getSelection) {{ var selection =
-window.getSelection(); var range = document.createRange();
-range.selectNodeContents(para); selection.removeAllRanges(); selection.addRange
-(range); }} """ # Then we execute JavaScript page.evaluate(js_script) ``` --
-- HTML: Query: Scroll up a bit Completion: ```python # Let's proceed step by
-step. # We don't need to use the HTML data as this is a stateless operation. #
-200 pixels should be sufficient. Let's execute the JavaScript to scroll up.
-page.evaluate("window.scrollBy(0, 200)") ``` --- --- HTML:
+proceed step by step. # Locate the third paragraph using the ID "para3" and get
+the first matching element third_paragraph = page.locator("//p
+[@id='para3']").first # Select the text inside the third paragraph
+third_paragraph.select_text() ``` --- HTML: Query: Scroll up a bit Completion:
+```python # Let's proceed step by step. # We don't need to use the HTML data as
+this is a stateless operation. # 200 pixels should be sufficient. Let's execute
+the JavaScript to scroll up. page.evaluate("window.scrollBy(0, 200)") ``` --- -
+-- HTML:
 ************ EEnnhhaanncceedd TTeesstt PPaaggee ffoorr PPllaayywwrriigghhtt ************
 First Button Action Button
 Test Button
 Hidden Button
 Query: Click on the Button 'Action Button' Completion: ```python # Let's
 proceed step by step. # First we need to identify the button first, then we can
 click on it. # Based on the HTML provided, we need to devise the best strategy
-to select the button. # The action button can be identified using the class
-name "action-btn" action_button = page.locator('.action-btn') # Then we can
-click on it await action_button.click() ``` --- HTML: {context_str} Query:
-{query_str} Completion: ```python # Let's proceed step by step. '''
+to select the button and get the first matching element. # The action button
+can be identified using the text "Action Button" action_button =
+page.get_by_text("Action Button").first # Then we can click on it
+action_button.click() ``` --- HTML: {context_str} Query: {query_str}
+Completion: ```python # Let's proceed step by step. '''
```

### Comparing `lavague-1.0.8/src/lavague/telemetry.py` & `lavague-1.0.9/src/lavague/telemetry.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,71 @@
 import os
 import requests
 import uuid
 
+from .version_checker import get_installed_version
+
 TELEMETRY_VAR = os.getenv("LAVAGUE_TELEMETRY")
 USER_ID = str(uuid.uuid4())
 
 
 def send_telemetry(
     model_name: str,
     code: str,
     screenshot: bytes,
     html: str,
     instruction: str,
     url: str,
     origin: str,
     success: bool,
     test: bool = False,
+    error: str = "",
+    source_nodes: str = "",
 ):
     """
     Telemetry to help performance.
     Mandatory telemetry variables - DO NOT DELETE ANY, else telemetry will fail: model_name, code, screenshot, html, source_nodes, instruction, url, origin, success
     """
     success_str = str(success)
     try:
         if TELEMETRY_VAR == "HIGH":
             r = requests.post(
                 "https://telemetrylavague.mithrilsecurity.io/send_data",
                 json={
+                    "version": get_installed_version("lavague"),
                     "code_produced": code,
                     "llm": model_name,
                     "screenshot": screenshot.decode("utf-8"),
                     "url": url,
                     "html_code": html,
                     "query": instruction,
                     "user_id": USER_ID,
                     "origin": origin,
                     "success": success_str,
+                    "source_nodes": source_nodes,
+                    "error_msg": error,
                     "test": test,
                 },
             )
             if r.status_code != 200:
                 raise ValueError(r.content)
         elif TELEMETRY_VAR is None or TELEMETRY_VAR == "LOW":
             r = requests.post(
                 "https://telemetrylavague.mithrilsecurity.io/telemetry",
                 json={
+                    "version": get_installed_version("lavague"),
+                    "code_produced": code,
                     "llm": model_name,
                     "user_id": USER_ID,
                     "origin": origin,
                     "url": url,
                     "success": success_str,
                     "instruction": instruction,
+                    "source_nodes": source_nodes,
+                    "error_msg": error,
                     "test": test,
                 },
             )
             if r.status_code != 200:
                 raise ValueError(r.content)
         elif TELEMETRY_VAR == "NONE":
             pass
```

### Comparing `lavague-1.0.8/src/lavague/version_checker.py` & `lavague-1.0.9/src/lavague/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.8/src/lavague.egg-info/PKG-INFO` & `lavague-1.0.9/src/lavague.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague
-Version: 1.0.8
+Version: 1.0.9
 Summary: Selenium code generation from text instructions
 Author-email: Mithril Security <contact@mithrilsecurity.io>
 Maintainer-email: Mithril Security <contact@mithrilsecurity.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -230,28 +230,31 @@
 Requires-Dist: llama-index-embeddings-azure-openai==0.1.5
 Requires-Dist: llama-index-embeddings-openai==0.1.6
 Requires-Dist: llama-index-indices-managed-llama-cloud==0.1.4
 Requires-Dist: llama-index-legacy==0.9.48
 Requires-Dist: llama-index-llms-azure-openai==0.1.5
 Requires-Dist: llama-index-llms-litellm==0.1.4
 Requires-Dist: llama-index-llms-openai==0.1.9
+Requires-Dist: llama-index-llms-anthropic==0.1.8
+Requires-Dist: llama-index-llms-groq==0.1.3
 Requires-Dist: llama-index-multi-modal-llms-openai==0.1.4
 Requires-Dist: llama-index-program-openai==0.1.4
 Requires-Dist: llama-index-question-gen-openai==0.1.3
 Requires-Dist: llama-index-readers-file==0.1.9
 Requires-Dist: llama-index-readers-llama-parse==0.1.3
 Requires-Dist: llama-index-retrievers-bm25==0.1.3
 Requires-Dist: tree-sitter==0.21.0
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: nest_asyncio==1.6.0
 Requires-Dist: selenium==4.18.1
 Requires-Dist: google-search-results==2.4.2
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: gradio==4.21.0
 Requires-Dist: ipython
+Requires-Dist: langchain==0.1.10
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Provides-Extra: cuda
 Requires-Dist: accelerate==0.28.0; extra == "cuda"
 Requires-Dist: bitsandbytes==0.42.0; extra == "cuda"
 Provides-Extra: huggingface
@@ -261,41 +264,40 @@
 Requires-Dist: playwright==1.42.0; extra == "playwright"
 
 <p align="center">
   <a href="https://github.com/lavague-ai/LaVague/stargazers"><img src="https://img.shields.io/github/stars/lavague-ai/LaVague.svg?style=for-the-badge" alt="Stargazers"></a>
   <a href="https://github.com/lavague-ai/LaVague/issues"><img src="https://img.shields.io/github/issues/lavague-ai/LaVague.svg?style=for-the-badge" alt="Issues"></a>
   <a href="https://github.com/lavague-ai/LaVague/network/members"><img src="https://img.shields.io/github/forks/lavague-ai/LaVague.svg?style=for-the-badge" alt="Forks"></a>
   <a href="https://github.com/lavague-ai/LaVague/graphs/contributors"><img src="https://img.shields.io/github/contributors/lavague-ai/LaVague.svg?style=for-the-badge" alt="Contributors"></a>
-  <a href="https://github.com/lavague-ai/LaVague/blob/master/LICENSE.md"><img src="https://img.shields.io/github/license/lavague-ai/LaVague.svg?style=for-the-badge" alt="Apache License"></a>
 </p>
 </br>
 
 <div align="center">
   <img src="static/logo.png" width=140px: alt="LaVague Logo">
   <h1>Welcome to LaVague</h1>
 
 <h4 align="center">
  <a href="https://discord.gg/SDxn9KpqX9" target="_blank">
-    <img src="https://img.shields.io/badge/discord-000000?style=for-the-badge&colorB=555" height='35px' alt="Join our Discord server!">
+    <img src="https://dcbadge.vercel.app/api/server/SDxn9KpqX9?compact=true" height='35px' alt="Join our Discord server!">
   </a>
-  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/docs-000000?style=for-the-badge&colorB=07f" height='35px' alt="Docs"></a>
+  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/📄-docs-000000?style=for-the-badge&colorA=09c&colorB=555" height='35px' alt="Docs"></a>
 </h4>
-  <p>Copilot for devs to automate automation</p>
+  <p>The open-source community for Large Action Models</p>
 <h1></h1>
 </div>
 
 ## 🏄‍♀️  What is LaVague?
 
-LaVague is an **open-source** project designed to automate automation for devs! 
+LaVague is an **open-source Large Action Model framework** for turning **natural language** into **browser actions**.
 
-We use **advanced AI techniques** (RAG, Few-shot learning, Chain of Thought) to turn **natural language instructions** into Python code leveraging **Selenium**. LaVague is designed to make it easy for users to **automate web workflows** and execute them on a browser.
+At LaVague's core, we have an **Action Engine** which uses **advanced AI techniques** (RAG, Few-shot learning, Chain of Thought) to “compile” natural language instructions into browser automation code, by leveraging **Selenium** or **Playwright**.
 
 ### LaVague in Action
 
-Here's an example to show how LaVague can execute natural language instructions on a browser to automate interactions with a website:
+Here's an example of LaVague being used to execute natural language instructions on a browser to automate web interactions. This example uses the Gradio interface available with the `lavague launch` CLI command:
 
 <div>
   <figure>
     <img src="static/hf_lavague.gif" alt="LaVague Interaction Example" style="margin-right: 20px;">
     <figcaption><b>LaVague interacting with Hugging Face's website.</b></figcaption>
   </figure>
   <br><br>
@@ -306,38 +308,40 @@
 ### Running LaVague in your local env
 
 You can get started with `LaVague` in 2 steps:
 
 1. Install LaVague & dependencies
 ```
 wget https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh &&
-sudo bash setup.sh
+bash setup.sh
 ```
 
 2. Run your LaVague command!
 
-You can either `launch` an interactive demo, where LaVague will execute and show you the results of the automation code it generates for your instruction.
+You can either `launch` an interactive Gradio interface, where you will see both the automation code generated for each instruction but also a live preview of the results of executing the code with a debug tab:
 ```
-lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py launch
+lavague launch
 ```
 
-Or you can use the `build` command to directly get the Python code leveraging Selenium in a file, which you can then inspect & execute locally.
+Or you can use the `build` command to directly get the Python code leveraging Selenium in a file, which you can then inspect & execute locally:
 ```
-lavague --instructions examples/instructions/huggingface.yaml --config examples/configurations/api/openai_api.py build
+lavague build
 ```
 
-For a step-by-step guide or to run LaVague in a Google Colab, see our [quick-tour](https://docs.lavague.ai/en/latest/docs/get-started/quick-tour/) which will walk you through how to get set-up and launch LaVague with our CLI tool.
+> Note, you'll need an OpenAI API key for this default example and will need the `OPENAI_API_KEY` set in your environment. To use LaVague with a different API, see our [integrations section](https://docs.lavague.ai/en/latest/docs/integrations/home/).
+
+For an end-to-end example of LaVague in a Google Colab, see our [quick-tour notebook](https://colab.research.google.com/github/lavague-ai/lavague/blob/main/docs/docs/get-started/quick-tour-notebook/quick-tour.ipynb)
 
 ## 🎭 Playwright integration
 
 If you want to get started with LaVague build using Playwright as your underlying automation tool, see our [Playwright integration guide](./docs/docs/get-started/playwright.md)
 
 ## 🙋 Contributing
 
-We would love your help in making La Vague a reality. 
+We would love your help and support on our quest to build a robust and reliable Large Action Model for web automation.
 
 To avoid having multiple people working on the same things & being unable to merge your work, we have outlined the following contribution process:
 
 1) 📢 We outline tasks on our [`backlog`](https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-ai/LaVague/labels/good%20first%20issue) labels
 2) 🙋‍♀️ If you are interested in working on one of these tasks, comment on the issue! 
 3) 🤝 We will discuss with you and assign you the task with a [`community assigned`](https://github.com/lavague-ai/LaVague/labels/community-assigned) label 
 4) 💬 We will then be available to discuss this task with you
@@ -350,8 +354,8 @@
 
 ## 🗺️ Roadmap
 
 TO keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
 
 ### 🚨 Disclaimer
 
-This project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
+Note, this project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
```

### Comparing `lavague-1.0.8/src/lavague.egg-info/SOURCES.txt` & `lavague-1.0.9/src/lavague.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 README.md
 pyproject.toml
 src/lavague/__init__.py
 src/lavague/action_engine.py
 src/lavague/command_center.py
 src/lavague/defaults.py
 src/lavague/driver.py
+src/lavague/evaluator.py
 src/lavague/format_utils.py
 src/lavague/prompts.py
+src/lavague/retrievers.py
 src/lavague/telemetry.py
 src/lavague/version_checker.py
 src/lavague/vscode_extension.py
 src/lavague.egg-info/PKG-INFO
 src/lavague.egg-info/SOURCES.txt
 src/lavague.egg-info/dependency_links.txt
 src/lavague.egg-info/entry_points.txt
```

### Comparing `lavague-1.0.8/src/lavague.egg-info/requires.txt` & `lavague-1.0.9/src/lavague.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 llama-index-embeddings-azure-openai==0.1.5
 llama-index-embeddings-openai==0.1.6
 llama-index-indices-managed-llama-cloud==0.1.4
 llama-index-legacy==0.9.48
 llama-index-llms-azure-openai==0.1.5
 llama-index-llms-litellm==0.1.4
 llama-index-llms-openai==0.1.9
+llama-index-llms-anthropic==0.1.8
+llama-index-llms-groq==0.1.3
 llama-index-multi-modal-llms-openai==0.1.4
 llama-index-program-openai==0.1.4
 llama-index-question-gen-openai==0.1.3
 llama-index-readers-file==0.1.9
 llama-index-readers-llama-parse==0.1.3
 llama-index-retrievers-bm25==0.1.3
 tree-sitter==0.21.0
 tree-sitter-languages==1.10.2
 nest_asyncio==1.6.0
 selenium==4.18.1
 google-search-results==2.4.2
 python-dotenv==1.0.1
 gradio==4.21.0
 ipython
+langchain==0.1.10
 
 [cuda]
 accelerate==0.28.0
 bitsandbytes==0.42.0
 
 [dev]
 ruff
```

