# Comparing `tmp/autoxx-0.0.13.tar.gz` & `tmp/autoxx-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.13.tar", max compression
+gzip compressed data, was "autoxx-0.0.15.tar", max compression
```

## Comparing `autoxx-0.0.13.tar` & `autoxx-0.0.15.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.13/README.md
--rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.13/autoxx/agent/base.py
--rw-r--r--   0        0        0     1064 2023-05-08 14:09:26.013131 autoxx-0.0.13/autoxx/agent/researcher.py
--rw-r--r--   0        0        0     4239 2023-05-09 11:57:08.681233 autoxx-0.0.13/autoxx/agi.py
--rw-r--r--   0        0        0    14378 2023-05-11 01:33:36.997520 autoxx-0.0.13/autoxx/babyagi.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.13/autoxx/js/overlay.js
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.13/autoxx/requirements.txt
--rw-r--r--   0        0        0     5882 2023-05-11 02:40:14.967698 autoxx-0.0.13/autoxx/search/simple_search.py
--rw-r--r--   0        0        0     4924 2023-05-08 14:12:25.878274 autoxx-0.0.13/autoxx/task_manager.py
--rw-r--r--   0        0        0      632 2023-05-21 06:57:39.781738 autoxx-0.0.13/pyproject.toml
--rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 autoxx-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.15/README.md
+-rw-r--r--   0        0        0    10711 2023-05-22 11:51:13.235984 autoxx-0.0.15/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.15/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.15/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.15/autoxx/requirements.txt
+-rw-r--r--   0        0        0      619 2023-05-22 02:04:48.341958 autoxx-0.0.15/autoxx/setup.py
+-rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.15/autoxx/tools/knowledge_base/utils.py
+-rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.15/autoxx/tools/llm/utils.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.15/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0     4940 2023-05-22 07:06:52.064497 autoxx-0.0.15/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0      656 2023-05-22 12:05:49.769773 autoxx-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0     1025 1970-01-01 00:00:00.000000 autoxx-0.0.15/PKG-INFO
```

### Comparing `autoxx-0.0.13/autoxx/babyagi.py` & `autoxx-0.0.15/autoxx/agent/babyagi/agi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,305 +1,178 @@
 import json, time
-from typing import Dict, List, Dict
+from typing import Dict, List, Dict, Optional
+import logging
 
 from autogpt.llm_utils import create_chat_completion
 from autogpt.config import Config
-from autoxx.search.simple_search import browse_website
-from autogpt.commands.google_search import google_search
 
-response_format = """[
-    {
-        "id": 1,
-        "task": "task description",
-        "tool": "tool used to complete task"
-    },
-    {
-        "id": 2,
-        "task": "task description",
-        "tool": "tool used to complete task"
-    }
-]"""
-
-def create_message(prompt: str) -> List[Dict]:
-    """Create a message for the chat completion
-
-    Args:
-        chunk (str): The chunk of text to summarize
-        question (str): The question to answer
-
-    Returns:
-        Dict[str, str]: The message to send to the chat completion
-    """
-    return [
-        {
-            "role": "system",
-            "content": "You are a task manager AI."
-        },
-        {
-            "role": "user",
-            "content": prompt
-        }
-    ]
-
-# Initialize task list
-task_list = []
-
-# Initialize session_summary
-session_summary = ""
-
-### Task list functions ##############################
-
-def get_task_by_id(task_id: int):
-    for task in task_list:
-        if task["id"] == task_id:
-            return task
-    return None
-
-def get_completed_tasks():
-    return [task for task in task_list if task["status"] == "completed"]
-
-def init_task_list(objective: str) -> List[Dict]:
-    create_task_prompt = f"Complete your assigned task based on the objective: {objective}. Your task: develop a task list to complete the objective. \n Response:"
-    messages = create_message(create_task_prompt)
-    create_task_response = create_chat_completion(
-        model=Config().fast_llm_model,
-        messages=messages,
-    )
-
-    task_id_counter = 0
-    prompt = (
-        f"You are a task management AI tasked with creating tasks for the following objective: {objective}.\n"
-        f"Create new tasks based on the following plan delimited by triple backtick if necessary for the objective. Limit tasks types to those that can be completed with the available tools listed below. Task description should be detailed. "
-        f"The plan:```{create_task_response}```.\n"
-        f"The current tool option is [text-completion, google-search, web-scrape] only. "
-        f"For tasks using [web-scrape], provide only the URL to scrape as the task description. Do not provide placeholder URLs, but use ones provided by a search step or the initial objective. "
-        f"For tasks using [web-scrape], do not select url under these domains [g2.com]. "
-        f"For tasks using [google-search], provide the search query, and only the search query to use (eg. not 'research waterproof shoes, but 'waterproof shoes').\n"
-        f"Make sure all task IDs are in chronological order.\n"
-        f"Do not provide example URLs for [web-scrape].\n"
-        f"Do not include the result from the last task in the JSON, that will be added after..\n"
-        f"For efficiency, let's think step by step and create the tasks (up to 5 tasks) that are most critical to objective. The last task is always to provide a final summary report of all tasks.\n"
-        f"An example of the desired output format is: "
-        "[{\"id\": 1, \"task\": \"https://untapped.vc\", \"tool\": \"web-scrape\", \"dependent_task_id\": null, \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 2, \"task\": \"Analyze the contents of...\", \"tool\": \"text-completion\", \"dependent_task_id\": 1, \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 3, \"task\": \"Untapped Capital\", \"tool\": \"google-search\", \"dependent_task_id\": [1,2], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}]."
-        f"\nEnsure the response can be parsed by Python json.loads\n"
-    )
-
-    messages = create_message(prompt)
-    response = create_chat_completion(
-        model=Config().fast_llm_model,
-        messages=messages,
-    )
-
-    new_tasks = json.loads(response)
-    task_list = []
-    for new_task in new_tasks:
-        task_id_counter += 1
-        new_task.update({"id": task_id_counter})
-        task_list.append(new_task)
-    return task_list
-
-def task_manager_agent(objective: str, task: Dict, result: str) -> List[Dict]:
-    global task_list
-    original_task_list = task_list.copy()
-    minified_task_list = [{k: v for k, v in task.items() if k != "result"} for task in task_list]
-    result = result[0:4000] #come up with better solution later.
-    
-    prompt = (
-        f"You are a task management AI tasked with cleaning the formatting of and reprioritizing the following tasks delimited by triple backtick:```{minified_task_list}```\n"
-        f"the last completed task (task id = {task['id']}, tool = {task['tool']}) has the following result delimited by triple backtick: ```{result}```\n\n"
-        f"Your task: Consider the ultimate objective of your team: {objective} and the completed tasks, re-create the task list (up to 8 tasks) to make it better to complete the objective. Don not remove the completed tasks.\n" 
-        f"The current tool option is [text-completion, google-search, web-scrape] only. "
-        f"If a [google-search] task is completed, create one or two necessary [web-scrape] tasks to get objective related documents will always be useful.\n"
-        f"For tasks using [web-scrape], provide only the URL to scrape as the task description. Do not provide placeholder URLs, but use ones provided by a search step or the initial objective. "
-        f"For tasks using [web-scrape], do not select url under these domains [g2.com], do not provide example URLs"
-        f"For tasks using [google-search], provide the search query, and only the search query to use (eg. not 'research waterproof shoes, but 'waterproof shoes'). "
-        f"The dependent_task_id should always be null or a number or a number list.\n"
-        f"Make sure all task IDs are in chronological order.\n"
-        f"Don not remove the completed tasks.\n"
-        f"Do not include the result from the last task in the JSON, that will be added after..\n"
-        f"The last task is always to provide a final summary report of all tasks.\n"
-        f"An example of the desired output format is: "
-        "[{\"id\": 1, \"task\": \"https://untapped.vc\", \"tool\": \"web-scrape\", \"dependent_task_id\": null, \"status\": \"incomplete\", \"result_summary\": null}, {\"id\": 2, \"task\": \"Analyze the contents of...\", \"tool\": \"text-completion\", \"dependent_task_id\": 1, \"status\": \"incomplete\", \"result_summary\": null}, {\"id\": 3, \"task\": \"Untapped Capital\", \"tool\": \"google-search\", \"dependent_task_id\": [1,2], \"status\": \"incomplete\", \"result_summary\": null}]."
-        f"\nEnsure the response can be parsed by Python json.loads\n"
-    )
-    print("\033[90m\033[3m" + "\nRunning task manager agent...\n" + "\033[0m")
-
-    messages = create_message(prompt)
-    result = create_chat_completion(
-        model=Config().fast_llm_model,
-        messages=messages,
-    )
-
-    print("\033[90m\033[3m" + "\nDone!\n" + "\033[0m")
-    try:
-      task_list = json.loads(result)
-    except Exception as error:
-      print(error)
-    # Add the 'result' field back in
-
-    for updated_task, original_task in zip(task_list, original_task_list):
-        if "result" in original_task:
-            updated_task["result"] = original_task["result"]
-
-    return task_list
-
-def LLM_agent(prompt: str) -> str:
-    messages = create_message(prompt)
-    response = create_chat_completion(
-        model=Config().fast_llm_model,
-        messages=messages,
-    )
-
-    return response
-
-def overview_agent(task: Dict) -> str:
-    global session_summary
-
-    completed_tasks = get_completed_tasks()
-    completed_tasks_text = "\n".join(
-        [f"{task['id']}. {task['task']} - {task['result_summary']}" for task in completed_tasks]
-    )
-
-    prompt = (
-        f"Here is the current session summary delimited by triple backtick: \n```{session_summary}```\n"
-        f"The last completed task is task {task['task']} using tools {task['tool']}. Please update the session summary with the information of the last task:\n{completed_tasks_text}\n"
-        f"For tasks using [google-search], keeps all links to the search results. And don't discard related links in updating\n"
-        f"Updated session summary, which should describe all tasks in chronological order:"
-    )
-    messages = create_message(prompt)
-    response = create_chat_completion(
-        model=Config().fast_llm_model,
-        messages=messages,
-    )
-    session_summary = response
-    return session_summary
-
-def web_browse_tool(url:str, dependent_task_ids: List, objective: str)-> str:
-    question = f"Extract relevant information from this article that is useful for objective: {objective}..."
-
-    dependent_task_description = []
-    for dependent_task_id in dependent_task_ids:
-        dependent_task = get_task_by_id(dependent_task_id)
-        if dependent_task and dependent_task["tool"] == "google-search":
-            dependent_task_description.append(dependent_task["task"])
-
-
-    if len(dependent_task_description) > 0:
-        question += f" and questions:[{', '.join(dependent_task_description)}]"
-
-    print(f"web_browse_tool {url} {question}\n")
-
-    result = '\n'.join(browse_website(url, question))
-    return result
-
-### Agent functions ##############################
-def execute_task(task: Dict, objective: str):
-    global task_list
-    # Check if dependent_task_id is completed
-    dependent_task_ids = []
-    dependent_task_prompt = ""
-    if task["dependent_task_id"]:
-        if isinstance(task["dependent_task_id"], list):
-            dependent_task_ids = task["dependent_task_id"]
-        else:
-            dependent_task_ids = [task["dependent_task_id"]]
+from autoxx.tools.web_search.search import web_search
+from autoxx.tools.llm.utils import llm_uils, create_message
 
-        for dependent_task_id in dependent_task_ids:
-            dependent_task = get_task_by_id(dependent_task_id)
-            if dependent_task and dependent_task["status"] != "completed":
-                return
-            elif dependent_task:
-                dependent_task_prompt += f"\ntask ({dependent_task['id']}. {dependent_task['task']}) result: {dependent_task['result']}"
 
-    # Execute task
-    
-    print("\033[92m\033[1m"+"\n*****NEXT TASK*****\n"+"\033[0m\033[0m")
-    print(str(task['id'])+": "+str(task['task'])+" ["+str(task['tool']+"]"))
-    task_prompt = f"Complete your assigned task based on the objective: {objective}. Your task: {task['task']}"
-    if dependent_task_prompt != "":
-        task_prompt += f"\nThe previous tasks: {dependent_task_prompt}"
-
-    task_prompt += "\nResponse:"
-    if task["tool"] == "text-completion":
-        result = LLM_agent(task_prompt)
-        summary_result_prompt = f"Please summarize the following text:\n{result}\nSummary:"
-        task["result_summary"] = LLM_agent(summary_result_prompt)
-    elif task["tool"] == "google-search":
-        result = google_search(str(task['task']))
-        summary_result_prompt = f"Please summarize the following google search result and keep all links:\n{result}\nSummary:"
-        task["result_summary"] = LLM_agent(summary_result_prompt)
-    elif task["tool"] == "web-scrape":
-        result = web_browse_tool(str(task['task']), dependent_task_ids, objective)
-        summary_result_prompt = f"Please summarize the following text:\n{result}\nSummary:"
-        task["result_summary"] = LLM_agent(summary_result_prompt)
-    else:
-        result = "Unknown tool"
+class AGIExecutor:
+    def __init__(self, objective:str, max_tasks_count: Optional[int] = 5):
+        if objective is None or len(objective) <= 1:  
+            raise ValueError("Must provide an objective")  
+
+        self.objective = objective
+        self.max_tasks_count = max_tasks_count
+
+        self.task_list = self.init_task_list(objective)
+        self.status = "initizing"
+        self.error_message = None
+        self.final_answer = None
+
+    def get_task_by_id(self, task_id: int):
+        for task in self.task_list:
+            if task["id"] == task_id:
+                return task
+        return None
+
+    def init_task_list(self, objective: str) -> List[Dict]:
+        task_id_counter = 0
+        prompt = (
+            f"You are a QA AI tasked with creating tasks for the following objective: {objective}.\n"
+            f"Create new tasks based on the following plan delimited by triple backtick if necessary for the objective. Limit tasks types to those that can be completed with the available tools listed below. Task description should be detailed. "
+            f"The plan:```decelop a task list```.\n"
+            f"The current tool option is [text-completion, web-search] only. What each tool does is as follows:\n"
+            f"web-search: It supports only searching for information from the Internet. For tasks using [web-search], provide the search query, and only the search query to use (eg. not 'research waterproof shoes, but 'waterproof shoes').\n"
+            f"text-completion: it is a text completion tool that can be used for content extraction, summarization, copywrite, translation, etc., and can also be used for LLM-based QA\n"
+            f"Make sure all task IDs are in chronological order.\n"
+            f"For efficiency, let's think step by step and create the tasks (up to 3 tasks) that are most critical to objective.\n"
+            f"An example of the desired output format is:"
+            "[{\"id\": 1, \"task\": \"https://untapped.vc\", \"tool\": \"web-scrape\", \"dependent_task_ids\": [], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 2, \"task\": \"Consider additional insights that can be reasoned from the results of...\", \"tool\": \"text-completion\", \"dependent_task_ids\": [1], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 3, \"task\": \"Untapped Capital\", \"tool\": \"web-search\", \"dependent_task_ids\": [], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}].\n"
+            f"Ensure the response can be parsed by Python json.loads. JSON TASK LIST="
+        )
+
+        messages = create_message(prompt)
+        response = create_chat_completion(
+            model=Config().fast_llm_model,
+            messages=messages,
+        )
+
+        new_tasks = json.loads(response)
+        task_list = []
+        for new_task in new_tasks:
+            task_id_counter += 1
+            new_task.update({"id": task_id_counter})
+            task_list.append(new_task)
+        return task_list
+
+    def orchestrate_task(self, last_task: Dict) -> List[Dict]:
+        original_task_list = self.task_list.copy()
+        minified_task_list = [{k: v for k, v in task.items() if k != "result"} for task in self.task_list]
+        result = last_task['result'][0:4000] #come up with better solution later.
+        
+        prompt = (
+            f"You are a QA AI assistant tasked with cleaning the formatting of and reprioritizing the following tasks delimited by triple backtick:```{minified_task_list}```\n"
+            f"the last completed task (task id = {last_task['id']}, tool = {last_task['tool']}) has the following result delimited by triple backtick: ```{last_task['result']}```\n\n"
+            f"Your task: Consider the ultimate objective of your team is to answer the question {self.objective} and reflect on the result of task that has been complted, re-create the task list (up to 5 tasks) to answer the question.\n" 
+            f"The current tool option is [text-completion, web-search] only. What each tool does is as follows:\n"
+            f"web-search: It supports searching for information on the Internet. For tasks using [web-search], provide the search query, and only the search query to use (eg. not 'research waterproof shoes, but 'waterproof shoes').\n"
+            f"text-completion: IT is a tool that can be used for content extraction, summarization, copywrite, translation, etc., and can also be used for LLM-based QA\n"
+            f"dependent_task_ids should always be an empty array, or an array of numbers representing the task ID it should pull results from."
+            f"Make sure all task IDs are in chronological order.\n"
+            f"Don not remove the completed tasks.\n"
+            f"The last task is always to provide a final answer for customer.\n"
+            f"An example of the desired output format is:"
+            "[{\"id\": 1, \"task\": \"https://untapped.vc\", \"tool\": \"web-scrape\", \"dependent_task_ids\": [], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 2, \"task\": \"Consider additional insights that can be reasoned from the results of...\", \"tool\": \"text-completion\", \"dependent_task_ids\": [1], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 3, \"task\": \"Untapped Capital\", \"tool\": \"web-search\", \"dependent_task_ids\": [], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}].\n"
+            f"Ensure the response can be parsed by Python json.loads. JSON TASK LIST="
+        )
+
+        messages = create_message(prompt)
+        result = create_chat_completion(
+            model=Config().fast_llm_model,
+            messages=messages,
+        )
+
+        try:
+            tmp_task_list = json.loads(result)
+        except Exception as error:
+            print(f"fail to decode ({error}): {result}")
+            return original_task_list
+        # Add the 'result' field back in
+
+        for updated_task, original_task in zip(tmp_task_list, original_task_list):
+            if "result" in original_task:
+                updated_task["result"] = original_task["result"]
+
+        return tmp_task_list
+
+    ### Agent functions ##############################
+    def execute_task(self, task: Dict) -> Dict:
+        # Check if dependent_task_id is completed
+        dependent_task_ids = []
+        dependent_task_prompt = ""
+        if task["dependent_task_ids"]:
+            if isinstance(task["dependent_task_ids"], list):
+                dependent_task_ids = task["dependent_task_ids"]
+            else:
+                dependent_task_ids = [task["dependent_task_ids"]]
+
+            for dependent_task_id in dependent_task_ids:
+                dependent_task = self.get_task_by_id(dependent_task_id)
+                if dependent_task and dependent_task["status"] != "completed":
+                    return
+                elif dependent_task:
+                    dependent_task_prompt += f"\ntask ({dependent_task['id']}. {dependent_task['task']}) result: {dependent_task['result']}"
+
+        # Execute task
+        
+        task_prompt = f"Complete your assigned task based on the objective: {self.objective}. Your task: {task['task']}"
+        if dependent_task_prompt != "":
+            task_prompt += f"\nThe previous tasks: {dependent_task_prompt}"
+
+        task_prompt += "\nResponse:"
+        if task["tool"] == "text-completion":
+            result = llm_uils().text_completion(task_prompt)
+            summary_result_prompt = f"Please summarize the following text:\n{result}\nSummary:"
+            task["result_summary"] = llm_uils().text_completion(summary_result_prompt)
+        elif task["tool"] == "web-search":
+            result = str(web_search(str(task['task'])))
+            summary_result_prompt = f"Please summarize the following text:\n{result}\nSummary:"
+            task["result_summary"] = llm_uils().text_completion(summary_result_prompt)
+        elif task["tool"] == "search-IT-knowledge-base":
+            result = str(self.it_kb.similarity_search(str(task['task'])))
+            summary_result_prompt = f"Please summarize the following text:\n{result}\nSummary:"
+            task["result_summary"] = llm_uils().text_completion(summary_result_prompt)
+        else:
+            result = "Unknown tool"
+        
+        # Update task status and result
+        task["status"] = "completed"
+        task["result"] = result
+        return task
     
-    print("\033[93m\033[1m"+"\n*****TASK RESULT*****\n"+"\033[0m\033[0m")
-    print_result = result[0:2000]
-    if result != result[0:2000]:
-      print(print_result+"...")
-    else:
-      print(result)
-    print("\033[93m\033[1m"+"\n*****TASK RESULT Summary *****\n"+"\033[0m\033[0m")
-    print(task["result_summary"])
-    # Update task status and result
-    task["status"] = "completed"
-    task["result"] = result
-
-    # overview_agent(task)
-
-    # Update task_manager_agent of tasks
-    task_manager_agent(
-        objective,
-        task,
-        result, 
-    )
-
-def execute(objective: str):
-    global task_list
-    task_list = init_task_list(objective)
-    print("\033[95m\033[1m"+"\n*****TASK LIST*****\n"+"\033[0m")
-    for t in task_list:
-            dependent_task = ""
-            if t['dependent_task_id'] is not None:
-                dependent_task = f"\033[31m<dependency: #{t['dependent_task_id']}>\033[0m"
-            status_color = "\033[32m" if t['status'] == "completd" else "\033[31m"
-            print(f"\033[1m{t['id']}\033[0m: {t['task']} {status_color}[{t['status']}]\033[0m \033[93m[{t['tool']}] {dependent_task}\033[0m")
-
-
-    # Continue the loop while there are incomplete tasks
-    while any(task["status"] == "incomplete" for task in task_list):
-
-        # Filter out incomplete tasks
-        incomplete_tasks = [task for task in task_list if task["status"] == "incomplete"]
-
-        if incomplete_tasks:
-            # Sort tasks by ID
-            incomplete_tasks.sort(key=lambda x: x["id"])
-
-            # Pull the first task
-            task = incomplete_tasks[0]
-
-            # Execute task & call task manager from function
-            execute_task(task, objective)
-
-            # Print task list and session summary
-            print("\033[95m\033[1m" + "\n*****TASK LIST*****\n" + "\033[0m")
-            for t in task_list:
-                dependent_task = ""
-                if t['dependent_task_id'] is not None:
-                    dependent_task = f"\033[31m<dependency: #{t['dependent_task_id']}>\033[0m"
-                status_color = "\033[32m" if t['status'] == "completed" else "\033[31m"
-                print(f"\033[1m{t['id']}\033[0m: {t['task']} {status_color}[{t['status']}]\033[0m \033[93m[{t['tool']}] {dependent_task}\033[0m")
-            #print("\033[93m\033[1m" + "\n*****SESSION SUMMARY*****\n" + "\033[0m\033[0m")
-            #print(session_summary)
-
-        time.sleep(1)  # Sleep before checking the task list again
-
-    ### Objective complete ##############################
-
-    # Print the full task list if there are no incomplete tasks
-    if all(task["status"] != "incomplete" for task in task_list):
-        print("\033[92m\033[1m" + "\n*****ALL TASKS COMPLETED*****\n" + "\033[0m\033[0m")
-        for task in task_list:
-            print(f"ID: {task['id']}, Task: {task['task']}, Result: {task['result']}")
+    def execute(self) -> str:
+        self.status = "running"
+        # Main loop
+        while any(task["status"] == "incomplete" for task in self.task_list):
+              # Filter out incomplete tasks
+            incomplete_tasks = [task for task in self.task_list if task["status"] == "incomplete"]
+            logging.info(f"\033[95m\033[1m INCOMPLETE TASK LIST({self.objective}) \033[0m\033[0m {[str(t['id'])+': '+t['task'] + '[' + t['tool'] + ']' for t in incomplete_tasks]}")
+            if incomplete_tasks:
+                # Sort tasks by ID
+                incomplete_tasks.sort(key=lambda x: x["id"])
+
+                # Pull the first task
+                task = incomplete_tasks[0]
+                logging.info(f"\033[92m\033[1m NEXT TASK({self.objective}) \033[0m\033[0m {task['id']}:{task['task']}[{task['tool']}]")
+
+                # Execute task & call task manager from function
+                try:
+                    completed_task = self.execute_task(task)
+                    logging.info(f"\033[93m\033[1m TASK RESULT({self.objective}) \033[0m\033[0m {completed_task['result']}")
+                except Exception as e:  
+                    logging.error(f"An error occurred while executing the task({self.objective}): {e.with_traceback()}")
+                    self.status = "error"
+                    self.error_message = str(e)  
+                    return str(e)
+                if len(self.task_list) - len(incomplete_tasks) + 1 < self.max_tasks_count or len(incomplete_tasks) > 1:
+                    logging.info(f"\033[90m\033[3m" + "\nOrchestrate_task list({self.objective})...\n" + "\033[0m")
+                    self.task_list = self.orchestrate_task(completed_task)
+
+            time.sleep(1)  # Sleep before checking the task list again
+        self.status = "completed"
+
+    def stat(self) -> Dict:
+        return {"task_list": self.task_list, "status": self.status, "error_message": self.error_message}
```

### Comparing `autoxx-0.0.13/autoxx/js/overlay.js` & `autoxx-0.0.15/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.13/autoxx/search/simple_search.py` & `autoxx-0.0.15/autoxx/tools/web_search/search.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,38 @@
 from typing import Dict, List, Optional
 import json
-import os
 from pathlib import Path
 from autogpt.config import Config
-import openai
 
 from autogpt.commands.web_selenium import scrape_text_with_selenium
 from selenium.webdriver.remote.webdriver import WebDriver
 from autogpt.commands.google_search import google_search
 from autogpt import token_counter
 from autogpt.llm_utils import create_chat_completion
 from autogpt.processing.text import split_text
 
-FILE_DIR = Path(__file__).parent.parent
+FILE_DIR = Path(__file__).parent
 CFG = Config()
 
-def setup_autgpt_config(
-        azure_config_file:Optional[str] = "",
-        only_gpt4:bool = False,
-        debug:bool = False,
-) -> Config:
-    CFG = Config()
-    if azure_config_file != "":
-        CFG.set_openai_api_key(os.getenv("AZURE_OPENAI_API_KEY", ""))
-        CFG.use_azure=True
-        CFG.load_azure_config(config_file=azure_config_file)
-
-    if only_gpt4:
-        CFG.set_fast_token_limit(CFG.smart_token_limit)
-        if CFG.use_azure:
-            CFG.set_azure_deployment_id_for_model(CFG.fast_llm_model, CFG.get_azure_deployment_id_for_model(CFG.smart_llm_model))
-        CFG.set_fast_llm_model(CFG.smart_llm_model)
-        CFG.set_browse_chunk_max_length(7000)
-
-    CFG.set_debug_mode(debug)
-
-    openai.api_type = CFG.openai_api_type
-    openai.api_base = CFG.openai_api_base
-    openai.api_version = CFG.openai_api_version
-    openai.api_key = CFG.openai_api_key
-    return CFG
-
 def create_message(chunk: str, question: str) -> Dict[str, str]:
     """Create a message for the chat completion
 
     Args:
         chunk (str): The chunk of text to summarize
         question (str): The question to answer
 
     Returns:
         Dict[str, str]: The message to send to the chat completion
     """
     return {
         "role": "user",
-        "content": f'"""{chunk}""" Using the above text, answer the following'
-        f' question: "{question}" -- if the question cannot be answered using the text,'
-        " summarize the text.",
+        "content": f'"""{chunk}""" Analyze the above text and extract all information in detail relevant to '
+        f'question: "{question}" -- if there is no relevant information, summarize the text in detail.'
     }
+    
 
 def scroll_to_percentage(driver: WebDriver, ratio: float) -> None:
     """Scroll to a percentage of the page
 
     Args:
         driver (WebDriver): The webdriver to use
         ratio (float): The percentage to scroll to
@@ -134,53 +106,51 @@
 
     Returns:
         None
     """
     driver.quit()
 
 
-def browse_website(url: str, question: str) -> List[str]:
+def browse_website(url: str, question: str) -> str:
     """Browse a website and summarize it
 
     Args:
         url (str): The url to browse
         question (str): The question to answer
 
     Returns:
         str: The summary of the website
     """
     driver, text = scrape_text_with_selenium(url=url)
     add_header(driver)
-    summary = summarize_chunks(text=text, question=question, url=url, driver=driver)
+    summaries = summarize_chunks(text=text, question=question, url=url, driver=driver)
     close_browser(driver)
-    return summary
+    return '\n'.join(summaries)
 
-def simple_search(question:str, search_num:Optional[int]=2) -> str:
+def web_search(question:str, search_num:Optional[int]=2) -> List[Dict]:
     search_result = google_search(query=question, num_results=search_num)
     search_search_json = json.loads(search_result)
-    summaries = []
+    search_summaries = []
 
     if isinstance(search_search_json, list):
         for res in search_search_json:
             print(f"{res['title']} x {res['href']}\n")
             summary = browse_website(url=res['href'], question=question)
-            summaries.extend(summary)
+
+            search_summaries.append({
+                "relevant_content": summary,
+                "title": res['title'],
+                "url": res['href']
+            })
+
             print(f"{res['title']} x {res['href']} summary: {summary}\n")
     else:
         print(f"{search_search_json['title']} x {search_search_json['href']}")
         summary = browse_website(url=search_search_json['href'], question=question)
-        summaries.extend(summary)
+        search_summaries.append({
+            "content": summary,
+            "title": res['title'],
+            "url": res['href']
+        })
         print(f"{search_search_json['title']} x {search_search_json['href']} summary: {summary}\n")
 
-    if len(summaries) == 1:
-        return summaries[0]
-
-    if len(summaries) == 1:
-        return summaries[0]
-
-    combined_summary = "\n".join(summaries)
-    messages = [create_message(combined_summary, question)]
-
-    return create_chat_completion(
-        model=CFG.fast_llm_model,
-        messages=messages,
-    )
+    return search_summaries
```

### Comparing `autoxx-0.0.13/pyproject.toml` & `autoxx-0.0.15/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.13"
+version = "0.0.15"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -17,13 +17,14 @@
 python-dotenv = "1.0.0"
 bs4 = "0.0.1"
 webdriver_manager = "3.8.6"
 tiktoken = "0.3.3"
 playsound = "1.2.2"
 gTTS = "2.3.1"
 orjson = "3.8.10"
-duckduckgo-search = "3.0.2"
+duckduckgo-search = "^2.9.3"
 spacy = ">=3.0.0,<4.0.0"
+llama-index = "^0.6.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autoxx-0.0.13/PKG-INFO` & `autoxx-0.0.15/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.13
+Version: 0.0.15
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: agpt (==0.2.2)
 Requires-Dist: auto_gpt_plugin_template (==0.0.3)
 Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: colorama (==0.4.6)
-Requires-Dist: duckduckgo-search (==3.0.2)
+Requires-Dist: duckduckgo-search (>=2.9.3,<3.0.0)
 Requires-Dist: gTTS (==2.3.1)
+Requires-Dist: llama-index (>=0.6.9,<0.7.0)
 Requires-Dist: openai (==0.27.6)
 Requires-Dist: orjson (==3.8.10)
 Requires-Dist: pinecone-client (==2.2.1)
 Requires-Dist: playsound (==1.2.2)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: selenium (==4.9.0)
 Requires-Dist: spacy (>=3.0.0,<4.0.0)
```

