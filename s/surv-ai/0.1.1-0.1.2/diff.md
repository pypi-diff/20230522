# Comparing `tmp/surv_ai-0.1.1.tar.gz` & `tmp/surv_ai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surv_ai-0.1.1.tar", max compression
+gzip compressed data, was "surv_ai-0.1.2.tar", max compression
```

## Comparing `surv_ai-0.1.1.tar` & `surv_ai-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.1.1/LICENSE
--rw-r--r--   0        0        0    19613 2023-05-22 16:58:47.362127 surv_ai-0.1.1/README.md
--rw-r--r--   0        0        0     1447 2023-05-22 16:59:10.479839 surv_ai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1300 2023-05-22 16:09:44.521296 surv_ai-0.1.1/surv_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.1.1/surv_ai/core/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.1.1/surv_ai/core/agent.py
--rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.1.1/surv_ai/core/agents/__init__.py
--rw-r--r--   0        0        0     1608 2023-05-22 15:04:42.549505 surv_ai-0.1.1/surv_ai/core/agents/binary.py
--rw-r--r--   0        0        0     6979 2023-05-22 15:18:19.376795 surv_ai-0.1.1/surv_ai/core/agents/reasoning.py
--rw-r--r--   0        0        0     1855 2023-05-22 16:09:44.526670 surv_ai-0.1.1/surv_ai/core/interfaces.py
--rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.1.1/surv_ai/core/model.py
--rw-r--r--   0        0        0     4718 2023-05-22 16:09:44.529673 surv_ai-0.1.1/surv_ai/core/survey.py
--rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.1.1/surv_ai/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.1.1/surv_ai/lib/conversation/__init__.py
--rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.1.1/surv_ai/lib/conversation/conversation.py
--rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.1.1/surv_ai/lib/conversation/interfaces.py
--rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.1.1/surv_ai/lib/knowledge_store/__init__.py
--rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.1.1/surv_ai/lib/knowledge_store/interfaces.py
--rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.1.1/surv_ai/lib/knowledge_store/local.py
--rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.1.1/surv_ai/lib/llm/__init__.py
--rw-r--r--   0        0        0     3755 2023-05-22 16:07:39.753305 surv_ai-0.1.1/surv_ai/lib/llm/anthropic.py
--rw-r--r--   0        0        0     4261 2023-05-22 16:07:57.537852 surv_ai-0.1.1/surv_ai/lib/llm/gpt.py
--rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.1.1/surv_ai/lib/llm/interfaces.py
--rw-r--r--   0        0        0     1960 2023-05-22 15:04:42.613196 surv_ai-0.1.1/surv_ai/lib/log.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.1.1/surv_ai/lib/tools/__init__.py
--rw-r--r--   0        0        0      656 2023-05-22 15:04:42.577518 surv_ai-0.1.1/surv_ai/lib/tools/interfaces.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.1.1/surv_ai/lib/tools/query/__init__.py
--rw-r--r--   0        0        0     7047 2023-05-22 16:09:44.603986 surv_ai-0.1.1/surv_ai/lib/tools/query/google_custom_search.py
--rw-r--r--   0        0        0      219 2023-05-19 05:42:04.105413 surv_ai-0.1.1/surv_ai/lib/tools/query/interfaces.py
--rw-r--r--   0        0        0     5918 2023-05-22 16:09:44.606441 surv_ai-0.1.1/surv_ai/lib/tools/query/wikipedia.py
--rw-r--r--   0        0        0     2922 2023-05-22 16:09:44.577037 surv_ai-0.1.1/surv_ai/lib/tools/toolbelt.py
--rw-r--r--   0        0        0    20963 1970-01-01 00:00:00.000000 surv_ai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.1.2/LICENSE
+-rw-r--r--   0        0        0    19691 2023-05-22 17:52:13.692320 surv_ai-0.1.2/README.md
+-rw-r--r--   0        0        0     1447 2023-05-22 17:53:16.594063 surv_ai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1300 2023-05-22 16:09:44.521296 surv_ai-0.1.2/surv_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.1.2/surv_ai/core/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.1.2/surv_ai/core/agent.py
+-rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.1.2/surv_ai/core/agents/__init__.py
+-rw-r--r--   0        0        0     1608 2023-05-22 15:04:42.549505 surv_ai-0.1.2/surv_ai/core/agents/binary.py
+-rw-r--r--   0        0        0     6979 2023-05-22 15:18:19.376795 surv_ai-0.1.2/surv_ai/core/agents/reasoning.py
+-rw-r--r--   0        0        0     1855 2023-05-22 16:09:44.526670 surv_ai-0.1.2/surv_ai/core/interfaces.py
+-rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.1.2/surv_ai/core/model.py
+-rw-r--r--   0        0        0     4718 2023-05-22 16:09:44.529673 surv_ai-0.1.2/surv_ai/core/survey.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.1.2/surv_ai/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.1.2/surv_ai/lib/conversation/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.1.2/surv_ai/lib/conversation/conversation.py
+-rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.1.2/surv_ai/lib/conversation/interfaces.py
+-rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.1.2/surv_ai/lib/knowledge_store/__init__.py
+-rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.1.2/surv_ai/lib/knowledge_store/interfaces.py
+-rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.1.2/surv_ai/lib/knowledge_store/local.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.1.2/surv_ai/lib/llm/__init__.py
+-rw-r--r--   0        0        0     3755 2023-05-22 16:07:39.753305 surv_ai-0.1.2/surv_ai/lib/llm/anthropic.py
+-rw-r--r--   0        0        0     4261 2023-05-22 16:07:57.537852 surv_ai-0.1.2/surv_ai/lib/llm/gpt.py
+-rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.1.2/surv_ai/lib/llm/interfaces.py
+-rw-r--r--   0        0        0     1960 2023-05-22 15:04:42.613196 surv_ai-0.1.2/surv_ai/lib/log.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.1.2/surv_ai/lib/tools/__init__.py
+-rw-r--r--   0        0        0      656 2023-05-22 15:04:42.577518 surv_ai-0.1.2/surv_ai/lib/tools/interfaces.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.1.2/surv_ai/lib/tools/query/__init__.py
+-rw-r--r--   0        0        0     7047 2023-05-22 16:09:44.603986 surv_ai-0.1.2/surv_ai/lib/tools/query/google_custom_search.py
+-rw-r--r--   0        0        0      219 2023-05-19 05:42:04.105413 surv_ai-0.1.2/surv_ai/lib/tools/query/interfaces.py
+-rw-r--r--   0        0        0     5918 2023-05-22 16:09:44.606441 surv_ai-0.1.2/surv_ai/lib/tools/query/wikipedia.py
+-rw-r--r--   0        0        0     2922 2023-05-22 16:09:44.577037 surv_ai-0.1.2/surv_ai/lib/tools/toolbelt.py
+-rw-r--r--   0        0        0    21041 1970-01-01 00:00:00.000000 surv_ai-0.1.2/PKG-INFO
```

### Comparing `surv_ai-0.1.1/LICENSE` & `surv_ai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/README.md` & `surv_ai-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# Multi-agent modeling with large language models
+# 🕵 Multi-agent modeling with large language models 
 <!-- [![PyPi](https://img.shields.io/badge/Official%20Website-agpt.co-blue?style=flat&logo=world&logoColor=white)](https://agpt.co) -->
 [![Unit Tests](https://shields.io/github/actions/workflow/status/DanielBalsam/surv_ai/.github/workflows/ci.yaml?branch=main)](https://github.com/DanielBalsam/surv_ai/actions/workflows/ci.yaml)
 [![GitHub Repo stars](https://img.shields.io/github/stars/DanielBalsam/surv_ai?style=social)](https://github.com/DanielBalsam/surv_ai/stargazers)
 
 
-**`surv_ai` is a large language model framework designed for multi-agent modeling allowing large-language models to be used as engines to power research into predictive modeling, bias analysis, and other forms of comparative analysis.**
+**`surv_ai` is a large language model framework designed for multi-agent modeling. This allows large-language models to be used as engines to power research into predictive modeling, bias analysis, and other forms of comparative analysis.**
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
 
 **Multi-agent modeling** is the process of using the actions of various agents in order to produce statistical models. In our case, these models are created by having agents query and process text from a robust data corpus, and then "reason" with the information extracted from that text to produce a data point.
 
 Given the stochastic nature of large language models, each data point may vary - however if a large enough sample of agents are used, the models that can be produced can be effective for comparative analysis.
 
 The abstraction in this repository that is capable of producing a data point is referred to as an `Survey`. A survey takes a statement as an argument and returns a percentage of agents which agreed with the statement.
 
 A model that varies with respect to some independent variable a further abstraction called a `Model`, which allows us to vary input parameters into a `Survey` creating a proper multi-agent model.
 
-The survey values produced are ultimately end up being a form of sentiment analysis against a corpus of text. This means they are subject to the biases of both the large language models, and the corpus of text itself. 
+The data points produced are ultimately end up being a form of sentiment analysis against a corpus of text. This means they are subject to the biases of both the large language models, and the corpus of text itself. 
 
 With further advances in large language models, and AI broadly, multi-agent modeling may continue to prove a useful paradigm for classification and regression models, and may become a valuable extra data point for researchers investigating complex issues with many complex underlying variables.
 
-# Installation
+## 📲 Installation 
 
-Package is available on PyPi: 
+Package is available on [PyPi](https://pypi.org/project/surv-ai/): 
 
 ```
 pip install surv-ai
 ```
 
-# Contact
+## 📻 Contact 
 
 For all inqueries, contact me at: daniel.balsam@survai.org
 
-# Responsible use
+## ✅ Responsible use 
 
 Examples below are meant to simply demonstrate the potential use-cases of this framework, and are not to be interpreted as scientifically rigorous.
 
 While approaches like this have the potential to be used in research and guide decision making, it is important to always use a wide-variety of data points and to take any particular model with a grain of salt.
 
 I am always eager for suggestions on how this approach can be further improved.
 
-# Basic usage
+## 📝 Basic usage 
 
 The two key abstractions in this repository are a `Survey` and a `Model`. 
 
 Calling `Survey.conduct` with a hypothesis will spin up a number of agents and seed them with some base knowledge. The agents are then asked to to assign a true or false value to the hypothesis provided. 
 
 ```
 class Survey:
@@ -78,25 +78,25 @@
 
     async def build(self, hypothesis: str) -> list[DataPoint]:
         ...
 ```
 
 Abstractions implemented in this repository all adhere to simple abstract interfaces - so you can easily build your own agents, surveys, and models.
 
-# Examples
+## 🎓 Examples 
 
 All the below examples will be conducted with either GPT or Claude, and Google Custom Search. Links to relevant docs to get your own API keys:
 
 [**OpenAI / GPT**](https://platform.openai.com/)
 [**Anthropic / Claude**](https://console.anthropic.com/docs)
 [**Google Custom Search**](https://developers.google.com/custom-search/v1/overview)
 
-## Comparing against a ground truth
+### Comparing against a ground truth
 
-### Making sure we can get unambigious answers
+#### Making sure we can get unambigious answers
 
 Let's start by establishing the system's ability to figure out if information is true.
 
 For instance:
 
 ```
 from surv_ai import (
@@ -139,15 +139,15 @@
 )  # This should always returns high a confidence agreement.
 ```
 
 Running this code should produce an output like: `PollResponse(in_favor=10, against=0, undecided=0, error=0, percent_in_favor=1.0, uncertainty=0.0)`
 
 It's worth noting that every so often, an agent or two may get a simple question like this wrong. That is why we use many agents in these systems - to combat the stochastic nature of LLMs.
 
-### The inverse statement should produce the inverse probability
+#### The inverse statement should produce the inverse probability
 
 Another way to test our system is to make the opposite assertion and make sure we can the opposite value.
 
 ```
 from surv_ai import (
     GPTClient,
     Survey,
@@ -185,15 +185,15 @@
 await survey.conduct(
     "California experienced little rainfall this winter.",
 )  # This should always returns a high confidence disagreement.
 ```
 
 Running this code should produce an output like: `PollResponse(in_favor=0, against=10, undecided=0, error=0, percent_in_favor=0.0, uncertainty=0.0)`
 
-## Comparing changes in sentiment over time
+### Comparing changes in sentiment over time
 
 One thing we can use this tool for is measuring changes in sentiment overtime. GPT's training data ends in late 2021, so one way we can test our models with GPT is by looking at events that happened after GPT's training cutoff.
 
 For instance, we can plot how sentiment regarding the United States' 2022 Midterm Elections evolved in the months leading up to it:
 
 ```
 from surv_ai import (
@@ -214,15 +214,14 @@
     ('2022-07-01', '2022-08-01'),
     ('2022-08-01', '2022-09-01'),
     ('2022-09-01', '2022-10-01'),
     ('2022-10-01', '2022-11-05'),
 ]
 
 model = Model(
-    client,
     Survey,
     parameters=[
         SurveyParameter(
             independent_variable=range[1],
             parameters={
                 "n_agents": 100,
                 "max_knowledge_per_agent": 3,
@@ -283,15 +282,14 @@
     ('2022-06-01', '2022-09-01'),
     ('2022-09-01', '2023-01-01'),
     ('2023-01-01', '2023-03-01'),
     ('2023-03-01', '2023-06-01'),
 ]
 
 model = Model(
-    client,
     Survey,
     parameters=[
         SurveyParameter(
             independent_variable=range[1],
             parameters={
                 "n_agents": 100,
                 "max_knowledge_per_agent": 3,
@@ -327,15 +325,15 @@
 ```
 
 This gives us the following graph:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/cci.png)
 *Websites crawled by the agents in this example: nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, nbcnews.com*
 
-## Measuring bias in different data corpuses
+### Measuring bias in different data corpuses
 
 One promising use of this technique is to observe biases between different language corpuses. For instance - we can create a model that uses different news sites as its independent variable, to see how the agents conclusions may difer using that data source.
 
 ```
 from surv_ai import (
     GPTClient,
     Model,
@@ -351,15 +349,14 @@
     "cnn.com",
     "wsj.com",
     "foxnews.com",
 ]
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 model = Model(
-    client,
     Survey,
     parameters=[
         SurveyParameter(
             independent_variable=source,
             parameters={
                 "toolbelt": Toolbelt(
                     client,
@@ -393,15 +390,15 @@
 )
 ```
 
 This gives us the following scatter plot for the news sources above:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/debt_ceiling.png)
 
-# Measuring biases in different large language models
+### Measuring biases in different large language models
 
 Another promising bias mesurement approach is to compare biases across large language models, otherwise given the same parameters as input.
 
 ```
 from surv_ai import (
     GPTClient,
     AnthropicClient,
@@ -456,15 +453,15 @@
 ```
 
 Comparing this statement between Claude and OpenAI, we get the following scatterplot:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/openai.png)
 
 
-# Tips
+## 🧠 Tips 
 
 Ultimately a `Survey` is powered by an LLM, and so the survey hypothesis may need to be tuned the same way that prompts more generally need to be tuned. Here are some tips for thinking about how to write hypotheses.
 
 In these systems, often ambiguity in the original hypothesis can lead to strange results. This is often because the agents are interpreting the statement a little too literally, and thus rejecting the exact phrasing of the statement.
 
 Another helpful trick is to seed base knowledge to the agents which provides additional context to the problem. To revisit an earlier example:
 
@@ -539,29 +536,29 @@
         source="Context"
     )
 )
 
 agent.prompt("There are multiple ways to teach an agent knowledge.")
 ```
 
-# Inspiration
+## 🤩 Inspiration 
 
 This project was inspired by many other cool projects and papers coming out recently. Some of the inspirations for this project are:
 
 1. [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442).
 2. [Large Language Models are Zero-Shot Reasoners](https://arxiv.org/abs/2205.11916)
 3. [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT)
 
 And the many other researchers and engineers out there helping unlock the power of these models!
 
-# Next steps
+## 📈 Next steps 
 
 A few of the next places I'd like to take this project are:
 
 1. I am considering migrating the core LLM interaction code to leverage [Microsoft's Guidance framework](https://github.com/microsoft/guidance).
 2. Continue to refine the agent code to lead to better decision making agents across a wide variety of problems. Very interested in exploring [Tree of Thought Prompting](https://arxiv.org/pdf/2305.10601.pdf) to see what results are yielded there.
 3. Integrations with more instruction-tuned and RL'd LLMs.
 
 
-# Contribute
+## 🤝 Contribute 
 
 If you'd like to contribute then please reach out!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `surv_ai-0.1.1/pyproject.toml` & `surv_ai-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surv_ai"
-version = "0.1.1"
+version = "0.1.2"
 description = "A framework for multi-agent modeling using large language models"
 authors = ["Daniel Balsam <daniel.balsam@survai.org>"]
 license = "MIT"
 readme = "README.md"
 keywords=[
     "ai",
     "artificial intelligence",
```

### Comparing `surv_ai-0.1.1/surv_ai/__init__.py` & `surv_ai-0.1.2/surv_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/core/agent.py` & `surv_ai-0.1.2/surv_ai/core/agent.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/core/agents/binary.py` & `surv_ai-0.1.2/surv_ai/core/agents/binary.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/core/agents/reasoning.py` & `surv_ai-0.1.2/surv_ai/core/agents/reasoning.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/core/interfaces.py` & `surv_ai-0.1.2/surv_ai/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/core/model.py` & `surv_ai-0.1.2/surv_ai/core/model.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/core/survey.py` & `surv_ai-0.1.2/surv_ai/core/survey.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/lib/conversation/conversation.py` & `surv_ai-0.1.2/surv_ai/lib/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/lib/knowledge_store/interfaces.py` & `surv_ai-0.1.2/surv_ai/lib/knowledge_store/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/lib/knowledge_store/local.py` & `surv_ai-0.1.2/surv_ai/lib/knowledge_store/local.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/lib/llm/anthropic.py` & `surv_ai-0.1.2/surv_ai/lib/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/lib/llm/gpt.py` & `surv_ai-0.1.2/surv_ai/lib/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/lib/log.py` & `surv_ai-0.1.2/surv_ai/lib/log.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/lib/tools/interfaces.py` & `surv_ai-0.1.2/surv_ai/lib/tools/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/lib/tools/query/google_custom_search.py` & `surv_ai-0.1.2/surv_ai/lib/tools/query/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/lib/tools/query/wikipedia.py` & `surv_ai-0.1.2/surv_ai/lib/tools/query/wikipedia.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/surv_ai/lib/tools/toolbelt.py` & `surv_ai-0.1.2/surv_ai/lib/tools/toolbelt.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.1/PKG-INFO` & `surv_ai-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surv-ai
-Version: 0.1.1
+Version: 0.1.2
 Summary: A framework for multi-agent modeling using large language models
 Home-page: https://github.com/DanielBalsam/surv_ai
 License: MIT
 Keywords: ai,artificial intelligence,data science,statistics,models,llm,agents,survai,surv_ai,survey,multi-agent,large language model,artificial intelligence,machine learning,natural language processing,nlp,sentiment analysis
 Author: Daniel Balsam
 Author-email: daniel.balsam@survai.org
 Requires-Python: >=3.9,<4.0
@@ -22,57 +22,57 @@
 Requires-Dist: exceptiongroup (>=1.1.1,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://github.com/DanielBalsam/surv_ai/blob/main/README.md
 Project-URL: Repository, https://github.com/DanielBalsam/surv_ai
 Description-Content-Type: text/markdown
 
-# Multi-agent modeling with large language models
+# 🕵 Multi-agent modeling with large language models 
 <!-- [![PyPi](https://img.shields.io/badge/Official%20Website-agpt.co-blue?style=flat&logo=world&logoColor=white)](https://agpt.co) -->
 [![Unit Tests](https://shields.io/github/actions/workflow/status/DanielBalsam/surv_ai/.github/workflows/ci.yaml?branch=main)](https://github.com/DanielBalsam/surv_ai/actions/workflows/ci.yaml)
 [![GitHub Repo stars](https://img.shields.io/github/stars/DanielBalsam/surv_ai?style=social)](https://github.com/DanielBalsam/surv_ai/stargazers)
 
 
-**`surv_ai` is a large language model framework designed for multi-agent modeling allowing large-language models to be used as engines to power research into predictive modeling, bias analysis, and other forms of comparative analysis.**
+**`surv_ai` is a large language model framework designed for multi-agent modeling. This allows large-language models to be used as engines to power research into predictive modeling, bias analysis, and other forms of comparative analysis.**
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
 
 **Multi-agent modeling** is the process of using the actions of various agents in order to produce statistical models. In our case, these models are created by having agents query and process text from a robust data corpus, and then "reason" with the information extracted from that text to produce a data point.
 
 Given the stochastic nature of large language models, each data point may vary - however if a large enough sample of agents are used, the models that can be produced can be effective for comparative analysis.
 
 The abstraction in this repository that is capable of producing a data point is referred to as an `Survey`. A survey takes a statement as an argument and returns a percentage of agents which agreed with the statement.
 
 A model that varies with respect to some independent variable a further abstraction called a `Model`, which allows us to vary input parameters into a `Survey` creating a proper multi-agent model.
 
-The survey values produced are ultimately end up being a form of sentiment analysis against a corpus of text. This means they are subject to the biases of both the large language models, and the corpus of text itself. 
+The data points produced are ultimately end up being a form of sentiment analysis against a corpus of text. This means they are subject to the biases of both the large language models, and the corpus of text itself. 
 
 With further advances in large language models, and AI broadly, multi-agent modeling may continue to prove a useful paradigm for classification and regression models, and may become a valuable extra data point for researchers investigating complex issues with many complex underlying variables.
 
-# Installation
+## 📲 Installation 
 
-Package is available on PyPi: 
+Package is available on [PyPi](https://pypi.org/project/surv-ai/): 
 
 ```
 pip install surv-ai
 ```
 
-# Contact
+## 📻 Contact 
 
 For all inqueries, contact me at: daniel.balsam@survai.org
 
-# Responsible use
+## ✅ Responsible use 
 
 Examples below are meant to simply demonstrate the potential use-cases of this framework, and are not to be interpreted as scientifically rigorous.
 
 While approaches like this have the potential to be used in research and guide decision making, it is important to always use a wide-variety of data points and to take any particular model with a grain of salt.
 
 I am always eager for suggestions on how this approach can be further improved.
 
-# Basic usage
+## 📝 Basic usage 
 
 The two key abstractions in this repository are a `Survey` and a `Model`. 
 
 Calling `Survey.conduct` with a hypothesis will spin up a number of agents and seed them with some base knowledge. The agents are then asked to to assign a true or false value to the hypothesis provided. 
 
 ```
 class Survey:
@@ -106,25 +106,25 @@
 
     async def build(self, hypothesis: str) -> list[DataPoint]:
         ...
 ```
 
 Abstractions implemented in this repository all adhere to simple abstract interfaces - so you can easily build your own agents, surveys, and models.
 
-# Examples
+## 🎓 Examples 
 
 All the below examples will be conducted with either GPT or Claude, and Google Custom Search. Links to relevant docs to get your own API keys:
 
 [**OpenAI / GPT**](https://platform.openai.com/)
 [**Anthropic / Claude**](https://console.anthropic.com/docs)
 [**Google Custom Search**](https://developers.google.com/custom-search/v1/overview)
 
-## Comparing against a ground truth
+### Comparing against a ground truth
 
-### Making sure we can get unambigious answers
+#### Making sure we can get unambigious answers
 
 Let's start by establishing the system's ability to figure out if information is true.
 
 For instance:
 
 ```
 from surv_ai import (
@@ -167,15 +167,15 @@
 )  # This should always returns high a confidence agreement.
 ```
 
 Running this code should produce an output like: `PollResponse(in_favor=10, against=0, undecided=0, error=0, percent_in_favor=1.0, uncertainty=0.0)`
 
 It's worth noting that every so often, an agent or two may get a simple question like this wrong. That is why we use many agents in these systems - to combat the stochastic nature of LLMs.
 
-### The inverse statement should produce the inverse probability
+#### The inverse statement should produce the inverse probability
 
 Another way to test our system is to make the opposite assertion and make sure we can the opposite value.
 
 ```
 from surv_ai import (
     GPTClient,
     Survey,
@@ -213,15 +213,15 @@
 await survey.conduct(
     "California experienced little rainfall this winter.",
 )  # This should always returns a high confidence disagreement.
 ```
 
 Running this code should produce an output like: `PollResponse(in_favor=0, against=10, undecided=0, error=0, percent_in_favor=0.0, uncertainty=0.0)`
 
-## Comparing changes in sentiment over time
+### Comparing changes in sentiment over time
 
 One thing we can use this tool for is measuring changes in sentiment overtime. GPT's training data ends in late 2021, so one way we can test our models with GPT is by looking at events that happened after GPT's training cutoff.
 
 For instance, we can plot how sentiment regarding the United States' 2022 Midterm Elections evolved in the months leading up to it:
 
 ```
 from surv_ai import (
@@ -242,15 +242,14 @@
     ('2022-07-01', '2022-08-01'),
     ('2022-08-01', '2022-09-01'),
     ('2022-09-01', '2022-10-01'),
     ('2022-10-01', '2022-11-05'),
 ]
 
 model = Model(
-    client,
     Survey,
     parameters=[
         SurveyParameter(
             independent_variable=range[1],
             parameters={
                 "n_agents": 100,
                 "max_knowledge_per_agent": 3,
@@ -311,15 +310,14 @@
     ('2022-06-01', '2022-09-01'),
     ('2022-09-01', '2023-01-01'),
     ('2023-01-01', '2023-03-01'),
     ('2023-03-01', '2023-06-01'),
 ]
 
 model = Model(
-    client,
     Survey,
     parameters=[
         SurveyParameter(
             independent_variable=range[1],
             parameters={
                 "n_agents": 100,
                 "max_knowledge_per_agent": 3,
@@ -355,15 +353,15 @@
 ```
 
 This gives us the following graph:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/cci.png)
 *Websites crawled by the agents in this example: nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, nbcnews.com*
 
-## Measuring bias in different data corpuses
+### Measuring bias in different data corpuses
 
 One promising use of this technique is to observe biases between different language corpuses. For instance - we can create a model that uses different news sites as its independent variable, to see how the agents conclusions may difer using that data source.
 
 ```
 from surv_ai import (
     GPTClient,
     Model,
@@ -379,15 +377,14 @@
     "cnn.com",
     "wsj.com",
     "foxnews.com",
 ]
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 model = Model(
-    client,
     Survey,
     parameters=[
         SurveyParameter(
             independent_variable=source,
             parameters={
                 "toolbelt": Toolbelt(
                     client,
@@ -421,15 +418,15 @@
 )
 ```
 
 This gives us the following scatter plot for the news sources above:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/debt_ceiling.png)
 
-# Measuring biases in different large language models
+### Measuring biases in different large language models
 
 Another promising bias mesurement approach is to compare biases across large language models, otherwise given the same parameters as input.
 
 ```
 from surv_ai import (
     GPTClient,
     AnthropicClient,
@@ -484,15 +481,15 @@
 ```
 
 Comparing this statement between Claude and OpenAI, we get the following scatterplot:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/openai.png)
 
 
-# Tips
+## 🧠 Tips 
 
 Ultimately a `Survey` is powered by an LLM, and so the survey hypothesis may need to be tuned the same way that prompts more generally need to be tuned. Here are some tips for thinking about how to write hypotheses.
 
 In these systems, often ambiguity in the original hypothesis can lead to strange results. This is often because the agents are interpreting the statement a little too literally, and thus rejecting the exact phrasing of the statement.
 
 Another helpful trick is to seed base knowledge to the agents which provides additional context to the problem. To revisit an earlier example:
 
@@ -567,30 +564,30 @@
         source="Context"
     )
 )
 
 agent.prompt("There are multiple ways to teach an agent knowledge.")
 ```
 
-# Inspiration
+## 🤩 Inspiration 
 
 This project was inspired by many other cool projects and papers coming out recently. Some of the inspirations for this project are:
 
 1. [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442).
 2. [Large Language Models are Zero-Shot Reasoners](https://arxiv.org/abs/2205.11916)
 3. [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT)
 
 And the many other researchers and engineers out there helping unlock the power of these models!
 
-# Next steps
+## 📈 Next steps 
 
 A few of the next places I'd like to take this project are:
 
 1. I am considering migrating the core LLM interaction code to leverage [Microsoft's Guidance framework](https://github.com/microsoft/guidance).
 2. Continue to refine the agent code to lead to better decision making agents across a wide variety of problems. Very interested in exploring [Tree of Thought Prompting](https://arxiv.org/pdf/2305.10601.pdf) to see what results are yielded there.
 3. Integrations with more instruction-tuned and RL'd LLMs.
 
 
-# Contribute
+## 🤝 Contribute 
 
 If you'd like to contribute then please reach out!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

