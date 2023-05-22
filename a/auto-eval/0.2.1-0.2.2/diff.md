# Comparing `tmp/auto-eval-0.2.1.tar.gz` & `tmp/auto-eval-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.2.1.tar", last modified: Fri May 19 09:43:59 2023, max compression
+gzip compressed data, was "auto-eval-0.2.2.tar", last modified: Mon May 22 09:20:07 2023, max compression
```

## Comparing `auto-eval-0.2.1.tar` & `auto-eval-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:43:59.835861 auto-eval-0.2.1/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.1/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    13744 2023-05-19 09:43:59.835506 auto-eval-0.2.1/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    13318 2023-05-12 08:18:35.000000 auto-eval-0.2.1/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:43:59.832618 auto-eval-0.2.1/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    13744 2023-05-19 09:43:59.000000 auto-eval-0.2.1/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-05-19 09:43:59.000000 auto-eval-0.2.1/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-19 09:43:59.000000 auto-eval-0.2.1/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-19 09:43:59.000000 auto-eval-0.2.1/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-19 09:43:59.000000 auto-eval-0.2.1/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-19 09:43:59.000000 auto-eval-0.2.1/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:43:59.833115 auto-eval-0.2.1/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.1/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     7953 2023-05-19 09:42:46.000000 auto-eval-0.2.1/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:43:59.833537 auto-eval-0.2.1/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.1/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     5552 2023-05-19 08:57:24.000000 auto-eval-0.2.1/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:43:59.834519 auto-eval-0.2.1/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.1/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3090 2023-05-19 09:15:03.000000 auto-eval-0.2.1/eval/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2083 2023-05-19 09:31:53.000000 auto-eval-0.2.1/eval/prompt_template/prompts.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:43:59.835107 auto-eval-0.2.1/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.1/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3422 2023-05-18 04:08:41.000000 auto-eval-0.2.1/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-19 09:43:59.835922 auto-eval-0.2.1/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-05-19 09:42:28.000000 auto-eval-0.2.1/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.287827 auto-eval-0.2.2/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.2/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    14210 2023-05-22 09:20:07.287564 auto-eval-0.2.2/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    13784 2023-05-22 08:54:26.000000 auto-eval-0.2.2/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.284974 auto-eval-0.2.2/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    14210 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.285426 auto-eval-0.2.2/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.2/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     8295 2023-05-22 09:15:23.000000 auto-eval-0.2.2/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.285852 auto-eval-0.2.2/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.2/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     5552 2023-05-19 08:57:24.000000 auto-eval-0.2.2/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.286709 auto-eval-0.2.2/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.2/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3090 2023-05-19 09:15:03.000000 auto-eval-0.2.2/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2134 2023-05-22 07:59:55.000000 auto-eval-0.2.2/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.287160 auto-eval-0.2.2/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.2/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3422 2023-05-18 04:08:41.000000 auto-eval-0.2.2/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-22 09:20:07.287877 auto-eval-0.2.2/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-05-22 09:17:45.000000 auto-eval-0.2.2/setup.py
```

### Comparing `auto-eval-0.2.1/LICENSE` & `auto-eval-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.1/PKG-INFO` & `auto-eval-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.1
+Version: 0.2.2
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -209,15 +209,15 @@
 If you want to use a custom template, make sure it has slots for "question", "answers", and "target". The first two are required, while "target" is only necessary if your evaluation data has a column named "target".
 ```json
 {
     "eval_with_target_template": "[Question]: {question}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}",
     "eval_without_target_template": "[Question]: {question}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}" 
 }
 ```
-
+`--template_type` string ${\color{grey}\text{Optional}}$  Defaults to null <br> Which template should be used for evaluation. The default template is shown above. Another optional template is specific to the e-commerce domain. To use it, pass `--template_type e_commerce`.
 
 `--verbose` bool ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to print every prompt and response evaluation detail.
 
 `--model` string ${\color{grey}\text{Optional}}$  Defaults to gpt-3.5-turbo or claude-v1.3 depends on `api_type`<br> Which model to perform evaluation, The default model for evaluation is either gpt-3.5-turbo or claude-v1.3, depending on the API type. You can specify which model to use for evaluation by providing its name, such as "gpt-4", "claude-instant-v1", or "claude-v1.3".
 
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 1 will make the output more random, while lower values like 0.1 will make it more focused and deterministic.
 
@@ -235,26 +235,24 @@
 
 `--target` ${\color{grey}\text{Optional}}$ Defaults to \'\'<br> The correct answer for the question. The prompt will be different depending on whether the target is provided, e.g., if no target is provided, the model is asked to solve the question first and then evaluate each candidate answer.
 
 ### Evaluate file arguments
 
 `--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
-
-
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
-
-
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
+`score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
+
 
 ## ToDo
 - [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
 - [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
 - [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.2.1/README.md` & `auto-eval-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 If you want to use a custom template, make sure it has slots for "question", "answers", and "target". The first two are required, while "target" is only necessary if your evaluation data has a column named "target".
 ```json
 {
     "eval_with_target_template": "[Question]: {question}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}",
     "eval_without_target_template": "[Question]: {question}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}" 
 }
 ```
-
+`--template_type` string ${\color{grey}\text{Optional}}$  Defaults to null <br> Which template should be used for evaluation. The default template is shown above. Another optional template is specific to the e-commerce domain. To use it, pass `--template_type e_commerce`.
 
 `--verbose` bool ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to print every prompt and response evaluation detail.
 
 `--model` string ${\color{grey}\text{Optional}}$  Defaults to gpt-3.5-turbo or claude-v1.3 depends on `api_type`<br> Which model to perform evaluation, The default model for evaluation is either gpt-3.5-turbo or claude-v1.3, depending on the API type. You can specify which model to use for evaluation by providing its name, such as "gpt-4", "claude-instant-v1", or "claude-v1.3".
 
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 1 will make the output more random, while lower values like 0.1 will make it more focused and deterministic.
 
@@ -223,26 +223,24 @@
 
 `--target` ${\color{grey}\text{Optional}}$ Defaults to \'\'<br> The correct answer for the question. The prompt will be different depending on whether the target is provided, e.g., if no target is provided, the model is asked to solve the question first and then evaluate each candidate answer.
 
 ### Evaluate file arguments
 
 `--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
-
-
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
-
-
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
+`score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
+
 
 ## ToDo
 - [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
 - [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
 - [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.2.1/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.2.2/auto_eval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.1
+Version: 0.2.2
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -209,15 +209,15 @@
 If you want to use a custom template, make sure it has slots for "question", "answers", and "target". The first two are required, while "target" is only necessary if your evaluation data has a column named "target".
 ```json
 {
     "eval_with_target_template": "[Question]: {question}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}",
     "eval_without_target_template": "[Question]: {question}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}" 
 }
 ```
-
+`--template_type` string ${\color{grey}\text{Optional}}$  Defaults to null <br> Which template should be used for evaluation. The default template is shown above. Another optional template is specific to the e-commerce domain. To use it, pass `--template_type e_commerce`.
 
 `--verbose` bool ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to print every prompt and response evaluation detail.
 
 `--model` string ${\color{grey}\text{Optional}}$  Defaults to gpt-3.5-turbo or claude-v1.3 depends on `api_type`<br> Which model to perform evaluation, The default model for evaluation is either gpt-3.5-turbo or claude-v1.3, depending on the API type. You can specify which model to use for evaluation by providing its name, such as "gpt-4", "claude-instant-v1", or "claude-v1.3".
 
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 1 will make the output more random, while lower values like 0.1 will make it more focused and deterministic.
 
@@ -235,26 +235,24 @@
 
 `--target` ${\color{grey}\text{Optional}}$ Defaults to \'\'<br> The correct answer for the question. The prompt will be different depending on whether the target is provided, e.g., if no target is provided, the model is asked to solve the question first and then evaluate each candidate answer.
 
 ### Evaluate file arguments
 
 `--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
-
-
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
-
-
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
+`score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
+
 
 ## ToDo
 - [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
 - [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
 - [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.2.1/eval/auto_llms_eval.py` & `auto-eval-0.2.2/eval/auto_llms_eval.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,18 +44,15 @@
     api_tool: OneAPITool,
     eval_prompter: Prompter,
     data_group: pd.DataFrame,
     engine: str,
     temperature=0.1,
     max_new_tokens=2048,
 ) -> Union[pd.DataFrame, None]:
-    group = data_group.reset_index()
-    if 'score' in group.keys() and group['score'].map(lambda x: x if x != '' and x == x else None).count() == len(group):
-        group['score'] = group['score'].map(float)
-        return group
+    group = data_group.reset_index(drop=True)
     question = group['question'].unique()[0]
     candidate_answers = group['output']
     if 'target' in data_group.keys():
         target = group['target'].unique()[0]
     else:
         target = ''
     scores, raw_response = eval_one_qa(api_tool=api_tool,
@@ -72,15 +69,15 @@
             group.at[i, 'score'] = scores[i]
         return group
     else:
         return None
 
 
 
-def prepare_eval_data(eval_data_path: List[str], eval_categories: Optional[List[str]] = None, sample_num: int=0, eval_models: Optional[List[str]] = None) -> List[pd.DataFrame]:
+def prepare_eval_data(eval_data_path: List[str], eval_categories: Optional[List[str]] = None, sample_num: int=0, eval_models: Optional[List[str]] = None) -> Tuple[List[pd.DataFrame],List[pd.DataFrame] ]:
     eval_data = df_reader(eval_data_path[0]) if len(eval_data_path) == 1 else pd.concat([df_reader(file_path) for file_path in eval_data_path])
     eval_data = eval_data.fillna('')
     if len({'instruction', 'input', 'output'} - set(eval_data.keys())) == 0:
         eval_data['question'] = eval_data['instruction'].str.cat(
             eval_data['input'], sep=' ')
     elif len({'prompt', 'output'} - set(eval_data.keys())) == 0:
         eval_data['quesion'] = eval_data['prompt'].copy()
@@ -100,15 +97,25 @@
             eval_models) > 0 and 'model' in eval_data.keys():
         eval_data = eval_data[eval_data['model'].isin(eval_models)]
     grouped = eval_data.groupby(by=['question'])
     if sample_num > 0:
         sample_keys = random.sample(grouped.groups.keys(), sample_num)
     else:
         sample_keys = grouped.groups.keys()
-    return [grouped.get_group(key) for key in sample_keys]
+    total_groups =  [grouped.get_group(key) for key in sample_keys]
+    scored_groups = []
+    unscored_groups = []
+    for group in total_groups:
+        if 'score' in group.keys() and group['score'].map(lambda x: x if x != '' and x == x else None).count() == len(group):
+            group['score'] = group['score'].map(float)
+            scored_groups.append(group)
+        else:
+            unscored_groups.append(group)
+    return scored_groups, unscored_groups
+     
 
 def log_score_results(eval_results_df: pd.DataFrame, score_by: List[str]):
     if 'model' in eval_results_df.keys():
         score_models = eval_results_df.groupby('model')['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}')
         print(f'{"-"*20} Scores by \'model\' {"-"*20}\n{score_models.to_markdown()}')
         if 'category' in eval_results_df.keys():
             score_category = eval_results_df.groupby([
@@ -123,17 +130,17 @@
             f'\n{"-"*20} Scores by {score_by} {"-"*20}\n{scores.to_markdown(index=False)}'
         )
         
 def evaluation_prompt_acc(eval_result_df: pd.DataFrame):
     if 'targe_score' in eval_result_df.keys():
         pass
 
-def save_results(eval_results_df: pd.DataFrame, output_path: str):
+def save_results(results_df: pd.DataFrame, output_path: str):
     print(f'Saving evaluation results: {output_path}')
-    df_saver(eval_results_df, output_path)
+    df_saver(results_df, output_path)
     print(f'Saved successfully.')
 
 @dataclass
 class EvalConfig:
     api_config_file: str
     eval_prompter: Prompter
     eval_data_path: str
@@ -148,41 +155,40 @@
     temperature: float = 0.1
     max_new_tokens: int = 2048
 
 def eval_groups(
     eval_config: EvalConfig
 ):
     # Preparing data
-    eval_groups = prepare_eval_data(eval_config.eval_data_path, eval_config.eval_categories, eval_config.sample_num, eval_config.eval_models)
+    scored_groups, unscored_groups = prepare_eval_data(eval_config.eval_data_path, eval_config.eval_categories, eval_config.sample_num, eval_config.eval_models)
 
     # Init api tool and prompter
     tool = OneAPITool.from_config_file(config_file=eval_config.api_config_file)
 
-    eval_results = []
-    failed_results = []
-    for group in tqdm(eval_groups):
+    failed_groups = []
+    for group in tqdm(unscored_groups):
         result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
         if result is not None:
-            eval_results.append(result)
+            scored_groups.append(result)
         else:
-            failed_results.append(group)
+            failed_groups.append(group)
         time.sleep(eval_config.request_interval)
 
     # Retry failed requests
-    if len(failed_results) > 0 and eval_config.retry:
-        for group in tqdm(failed_results.copy(), desc='RETRY'):
+    if len(failed_groups) > 0 and eval_config.retry:
+        for group in tqdm(failed_groups.copy(), desc='RETRY'):
             result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
             if result is not None:
-                eval_results.append(result)
-                failed_results = [df for df in failed_results if not df.equals(group)]
+                scored_groups.append(result)
+                failed_groups = [df for df in failed_groups if not df.equals(group)]
             time.sleep(eval_config.request_interval)
 
-    eval_results.extend(failed_results)
-    eval_results_df = pd.concat(eval_results)
-    log_score_results(eval_results_df=eval_results_df, score_by=eval_config.score_by)
+    scored_results_df = pd.concat(scored_groups)
+    log_score_results(eval_results_df=scored_results_df, score_by=eval_config.score_by)
     # Log score results
     print(f'Eval engine: {eval_config.engine}')
     print(f'Eval files: {eval_config.eval_data_path}')
-    print(f'Failed requests: {len(failed_results)}/{len(eval_groups)}')
+    print(f'Failed requests: {len(failed_groups)}/{len(scored_groups) + len(failed_groups)}')
+    results_df = pd.concat([scored_results_df, pd.concat(failed_groups)]) if len(failed_groups) > 0 else scored_results_df
     # Save results
     if eval_config.output_path:
-        save_results(eval_results_df=eval_results_df, output_path=eval_config.output_path)
+        save_results(results_df=results_df, output_path=eval_config.output_path)
```

### Comparing `auto-eval-0.2.1/eval/commands/auto_eval.py` & `auto-eval-0.2.2/eval/commands/auto_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.1/eval/prompt_template/prompter.py` & `auto-eval-0.2.2/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.1/eval/prompt_template/prompts.py` & `auto-eval-0.2.2/eval/prompt_template/prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 EVAL_WITH_TARGET_TEMPLATE = """
 [Question]: {question}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{answers}\n\n[System]:\n
 Please evaluate and comment each [Candidate answer] based on the [Correct answer].
 Then output all [Candidate answer] scores (0-1) in a summary format of
 {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}.
 """
 
-
 EVAL_WITHOUT_TARGET_TEMPLATE = """
 [Question]: {question}\n\n[Candidate answer]:\n{answers}\n\n[System]:\n
-Please solve the [Question] independently to obtain the [Correct answer],
+Please solve the [Question] independently without referring to candidate answers to obtain the [Correct answer],
 and then evaluate and comment each [Candidate answer] based on the [Correct answer].
 Finally, output all [Candidate answers] scores (0-1) in a summary format of
 {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}.
 """
 
 EVAL_WITH_TARGET_TEMPLATE_ECOMMERCE = """
 The following text contains a question from the customer along with some context. A reference answer is also provided for comparison purposes.\n
-Question:
+\nQuestion:
 \n```text\n\n{question}\n\n```\n
-Referece answer:
-\n```text\n\n{target}\n\n```\n
-Please evaluate and comment on each candidate answer based on its accurately and professionalism, 
+\nReferece answer:
+\n```text\n\n{target}\n\n```
+\nPlease evaluate and comment on each candidate answer based on its accurately and professionalism, 
 and ability to provide necessary information without being too verbose.
-Candidate answers:
+\nCandidate answers:
 \n```text\n\n{answers}\n\n```\n
-Finally output all answers' scores (0-1) in a summary format of {{\"number\": \"score\"}}"""
+\nFinally output all answers' scores (0-1) in a summary format of {{\"number\": \"score\"}}"""
 
 EVAL_WITHOUT_TARGET_TEMPLATE_ECOMMERCE = """
 The following text contains a question from the customer along with some context.
-Question:
-\n```text\n\n{question}\n\n```\n
-Please first answer the question independently without referring to candidate answers to obtain the correct answer, 
+\nQuestion:
+\n```text\n\n{question}\n\n```
+\nPlease first answer the question independently without referring to candidate answers to obtain the correct answer, 
 and then evaluate and comment each answer based on its accurately and professionalism, 
 and ability to provide necessary information without being too verbose.
-Candidate answers:
+\nCandidate answers:
 \n```text\n\n{answers}\n\n```\n
+
 Finally output all answers' scores (0-1) in a summary format of {{\"number\": \"score\"}}"""
```

### Comparing `auto-eval-0.2.1/eval/utils/data_utils.py` & `auto-eval-0.2.2/eval/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.1/setup.py` & `auto-eval-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.2.1",
+    version="0.2.2",
     packages=find_packages(),
     # package_data={
     #   "eval":["prompt_template/eval_prompt_template.json"]  
     # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

