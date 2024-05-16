# Comparing `tmp/ragtime-0.0.32.tar.gz` & `tmp/ragtime-0.0.33.tar.gz`

## Comparing `ragtime-0.0.32.tar` & `ragtime-0.0.33.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 ragtime-0.0.32/CHANGELOG.md
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 ragtime-0.0.32/CONTRIBUTING.md
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.32/deploy/deploy.py
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.32/img/Ragtime_logo.png
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/api.py
--rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/config.py
--rw-r--r--   0        0        0    20377 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/expe.py
--rw-r--r--   0        0        0    40177 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/generators.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/README.md
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/classes.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/main.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/html_templates/basic_template.jinja
--rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
--rw-r--r--   0        0        0    27626 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
--rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx
--rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 ragtime-0.0.32/tests/full_test.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.32/tests/run_tests.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.32/tests/test_quest.json
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ragtime-0.0.32/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.32/LICENSE
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ragtime-0.0.32/README.md
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 ragtime-0.0.32/pyproject.toml
--rw-r--r--   0        0        0     7473 2020-02-02 00:00:00.000000 ragtime-0.0.32/PKG-INFO
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 ragtime-0.0.33/CHANGELOG.md
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 ragtime-0.0.33/CONTRIBUTING.md
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.33/deploy/deploy.py
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.33/img/Ragtime_logo.png
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/api.py
+-rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/config.py
+-rw-r--r--   0        0        0    21163 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/expe.py
+-rw-r--r--   0        0        0    42943 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/generators.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/README.md
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/classes.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/main.py
+-rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/res/html_templates/basic_template.jinja
+-rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
+-rw-r--r--   0        0        0    21761 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx
+-rw-r--r--   0        0        0    33574 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx
+-rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx
+-rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx
+-rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 ragtime-0.0.33/tests/full_test.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.33/tests/run_tests.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.33/tests/test_quest.json
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ragtime-0.0.33/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.33/LICENSE
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ragtime-0.0.33/README.md
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 ragtime-0.0.33/pyproject.toml
+-rw-r--r--   0        0        0     7473 2020-02-02 00:00:00.000000 ragtime-0.0.33/PKG-INFO
```

### Comparing `ragtime-0.0.32/CONTRIBUTING.md` & `ragtime-0.0.33/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/img/Ragtime_logo.png` & `ragtime-0.0.33/img/Ragtime_logo.png`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/__init__.py` & `ragtime-0.0.33/src/ragtime/__init__.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/api.py` & `ragtime-0.0.33/src/ragtime/api.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/config.py` & `ragtime-0.0.33/src/ragtime/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 DEFAULT_QUESTION_COL:int = DEFAULT_QUESTION_COL if "DEFAULT_QUESTION_COL" in globals() else None
 DEFAULT_FACTS_COL:int = DEFAULT_FACTS_COL if "DEFAULT_FACTS_COL" in globals() else None
 DEFAULT_ANSWERS_COL:int = DEFAULT_ANSWERS_COL if "DEFAULT_ANSWERS_COL" in globals() else None
 DEFAULT_HUMAN_EVAL_COL:int = DEFAULT_HUMAN_EVAL_COL if "DEFAULT_HUMAN_EVAL_COL" in globals() else None
 # # # LLMs
 DEFAULT_LITELLM_RETRIES:int = DEFAULT_LITELLM_RETRIES if "DEFAULT_LITELLM_RETRIES" in globals() else None
 DEFAULT_LITELLM_TEMP:int = DEFAULT_LITELLM_TEMP if "DEFAULT_LITELLM_TEMP" in globals() else None
+DEFAULT_MAX_TOKENS:int = DEFAULT_MAX_TOKENS if "DEFAULT_MAX_TOKENS" in globals() else None
 
 # Logging - class to add msg
 class RagtimeLogger(logging.LoggerAdapter):
     prefix:str = ""
     def process(self, msg, kwargs):
         return f'{self.prefix + " " if self.prefix else ""}{msg}', kwargs
 
@@ -55,15 +56,15 @@
     global ROOT_FOLDER, FOLDER_EXPE, FOLDER_QUESTIONS, FOLDER_ANSWERS, FOLDER_FACTS, FOLDER_EVALS, FOLDER_TEMPLATES, FOLDER_SST_TEMPLATES, FOLDER_HTML_TEMPLATES
     # # # HTML
     global DEFAULT_HTML_RENDERING, DEFAULT_HTML_TEMPLATE
     # # # Spreadheet
     global DEFAULT_SPREADSHEET_TEMPLATE, DEFAULT_WORKSHEET, DEFAULT_HEADER_SIZE, DEFAULT_QUESTION_COL, DEFAULT_FACTS_COL
     global DEFAULT_ANSWERS_COL, DEFAULT_HUMAN_EVAL_COL
     # # # LLMs
-    global DEFAULT_LITELLM_RETRIES, DEFAULT_LITELLM_TEMP
+    global DEFAULT_LITELLM_RETRIES, DEFAULT_LITELLM_TEMP, DEFAULT_MAX_TOKENS
     # Logger
     global logger
     
     # Folders
     ROOT_FOLDER = root_folder
     FOLDER_EXPE = root_folder / 'expe'
     FOLDER_QUESTIONS = FOLDER_EXPE / QUESTIONS_FOLDER_NAME
@@ -83,14 +84,15 @@
     DEFAULT_QUESTION_COL = 2
     DEFAULT_FACTS_COL = 4
     DEFAULT_ANSWERS_COL = 11
     DEFAULT_HUMAN_EVAL_COL = 24
     # # # LLMs
     DEFAULT_LITELLM_RETRIES = 3
     DEFAULT_LITELLM_TEMP = 0
+    DEFAULT_MAX_TOKENS = 1000 # empirically noticed the biggest answers are 4000 characters long - and 1 token is between 4 and 5 chars - keep the largest value, i.e. 4 chars per token
 
     ####################
     # LOGGING
     # You can choose the file where the logs are written in "log_conf" dict, key "handlers"/"file"/"filename" - default is "logs/logs.txt"
     # You can otherwise change everything you need as detailed in https://docs.python.org/3/library/logging.config.html
 
     log_conf:dict = {
```

### Comparing `ragtime-0.0.32/src/ragtime/expe.py` & `ragtime-0.0.33/src/ragtime/expe.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,35 +208,32 @@
         
         # If path exists and overwrite not allowed, raise an Exception
         if result_path.is_file() and not b_overwrite: 
             raise FileExistsError(f'"{path}" already exists! Set b_overwrite=True to allow overwriting.')
 
         return result_path
 
-    def save_temp(self, name:str = "TEMP_"):
-        '''Save the expe as is as a temporary backup. Useful to save the work already done
-        when an Exception occurs or if you want to create intermediate backups while computing.'''
-        if self.json_path:
-            file_name:str = f'{name}{self.json_path.stem}'
-            file_path:str = self.json_path.parent
-        else:
-            file_name:str = f'{name}.json'
-            file_path:str = ''
-        self.save_to_json(path=Path(file_path) / Path(file_name), b_overwrite=True, b_add_suffix=True)
-
     def load_from_json(self, path:Path):
         with open(path, mode="r", encoding="utf-8") as file:
             data:list = json.load(file)
             qa_list:dict = data
             if 'meta' in data:
                 self.meta = data['meta']
                 qa_list = data['items']
             for json_qa in qa_list:
                 qa:QA = QA(**json_qa)
                 self.append(qa)
+    
+    # TODO: Cannot implement this function due to circular imports issue (need objects from generators.py objects and generators.py needs
+    # expe.py objects too) - if someone finds a way, that would be nice since it would allow to easily chain Answer, Facts and Eval generation
+    # def gen_Eval(self, folder_out:Path, prompter:Prompter, llm_names:list[str],
+    #             start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0):
+    #     eval_gen:EvalGenerator = EvalGenerator(llm_names=llm_names, prompter=prompter)
+    #     eval_gen.generate(self, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
+    #     self.save_to_json(path=folder_out / self.json_file)
    
     def update_from_spreadsheet(self, path:Path, update_type:UpdateTypes, data_col:int=None, 
                                 question_col:int = DEFAULT_QUESTION_COL-1, answer_col:int = DEFAULT_ANSWERS_COL-1,
                                 sheet_name:str = DEFAULT_WORKSHEET, header_size:int=DEFAULT_HEADER_SIZE):
         """Updates data from a spreadsheet, e.g. human evaluation or facts
         Args:
         - data_col (int): indicates the column number (starts at 0) from where the data will be imported in the spreadsheet
@@ -286,16 +283,26 @@
                         if cur_ans: # corresponding Answer has been found
                             try:
                                 human_eval:int = int(data_in_ws)
                                 cur_ans.eval.human = human_eval
                             except (TypeError, ValueError):
                                 logger.warn(f'Human eval should be a value between 0 and 1 - cannot use "{data_in_ws}" as found in line {i}')
                         else:
-                            logger.warn(f'Cannot find Answer corresponding with the human eval "{data_in_ws}" - Answer should contain the text "{answer_text}"')
-                        
+                            logger.warn(f'Cannot find Answer corresponding with the human eval "{data_in_ws}" - Answer should contain the text "{answer_text}"')                
+
+    def save_temp(self, name:str = "TEMP_"):
+        '''Save the expe as is as a temporary backup. Useful to save the work already done
+        when an Exception occurs or if you want to create intermediate backups while computing.'''
+        if self.json_path:
+            file_name:str = f'{name}{self.json_path.stem}'
+            file_path:str = self.json_path.parent
+        else:
+            file_name:str = f'{name}.json'
+            file_path:str = ''
+        self.save_to_json(path=Path(file_path) / Path(file_name), b_overwrite=True, b_add_suffix=True)
 
     def save_to_json(self, path:Path=None, b_overwrite:bool=False, b_add_suffix:bool = True) -> Path:
         """Saves Expe to JSON - can generate a suffix for the filename
         Returns the Path of the file actually saved"""
         path:Path = self._file_check_before_writing(path, b_overwrite=b_overwrite, 
                                                     b_add_suffix=b_add_suffix, force_ext='.json')
         with open(path, mode='w', encoding='utf-8') as file:
```

### Comparing `ragtime-0.0.32/src/ragtime/generators.py` & `ragtime-0.0.33/src/ragtime/generators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 from pathlib import Path
-import time
 from langdetect import detect
 import json
 from unidecode import unidecode
 from enum import IntEnum
 from typing import Optional, Union
 from ragtime.expe import Answer, Answers, Chunks, Eval, Expe, Fact, Facts, LLMAnswer, Question, RagtimeBase, QA, Prompt, WithLLMAnswer
 from litellm import completion_cost, acompletion
 from litellm.exceptions import RateLimitError
-from ragtime.config import RagtimeException, logger, div0
+from ragtime.config import DEFAULT_HTML_TEMPLATE, DEFAULT_SPREADSHEET_TEMPLATE, RagtimeException, logger, div0, DEFAULT_MAX_TOKENS
 import re
 import asyncio
 
 import litellm
 litellm.telemetry = False
 
 #################################
@@ -50,28 +49,28 @@
     def get_prompt(self) -> Prompt:
         raise NotImplementedError('Must implement this!')
 
     @abstractmethod
     def post_process(self, qa:QA, cur_obj:WithLLMAnswer) -> WithLLMAnswer:
         raise NotImplementedError('Must implement this!')
 
-class PptrBaseAns(Prompter):
+class PptrAnsBase(Prompter):
     """This simple prompter just send the question as is to the LLM
     and does not perform any post-processing"""
     def get_prompt(self, question:Question, chunks:Optional[Chunks] = None) -> Prompt:
         result:Prompt = Prompt()
         result.user = f'{question.text}'
         result.system = ""
         return result
     
     def post_process(self, qa:QA=None, cur_obj:Answer=None):
         """Does not do anything by default, but can be overridden to add fields in meta data for instance"""
         cur_obj.text = cur_obj.llm_answer.text
 
-class PptrRAGAnsFR(Prompter):
+class PptrAnsWithRetrieverFR(Prompter):
     """This prompter uses a prompt asking the LLM to generate a JSON structure
     and includes chunks in its prompt. It performs post-processing to exploit
     the JSON structure the LLM is supposed to generate."""
     FLD_QUEST_OK:str = "q_ok"
     FLD_CHUNKS_OK:str = "chunks_ok"
     FLD_ANSWER:str = "answer" 
 
@@ -191,29 +190,29 @@
         cur_obj.meta['docs_in_ans'] = [orig_name for (orig_name, fmt_name) 
                                     in docs_in_chunks.items() 
                                     if fmt_name in ans_formatted]
         cur_obj.meta['docs_and_page_in_ans'] = [orig_name for (orig_name, fmt_name) 
                                         in docs_page_in_chunks.items() 
                                         if fmt_name in ans_formatted]
 
-class PptrSimpleFactsFR(Prompter):
-    """Simple Prompter to generate Facts.
-    Asks for 1 to 5 facts in French"""
-    def get_prompt(self, answer:Answer) -> Prompt:
-        result:Prompt = Prompt()
-        result.user = f'{answer.llm_answer.text}'
-        result.system = "Extrait entre 3 et 5 faits décrivant le paragraphe fourni."
-        return result
+# class PptrSimpleFactsFR(Prompter):
+#     """Simple Prompter to generate Facts.
+#     Asks for 1 to 5 facts in French"""
+#     def get_prompt(self, answer:Answer) -> Prompt:
+#         result:Prompt = Prompt()
+#         result.user = f'{answer.llm_answer.text}'
+#         result.system = "Extrait entre 3 et 5 faits décrivant le paragraphe fourni."
+#         return result
     
-    def post_process(self, qa:QA, cur_obj:Facts):
-        """Processes the answer returned by the LLM to return a list of Fact
-        Can be overriden to fit specific prompts"""
-        cur_obj.items = [Fact(text=t.strip()) for t in cur_obj.llm_answer.text.split('\n') if t.strip()]
+#     def post_process(self, qa:QA, cur_obj:Facts):
+#         """Processes the answer returned by the LLM to return a list of Fact
+#         Can be overriden to fit specific prompts"""
+#         cur_obj.items = [Fact(text=t.strip()) for t in cur_obj.llm_answer.text.split('\n') if t.strip()]
 
-class PptrFactsFRv2(Prompter):
+class PptrFactsFR(Prompter):
     """New version of Facts Prompters 
     Asks for 1 to 5 facts in French"""
     def get_prompt(self, answer:Answer) -> Prompt:
         result:Prompt = Prompt()
         result.user = f'{answer.text}'
         result.system = """Génère un minimum de phrases numérotées courtes et simples qui décrivent ce paragraphe.
         Chaque phrase doit être indépendante et aucune phrase ne doit contenir la même information qu'une autre phrase.
@@ -224,21 +223,21 @@
     def post_process(self, qa:QA, cur_obj:Facts):
         """Processes the answer returned by the LLM to return a list of Fact
         Can be overriden to fit specific prompts"""
         temp_list:list[str] = [t.strip() for t in cur_obj.llm_answer.text.split('\n') if t.strip()]
         temp_list = [Fact(text=f'{i}. {t}' if t[1] != '.' and t[2] != '.' else t) for i, t in enumerate(temp_list, start=1) if len(t)>2]
         cur_obj.items = temp_list
 
-class PptrEvalFRv2(Prompter):
+class PptrEvalFR(Prompter):
     """
     Prompt: FAITS and REPONSE - expect the REPONSE to be rewritten including the FACTS in the text
-    Post_process: analyse cited factsfacts not cited, and facts invented (?)"""
+    Post_process: analyse cited facts, facts not cited, and facts invented (?)"""
     def get_prompt(self, answer:Answer, facts:Facts) -> Prompt:
         result:Prompt = Prompt()
-        facts_as_str:str = '\n'.join(f'{i}. {fact.text}' for i, fact in enumerate(facts, start=1))
+        facts_as_str:str = '\n'.join(f'{fact.text}' for fact in facts)
         result.user = f'-- FAITS --\n{facts_as_str}\n\n-- REPONSE --\n{answer.text}'
         result.system = """Tu dois comparer une liste numérotée de FAITS avec une REPONSE.
         Tu dois reprendre exactement la REPONSE en insérant dans le texte le numéro du FAIT auquel correspond exactement le passage ou la phrase.
         Si la phrase correspond à plusieurs FAITS, indique les entre parenthèses.
         Il ne faut pas insérer le FAIT s'il est en contradiction avec le passage ou la phrase.
         Si un passage ou une phrase dans la REPONSE ne correspond à aucun FAIT il faut mettre un point d'interrogation entre parenthèses (?) 
         sauf si ce passage fait référence à un emplacement dans le document, auquel cas il ne faut rien indiquer."""
@@ -257,83 +256,83 @@
         nb_false_facts_in_answer:int = len(re.findall("\(\?\)", answer))
         # compute metrics
         precision:float = div0(len(true_facts_in_answer), len(facts_in_answer)+nb_false_facts_in_answer)
         recall:float = div0(len(true_facts_in_answer), len(true_facts))
         cur_obj.meta["precision"] = precision
         cur_obj.meta["recall"] = recall
         cur_obj.meta["hallus"] = nb_false_facts_in_answer
-        cur_obj.meta["missing"] = ', '.join(list(true_facts_not_in_answer))
+        cur_obj.meta["missing"] = ', '.join(map(str, true_facts_not_in_answer))
         cur_obj.meta["nb_missing"] = len(cur_obj.meta["missing"])
         cur_obj.meta["facts_in_ans"] = str(sorted(facts_in_answer))
         cur_obj.auto = div0(2*precision*recall, precision+recall)
         cur_obj.text = answer
 
-class PptrSimpleEvalFR(Prompter):
-    def get_prompt(self, answer:Answer, facts:Facts) -> Prompt:
-        result:Prompt = Prompt()
-        temp:str = '\n'.join(f'{i}. {fact.text}' for i, fact in enumerate(facts, start=1))
-        result.user = f'Réponse: {answer.text}\n\n{temp}'
-        result.system = """Tu dois dire pour chaque fait numérotés 1, 2, 3...s'il est présent dans la Réponse.
-        Si le fait 1 est présent dans la réponse, renvoie 1. Si le fait 2 est présent dans la réponse, renvoie 2 etc...
-        Si le fait est vrai mais qu'il n'est pas présent dans la réponse, tu ne dois pas le renvoyer."""
-        return result
-
-    def post_process(self, qa:QA, cur_obj:Eval):
-        """Processes the answer returned by the LLM to return an Eval
-        Update the previously existing eval associated with the answer, if any - if None, creates a new Eval object
-        This is used to save the human eval previously entered, if any
-        Can be overriden to fit specific prompts
-        By default, the LLM is supposed to return a list of validated facts"""
-        text:str = cur_obj.llm_answer.text if cur_obj.llm_answer.text != "[]" else ""
-        validated_facts:list[str] = [f.strip() for f in text.split(',') if f.strip()]
-        not_validated_facts:list[str] = [str(i) for i, f in enumerate(qa.facts, start=1) if str(i) not in validated_facts]
-        cur_obj.text = f'Validated: {validated_facts} - Not validated: {not_validated_facts}'
-        cur_obj.auto = len(validated_facts) / len(qa.facts)
-
-class PptrTwoFactsEvalFR(Prompter):
-    def get_prompt(self, answer_facts:Facts, gold_facts:Facts) -> Prompt:
-        """Compares the facts extracted from the answer to evaluate (answer_facts) with the
-        ground truth facts (gold_facts) to evaluate the answer"""
-        result:Prompt = Prompt()
-        gold_list:str = '\n'.join(f'{chr(i + 65)}. {fact.text[3:] if fact.text[1]=="." else fact.text}' for i, fact in enumerate(gold_facts))
-        answer_list:str = '\n'.join(f'{i + 1}. {fact.text[3:] if fact.text[1]=="." else fact.text}'
-                                    for i, fact in enumerate(answer_facts) if len(fact.text.strip()) > 3)
-        result.user = f'Liste 1:\n{gold_list}\n\nListe 2:\n{answer_list}'
-        result.system = """Compare deux listes de faits (Liste 1 et Liste 2) et renvoie les faits identiques dans les deux listes.
-        Les faits de la première liste sont précédés par des lettres, les faits de la seconde liste sont précédés par des chiffres.
-        Assemble les lettres et les chiffres pour les faits identiques.
-        Ne renvoie que des couples Lettres+Chiffres.
-        Ne répète pas les phrases des listes.
-        Si aucun fait n'est identique dans les deux listes, ne renvoie rien.
-        
-        Par exemple si les deux listes suivantes sont fournies, le résultat attendu est A2, B1
-        
-        Liste 1 :
-        A. Les chats sont plus petits que les chiens
-        B. Les chats mangent les souris
-        C. Les chats vivent au plus 30 ans
-        
-        Liste 2 :
-        1. Les souris sont mangées par les chats
-        2. Les chiens sont la plupart du temps plus grand en taille que les chats
-        3. Les chats et les chiens se disputent souvent"""
-        return result
-
-    def post_process(self, qa:QA, cur_obj:Eval):
-        """Processes the answer returned by the LLM to return an Eval
-        Assumes a list like A3, B1"""
-        text:str = cur_obj.llm_answer.text if cur_obj.llm_answer.text != "[]" else ""
-        text_list:list = [t.strip() for t in text.split(',')]
-        num_true_facts:int = len(qa.facts)
-        num_returned_facts:int = len(cur_obj.meta["answer_facts"])
-        num_true_returned:int = len(set(t[1] for t in text_list))
-        cur_obj.meta["precision"] = float(num_true_returned / num_returned_facts)
-        cur_obj.meta["recall"] = float(num_true_returned / num_true_facts)
-        cur_obj.auto = float(2*cur_obj.meta["precision"]*cur_obj.meta["recall"] / (cur_obj.meta["precision"]+cur_obj.meta["recall"]))
-        cur_obj.text = text
+# class PptrSimpleEvalFR(Prompter):
+#     def get_prompt(self, answer:Answer, facts:Facts) -> Prompt:
+#         result:Prompt = Prompt()
+#         temp:str = '\n'.join(f'{i}. {fact.text}' for i, fact in enumerate(facts, start=1))
+#         result.user = f'Réponse: {answer.text}\n\n{temp}'
+#         result.system = """Tu dois dire pour chaque fait numérotés 1, 2, 3...s'il est présent dans la Réponse.
+#         Si le fait 1 est présent dans la réponse, renvoie 1. Si le fait 2 est présent dans la réponse, renvoie 2 etc...
+#         Si le fait est vrai mais qu'il n'est pas présent dans la réponse, tu ne dois pas le renvoyer."""
+#         return result
+
+#     def post_process(self, qa:QA, cur_obj:Eval):
+#         """Processes the answer returned by the LLM to return an Eval
+#         Update the previously existing eval associated with the answer, if any - if None, creates a new Eval object
+#         This is used to save the human eval previously entered, if any
+#         Can be overriden to fit specific prompts
+#         By default, the LLM is supposed to return a list of validated facts"""
+#         text:str = cur_obj.llm_answer.text if cur_obj.llm_answer.text != "[]" else ""
+#         validated_facts:list[str] = [f.strip() for f in text.split(',') if f.strip()]
+#         not_validated_facts:list[str] = [str(i) for i, f in enumerate(qa.facts, start=1) if str(i) not in validated_facts]
+#         cur_obj.text = f'Validated: {validated_facts} - Not validated: {not_validated_facts}'
+#         cur_obj.auto = len(validated_facts) / len(qa.facts)
+
+# class PptrTwoFactsEvalFR(Prompter):
+#     def get_prompt(self, answer_facts:Facts, gold_facts:Facts) -> Prompt:
+#         """Compares the facts extracted from the answer to evaluate (answer_facts) with the
+#         ground truth facts (gold_facts) to evaluate the answer"""
+#         result:Prompt = Prompt()
+#         gold_list:str = '\n'.join(f'{chr(i + 65)}. {fact.text[3:] if fact.text[1]=="." else fact.text}' for i, fact in enumerate(gold_facts))
+#         answer_list:str = '\n'.join(f'{i + 1}. {fact.text[3:] if fact.text[1]=="." else fact.text}'
+#                                     for i, fact in enumerate(answer_facts) if len(fact.text.strip()) > 3)
+#         result.user = f'Liste 1:\n{gold_list}\n\nListe 2:\n{answer_list}'
+#         result.system = """Compare deux listes de faits (Liste 1 et Liste 2) et renvoie les faits identiques dans les deux listes.
+#         Les faits de la première liste sont précédés par des lettres, les faits de la seconde liste sont précédés par des chiffres.
+#         Assemble les lettres et les chiffres pour les faits identiques.
+#         Ne renvoie que des couples Lettres+Chiffres.
+#         Ne répète pas les phrases des listes.
+#         Si aucun fait n'est identique dans les deux listes, ne renvoie rien.
+        
+#         Par exemple si les deux listes suivantes sont fournies, le résultat attendu est A2, B1
+        
+#         Liste 1 :
+#         A. Les chats sont plus petits que les chiens
+#         B. Les chats mangent les souris
+#         C. Les chats vivent au plus 30 ans
+        
+#         Liste 2 :
+#         1. Les souris sont mangées par les chats
+#         2. Les chiens sont la plupart du temps plus grand en taille que les chats
+#         3. Les chats et les chiens se disputent souvent"""
+#         return result
+
+#     def post_process(self, qa:QA, cur_obj:Eval):
+#         """Processes the answer returned by the LLM to return an Eval
+#         Assumes a list like A3, B1"""
+#         text:str = cur_obj.llm_answer.text if cur_obj.llm_answer.text != "[]" else ""
+#         text_list:list = [t.strip() for t in text.split(',')]
+#         num_true_facts:int = len(qa.facts)
+#         num_returned_facts:int = len(cur_obj.meta["answer_facts"])
+#         num_true_returned:int = len(set(t[1] for t in text_list))
+#         cur_obj.meta["precision"] = float(num_true_returned / num_returned_facts)
+#         cur_obj.meta["recall"] = float(num_true_returned / num_true_facts)
+#         cur_obj.auto = float(2*cur_obj.meta["precision"]*cur_obj.meta["recall"] / (cur_obj.meta["precision"]+cur_obj.meta["recall"]))
+#         cur_obj.text = text
 
 #################################
 ## LLM + LLMS
 #################################
 class StartFrom(IntEnum):
 	beginning = 0
 	chunks = 1
@@ -346,14 +345,15 @@
     Base class for text to text LLMs.
     Class deriving from LLM must implement `complete`.
     A Prompter must be provided at creation time.
     Instantiates a get_prompt so as to be able change the prompt LLM-wise.
     """
     name:Optional[str] = None
     prompter:Prompter
+    max_tokens:int = DEFAULT_MAX_TOKENS
 
     async def generate(self, cur_obj:WithLLMAnswer, prev_obj:WithLLMAnswer, qa:QA,
                 start_from:StartFrom, b_missing_only:bool, **kwargs) -> WithLLMAnswer:
         """Generate prompt and execute LLM
         Returns the retrieved or created object containing the LLMAnswer
         If None, LLMAnswer retrieval or generation went wrong and post-processing
         must be skipped"""
@@ -410,19 +410,22 @@
 
     async def complete(self, prompt:Prompt) -> LLMAnswer:
         messages:list[dict] = [{"content":prompt.system, "role":"system"},
                                {"content":prompt.user, "role":"user"}]
         retry:int = 1
         wait_step:float = 3.0
         start_ts:datetime = datetime.now()
+        cur_logger_prefix:str = logger.prefix
         while retry:
+            logger.prefix = cur_logger_prefix
             try:
                 time_to_wait:float = wait_step
                 ans:dict = await acompletion(messages=messages, model=self.name,
-                                        temperature=self.temperature, num_retries=self.num_retries)
+                                        temperature=self.temperature, num_retries=self.num_retries,
+                                        max_tokens=self.max_tokens)
                 retry = 0
             except RateLimitError as e:
                 logger.debug(f'Rate limit reached - will retry in {time_to_wait:.2f}s ({str(e)})')
                 asyncio.sleep(time_to_wait)
                 retry += 1
             except Exception as e:
                 logger.exception(f'The following exception occurred with prompt {prompt}' + '\n' + str(e))
@@ -495,30 +498,31 @@
             even if a value already exists
             - only_llms: restrict the llms to be computed again - used in conjunction with start_from -
             if start from beginning, chunks or prompts, compute prompts and llm answers for the list only -
             if start from llm, recompute llm answers for these llm only - has not effect if start 
             """
 
         nb_q:int = len(expe)
-        async def generate_for_qa(num_q:int, qa:QA):
+        async def _generate_for_qa(num_q:int, qa:QA):
             logger.prefix = f"({num_q}/{nb_q})"
             logger.info(f'*** {self.__class__.__name__} for question "{qa.question.text}"')
             try:
                 await self.gen_for_qa(qa=qa, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms)
             except Exception as e:
                 logger.exception(f"Exception caught - saving what has been done so far:\n{e}")
-                expe.save_temp(name=f"Stopped_at_{num_q}_of_{nb_q}_")
+                expe.save_to_json()
+                # expe.save_temp(name=f"Stopped_at_{num_q}_of_{nb_q}_")
                 return
             logger.info(f'End question "{qa.question.text}"')
             if save_every and (num_q % save_every == 0): expe.save_to_json()
 
         loop = asyncio.get_event_loop()
-        tasks = [generate_for_qa(num_q, qa) for num_q, qa in enumerate(expe, start=1)]
+        tasks = [_generate_for_qa(num_q, qa) for num_q, qa in enumerate(expe, start=1)]
         logger.info(f'{len(tasks)} tasks created')
-        all_qa = loop.run_until_complete(asyncio.gather(*tasks))
+        loop.run_until_complete(asyncio.gather(*tasks))
 
     def write_chunks(self, qa:QA):
         """Write chunks in the current qa if a Retriever has been given when creating the object. Ignore otherwise"""
         raise NotImplementedError('Must implement this if you want to use it!')
     
     @abstractmethod
     async def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, 
@@ -660,77 +664,104 @@
                                     qa=qa, start_from=start_from,
                                     b_missing_only=b_missing_only,
                                     answer=ans, facts=qa.facts)          
 
             # save previous human eval if any
             if prev_eval and prev_eval.human: ans.eval.human = prev_eval.human
 
-class TwoFactsEvalGenerator(TextGenerator):
-    """Generate Eval from Answers and Facts. Converts first the Answer to a list of Facts and
-    perform evaluation"""
-
-    def __init__(self, llms:list[LLM] = None):
-        super().__init__(llms=llms)
-        if len(self.llms) < 2:
-            raise RagtimeException("""Need at least 2 LLMs to run this generator!
-                                   1st LLM is used to generate Facts from the Answer.
-                                   2nd LLM is used to generate Eval from the golden Facts and the Facts from the Answer.""")
-
-    async def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool=False):
-        """Create Eval for each QA where Facts are available"""
-
-        if len(qa.answers) == 0:
-            logger.error(f'No Answers, cannot generate Evals'); return
-        if len(qa.facts) == 0:
-            logger.error(f'No Facts, cannot generate Evals'); return
-        
-        # Eval loop
-        for ans in (a for a in qa.answers if a.text):
-            llm_name:str = ans.llm_answer.name if ans.llm_answer else "unkown LLM (manual ?)"
-            logger.debug(f'Generate Facts for answer generated with "{llm_name}"')
-            prev_eval:Eval = ans.eval
+# class TwoFactsEvalGenerator(TextGenerator):
+#     """Generate Eval from Answers and Facts. Converts first the Answer to a list of Facts and
+#     perform evaluation"""
+
+#     def __init__(self, llms:list[LLM] = None):
+#         super().__init__(llms=llms)
+#         if len(self.llms) < 2:
+#             raise RagtimeException("""Need at least 2 LLMs to run this generator!
+#                                    1st LLM is used to generate Facts from the Answer.
+#                                    2nd LLM is used to generate Eval from the golden Facts and the Facts from the Answer.""")
+
+#     async def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool=False):
+#         """Create Eval for each QA where Facts are available"""
+
+#         if len(qa.answers) == 0:
+#             logger.error(f'No Answers, cannot generate Evals'); return
+#         if len(qa.facts) == 0:
+#             logger.error(f'No Facts, cannot generate Evals'); return
+        
+#         # Eval loop
+#         for ans in (a for a in qa.answers if a.text):
+#             llm_name:str = ans.llm_answer.name if ans.llm_answer else "unkown LLM (manual ?)"
+#             logger.debug(f'Generate Facts for answer generated with "{llm_name}"')
+#             prev_eval:Eval = ans.eval
     
-            # Use 1st LLM to generate facts from the Answer
-            ans_facts:Facts = await self.llms[0].generate(cur_obj=Facts(), prev_obj=None,
-                                    qa=qa, start_from=start_from,
-                                    b_missing_only=b_missing_only,
-                                    answer=ans)    
+#             # Use 1st LLM to generate facts from the Answer
+#             ans_facts:Facts = await self.llms[0].generate(cur_obj=Facts(), prev_obj=None,
+#                                     qa=qa, start_from=start_from,
+#                                     b_missing_only=b_missing_only,
+#                                     answer=ans)    
                       
-            # Use 2nd LLM to generate Eval
-            logger.debug(f'Then generate Eval using answer facts and gold facts')
-            cur_eval:Eval = Eval()
-            cur_eval.meta['answer_facts'] = [af.text for af in ans_facts] # stores the answer's facts in the current eval
-            ans.eval = await self.llms[1].generate(cur_obj=cur_eval, prev_obj=prev_eval,
-                                    qa=qa, start_from=start_from,
-                                    b_missing_only=b_missing_only,
-                                    answer_facts=ans_facts, gold_facts=qa.facts)
-
-            # save previous human eval if any
-            if prev_eval and prev_eval.human: ans.eval.human = prev_eval.human
-
-def gen_Answers(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str], retriever:Retriever=None, 
-                start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
-  """Standard function to generate answers - returns the updated Expe or None if an error occurred"""
-  expe:Expe = Expe(json_path=folder_in / json_file)
-  ans_gen:AnsGenerator = AnsGenerator(retriever=retriever, llm_names=llm_names, prompter=prompter)
-  ans_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
-  expe.save_to_json(path=folder_out / json_file)
-  return expe
+#             # Use 2nd LLM to generate Eval
+#             logger.debug(f'Then generate Eval using answer facts and gold facts')
+#             cur_eval:Eval = Eval()
+#             cur_eval.meta['answer_facts'] = [af.text for af in ans_facts] # stores the answer's facts in the current eval
+#             ans.eval = await self.llms[1].generate(cur_obj=cur_eval, prev_obj=prev_eval,
+#                                     qa=qa, start_from=start_from,
+#                                     b_missing_only=b_missing_only,
+#                                     answer_facts=ans_facts, gold_facts=qa.facts)
+
+#             # save previous human eval if any
+#             if prev_eval and prev_eval.human: ans.eval.human = prev_eval.human
+
+def generate(text_generator: TextGenerator, folder_in:Path, folder_out:Path, json_file: Union[Path,str], 
+                start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0,
+                save_to_json:bool=True, save_to_html:bool=False, template_html_path:Path=DEFAULT_HTML_TEMPLATE,
+                save_to_spreadsheet:bool=False, template_spreadsheet_path:Path=DEFAULT_SPREADSHEET_TEMPLATE) -> Expe:
+    expe:Expe = Expe(json_path=folder_in / json_file)
+    text_generator.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
+    if save_to_json: expe.save_to_json(path=folder_out / json_file)
+    if save_to_html: expe.save_to_html(template_path=template_html_path)
+    if save_to_spreadsheet: expe.save_to_spreadsheet(template_path=template_spreadsheet_path)
+    return expe 
+
+# def gen_Answers(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str], retriever:Retriever=None, 
+#                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0,
+#                 save_to_json:bool=True, save_to_html:bool=False, template_html_path:Path=DEFAULT_HTML_TEMPLATE,
+#                 save_to_spreadsheet:bool=False, template_spreadsheet_path:Path=DEFAULT_SPREADSHEET_TEMPLATE) -> Expe:
+#   """Standard function to generate answers - returns the updated Expe or None if an error occurred"""
+#   ans_gen:AnsGenerator = AnsGenerator(retriever=retriever, llm_names=llm_names, prompter=prompter)
+#   expe:Expe = Expe(json_path=folder_in / json_file)
+#   ans_gen:AnsGenerator = AnsGenerator(retriever=retriever, llm_names=llm_names, prompter=prompter)
+#   ans_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
+#   expe.save_to_json(path=folder_out / json_file)
+#   if save_to_html: expe.save_to_html(template_path=template_html_path)
+#   if save_to_spreadsheet: expe.save_to_spreadsheet(template_path=template_spreadsheet_path)
+#   return expe
   
 
-def gen_Facts(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str],
-                start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
-  """Standard function to generate facts - returns the updated Expe or None if an error occurred"""
-  expe:Expe = Expe(json_path=folder_in / json_file)
-  fact_gen:FactGenerator = FactGenerator(llm_names=llm_names, prompter=prompter)
-  fact_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
-  expe.save_to_json(path=folder_out / json_file)
-  return expe
-
-def gen_Evals(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str],
-                start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
-  """Standard function to generate evals - returns the updated Expe or None if an error occurred"""
-  expe:Expe = Expe(json_path=folder_in / json_file)
-  eval_gen:EvalGenerator = EvalGenerator(llm_names=llm_names, prompter=prompter)
-  eval_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
-  expe.save_to_json(path=folder_out / json_file)
-  return expe
+# def gen_Facts(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str],
+#                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
+#   """Standard function to generate facts - returns the updated Expe or None if an error occurred"""
+#   expe:Expe = Expe(json_path=folder_in / json_file)
+#   fact_gen:FactGenerator = FactGenerator(llm_names=llm_names, prompter=prompter)
+#   fact_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
+#   expe.save_to_json(path=folder_out / json_file)
+#   return expe
+
+# def gen_Evals(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str],
+#                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
+#   """Standard function to generate evals - returns the updated Expe or None if an error occurred"""
+#   expe:Expe = Expe(json_path=folder_in / json_file)
+#   expe.gen_Evals()
+#   eval_gen:EvalGenerator = EvalGenerator(llm_names=llm_names, prompter=prompter)
+#   eval_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
+#   expe.save_to_json(path=folder_out / json_file)
+#   return expe
+
+# TODO: the function below cannot be implemented as of now since `expe.gen_Eval` cannot be too - see TODO with expe.gen_Eval for more details
+# def gen_Evals(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str],
+#                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
+#   """Standard function to generate evals - returns the updated Expe or None if an error occurred"""
+#   expe:Expe = Expe(json_path=folder_in / json_file)
+#   expe.gen_Evals(folder_out=folder_out, prompter=prompter, llm_names=llm_names, start_from=start_from,
+#                  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
+#   return expe
+
```

### Comparing `ragtime-0.0.32/src/ragtime/base_folder/.gitignore` & `ragtime-0.0.33/src/ragtime/base_folder/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/base_folder/LICENSE` & `ragtime-0.0.33/src/ragtime/base_folder/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/base_folder/classes.py` & `ragtime-0.0.33/src/ragtime/base_folder/classes.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/base_folder/main.py` & `ragtime-0.0.33/src/ragtime/base_folder/main.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx` & `ragtime-0.0.33/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/base_folder/res/html_templates/basic_template.jinja` & `ragtime-0.0.33/src/ragtime/base_folder/res/html_templates/basic_template.jinja`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx` & `ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx` & `ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx`

 * *Files 10% similar despite different names*

```diff
@@ -108,91 +108,91 @@
 000006b0: edad 86b0 b737 a0ea 93cf 9b7f d796 a6e9  .....7..........
 000006c0: 0d3f 8839 4cec d299 15c8 7362 67d9 ae7c  .?.9L.....sbg..|
 000006d0: c86c 21f5 f91a 5553 6839 69b0 629e 723a  .l!...USh9i.b.r:
 000006e0: 2279 5f64 6cc0 f344 9bbf 13fd 7c2d 4e9c  "y_dl..D....|-N.
 000006f0: c852 2234 12f8 32cf 47c7 25a0 f57f 5ab4  .R"4..2.G.%...Z.
 00000700: 34f1 cb9d 79c4 3709 c3ab c8f0 c982 8b1f  4...y.7.........
 00000710: a8de 0100 00ff ff03 0050 4b03 0414 0006  .........PK.....
-00000720: 0008 0000 0021 00f0 be93 b7a9 0400 009c  .....!..........
+00000720: 0008 0000 0021 005d f2ab 8aa9 0400 0096  .....!.]........
 00000730: 0d00 000f 0000 0078 6c2f 776f 726b 626f  .......xl/workbo
-00000740: 6f6b 2e78 6d6c a457 6d6f e246 10fe 5ea9  ok.xml.Wmo.F..^.
-00000750: ffc1 71f3 a195 e2f8 05e3 8015 3819 6c37  ..q.........8.l7
-00000760: e878 49b1 49ae 1592 b5b1 17b0 e2b7 5b2f  .xI.I.........[/
-00000770: 17a2 d3fd f7ce 1a4c 6c72 aae9 1d4a d6ec  .......Llr...J..
-00000780: eecc ec33 33cf 8c97 db0f bb38 e2be 6092  ...33......8..`.
-00000790: 8769 d2e3 e56b 89e7 70e2 a741 98ac 7bfc  .i...k..p..A..{.
-000007a0: c2b5 850e cfe5 1425 018a d204 f7f8 579c  .......%......W.
-000007b0: f31f fabf fe72 fb92 92e7 a734 7de6 c040  .....r.....4}..@
-000007c0: 92f7 f80d a599 2e8a b9bf c131 caaf d30c  ...........1....
-000007d0: 27b0 b34a 498c 284c c95a cc33 8251 906f  '..JI.(L.Z.3.Q.o
-000007e0: 30a6 7124 2a92 a489 310a 137e 6f41 27e7  0.q$*...1..~oA'.
-000007f0: d848 57ab d0c7 66ea 6f63 9cd0 bd11 8223  .HW...f.oc.....#
-00000800: 4401 7ebe 09b3 bcb4 16fb e798 8b11 79de  D.~...........y.
-00000810: 6682 9fc6 1998 780a a390 be16 4679 2ef6  f.....x.....Fy..
-00000820: f5d1 3a49 097a 8ac0 ed9d dce6 7604 fe34  ..:I.z......v..4
-00000830: f897 2518 94f2 24d8 7a77 541c fa24 cdd3  ..%...$.zwT..$..
-00000840: 15bd 06d3 e21e f43b ff65 4994 e55a 0876  .......;.eI..Z.v
-00000850: ef63 709e 2555 24f8 4bc8 7278 4445 b41f  .cp.%U$.K.rxDE..
-00000860: 44a5 1d6d 696f c664 e9a7 adc9 40ad 822b  D..mio.d....@..+
-00000870: 3a04 ef07 adb5 8fd8 14be 7fbb 0a23 fcb0  :............#..
-00000880: a72e 87b2 6c8a 6296 a988 e722 9453 2b08  ....l.b....".S+.
-00000890: 290e 7afc 0d4c d317 5c5b 20db 6cb0 0d23  ).z..L..\[ .l..#
-000008a0: d855 6e54 a5cd 8bfd 239d ef09 17e0 15da  .UnT....#.......
-000008b0: 46d4 0522 97e6 a132 34ad bb97 0462 1811  F.."...24....b..
-000008c0: c524 4114 0fd3 8402 0f0f 7efd 2ce7 fab7  .$A.......~.,...
-000008d0: 607b b849 81e1 dc1c 7fde 8604 4361 01bf  `{.I........Ca..
-000008e0: c057 1891 afa3 a7fc 1ed1 0db7 2551 8f1f  .W..........%Q..
-000008f0: eacb 450e ee2f d761 14e1 dc23 d80f 298a  ..E../.a...#..).
-00000900: 9679 ba25 3e5e 129c a5f9 92a0 b590 21ff  .y.%>^........!.
-00000910: 19ad f192 4214 f262 f450 fe9a f820 922f  ....B..b.P... ./
-00000920: 2b55 e951 1c67 504b b05a 2137 7a5f 49ff  +U.Q.gPK.Z!7z_I.
-00000930: 83de c867 d115 8f8e edbf 9f06 10fc 237a  ...g..........#z
-00000940: 49e1 7b4a 38f8 3e32 c790 4607 7d81 a402  I.{J8.>2..F.}...
-00000950: 7582 43cd 8f20 6b72 cb4b 7ca2 cbde 57a9  u.C.. kr.K|...W.
-00000960: a3dd 7424 5915 24a3 3510 d41b d510 06b6  ..t$Y.$.5.......
-00000970: a209 5247 55b5 aed9 ea98 46fb 1b38 4334  ..RGU.....F..8C4
-00000980: dd4f d196 6e0e 7c61 a67b bc0a e478 b735  .O..n.|a.{...x.5
-00000990: 41bb 7247 96f4 6d18 bcc1 f82a 1d3e 027b  A.rG..m....*.>.{
-000009a0: 9e0c e5de 37e6 30eb 8c0f 217e c9df 98c5  ....7.0...!~....
-000009b0: a6dc ee31 4c82 f4a5 c70b b204 9df5 b53e  ...1L..........>
-000009c0: 7d29 361f c380 6e80 9a2d a50d 15b8 5fbb  })6...n..-...._.
-000009d0: c3e1 7a03 8865 4565 8b50 410c 598f af21  ..z..eEe.PA.Y..!
-000009e0: 32f7 886c f808 6ca8 2112 2b90 8a1e 0cd0  2..l..l.!.+.....
-000009f0: 8a27 9714 7563 ed32 0cad 9e75 e722 c43c  .'..uc.2...u.".<
-00000a00: 4774 7602 1905 32f3 a82a eb50 e8e9 1561  Gtv...2..*.P...a
-00000a10: e885 4761 e554 f81e 1114 57a5 5b15 e956  ..Ga.T....W.[..V
-00000a20: c18e 120f 545e 98e0 8015 32a0 abcc 0e18  ....T^....2.....
-00000a30: bd5d 94c4 d79e 1db2 fa33 1145 4f28 07d0  .].......3.EO(..
-00000a40: 51ea a3c8 2991 0357 3661 1060 f63a e3fb  Q...)..W6a.`.:..
-00000a50: ccad 8b4b e352 d12f 9d4b e556 ac18 fdde  ...K.R./.K.V....
-00000a60: 0983 f16c f8d1 7346 ff58 7c7f 0ffc e272  ...l..sF.X|....r
-00000a70: 7029 df34 2a0e ef16 d38f de70 36ae eab5  p).4*......p6...
-00000a80: ce53 73bc d9c7 a3da 6f73 cbbe 68d6 9b39  .Ss.....os..h..9
-00000a90: 6ef5 24ad 51c3 5ccc 0d77 349b 56b5 9add  n.$.Q.\..w4.V...
-00000aa0: b2a6 a667 1a6e 2d1a ddc6 b3ac 0763 ec19  ...g.n-......c..
-00000ab0: 0b77 560b a274 9ede dd62 62d4 50ca 72b3  .wV..t...bb.P.r.
-00000ac0: e2a7 7b80 38b3 6dc7 727f 2f53 2e5f 7177  ..{.8.m.r./S._qw
-00000ad0: 9661 5af3 229f 579c 74c5 4d07 de7c f6e8  .aZ.".W.t.M..|..
-00000ae0: 5c71 f21f 8d36 6d63 e89e 2654 6dd4 ba33  \q...6mc..&Tm..3
-00000af0: c6e3 8553 f3bb 9975 1598 35cd c6d3 c6e3  ...S...u..5.....
-00000b00: c929 c476 a3d2 64e4 38a3 e99f b593 9a99  .).v..d.8.......
-00000b10: 0aa1 6311 a9bb d64c 3b50 0390 75ad e628  ..c....L;P..u..(
-00000b20: 82d6 5f0b cb61 7cad ab36 7b77 4871 cdbb  .._..a|..6{wHq..
-00000b30: 4e63 4cca d34e a3d9 9c3b c735 e6ee bb1a  NcL..N...;.5....
-00000b40: 393d b1da 77a0 b541 bff2 e1a6 c11e 45b3  9=..w..A......E.
-00000b50: edca 92d2 65ad 10ef e838 a7c5 135e f221  ....e....8...^.!
-00000b60: 34f8 41bb 3390 5a5d 4550 6dd9 1654 b92b  4.A.3.Z]EPm..T.+
-00000b70: 0983 81a6 0a6d d36e b56f 6473 68b5 6df6  .....m.n.odsh.m.
-00000b80: 8663 b770 7dc7 2cae 7ef0 72d5 110b 6d8c  .c.p}.,.~.r...m.
-00000b90: e816 2e06 ecce 51cc 7536 da87 d5e3 e26a  ......Q.u6.....j
-00000ba0: bf70 68cc b50b 813e 3799 2b07 edff 1274  .ph....>7.+....t
-00000bb0: e057 4684 cf14 b61f ce14 1c4e 27ee e44c  .WF........N'..L
-00000bc0: d9b1 e57a 8ff6 b9c2 c664 601a e7cb 1bf3  ...z.....d`.....
-00000bd0: b9f1 b76b 7d2a 8f10 bf1b 5011 720e b7a2  ...k}*....P.r...
-00000be0: 32f3 62f9 c3aa ff2f 0000 00ff ff03 0050  2.b..../.......P
+00000740: 6f6b 2e78 6d6c a457 6d6f a338 10fe 7ed2  ok.xml.Wmo.8..~.
+00000750: fd07 96eb 873b a914 4c5e daa0 a62b 12e0  .....;..L^...+..
+00000760: 1a35 2fbd 40da bd53 25e4 8293 b005 cc1a  .5/.@..S%.......
+00000770: 679b 6ab5 fffd c624 64a1 5d1d b9dd a835  g.j....$d.]....5
+00000780: b13d 337e 66e6 99c1 b97c bf4d 62e9 3361  .=3~f....|.Mb.3a
+00000790: 7944 d3be 8cce 3459 2269 40c3 285d f5e5  yD....4Y"i@.(]..
+000007a0: 85e7 2817 b294 739c 8638 a629 e9cb 2f24  ..(...s..8.)../$
+000007b0: 97df 5ffd facb e533 654f 8f94 3e49 6020  .._....3eO..>I` 
+000007c0: cdfb f29a f3cc 50d5 3c58 9304 e767 3423  ......P.<X...g4#
+000007d0: 29ec 2c29 4b30 8729 5ba9 79c6 080e f335  ).,)K0.)[.y....5
+000007e0: 213c 8955 5dd3 ba6a 82a3 54de 5930 d831  !<.U]..j..T.Y0.1
+000007f0: 36e8 7219 05c4 a2c1 2621 29df 1961 24c6  6.r.....&!)..a$.
+00000800: 1ce0 e7eb 28cb 4b6b 4970 8cb9 04b3 a74d  ....(.KkIp.....M
+00000810: a604 34c9 c0c4 6314 47fc a530 2a4b 4960  ..4...c.G..0*KI`
+00000820: 8c56 2965 f831 06b7 b7a8 236d 19fc 75e1  .V)e.1....#m..u.
+00000830: 1f69 30e8 e549 b0f5 e6a8 240a 18cd e992  .i0..I....$.....
+00000840: 9f81 6975 07fa 8dff 4853 11aa 8560 fb36  ..iu....HS...`.6
+00000850: 06c7 596a ab8c 7c8e 440e 0fa8 58f7 0751  ..Yj..|.D...X..Q
+00000860: 750f b6ba df8c 21ed a7ad 21a0 56c1 1503  u.....!...!.V...
+00000870: 82f7 83d6 3a07 6cba 7c75 b98c 6272 b7a3  ....:.l.|u..br..
+00000880: ae84 b36c 8a13 91a9 5896 629c 733b 8c38  ...l....X.b.s;.8
+00000890: 09fb f239 4ce9 33a9 2db0 4d36 d844 31ec  ...9L.3.-.M6.D1.
+000008a0: eae7 9d16 92d5 ab03 9d6f 9914 9225 dec4  .........o...%..
+000008b0: dc03 2297 e6a1 32ba dd9e de11 9240 0c33  .."...2......@.3
+000008c0: e684 a598 9321 4d39 f070 efd7 cf72 aeb0  .....!M9.p...r..
+000008d0: 3d5c 5360 b834 279f 3611 2350 58c0 2ff0  =\S`.4'.6.#PX./.
+000008e0: 1546 1c18 f831 bfc5 7c2d 6d58 dc97 87c6  .F...1..|-mX....
+000008f0: c322 07f7 1f56 511c 93dc 6724 8838 8e1f  ."...VQ...g$.8..
+00000900: 72ba 6101 7960 24a3 f903 c32b 2563 f423  r.a.y`$....+%c.#
+00000910: 0938 0852 ba8a 899f 7e82 cdfc a152 8f3e  .8.R....~....R.>
+00000920: 2749 0655 04ab 155a e3b7 35f4 3f88 8d03  'I.U...Z..5.?...
+00000930: 112d 15c2 b573 69f7 fd75 e8c0 3366 94e4  .-...si..u..3f..
+00000940: bde5 4c82 ef23 6b0c 0974 f167 4827 9026  ..L..#k..t.gH'.&
+00000950: dc57 fb08 f285 5a7e 1a30 03f9 5ff4 8b1e  .W....Z~.0.._...
+00000960: ea68 565b 4166 db54 da3d a7a7 98ce b9a6  .hV[Af.T.=......
+00000970: f486 9a35 d006 4ea7 87ac afe0 0ceb 1a01  ...5..N.........
+00000980: c51b bede 3345 98ee cb6d a0c5 9bad 09de  ....3E...m......
+00000990: 963b 4833 3651 f80d c617 6dff 51c4 f3d5  .;H36Q....m.Q...
+000009a0: 50ee 7d15 0e8b 9e78 1791 e7fc 1ba7 c454  P.}....x.......T
+000009b0: dade 4769 489f fbb2 8234 e8a9 2ff5 e973  ..GiH....4../..s
+000009c0: b179 1f85 7c0d a46c e91d a8bd ddda 3589  .y..|..l......5.
+000009d0: 566b 408c f4b6 5884 da11 c8fa 720d 91b5  Vk@...X.....r...
+000009e0: 43e4 c047 1143 0d91 5a81 5474 5f80 563c  C..G.C..Z.Tt_.V<
+000009f0: a5b4 a818 7b9b 1168 f2a2 2f17 2196 2566  ....{..h../.!.%f
+00000a00: 8813 d828 2c4a a32a eb72 e8e6 1561 e882  ...(,J.*.r...a..
+00000a10: 0761 5db8 5f15 bec5 0c27 55e9 5645 ba55  .a]._....'U.VE.U
+00000a20: b0a3 c403 3517 a524 1425 0ce8 2ab3 3d46  ....5..$.%..*.=F
+00000a30: 7f1b a7c9 99ef 44a2 f22c ccf1 23ce 0174  ......D..,..#..t
+00000a40: 4c03 1cbb 2572 e0ca 3a0a 4322 5e64 f295  L...%r..:.C"^d..
+00000a50: 70eb dd89 79a2 1b27 ee89 7ea9 568c 7eef  p...y..'..~.V.~.
+00000a60: 84c1 7836 bcf1 ddd1 3fb6 7cb5 03fe ee64  ..x6....?.|....d
+00000a70: 7082 ce1b 1587 d78b e98d 3f9c 8dab 7aad  p.........?...z.
+00000a80: e3d4 5c7f 7673 50fb 6d6e 3bef 9af5 66ae  ..\.vsP.mn;...f.
+00000a90: 573d a9db a861 2de6 a637 9a4d ab5a cd6e  W=...a-..7.M.Z.n
+00000aa0: d953 cbb7 4caf 168d 5ee3 59f6 9d39 f6cd  .S..L...^.Y..9..
+00000ab0: 8537 ab05 513b 4eef 7a31 316b 2811 6a56  .7..Q;N.z11k(.jV
+00000ac0: fc70 0b10 678e e3da deef 65ca d1a9 746d  .p..g.....e...tm
+00000ad0: 9b96 3d2f f279 2a69 a7d2 74e0 cf67 f7ee  ..=/.y*i..t..g..
+00000ae0: a984 fe68 b4e9 9843 ef75 42db 8d5a d7e6  ...h...C.uB..Z..
+00000af0: 78bc 706b 7e37 b3ae 02b3 a6d9 78da 783c  x.pk~7......x.x<
+00000b00: 790d b1d3 a834 19b9 ee68 fa67 eda4 66a6  y....4...h.g..f.
+00000b10: 42e8 4444 eaae 35d3 0ed4 0064 5dab 398a  B.DD..5....d].9.
+00000b20: a0f5 d7c2 7605 5feb aacd deed 535c f3ee  ....v._.....S\..
+00000b30: a231 26e5 69af a3d9 9c3b d733 e7de 9b1a  .1&.i....;.3....
+00000b40: 797d 62b5 ef40 6b83 7e15 c01d 433c 8a66  y}b..@k.~...C<.f
+00000b50: db43 9ade 13ad 906c f938 e7c5 135e ef11  .C.....l.8...^..
+00000b60: 34f8 41e7 62a0 b57a bad2 7690 a3b4 514f  4.A.b..z..v...QO
+00000b70: 5306 836e 5be9 584e ab73 8eac a1dd 71c4  S..n[.XN.s....q.
+00000b80: 1b4e dcbf 8dad b0b8 fcc1 6bd5 855a 6813  .N........k..Zh.
+00000b90: cc37 7031 10b7 8d62 6e88 d1d9 af1e 1697  .7p1...bn.......
+00000ba0: bb85 7d63 ae5d 088c b925 5cd9 6bff 97a0  ..}c.]...%\.k...
+00000bb0: 0bbf 2f62 72a4 b073 77a4 e070 3af1 2647  ../br..sw..p:.&G
+00000bc0: ca8e 6dcf bf77 8e15 3627 03cb 3c5e de9c  ..m..w..6'..<^..
+00000bd0: cfcd bf3d fb43 7984 fadd 80aa 9073 b815  ...=.Cy......s..
+00000be0: 9599 57cb 9f54 57ff 0200 00ff ff03 0050  ..W..TW........P
 00000bf0: 4b03 0414 0006 0008 0000 0021 00a1 890e  K..........!....
 00000c00: 7a25 0100 00e1 0400 001a 0008 0178 6c2f  z%...........xl/
 00000c10: 5f72 656c 732f 776f 726b 626f 6f6b 2e78  _rels/workbook.x
 00000c20: 6d6c 2e72 656c 7320 a204 0128 a000 0100  ml.rels ...(....
 00000c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -224,15 +224,15 @@
 00000df0: bead 3b50 8dc8 33c4 2491 1c3b ab10 ccfd  ..;P..3.$..;....
 00000e00: 9230 63dc 2b32 14c0 3003 757f 4a88 23bb  .0c.+2..0.u.J.#.
 00000e10: f0a3 6421 98f4 c230 6908 66bd ec84 c061  ..d!...0i.f....a
 00000e20: f1ce ce7f 499a 2744 f591 1c82 b95b 1486  ....I.'D.....[..
 00000e30: 87d6 6f80 e9f7 d058 87e2 6f97 8c67 bf57  ..o....X..o..g.W
 00000e40: 704e 1f4b 399e d33c e4c9 62ca 7f01 0000  pN.K9..<..b.....
 00000e50: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00000e60: 2100 0881 087e 6212 0000 62aa 0000 1800  !....~b...b.....
+00000e60: 2100 c712 3e03 6812 0000 6daa 0000 1800  !...>.h...m.....
 00000e70: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
 00000e80: 7368 6565 7431 2e78 6d6c ac55 5d6f da30  sheet1.xml.U]o.0
 00000e90: 147d 9fb4 ff10 f9bd 0986 1028 2254 1d55  .}.........("T.U
 00000ea0: b54a 7da8 ca3e 9e8d 7303 5693 38b3 cdd7  .J}..>..s.V.8...
 00000eb0: a6fd f75d 3b1f b4a5 6350 ada2 b1b1 7d8f  ...];...cP....}.
 00000ec0: cf3d f7dc 30be dae6 99b7 06a5 852c 6242  .=..0........,bB
 00000ed0: fd0e f1a0 e032 11c5 2226 5fbf dc5e 0c89  .....2.."&_..^..
@@ -271,1318 +271,1318 @@
 000010e0: 0674 38c0 406d 76f6 d530 380a 81e7 1c04  .t8.@mv..08.....
 000010f0: 8e6f 40bc 22fd 4220 9b15 4ade 6611 d548  .o@.".B ..J.f..H
 00001100: 38fe 9d0c 45aa e780 2279 470f c723 a0d8  8...E..."yG..#..
 00001110: 6ae7 80e2 6f86 03c5 f108 e861 cd8e a67f  j...o......a....
 00001120: 5983 e2f8 de5a d0d6 44b6 bd6b a7d8 d748  Y....Z..D..k...H
 00001130: 55c8 73b5 a38d afec e4ff a947 1bd7 d949  U.s........G...I
 00001140: 0d1b f961 486b bf36 6ccf d4cf 6657 75d0  ...aHk.6l...fWu.
-00001150: decd 8343 375b 8dce a935 6d0c 6e27 ad08  ...C7[...5m.n'..
-00001160: 7bb6 27b6 286d dc6d 2735 4ce8 0f06 835e  {.'.(m.m'5L....^
-00001170: d8b3 bd76 16a5 c6d4 f46d 579f 85d5 78b9  ...v.....mW...x.
-00001180: 8b3e f937 2ffb 8a74 2fae 3f00 0000 ffff  .>.7/..t/.?.....
-00001190: 0000 00ff ffac 9d5b 6fdc d615 46ff 8aab  .......[o...F...
-000011a0: beb4 6851 cdb9 7066 64c8 02e2 c88e efce  ..hQ..pfd.......
-000011b0: 05ed bbe0 2ac8 4be2 c272 d3f6 df67 e6ec  ....*.K..r...g..
-000011c0: c988 a4ce a267 017d 0890 50cb 673e 8a1f  .....g.}..P.g>..
-000011d0: b768 ad90 bcbc fbe9 f6f6 f3f5 cde7 9bab  .h..............
-000011e0: cb4f 1fff f3e8 d393 b374 f6e8 ee5f 37bf  .O.......t..._7.
-000011f0: dced feed 71ba d8fd 47db f4e1 df77 9f3f  ....q...G....w.?
-00001200: fefc fce3 a79f 6f3e b70d ff4d f5e6 c3e3  ......o>...M....
-00001210: 7ffe effa f6ee c3ed 2fbb 6dab bf95 b3ab  ......../.m.....
-00001220: cb0f fb25 beda aff1 e46c 7b76 7ed8 f0f4  ...%.....l{v~...
-00001230: f70d 8f76 e0dd 0efb f56a 7579 feeb d5e5  ...v.....juy....
-00001240: f987 03f1 7510 ebb3 7b22 4d89 eb20 7689  ....u...{"M.. v.
-00001250: 8e6b e429 f16c feb1 cf63 43ca c720 df1c  .k.).l...cC.. ..
-00001260: b60c c72d 2f0e 5b36 c72d 2f1f 4629 d30f  ...-/.[6.-/.F)..
-00001270: 7a7d f833 e5f8 67de 1cb6 ac8f 5bde 1eb6  z}.3..g.....[...
-00001280: dc7f 13de 3dd8 f2fe b065 bc4f f5f8 51e7  ....=....e.O..Q.
-00001290: bb03 723c 2af9 ff70 54f6 6bb4 6377 fc06  ..r<*..pT.k.cw..
-000012a0: 0ed3 fd7a fa90 58cf 0e53 10e3 c334 23ae  ...z..X..S...4#.
-000012b0: bf48 3c7b f829 9be9 a73c 3f10 6574 acb7  .H<{.)...<?.et..
-000012c0: 53e4 9b03 324e 7231 455e 1c90 edb8 53b3  S...2Nr1E^....S.
-000012d0: dabd fc62 da57 0fd3 a659 335f 7f39 ee9b  ...b.W...Y3_.9..
-000012e0: 2fc7 7d7b 42dc 771d a6ce ce82 f79d c033  /.}{B.w........3
-000012f0: e4db 0e32 abf8 775f acc2 f79d 45ee cbdb  ...2..w_....E...
-00001300: e6c0 0f9d 45ee 3f67 d2ef dda1 9e4c 9dc5  ....E.?g.....L..
-00001310: f132 ee45 9df5 efe9 e48b b362 7dbd ff98  .2.E.......b}...
-00001320: 2767 9b51 23ea ac58 d71d 6456 ac67 e38f  'g.Q#..X..dV.g..
-00001330: 1866 8d7a 1e7f 3ed5 d167 0cb3 c27c 7360  .f.z..>..g...|s`
-00001340: 5663 6676 8c5e 1c98 dd88 b83f 5d67 07e9  Vcfv.^.....?]g..
-00001350: e5c3 acc3 ec10 bcea c459 cf98 d7bd c8b3  .........Y......
-00001360: d1f0 a617 79f6 ad7f db8b 3c3b 02ef 26cc  ....y.....<;..&.
-00001370: edee 47c1 8f57 2f9f ffe9 4d79 7276 f6d7  ..G..W/...Myrv..
-00001380: 47fb 7fde 94f3 edba ae56 7f79 5bfe 7c79  G........V.y[.|y
-00001390: fee3 fe67 c51f fff1 d59b bf3f fbc3 f4f4  ...g.......?....
-000013a0: 7e3f 390a b3a3 f8ed e48b b3e3 f7dd f88b  ~?9.............
-000013b0: ebd9 f1fb 7ef2 c5d9 81fb 61f2 c5fb 2336  ....~.....a...#6
-000013c0: a9f2 eec8 9f5c e557 7b78 3793 ebf1 e7c6  .....\.W{x7.....
-000013d0: fbd8 52da cf96 c9ba 8359 770f 4fd7 8d2d  ..R......Yw.O..-
-000013e0: 9d75 7723 f4e4 bccf f6f0 6edd 74cc fbea  .uw#......n.t...
-000013f0: b065 b407 b1a5 f349 bbf3 eef4 efcc 1e9e  .e.....I........
-00001400: ee41 6ce9 acbb 9bf0 a7af bb87 a7eb c696  .Al.............
-00001410: ceba fbab 9ff1 a5d0 d250 7a75 b854 6adf  .........Pzu.Tj.
-00001420: 87c9 714b bbd3 fcf4 651a fd7b bee9 3af3  ..qK....e..{..:.
-00001430: 2bb3 c538 bb43 74bf 9fd3 75f6 53f9 e4dd  +..8.Ct...u.S...
-00001440: da5d 3cd1 3afb 53f9 f475 8e43 6677 5138  .]<.:.S..u.CfwQ8
-00001450: cda3 4e98 fd60 3d1e bfe9 3aea 0449 e333  ..N..`=...:..I.3
-00001460: 64ba 8e39 215e a571 ffa7 eb8c eabe 7abc  d..9!^.q......z.
-00001470: 3fae cb07 6c5c f8e9 42a3 7e9f b2d0 b8e1  ?...l\..B.~.....
-00001480: d385 4685 3e65 21ac 741e 55fa 8485 1ade  ..F.>e!.t.U.....
-00001490: ed74 1e75 fa94 85b0 d479 54ea 5316 c256  .t.u.....yT.S..V
-000014a0: e751 ab4f 5908 6b9d 47b5 3e65 21ec 751e  .Q.OY.k.G.>e!.u.
-000014b0: f5fa 9485 b0d8 7954 ec53 16c2 6667 d7ec  ......yT.S..fg..
-000014c0: 86f7 0fbf 6b76 c666 67d7 ec86 7713 15d7  ....kv.fg...w...
-000014d0: ec86 f717 72cd 2ed8 ece2 9add f07e 22d7  ....r........~".
-000014e0: ecdd cf43 18b4 c535 bbe1 fd44 aed9 059b  ...C...5...D....
-000014f0: 5d5c b31b de4f e49a 5d70 6617 d7ec 86f7  ]\...O..]pf.....
-00001500: 13b9 6617 9cd9 d535 bbe1 dd44 d535 bbe1  ..f....5...D.5..
-00001510: fd85 5cb3 2bce ecea 9add f07e 22d7 ec8a  ..\.+......~"...
-00001520: 33bb ba66 37bc 9fc8 35bb e2cc aeae d90d  3..f7...5.......
-00001530: ef27 72cd ae38 b3ab 6b76 c3bb 8906 d7ec  .'r..8..kv......
-00001540: 86f7 1772 cd1e 7066 0fae d90d ef27 72cd  ...r..pf.....'r.
-00001550: 1e70 660f aed9 0def 2772 cd1e 7066 0fae  .pf.....'r..pf..
-00001560: d90d ef27 72cd 1e70 660f aed9 0def 2772  ...'r..pf.....'r
-00001570: cd1e 7066 af5d b31b de4d b476 cd6e 787f  ..pf.]...M.v.nx.
-00001580: 21d7 ec35 ceec b56b 76c3 fb89 5cb3 d738  !..5...kv...\..8
-00001590: b3d7 aed9 0def 2772 cd5e e3cc 5ebb 6637  ......'r.^..^.f7
-000015a0: bc9f c835 7b8d 337b ed9a ddf0 6ea2 8d6b  ...5{.3{....n..k
-000015b0: 76c3 fb0b b966 6f70 666f 5cb3 1bde 4fe4  v....fopfo\...O.
-000015c0: 9abd c199 bd71 cd6e 783f 916b f606 67f6  .....q.nx?.k..g.
-000015d0: c635 bbe1 fd44 aed9 1b9c d91b d7ec 86f7  .5...D..........
-000015e0: 13b9 666f 7066 6f5d b31b de4d b475 cd6e  ..fopfo]...M.u.n
-000015f0: 787f 21d7 ec2d ceec ad6b 76c3 fb89 5cb3  x.!..-...kv...\.
-00001600: b738 b3b7 aed9 0def 2772 cdde e2cc deba  .8......'r......
-00001610: 6637 bc9f c835 7b8b 337b eb9a ddf0 6ea2  f7...5{.3{....n.
-00001620: 0bd7 ec86 f717 72cd bec0 997d e19a ddf0  ......r....}....
-00001630: 7e22 d7ec 0b9c d917 aed9 0def 2772 cdbe  ~"..........'r..
-00001640: c099 7de1 9add f07e 22d7 ec0b 9cd9 17ae  ..}....~".......
-00001650: d90d ef27 72cd be58 5034 aeda 69b5 e7bb  ...'r..XP4..i...
-00001660: 99d2 ca95 3b78 58ca d53b add8 d5ac 5cc1  ....;xX..;....\.
-00001670: 53e3 2195 ab78 5ab1 b159 b992 a7c6 432a  S.!..xZ..Y....C*
-00001680: 57f3 b462 6fb3 92e2 a6f1 904a aa9b 15bb  W..bo......J....
-00001690: 9b95 9437 8def a71a 1bc9 533c d092 9394  ...7......S<....
-000016a0: 6d5f d092 cd34 1e7c e249 a9b8 ed49 b6bd  m_...4.|.I...I..
-000016b0: f1f0 bd92 6d5f f093 4d39 9a1d 6445 d9ac  ....m_..M9..dE..
-000016c0: a359 8adb 9e64 db1b 0fdf 2bd9 f6c4 6d6f  .Y...d....+...mo
-000016d0: ffe7 a1d9 419e ed52 5626 b695 49ea cae0  ....A..RV&..I...
-000016e0: fbdf 2b29 2c53 e361 29d9 f6a6 3861 29d9  ..+),S.a)...8a).
-000016f0: f626 3961 2939 db9b e684 a5e4 6c6f a213  .&9a)9......lo..
-00001700: 9692 6d67 7799 9a8d 1415 657b 99a4 be0c  ..mgw.....e{....
-00001710: bebf 8352 6026 3698 a939 49b1 83ec 3093  ...R`&6..9I...0.
-00001720: 9498 c1c3 0eca b6b3 c74c 5264 060f a964  .........LRd...d
-00001730: dbd9 6526 2933 8387 54b2 edec 3393 149a  ..e&)3..T...3...
-00001740: c143 2a79 25c3 4e33 49a9 197c 3f95 d49a  .C*y%.N3I..|?...
-00001750: 89bd 666a a652 9c38 6c36 9354 9bc1 c30e  ..fj.R.8l6.T....
-00001760: cad9 ce76 3349 bd19 3ca4 92b3 9d0d 6792  ...v3I..<.....g.
-00001770: 8a33 7848 25af 64d8 7226 a939 83ef a792  .3xH%.d.r&.9....
-00001780: a233 b1e9 4ccd 5d8a 8ab2 eb4c 5276 060f  .3..L.]....LRv..
-00001790: 3b28 673b fbce 2485 67f0 904a ce76 769e  ;(g;..$.g..J.vv.
-000017a0: 494a cfe0 2195 9ced ec3d 9314 9fc1 432a  IJ..!....=....C*
-000017b0: 39db d97d 2629 3f83 efa7 92fa 33b1 ff4c  9..}&)?.....3..L
-000017c0: cd68 8a13 870d 6892 0a34 78d8 4139 dbd9  .h....h..4x.A9..
-000017d0: 8226 a941 8387 5472 b6b3 094d 5285 060f  .&.A..Tr...MR...
-000017e0: a9e4 6c67 1b9a a40e 0dbe 9f4a 0ad1 c446  ..lg.......J...F
-000017f0: 3435 c729 2aca 4e34 4929 1a3c eca0 9ced  45.)*.N4I).<....
-00001800: ec45 9314 a3c1 432a 39db d98d 2629 4783  .E....C*9...&)G.
-00001810: 8754 72b6 b31f 4d52 9006 0fa9 e46c 6747  .Tr...MR.....lgG
-00001820: 9aa4 240d be9f 4a6a d2c4 9e34 35f3 294e  ..$...Jj...45.)N
-00001830: 1c36 a549 aad2 e061 07e5 6c67 5b9a a42e  .6.I...a..lg[...
-00001840: 0d1e 52c9 d9ce c634 4965 1a3c a492 b39d  ..R....4Ie.<....
-00001850: ad69 92da 34f8 7e2a 294e 139b d3d4 5ca8  .i..4.~*)N....\.
-00001860: a828 bbd3 24e5 69f0 b083 72b6 b33f 4d52  .(..$.i...r..?MR
-00001870: a006 0fa9 e46c 6787 9aa4 440d 1e52 c9d9  .....lg...D..R..
-00001880: ce1e 3549 911a 3ca4 92b3 9d5d 6a6e 6ef4  ..5I..<....]jnn.
-00001890: f48a 06df 4d95 a54b 0d1e 9692 3708 b14b  ....M..K....7..K
-000018a0: cdd2 a506 0fa9 dc6c cfec 52b3 74a9 c143  .......l..R.t..C
-000018b0: 2a37 db33 bbd4 2c5d 6af0 90ca cdf6 cc2e  *7.3..,]j.......
-000018c0: 354b 971a 7c3f 9574 a999 5d6a 6e6e 549c  5K..|?.t..]jnnT.
-000018d0: 38ec 52b3 74a9 c1c3 0eba d99e d9a5 e6e6  8.R.t...........
-000018e0: 46cd 0ee2 ff39 90a5 4b0d 1e76 50b6 9def  F....9..K..vP...
-000018f0: f8cc d2a5 060f a964 dbd9 a566 e952 83ef  .......d...f.R..
-00001900: a7b2 377e 2edc f969 6ffd 6c3c a4b2 377f  ..7~...io.l<..7.
-00001910: f2dd 9ff6 f64f 76a9 d9de 00ca 2e35 db5b  .....Ov......5.[
-00001920: 40d9 a566 7b13 28bb d46c 6f03 5db8 0f54  @..f{.(..lo.]..T
-00001930: bad4 bc70 27a8 bd15 94ef 05cd d2a5 06df  ...p'...........
-00001940: afa8 74a9 995d 6a96 2e35 7848 2567 3bbb  ..t..]j..5xH%g;.
-00001950: d42c 5d6a f090 ca5d b767 76a9 59ba d4e0  .,]j...].gv.Y...
-00001960: 2195 bb6e cfec 52b3 74a9 c143 2a77 dd9e  !..n..R.t..C*w..
-00001970: d9a5 66e9 5283 efa7 922e 35b3 4bcd d2a5  ..f.R.....5.K...
-00001980: 060f a964 dbf9 3ed1 dcdc a8b8 9261 979a  ...d..>......a..
-00001990: a54b 0d1e 7650 5ec9 b04b cdd2 a506 0fa9  .K..vP^..K......
-000019a0: e495 0cbb d42c 5d6a f0fd 54d2 a566 76a9  .....,]j..T..fv.
-000019b0: 59ba d4e0 2195 bc92 e13b 4773 73a3 a2a2  Y...!....;Gss...
-000019c0: ec52 b374 a9c1 c30e cad9 ce2e 354b 971a  .R.t........5K..
-000019d0: 3ca4 92b3 9d5d 6a96 2e35 7848 2567 3bbb  <....]j..5xH%g;.
-000019e0: d42c 5d6a f0fd 54d2 a566 76a9 59ba d4e0  .,]j..T..fv.Y...
-000019f0: 2195 9ced 7c3f 696e 6e54 9c38 ec52 b374  !...|?innT.8.R.t
-00001a00: a9c1 c30e cad9 ce2e 354b 971a 3ca4 92b3  ........5K..<...
-00001a10: 9d5d 6a96 2e35 f87e 2ae9 5233 bbd4 2c5d  .]j..5.~*.R3..,]
-00001a20: 6af0 904a ce76 bec3 3437 372a 2aca 2e35  j..J.v..477**..5
-00001a30: 4b97 1a3c eca0 9ced ec52 b374 a9c1 432a  K..<.....R.t..C*
-00001a40: 39db d9a5 66e9 5283 8754 72b6 b34b cdd2  9...f.R..Tr..K..
-00001a50: a506 df4f 255d 6a66 979a a54b 0d1e 52c9  ...O%]jf...K..R.
-00001a60: d9ce f79d e6e6 46c5 89c3 2e35 4b97 1a3c  ......F....5K..<
-00001a70: eca0 9ced ec52 b374 a9c1 432a 39db d9a5  .....R.t..C*9...
-00001a80: 66e9 5283 efa7 922e 35b3 4bcd d2a5 060f  f.R.....5.K.....
-00001a90: a9e4 6ce7 3b51 7373 a3a2 a2ec 52b3 74a9  ..l.;Qss....R.t.
-00001aa0: c1c3 0eca d9ce 2e35 4b97 1a3c a492 b39d  .......5K..<....
-00001ab0: 5d6a 962e 3578 4825 673b bbd4 225d 6af0  ]j..5xH%g;.."]j.
-00001ac0: dd54 45ba d4e0 6129 d7f6 c22e b548 971a  .TE...a).....H..
-00001ad0: 3ca4 722e b5b0 4b2d d2a5 060f a9dc 6c2f  <.r...K-......l/
-00001ae0: ec52 8b74 a9c1 432a 37db 0bbb d422 5d6a  .R.t..C*7...."]j
-00001af0: f0fd 54d2 a516 76a9 45ba d4e0 2195 6c3b  ..T...v.E...!.l;
-00001b00: 3f31 b7c8 fb52 8387 54b2 ed7c 5f6a 912e  ?1...R..T..|_j..
-00001b10: 3578 4825 dbce 2eb5 4897 1a3c a492 6d67  5xH%....H..<..mg
-00001b20: 975a a44b 0dbe 9f4a bad4 c22e b548 971a  .Z.K...J.....H..
-00001b30: 3ca4 926d e7fb 528b 74a9 c143 2ad9 7676  <..m..R.t..C*.vv
-00001b40: a945 bad4 e021 956c 3bbb d422 5d6a f090  .E...!.l;.."]j..
-00001b50: 4ab6 9d5d 6a91 2e35 f87e 2afb 60dd 8527  J..]j..5.~*.`..'
-00001b60: eb4a 975a 169e ad6b 1fae bbf4 745d f7b7  .J.Z...k....t]..
-00001b70: d4b2 f07c 5dfb 80dd 8527 ec36 377a fadf  ...|]....'.67z..
-00001b80: 26ca c233 76ed 4376 179e b2db dca8 4985  &..3v.Cv......I.
-00001b90: cf92 29f6 41bb 0b4f da6d 6ed4 a4c2 670e  ..).A..O.mn...g.
-00001ba0: 14e9 5283 ef9f 38d2 a516 76a9 45ba d4e0  ..R...8...v.E...
-00001bb0: 2195 6c3b bbd4 225d 6af0 90ca fd2d b5f0  !.l;.."]j....-..
-00001bc0: 7377 4b73 a3a2 0cec 528b 74a9 c1c3 0eca  swKs....R.t.....
-00001bd0: d9ce 2eb5 4897 1a7c 3f95 74a9 855d 6a91  ....H..|?.t..]j.
-00001be0: 2e35 7848 25af 64d8 a516 e952 8387 54f2  .5xH%.d....R..T.
-00001bf0: 4a86 9fc4 5b9a 1b15 1565 975a a44b 0d1e  J...[....e.Z.K..
-00001c00: 76d0 fd4e a6b0 4b2d d2a5 060f a9dc ef64  v..N..K-.......d
-00001c10: 0abb d422 5d6a f0fd 54d2 a516 76a9 45ba  ..."]j..T...v.E.
-00001c20: d4e0 2195 9ced ec52 8b74 a9c1 432a 39db  ..!....R.t..C*9.
-00001c30: f9f9 bca5 b951 71e2 b04b 2dd2 a506 0f3b  .....Qq..K-....;
-00001c40: 2867 3bbb d422 5d6a f0fd 54d2 a516 76a9  (g;.."]j..T...v.
-00001c50: 45ba d4e0 2195 9ced ec52 8b74 a9c1 432a  E...!....R.t..C*
-00001c60: 39db f989 bda5 b951 5151 76a9 45ba d4e0  9......QQQv.E...
-00001c70: 6107 e56c 6797 5aa4 4b0d 1e52 c9d9 ce2e  a..lg.Z.K..R....
-00001c80: b548 971a 7c3f 9574 a985 5d6a 912e 3578  .H..|?.t..]j..5x
-00001c90: 4825 673b bbd4 225d 6af0 904a ce76 7e8e  H%g;.."]j..J.v~.
-00001ca0: 6f69 6e54 9c38 ec52 8b74 a9c1 c30e cad9  oinT.8.R.t......
-00001cb0: ce2e b548 971a 7c3f 9574 a985 5d6a 912e  ...H..|?.t..]j..
-00001cc0: 3578 4825 673b bbd4 225d 6af0 904a ce76  5xH%g;.."]j..J.v
-00001cd0: 7eb2 6f69 6e54 5494 5d6a 912e 3578 d841  ~.oinTT.]j..5x.A
-00001ce0: 39db d9a5 16e9 5283 8754 72b6 b34b ddbd  9.....R..Tr..K..
-00001cf0: 52f4 fe7d 8527 3c5f 34f8 6eaa 2a5d 6af0  R..}.'<_4.n.*]j.
-00001d00: b094 6b7b 6597 5aa5 4b0d 1e52 b9b6 5776  ..k{e.Z.K..R..Wv
-00001d10: a955 bad4 e021 95fb 7d7b 6597 5aa5 4b0d  .U...!..}{e.Z.K.
-00001d20: 1e52 b9d9 5ed9 a556 e952 83ef a792 2eb5  .R..^..V.R......
-00001d30: b24b add2 a506 0fa9 64db d9a5 56e9 5283  .K......d...V.R.
-00001d40: 8754 b2ed ec52 ab74 a9c1 432a d976 76a9  .T...R.t..C*.vv.
-00001d50: 55ba d4e0 2195 6c3b bbd4 2a5d 6af0 fd54  U...!.l;..*]j..T
-00001d60: d2a5 5676 a955 bad4 e021 956c 3bbb d42a  ..Vv.U...!.l;..*
-00001d70: 5d6a f090 4ab6 9d5d 6a95 2e35 7848 25db  ]j..J..]j..5xH%.
-00001d80: ce2e b54a 971a 3ca4 926d 6797 5aa5 4b0d  ...J..<..mg.Z.K.
-00001d90: be9f 4aba d4ca 2eb5 4a97 1a3c a492 6d67  ..J.....J..<..mg
-00001da0: 975a 9b1b 3dfd 0a39 7848 25db ce2e b54a  .Z..=..9xH%....J
-00001db0: 971a 3ca4 926d 6797 5aa5 4b0d 1e52 c9b6  ..<..mg.Z.K..R..
-00001dc0: b34b add2 a506 df4f 655f 5cba f0e6 52fb  .K.....Oe_\...R.
-00001dd0: ead2 8577 974a 975a 17de 5e6a 5f5f baf4  ...w.J.Z..^j__..
-00001de0: fe52 d9f6 8537 98da 5798 2ebc c354 bad4  .R...7..W....T..
-00001df0: baf0 1653 fb1a d385 f798 3637 2a86 ccc2  ...S......67*...
-00001e00: 9b4c edab 4cf9 5da6 55ba d4e0 fb27 8e74  .L..L.].U....'.t
-00001e10: a995 9ff1 5be5 337e 8387 54ee 3790 95ef  ....[.3~..T.7...
-00001e20: 4bad f2be d4e0 2195 fb0d 6465 975a a54b  K.....!...de.Z.K
-00001e30: 0d1e 52b9 dfc9 5476 a955 bad4 e021 95fb  ..R...Tv.U...!..
-00001e40: 9d4c 6597 5aa5 4b0d be9f 4aba d4ca 2eb5  .Le.Z.K...J.....
-00001e50: 4a97 1a3c a492 6d67 975a a54b 0d1e 52c9  J..<..mg.Z.K..R.
-00001e60: b6b3 4bad d2a5 060f a964 dbf9 7da7 b5b9  ..K......d..}...
-00001e70: 5131 dbd9 a556 e952 83ef efa0 74a9 955d  Q1...V.R....t..]
-00001e80: 6a95 2e35 7848 25af dbd9 a556 e952 8387  j..5xH%....V.R..
-00001e90: 54f2 4a86 5d6a 952e 3578 4825 afdb f90d  T.J.]j..5xH%....
-00001ea0: a8b5 b951 5151 76a9 55ba d4e0 6107 e56c  ...QQQv.U...a..l
-00001eb0: 6797 5aa5 4b0d be9f 4aba d4ca 2eb5 4a97  g.Z.K...J.....J.
-00001ec0: 1a3c a492 b39d 5d6a 952e 3578 4825 673b  .<....]j..5xH%g;
-00001ed0: bbd4 2a5d 6af0 904a ce76 7e2f 6a6d 6e54  ..*]j..J.v~/jmnT
-00001ee0: 9c38 ec52 ab74 a9c1 f777 50ba d4ca 2eb5  .8.R.t...wP.....
-00001ef0: 4a97 1a3c a492 b39d 5d6a 952e 3578 4825  J..<....]j..5xH%
-00001f00: 673b bbd4 2a5d 6af0 904a ce76 7e53 6a6d  g;..*]j..J.v~Sjm
-00001f10: 6e54 5494 5d6a 952e 3578 d841 39db d9a5  nTT.]j..5x.A9...
-00001f20: 0ed2 a506 df4d 3548 971a 3c2c e5da 3eb0  .....M5H..<,..>.
-00001f30: 4b1d a44b 0d1e 52b9 b60f ec52 07e9 5283  K..K..R....R..R.
-00001f40: 8754 ee77 7d03 5bcb 415a cbe0 fba9 a4b5  .T.w}.[.AZ......
-00001f50: 1cd8 5a0e d20f 060f a9e4 1164 3f38 483f  ..Z........d?8H?
-00001f60: 183c a492 4790 4ddc 204d 5cf0 fd54 d2c4  .<..G.M. M\..T..
-00001f70: 0d6c e206 e9bc 8287 54f2 08b2 f31a a4f3  .l......T.......
-00001f80: 0a1e 52c9 23c8 7669 9076 29f8 7e2a 6997  ..R.#.vi.v).~*i.
-00001f90: 06b6 4b83 f438 c143 2a79 04d9 e30c d2e3  ..K..8.C*y......
-00001fa0: 043f 4d75 7ef7 d3ed ede7 eb9b cf37 57bf  .?Mu~........7W.
-00001fb0: 0100 00ff ff00 0000 ffff 6c51 4d4f c240  ..........lQMO.@
-00001fc0: 10fd 2b9b 0921 9aa8 a505 252d 6d13 0821  ..+..!....%-m..!
-00001fd0: e1a0 07b8 785d e9b4 dd58 baeb 74aa 80f1  ....x]...X..t...
-00001fe0: bf3b 151a 3db8 87d9 79f3 f166 e76d ac5b  .;..=...y..f.m.[
-00001ff0: b62b 5331 9222 cc13 9807 d136 0075 a0a8  .+S1.".....6.u..
-00002000: 3559 029f a3cb b995 dbef cce8 d7f4 b92f  5Y............./
-00002010: f0d2 7867 ebcc b0b1 b5ae 5696 f69a d9d4  ..xg......V.....
-00002020: 856a dece ace3 e879 b5f4 a501 a432 dfb4  .j.....y.....2..
-00002030: 152a 3e3a 4c00 0f8e b069 a40f 5476 c8d7  .*>:L....i..Tv..
-00002040: 3273 04ca 91b1 64f8 9880 2f0d b9f0 b595  2s....d.../.....
-00002050: 4ee7 4fcb abc1 623c ac78 362c 7836 5804  N.O...b<.x6,x6X.
-00002060: 37ea 0f06 b88e bdbe 36f6 ce63 5271 fe7b  7.......6..cRq.{
-00002070: 591a 3b5d e0a3 a6c2 d48d aa30 6719 7c37  Y.;].......0g.|7
-00002080: 0545 a628 7b9f adfb 89de 837a b1cc 76df  .E.({......z..v.
-00002090: a312 7586 d4a1 31a8 dc5a 91ef 0c44 888e  ..u...1..Z...D..
-000020a0: 778b dc3a e5b4 43da 9a93 ac19 8292 85b0  w..:..C.........
-000020b0: 66dd 4994 80b3 c4a4 0d83 2a25 7eb2 92a8  f.I.......*%~...
-000020c0: 96ce 2430 09c2 49f8 300d 4221 7e47 62b3  ..$0..I.0.B!~Gb.
-000020d0: bb24 4415 8aba 2fa1 75e6 7782 7b1f 965e  .$D.../.u.w.{..^
-000020e0: 9b12 91d3 6f00 0000 ffff 0300 504b 0304  ....o.......PK..
-000020f0: 1400 0600 0800 0000 2100 d96a c756 cc0a  ........!..j.V..
-00002100: 0000 2e4c 0000 1800 0000 786c 2f77 6f72  ...L......xl/wor
-00002110: 6b73 6865 6574 732f 7368 6565 7432 2e78  ksheets/sheet2.x
-00002120: 6d6c 9c94 5d6f da30 1486 ef27 ed3f 44be  ml..]o.0...'.?D.
-00002130: 2789 9310 6844 a8d6 5568 95a6 aa6a f771  '...hD..Uh...j.q
-00002140: 6d9c 1362 11c7 996d 0a74 da7f df71 1228  m..b...m.t...q.(
-00002150: 1352 c51a 8163 92e3 e7bc e78b d9f5 4ed6  .R...c........N.
-00002160: de33 6823 5493 13ea 87c4 8386 ab42 34ab  .3h#T........B4.
-00002170: 9c7c ffb6 184d 8967 2c6b 0a56 ab06 72b2  .|...M.g,k.V..r.
-00002180: 0743 aee7 1f3f ccb6 4aaf 4d05 603d 2434  .C...?..J.M.`=$4
-00002190: 2627 95b5 6d16 0486 5720 99f1 550b 0dbe  &'..m...W ..U...
-000021a0: 2995 96cc e24f bd0a 4cab 8115 dd21 5907  )....O..L....!Y.
-000021b0: 5118 a681 64a2 213d 21d3 9730 5459 0a0e  Q...d.!=!..0TY..
-000021c0: b78a 6f24 34b6 8768 a899 45fd a612 ad39  ..o$4..h..E....9
-000021d0: d024 bf04 2799 5e6f da11 57b2 45c4 52d4  .$..'.^o..W.E.R.
-000021e0: c2ee 3b28 f124 cfee 568d d26c 5963 dc3b  ..;(.$..V..lYc.;
-000021f0: 9a30 eeed 347e 22fc c607 37dd f333 4f52  .0..4~"...7..3OR
-00002200: 70ad 8c2a ad8f e4a0 d77c 1efe 5570 1530  p..*.....|..Up.0
-00002210: 7e24 9dc7 7f11 8626 8186 67e1 0af8 8a8a  ~$.....&..g.....
-00002220: de27 898e 8fac e815 16bf 1396 1e61 2e5d  .'...........a.]
-00002230: 3adb 8822 27bf c3e1 1ae1 9dba 251c 85d4  :.."'.......%...
-00002240: 2d27 d71f 329f 1502 2bec a2f2 3494 39f9  -'..2...+...4.9.
-00002250: 44b3 7b3a 21c1 7cd6 35d0 0f01 5b73 b2f7  D.{:!.|.5...[s..
-00002260: 5e94 924f 9cd5 70ef 3aae c65e 0eb1 975d  ^..O..p.:..^...]
-00002270: 972e 955a 3bf3 3bf4 1e22 b865 0d78 bba7  ...Z;.;..".e.x..
-00002280: 166b 8d56 c4db 0f5b 8cd8 aaf6 2b94 f633  .k.V...[....+..3
-00002290: d408 b841 d58c 5bf1 0c0f 7822 274b 65ad  ...A..[...x"'Ke.
-000022a0: 928f 6255 d96e 262c 3e2b b57a 81a6 5305  ..bU.n&,>+.z..S.
-000022b0: 35a0 31ca edcf 0c8c 319a feea 02b8 19ff  5.1.....1.......
-000022c0: 6be6 64e4 043d 0ec4 ff3a d66b 715a 0f1a  k.d..=...:.kqZ..
-000022d0: 2ff4 771a 04e6 3238 26f3 747f 48ec a21b  /.w...28&.t.H...
-000022e0: de07 ed15 50b2 4d6d 1fd5 f60b b8f8 316f  ....P.Mm......1o
-000022f0: 899f 6051 dd54 64c5 fe16 0cc7 71c4 fcfa  ..`Q.Td.....q...
-00002300: b18b 92ab 1a19 b87a 52b8 bf15 9c26 b6eb  .......zR....&..
-00002310: ee5b 51d8 2a27 d1d8 1f8f 9374 3a71 f9b1  .[Q.*'.....t:q..
-00002320: 7b37 6111 f2f8 c660 8a7f f636 7420 f50c  {7a....`...6t ..
-00002330: 2c46 c7c0 fbc0 a091 1fc7 5118 d308 214b  ,F........Q...!K
-00002340: 3076 3114 f40d 0ac5 9ee8 a5b8 e6e8 fd4c  0v1............L
-00002350: fde9 349d d053 2d93 37a5 50ec 941e 829b  ..4..S-.7.P.....
-00002360: 2324 4d93 3075 52ce dd07 5d3e fe02 0000  #$M.0uR...]>....
-00002370: ffff 0000 00ff ffcc 9c7d 73da 4610 87bf  .........}s.F...
-00002380: 8aa2 7832 a625 4602 fc1a cc0c a0d3 8b83  ..x2.%F.........
-00002390: a135 9066 dae9 308c 839b cc38 6e06 5c27  .5.f..0....8n.\'
-000023a0: f9f6 dd93 4ed2 dd21 e9de c0f8 8fc4 c9b1  ....N..!........
-000023b0: 8b9e 3b89 dddf ee1d eeac 3f2f 978f dee2  ..;.......?/....
-000023c0: 71d1 edac fefd 6ead 2e6d d7b6 d6df 160f  q.....n..m......
-000023d0: 6bf8 d785 dbb6 ad1f 6e7b 717b f1e9 a7b7  k.......n{q{....
-000023e0: 5cdf 2e1f 1e2f 6de7 a865 773b b7d8 b687  \..../m..ew;....
-000023f0: 8d2f eda6 0303 77d6 ed02 7b77 47fd f9ef  ./....w...{wG...
-00002400: 3334 9946 e3d1 a4d3 b8eb 769e ba6e a7f1  34.F......v..n..
-00002410: d4ed 346e 895b 3f71 83bf e1ed d6e0 0b16  ..4n.[?q........
-00002420: c7ac c920 3139 b31b c4c7 2397 72b3 11b4  ... 19....#.r...
-00002430: 31e2 6f8c 5c25 2327 f495 4ed8 2bbd 2f80  1.o.\%#'..N.+./.
-00002440: 3965 4d86 c404 cf3b 9be6 6476 7d38 f6fd  9eM....;..dv}8..
-00002450: 099a 1ea2 8fbf a1ba e5d4 adc1 7832 add5  ............x2..
-00002460: c8a4 9dec 4d1a b0b4 d9fa 3655 d617 1bc3  ....M.....6U....
-00002470: fa36 b9f5 f57b 8369 d9da 1217 32e5 c715  .6...{.i....2...
-00002480: ed1a f987 83f1 7076 3d3a ecb9 b537 ff3c  ......pv=:...7.<
-00002490: be83 7b35 1c5e 4fea 966d d7ad 7436 3fbe  ..{5.^O..m..t6?.
-000024a0: 2d5f 1df4 0edc ba15 a29e 876e e693 e84f  -_.........n...O
-000024b0: f46b eef8 165e 01af 398c 6493 8507 e6fb  .k...^..9.d.....
-000024c0: 72b5 feeb cbdf 47f7 f75f e7c9 7f8f eefe  r.....G.._......
-000024d0: bbbf 9f3f 2cbe 2eb9 9b2b c7d8 d765 04c7  ...?,....+...e..
-000024e0: 0246 7892 b227 d093 2318 e812 80a3 8000  .Fx..'..#.......
-000024f0: c911 78ba 04e0 2820 f0e5 0890 2e01 380a  ..x...( ......8.
-00002500: 0802 3902 5f97 001c 0504 a11c 41a0 4b00  ..9._.......A.K.
-00002510: 8e02 8248 8e20 d425 0047 01c1 5542 d06a  ...H. .%.G..UB.j
-00002520: 6691 f57d 32c2 c4e7 332e 2412 ecf3 38b2  f..}2...3.$...8.
-00002530: 2e6d ebf6 6b1c fc21 3e42 4c5f ac56 8b9f  .m..k..!>BL_.V..
-00002540: b6b5 4832 82b5 5ade 5dda 43f0 2019 62fe  ..H2..Z.].C. .b.
-00002550: e3fe eee1 e8ba f731 f227 4c0c 75ea 68e4  .......1.'L.u.h.
-00002560: cdbd de14 d5ea 5616 8f70 7465 5eb1 dfdc  ......V..pte^...
-00002570: 3fbe c3e1 cbae 596f 2df2 6ed1 c8fc dd48  ?.....Yo-.n....H
-00002580: e47e fda1 379c a157 ec8c afc9 32d1 abd2  .~..7..W....2...
-00002590: 6eb1 36a3 6c55 2a12 8553 f766 373d 9c1e  n.6.lU*..S.f7=..
-000025a0: 6bb5 c6d9 49db 8144 1167 c992 84d1 5249  k...I..D.g....RI
-000025b0: 18d8 1812 06fc c853 eb39 977d 139b c464  .......S.9.}...d
-000025c0: 19a7 8792 5bd6 071b 72cb 2073 f40f 9a97  ....[...r. s....
-000025d0: 384d e03f bd0f e8a6 1720 18e5 5360 9a18  8M.?..... ..S`..
-000025e0: ea16 d8e7 3925 cd90 f9d4 d334 f9da 8b3e  ....9%.....4...>
-000025f0: 341c 6eb1 0734 e39a 24b1 124a 6c9b 530e  4.n..4..$..Jl.S.
-00002600: 1429 c15e 8292 c91d 0a6c 1ec3 e629 b281  .).^.....l...)..
-00002610: bd22 1b52 60c3 b6f9 ba21 4536 b057 64f3  .".R`....!E6.Wd.
-00002620: 15d8 b06d cee6 2bb2 81bd 225b a0c0 866d  ...m..+..."[...m
-00002630: 73b6 4091 0dec 15d9 4205 366c 9bb3 858a  s.@.....B.6l....
-00002640: 6c60 afc8 1629 b061 db9c 2d52 6403 7b45  l`...).a..-Rd.{E
-00002650: b62b c2e6 e0bc c648 70a8 6ae4 4b1c 6ccc  .+.....Hp.j.K.l.
-00002660: 45d4 661e a9e3 32a8 9fd8 b4e0 07c4 2899  E.f...2.......(.
-00002670: 6488 3db6 1c59 93da e317 d771 aa23 2bc3  d.=..Y.....q.#+.
-00002680: 8a43 ab38 750f 18da ad44 d80d 5a26 c26a  .C.8u....D..Z&.j
-00002690: 307a 0ce3 5622 6d25 23d2 60c4 3e5b 8eb8  0z..V"m%#.`.>[..
-000026a0: 958c be06 23f6 d972 e4ad 640c 3418 b1cf  ....#..r..d.4...
-000026b0: 9623 7025 63a8 c188 7db6 1c89 2b19 a384  .#p%c...}...+...
-000026c0: 3109 4102 c584 6db7 1c89 1336 1279 e8cf  1.A...m....6.y..
-000026d0: f215 59bb cd28 7cac 1285 b171 1c85 d37e  ..Y..(|....q...~
-000026e0: 503f 1939 ce8a 9601 3fe0 f103 881f f0f9  P?.9....?.......
-000026f0: 8180 1f08 f981 881f b84a 065a 9bf3 830e  .........J.Z....
-00002700: 8c7c 96c1 c67c 96e1 bb66 890d 3563 7ec0  .|...|...f..5c~.
-00002710: e307 103f e0f3 0301 3f10 f203 1135 c064  ...?....?....5.d
-00002720: d153 95f9 6163 be2e 6973 7509 b139 e33a  .S..ac..isu..9.:
-00002730: 5674 dd01 4d37 aae6 881b 557d ae51 95f5  Vt..M7....U}.Q..
-00002740: a6ea 1674 b76e c67f 4ca0 9664 6a91 12b7  ...t.n..L..dj...
-00002750: b037 1cce a015 967a 1534 f2e2 6c3f c838  .7.....z.4..l?.8
-00002760: e31a 6bb3 c346 291b 5d5e a62a 51e4 6532  ..k..F).]^.*Q.e2
-00002770: a980 95ce 93ba ac4c 9562 c08a 04ac 7485  .......L.b....t.
-00002780: a2cb ca54 2d06 acbe 8095 ae58 7459 992a  ...T-......XtY.*
-00002790: c680 3510 b0d2 158c 2e2b 53d5 18b0 8602  ..5......+S.....
-000027a0: 56ba a2d1 6565 aa1c 03d6 48c0 4a57 38ba  V...ee....H.JW8.
-000027b0: ac4c d5a3 c7ca c4ec 3395 988d 8dd9 9c4b  .L......3......K
-000027c0: 464e d3a6 d1fa f362 b5fc 6427 0dbe fed9  FN.....b..d'....
-000027d0: 4504 06a4 e7b7 fe02 3b45 7697 eb1b f54f  E.......;Ev....O
-000027e0: 1bf4 f6d0 e656 4912 61b3 ebd0 1116 37b4  .....VI.a.....7.
-000027f0: c8f5 986b 40bc 7b62 629e 9137 32f2 f68d  ...k@.{bb..72...
-00002800: bc03 23ef d0c8 1bdf 3a7c b7e1 a1c6 0b9d  ..#.....:|......
-00002810: b7dc 446b ce3c 5fd0 0e96 d73c d898 d73c  ..Dk.<_....<...<
-00002820: 4d4e 1310 9b2a 4d30 18cf 4653 baf7 bb5b  MN...*M0..FS...[
-00002830: 5900 1b7d a5ca 20a3 152b 0303 6a1d 7140  Y..}.. ..+..j.q@
-00002840: 5133 9f15 0131 ad0f 0c88 7524 4209 3112  Q3...1....u$B.1.
-00002850: 10d3 2ac1 8058 4728 9410 fb02 625a 2b18  ..*..XG(....bZ+.
-00002860: 10eb c885 12e2 4040 4c2b 0603 621d d150  ......@@L+..b..P
-00002870: 421c 0a88 69dd 6040 ac23 1d4a 8823 0131  B...i.`@.#.J.#.1
-00002880: ad1e 0c88 7504 c426 3113 e35d 4725 c8c7  ....u..&1..]G%..
-00002890: d6ac 8a48 874a 6484 eb5c 44d8 844a f270  ...H.Jd..\D..J.p
-000028a0: aa84 1712 e752 4222 bf94 38ab c527 4b58  .....RB"..8..'KX
-000028b0: 2561 e68e ccdc 7d33 f7c0 cc3d 3473 8fef  %a....}3...=4s..
-000028c0: a0ac 9e60 569e 7dd6 d44e 2391 f33f d0f8  ...`V.}..N#..?..
-000028d0: cf76 3f9b dc16 6ddf 2546 a457 4f6d d40a  .v?...m.%F.WOm..
-000028e0: f738 b72b 2c10 ec32 cf7b b3e9 b8a0 e550  .8.+,..2.{.....P
-000028f0: bc29 caa0 a712 4d76 eb53 1e5e 465f 54c0  .)....Mv.S.^F_T.
-00002900: 33fa 4280 5cdd a797 4796 1118 92c8 4880  3.B.\...G.....H.
-00002910: 5cbd 512a 8f2c a330 2491 7d01 72f5 fea9  \.Q*.,.0$.}.r...
-00002920: 3cb2 8cc4 9044 0e04 c8d5 dbaa f2c8 321a  <....D........2.
-00002930: 4312 3914 2057 efb6 ca23 cb88 0c49 e448  C.9. W...#...I.H
-00002940: 805c bd09 2b8f 2ca3 32c4 c86c e4c7 4769  .\..+.,.2..l..Gi
-00002950: e4cf a192 8337 f884 e653 97df 9e75 9357  .....7...S...u.W
-00002960: 8f2b 1acb 3b2e 220b 265f 5547 66c0 7baf  .+..;.".&_UGf.{.
-00002970: 23ab c1d9 509f ae72 31f4 3396 92f2 d048  #...P..r1.3....H
-00002980: b0d2 cf58 4dca 43fb 02e8 672c 28e5 a103  ...XM.C...g,(...
-00002990: 01f4 33d6 94f2 d0a1 00fa 19cb 4a79 e848  ..3.........Jy.H
-000029a0: 00fd 8c95 a514 341b f6f1 a11d f9b0 9f1c  ......4.........
-000029b0: f181 e38e d9b6 b04b 86ca 8acb 1614 97d9  .......K........
-000029c0: 4124 0b77 a9e1 703d 5f5c ba4d b9ea 32bb  A$.w..p=_\.M..2.
-000029d0: 96b8 ba8c 4fd7 72d5 a591 3bca 67aa 7375  ....O.r...;.g.su
-000029e0: dfcc 3d30 730f cddc e35b 285b 5d32 2bcf  ..=0s....[([]2+.
-000029f0: 3e6c f86c 82fc c396 9c64 60ce d636 f93d  >l.l.....d`..6.=
-00002a00: 6cfc 8d19 007b 6952 c3c6 a7a5 1d38 b8cb  l....{iR.....8..
-00002a10: 7ec9 6373 efbc f013 1b9f b776 edd2 b677  ~.cs.......v...w
-00002a20: 36e9 9729 57b6 3a79 56f2 a477 fb65 4a9e  6..)W.:yV..w.eJ.
-00002a30: 9d4d 1c09 eef8 be65 d3ce 26ee 0b26 be6f  .M.....e..&..&.o
-00002a40: e9b5 b389 0782 89ef 5bbe ed6c e2a1 60e2  ........[..l..`.
-00002a50: fb96 803b 9b78 2498 f8be 65e4 2e26 ceaa  ...;.x$...e..&..
-00002a60: 03a5 038a eee6 09c5 74a8 4c8a 1e83 1405  ........t.L.....
-00002a70: 2f6a 9f03 da17 1b52 b42d 2745 c9e5 65b6  /j.....R.-'E..e.
-00002a80: ef63 b5cc 4951 2377 94cf 542c 4537 afee  .c..IQ#w..T,E7..
-00002a90: 9bb9 0766 eea1 997b 7c0b 65a5 2833 77f6  ...f...{|.e.(3w.
-00002aa0: 6153 3a2d ea66 c745 0bbf 5d9d 9ed8 2cdf  aS:-.f.E..]...,.
-00002ab0: dbd8 47bb cb2d d78f 29f0 cbd4 8f19 38ab  ..G..-..).....8.
-00002ac0: fdaa a1f7 ddee 2a84 46e4 c181 4f3b 75c8  ......*.F...O;u.
-00002ad0: a7f8 2b09 3b3e 3c51 5868 1442 fb02 e87d  ..+.;><QXh.B...}
-00002ae0: 6bae 42e8 4000 bd6f bd54 081d 0aa0 f7ad  k.B.@..o.T......
-00002af0: 750a a123 01f4 be75 0a0f cd86 7dfa 103d  u..#...u....}..=
-00002b00: 9c08 a9fe 651b d921 fabc db45 86ca 24c6  ....e..!...E..$.
-00002b10: 2948 0c30 a124 46bb 4062 9cc8 498c ec5a  )H.0.$F.@b..I..Z
-00002b20: e224 dfc6 0d39 4e62 18b9 233c 0dd9 34bb  .$...9Nb..#<..4.
-00002b30: 7975 dfcc 3d30 730f cddc e35b a835 f7e4  yu..=0s....[.5..
-00002b40: 596b e4bf e4e5 7f00 0000 ffff 0000 00ff  Yk..............
-00002b50: ff44 8c41 0e82 3010 45af d2cc 0144 1125  .D.A..0.E....D.%
-00002b60: 3594 951b 17ae 3841 0d43 3b51 3bcd 3086  5.....8A.C;Q;.0.
-00002b70: 84d3 0b26 c4dd 7fef 27af c93e e0dd 4ba0  ...&....'..>..K.
-00002b80: 349a 170e ea60 bfab c108 85b8 6de5 fcb3  4....`......m...
-00002b90: 2730 0f56 e5f7 4611 7d8f b2d2 11cc c0ac  '0.V..F.}.......
-00002ba0: 1b14 6db3 763b d44f 36d9 6794 8e66 7460  ..m.v;.O6.g..ft`
-00002bb0: c1b0 1026 f54a 9c1c 6416 154f 0a26 2e7e  ...&.J..d..O.&.~
-00002bc0: e6e5 785d 3339 a84a 5bd9 735d da25 2c17  ..x]39.J[.s].%,.
-00002bd0: ea1d c8ad 3fc0 d2ed c54f 94c2 df96 ab2d  ....?....O.....-
-00002be0: 2696 e718 11b5 fd02 0000 ffff 0300 504b  &.............PK
-00002bf0: 0304 1400 0600 0800 0000 2100 b590 2cdd  ..........!...,.
-00002c00: b704 0000 690f 0000 1800 0000 786c 2f77  ....i.......xl/w
-00002c10: 6f72 6b73 6865 6574 732f 7368 6565 7433  orksheets/sheet3
-00002c20: 2e78 6d6c 9c93 df6b db30 10c7 df07 fb1f  .xml...k.0......
-00002c30: 84de 6349 4eda 3526 4e19 94d0 421f c658  ..cIN.5&N...B..X
-00002c40: bb67 453e c722 9664 24b9 4918 fbdf 7752  .gE>.".d$.I...wR
-00002c50: 9a74 9097 5023 eb87 effc b93b dfd7 8bfb  .t..P#.....;....
-00002c60: bde9 c91b f8a0 9dad a928 3825 6095 6bb4  .........(8%`.k.
-00002c70: ddd4 f4e5 d76a 7247 4988 d236 b277 166a  .....jrGI..6.w.j
-00002c80: 7a80 40ef 975f bf2c 76ce 6f43 0710 0912  z.@.._.,v.oC....
-00002c90: 6ca8 6917 e350 3116 5407 4686 c20d 60d1  l.i..P1.T.F...`.
-00002ca0: d23a 6f64 c4a3 dfb0 3078 904d 7ec9 f4ac  .:od....0x.M~...
-00002cb0: e4fc 9619 a92d 3d12 2a7f 0dc3 b5ad 56f0  .....-=.*.....V.
-00002cc0: e0d4 68c0 c623 c443 2f23 e61f 3a3d 8413  ..h..#.C/#..:=..
-00002cd0: cda8 6b70 46fa ed38 4c94 3303 22d6 bad7  ..kpF..8L.3."...
-00002ce0: f190 a194 1855 3d6d acf3 72dd 63dd 7b31  .....U=m..r.c.{1
-00002cf0: 938a ec3d 8e12 efe9 294c 7e7e 11c9 68e5  ...=....)L~~..h.
-00002d00: 5d70 6d2c 90cc 8e39 5f96 3f67 7326 d599  ]pm,...9_.?gs&..
-00002d10: 7459 ff55 1831 631e de74 6ae0 07aa fc5c  tY.U.1c..tj....\
-00002d20: 4ae2 e6cc 2a3f 60d3 4fc2 6ecf b0f4 b97c  J...*?`.O.n....|
-00002d30: 35ea a6a6 7ff8 fb35 c155 a489 4f38 6a21  5......5.U..O8j!
-00002d40: ef4e b6bf 74b9 6834 7638 5545 3cb4 35fd  .N..t.h4v8UE<.5.
-00002d50: 2eaa 6771 47d9 7291 05f4 aa61 17fe db93  ..gqG.r....a....
-00002d60: a4c7 b573 db64 78c2 383c b9b2 0bdf 55d6  ...s.dx.8<....U.
-00002d70: e30f 4f1a 68e5 d8c7 9f6e f708 7ad3 4514  ..O.h....n..z.E.
-00002d80: ffac 9861 9ea9 d155 7378 80a0 5061 082a  ...a...Usx..Pa.*
-00002d90: a609 a55c 8ff1 7026 46a7 3f05 0522 f779  ...\..p&F.?..".y
-00002da0: dde9 2676 352d 7921 f87c faed 8692 3584  ..&v5-y!.|....5.
-00002db0: b8d2 0949 891a 4374 e6f7 d147 e4a4 32ea  ...I..Ct...G..2.
-00002dc0: 1f00 0000 ffff 0000 00ff ff9c 566d 8f9a  ............Vm..
-00002dd0: 4010 fe2b 5b7a b940 4b8a abf8 76a7 2680  @..+[z.@K...v.&.
-00002de0: 18ad 28a9 627a e997 0b45 bc4b 6a4f 839c  ..(.bz...E.KjO..
-00002df0: 77fe fbce b2ca b2ab 56f7 fc24 b3c3 3c33  w.......V..$..<3
-00002e00: cf0c cf6c 6bf3 1cc7 6937 4cc3 4e2b 59bd  ...lk...i7L.N+Y.
-00002e10: a1a4 ad60 056d d6e1 cb06 fedd e1b2 82de  ...`.m..........
-00002e20: b119 4677 f35d 37de 44f1 4bda 564a df2a  ..Fw.]7.D.K.VJ.*
-00002e30: 4aa7 1511 5f0b 9cc1 b281 e76d a75c 6d19  J..._......m.\m.
-00002e40: db4e cb88 f687 36a6 66de dae5 5ea9 f187  .N....6.f...^...
-00002e50: 0302 de56 ca55 1a36 4d20 c2a2 a338 abbf  ...V.U.6M ...8..
-00002e60: ebd7 349e a328 5e2e 37e8 39dc c628 443b  ..4..(^.7.9..(D;
-00002e70: 7880 947f 87d1 9fa7 64f5 fa32 575a c682  x.......d..2WZ..
-00002e80: 2472 a53b 0ffd 3d87 36f6 f90f 8f2c 5ed1  $r.;..=.6....,^.
-00002e90: 6200 5f39 69c0 d3f5 a481 3323 ad2e 9056  b._9i.....3#...V
-00002ea0: ce48 c302 69dc 2b8d fc90 cba1 2293 0338  .H..i.+....."..8
-00002eb0: b31c 9a42 0ea4 bfd0 cfd3 30a6 0c0c 38e7  ...B......0...8.
-00002ec0: 3095 9200 6366 3095 d330 3002 d733 ba9f  0...cf0..00..3..
-00002ed0: 171a 4fe0 ceae 6666 5623 475a 4d06 069c  ..O...ffV#GZM...
-00002ee0: 5935 8c9e ec53 b06b b471 ac48 0ea7 2e83  Y5...S.k.q.H....
-00002ef0: 03ce 0c87 f143 71ea 1487 55c9 e134 6470  .....Cq...U..4dp
-00002f00: c039 c731 4da1 3b0d 8a73 660a 9a32 38e0  .9.1M.;..sf..28.
-00002f10: cc70 4495 6852 9c33 6380 4b52 7204 de8c  .pD.hR.3c.KRr...
-00002f20: 39b1 2288 45e6 1a33 3b47 1d96 53be a28e  9.".E..3;G..S...
-00002f30: 558e a48f 6a1f 6676 1e4a 4a2f 880a b3aa  U...j.fv.JJ/....
-00002f40: 04c9 b4e1 34ab 8ad9 7928 2959 c045 5da8  ....4...y()Y.E].
-00002f50: 1d55 4585 0133 cde2 a1a4 a401 73da 20ca  .UE..3......s. .
-00002f60: 2039 a59b 0036 008a 42b2 973a 8e3f 1b07   9...6..B..:.?..
-00002f70: 96ea f77a 5337 50dd f775 fce9 c6ba c13a  ...zS7P..u.....:
-00002f80: eabb 56d7 9d3c 4e07 bf5c 1d79 dee8 d1f1  ..V..<N..\.y....
-00002f90: 3d1d d99e ef0c f746 ac69 fbed 70e6 c3c1  =......F.i..p...
-00002fa0: 5282 43bc 594b 9820 d34f 348b 95ad b12b  R.C.YK. .O4....+
-00002fb0: 922f e6fe 63e6 4e83 813f a6f9 e352 f6d3  ./..c.N..?...R..
-00002fc0: d1e5 e4a5 640c 733a 268a 3f39 bd9a f962  ....d.s:&.?9...b
-00002fd0: f23d cb09 a413 2fea e2c5 cb46 5117 4d71  .=..../....FQ.Mq
-00002fe0: 9b60 122a bf3b c4e4 e640 5a14 2649 b853  .`.*.;...@Z.&I.S
-00002ff0: 5048 4708 25f1 a2ad d8c4 773f 5323 2b70  PHG.%.....w?S#+p
-00003000: fa6a 3099 c1e4 8cfd 401d 4c6d cf1a 0f8f  .j0.....@.Lm....
-00003010: 87ac 50ea 57ac 9fef 94a6 a3d2 61d6 3e8f  ..P.W.......a.>.
-00003020: 0deb f47a c345 a1be 5838 27d4 e27e cb42  ...z.E..X8'..~.B
-00003030: e5d3 76b6 6488 9197 fca0 8eac 07f5 bf35  ..v.d..........5
-00003040: ea4e 7f36 1e66 fda4 73a8 63ed 7699 dedf  .N.6.f..s.c.v...
-00003050: 3ea5 f78a a2a1 2f48 9df8 3fa5 4368 1af0  >...../H..?.Ch..
-00003060: 7319 3c9f a50f 631f 47b8 12fa 201f 1f46  s.<...c.G... ..F
-00003070: 3e0a 00c0 8781 10b7 9cc1 eedf ff00 0000  >...............
-00003080: ffff 0000 00ff ffb2 2948 4c4f f54d 2c4a  ........)HLO.M,J
-00003090: cfcc 2b56 c849 4d2b b155 32d0 3357 5228  ..+V.IM+.U2.3WR(
-000030a0: ca4c cf80 b14b f20b c0a2 a64a 0a49 f925  .L...K.....J.I.%
-000030b0: 25f9 b930 5e46 6a62 4a6a 1188 67ac a490  %..0^FjbJj..g...
-000030c0: 969f 5f02 e3e8 dbd9 e897 e717 6517 67a4  .._.........e.g.
-000030d0: a696 d801 0000 00ff ff03 0050 4b03 0414  ...........PK...
-000030e0: 0006 0008 0000 0021 00b1 450d ec5c 0700  .......!..E..\..
-000030f0: 0002 2100 0013 0000 0078 6c2f 7468 656d  ..!......xl/them
-00003100: 652f 7468 656d 6531 2e78 6d6c ec59 4b8f  e/theme1.xml.YK.
-00003110: 1b37 12be 07c8 7f20 fa2e ebd5 adc7 c0b2  .7..... ........
-00003120: a1a7 27f6 8c6d 7864 2f72 e448 949a 1e76  ..'..mxd/r.H...v
-00003130: 5320 a919 0b81 81c0 39e5 1220 4076 b197  S ......9.. @v..
-00003140: 05f6 b687 2048 8004 5823 97fc 1803 36b2  .... H..X#....6.
-00003150: d91f b145 764b 4d8e a878 6c8f 174e 3033  ...EvKM..xl..N03
-00003160: c08c 9afa aa58 ac2a 7eac 2e5e bff9 2461  .....X.*~..^..$a
-00003170: e894 0849 79da 09aa d72a 0122 e984 4f69  ...Iy....*."..Oi
-00003180: 3aef 040f c7a3 522b 4052 e174 8a19 4f49  :.....R+@R.t..OI
-00003190: 2758 1119 dcbc f1f1 47d7 f19e 8a49 4210  'X......G....IB.
-000031a0: c8a7 720f 7782 58a9 c55e b92c 2730 8ce5  ..r.w.X..^.,'0..
-000031b0: 35be 2029 7c37 e322 c10a 1ec5 bc3c 15f8  5. )|7.".....<..
-000031c0: 0cf4 26ac 5cab 541a e504 d334 4029 4e40  ..&.\.T....4@)N@
-000031d0: edbd d98c 4e08 aa55 aa75 5482 7fb5 1a1a  ....N..U.uT.....
-000031e0: 6bf5 c18d f544 4306 8fa9 927a 60c2 c491  k....DC....z`...
-000031f0: 9e86 ec94 3672 d393 aa46 cb95 ec33 814e  ....6r...F...3.N
-00003200: 31eb 0430 ff94 9f8d c913 1520 86a5 822f  1..0....... .../
-00003210: 3a41 c5fc 04e5 1bd7 cb78 2f17 626a 87ac  :A.......x/.bj..
-00003220: 2537 323f b95c 2e30 3da9 9939 c5fc 7833  %72?.\.0=..9..x3
-00003230: 6918 4661 a3bb d16f 004c 6de3 86cd 6163  i.Fa...o.Lm...ac
-00003240: d8d8 e833 003c 99c0 aa33 5b5c 9dcd 5a3f  ...3.<...3[\..Z?
-00003250: ccb1 1628 fbe8 d13d 680e ea55 076f e9af  ...(...=h..U.o..
-00003260: 6fd9 dc8d f4af 8337 a04c 7fb8 851f 8dfa  o......7.L......
-00003270: e045 076f 4019 3eda c247 bd76 6fe0 ea37  .E.o@.>..G.vo..7
-00003280: a00c dfd8 c237 2bdd 41d8 74f4 1b50 cc68  .....7+.A.t..P.h
-00003290: 7ab2 85ae 448d 7a7f bdda 0d64 c6d9 be17  z...D.z....d....
-000032a0: de8e c251 b396 2b2f 5090 0d9b 4cd3 53cc  ...Q..+/P...L.S.
-000032b0: 78aa 2e92 7709 7ecc c508 c05a 8861 4553  x...w.~....Z.aES
-000032c0: a456 0b32 c313 c8f4 3e66 f458 5074 40e7  .V.2....>f.XPt@.
-000032d0: 3124 e102 a75c c270 a556 1955 eaf0 57ff  1$...\.p.V.U..W.
-000032e0: 86e6 9389 2ede 23d8 92d6 3682 5572 6b48  ......#...6.UrkH
-000032f0: db86 e444 d085 ea04 b741 6b60 415e 3e7f  ...D.....Ak`A^>.
-00003300: fee2 d94f 2f9e fdfb c517 5fbc 78f6 7d3e  ...O/....._.x.}>
-00003310: b751 e5c8 ede3 746e cbfd f6af afff fb8f  .Q....tn........
-00003320: cfd1 7f7e fce7 6fdf fc35 9bfa 3c5e daf8  ...~..o..5..<^..
-00003330: 57df 7df9 eae7 5f7e 4f3d acb8 70c5 cbbf  W.}..._~O=..p...
-00003340: fdf0 eaa7 1f5e fefd ab5f bffd c6a3 bd2b  .....^..._.....+
-00003350: f0b1 0d1f d384 4874 979c a107 3c81 057a  ......Ht....<..z
-00003360: ec27 c7e2 cd24 c631 a68e 048e 41b7 47f5  .'...$.1....A.G.
-00003370: 50c5 0ef0 ee0a 331f ae47 5c17 3e12 c038  P.....3..G\.>..8
-00003380: 3ee0 ade5 63c7 d6a3 582c 15f5 cc7c 274e  >...c...X,...|'N
-00003390: 1ce0 21e7 acc7 85d7 0177 f45c 9687 c7cb  ..!......w.\....
-000033a0: 74ee 9f5c 2c6d dc03 8c4f 7d73 f771 ea04  t..\,m...O}s.q..
-000033b0: 78b8 5c00 ed52 9fca 7e4c 1c33 ef33 9c2a  x.\..R..~L.3.3.*
-000033c0: 3c27 2951 487f c74f 08f1 acee 534a 1dbf  <')QH..O....SJ..
-000033d0: 1ed2 89e0 92cf 14fa 94a2 1ea6 5e97 8ce9  ............^...
-000033e0: b193 4885 d03e 4d20 2e2b 9f81 106a c737  ..H..>M .+...j.7
-000033f0: 878f 508f 33df aa07 e4d4 45c2 b6c0 cc63  ..P.3.....E....c
-00003400: fc98 30c7 8db7 f052 e1c4 a772 8c13 663b  ..0....R...r..f;
-00003410: fc00 abd8 67e4 d14a 4c6c dc50 2a88 f49c  ....g..JLl.P*...
-00003420: 308e 8653 22a5 4fe6 9e80 f55a 41bf 030c  0..S".O....ZA...
-00003430: e30f fb21 5b25 2e52 287a e2d3 7980 39b7  ...![%.R(z..y.9.
-00003440: 9103 7ed2 8f71 b2f0 da4c d3d8 c67e 224f  ..~..q...L...~"O
-00003450: 2045 31ba cf95 0f7e c8dd 1da2 9f21 0e38   E1....~.....!.8
-00003460: dd19 ee47 9438 e17e 3d11 3c04 72b5 4d2a  ...G.8.~=.<.r.M*
-00003470: 1244 7fb3 149e 58de 22dc dd8f 2b36 c3c4  .D....X."...+6..
-00003480: c732 5d91 38ec da15 d49b 1dbd e5dc 49ed  .2].8.........I.
-00003490: 0342 183e c353 42d0 c34f 3c16 f4f8 c2f1  .B.>.SB..O<.....
-000034a0: 7961 f4ed 1858 659f f812 eb36 7673 553f  ya...Xe....6vsU?
-000034b0: a744 1264 6a9c 6d8a 3ca0 d249 d923 32e7  .D.dj.m.<..I.#2.
-000034c0: 3bec 395c 9d23 9e15 4e13 2c76 69be 0b51  ;.9\.#..N.,vi..Q
-000034d0: 7752 174e 392f 95de 6393 131b 7897 4289  wR.N9/..c...x.B.
-000034e0: 08f9 e275 ca3d 093a ace4 1eee d27a 3fc6  ...u.=.:.....z?.
-000034f0: ced9 a59f a53f 5f57 c289 df45 f618 eccb  .....?_W...E....
-00003500: c76f ba2f 4186 bcb1 0c10 fb85 7d33 c6cc  .o./A.......}3..
-00003510: 99a0 4898 3186 02c3 47b7 20e2 84bf 10d1  ..H.1...G. .....
-00003520: e7aa 115b 7ae5 66ee a62d c200 4592 53ef  ...[z.f..-..E.S.
-00003530: 2434 7d6d f173 aeec 89fe 3f65 8fbf 80b9  $4}m.s....?e....
-00003540: 8482 c7af f85d 4a9d 5d94 b27f aec0 d985  .....]J.].......
-00003550: fb03 9635 03bc 4cef 1338 49b6 39eb aaaa  ...5..L..8I.9...
-00003560: b9aa 6a82 3f7d 55b3 6b2f 5fd5 3257 b5cc  ..j.?}U.k/_.2W..
-00003570: 552d e37b fb7a 2fb5 4c51 be40 6553 747c  U-.{.z/.LQ.@eSt|
-00003580: 4cff 27b9 50fb 6746 193b 522b 460e a4e9  L.'.P.gF.;R+F...
-00003590: 0049 78bb 998e 60d0 b4a9 4cdf 72d3 1a5c  .Ix...`...L.r..\
-000035a0: c4f0 316f 3c39 b8b9 c046 0609 aefe 4255  ..1o<9...F....BU
-000035b0: 7c14 e305 b489 aaa6 b139 97b9 eab9 440b  |........9....D.
-000035c0: 2ea1 7b64 864d eb95 9cd3 6d7a 50cb e490  ..{d.M....mzP...
-000035d0: 4fb3 0e68 b5aa bb9d 993b 2556 c578 25da  O..h.....;%V.x%.
-000035e0: 8c43 c74a 65e8 46b3 e8ea 6dd4 9b3e e9dc  .C.Je.F...m..>..
-000035f0: 7462 d706 68d9 3731 c29a cc35 a2ee 31a2  tb..h.71...5..1.
-00003600: b91e 8488 fc9e 1166 6597 6245 db63 454b  .......fe.bE.cEK
-00003610: ab5f 876a 1dc5 8d2b c0b4 4d54 e0f5 1bc1  ._.j...+..MT....
-00003620: 4b7b 2788 c2ac b30c 8d39 28d5 a73a 4e59  K{'......9(..:NY
-00003630: 9379 1d5d 1d9c 4b8d f42e 6732 3b03 a0dc  .y.]..K...g2;...
-00003640: 5e67 4011 e9b6 b675 e7f2 f4ea b254 bb40  ^g@....u.....T.@
-00003650: a41d 23ac 7473 8db0 d230 8697 e23c 3bed  ..#.ts...0...<;.
-00003660: 56fc 65c6 ba5d 84d4 314f bb62 bd1b 0a33  V.e..]..1O.b...3
-00003670: 9aad f711 6b4d 28e7 b881 a536 53b0 149d  ....kM(....6S...
-00003680: 7582 463d 825b 9809 5e74 8219 748f e163  u.F=.[..^t..t..c
-00003690: b280 dc91 fa0d 0cb3 395c d34c 94c8 36fc  ........9\.L..6.
-000036a0: db30 cb42 4835 c032 ce1c 6e48 2763 8384  .0.BH5.2..nH'c..
-000036b0: 2a22 10a3 4927 d0cb df64 034b 0d87 18db  *"..I'...d.K....
-000036c0: aa35 2084 0fd6 b836 d0ca 8766 1c04 dd0d  .5 ....6...f....
-000036d0: 3299 cdc8 44d9 61b7 46b4 a7b3 4760 f88c  2...D.a.F...G`..
-000036e0: 2bbc df1a f1b7 076b 49be 8470 1fc5 d333  +......kI..p...3
-000036f0: 74cc 96e2 0186 148b 9a55 edc0 2995 7089  t........U..).p.
-00003700: 50cd bc39 a570 43b6 21b2 22ff ce1d 4c39  P..9.pC.!."...L9
-00003710: edda 5754 2687 b271 cc16 31ce 4f14 9bcc  ..WT&..q..1.O...
-00003720: 33b8 21d1 8d39 e669 e303 eb29 5f33 3874  3.!..9.i...)_38t
-00003730: db85 c773 7dc0 bef3 a9fb faa3 5a7b ce22  ...s}.......Z{."
-00003740: cde2 cc74 5845 9f9a 7e32 7d7f 87bc 6555  ...tXE..~2}...eU
-00003750: 7188 3a56 65d4 6dde af65 c175 ed35 d741  q.:Ve.m..e.u.5.A
-00003760: a27a 4f89 d79c ba17 3810 2cd3 8ac9 1cd3  .zO.....8.,.....
-00003770: b4c5 db34 ac39 3b1f 754d bbc4 82c0 f244  ...4.9;.uM.....D
-00003780: 6387 df36 6784 d713 6f7b f283 dcf9 acd5  c..6g...o{......
-00003790: 07c4 bac6 3489 6fae d8ed 9b6f 7efc 18c8  ....4.o....o~...
-000037a0: 6300 7789 4ba6 a409 25dc 650b 0c45 5f76  c.w.K...%.e..E_v
-000037b0: 3399 d106 6c91 272a af11 e113 5a0a da09  3...l.'*....Z...
-000037c0: 3eab 44dd b05f 8bfa a54a 2b1a 96c2 7a58  >.D.._...J+...zX
-000037d0: 29b5 a26e bdd4 8da2 7a75 1855 2b83 5eed  )..n....zu.U+.^.
-000037e0: 291c 2c2a 4eaa 5176 bd3f 82eb 0cb6 ca2f  ).,*N.Qv.?...../
-000037f0: f9cd f8d6 457f b2be b1b9 36e1 4999 9b8b  ....E.....6.I...
-00003800: fcb2 31dc 5cf4 576b 17bb e847 1408 e8b3  ..1.\.Wk...G....
-00003810: 466d d4ae b77b 8d52 bbde 1d95 c241 af55  Fm...{.R.....A.U
-00003820: 6af7 1bbd d2a0 d16f 0e46 837e d46a 8f9e  j......o.F.~.j..
-00003830: 06e8 d480 c36e bd1f 3686 ad52 a3da ef97  .....n..6..R....
-00003840: c246 452f a5d5 2e35 c35a ad1b 36bb ad61  .FE/...5.Z..6..a
-00003850: d87d 9a97 34e0 858c 4a72 bf80 ab8d 8d37  .}..4...Jr.....7
-00003860: fe07 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00003870: 0800 0000 2100 d2e5 2255 4305 0000 481a  ....!..."UC...H.
-00003880: 0000 0d00 0000 786c 2f73 7479 6c65 732e  ......xl/styles.
-00003890: 786d 6ccc 59dd 6fe2 3810 7f3f e9fe 8728  xml.Y.o.8..?...(
-000038a0: adee e968 1220 69e1 08ab 8536 d24a dbaa  ...h. i....6.J..
-000038b0: 527b d249 d77b 0889 03d6 3a31 eb38 5dd8  R{.I.{....:1.8].
-000038c0: d3fd ef37 b613 30df d0a6 dde5 81c4 1f33  ...7..0........3
-000038d0: f3b3 673c 9e99 f43e cc52 623c 2396 639a  ..g<...>.Rb<#.c.
-000038e0: f9a6 7361 9b06 ca22 1ae3 6cec 9b7f 3e06  ..sa..."..l...>.
-000038f0: 8d2b d3c8 7998 c521 a119 f2cd 39ca cd0f  .+..y..!....9...
-00003900: fd5f 7fe9 e57c 4ed0 c304 216e 008b 2cf7  ._...|N...!n..,.
-00003910: cd09 e7d3 ae65 e5d1 04a5 617e 41a7 2883  .....e....a~A.(.
-00003920: 9184 b234 e4d0 6463 2b9f 3214 c6b9 204a  ...4..dc+.2... J
-00003930: 89d5 b46d cf4a 439c 998a 4337 8d8e 6192  ...m.JC...C7..a.
-00003940: 86ec 4b31 6d44 349d 861c 8f30 c17c 2e79  ..K1mD4....0.|.y
-00003950: 9946 1a75 3f8d 33ca c211 01a8 33a7 1d46  .F.u?.3.....3..F
-00003960: c6cc f158 d398 b14a 88ec dd90 93e2 88d1  ...X...J........
-00003970: 9c26 fc02 f85a 3449 7084 36e1 76ac 8e15  .&...Z4Ip.6.v...
-00003980: 464b 4ec0 f965 9c1c d7b2 9b2b 6b9f b117  FKN..e.....+k...
-00003990: 726a 5b0c 3d63 a13e b3df cb8a 3448 796e  rj[.=c.>....4Hyn
-000039a0: 44b4 c8b8 6f76 165d 861a f914 838e bdb6  D...ov.]........
-000039b0: 6928 ad0c 690c fb64 5fd8 bf7d 2d28 ffc3  i(..i..d_..}-(..
-000039c0: c8d5 d3b4 2a4e 2b64 ee06 995d 119e ef25  ....*N+d...]...%
-000039d0: f436 09d5 fcfd f22e 57c9 e2d8 4a53 6b0e  .6......W...JSk.
-000039e0: bf27 6332 e9a6 6937 cf77 2005 9bd5 17f8  .'c2..i7.w .....
-000039f0: 747e f6fb d919 2cd3 b677 1074 5609 14ba  t~....,..w.tV...
-00003a00: bb91 f1b5 4039 87ad cdbb 86ea dbc1 e012  ....@9..........
-00003a10: 8e8d 2e71 c120 0923 7e90 d859 25fe fbbc  ...q. .#~..Y%...
-00003a20: 11b4 6dfb 9f72 8d4f c6c7 5beb fe76 3bf2  ..m..r.O..[..v;.
-00003a30: cbe6 6ea5 449a 56ac d232 fabd 8466 4b03  ..n.D.V..2...fK.
-00003a40: 0195 caf3 d0fd 92d1 6f59 2086 c040 c06a  ........oY ..@.j
-00003a50: c4ac 7e2f ff6e 3c87 047a 1c21 3da2 8432  ..~/.n<..z.!=..2
-00003a60: 83c3 e906 a391 3d59 9822 3563 1812 3c62  ......=Y."5c..<b
-00003a70: 584c 4bc2 1493 b9ea 6e8a 0ee9 10ca 7929  XLK.....n.....y)
-00003a80: 86e3 293a 2d25 41fd 8fc4 ac77 92f5 9e6b  ..):-%A....w...k
-00003a90: c2ef b8ae f791 25d5 9683 9231 210b 37d3  ......%....1!.7.
-00003aa0: 1206 031d fd1e 7864 8e58 1640 c328 df1f  ......xd.X.@.(..
-00003ab0: e753 3097 0c2e 0fa5 7639 efc0 ec31 0be7  .S0.....v9...1..
-00003ac0: 4ed3 3d9e 20a7 04c7 02c5 7828 8d94 8d47  N.=. .....x(...G
-00003ad0: be19 c89f 3af3 a372 0067 319a 21f0 82e0  ....:..r.g1.!...
-00003ae0: 0485 156a 8085 4d4a 70f2 016b 1c51 16c3  ...j..MJp..k.Q..
-00003af0: c558 39d3 26f0 575d fd1e 4109 0772 86c7  .X9.&.W]..A..r..
-00003b00: 13f1 e474 0aff 23ca 395c 1efd 5e8c c331  ...t..#.9\..^..1
-00003b10: cd42 2204 5414 3a25 5ca8 7077 fa26 9fc0  .B".T.:%\.pw.&..
-00003b20: dd57 9dab 7564 42c4 4912 4a51 003c 4284  .W..udB.I.JQ.<B.
-00003b30: 3c08 117f 252b e867 89e6 cfa5 c7ca b8b8  <...%+.g........
-00003b40: 11c4 2bac bc7c 5548 5503 56b0 4224 fda4  ..+..|UHU.V.B$..
-00003b50: 2212 8e67 2791 a543 5080 342c 2d17 567d  "..g'..CP.4,-.V}
-00003b60: 3a18 6396 6c47 a52d 45b8 d2ed a816 d446  :.c.lG.-E......F
-00003b70: 389d 92b9 f075 a517 3b7d 8525 2fe9 0357  8....u..;}.%/..W
-00003b80: a8cb bbf5 d00e 2de8 1596 bb22 1d21 16c8  ......-....".!..
-00003b90: 4069 1b26 c793 576f cd5c b55d dbad cb13  @i.&..Wo.\.]....
-00003ba0: 911e a109 d050 a5c7 554d a8d6 401e ba6d  .....P..UM..@..m
-00003bb0: bb70 84c1 6ef0 3e8a dbc9 36a3 907e 2478  .p..n.>...6..~$x
-00003bc0: 9ca5 4899 51bf 0717 a06a 1a13 caf0 7730  ..H.Q....j....w0
-00003bd0: 2f71 7346 308e d810 5a38 2b68 2103 166b  /qsF0...Z8+h!..k
-00003be0: 96ec 36ff 5d60 8ede b6da c139 9e8c df0e  ..6.]`.....9....
-00003bf0: b98a 35ad 1eb6 6919 ded5 ce55 867e 8aeb  ..5...i....U.~..
-00003c00: d17a 5dc7 bacd 2e6b d4b6 e3d5 0f72 dd51  .z]....k.....r.Q
-00003c10: afc8 d8ed df4f 569a 660a 3fef f6d6 0f72  .....OV.f.?....r
-00003c20: 737b 35eb fd79 37a2 7e90 eb1b a139 e5d6  s{5..y7.~....9..
-00003c30: 6baf 5ec7 d3c2 8bf7 df54 19cc c9a0 709f  k.^......T....p.
-00003c40: 7f3e fa2c d5e9 3054 7af9 a3bc da71 1bf3  .>.,..0Tz....q..
-00003c50: 96b7 e88f 50cd c932 2188 d243 e7f5 2807  ....P..2!..C..(.
-00003c60: a2d2 0351 cddb c721 a6a8 f471 1c89 c804  ...Q...!...q....
-00003c70: 7296 edc6 ae1d 4251 28da 1b4d 03e4 bdd1  r.....BQ(..M....
-00003c80: b4ac 6cd4 1d0d 5f6a 5c6b 7213 7bdc daae  ..l..._j\kr.{...
-00003c90: 3da8 238e 7d4b 8d8b fcf1 287d d719 b39f  =.#.}K....(}....
-00003ca0: 1c7c 1e85 50d6 b8ea 8e14 55e5 ecf5 b629  .|..P.....U....)
-00003cb0: 535d 486e b5b4 7b25 e95e 64c2 86a8 96f9  S]Hn..{%.^d.....
-00003cc0: e69d 48f3 8896 048d 0a4c 203b 58a4 b6eb  ..H......L ;X...
-00003cd0: 04f7 8889 2ca2 a200 9bd1 2854 8d64 4102  ....,.....(T.dA.
-00003ce0: 28e2 d932 e917 953c 682f eb16 70e8 b716  (..2...<h/..p...
-00003cf0: 1fc2 82d3 d23b 5930 a7df abfc 041c 8c65  .....;Y0.......e
-00003d00: 3aa3 d733 2cc9 57fc 834c 2e0a eeb2 e2b0  :..3,.W..L......
-00003d10: 583a 5855 8c92 b020 fc71 31e8 9bcb f75b  X:XU... .q1....[
-00003d20: 14e3 2205 cd96 b3ee f133 e592 856f 2edf  .."......3...o..
-00003d30: 3f8b 028b e309 4785 66fc 730e 1511 781a  ?.....G.f.s...x.
-00003d40: 05c3 bef9 efcd e0b2 737d 1334 1b57 f6e0  ........s}.4.W..
-00003d50: aad1 6e21 b7d1 7107 d70d b73d 1c5c 5f07  ..n!..q....=.\_.
-00003d60: 1dbb 690f ffd3 cafe af28 facb af14 90b4  ..i......(......
-00003d70: 39ed 6e4e e0d3 002b 175b 827f 58f6 f9a6  9.nN...+.[..X...
-00003d80: d650 f0a5 9b05 d83a f64e d3b3 3fba 8edd  .P.....:.N..?...
-00003d90: 085a b6d3 687b e155 e3ca 6bb9 8dc0 759a  .Z..h{.U..k...u.
-00003da0: d75e 7b70 e306 ae86 dd7d e1c7 01db 721c  .^{p.....}....r.
-00003db0: f599 4180 77bb 1ca7 88e0 acd2 55a5 21bd  ..A.w.......U.!.
-00003dc0: 1794 04cd 3d8b b02a 4d58 cb4f 40fd ff01  ....=..*MX.O@...
-00003dd0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00003de0: 0000 2100 1152 c103 8702 0000 2e08 0000  ..!..R..........
-00003df0: 1400 0000 786c 2f73 6861 7265 6453 7472  ....xl/sharedStr
-00003e00: 696e 6773 2e78 6d6c 9c55 ed6e d330 14fd  ings.xml.U.n.0..
-00003e10: 8fc4 3b58 66e2 df9a 0ea1 81b6 3693 9766  ..;Xf.......6..f
-00003e20: b45a 9ab2 2661 88aa 8abc c459 2262 bbc4  .Z..&a.....Y"b..
-00003e30: 4e37 de8a 67e0 c970 9a21 2adb 9d26 7ee6  N7..g..p.!*..&~.
-00003e40: dc73 afef c7b9 37a3 8b47 5a83 2d69 44c5  .s....7..GZ.-iD.
-00003e50: d918 9e0c 8610 1096 f1bc 62f7 6398 c457  ..........b.c..W
-00003e60: c71f 2110 12b3 1cd7 9c91 31fc 4904 bc70  ..!.......1.I..p
-00003e70: 5fbf 1a09 2181 f265 620c 4b29 3767 8e23  _...!..eb.K)7g.#
-00003e80: b292 502c 067c 4398 b214 bca1 58aa cfe6  ..P,.|C.....X...
-00003e90: de11 9b86 e05c 9484 485a 3bef 86c3 5387  .....\..HZ;...S.
-00003ea0: e28a 4190 f196 c931 fcf0 1e82 9655 3f5a  ..A....1.....U?Z
-00003eb0: e2f5 c0e9 2974 47a2 7247 d2bd 6989 902a  ....)tG.rG..i..*
-00003ec0: 3b31 72a4 3b72 3ab0 3778 65cb beeb e015  ;1r.;r:.7xe.....
-00003ed0: cea4 c144 4c3c a812 75ae bfc5 b58e 85bf  ...DL<..u.......
-00003ee0: 7fe9 504c 1ea5 8ecd 794e 0c5f 8f0b 8338  ..PL....yN._...8
-00003ef0: 691b dc65 af07 9860 4974 2c08 e63a 845a  i..e...`It,..:.Z
-00003f00: c975 6cda 526c c49b e2ba 6ecd c2c3 e8d6  .ul.Rl....n.....
-00003f10: 5f46 46e1 5f3f fb3a 9659 92cf edc9 7773  _FF._?.:.Y....ws
-00003f20: 3f13 1b9c 293d a8c1 0ad2 6c09 7401 5232  ?...)=....l.t.R2
-00003f30: c2f7 04fc 9f97 ed7d 94c4 0be0 7f41 4182  .......}.....AA.
-00003f40: e2d9 2234 6675 0770 3f59 f0e0 7050 da5b  .."4fu.p?Y..pP.[
-00003f50: f094 95c8 7863 747c 3d3c 0727 2ba3 c13e  ....xct|=<.'+..>
-00003f60: 9af8 cb34 9a7d 33ba f4b6 96e7 c720 2e55  ...4.}3...... .U
-00003f70: d140 a947 4913 e086 2819 b36e 494c e5dd  .@.GI...(..nIL..
-00003f80: 247e d4a5 9e7a 8b40 7fe6 402c 5e14 8248  $~...z.@..@,^..H
-00003f90: 5034 9c82 2374 7462 c87e 9a84 d7b6 7857  P4..#ttb.~....xW
-00003fa0: c88b 6db8 9295 0df6 1651 6ca8 3259 5a3b  ..m......Ql.2YZ;
-00003fb0: ddcd 20ed a661 28a9 334c 9339 3286 3345  .. ..a(.3L.92.3E
-00003fc0: 4190 18ca 0b2f 5395 8e0d fedb 299b adab  A..../S.....)...
-00003fd0: ccc0 2f83 8577 6d1d 927a 64b9 b835 55cf  ../..wm..zd..5U.
-00003fe0: 7290 5bd6 4eb4 14f0 e290 6cdd 2846 cb38  r.[.N.....l.(F.8
-00003ff0: 9da0 d810 831f 4eac f81b bd4b eaae ed4e  ......N....K...N
-00004000: d840 5a4e 49d6 9d31 b1aa d656 6bd1 ddb3  .@ZNI..1...Vk...
-00004010: 678d 83ba a669 bf07 83a2 adeb 9461 6a08  g....i.......aj.
-00004020: 7d17 669f 695b 3783 7460 935d 8328 2baa  }.f.i[7.t`.].(+.
-00004030: 2ac4 74a3 57fe b49f 870a d833 ef55 61cb  *.t.W......3.Ua.
-00004040: cdce 3c94 a09d fd92 2c89 daea 01b6 5cdd  ..<.....,.....\.
-00004050: bd90 3b4e 69bb c23a c936 6f9d 4389 c42b  ..;Ni..:.6o.C..+
-00004060: d81f 2fb8 7ea6 81bb 677b f65d 4a2b 21d4  ../.~...g{.]J+!.
-00004070: 3fda 7498 f786 67e2 bc44 2ff3 5914 cdc2  ?.t...g..D/.Y...
-00004080: 4fff a238 ea7f effe 0100 00ff ff03 0050  O..8...........P
-00004090: 4b03 0414 0006 0008 0000 0021 0072 a0d0  K..........!.r..
-000040a0: dc58 0200 00c1 0800 0018 0000 0078 6c2f  .X...........xl/
-000040b0: 6472 6177 696e 6773 2f64 7261 7769 6e67  drawings/drawing
-000040c0: 312e 786d 6cec 565d 6f9b 3014 7d9f b4ff  1.xml.V]o.0.}...
-000040d0: 60f9 9d60 0c23 0c05 aae5 83a9 d2d4 f661  `..`.#.........a
-000040e0: fb01 9631 0109 7064 bb49 aaaa ff7d b631  ...1..pd.I...}.1
-000040f0: 69b6 256a 53ad 0f93 c683 b9dc cbbd d73e  i.%jS..........>
-00004100: e71e 92d9 d5be 6bc1 9609 d9f0 3e83 c104  ......k.....>...
-00004110: 41c0 7aca cba6 5f67 f0c7 f7c2 4b20 908a  A.z..._g....K ..
-00004120: f425 6979 cf32 f8c0 24bc ca3f 7e98 ed4b  .%iy.2..$..?~..K
-00004130: 91ee e452 005d a097 a97e cc60 add4 26f5  ...R.]...~.`..&.
-00004140: 7d49 6bd6 1139 e11b d6eb 68c5 4547 947e  }Ik..9....h.EG.~
-00004150: 146b bf14 64a7 4b77 ad8f 118a 7db9 118c  .k..d.Kw....}...
-00004160: 94b2 664c 2d87 0874 f5c8 1baa 75a4 e961  ..fL-..t....u..a
-00004170: 6e77 a676 7cc1 daf6 4b4f 6b2e 0657 2578  nw.v|...KOk..W%x
-00004180: 3758 94b7 7930 f3cd 098c 6913 b471 5b55  7X..y0....i..q[U
-00004190: f934 c6f1 2162 1c36 28f8 2e0f 92c1 6fec  .4..!b.6(.....o.
-000041a0: d169 5ec0 3889 5d8a 0ed9 145b f9b9 9de2  .i^.8.]....[....
-000041b0: 476d d1d9 bee8 4ce3 30bc acf1 d86e 2dc8  Gm....L.0....n-.
-000041c0: a66e 6821 48c7 4047 a8e0 1974 e8f4 dbaf  .nh!H.@G...t....
-000041d0: 47c1 3b07 10bd d9de 09d0 9419 0c21 e875  G.;..........!.u
-000041e0: 5606 1735 110a 609d 4652 b657 dfa4 7216  V..5..`.FR.W..r.
-000041f0: b817 4d06 1f8b 02cf 3fad 8ac8 2bb4 e545  ..M.....?...+..E
-00004200: 681e 79f3 55f4 d92b 7098 acf0 b458 e030  h.y.U..+p....X.0
-00004210: 7e32 d941 9c52 4db5 d253 765d 8e14 07f1  ~2.A.RM..Sv]....
-00004220: 1f24 778d dea7 e495 9a50 def9 bcaa 1aca  .$w......P......
-00004230: c6a1 d123 1344 be25 d9ee f211 b9cb d3f7  ...#.D.%........
-00004240: c42c c843 8159 cc15 0ec1 27e8 e733 dfee  .,.C.Y....'..3..
-00004250: 7ebc db53 0cec 9b13 3b72 6e7e c3c4 a499  ~..S....;rn~....
-00004260: 0939 8dd5 be12 7a98 48aa 7708 f619 d4aa  .9....z.H.w.....
-00004270: 7930 ab4e b2ad 001d 9c74 f4da 5263 9263  y0.N.....t..Rc.c
-00004280: c6bc ebcc 2551 6480 f462 0951 4391 8698  ....%Qd..b.QC...
-00004290: a6d6 72d8 d237 c867 a8e4 0abc 4acd 033f  ..r..7.g....J..?
-000042a0: 4b4e ef3b d6ab 41d2 82b5 9666 5937 1b09  KN.;..A....fY7..
-000042b0: 8148 cd40 89eb 3270 441c 9dd8 1272 00c3  .H.@..2pD....r..
-000042c0: 4274 3cb4 8e98 b6d1 b50d 4023 2327 b4fd  Bt<.......@##'..
-000042d0: b2dc cfe8 2e88 11c2 cfb1 5729 3e4c f490  ..........W)>L..
-000042e0: 1d34 f9a2 e2a7 a715 1fc5 5172 ae73 884f  .4........Qr.s.O
-000042f0: 4b3e 4071 9c9c 6afd 1734 1ffd aaf9 f05f  K>@q..j..4....._
-00004300: d47c f45f f317 fe00 bfaf e6f1 7b69 de7e  .|._........{i.~
-00004310: 2bcc bf8f fc27 0000 00ff ff03 0050 4b03  +....'.......PK.
-00004320: 0414 0006 0008 0000 0021 0031 b025 e426  .........!.1.%.&
-00004330: 0900 00f4 3300 0014 0000 0078 6c2f 6368  ....3......xl/ch
-00004340: 6172 7473 2f63 6861 7274 312e 786d 6cec  arts/chart1.xml.
-00004350: 5b5b 6fe3 b815 7e2f d0ff a00a 415f 0ac7  [[o...~/....A_..
-00004360: d6c5 d78e b3b0 e578 3168 6627 9864 b740  .......x1hf'.d.@
-00004370: 8b62 414b b4a3 8622 3524 95cb 2cf6 07f5  .bAK..."5$..,...
-00004380: 37ec e3fe b13d bcc8 961c 679c 384e 9b66  7....=....g.8N.f
-00004390: e387 c4bc 883a 3ce7 f0f0 fb0e e977 dfdc  .....:<......w..
-000043a0: 64c4 b9c2 5ca4 8c0e 5def b0e5 3a98 c62c  d...\...]...:..,
-000043b0: 49e9 62e8 7e7f 3e6d f45c 4748 4413 4418  I.b.~.>m.\GHD.D.
-000043c0: c543 f716 0bf7 9ba3 3ffe e15d 3c88 2f10  .C......?..]<./.
-000043d0: 9767 398a b103 8350 3188 87ee 8594 f9a0  .g9....P1.......
-000043e0: d914 f105 ce90 3864 39a6 d036 673c 4312  ......8d9..6g<C.
-000043f0: 8a7c d14c 38ba 86c1 33d2 f45b ad4e 530f  .|.L8...3..[.NS.
-00004400: e2da 01d0 0e03 6428 a5e5 f3fc 21cf b3f9  ......d(....!...
-00004410: 3c8d f184 c545 86a9 3452 704c 9004 0d88  <....E..4RpL....
-00004420: 8b34 17e5 68b1 d7e1 fe9d 11b3 34e6 4cb0  .4..h.......4.L.
-00004430: b93c 8c59 d634 8395 9382 c1bc 7673 39ab  .<.Y.4......vs9.
-00004440: 2350 5282 24f6 faad d0b9 4264 e8b6 dca6  #PR.$.....Bd....
-00004450: aa24 882e 4c05 a68d efcf 4c25 6705 4d70  .$..L.....L%g.Mp
-00004460: 1231 4ec1 1c95 fe59 3c18 1189 3985 a122  .1N....Y<...9.."
-00004470: 4625 486d f595 3d48 e319 e297 45de 0071  F%Hm..=H....E..q
-00004480: 7398 e42c 25a9 bcd5 d376 8fde c1d8 d105  s..,%....v......
-00004490: 037d 389f f0e7 22e5 580c ddd8 0b57 2a08  .}8...".X....W*.
-000044a0: 1fab 8056 b7d9 6bfa d6ae 3059 2f1c 0879  ...V..k...0Y/..y
-000044b0: 4bb0 9990 d7f2 d56c 9bcb f76a 11a6 8890  K......l...j....
-000044c0: 198a 2f95 6e2a 9d97 5d57 edea c175 65a8  ../.n*..]W...ue.
-000044d0: a7b4 1ba9 2f32 9504 eb2f 37ea 2f4f e38b  ..../2.../7./O..
-000044e0: a377 6830 63c9 ed29 7738 93ca 088e c8e3  .wh0c..)w8......
-000044f0: 69ca 853c 4142 9e22 0e7e e7b9 6a15 c88f  i..<AB.".~..j...
-00004500: f067 4ed8 f5d0 c584 802f a4e0 0daa 1eb4  .gN....../......
-00004510: c0f8 17d7 b9e6 281f bae2 7381 3876 1d44  ......(...s.8v.D
-00004520: 63a8 068d 495e 1622 0965 4fcd 110d 8890  c...I^.".eO.....
-00004530: 676a eaba 90ab 9afc 94ab 7f09 9e7f 0269  gj.............i
-00004540: c417 e81a b640 9e99 962a 35b2 499e 5ec2  .....@...*5.I.^.
-00004550: 4aa3 ec4c 7f73 9d4b b03d f484 f5a2 25d7  J..L.s.K.=....%.
-00004560: bd66 4860 92aa 15d9 0233 a281 6024 4da6  .fH`.....3..`$M.
-00004570: 2921 baa0 961f 8e08 374a 9737 9eee 438a  )!......7J.7..C.
-00004580: ec03 4b4c 5da7 dd82 e18c 9845 f671 3e37  ..KL]......E.q>7
-00004590: d541 59dd 8421 cb51 c05e 6b2f 50ab 853a  .AY..!.Q.^k/P..:
-000045a0: f236 c773 58fe 43f7 2f19 6d10 6986 c368  .6.sX.C./.m.i..h
-000045b0: ad01 23d3 108b b586 5868 5f28 f5a1 5f63  ..#.....Xh_(.._c
-000045c0: 35a4 d5c4 4147 6aa9 0cdd 396f 4c3f 9951  5...AGj...9oL?.Q
-000045d0: e4d1 39ce 72e1 60e9 c4ec d75f a493 23b0  ..9.r.`...._..#.
-000045e0: ebaf ffc9 61f5 6225 a8d4 e3c0 00f0 1d94  ....a.b%........
-000045f0: de2c 9d00 be48 ed13 0c0c 4ad0 6d6d 450a  .,...H....J.mmE.
-00004600: fb5e ca94 0e8d 5aa8 5265 a522 0787 9920  .^....Z.Re."... 
-00004610: 7161 1ed4 0ab7 f213 e80a c39b 41d4 7b4a  qa..........A.{J
-00004620: 2744 8564 e7aa 30c1 044b 6c75 6fa3 404e  'D.d..0..Kluo.@N
-00004630: 981c 718c 4c44 b865 85d4 c161 8678 a422  ..q.LD.e...a.x."
-00004640: abaa 86ef 93d4 5a31 66c4 048a 0544 8a1c  ......Z1f....D..
-00004650: 42a8 9123 2685 80e0 8013 d378 85f8 6dc4  B..#&......x..m.
-00004660: 08ab 4510 100d 8342 e241 9adc d4a6 cd78  ..E....B.A.....x
-00004670: 82ed f056 28a3 2221 f927 3c57 4fcc 8fce  ...V(."!.'<WO...
-00004680: 2484 ee3f 1d8c 0e02 3547 5d09 cd11 02ef  $..?....5G].....
-00004690: 501d 7219 41e0 9276 791b 2172 e9c0 9b8c  P.r.A..vy.!r....
-000046a0: 6bc6 83ab 2367 042a 470b ec24 05d7 7156  k...#g.*G..$..qV
-000046b0: 8d74 a575 962b 73a9 555f 8e68 0afa ed4b  .t.u.+s.U_.h...K
-000046c0: 8b95 d6f9 9a93 a338 86c0 a857 de1d 6fdd  .......8...W..o.
-000046d0: d192 a02f aa16 fffb f977 7801 725f d920  .../.....wx.r_. 
-000046e0: 6655 959c 6a1b adeb f4ab cfcc 8ad9 8ce0  fU..j...........
-000046f0: 60b2 d1f9 b6ad 6115 38d7 17e2 ce53 c337  `.....a.8....S.7
-00004700: f244 e809 c037 a7e0 107c 7e8a 82a0 d78a  .D...7...|~.....
-00004710: a2b0 d19e 748e 1b61 ab1f 35c6 c781 df38  ....t..a..5....8
-00004720: eefa 13bf df0d da41 14fd 5cd9 1e1f bd39  .......A..\....9
-00004730: 8695 7da1 3328 68fa b9c0 efed aaf8 0902  ..}.3(h.........
-00004740: 92fa 788d 696f 1236 42f8 347a c741 d808  ..x.io.6B.4z.A..
-00004750: 7a41 d8ed 8c47 e391 d7fa 59af b878 0032  zA...G....Y..x.2
-00004760: 6bbf 2967 01ae 62cd b16e 15ed 115b 2cf9  k.)g..b..n...[,.
-00004770: 24ab e848 5f89 ac2a 826e 88ac cbea 2d91  $..H_..*.n....-.
-00004780: f5f5 1934 d8af 4135 2ad8 9f41 f962 b6dc  ...4..A5*..A.b..
-00004790: 2843 bfd7 9e86 36a8 d756 a38a f0bb 6c06  (C....6..V....l.
-000047a0: da53 5fe6 3a6b efd7 2c81 09fd fb8a 7e55  .S_.:k..,.....~U
-000047b0: b34c fbd3 f6f1 e877 6296 ee7e cda2 bdf9  .L.....wb..~....
-000047c0: 7956 cbb4 1bf5 4ca4 fb1d ec4a fd27 9ae5  yV....L....J.'..
-000047d0: 6446 84a6 37fb 039a 0acf 1a3e f13c ec86  dF..7......>.<..
-000047e0: bca7 c006 839e a778 87d4 0560 b26d 28f0  .......x...`.m(.
-000047f0: 6acb acda 723f 23d2 bc24 1f01 209e a60a  j...r?#..$.. ...
-00004800: e882 cf18 b11f ca94 fa8f 234a 4f25 48dd  ..........#JO%H.
-00004810: cd04 c97f 2104 09d3 4411 5745 23d7 28d2  ....!...D.WE#.(.
-00004820: 92f6 18ef 006c 7dc1 ae4f f002 9ef8 1b5e  .....l}..O.....^
-00004830: 633d d0f2 0382 fc8f ca4d 58a0 a47a 4748  c=.......MX..zGH
-00004840: 7e87 b23a da55 f567 986f ac3f c55c 81ef  ~..:.U.g.o.?.\..
-00004850: 3aa8 85fe 638d 76cf d22f 7787 3ac1 08a8  :...c.v../w.:...
-00004860: c709 30d8 6aaa e39e edf2 b8d3 0eba 23af  ..0.j.........#.
-00004870: 31e9 4ca3 4638 efb4 1bfd 49df 6b74 7d3f  1.L.F8....I.kt}?
-00004880: 8cc2 7ed8 ee8d c715 58da 7e34 2cad a62b  ..~.....X.~4,..+
-00004890: da56 5f9b c403 94b9 0978 966b 3b46 1a4f  .V_......x.k;F.O
-000048a0: 6f20 4fe3 037f 70f0 fec0 df99 4121 2aae  o O...p.....A!*.
-000048b0: 212b f4cf f45f 8784 643f 9ae2 e1bc 20e4  !+..._..d?.... .
-000048c0: 470a 967a 309f b222 82c1 5530 a245 b64e  G..z0.."..U0.E.N
-000048d0: f3c6 0781 9274 c5f5 a0cf 92eb 993c 5ec4  .....t.......<^.
-000048e0: 127c d452 9942 e1ea 09e9 ec9e ae5d e783  .|.R.B.......]..
-000048f0: bdcd 7cb0 5597 5791 4843 1855 9e42 31c3  ..|.U.W.HC.U.B1.
-00004900: 7b3b f8db 3a04 db3a 84db 3ab4 b775 e86c  {;..:..:..:..u.l
-00004910: ebd0 dddc 01bc 67a5 4c53 2869 aeb5 c78b  ......g.LS(i....
-00004920: e564 a31d 773f 9b76 4896 bbdf c342 9125  .d..w?.vH....B.%
-00004930: d8cf 1e8a 146b 2c45 5ba0 fcef 6922 6d76  .....k,E[...i"mv
-00004940: 07a2 bc71 5d74 53f2 d320 f0db bd4e bbb3  ...q]tS.. ...N..
-00004950: a1a1 dbed 773b 5ec7 72d3 6a02 47a5 e896  ....w;^.r.j.G...
-00004960: d99c 7ae2 c664 d5f9 e3f2 3636 4857 f236  ..z..d....66HW.6
-00004970: b6e6 2b79 9bf0 e979 9b98 09b9 63ce 8650  ..+y...y....c..P
-00004980: 07b2 a940 acba 6dd7 8955 f694 d364 6bca  ...@..m..U...dk.
-00004990: d264 734c 0278 2de5 714f 1a0e 0d74 02dd  .dsL.x-.qO...t..
-000049a0: 208b 5a42 2e1e a80c b849 8089 db6c c6ec   .ZB.....I...l..
-000049b0: 8647 e140 c39a 6cd5 61e5 aa6f 40ed 0da8  .G.@..l.a..o@...
-000049c0: ed21 93fd 06d4 de80 daf3 00b5 5001 b555  .!..........P..U
-000049d0: 70bf 1fa8 29e2 141f bc61 b5d5 89c3 0a71  p...)....a.....q
-000049e0: 765d 6785 6ae1 c4e2 1092 b77f fe5c 30f9  v]g.j........\0.
-000049f0: 57e7 c0fc df15 cc89 8cb1 124e 58cc f062  W..........NX..b
-00004a00: f1dd f8f5 e33b b3c5 d7a9 ee5d 0bad e09e  .....;.....]....
-00004a10: d769 f95e d0b9 8b03 bdbe efb5 ba81 1f18  .i.^............
-00004a20: 7402 a7f9 558c 0704 6ba4 4f19 ef05 8e22  t...U...k.O...."
-00004a30: 46f0 c442 111d c653 a0cd fa44 cc08 96a5  F..B...S...D....
-00004a40: f403 bab1 a0a4 d231 d1c7 8735 7e8d 6e4e  .......1...5~.nN
-00004a50: 99a5 ce33 0355 2100 4c33 5973 e76f 31dc  ...3.U!.L3Ys.o1.
-00004a60: 2540 0498 1a2b 80a2 03dd bec4 c992 ea67  %@...+.........g
-00004a70: e8df 8c9f a7f1 e507 c047 66f0 1213 0166  .........Gf....f
-00004a80: 4ae9 fd8d 121e 02e0 bc94 8082 679f 3323  J...........g.3#
-00004a90: c6c6 a354 8501 fb6d bf84 8073 3840 8698  ...T...m...s8@..
-00004aa0: 94e5 208c a00b 383c 270b 38e2 56e7 e8bb  .. ...8<'.8.V...
-00004ab0: 1c66 7b9b 7335 bd87 e56a 7600 949b 126f  .f{.s5...jv....o
-00004ac0: 0df0 15fd 7949 d70b fecb 49b3 177e abe0  ....yI....I..~..
-00004ad0: 1158 4c5d f211 237b 5a1e 0415 8607 974d  .XL]..#{Z......M
-00004ae0: 545b 99b7 5247 fcff c0dc 3abf 2ad5 620c  T[..RG....:.*.b.
-00004af0: 9991 11f8 b63d ab07 ff36 1780 6604 ae5c  .....=...6..f..\
-00004b00: 08b8 c360 526f 6594 a1ec 4341 647a 7245  ...`Roe...CAdzrE
-00004b10: 6075 5596 3b10 d565 6081 27ee 4698 9a7c  `uU.;..e`.'.F..|
-00004b20: fb8f 30f6 e681 0e18 dff2 3451 21af 96ce  ..0.......4Q!...
-00004b30: 362c efd5 ac70 d0f7 ddb9 6e88 af00 172c  6,...p....n....,
-00004b40: 5810 162c fccf 23ed aee7 946f 216d e8fe  X..,..#....o!m..
-00004b50: 1f5e 94da 3da4 d5b2 595f 0969 ba69 8ce5  .^..=...Y_.i.i..
-00004b60: 35c6 368c cd4c c1c2 9465 3cda 007d d640  5.6..L...e<..}.@
-00004b70: d453 0393 cd75 3d0f f481 fb57 2638 ef8c  .S...u=....W&8..
-00004b80: 7c6a 7b46 1d26 bec0 4d63 5dc0 fdef 1a76  |j{F.&..Mc]....v
-00004b90: b3db 1c37 9734 2b2e 79d6 8343 e7d3 2db5  ...7.4+.y..C..-.
-00004ba0: c7eb 7e9b 4f61 dfc0 e0d0 7da5 6070 2da6  ..~.Oa....}.`p-.
-00004bb0: d522 6766 c89b 5ded db83 26e0 8cda 2d50  ."gf..]...&...-P
-00004bc0: 7d4a abef 83ea 6feb 0cef 996f ae3e f785  }J....o....o.>..
-00004bd0: 823d 5c97 7ee3 33d5 5bd2 0fde fcc1 cfc8  .=\.~.3.[.......
-00004be0: d2b7 94c7 fd90 8a8f 94d8 db00 765b 4d52  ............v[MR
-00004bf0: 918f e132 c1a5 18d9 c402 9c89 594e 0fe7  ...2........YN..
-00004c00: 7613 7552 a6ee c743 8662 8d9a 94d7 951f  v.uR...C.b......
-00004c10: 724f 77b6 b8e7 8eee 2b4b 11e4 3ca5 f20c  rOw.....+K..<...
-00004c20: 4bb8 28bf d054 e942 df78 9842 5210 734d  K.(..T.B.x.BR.sM
-00004c30: 0273 b811 0d99 9745 4a85 fe01 c0a1 3a21  .s.....EJ.....:!
-00004c40: 533f 1239 84a4 24fc 8a40 ff57 bf57 d00d  S?.9..$..@.W.W..
-00004c50: e671 550a 54ca 528d 620a cbb1 e065 45ae  .qU.T.R.b....eE.
-00004c60: cebf 20a8 d45f aee8 e3f2 c73a 47bf 0100  .. .._.....:G...
-00004c70: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00004c80: 0021 0076 7ea5 b1d3 0700 00d9 2600 0014  .!.v~.......&...
-00004c90: 0000 0078 6c2f 6368 6172 7473 2f63 6861  ...xl/charts/cha
-00004ca0: 7274 322e 786d 6cec 5a6d 6fdb 3610 fe3e  rt2.xml.Zmo.6..>
-00004cb0: 60ff 4113 b24f 8363 c9ef 166a 0f89 126f  `.A..O.c...j...o
-00004cc0: c3d2 3668 ba0d d830 0c34 45db 5c28 5225  ..6h...0.4E.\(R%
-00004cd0: a9c4 eeb0 ffbe e38b 1ccb 71da d46d b12c  ..........q..m.,
-00004ce0: 4b3e 38e2 8b4e c7e3 ddc3 bb47 7af6 ed32  K>8..N.....Gz..2
-00004cf0: 67c1 1591 8a0a 3e0a e3c3 280c 08c7 22a3  g.....>...(...".
-00004d00: 7c3e 0a7f 7a3d 690c c240 69c4 33c4 0427  |>..z=i..@i.3..'
-00004d10: a370 4554 f8ed f8cb 2f9e e104 2f90 d417  .pET..../.../...
-00004d20: 05c2 2400 215c 2578 142e b42e 9266 53e1  ..$.!\%x.....fS.
-00004d30: 05c9 913a 1405 e130 3613 3247 1a9a 72de  ...:...06.2G..r.
-00004d40: cc24 ba06 e139 6bb6 a2a8 d7b4 4242 2f00  .$...9k.....BB/.
-00004d50: ed21 2047 9457 f7cb fbdc 2f66 338a c989  .! G.W..../f3...
-00004d60: c065 4eb8 765a 48c2 9006 0ba8 052d 5425  .eN.vZH......-T%
-00004d70: 0dc7 3dd9 ba25 31a7 580a 2566 fa10 8bbc  ..=..%1.X.%f....
-00004d80: e984 558b 0261 71b7 b95e d518 8c94 214d  ..U..aq..^....!M
-00004d90: e261 d409 ae10 1b85 51d8 349d 0cf1 b9eb  .a......Q.4.....
-00004da0: 20bc f1d3 85eb 94a2 e419 c952 2139 6cc7   ..........R!9l.
-00004db0: c6fc 1c27 474c 13c9 4154 2ab8 06ad bdbd  ...'GL..AT*.....
-00004dc0: f27b 593c 47f2 b22c 1aa0 6e01 8b9c 5246  .{Y<G..,..n...RF
-00004dd0: f5ca 2e3b 1c3f 03d9 e942 803d 8257 e44d  ...;.?...B.=.W.M
-00004de0: 4925 51a3 10c7 9d1b 1374 3ed4 0051 bf39  I%Q......t>..Q.9
-00004df0: 68b6 fcbe c262 e34e a2f4 8a11 b7a0 386a  h....b.N......8j
-00004e00: 99d5 36d7 cfb5 2a4c 1063 5384 2f8d 6d36  ..6...*L.cS./.m6
-00004e10: 26af a7de 8c9b 1bb7 8d61 eeb2 6e64 2e34  &........a..nd.4
-00004e20: d58c d88b a5f9 9514 2fc6 cf50 3215 d9ea  ......../..P2...
-00004e30: 5c06 5268 b309 812a f084 4aa5 cf90 d2e7  \.Rh...*..J.....
-00004e40: 4882 dfc5 a189 02fd 127e 664c 5c8f 42c2  H........~fL\.B.
-00004e50: 18f8 0205 6f30 fd60 0521 df86 c1b5 44c5  ....o0.`.!....D.
-00004e60: 2854 6f4a 2449 1820 8ea1 1b2c a665 d548  (ToJ$I. ...,.e.H
-00004e70: 35b4 63b3 4694 30a5 2fcc d26d a330 3dc5  5.c.F.0./..m.0=.
-00004e80: b934 ff32 327b 05da a8b7 30b5 1381 3e53  .4.22{....0...>S
-00004e90: ab15 75ba 6949 2f21 d2b8 b8b0 5761 7009  ..u.iI/!....Wap.
-00004ea0: 7b0f 3321 5eac e676 d614 29c2 a889 c808  {.3!^..v..).....
-00004eb0: b611 254a 309a 4d28 63b6 61c2 8fa4 4c3a  ..%J0.M(c.a...L:
-00004ec0: a3eb 656c e7b0 327f 2e32 d7d7 eb46 20ce  ..el..2..2...F .
-00004ed0: a959 e62f 6733 d7dd aeba 9b20 b292 02fb  .Y./g3..... ....
-00004ee0: b5f5 0013 2d3c d0ab 82cc 20fc 47e1 3739  ....-<.... .G.79
-00004ef0: 6f30 edc4 11b4 3540 901b c06a 6b00 2beb  o0....5@...jk.+.
-00004f00: 0b95 3dec 63bc 85ac 9924 d8c8 84ca 289c  ..=.c....$....(.
-00004f10: c9c6 e495 93a2 c7a7 104a a50b 57a3 98b6  .........J..W...
-00004f20: f7c1 0d70 0d46 6e56 9b0e 17da fa80 800d  ...p.FnV........
-00004f30: 6468 558b 40e5 9fc3 85b1 9933 0337 a6db  dhU.@......3.7..
-00004f40: e828 c041 4e90 5ab8 1bad 81bd be0c a682  .(.AN.Z.........
-00004f50: 7827 c43c a772 3a54 6af1 da34 4e08 239a  x'.<.r:Tj..4N.#.
-00004f60: 785b fba8 2f98 d047 9220 8700 2b51 6a0b  x[../..G. ..+Qj.
-00004f70: 0653 2453 83a4 a61b ae4f a8df 352c 9803  .S$S.....O..5,..
-00004f80: 8639 2043 0190 e9f4 c0ac 5400 0624 7383  .9 C......T..$s.
-00004f90: 5748 ae52 c144 0d31 4035 0206 c109 cd96  WH.R.D.1@5......
-00004fa0: b565 0b99 112f de2b e54c a4b4 7c45 66e6  .e.../.+.L..|Ef.
-00004fb0: 8ed9 f842 0354 7f75 7074 d037 6bb4 9d30  ...B.T.upt.7k..0
-00004fc0: 9c22 f006 33a1 d029 0095 f6e1 ec94 2874  ."..3..)......(t
-00004fd0: 004f 72ae 8893 abf1 f710 cfa5 32b7 5f59  .Or.........2._Y
-00004fe0: 4315 668f 4c68 5762 5cc3 3e72 bd4d d596  C.f.LhWb\.>r.M..
-00004ff0: bccb 9311 c680 7e36 bc6e b9e4 9edb 0746  ......~6.n.....F
-00005000: e226 c27f 98bd 2073 f0aa 2b8f 54de 3e18  .&.... s..+.T.>.
-00005010: d98d d961 a0e3 8356 7230 3968 ed6d 25c4  ...a...Vr09h.m%.
-00005020: d535 20fd 6ff4 f743 c6f2 3f5c f370 5632  .5 .o..C..?\.pV2
-00005030: f607 4739 b9b7 f9bc 8a10 1566 7f78 996f  ..G9.......f.x.o
-00005040: 6fe5 f1c1 c068 3a58 6b0a 73d6 fbe9 cee6  o....h:Xk.s.....
-00005050: 5464 641c 7d6d 67d8 c3da 766c 6f77 77f7  Tdd.}mg...vloww.
-00005060: 7647 7555 8d8f 387f 30b0 637c e0ce 09ad  vGuU..8.0.c|....
-00005070: f74d 68bf 6f42 67f7 04f0 aa9b 45ba 46e5  .Mh.oBg.....E.F.
-00005080: 6dde 4e64 a9cf 94dd 5bb8 0a4a 09e0 fb57  m.Nd....[..J...W
-00005090: da6e 0fa2 34ed 34ba 27bd d346 271a a68d  .n..4.4.'..F'...
-000050a0: e3d3 76ab 71da 6f9d b486 fd76 b79d a67f  ..v.q.o....v....
-000050b0: 6fa4 071f 9c1c 7436 cec5 5e52 72fa a624  o.....t6..^Rr..$
-000050c0: 3f78 94f8 0b00 d9fe 35a2 616f d8e8 c469  ?x......5.ao...i
-000050d0: da18 9c74 278d 388a 3aa7 ad56 e7b8 d38a  ...t'.8.:..V....
-000050e0: feb6 0884 13d0 d986 54b5 0a13 502e e4b7  ........T...P...
-000050f0: 23df 060b 4e36 22df f7bc 23f2 877b fbf4  #...N6"...#..{..
-00005100: 8b29 1c8a d6ad 83eb a608 169f 1708 5c82  .)............\.
-00005110: b07d 363d 01c1 dd40 1047 0609 621b 9016  .}6=...@.G..b...
-00005120: da9f a0c0 06d3 c384 82f8 e3a0 203b 9b32  ............ ;.2
-00005130: 6573 ea85 b83e 2373 c2b3 1fc9 561e 0423  es...>#s....V..#
-00005140: 3f23 a800 37aa 1305 7d29 d22f e00c bad5  ?#..7...})./....
-00005150: 7f41 e4ce fe73 22cd c97c 6bfe 7139 9d32  .A...s"..|k.q9.2
-00005160: 7241 df6e 8a02 b05a ab36 47c5 2f34 d33e  rA.n...Z.6G./4.>
-00005170: c96a c543 77c4 a065 058b ddc1 70d0 efc7  .j.Cw..e....p...
-00005180: c3db 0350 55f5 db43 3700 2237 f328 9319  ...PU..C7."7.(..
-00005190: af93 aa7a fee4 8a59 f961 e993 059a 1a88  ...z...Y.a......
-000051a0: fa9e 7780 681c ef8d a247 9090 a039 0914  ..w.h....G...9..
-000051b0: 16f2 fe79 80d7 c567 b68c 0750 c5b4 06dd  ...y...g...P....
-000051c0: 7e37 0cb0 a95a 24cf de5b 2ab8 04ab edf3  ~7...Z$..[*.....
-000051d0: dc5a 2a76 473a 8c12 5bb8 9aa2 0e2a 9ecd  .Z*vG:..[....*..
-000051e0: c418 27a6 f2f4 a7d2 2a9f 0aef 661c 8804  ..'.....*...f...
-000051f0: 7f8c dd4c 781c 7956 1c5b 78bd d9f9 2778  ...Lx.yV.[x...'x
-00005200: 85c4 2417 a20a 709f 553f d8e4 abf5 f811  ..$...p.U?......
-00005210: d7c5 5cad 7edb b143 1b00 3c6c 03d0 f63b  ..\.~..C..<l...;
-00005220: 1614 7072 3330 e876 e24e af37 e8fb 60ae  ..pr30.v.N.7..`.
-00005230: 812e c4f3 91ad beef 4472 8511 dc31 37e7  ........Dr...17.
-00005240: 9390 140e 0f5b d23b bd72 ca9f a3a5 97bb  .....[.;.r......
-00005250: 3131 b365 75ed 9441 cb73 e1d9 b2a9 3b3b  11.eu..A.s....;;
-00005260: 20e6 26b9 0e6e 0a9b 51f8 1d01 4e0d 31a0   .&..n..Q...N.1.
-00005270: 4f44 0907 d519 e597 24f3 3c8d 81a9 3f85  OD......$.<...?.
-00005280: 7c4d f1e5 73c0 2b27 bcc2 2818 a4fc ee41  |M..s.+'..(....A
-00005290: 0d37 c121 bbd6 8083 63bf 164e 8d9d 1483  .7.!....c..N....
-000052a0: c1e4 61b7 5541 f20c 8814 40e7 bc00 6514  ..a.UA....@...e.
-000052b0: 9f03 89c4 e640 f518 3e69 1f52 27de 4dea  .....@..>i.R'.M.
-000052c0: 0cee 47ea ec01 f07a e908 ad4d 7aad d1f3  ..G....z...Mz...
-000052d0: 75cc 43a2 d986 1fc6 b23d 7276 0d12 41c3  u.C......=rv..A.
-000052e0: 7a1a 0e72 8b5f 5b73 686e 6781 5805 b25b  z..r._[shng.X..[
-000052f0: 1d79 16a9 bb99 72f9 31e2 83cf 505f bf12  .y....r.1...P_..
-00005300: e99d dfb4 6a10 c3a6 ec08 7cdb 7358 e0df  ....j.....|.sX..
-00005310: 8e08 9f32 a01e 15a9 e824 4749 42ed 2e9e  ...2.....$GIB...
-00005320: 974c d3b3 2b06 d1b5 11ee 90e6 ad81 0552  .L..+..........R
-00005330: d65b 0853 d7ef d323 8c67 e42c 607c 2769  .[.S...#.g.,`|'i
-00005340: 6620 cf65 d8b5 aceb d144 38d8 fbf6 5a77  f .e.....D8...Zw
-00005350: e06b f4f5 bf0f adfb b1b7 8624 7ec2 b0ff  .k.........$~...
-00005360: e01b 82bd 31ac 5e4f 5a7c db8d 6176 e898  ....1.^OZ|..av..
-00005370: e86b 423c 6e4d 5dc3 e725 6b00 da95 ebd4  .kB<nM]..%k.....
-00005380: 93a6 8f45 224f d97d 9e5c 075e 4438 34de  ...E"O.}.\.^D84.
-00005390: 3bd5 a91d 12b5 b4f0 011e 125b fa7d fa43  ;..........[.}.C
-000053a0: c29f 6d1f 0993 1fbf 2b9f f01d d713 4a1a  ..m.....+.....J.
-000053b0: 7eec ff84 9275 fcaa a164 ee2a 331f daef  ~....u...d.*3...
-000053c0: 0748 4822 6aaf 3e2d 1169 5f82 daab edf2  .HH"j.>-.i_.....
-000053d0: ed33 bfae dded ca0f ea9b 80a7 6265 f353  .3..........be.S
-000053e0: 807b 1ff4 e067 6ced 5bc6 e37e a6ea 2567  .{...gl.[..~..%g
-000053f0: 9ef0 f647 6846 5571 0c45 cfa5 3af2 850b  ...GhFUq.E..:...
-00005400: 30d0 be60 07de fbc4 50e6 e623 10a0 1fb6  0..`....P..#....
-00005410: ea8e ea1d fd7d de53 4fe7 77bc a37e 64f5  .....}.SO.w..~d.
-00005420: 7f21 29d7 1744 c3d7 2073 5b07 2d08 822f  .!)..D.. s[.-../
-00005430: 0c26 40f8 1169 2bbc 0278 6ca0 55e6 942b  .&@..i+..xl.U..+
-00005440: fb95 cba1 a1a3 cd97 5087 fd30 804f 65ec  ........P..0.Oe.
-00005450: 7ff3 518e 1d70 b79b 563b 0402 c748 718d  ..Q..p..V;...Hq.
-00005460: b52c 7858 5918 b219 40a5 fe70 531b aebf  .,xXY...@..pS...
-00005470: 481b ff03 0000 ffff 0300 504b 0304 1400  H.........PK....
-00005480: 0600 0800 0000 2100 3b6d 324b c100 0000  ......!.;m2K....
-00005490: 4201 0000 2300 0000 786c 2f77 6f72 6b73  B...#...xl/works
-000054a0: 6865 6574 732f 5f72 656c 732f 7368 6565  heets/_rels/shee
-000054b0: 7431 2e78 6d6c 2e72 656c 7384 8fc1 8ac2  t1.xml.rels.....
-000054c0: 3014 45f7 03fe 4378 7b93 d685 0c43 5337  0.E...Cx{....CS7
-000054d0: 22b8 55e7 0362 fada 06db 9790 f714 fd7b  ".U..b.........{
-000054e0: b31c 65c0 e5e5 70cf e536 9bfb 3ca9 1b66  ..e...p..6..<..f
-000054f0: 0e91 2cd4 ba02 85e4 6317 68b0 f07b da2d  ..,.....c.h..{.-
-00005500: bf41 b138 eadc 1409 2d3c 9061 d32e be9a  .A.8....-<.a....
-00005510: 034e 4e4a 89c7 9058 150b b185 5124 fd18  .NNJ...X....Q$..
-00005520: c37e c4d9 b18e 09a9 903e e6d9 4989 7930  .~.......>..I.y0
-00005530: c9f9 8b1b d0ac aa6a 6df2 5f07 b42f 4eb5  .......jm._../N.
-00005540: ef2c e47d 5783 3a3d 5259 feec 8e7d 1f3c  .,.}W.:=RY...}.<
-00005550: 6ea3 bfce 48f2 cf84 4939 9060 3ea2 4839  n...H...I9.`>.H9
-00005560: c845 edf2 8062 41eb 77f6 9e6b 7d0e 04a6  .E...bA.w..k}...
-00005570: 6dcc cbf3 f609 0000 ffff 0300 504b 0304  m...........PK..
-00005580: 1400 0600 0800 0000 2100 1198 abc9 db00  ........!.......
-00005590: 0000 d001 0000 2300 0000 786c 2f77 6f72  ......#...xl/wor
-000055a0: 6b73 6865 6574 732f 5f72 656c 732f 7368  ksheets/_rels/sh
-000055b0: 6565 7432 2e78 6d6c 2e72 656c 73ac 91cd  eet2.xml.rels...
-000055c0: 4ec3 300c 80ef 48bc 43e4 3b49 db03 4268  N.0...H.C.;I..Bh
-000055d0: e92e 68d2 ae30 1e20 246e 1bd1 3a51 ec01  ..h..0. $n..:Q..
-000055e0: 7b7b c261 129d 2671 e1e6 1ff9 f367 79b3  {{.a..&q.....gy.
-000055f0: fd5a 66f5 8185 6322 0bad 6e40 21f9 1422  .Zf...c"..n@!.."
-00005600: 8d16 5e0f bbbb 0750 2c8e 829b 13a1 8513  ..^....P,.......
-00005610: 326c fbdb 9bcd 33ce 4eea 104f 31b3 aa14  2l....3.N..O1...
-00005620: 620b 9348 7e34 86fd 848b 639d 3252 ed0c  b..H~4....c.2R..
-00005630: a92c 4e6a 5a46 939d 7f77 239a ae69 ee4d  .,NjZF...w#..i.M
-00005640: f9cd 807e c554 fb60 a1ec 4307 ea70 ca75  ...~.T.`..C..p.u
-00005650: f3df ec34 0cd1 e353 f2c7 0549 aeac 30a1  ...4...S...I..0.
-00005660: b8cf 7a59 45ba 32a2 58d0 fa5c e373 d0ea  ..zYE.2.X..\.s..
-00005670: aa0c e6ba 4dfb 9f36 b944 122c 2f28 52a5  ....M..6.D.,/(R.
-00005680: 7865 75d1 3317 79a7 df22 fd48 9ad5 1ffa  xeu.3.y..".H....
-00005690: 6f00 0000 ffff 0300 504b 0304 1400 0600  o.......PK......
-000056a0: 0800 0000 2100 81f1 a03f c400 0000 ad01  ....!....?......
-000056b0: 0000 2300 0000 786c 2f64 7261 7769 6e67  ..#...xl/drawing
-000056c0: 732f 5f72 656c 732f 6472 6177 696e 6731  s/_rels/drawing1
-000056d0: 2e78 6d6c 2e72 656c 73bc 90cf 0ac2 300c  .xml.rels.....0.
-000056e0: 87ef 82ef 5072 b7dd 7610 11bb 5d44 d855  ....Pr..v...]D.U
-000056f0: f401 4297 fdc1 ad2d 4d15 f7f6 1644 5010  ..B....-M....DP.
-00005700: bc79 0a49 c8f7 fbc8 aeba 4fa3 b851 e0c1  .y.I......O..Q..
-00005710: 590d b9cc 4090 35ae 196c a7e1 7c3a ac36  Y...@.5..l..|:.6
-00005720: 2038 a26d 7074 9634 ccc4 5095 cbc5 ee48   8.mpt.4..P....H
-00005730: 23c6 74c4 fde0 5924 8a65 0d7d 8c7e ab14  #.t...Y$.e.}.~..
-00005740: 9b9e 2664 e93c d9b4 695d 9830 a636 74ca  ..&d.<..i].0.6t.
-00005750: a3b9 6047 aac8 b2b5 0aef 0c28 3f98 a26e  ..`G.......(?..n
-00005760: 3484 ba29 409c 669f 927f b35d db0e 86f6  4..)@.f....]....
-00005770: ce5c 27b2 f14b 8432 3d86 9880 183a 8a1a  .\'..K.2=....:..
-00005780: a47c 4ef8 590a 9964 417d f7c8 ffe7 91bf  .|N.Y..dA}......
-00005790: 3cd4 c793 cb07 0000 00ff ff03 0050 4b03  <............PK.
-000057a0: 0414 0006 0008 0000 0021 0090 000d b0a6  .........!......
-000057b0: 0100 00dd 0200 000f 0000 0078 6c2f 6d65  ...........xl/me
-000057c0: 7461 6461 7461 2e78 6d6c 6451 4b4f 1b31  tadata.xmldQKO.1
-000057d0: 10be 57e2 3f58 be6f bc21 1442 b4bb 2802  ..W.?X.o.!.B..(.
-000057e0: e544 2554 28ea d5b1 c789 55bf 647b 6956  .D%T(.....U.d{iV
-000057f0: 55ff 7b67 bd84 0638 d9e3 197f f33d 9a9b  U.{g...8.....=..
-00005800: 8335 e405 62d2 deb5 743e ab29 0127 bcd4  .5..b...t>.).'..
-00005810: 6ed7 d21f 4f9b 6a49 49ca dc49 6ebc 8396  n...O.jII..In...
-00005820: 0e90 e84d 77f6 a5b1 90b9 e499 1304 70a9  ...Mw.........p.
-00005830: a5fb 9cc3 8ab1 24f6 6079 9af9 000e 3bca  ......$.`y....;.
-00005840: 47cb 3396 71c7 5288 c065 da03 646b d879  G.3.q.R..e..dk.y
-00005850: 5d5f 32cb b5a3 13c2 ea20 f927 14ab 45f4  ]_2...... .'..E.
-00005860: c9ab 3c13 de32 af94 16f0 0967 7ec5 e4e0  ..<..2.....g~...
-00005870: 38ce f218 f940 bb37 6e4f 4380 4484 ef5d  8....@.7nOC.D..]
-00005880: 466d 1f1a 04bf a0a0 9ff7 77eb 87ef 9458  Fm........w....X
-00005890: ed1e fb10 7ccc 209f dffc 4096 355a 227c  ....|. ...@.5Z"|
-000058a0: 1846 0412 78ca b036 e67f f1cc 4d0f a81f  .F..x..6....M...
-000058b0: 9b16 e20e 11f1 9682 d179 a363 2a7b 49f4  .........y.c*{I.
-000058c0: bf6f bd79 dc6b 35d5 c200 8f9b c99a 325f  .o.y.k5.......2_
-000058d0: 1e6e bdb5 e0f2 84c5 53d2 bb31 9171 3944  .n......S..1.q9D
-000058e0: 31e1 0a30 e61b 1a3f beb3 ae61 c710 8ad0  1..0...?...a....
-000058f0: ae51 7dee 238c 0325 99f7 024f 6cd8 feea  .Q}.#..%...Ol...
-00005900: 1a38 e4fb 94cb 49fa a85b fa67 2bb7 dba5  .8....I..[.g+...
-00005910: 90a2 527c 0ed5 c5f5 2554 7cf9 f5aa 5a88  ..R|....%T|...Z.
-00005920: 855a d4a2 3ebf 168b bf68 2206 b57a 357c  .Z..>....h"..z5|
-00005930: 3d1a fe10 31ec 9835 5aad eea6 200a 6f85  =...1..5Z... .o.
-00005940: 9a0d 0f09 644b eb42 1777 22e9 e366 36d2  ....dK.B.w"..f6.
-00005950: 60ef 3977 cd51 6251 f081 7314 6432 f0e5  `.9w.QbQ..s.d2..
-00005960: 8858 204e bf9c 98d2 fd03 0000 ffff 0300  .X N............
-00005970: 504b 0304 1400 0600 0800 0000 2100 3585  PK..........!.5.
-00005980: fa75 af01 0000 3c10 0000 2700 0000 786c  .u....<...'...xl
-00005990: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
-000059a0: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
-000059b0: 312e 6269 6eec 57bd 4a03 4110 feee 1221  1.bin.W.J.A....!
-000059c0: f102 b148 6161 112b 1b0b 8580 969a 68a1  ...Haa.+......h.
-000059d0: a807 3142 ca88 1114 248a 492f 3e83 9de0  ..1B....$.I/>...
-000059e0: 03f8 0abe 85a5 20d8 08fa 00b6 12e7 cb65  ...... ........e
-000059f0: c9ba b777 2954 44d9 5926 fb33 b333 b35f  ...w)TD.Y&.3.3._
-00005a00: be62 ae86 7d74 702a 5a46 03bb 5842 050b  .b..}tp*ZF..XB..
-00005a10: 32ca e8e2 10e7 3896 df2e 92c5 cb06 8547  2.....8........G
-00005a20: b48a 99a7 cb8c 873c ae83 4aae 0d0f 25ef  .......<..J...%.
-00005a30: bdef cb0c 510f ab12 f5fb 85d1 fd41 0666  ....Q........A.f
-00005a40: 894b ab08 5437 d7b6 8342 649b 0980 0759  .K..T7...Bd....Y
-00005a50: 5295 f05e ae0e 647b c0bc 6c1a a2ad 1078  R..^..d{..l....x
-00005a60: 3e8b ef4d 3ffa be59 fcd5 b98a 67fa 35fd  >..M?..Y....g.5.
-00005a70: a63f 8d2a ea08 b187 0d6c c908 b1f3 0308  .?.*.....l......
-00005a80: 8d0f b98e 031c 0d38 d093 fffa 4446 c485  .......8....DF..
-00005a90: 0eee 8403 8bbf 52d3 5793 4ecd fdc9 b25d  ......R.W.N....]
-00005aa0: d10e 0187 8043 c021 e010 8821 c03e 2733  .....C.!...!.>'3
-00005ab0: 541a a3de ca06 943f f073 103a 0446 08e4  T......?.s.:.F..
-00005ac0: a533 1ff1 875c 3225 2b07 ec85 c9b1 922c  .3...\2%+......,
-00005ad0: 3853 6c7d 35cf 6957 bdb7 e9d7 9603 e653  8Sl}5.iW.......S
-00005ae0: fd32 ede6 5ed5 107d 2124 e719 9681 2bb5  .2..^..}!$....+.
-00005af0: 9079 6532 f2e7 dd59 ed5c 5fd2 d6ef 7f36  .ye2...Y.\_....6
-00005b00: cab5 98d8 de97 f466 fd9d 666c 1353 1523  .......f..fl.S.#
-00005b10: 2996 8e0d 7d2e 0cd5 7371 fd22 801b cfb1  )...}...sq."....
-00005b20: be3c adf6 04a8 5231 b161 c65a c6c9 84e6  .<....R1.a.Z....
-00005b30: a0b0 d1f9 62de 7f1d c6b4 e196 842d 39ab  ....b........-9.
-00005b40: 44f1 28ad ae34 aed9 7063 7c72 795c 4cda  D.(..4..pc|ry\L.
-00005b50: f55a 947f ed1f 7f5b df2f dfdc 7e00 0000  .Z.....[./..~...
-00005b60: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00005b70: 2100 3585 fa75 af01 0000 3c10 0000 2700  !.5..u....<...'.
-00005b80: 0000 786c 2f70 7269 6e74 6572 5365 7474  ..xl/printerSett
-00005b90: 696e 6773 2f70 7269 6e74 6572 5365 7474  ings/printerSett
-00005ba0: 696e 6773 322e 6269 6eec 57bd 4a03 4110  ings2.bin.W.J.A.
-00005bb0: feee 1221 f102 b148 6161 112b 1b0b 8580  ...!...Haa.+....
-00005bc0: 969a 68a1 a807 3142 ca88 1114 248a 492f  ..h...1B....$.I/
-00005bd0: 3e83 9de0 03f8 0abe 85a5 20d8 08fa 00b6  >......... .....
-00005be0: 12e7 cb65 c9ba b777 2954 44d9 5926 fb33  ...e...w)TD.Y&.3
-00005bf0: b333 b35f be62 ae86 7d74 702a 5a46 03bb  .3._.b..}tp*ZF..
-00005c00: 5842 050b 32ca e8e2 10e7 3896 df2e 92c5  XB..2.....8.....
-00005c10: cb06 8547 b48a 99a7 cb8c 873c ae83 4aae  ...G.......<..J.
-00005c20: 0d0f 25ef bdef cb0c 510f ab12 f5fb 85d1  ..%.....Q.......
-00005c30: fd41 0666 894b ab08 5437 d7b6 8342 649b  .A.f.K..T7...Bd.
-00005c40: 0980 0759 5295 f05e ae0e 647b c0bc 6c1a  ...YR..^..d{..l.
-00005c50: a2ad 1078 3e8b ef4d 3ffa be59 fcd5 b98a  ...x>..M?..Y....
-00005c60: 67fa 35fd a63f 8d2a ea08 b187 0d6c c908  g.5..?.*.....l..
-00005c70: b1f3 0308 8d0f b98e 031c 0d38 d093 fffa  ...........8....
-00005c80: 4446 c485 0eee 8403 8bbf 52d3 5793 4ecd  DF........R.W.N.
-00005c90: fdc9 b25d d10e 0187 8043 c021 e010 8821  ...].....C.!...!
-00005ca0: c03e 2733 541a a3de ca06 943f f073 103a  .>'3T......?.s.:
-00005cb0: 0446 08e4 a533 1ff1 875c 3225 2b07 ec85  .F...3...\2%+...
-00005cc0: c9b1 922c 3853 6c7d 35cf 6957 bdb7 e9d7  ...,8Sl}5.iW....
-00005cd0: 9603 e653 fd32 ede6 5ed5 107d 2124 e719  ...S.2..^..}!$..
-00005ce0: 9681 2bb5 9079 6532 f2e7 dd59 ed5c 5fd2  ..+..ye2...Y.\_.
-00005cf0: d6ef 7f36 cab5 98d8 de97 f466 fd9d 666c  ...6.......f..fl
-00005d00: 1353 1523 2996 8e0d 7d2e 0cd5 7371 fd22  .S.#)...}...sq."
-00005d10: 801b cfb1 be3c adf6 04a8 5231 b161 c65a  .....<....R1.a.Z
-00005d20: c6c9 84e6 a0b0 d1f9 62de 7f1d c6b4 e196  ........b.......
-00005d30: 842d 39ab 44f1 28ad ae34 aed9 7063 7c72  .-9.D.(..4..pc|r
-00005d40: 795c 4cda f55a 947f ed1f 7f5b df2f dfdc  y\L..Z.....[./..
-00005d50: 7e00 0000 ffff 0300 504b 0304 1400 0600  ~.......PK......
-00005d60: 0800 0000 2100 ecff 94f0 8002 0000 620c  ....!.........b.
-00005d70: 0000 1000 0000 786c 2f63 616c 6343 6861  ......xl/calcCha
-00005d80: 696e 2e78 6d6c 7c57 db8a db30 107d 2ff4  in.xml|W...0.}/.
-00005d90: 1f8c debb 8eb2 edf6 4292 a5ba dab0 ec53  ........B......S
-00005da0: fb01 2671 3701 db09 b129 eddf 578d 2309  ..&q7....)..W.#.
-00005db0: cd68 fc62 c88c 7474 2e23 4136 cf7f faae  .h.b..tt.#A6....
-00005dc0: f8dd 5ec7 d379 d832 feb0 6245 3bec cf87  ..^..y.2..bE;...
-00005dd0: d3f0 b665 3f7f 980f 5f58 314e cd70 68ba  ...e?..._X1N.ph.
-00005de0: f3d0 6ed9 df76 64cf bbf7 ef36 fba6 dbcb  ..n..vd....6....
-00005df0: 6373 1a0a 8730 8c5b 769c a6cb b7b2 1cf7  cs...0.[v.......
-00005e00: c7b6 6fc6 87f3 a51d 5ce7 d7f9 da37 93fb  ..o.....\....7..
-00005e10: 797d 2bc7 cbb5 6d0e e3b1 6da7 be2b d7ab  y}+...m...m..+..
-00005e20: d553 d93b 00b6 dbec 8beb 96bd 3eb2 e2e4  .S.;........>...
-00005e30: 38b0 a2fb ff2d ef65 c11d 0557 77dd 5bbd  8....-.e...Ww.[.
-00005e40: 6888 aee3 1077 bdac 6f9b dcf7 564e 3781  h....w..o...VN7.
-00005e50: 663c e9b3 3f09 9c11 eac9 1982 7ff4 eb41  f<..?..........A
-00005e60: fde9 5ef7 c8df 5336 f1c0 4f70 a153 efb4  ..^...S6..Op.S..
-00005e70: 7ada 7e61 3d97 1f83 2955 004c bcaa 7dd9  z.~a=...)U.L..}.
-00005e80: 6fb4 a830 53ce fb62 d3a6 0731 10c4 2c81  o..0S..b...1..,.
-00005e90: 80a6 07d1 1044 2f81 80a6 0751 1044 2d81  .....D/....Q.D-.
-00005ea0: 80a6 0791 1044 2e81 8066 880e 8288 2510  .....D...f....%.
-00005eb0: d0f4 20af 10e4 c5c7 ef57 54f7 1173 0b93  .. ......WT..s..
-00005ec0: a02b 3e4f 0e1c 942a b048 2638 9693 41ad  .+>O...*.H&8..A.
-00005ed0: bede a72d 1ee7 ee7f 66fe 2a3e 4ff4 3a0e  ...-....f.*>O.:.
-00005ee0: 209f ef04 22c0 a1a6 8acf f71a af44 62c3   ..."........Db.
-00005ef0: c294 3cb1 df13 08e4 e777 02df 1d6f 55b8  ..<......w...oU.
-00005f00: 4d70 679d 772d 9613 d7ea 9049 00cc 13af  Mpg.w-.....I....
-00005f10: f3c4 6b64 661d 2c8a 171e da58 7368 57cd  ..kdf.,....XshW.
-00005f20: 7d58 7117 5206 13ae bd49 f10d 82b8 0282  }Xq.R....I......
-00005f30: 88bc b102 e910 c450 0834 1482 180a 01f9  .......P.4......
-00005f40: 8a20 727e c803 edbc e522 6fb9 7fa9 e3fc  . r~....."o.....
-00005f50: 0ae2 0249 244a 12a2 2412 2509 5112 8a92  ...I$J..$.%.Q...
-00005f60: 8428 9917 15cb c91c 4a34 8792 1405 3396  .(......J4....3.
-00005f70: 3063 99cf 5821 3b14 6187 4276 28c2 0e95  0c..X!;.a.Bv(...
-00005f80: 5719 cb89 4a05 cd53 8479 0ad9 a108 3b14  W...J..S.y....;.
-00005f90: ba4a 0ada a1f2 7668 4846 1364 3422 a309  .J....vhHF.d4"..
-00005fa0: 321a 91d1 908c 26c8 a06c 3491 8d46 d968  2.....&..l4..F.h
-00005fb0: 221b 9dcf 2696 936c 0cb4 c310 7618 6487  "...&..l....v.d.
-00005fc0: 21ec 30c8 0e03 ed30 793b 4c9e 7a2c a7d4  !.0....0y;L.z,..
-00005fd0: 9179 8630 cf20 f30c 619e 452a 2da1 d222  .y.0. ..a.E*-.."
-00005fe0: 9516 aab4 7995 36af 3296 1395 16a9 b484  ....y.6.2.......
-00005ff0: 4a8b 545a 4a25 0cdd e2d0 cbf0 ef60 f70f  J.TZJ%.......`..
-00006000: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00006010: 0000 2100 7707 ca82 4d01 0000 6902 0000  ..!.w...M...i...
-00006020: 1100 0801 646f 6350 726f 7073 2f63 6f72  ....docProps/cor
-00006030: 652e 786d 6c20 a204 0128 a000 0100 0000  e.xml ...(......
-00006040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001150: decd 8343 375b 8d96 2249 a0ea b973 ca4e  ...C7[.."I...s.N
+00001160: 1baf db49 abc7 9ef8 89dd 4a1b a3db 490d  ...I......J...I.
+00001170: 13fa 83c1 a017 f66c db9d 45a9 f137 7ddb  .......l..E..7}.
+00001180: e067 6135 b6ee a265 fecd cbbe 2ddd 3bec  .ga5...e....-.;.
+00001190: 0f00 0000 ffff 0000 00ff ffac 9d5b 6fdc  .............[o.
+000011a0: d615 46ff 8aab beb4 6851 cdb9 7066 64c8  ..F.....hQ..pfd.
+000011b0: 02e2 c88e efce 05ed bbe0 2ac8 4be2 c272  ..........*.K..r
+000011c0: d3f6 df67 e6ec c988 a4ce a267 017d 0890  ...g.......g.}..
+000011d0: 50cb 673e 8a1f b768 ad90 bcbc fbe9 f6f6  P.g>...h........
+000011e0: f3f5 cde7 9bab cb4f 1fff f3e8 d393 b374  .......O.......t
+000011f0: f6e8 ee5f 37bf dced feed 71ba d8fd 47db  ..._7.....q...G.
+00001200: f4e1 df77 9f3f fefc fce3 a79f 6f3e b70d  ...w.?......o>..
+00001210: ff4d f5e6 c3e3 7ffe effa f6ee c3ed 2fbb  .M............/.
+00001220: 6dab bf95 b3ab cb0f fb25 beda aff1 e46c  m........%.....l
+00001230: 7b76 7ed8 f0f4 f70d 8f76 e0dd 0efb f56a  {v~......v.....j
+00001240: 7579 feeb d5e5 f987 03f1 7510 ebb3 7b22  uy........u...{"
+00001250: 4d89 eb20 7689 8e6b e429 f16c feb1 cf63  M.. v..k.).l...c
+00001260: 43ca c720 df1c b60c c72d 2f0e 5b36 c72d  C.. .....-/.[6.-
+00001270: 2f1f 4629 d30f 7a7d f833 e5f8 67de 1cb6  /.F)..z}.3..g...
+00001280: ac8f 5bde 1eb6 dc7f 13de 3dd8 f2fe b065  ..[.......=....e
+00001290: bc4f f5f8 51e7 bb03 723c 2af9 ff70 54f6  .O..Q...r<*..pT.
+000012a0: 6bb4 6377 fc06 0ed3 fd7a fa90 58cf 0e53  k.cw.....z..X..S
+000012b0: 10e3 c334 23ae bf48 3c7b f829 9be9 a73c  ...4#..H<{.)...<
+000012c0: 3f10 6574 acb7 53e4 9b03 324e 7231 455e  ?.et..S...2Nr1E^
+000012d0: 1c90 edb8 53b3 dabd fc62 da57 0fd3 a659  ....S....b.W...Y
+000012e0: 335f 7f39 ee9b 2fc7 7d7b 42dc 771d a6ce  3_.9../.}{B.w...
+000012f0: ce82 f79d c033 e4db 0e32 abf8 775f acc2  .....3...2..w_..
+00001300: f79d 45ee cbdb e6c0 0f9d 45ee 3f67 d2ef  ..E.......E.?g..
+00001310: dda1 9e4c 9dc5 f132 ee45 9df5 efe9 e48b  ...L...2.E......
+00001320: b362 7dbd ff98 2767 9b51 23ea ac58 d71d  .b}...'g.Q#..X..
+00001330: 6456 ac67 e38f 1866 8d7a 1e7f 3ed5 d167  dV.g...f.z..>..g
+00001340: 0cb3 c27c 7360 5663 6676 8c5e 1c98 dd88  ...|s`Vcfv.^....
+00001350: b83f 5d67 07e9 e5c3 acc3 ec10 bcea c459  .?]g...........Y
+00001360: cf98 d7bd c8b3 d1f0 a617 79f6 ad7f db8b  ..........y.....
+00001370: 3c3b 02ef 26cc edee 47c1 8f57 2f9f ffe9  <;..&...G..W/...
+00001380: 4d79 7276 f6d7 47fb 7fde 94f3 edba ae56  Myrv..G........V
+00001390: 7f79 5bfe 7c79 fee3 fe67 c51f fff1 d59b  .y[.|y...g......
+000013a0: bf3f fbc3 f4f4 7e3f 390a b3a3 f8ed e48b  .?....~?9.......
+000013b0: b3e3 f7dd f88b ebd9 f1fb 7ef2 c5d9 81fb  ..........~.....
+000013c0: 61f2 c5fb 2336 a9f2 eec8 9f5c e557 7b78  a...#6.....\.W{x
+000013d0: 3793 ebf1 e7c6 fbd8 52da cf96 c9ba 8359  7.......R......Y
+000013e0: 770f 4fd7 8d2d 9d75 7723 f4e4 bccf f6f0  w.O..-.uw#......
+000013f0: 6edd 74cc fbea b065 b407 b1a5 f349 bbf3  n.t....e.....I..
+00001400: eef4 efcc 1e9e ee41 6ce9 acbb 9bf0 a7af  .......Al.......
+00001410: bb87 a7eb c696 ceba fbab 9ff1 a5d0 d250  ...............P
+00001420: 7a75 b854 6adf 87c9 714b bbd3 fcf4 651a  zu.Tj...qK....e.
+00001430: fd7b bee9 3af3 2bb3 c538 bb43 74bf 9fd3  .{..:.+..8.Ct...
+00001440: 75f6 53f9 e4dd da5d 3cd1 3afb 53f9 f475  u.S....]<.:.S..u
+00001450: 8e43 6677 5138 cda3 4e98 fd60 3d1e bfe9  .CfwQ8..N..`=...
+00001460: 3aea 0449 e333 64ba 8e39 215e a571 ffa7  :..I.3d..9!^.q..
+00001470: eb8c eabe 7abc 3fae cb07 6c5c f8e9 42a3  ....z.?...l\..B.
+00001480: 7e9f b2d0 b8e1 d385 4685 3e65 21ac 741e  ~.......F.>e!.t.
+00001490: 55fa 8485 1ade ed74 1e75 fa94 85b0 d479  U......t.u.....y
+000014a0: 54ea 5316 c256 e751 ab4f 5908 6b9d 47b5  T.S..V.Q.OY.k.G.
+000014b0: 3e65 21ec 751e f5fa 9485 b0d8 7954 ec53  >e!.u.......yT.S
+000014c0: 16c2 6667 d7ec 86f7 0fbf 6b76 c666 67d7  ..fg......kv.fg.
+000014d0: ec86 7713 15d7 ec86 f717 72cd 2ed8 ece2  ..w.......r.....
+000014e0: 9add f07e 22d7 ecdd cf43 18b4 c535 bbe1  ...~"....C...5..
+000014f0: fd44 aed9 059b 5d5c b31b de4f e49a 5d70  .D....]\...O..]p
+00001500: 6617 d7ec 86f7 13b9 6617 9cd9 d535 bbe1  f.......f....5..
+00001510: dd44 d535 bbe1 fd85 5cb3 2bce ecea 9add  .D.5....\.+.....
+00001520: f07e 22d7 ec8a 33bb ba66 37bc 9fc8 35bb  .~"...3..f7...5.
+00001530: e2cc aeae d90d ef27 72cd ae38 b3ab 6b76  .......'r..8..kv
+00001540: c3bb 8906 d7ec 86f7 1772 cd1e 7066 0fae  .........r..pf..
+00001550: d90d ef27 72cd 1e70 660f aed9 0def 2772  ...'r..pf.....'r
+00001560: cd1e 7066 0fae d90d ef27 72cd 1e70 660f  ..pf.....'r..pf.
+00001570: aed9 0def 2772 cd1e 7066 af5d b31b de4d  ....'r..pf.]...M
+00001580: b476 cd6e 787f 21d7 ec35 ceec b56b 76c3  .v.nx.!..5...kv.
+00001590: fb89 5cb3 d738 b3d7 aed9 0def 2772 cd5e  ..\..8......'r.^
+000015a0: e3cc 5ebb 6637 bc9f c835 7b8d 337b ed9a  ..^.f7...5{.3{..
+000015b0: ddf0 6ea2 8d6b 76c3 fb0b b966 6f70 666f  ..n..kv....fopfo
+000015c0: 5cb3 1bde 4fe4 9abd c199 bd71 cd6e 783f  \...O......q.nx?
+000015d0: 916b f606 67f6 c635 bbe1 fd44 aed9 1b9c  .k..g..5...D....
+000015e0: d91b d7ec 86f7 13b9 666f 7066 6f5d b31b  ........fopfo]..
+000015f0: de4d b475 cd6e 787f 21d7 ec2d ceec ad6b  .M.u.nx.!..-...k
+00001600: 76c3 fb89 5cb3 b738 b3b7 aed9 0def 2772  v...\..8......'r
+00001610: cdde e2cc deba 6637 bc9f c835 7b8b 337b  ......f7...5{.3{
+00001620: eb9a ddf0 6ea2 0bd7 ec86 f717 72cd bec0  ....n.......r...
+00001630: 997d e19a ddf0 7e22 d7ec 0b9c d917 aed9  .}....~"........
+00001640: 0def 2772 cdbe c099 7de1 9add f07e 22d7  ..'r....}....~".
+00001650: ec0b 9cd9 17ae d90d ef27 72cd be58 5034  .........'r..XP4
+00001660: aeda 69b5 e7bb 99d2 ca95 3b78 58ca d53b  ..i.......;xX..;
+00001670: add8 d5ac 5cc1 53e3 2195 ab78 5ab1 b159  ....\.S.!..xZ..Y
+00001680: b992 a7c6 432a 57f3 b462 6fb3 92e2 a6f1  ....C*W..bo.....
+00001690: 904a aa9b 15bb 9b95 9437 8def a71a 1bc9  .J.......7......
+000016a0: 533c d092 9394 6d5f d092 cd34 1e7c e249  S<....m_...4.|.I
+000016b0: a9b8 ed49 b6bd f1f0 bd92 6d5f f093 4d39  ...I......m_..M9
+000016c0: 9a1d 6445 d9ac a359 8adb 9e64 db1b 0fdf  ..dE...Y...d....
+000016d0: 2bd9 f6c4 6d6f ffe7 a1d9 419e ed52 5626  +...mo....A..RV&
+000016e0: b695 49ea cae0 fbdf 2b29 2c53 e361 29d9  ..I.....+),S.a).
+000016f0: f6a6 3861 29d9 f626 3961 2939 db9b e684  ..8a)..&9a)9....
+00001700: a5e4 6c6f a213 9692 6d67 7799 9a8d 1415  ..lo....mgw.....
+00001710: 657b 99a4 be0c bebf 8352 6026 3698 a939  e{.......R`&6..9
+00001720: 49b1 83ec 3093 9498 c1c3 0eca b6b3 c74c  I...0..........L
+00001730: 5264 060f a964 dbd9 6526 2933 8387 54b2  Rd...d..e&)3..T.
+00001740: edec 3393 149a c143 2a79 25c3 4e33 49a9  ..3....C*y%.N3I.
+00001750: 197c 3f95 d49a 89bd 666a a652 9c38 6c36  .|?.....fj.R.8l6
+00001760: 9354 9bc1 c30e cad9 ce76 3349 bd19 3ca4  .T.......v3I..<.
+00001770: 92b3 9d0d 6792 8a33 7848 25af 64d8 7226  ....g..3xH%.d.r&
+00001780: a939 83ef a792 a233 b1e9 4ccd 5d8a 8ab2  .9.....3..L.]...
+00001790: eb4c 5276 060f 3b28 673b fbce 2485 67f0  .LRv..;(g;..$.g.
+000017a0: 904a ce76 769e 494a cfe0 2195 9ced ec3d  .J.vv.IJ..!....=
+000017b0: 9314 9fc1 432a 39db d97d 2629 3f83 efa7  ....C*9..}&)?...
+000017c0: 92fa 33b1 ff4c cd68 8a13 870d 6892 0a34  ..3..L.h....h..4
+000017d0: 78d8 4139 dbd9 8226 a941 8387 5472 b6b3  x.A9...&.A..Tr..
+000017e0: 094d 5285 060f a9e4 6c67 1b9a a40e 0dbe  .MR.....lg......
+000017f0: 9f4a 0ad1 c446 3435 c729 2aca 4e34 4929  .J...F45.)*.N4I)
+00001800: 1a3c eca0 9ced ec45 9314 a3c1 432a 39db  .<.....E....C*9.
+00001810: d98d 2629 4783 8754 72b6 b31f 4d52 9006  ..&)G..Tr...MR..
+00001820: 0fa9 e46c 6747 9aa4 240d be9f 4a6a d2c4  ...lgG..$...Jj..
+00001830: 9e34 35f3 294e 1c36 a549 aad2 e061 07e5  .45.)N.6.I...a..
+00001840: 6c67 5b9a a42e 0d1e 52c9 d9ce c634 4965  lg[.....R....4Ie
+00001850: 1a3c a492 b39d ad69 92da 34f8 7e2a 294e  .<.....i..4.~*)N
+00001860: 139b d3d4 5ca8 a828 bbd3 24e5 69f0 b083  ....\..(..$.i...
+00001870: 72b6 b33f 4d52 a006 0fa9 e46c 6787 9aa4  r..?MR.....lg...
+00001880: 440d 1e52 c9d9 ce1e 3549 911a 3ca4 92b3  D..R....5I..<...
+00001890: 9d5d 6a6e 6ef4 f48a 06df 4d95 a54b 0d1e  .]jnn.....M..K..
+000018a0: 9692 3708 b14b cdd2 a506 0fa9 dc6c cfec  ..7..K.......l..
+000018b0: 52b3 74a9 c143 2a37 db33 bbd4 2c5d 6af0  R.t..C*7.3..,]j.
+000018c0: 90ca cdf6 cc2e 354b 971a 7c3f 9574 a999  ......5K..|?.t..
+000018d0: 5d6a 6e6e 549c 38ec 52b3 74a9 c1c3 0eba  ]jnnT.8.R.t.....
+000018e0: d99e d9a5 e6e6 46cd 0ee2 ff39 90a5 4b0d  ......F....9..K.
+000018f0: 1e76 50b6 9def f8cc d2a5 060f a964 dbd9  .vP..........d..
+00001900: a566 e952 83ef a7b2 377e 2edc f969 6ffd  .f.R....7~...io.
+00001910: 6c3c a4b2 377f f2dd 9ff6 f64f 76a9 d9de  l<..7......Ov...
+00001920: 00ca 2e35 db5b 40d9 a566 7b13 28bb d46c  ...5.[@..f{.(..l
+00001930: 6f03 5db8 0f54 bad4 bc70 27a8 bd15 94ef  o.]..T...p'.....
+00001940: 05cd d2a5 06df afa8 74a9 995d 6a96 2e35  ........t..]j..5
+00001950: 7848 2567 3bbb d42c 5d6a f090 ca5d b767  xH%g;..,]j...].g
+00001960: 76a9 59ba d4e0 2195 bb6e cfec 52b3 74a9  v.Y...!..n..R.t.
+00001970: c143 2a77 dd9e d9a5 66e9 5283 efa7 922e  .C*w....f.R.....
+00001980: 35b3 4bcd d2a5 060f a964 dbf9 3ed1 dcdc  5.K......d..>...
+00001990: a8b8 9261 979a a54b 0d1e 7650 5ec9 b04b  ...a...K..vP^..K
+000019a0: cdd2 a506 0fa9 e495 0cbb d42c 5d6a f0fd  ...........,]j..
+000019b0: 54d2 a566 76a9 59ba d4e0 2195 bc92 e13b  T..fv.Y...!....;
+000019c0: 4773 73a3 a2a2 ec52 b374 a9c1 c30e cad9  Gss....R.t......
+000019d0: ce2e 354b 971a 3ca4 92b3 9d5d 6a96 2e35  ..5K..<....]j..5
+000019e0: 7848 2567 3bbb d42c 5d6a f0fd 54d2 a566  xH%g;..,]j..T..f
+000019f0: 76a9 59ba d4e0 2195 9ced 7c3f 696e 6e54  v.Y...!...|?innT
+00001a00: 9c38 ec52 b374 a9c1 c30e cad9 ce2e 354b  .8.R.t........5K
+00001a10: 971a 3ca4 92b3 9d5d 6a96 2e35 f87e 2ae9  ..<....]j..5.~*.
+00001a20: 5233 bbd4 2c5d 6af0 904a ce76 bec3 3437  R3..,]j..J.v..47
+00001a30: 372a 2aca 2e35 4b97 1a3c eca0 9ced ec52  7**..5K..<.....R
+00001a40: b374 a9c1 432a 39db d9a5 66e9 5283 8754  .t..C*9...f.R..T
+00001a50: 72b6 b34b cdd2 a506 df4f 255d 6a66 979a  r..K.....O%]jf..
+00001a60: a54b 0d1e 52c9 d9ce f79d e6e6 46c5 89c3  .K..R.......F...
+00001a70: 2e35 4b97 1a3c eca0 9ced ec52 b374 a9c1  .5K..<.....R.t..
+00001a80: 432a 39db d9a5 66e9 5283 efa7 922e 35b3  C*9...f.R.....5.
+00001a90: 4bcd d2a5 060f a9e4 6ce7 3b51 7373 a3a2  K.......l.;Qss..
+00001aa0: a2ec 52b3 74a9 c1c3 0eca d9ce 2e35 4b97  ..R.t........5K.
+00001ab0: 1a3c a492 b39d 5d6a 962e 3578 4825 673b  .<....]j..5xH%g;
+00001ac0: bbd4 225d 6af0 dd54 45ba d4e0 6129 d7f6  .."]j..TE...a)..
+00001ad0: c22e b548 971a 3ca4 722e b5b0 4b2d d2a5  ...H..<.r...K-..
+00001ae0: 060f a9dc 6c2f ec52 8b74 a9c1 432a 37db  ....l/.R.t..C*7.
+00001af0: 0bbb d422 5d6a f0fd 54d2 a516 76a9 45ba  ..."]j..T...v.E.
+00001b00: d4e0 2195 6c3b 3f31 b7c8 fb52 8387 54b2  ..!.l;?1...R..T.
+00001b10: ed7c 5f6a 912e 3578 4825 dbce 2eb5 4897  .|_j..5xH%....H.
+00001b20: 1a3c a492 6d67 975a a44b 0dbe 9f4a bad4  .<..mg.Z.K...J..
+00001b30: c22e b548 971a 3ca4 926d e7fb 528b 74a9  ...H..<..m..R.t.
+00001b40: c143 2ad9 7676 a945 bad4 e021 956c 3bbb  .C*.vv.E...!.l;.
+00001b50: d422 5d6a f090 4ab6 9d5d 6a91 2e35 f87e  ."]j..J..]j..5.~
+00001b60: 2afb 60dd 8527 eb4a 975a 169e ad6b 1fae  *.`..'.J.Z...k..
+00001b70: bbf4 745d f7b7 d4b2 f07c 5dfb 80dd 8527  ..t].....|]....'
+00001b80: ec36 377a fadf 26ca c233 76ed 4376 179e  .67z..&..3v.Cv..
+00001b90: b2db dca8 4985 cf92 29f6 41bb 0b4f da6d  ....I...).A..O.m
+00001ba0: 6ed4 a4c2 670e 14e9 5283 ef9f 38d2 a516  n...g...R...8...
+00001bb0: 76a9 45ba d4e0 2195 6c3b bbd4 225d 6af0  v.E...!.l;.."]j.
+00001bc0: 90ca fd2d b5f0 7377 4b73 a3a2 0cec 528b  ...-..swKs....R.
+00001bd0: 74a9 c1c3 0eca d9ce 2eb5 4897 1a7c 3f95  t.........H..|?.
+00001be0: 74a9 855d 6a91 2e35 7848 25af 64d8 a516  t..]j..5xH%.d...
+00001bf0: e952 8387 54f2 4a86 9fc4 5b9a 1b15 1565  .R..T.J...[....e
+00001c00: 975a a44b 0d1e 76d0 fd4e a6b0 4b2d d2a5  .Z.K..v..N..K-..
+00001c10: 060f a9dc ef64 0abb d422 5d6a f0fd 54d2  .....d..."]j..T.
+00001c20: a516 76a9 45ba d4e0 2195 9ced ec52 8b74  ..v.E...!....R.t
+00001c30: a9c1 432a 39db f9f9 bca5 b951 71e2 b04b  ..C*9......Qq..K
+00001c40: 2dd2 a506 0f3b 2867 3bbb d422 5d6a f0fd  -....;(g;.."]j..
+00001c50: 54d2 a516 76a9 45ba d4e0 2195 9ced ec52  T...v.E...!....R
+00001c60: 8b74 a9c1 432a 39db f989 bda5 b951 5151  .t..C*9......QQQ
+00001c70: 76a9 45ba d4e0 6107 e56c 6797 5aa4 4b0d  v.E...a..lg.Z.K.
+00001c80: 1e52 c9d9 ce2e b548 971a 7c3f 9574 a985  .R.....H..|?.t..
+00001c90: 5d6a 912e 3578 4825 673b bbd4 225d 6af0  ]j..5xH%g;.."]j.
+00001ca0: 904a ce76 7e8e 6f69 6e54 9c38 ec52 8b74  .J.v~.oinT.8.R.t
+00001cb0: a9c1 c30e cad9 ce2e b548 971a 7c3f 9574  .........H..|?.t
+00001cc0: a985 5d6a 912e 3578 4825 673b bbd4 225d  ..]j..5xH%g;.."]
+00001cd0: 6af0 904a ce76 7eb2 6f69 6e54 5494 5d6a  j..J.v~.oinTT.]j
+00001ce0: 912e 3578 d841 39db d9a5 16e9 5283 8754  ..5x.A9.....R..T
+00001cf0: 72b6 b34b ddbd 52f4 fe7d 8527 3c5f 34f8  r..K..R..}.'<_4.
+00001d00: 6eaa 2a5d 6af0 b094 6b7b 6597 5aa5 4b0d  n.*]j...k{e.Z.K.
+00001d10: 1e52 b9b6 5776 a955 bad4 e021 95fb 7d7b  .R..Wv.U...!..}{
+00001d20: 6597 5aa5 4b0d 1e52 b9d9 5ed9 a556 e952  e.Z.K..R..^..V.R
+00001d30: 83ef a792 2eb5 b24b add2 a506 0fa9 64db  .......K......d.
+00001d40: d9a5 56e9 5283 8754 b2ed ec52 ab74 a9c1  ..V.R..T...R.t..
+00001d50: 432a d976 76a9 55ba d4e0 2195 6c3b bbd4  C*.vv.U...!.l;..
+00001d60: 2a5d 6af0 fd54 d2a5 5676 a955 bad4 e021  *]j..T..Vv.U...!
+00001d70: 956c 3bbb d42a 5d6a f090 4ab6 9d5d 6a95  .l;..*]j..J..]j.
+00001d80: 2e35 7848 25db ce2e b54a 971a 3ca4 926d  .5xH%....J..<..m
+00001d90: 6797 5aa5 4b0d be9f 4aba d4ca 2eb5 4a97  g.Z.K...J.....J.
+00001da0: 1a3c a492 6d67 975a 9b1b 3dfd 0a39 7848  .<..mg.Z..=..9xH
+00001db0: 25db ce2e b54a 971a 3ca4 926d 6797 5aa5  %....J..<..mg.Z.
+00001dc0: 4b0d 1e52 c9b6 b34b add2 a506 df4f 655f  K..R...K.....Oe_
+00001dd0: 5cba f0e6 52fb ead2 8577 974a 975a 17de  \...R....w.J.Z..
+00001de0: 5e6a 5f5f baf4 fe52 d9f6 8537 98da 5798  ^j__...R...7..W.
+00001df0: 2ebc c354 bad4 baf0 1653 fb1a d385 f798  ...T.....S......
+00001e00: 3637 2a86 ccc2 9b4c edab 4cf9 5da6 55ba  67*....L..L.].U.
+00001e10: d4e0 fb27 8e74 a995 9ff1 5be5 337e 8387  ...'.t....[.3~..
+00001e20: 54ee 3790 95ef 4bad f2be d4e0 2195 fb0d  T.7...K.....!...
+00001e30: 6465 975a a54b 0d1e 52b9 dfc9 5476 a955  de.Z.K..R...Tv.U
+00001e40: bad4 e021 95fb 9d4c 6597 5aa5 4b0d be9f  ...!...Le.Z.K...
+00001e50: 4aba d4ca 2eb5 4a97 1a3c a492 6d67 975a  J.....J..<..mg.Z
+00001e60: a54b 0d1e 52c9 b6b3 4bad d2a5 060f a964  .K..R...K......d
+00001e70: dbf9 7da7 b5b9 5131 dbd9 a556 e952 83ef  ..}...Q1...V.R..
+00001e80: efa0 74a9 955d 6a95 2e35 7848 25af dbd9  ..t..]j..5xH%...
+00001e90: a556 e952 8387 54f2 4a86 5d6a 952e 3578  .V.R..T.J.]j..5x
+00001ea0: 4825 afdb f90d a8b5 b951 5151 76a9 55ba  H%.......QQQv.U.
+00001eb0: d4e0 6107 e56c 6797 5aa5 4b0d be9f 4aba  ..a..lg.Z.K...J.
+00001ec0: d4ca 2eb5 4a97 1a3c a492 b39d 5d6a 952e  ....J..<....]j..
+00001ed0: 3578 4825 673b bbd4 2a5d 6af0 904a ce76  5xH%g;..*]j..J.v
+00001ee0: 7e2f 6a6d 6e54 9c38 ec52 ab74 a9c1 f777  ~/jmnT.8.R.t...w
+00001ef0: 50ba d4ca 2eb5 4a97 1a3c a492 b39d 5d6a  P.....J..<....]j
+00001f00: 952e 3578 4825 673b bbd4 2a5d 6af0 904a  ..5xH%g;..*]j..J
+00001f10: ce76 7e53 6a6d 6e54 5494 5d6a 952e 3578  .v~SjmnTT.]j..5x
+00001f20: d841 39db d9a5 0ed2 a506 df4d 3548 971a  .A9........M5H..
+00001f30: 3c2c e5da 3eb0 4b1d a44b 0d1e 52b9 b60f  <,..>.K..K..R...
+00001f40: ec52 07e9 5283 8754 ee77 7d03 5bcb 415a  .R..R..T.w}.[.AZ
+00001f50: cbe0 fba9 a4b5 1cd8 5a0e d20f 060f a9e4  ........Z.......
+00001f60: 1164 3f38 483f 183c a492 4790 4ddc 204d  .d?8H?.<..G.M. M
+00001f70: 5cf0 fd54 d2c4 0d6c e206 e9bc 8287 54f2  \..T...l......T.
+00001f80: 08b2 f31a a4f3 0a1e 52c9 23c8 7669 9076  ........R.#.vi.v
+00001f90: 29f8 7e2a 6997 06b6 4b83 f438 c143 2a79  ).~*i...K..8.C*y
+00001fa0: 04d9 e30c d2e3 043f 4d75 7ef7 d3ed ede7  .......?Mu~.....
+00001fb0: eb9b cf37 57bf 0100 00ff ff00 0000 ffff  ...7W...........
+00001fc0: 6c51 4d4f c240 10fd 2b9b 0921 9aa8 a505  lQMO.@..+..!....
+00001fd0: 252d 6d13 0821 e1a0 07b8 785d e9b4 dd58  %-m..!....x]...X
+00001fe0: baeb 74aa 80f1 bf3b 151a 3db8 87d9 79f3  ..t....;..=...y.
+00001ff0: f166 e76d ac5b b62b 5331 9222 cc13 9807  .f.m.[.+S1."....
+00002000: d136 0075 a0a8 3559 029f a3cb b995 dbef  .6.u..5Y........
+00002010: cce8 d7f4 b92f f0d2 7867 ebcc b0b1 b5ae  ...../..xg......
+00002020: 5696 f69a d9d4 856a dece ace3 e879 b5f4  V......j.....y..
+00002030: a501 a432 dfb4 152a 3e3a 4c00 0f8e b069  ...2...*>:L....i
+00002040: a40f 5476 c8d7 3273 04ca 91b1 64f8 9880  ..Tv..2s....d...
+00002050: 2f0d b9f0 b595 4ee7 4fcb abc1 623c ac78  /.....N.O...b<.x
+00002060: 362c 7836 5804 37ea 0f06 b88e bdbe 36f6  6,x6X.7.......6.
+00002070: ce63 5271 fe7b 591a 3b5d e0a3 a6c2 d48d  .cRq.{Y.;]......
+00002080: aa30 6719 7c37 0545 a628 7b9f adfb 89de  .0g.|7.E.({.....
+00002090: 837a b1cc 76df a312 7586 d4a1 31a8 dc5a  .z..v...u...1..Z
+000020a0: 91ef 0c44 888e 778b dc3a e5b4 43da 9a93  ...D..w..:..C...
+000020b0: ac19 8292 85b0 66dd 4994 80b3 c4a4 0d83  ......f.I.......
+000020c0: 2a25 7eb2 92a8 96ce 2430 09c2 49f8 300d  *%~.....$0..I.0.
+000020d0: 4221 7e47 62b3 bb24 4415 8aba 2fa1 75e6  B!~Gb..$D.../.u.
+000020e0: 7782 7b1f 965e 9b12 91d3 6f00 0000 ffff  w.{..^....o.....
+000020f0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00002100: 46d3 a5b7 d30a 0000 4b4c 0000 1800 0000  F.......KL......
+00002110: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00002120: 6565 7432 2e78 6d6c 9c94 5d6f da30 1486  eet2.xml..]o.0..
+00002130: ef27 ed3f 44be 2789 0304 1a11 aa75 155a  .'.?D.'......u.Z
+00002140: a5a9 aada 7d5c 1be7 042c e238 b34d 8156  ....}\...,.8.M.V
+00002150: fbef 3b76 0205 2155 ac11 3826 397e ce7b  ..;v..!U..8&9~.{
+00002160: be98 5c6f 6515 3c83 3642 d539 a161 4c02  ..\oe.<.6B.9.aL.
+00002170: a8b9 2a44 bdc8 c9cf 1fb3 de98 04c6 b2ba  ..*D............
+00002180: 6095 aa21 273b 30e4 7afa f9d3 64a3 f4ca  `..!';0.z...d...
+00002190: 2c01 6c80 84da e464 696d 9345 91e1 4b90  ,.l....dim.E..K.
+000021a0: cc84 aa81 1adf 944a 4b66 f1a7 5e44 a6d1  .......JKf..^D..
+000021b0: c00a 7f48 5651 12c7 6924 99a8 494b c8f4  ...HVQ..i$..IK..
+000021c0: 250c 5596 82c3 ade2 6b09 b56d 211a 2a66  %.U.....k..m!.*f
+000021d0: 51bf 598a c6ec 6992 5f82 934c afd6 4d8f  Q.Y...i._..L..M.
+000021e0: 2bd9 2062 2e2a 6177 1e4a 02c9 b3bb 45ad  +. b.*aw.J....E.
+000021f0: 349b 5718 f796 0e18 0fb6 1a3f 097e fb7b  4.W........?.~.{
+00002200: 37fe f999 2729 b856 4695 3644 72d4 6a3e  7...').VF.6Dr.j>
+00002210: 0fff 2aba 8a18 3f90 cee3 bf08 4307 9186  ..*...?.....C...
+00002220: 67e1 0af8 864a 3e26 890e 0fac e40d d6ff  g....J>&........
+00002230: 202c 3dc0 5cba 74b6 1645 4e5e e3ee eae1   ,=.\.t..EN^....
+00002240: 9dba 25ee c5d4 2d47 d75f 329d 1402 2bec  ..%...-G._2...+.
+00002250: a20a 3494 39f9 42b3 7b3a 22d1 74e2 1be8  ..4.9.B.{:".t...
+00002260: 9780 8d39 da07 2f4a c927 ce2a b877 1d57  ...9../J.'.*.w.W
+00002270: 612f c7d8 cbae 4be7 4aad 9cf9 1d7a 8f11  a/....K.J....z..
+00002280: dcb0 1a82 ed53 83b5 462b 12ec ba2d 466c  .....S..F+...-Fl
+00002290: 55f3 1d4a fb15 2a04 dca0 6ac6 ad78 8607  U..J..*...j..x..
+000022a0: 3c91 93b9 b256 c947 b158 5a3f 1316 9f95  <....V.G.XZ?....
+000022b0: 5abd 40ed 5541 0568 8c72 db33 1d63 88a6  Z.@.UA.h.r.3.c..
+000022c0: 7f7c 0037 c353 3327 2327 e8b1 23fe d7b1  .|.7.S3'#'..#...
+000022d0: 568b d3ba d778 a1bf 9320 4e5c 524c c55e  V....x... N\RL.^
+000022e0: 2aee 31d1 d121 d3c7 fb7d d667 7eb2 1f74  *.1..!...}.g~..t
+000022f0: 5040 c9d6 957d 549b 6fe0 9283 491d 8403  P@...}T.o...I...
+00002300: acb8 1b99 acd8 dd82 e138 ab98 fcb0 efb0  .........8......
+00002310: 5c55 c8c0 3590 c2fd e7e0 a8b1 adbf 6f44  \U..5.........oD
+00002320: 6197 3949 86e1 7038 48c7 2397 3cbb 73e3  a.9I..p8H.#.<.s.
+00002330: 9720 8faf 0de6 ff77 6be3 051e 1858 29cf  . .....wk....X).
+00002340: c07b c7a0 49d8 ef27 719f 2608 9983 b1b3  .{..I..'q.&.....
+00002350: aeda ef50 2836 4c2b c575 4eeb 671c 8ec7  ...P(6L+.uN.g...
+00002360: e988 1e6b 19bd 2b85 621b b510 dc1c 2069  ...k..+.b..... i
+00002370: 3a88 5327 e5dc 7de4 f3f1 0f00 00ff ff00  :.S'..}.........
+00002380: 0000 ffff cc9c 7d73 da46 1087 bf8a a278  ......}s.F.....x
+00002390: 32a6 2546 02fc 1acc 0ca0 d38b 83a1 3590  2.%F..........5.
+000023a0: 66da e930 8c83 9bcc 386e 065c 27f9 f6dd  f..0....8n.\'...
+000023b0: 934e d2dd 21e9 dec0 f88f c4c9 b18b 9e3b  .N..!..........;
+000023c0: 89dd dfee 1dee ac3f 2f97 8fde e271 d1ed  .......?/....q..
+000023d0: acfe fd6e ad2e 6dd7 b6d6 df16 0f6b f8d7  ...n..m......k..
+000023e0: 85db b6ad 1f6e 7b71 7bf1 e9a7 b75c df2e  .....n{q{....\..
+000023f0: 1f1e 2f6d e7a8 6577 3bb7 d8b6 878d 2fed  ../m..ew;...../.
+00002400: a603 0377 d6ed 027b 7747 fdf9 ef33 3499  ...w...{wG...34.
+00002410: 46e3 d1a4 d3b8 eb76 9eba 6ea7 f1d4 ed34  F......v..n....4
+00002420: 6e89 5b3f 7183 bfe1 edd6 e00b 16c7 acc9  n.[?q...........
+00002430: 2031 39b3 1bc4 c723 9772 b311 b431 e26f   19....#.r...1.o
+00002440: 8c5c 2523 27f4 954e d82b bd2f 8039 654d  .\%#'..N.+./.9eM
+00002450: 86c4 04cf 3b9b e664 767d 38f6 fd09 9a1e  ....;..dv}8.....
+00002460: a28f bfa1 bae5 d4ad c178 32ad d5c8 a49d  .........x2.....
+00002470: ec4d 1ab0 b4d9 fa36 55d6 171b c3fa 36b9  .M.....6U.....6.
+00002480: f5f5 7b83 69d9 da12 1732 e5c7 15ed 1af9  ..{.i....2......
+00002490: 8783 f170 763d 3aec b9b5 37ff 3cbe 837b  ...pv=:...7.<..{
+000024a0: 351c 5e4f ea96 6dd7 ad74 363f be2d 5f1d  5.^O..m..t6?.-_.
+000024b0: f40e dcba 15a2 9e87 6ee6 93e8 4ff4 6bee  ........n...O.k.
+000024c0: f816 5e01 af39 8c64 9385 07e6 fb72 b5fe  ..^..9.d.....r..
+000024d0: ebcb df47 f7f7 5fe7 c97f 8fee febb bf9f  ...G.._.........
+000024e0: 3f2c be2e b99b 2bc7 d8d7 6504 c702 4678  ?,....+...e...Fx
+000024f0: 92b2 27d0 9323 18e8 1280 a380 00c9 1178  ..'..#.........x
+00002500: ba04 e028 20f0 e508 902e 0138 0a08 0239  ...( ......8...9
+00002510: 025f 9700 1c05 04a1 1c41 a04b 008e 0282  ._.......A.K....
+00002520: 488e 20d4 2500 4701 c155 42d0 6a66 91f5  H. .%.G..UB.jf..
+00002530: 7d32 c2c4 e733 2e24 12ec f338 b22e 6deb  }2...3.$...8..m.
+00002540: f66b 1cfc 213e 424c 5fac 568b 9fb6 b548  .k..!>BL_.V....H
+00002550: 3282 b55a de5d da43 f020 1962 fee3 feee  2..Z.].C. .b....
+00002560: e1e8 baf7 31f2 274c 0c75 ea68 e4cd bdde  ....1.'L.u.h....
+00002570: 14d5 ea56 168f 7074 655e b1df dc3f bec3  ...V..pte^...?..
+00002580: e1cb ae59 6f2d f26e d1c8 fcdd 48e4 7efd  ...Yo-.n....H.~.
+00002590: a137 9ca1 57ec 8caf c932 d1ab d26e b136  .7..W....2...n.6
+000025a0: a36c 552a 1285 53f7 6637 3d9c 1e6b b5c6  .lU*..S.f7=..k..
+000025b0: d949 db81 4411 67c9 9284 d152 4918 d818  .I..D.g....RI...
+000025c0: 1206 fcc8 53eb 3997 7d13 9bc4 6419 a787  ....S.9.}...d...
+000025d0: 925b d607 1b72 cb20 73f4 0f9a 9738 4de0  .[...r. s....8M.
+000025e0: 3fbd 0fe8 a617 2018 e553 609a 18ea 16d8  ?..... ..S`.....
+000025f0: e739 25cd 90f9 d4d3 34f9 da8b 3e34 1c6e  .9%.....4...>4.n
+00002600: b107 34e3 9a24 b112 4a6c 9b53 0e14 29c1  ..4..$..Jl.S..).
+00002610: 5e82 92c9 1d0a 6c1e c3e6 29b2 81bd 221b  ^.....l...)...".
+00002620: 5260 c3b6 f9ba 2145 36b0 5764 f315 d8b0  R`....!E6.Wd....
+00002630: 6dce e62b b281 bd22 5ba0 c086 6d73 b640  m..+..."[...ms.@
+00002640: 910d ec15 d942 0536 6c9b b385 8a6c 60af  .....B.6l....l`.
+00002650: c816 29b0 61db 9c2d 5264 037b 45b6 2bc2  ..).a..-Rd.{E.+.
+00002660: e6e0 bcc6 4870 a86a e44b 1c6c cc45 d466  ....Hp.j.K.l.E.f
+00002670: 1ea9 e332 a89f d8b4 e007 c428 9964 883d  ...2.......(.d.=
+00002680: b61c 5993 dae3 17d7 71aa 232b c38a 43ab  ..Y.....q.#+..C.
+00002690: 3875 0f18 daad 44d8 0d5a 26c2 6a30 7a0c  8u....D..Z&.j0z.
+000026a0: e356 226d 2523 d260 c43e 5b8e b895 8cbe  .V"m%#.`.>[.....
+000026b0: 0623 f6d9 72e4 ad64 0c34 18b1 cf96 2370  .#..r..d.4....#p
+000026c0: 2563 a8c1 887d b61c 892b 19a3 8431 0941  %c...}...+...1.A
+000026d0: 02c5 846d b71c 8913 3612 79e8 cff2 1559  ...m....6.y....Y
+000026e0: bbcd 287c ac12 85b1 711c 85d3 7e50 3f19  ..(|....q...~P?.
+000026f0: 39ce 8a96 013f e0f1 0388 1ff0 f981 801f  9....?..........
+00002700: 08f9 8188 1fb8 4a06 5a9b f383 0e8c 7c96  ......J.Z.....|.
+00002710: c1c6 7c96 e1bb 6689 0d35 637e c0e3 0710  ..|...f..5c~....
+00002720: 3fe0 f303 013f 10f2 0311 35c0 64d1 5395  ?....?....5.d.S.
+00002730: f961 63be 2e69 7375 09b1 39e3 3a56 74dd  .ac..isu..9.:Vt.
+00002740: 014d 37aa e688 1b55 7dae 5195 f5a6 ea16  .M7....U}.Q.....
+00002750: 74b7 6ec6 7f4c a096 646a 9112 b7b0 371c  t.n..L..dj....7.
+00002760: cea0 1596 7a15 34f2 e26c 3fc8 38e3 1a6b  ....z.4..l?.8..k
+00002770: b3c3 4629 1b5d 5ea6 2a51 e465 32a9 8095  ..F).]^.*Q.e2...
+00002780: ce93 baac 4c95 62c0 8a04 ac74 85a2 cbca  ....L.b....t....
+00002790: 542d 06ac be80 95ae 5874 5999 2ac6 8035  T-......XtY.*..5
+000027a0: 10b0 d215 8c2e 2b53 d518 b086 0256 baa2  ......+S.....V..
+000027b0: d165 65aa 1c03 d648 c04a 5738 baac 4cd5  .ee....H.JW8..L.
+000027c0: a3c7 cac4 ec33 9598 8d8d d99c 4b46 4ed3  .....3......KFN.
+000027d0: a6d1 faf3 62b5 fc64 270d befe d945 0406  ....b..d'....E..
+000027e0: a4e7 b7fe 023b 4576 97eb 1bf5 4f1b f4f6  .....;Ev....O...
+000027f0: d0e6 5649 1261 b3eb d011 1637 b4c8 f598  ..VI.a.....7....
+00002800: 6b40 bc7b 6262 9e91 3732 f2f6 8dbc 0323  k@.{bb..72.....#
+00002810: efd0 c81b df3a 7cb7 e1a1 c60b 9db7 dc44  .....:|........D
+00002820: 6bce 3c5f d00e 96d7 3cd8 98d7 3c4d 4e13  k.<_....<...<MN.
+00002830: 109b 2a4d 3018 cf46 53ba f7bb 5b59 001b  ..*M0..FS...[Y..
+00002840: 7da5 ca20 a315 2b03 036a 1d71 4051 339f  }.. ..+..j.q@Q3.
+00002850: 1501 31ad 0f0c 8875 2442 0931 1210 d32a  ..1....u$B.1...*
+00002860: c180 5847 2894 10fb 0262 5a2b 1810 ebc8  ..XG(....bZ+....
+00002870: 8512 e240 404c 2b06 0362 1dd1 5042 1c0a  ...@@L+..b..PB..
+00002880: 8869 dd60 40ac 231d 4a88 2301 31ad 1e0c  .i.`@.#.J.#.1...
+00002890: 8875 04c4 2631 13e3 5d47 25c8 c7d6 ac8a  .u..&1..]G%.....
+000028a0: 4887 4a64 84eb 5c44 d884 4af2 70aa 8417  H.Jd..\D..J.p...
+000028b0: 12e7 5242 22bf 9438 abc5 274b 5825 61e6  ..RB"..8..'KX%a.
+000028c0: 8ecc dc7d 33f7 c0cc 3d34 738f efa0 ac9e  ...}3...=4s.....
+000028d0: 6056 9e7d d6d4 4e23 91f3 3fd0 f8cf 763f  `V.}..N#..?...v?
+000028e0: 9bdc 166d df25 46a4 574f 6dd4 0af7 38b7  ...m.%F.WOm...8.
+000028f0: 2b2c 10ec 32cf 7bb3 e9b8 a0e5 50bc 29ca  +,..2.{.....P.).
+00002900: a0a7 124d 76eb 531e 5e46 5f54 c033 fa42  ...Mv.S.^F_T.3.B
+00002910: 805c dda7 9747 9611 1892 c848 805c bd51  .\...G.....H.\.Q
+00002920: 2a8f 2ca3 3024 917d 0172 f5fe a93c b28c  *.,.0$.}.r...<..
+00002930: c490 440e 04c8 d5db aaf2 c832 1a43 1239  ..D........2.C.9
+00002940: 1420 57ef b6ca 23cb 880c 49e4 4880 5cbd  . W...#...I.H.\.
+00002950: 092b 8f2c a332 c4c8 6ce4 c747 69e4 cfa1  .+.,.2..l..Gi...
+00002960: 9283 37f8 84e6 5397 df9e 7593 578f 2b1a  ..7...S...u.W.+.
+00002970: cb3b 2e22 0b26 5f55 4766 c07b af23 abc1  .;.".&_UGf.{.#..
+00002980: d950 9fae 7231 f433 9692 f2d0 48b0 d2cf  .P..r1.3....H...
+00002990: 584d ca43 fb02 e867 2c28 e5a1 0301 f433  XM.C...g,(.....3
+000029a0: d694 f2d0 a100 fa19 cb4a 79e8 4800 fd8c  .........Jy.H...
+000029b0: 95a5 1434 1bf6 f1a1 1df9 b09f 1cf1 81e3  ...4............
+000029c0: 8ed9 b6b0 4b86 ca8a cb16 1497 d941 240b  ....K........A$.
+000029d0: 77a9 e170 3d5f 5cba 4db9 ea32 bb96 b8ba  w..p=_\.M..2....
+000029e0: 8c4f d772 d5a5 913b ca67 aa73 75df cc3d  .O.r...;.g.su..=
+000029f0: 3073 0fcd dce3 5b28 5b5d 322b cf3e 6cf8  0s....[([]2+.>l.
+00002a00: 6c82 fcc3 969c 6460 ced6 36f9 3d6c fc8d  l.....d`..6.=l..
+00002a10: 1900 7b69 52c3 c6a7 a51d 38b8 cb7e c963  ..{iR.....8..~.c
+00002a20: 73ef bcf0 131b 9fb7 76ed d2b6 7736 e997  s.......v...w6..
+00002a30: 2957 b63a 7956 f2a4 77fb 654a 9e9d 4d1c  )W.:yV..w.eJ..M.
+00002a40: 09ee f8be 65d3 ce26 ee0b 26be 6fe9 b5b3  ....e..&..&.o...
+00002a50: 8907 8289 ef5b beed 6ce2 a160 e2fb 9680  .....[..l..`....
+00002a60: 3b9b 7824 98f8 be65 e42e 26ce aa03 a503  ;.x$...e..&.....
+00002a70: 8aee e609 c574 a84c 8a1e 8314 052f 6a9f  .....t.L...../j.
+00002a80: 03da 171b 52b4 2d27 45c9 e565 b6ef 63b5  ....R.-'E..e..c.
+00002a90: cc49 5123 7794 cf54 2c45 37af ee9b b907  .IQ#w..T,E7.....
+00002aa0: 66ee a199 7b7c 0b65 a528 3377 f661 533a  f...{|.e.(3w.aS:
+00002ab0: 2dea 66c7 450b bf5d 9d9e d82c dfdb d847  -.f.E..]...,...G
+00002ac0: bbcb 2dd7 8f29 f0cb d48f 1938 abfd aaa1  ..-..).....8....
+00002ad0: f7dd ee2a 8446 e4c1 814f 3b75 c8a7 f82b  ...*.F...O;u...+
+00002ae0: 093b 3e3c 5158 6814 42fb 02e8 7d6b ae42  .;><QXh.B...}k.B
+00002af0: e840 00bd 6fbd 5408 1d0a a0f7 ad75 0aa1  .@..o.T......u..
+00002b00: 2301 f4be 750a 0fcd 867d fa10 3d9c 08a9  #...u....}..=...
+00002b10: fe65 1bd9 21fa bcdb 4586 ca24 c629 480c  .e..!...E..$.)H.
+00002b20: 30a1 2446 bb40 629c c849 8cec 5ae2 24df  0.$F.@b..I..Z.$.
+00002b30: c60d 394e 6218 b923 3c0d d934 bb79 75df  ..9Nb..#<..4.yu.
+00002b40: cc3d 3073 0fcd dce3 5ba8 35f7 e459 6be4  .=0s....[.5..Yk.
+00002b50: bfe4 e57f 0000 00ff ff00 0000 ffff 448c  ..............D.
+00002b60: 410e 8230 1045 afd2 cc01 4411 2535 9495  A..0.E....D.%5..
+00002b70: 1b17 ae38 410d 433b 513b cd30 8684 d30b  ...8A.C;Q;.0....
+00002b80: 26c4 dd7f ef27 afc9 3ee0 dd4b a034 9a17  &....'..>..K.4..
+00002b90: 0eea 60bf abc1 0885 b86d e5fc b327 300f  ..`......m...'0.
+00002ba0: 56e5 f746 117d 8fb2 d211 ccc0 ac1b 146d  V..F.}.........m
+00002bb0: b376 3bd4 4f36 d967 948e 6674 60c1 b010  .v;.O6.g..ft`...
+00002bc0: 26f5 4a9c 1c64 1615 4f0a 262e 7ee6 e578  &.J..d..O.&.~..x
+00002bd0: 5d33 39a8 4a5b d973 5dda 252c 17ea 1dc8  ]39.J[.s].%,....
+00002be0: ad3f c0d2 edc5 4f94 c2df 96ab 2d26 96e7  .?....O.....-&..
+00002bf0: 1811 b5fd 0200 00ff ff03 0050 4b03 0414  ...........PK...
+00002c00: 0006 0008 0000 0021 00b5 902c ddb7 0400  .......!...,....
+00002c10: 0069 0f00 0018 0000 0078 6c2f 776f 726b  .i.......xl/work
+00002c20: 7368 6565 7473 2f73 6865 6574 332e 786d  sheets/sheet3.xm
+00002c30: 6c9c 93df 6bdb 3010 c7df 07fb 1f84 de63  l...k.0........c
+00002c40: 494e da35 264e 1994 d042 1fc6 58bb 6745  IN.5&N...B..X.gE
+00002c50: 3ec7 2296 6424 b949 18fb df77 529a 7490  >.".d$.I...wR.t.
+00002c60: 9750 23eb 87ef fcb9 3bdf d78b fbbd e9c9  .P#.....;.......
+00002c70: 1bf8 a09d ada9 2838 2560 956b b4dd d4f4  ......(8%`.k....
+00002c80: e5d7 6a72 4749 88d2 36b2 7716 6a7a 8040  ..jrGI..6.w.jz.@
+00002c90: ef97 5fbf 2c76 ce6f 4307 1009 126c a869  .._.,v.oC....l.i
+00002ca0: 17e3 5031 1654 0746 86c2 0d60 d1d2 3a6f  ..P1.T.F...`..:o
+00002cb0: 64c4 a3df b030 7890 4d7e c9f4 ace4 fc96  d....0x.M~......
+00002cc0: 19a9 2d3d 122a 7f0d c3b5 ad56 f0e0 d468  ..-=.*.....V...h
+00002cd0: c0c6 23c4 432f 23e6 1f3a 3d84 13cd a86b  ..#.C/#..:=....k
+00002ce0: 7046 faed 384c 9433 0322 d6ba d7f1 90a1  pF..8L.3."......
+00002cf0: 9418 553d 6dac f372 dd63 dd7b 3193 8aec  ..U=m..r.c.{1...
+00002d00: 3d8e 12ef e929 4c7e 7e11 c968 e55d 706d  =....)L~~..h.]pm
+00002d10: 2c90 cc8e 395f 963f 6773 26d5 9974 59ff  ,...9_.?gs&..tY.
+00002d20: 5518 3163 1ede 746a e007 aafc 5c4a e2e6  U.1c..tj....\J..
+00002d30: cc2a 3f60 d34f c26e cfb0 f4b9 7c35 eaa6  .*?`.O.n....|5..
+00002d40: a67f f8fb 35c1 55a4 894f 386a 21ef 4eb6  ....5.U..O8j!.N.
+00002d50: bf74 b968 3476 3855 453c b435 fd2e aa67  .t.h4v8UE<.5...g
+00002d60: 7147 d972 9105 f4aa 6117 fedb 93a4 c7b5  qG.r....a.......
+00002d70: 73db 6478 c238 3cb9 b20b df55 d6e3 0f4f  s.dx.8<....U...O
+00002d80: 1a68 e5d8 c79f 6ef7 087a d345 14ff ac98  .h....n..z.E....
+00002d90: 619e a9d1 5573 7880 a050 6108 2aa6 09a5  a...Usx..Pa.*...
+00002da0: 5c8f f170 2646 a73f 0505 22f7 79dd e926  \..p&F.?..".y..&
+00002db0: 7635 2d79 21f8 7cfa ed86 9235 84b8 d209  v5-y!.|....5....
+00002dc0: 4989 1a43 74e6 f7d1 47e4 a432 ea1f 0000  I..Ct...G..2....
+00002dd0: 00ff ff00 0000 ffff 9c56 6d8f 9a40 10fe  .........Vm..@..
+00002de0: 2b5b 7ab9 404b 8aab f876 a726 8018 ad28  +[z.@K...v.&...(
+00002df0: a962 7ae9 970b 45bc 4b6a 4f83 9c77 fefb  .bz...E.KjO..w..
+00002e00: ceb2 cab2 ab56 f7fc 24b3 c33c 33cf 0ccf  .....V..$..<3...
+00002e10: 6c6b f31c c769 374c c34e 2b59 bda1 a4ad  lk...i7L.N+Y....
+00002e20: 6005 6dd6 e1cb 06fe dde1 b282 deb1 1946  `.m............F
+00002e30: 77f3 5d37 de44 f14b da56 4adf 2a4a a715  w.]7.D.K.VJ.*J..
+00002e40: 115f 0b9c c1b2 81e7 6da7 5c6d 19db 4ecb  ._......m.\m..N.
+00002e50: 88f6 8736 a666 deda e55e a9f1 8703 02de  ...6.f...^......
+00002e60: 56ca 551a 364d 20c2 a2a3 38ab bfeb d734  V.U.6M ...8....4
+00002e70: 9ea3 285e 2e37 e839 dcc6 2844 3b78 8094  ..(^.7.9..(D;x..
+00002e80: 7f87 d19f a764 f5fa 3257 5ac6 8224 72a5  .....d..2WZ..$r.
+00002e90: 3b0f fd3d 8736 f6f9 0f8f 2c5e d162 005f  ;..=.6....,^.b._
+00002ea0: 3969 c0d3 f5a4 8133 23ad 2e90 56ce 48c3  9i.....3#...V.H.
+00002eb0: 0269 dc2b 8dfc 90cb a122 9303 38b3 1c9a  .i.+....."..8...
+00002ec0: 420e a4bf d0cf d330 a60c 0c38 e730 9592  B......0...8.0..
+00002ed0: 0063 6630 95d3 3030 02d7 33ba 9f17 1a4f  .cf0..00..3....O
+00002ee0: e0ce ae66 6656 2347 5a4d 0606 9c59 358c  ...ffV#GZM...Y5.
+00002ef0: 9eec 53b0 6bb4 71ac 480e a72e 8303 ce0c  ..S.k.q.H.......
+00002f00: 87f1 4371 ea14 8755 c9e1 3464 70c0 39c7  ..Cq...U..4dp.9.
+00002f10: 314d a13b 0d8a 7366 0a9a 3238 e0cc 7044  1M.;..sf..28..pD
+00002f20: 9568 529c 3363 804b 5272 04de 8c39 b122  .hR.3c.KRr...9."
+00002f30: 8845 e61a 333b 471d 9653 bea2 8e55 8ea4  .E..3;G..S...U..
+00002f40: 8f6a 1f66 761e 4a4a 2f88 0ab3 aa04 c9b4  .j.fv.JJ/.......
+00002f50: e134 ab8a d979 2829 59c0 455d a81d 5545  .4...y()Y.E]..UE
+00002f60: 8501 33cd e2a1 a4a4 0173 da20 ca20 39a5  ..3......s. . 9.
+00002f70: 9b00 3600 8a42 b297 3a8e 3f1b 0796 eaf7  ..6..B..:.?.....
+00002f80: 7a53 3750 ddf7 75fc e9c6 bac1 3aea bb56  zS7P..u.....:..V
+00002f90: d79d 3c4e 07bf 5c1d 79de e8d1 f13d 1dd9  ..<N..\.y....=..
+00002fa0: 9eef 0cf7 46ac 69fb ed70 e6c3 c152 8243  ....F.i..p...R.C
+00002fb0: bc59 4b98 20d3 4f34 8b95 adb1 2b92 2fe6  .YK. .O4....+./.
+00002fc0: fe63 e64e 8381 3fa6 f9e3 52f6 d3d1 e5e4  .c.N..?...R.....
+00002fd0: a564 0c73 3a26 8a3f 39bd 9af9 62f2 3dcb  .d.s:&.?9...b.=.
+00002fe0: 09a4 132f eae2 c5cb 4651 174d 719b 6012  .../....FQ.Mq.`.
+00002ff0: 2abf 3bc4 e4e6 405a 1426 49b8 5350 4847  *.;...@Z.&I.SPHG
+00003000: 0825 f1a2 add8 c477 3f53 232b 70fa 6a30  .%.....w?S#+p.j0
+00003010: 99c1 e48c fd40 1d4c 6dcf 1a0f 8f87 ac50  .....@.Lm......P
+00003020: ea57 ac9f ef94 a6a3 d261 d63e 8f0d ebf4  .W.......a.>....
+00003030: 7ac3 45a1 be58 3827 d4e2 7ecb 42e5 d376  z.E..X8'..~.B..v
+00003040: b664 8891 97fc a08e ac07 f5bf 35ea 4e7f  .d..........5.N.
+00003050: 361e 66fd a473 a863 ed76 99de df3e a5f7  6.f..s.c.v...>..
+00003060: 8aa2 a12f 489d f83f a543 681a f073 193c  .../H..?.Ch..s.<
+00003070: 9fa5 0f63 1f47 b812 fa20 1f1f 463e 0a00  ...c.G... ..F>..
+00003080: c087 8110 b79c c1ee dfff 0000 00ff ff00  ................
+00003090: 0000 ffff b229 484c 4ff5 4d2c 4acf cc2b  .....)HLO.M,J..+
+000030a0: 56c8 494d 2bb1 5532 d033 5752 28ca 4ccf  V.IM+.U2.3WR(.L.
+000030b0: 80b1 4bf2 0bc0 a2a6 4a0a 49f9 2525 f9b9  ..K.....J.I.%%..
+000030c0: 305e 466a 624a 6a11 8867 aca4 9096 9f5f  0^FjbJj..g....._
+000030d0: 02e3 e8db d9e8 97e7 1765 1767 a4a6 96d8  .........e.g....
+000030e0: 0100 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+000030f0: 0800 0000 2100 b145 0dec 5c07 0000 0221  ....!..E..\....!
+00003100: 0000 1300 0000 786c 2f74 6865 6d65 2f74  ......xl/theme/t
+00003110: 6865 6d65 312e 786d 6cec 594b 8f1b 3712  heme1.xml.YK..7.
+00003120: be07 c87f 20fa 2eeb d5ad c7c0 b2a1 a727  .... ..........'
+00003130: f68c 6d78 642f 72e4 4894 9a1e 7653 20a9  ..mxd/r.H...vS .
+00003140: 190b 8181 c039 e512 2040 76b1 9705 f6b6  .....9.. @v.....
+00003150: 8720 4880 0458 2397 fc18 0336 b2d9 1fb1  . H..X#....6....
+00003160: 4576 4b4d 8ea8 786c 8f17 4e30 33c0 8c9a  EvKM..xl..N03...
+00003170: faaa 58ac 2a7e ac2e 5ebf f924 61e8 9408  ..X.*~..^..$a...
+00003180: 4979 da09 aad7 2a01 22e9 844f 693a ef04  Iy....*."..Oi:..
+00003190: 0fc7 a352 2b40 52e1 748a 194f 4927 5811  ...R+@R.t..OI'X.
+000031a0: 19dc bcf1 f147 d7f1 9e8a 4942 10c8 a772  .....G....IB...r
+000031b0: 0f77 8258 a9c5 5eb9 2c27 308c e535 be20  .w.X..^.,'0..5. 
+000031c0: 297c 37e3 22c1 0a1e c5bc 3c15 f80c f426  )|7.".....<....&
+000031d0: ac5c ab54 1ae5 04d3 3440 294e 40ed bdd9  .\.T....4@)N@...
+000031e0: 8c4e 08aa 55aa 7554 827f b51a 1a6b f5c1  .N..U.uT.....k..
+000031f0: 8df5 4443 068f a992 7a60 c2c4 919e 86ec  ..DC....z`......
+00003200: 9436 72d3 93aa 46cb 95ec 3381 4e31 eb04  .6r...F...3.N1..
+00003210: 30ff 949f 8dc9 1315 2086 a582 2f3a 41c5  0....... .../:A.
+00003220: fc04 e51b d7cb 782f 1762 6a87 ac25 3732  ......x/.bj..%72
+00003230: 3fb9 5c2e 303d a999 39c5 fc78 3369 1846  ?.\.0=..9..x3i.F
+00003240: 61a3 bbd1 6f00 4c6d e386 cd61 63d8 d8e8  a...o.Lm...ac...
+00003250: 3300 3c99 c0aa 335b 5c9d cd5a 3fcc b116  3.<...3[\..Z?...
+00003260: 28fb e8d1 3d68 0eea 5507 6fe9 af6f d9dc  (...=h..U.o..o..
+00003270: 8df4 af83 37a0 4c7f b885 1f8d fae0 4507  ....7.L.......E.
+00003280: 6f40 193e dac2 47bd 766f e0ea 37a0 0cdf  o@.>..G.vo..7...
+00003290: d8c2 372b dd41 d874 f41b 50cc 687a b285  ..7+.A.t..P.hz..
+000032a0: ae44 8d7a 7fbd da0d 64c6 d9be 17de 8ec2  .D.z....d.......
+000032b0: 51b3 962b 2f50 900d 9b4c d353 cc78 aa2e  Q..+/P...L.S.x..
+000032c0: 9277 097e ccc5 08c0 5a88 6145 53a4 560b  .w.~....Z.aES.V.
+000032d0: 32c3 13c8 f43e 66f4 5850 7440 e731 24e1  2....>f.XPt@.1$.
+000032e0: 02a7 5cc2 70a5 5619 55ea f057 ff86 e693  ..\.p.V.U..W....
+000032f0: 892e de23 d892 d636 8255 726b 48db 86e4  ...#...6.UrkH...
+00003300: 44d0 85ea 04b7 416b 6041 5e3e 7ffe e2d9  D.....Ak`A^>....
+00003310: 4f2f 9efd fbc5 175f bc78 f67d 3eb7 51e5  O/....._.x.}>.Q.
+00003320: c8ed e374 6ecb fdf6 afaf fffb 8fcf d17f  ...tn...........
+00003330: 7efc e76f dffc 359b fa3c 5eda f857 df7d  ~..o..5..<^..W.}
+00003340: f9ea e75f 7e4f 3dac b870 c5cb bffd f0ea  ..._~O=..p......
+00003350: a71f 5efe fdab 5fbf fdc6 a3bd 2bf0 b10d  ..^..._.....+...
+00003360: 1fd3 8448 7497 9ca1 073c 8105 7aec 27c7  ...Ht....<..z.'.
+00003370: e2cd 24c6 31a6 8e04 8e41 b747 f550 c50e  ..$.1....A.G.P..
+00003380: f0ee 0a33 1fae 475c 173e 12c0 383e e0ad  ...3..G\.>..8>..
+00003390: e563 c7d6 a358 2c15 f5cc 7c27 4e1c e021  .c...X,...|'N..!
+000033a0: e7ac c785 d701 77f4 5c96 87c7 cb74 ee9f  ......w.\....t..
+000033b0: 5c2c 6ddc 038c 4f7d 73f7 71ea 0478 b85c  \,m...O}s.q..x.\
+000033c0: 00ed 529f ca7e 4c1c 33ef 339c 2a3c 2729  ..R..~L.3.3.*<')
+000033d0: 5148 7fc7 4f08 f1ac ee53 4a1d bf1e d289  QH..O....SJ.....
+000033e0: e092 cf14 fa94 a21e a65e 978c e9b1 9348  .........^.....H
+000033f0: 85d0 3e4d 202e 2b9f 8110 6ac7 3787 8f50  ..>M .+...j.7..P
+00003400: 8f33 dfaa 07e4 d445 c2b6 c0cc 63fc 9830  .3.....E....c..0
+00003410: c78d b7f0 52e1 c4a7 728c 1366 3bfc 00ab  ....R...r..f;...
+00003420: d867 e4d1 4a4c 6cdc 502a 88f4 9c30 8e86  .g..JLl.P*...0..
+00003430: 5322 a54f e69e 80f5 5a41 bf03 0ce3 0ffb  S".O....ZA......
+00003440: 215b 252e 5228 7ae2 d379 8039 b791 037e  ![%.R(z..y.9...~
+00003450: d28f 71b2 f0da 4cd3 d8c6 7e22 4f20 4531  ..q...L...~"O E1
+00003460: bacf 950f 7ec8 dd1d a29f 210e 38dd 19ee  ....~.....!.8...
+00003470: 4794 38e1 7e3d 113c 0472 b54d 2a12 447f  G.8.~=.<.r.M*.D.
+00003480: b314 9e58 de22 dcdd 8f2b 36c3 c4c7 325d  ...X."...+6...2]
+00003490: 9138 ecda 15d4 9b1d bde5 dc49 ed03 4218  .8.........I..B.
+000034a0: 3ec3 5342 d0c3 4f3c 16f4 f8c2 f179 61f4  >.SB..O<.....ya.
+000034b0: ed18 5865 9ff8 12eb 3676 7355 3fa7 4412  ..Xe....6vsU?.D.
+000034c0: 646a 9c6d 8a3c a0d2 49d9 2332 e73b ec39  dj.m.<..I.#2.;.9
+000034d0: 5c9d 239e 154e 132c 7669 be0b 5177 5217  \.#..N.,vi..QwR.
+000034e0: 4e39 2f95 de63 9313 1b78 9742 8908 f9e2  N9/..c...x.B....
+000034f0: 75ca 3d09 3aac e41e eed2 7a3f c6ce d9a5  u.=.:.....z?....
+00003500: 9fa5 3f5f 57c2 89df 45f6 18ec cbc7 6fba  ..?_W...E.....o.
+00003510: 2f41 86bc b10c 10fb 857d 33c6 cc99 a048  /A.......}3....H
+00003520: 9831 8602 c347 b720 e284 bf10 d1e7 aa11  .1...G. ........
+00003530: 5b7a e566 eea6 2dc2 0045 9253 ef24 347d  [z.f..-..E.S.$4}
+00003540: 6df1 73ae ec89 fe3f 658f bf80 b984 82c7  m.s....?e.......
+00003550: aff8 5d4a 9d5d 94b2 7fae c0d9 85fb 0396  ..]J.]..........
+00003560: 3503 bc4c ef13 3849 b639 ebaa aab9 aa6a  5..L..8I.9.....j
+00003570: 823f 7d55 b36b 2f5f d532 57b5 cc55 2de3  .?}U.k/_.2W..U-.
+00003580: 7bfb 7a2f b54c 51be 4065 5374 7c4c ff27  {.z/.LQ.@eSt|L.'
+00003590: b950 fb67 4619 3b52 2b46 0ea4 e900 4978  .P.gF.;R+F....Ix
+000035a0: bb99 8e60 d0b4 a94c df72 d31a 5cc4 f031  ...`...L.r..\..1
+000035b0: 6f3c 39b8 b9c0 4606 09ae fe42 557c 14e3  o<9...F....BU|..
+000035c0: 05b4 89aa a6b1 3997 b9ea b944 0b2e a17b  ......9....D...{
+000035d0: 6486 4deb 959c d36d 7a50 cbe4 904f b30e  d.M....mzP...O..
+000035e0: 68b5 aabb 9d99 3b25 56c5 7825 da8c 43c7  h.....;%V.x%..C.
+000035f0: 4a65 e846 b3e8 ea6d d49b 3ee9 dc74 62d7  Je.F...m..>..tb.
+00003600: 0668 d937 31c2 9acc 35a2 ee31 a2b9 1e84  .h.71...5..1....
+00003610: 88fc 9e11 6665 9762 45db 6345 4bab 5f87  ....fe.bE.cEK._.
+00003620: 6a1d c58d 2bc0 b44d 54e0 f51b c14b 7b27  j...+..MT....K{'
+00003630: 88c2 acb3 0c8d 3928 d5a7 3a4e 5993 791d  ......9(..:NY.y.
+00003640: 5d1d 9c4b 8df4 2e67 323b 03a0 dc5e 6740  ]..K...g2;...^g@
+00003650: 11e9 b6b6 75e7 f2f4 eab2 54bb 40a4 1d23  ....u.....T.@..#
+00003660: ac74 738d b0d2 3086 97e2 3c3b ed56 fc65  .ts...0...<;.V.e
+00003670: c6ba 5d84 d431 4fbb 62bd 1b0a 339a adf7  ..]..1O.b...3...
+00003680: 116b 4d28 e7b8 81a5 3653 b014 9d75 8246  .kM(....6S...u.F
+00003690: 3d82 5b98 095e 7482 1974 8fe1 63b2 80dc  =.[..^t..t..c...
+000036a0: 91fa 0d0c b339 5cd3 4c94 c836 fcdb 30cb  .....9\.L..6..0.
+000036b0: 4248 35c0 32ce 1c6e 4827 6383 842a 2210  BH5.2..nH'c..*".
+000036c0: a349 27d0 cbdf 6403 4b0d 8718 dbaa 3520  .I'...d.K.....5 
+000036d0: 840f d6b8 36d0 ca87 661c 04dd 0d32 99cd  ....6...f....2..
+000036e0: c844 d961 b746 b4a7 b347 60f8 8c2b bcdf  .D.a.F...G`..+..
+000036f0: 1af1 b707 6b49 be84 701f c5d3 3374 cc96  ....kI..p...3t..
+00003700: e201 8614 8b9a 55ed c029 9570 8950 cdbc  ......U..).p.P..
+00003710: 39a5 7043 b621 b222 ffce 1d4c 39ed da57  9.pC.!."...L9..W
+00003720: 5426 87b2 71cc 1631 ce4f 149b cc33 b821  T&..q..1.O...3.!
+00003730: d18d 39e6 69e3 03eb 295f 3338 74db 85c7  ..9.i...)_38t...
+00003740: 737d c0be f3a9 fbfa a35a 7bce 22cd e2cc  s}.......Z{."...
+00003750: 7458 459f 9a7e 327d 7f87 bc65 5571 883a  tXE..~2}...eUq.:
+00003760: 5665 d46d deaf 65c1 75ed 35d7 41a2 7a4f  Ve.m..e.u.5.A.zO
+00003770: 89d7 9cba 1738 102c d38a c91c d3b4 c5db  .....8.,........
+00003780: 34ac 393b 1f75 4dbb c482 c0f2 4463 87df  4.9;.uM.....Dc..
+00003790: 3667 84d7 136f 7bf2 83dc f9ac d507 c4ba  6g...o{.........
+000037a0: c634 896f aed8 ed9b 6f7e fc18 c863 0077  .4.o....o~...c.w
+000037b0: 894b a6a4 0925 dc65 0b0c 455f 7633 99d1  .K...%.e..E_v3..
+000037c0: 066c 9127 2aaf 11e1 135a 0ada 093e ab44  .l.'*....Z...>.D
+000037d0: ddb0 5f8b faa5 4a2b 1a96 c27a 5829 b5a2  .._...J+...zX)..
+000037e0: 6ebd d48d a27a 7518 552b 835e ed29 1c2c  n....zu.U+.^.).,
+000037f0: 2a4e aa51 76bd 3f82 eb0c b6ca 2ff9 cdf8  *N.Qv.?...../...
+00003800: d645 7fb2 beb1 b936 e149 999b 8bfc b231  .E.....6.I.....1
+00003810: dc5c f457 6b17 bbe8 4714 08e8 b346 6dd4  .\.Wk...G....Fm.
+00003820: aeb7 7b8d 52bb de1d 95c2 41af 556a f71b  ..{.R.....A.Uj..
+00003830: bdd2 a0d1 6f0e 4683 7ed4 6a8f 9e06 e8d4  ....o.F.~.j.....
+00003840: 80c3 6ebd 1f36 86ad 52a3 daef 97c2 4645  ..n..6..R.....FE
+00003850: 2fa5 d52e 35c3 5aad 1b36 bbad 61d8 7d9a  /...5.Z..6..a.}.
+00003860: 9734 e085 8c4a 72bf 80ab 8d8d 37fe 0700  .4...Jr.....7...
+00003870: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00003880: 0021 00d2 e522 5543 0500 0048 1a00 000d  .!..."UC...H....
+00003890: 0000 0078 6c2f 7374 796c 6573 2e78 6d6c  ...xl/styles.xml
+000038a0: cc59 dd6f e238 107f 3fe9 fe87 28ad eee9  .Y.o.8..?...(...
+000038b0: 6812 2069 e108 ab85 36d2 4adb aa52 7bd2  h. i....6.J..R{.
+000038c0: 49d7 7b08 8903 d63a 31eb 385d d8d3 fdef  I.{....:1.8]....
+000038d0: 37b6 1330 dfd0 a6dd e581 c41f 33f3 b367  7..0........3..g
+000038e0: 3c9e 99f4 3ecc 5262 3c23 9663 9af9 a673  <...>.Rb<#.c...s
+000038f0: 619b 06ca 221a e36c ec9b 7f3e 068d 2bd3  a..."..l...>..+.
+00003900: c879 98c5 21a1 19f2 cd39 cacd 0ffd 5f7f  .y..!....9...._.
+00003910: e9e5 7c4e d0c3 0421 6e00 8b2c f7cd 09e7  ..|N...!n..,....
+00003920: d3ae 65e5 d104 a561 7e41 a728 8391 84b2  ..e....a~A.(....
+00003930: 34e4 d064 632b 9f32 14c6 b920 4a89 d5b4  4..dc+.2... J...
+00003940: 6dcf 4a43 9c99 8a43 378d 8e61 9286 ec4b  m.JC...C7..a...K
+00003950: 316d 4434 9d86 1c8f 30c1 7c2e 7999 461a  1mD4....0.|.y.F.
+00003960: 753f 8d33 cac2 1101 a833 a71d 46c6 ccf1  u?.3.....3..F...
+00003970: 58d3 98b1 4a88 ecdd 9093 e288 d19c 26fc  X...J.........&.
+00003980: 02f8 5a34 4970 8436 e176 ac8e 1546 4b4e  ..Z4Ip.6.v...FKN
+00003990: c0f9 659c 1cd7 b29b 2b6b 9fb1 1772 6a5b  ..e.....+k...rj[
+000039a0: 0c3d 63a1 3eb3 dfcb 8a34 4879 6e44 b4c8  .=c.>....4HynD..
+000039b0: b86f 7616 5d86 1af9 1483 8ebd b669 28ad  .ov.]........i(.
+000039c0: 0c69 0cfb 645f d8bf 7d2d 28ff c3c8 d5d3  .i..d_..}-(.....
+000039d0: b42a 4e2b 64ee 0699 5d11 9eef 25f4 3609  .*N+d...]...%.6.
+000039e0: d5fc fdf2 2e57 c9e2 d84a 536b 0ebf 2763  .....W...JSk..'c
+000039f0: 32e9 a669 37cf 7720 059b d517 f874 7ef6  2..i7.w .....t~.
+00003a00: fbd9 192c d3b6 7710 7456 0914 babb 91f1  ...,..w.tV......
+00003a10: b540 3987 adcd bb86 eadb c1e0 128e 8d2e  .@9.............
+00003a20: 71c1 2009 237e 90d8 5925 fefb bc11 b46d  q. .#~..Y%.....m
+00003a30: fb9f 728d 4fc6 c75b ebfe 763b f2cb e66e  ..r.O..[..v;...n
+00003a40: a544 9a56 acd2 32fa bd84 664b 0301 95ca  .D.V..2...fK....
+00003a50: f3d0 fd92 d16f 5920 86c0 40c0 6ac4 ac7e  .....oY ..@.j..~
+00003a60: 2fff 6e3c 8704 7a1c 213d a284 3283 c3e9  /.n<..z.!=..2...
+00003a70: 06a3 913d 5998 2235 6318 123c 6258 4c4b  ...=Y."5c..<bXLK
+00003a80: c214 93b9 ea6e 8a0e e910 ca79 2986 e329  .....n.....y)..)
+00003a90: 3a2d 2541 fd8f c4ac 7792 f59e 6bc2 efb8  :-%A....w...k...
+00003aa0: aef7 9125 d596 8392 3121 0b37 d312 0603  ...%....1!.7....
+00003ab0: 1dfd 1e78 648e 5816 40c3 28df 1fe7 5330  ...xd.X.@.(...S0
+00003ac0: 970c 2e0f a576 39ef c0ec 310b e74e d33d  .....v9...1..N.=
+00003ad0: 9e20 a704 c702 c578 288d 948d 47be 19c8  . .....x(...G...
+00003ae0: 9f3a f3a3 7200 6731 9a21 f082 e004 8515  .:..r.g1.!......
+00003af0: 6a80 854d 4a70 f201 6b1c 5116 c3c5 5839  j..MJp..k.Q...X9
+00003b00: d326 f057 5dfd 1e41 0907 7286 c713 f1e4  .&.W]..A..r.....
+00003b10: 740a ff23 ca39 5c1e fd5e 8cc3 31cd 4222  t..#.9\..^..1.B"
+00003b20: 0454 143a 255c a870 77fa 269f c0dd 579d  .T.:%\.pw.&...W.
+00003b30: ab75 6442 c449 124a 5100 3c42 843c 0811  .udB.I.JQ.<B.<..
+00003b40: 7f25 2be8 6789 e6cf a5c7 cab8 b811 c42b  .%+.g..........+
+00003b50: acbc 7c55 4855 0356 b042 24fd a422 128e  ..|UHU.V.B$.."..
+00003b60: 6727 91a5 4350 8034 2c2d 1756 7d3a 1863  g'..CP.4,-.V}:.c
+00003b70: 966c 47a5 2d45 b8d2 eda8 16d4 4638 9d92  .lG.-E......F8..
+00003b80: b9f0 75a5 173b 7d85 252f e903 57a8 cbbb  ..u..;}.%/..W...
+00003b90: f5d0 0e2d e815 96bb 221d 2116 c840 691b  ...-....".!..@i.
+00003ba0: 26c7 9357 6fcd 5cb5 5ddb adcb 1391 1ea1  &..Wo.\.].......
+00003bb0: 09d0 50a5 c755 4da8 d640 1eba 6dbb 7084  ..P..UM..@..m.p.
+00003bc0: c16e f03e 8adb c936 a390 7e24 789c a548  .n.>...6..~$x..H
+00003bd0: 9951 bf07 17a0 6a1a 13ca f077 302f 7173  .Q....j....w0/qs
+00003be0: 4630 8ed8 105a 382b 6821 0316 6b96 ec36  F0...Z8+h!..k..6
+00003bf0: ff5d 608e deb6 dac1 399e 8cdf 0eb9 8a35  .]`.....9......5
+00003c00: ad1e b669 19de d5ce 5586 7e8a ebd1 7a5d  ...i....U.~...z]
+00003c10: c7ba cd2e 6bd4 b6e3 d50f 72dd 51af c8d8  ....k.....r.Q...
+00003c20: eddf 4f56 9a66 0a3f eff6 d60f 7273 7b35  ..OV.f.?....rs{5
+00003c30: ebfd 7937 a27e 90eb 1ba1 39e5 d66b af5e  ..y7.~....9..k.^
+00003c40: c7d3 c28b f7df 5419 ccc9 a070 9f7f 3efa  ......T....p..>.
+00003c50: 2cd5 e930 547a f9a3 bcda 711b f396 b7e8  ,..0Tz....q.....
+00003c60: 8f50 cdc9 3221 88d2 43e7 f528 07a2 d203  .P..2!..C..(....
+00003c70: 51cd dbc7 21a6 a8f4 711c 89c8 0472 96ed  Q...!...q....r..
+00003c80: c6ae 1d42 5128 da1b 4d03 e4bd d1b4 ac6c  ...BQ(..M......l
+00003c90: d41d 0d5f 6a5c 6b72 137b dcda ae3d a823  ..._j\kr.{...=.#
+00003ca0: 8e7d 4b8d 8bfc f128 7dd7 19b3 9f1c 7c1e  .}K....(}.....|.
+00003cb0: 8550 d6b8 ea8e 1455 e5ec f5b6 2953 5d48  .P.....U....)S]H
+00003cc0: 6eb5 b47b 25e9 5e64 c286 a896 f9e6 9d48  n..{%.^d.......H
+00003cd0: f388 9604 8d0a 4c20 3b58 a4b6 eb04 f788  ......L ;X......
+00003ce0: 892c a2a2 009b d128 548d 6441 0228 e2d9  .,.....(T.dA.(..
+00003cf0: 32e9 1795 3c68 2feb 1670 e8b7 161f c282  2...<h/..p......
+00003d00: d3d2 3b59 30a7 dfab fc04 1c8c 653a a3d7  ..;Y0.......e:..
+00003d10: 332c c957 fc83 4c2e 0aee b2e2 b058 3a58  3,.W..L......X:X
+00003d20: 558c 92b0 20fc 7131 e89b cbf7 5b14 e322  U... .q1....[.."
+00003d30: 05cd 96b3 eef1 33e5 9285 6f2e df3f 8b02  ......3...o..?..
+00003d40: 8be3 0947 8566 fc73 0e15 1178 1a05 c3be  ...G.f.s...x....
+00003d50: f9ef cde0 b273 7d13 341b 57f6 e0aa d16e  .....s}.4.W....n
+00003d60: 21b7 d171 07d7 0db7 3d1c 5c5f 071d bb69  !..q....=.\_...i
+00003d70: 0fff d3ca feaf 28fa cbaf 1490 b439 ed6e  ......(......9.n
+00003d80: 4ee0 d300 2b17 5b82 7f58 f6f9 a6d6 50f0  N...+.[..X....P.
+00003d90: a59b 05d8 3af6 4ed3 b33f ba8e dd08 5ab6  ....:.N..?....Z.
+00003da0: d368 7be1 55e3 ca6b b98d c075 9ad7 5e7b  .h{.U..k...u..^{
+00003db0: 70e3 06ae 86dd 7de1 c701 db72 1cf5 9941  p.....}....r...A
+00003dc0: 8077 bb1c a788 e0ac d255 a521 bd17 9404  .w.......U.!....
+00003dd0: cd3d 8bb0 2a4d 58cb 4f40 fdff 0100 00ff  .=..*MX.O@......
+00003de0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00003df0: 0011 52c1 0387 0200 002e 0800 0014 0000  ..R.............
+00003e00: 0078 6c2f 7368 6172 6564 5374 7269 6e67  .xl/sharedString
+00003e10: 732e 786d 6c9c 55ed 6ed3 3014 fd8f c43b  s.xml.U.n.0....;
+00003e20: 5866 e2df 9a0e a181 b636 9397 66b4 5a9a  Xf.......6..f.Z.
+00003e30: b226 6188 aa8a bcc4 5922 62bb c44e 37de  .&a.....Y"b..N7.
+00003e40: 8a67 e0c9 709a 212a db9d 267e e6dc 73af  .g..p.!*..&~..s.
+00003e50: efc7 b937 a38b 475a 832d 6944 c5d9 189e  ...7..GZ.-iD....
+00003e60: 0c86 1010 96f1 bc62 f763 98c4 57c7 1f21  .......b.c..W..!
+00003e70: 1012 b31c d79c 9131 fc49 04bc 705f bf1a  .......1.I..p_..
+00003e80: 0921 81f2 6562 0c4b 2937 678e 23b2 9250  .!..eb.K)7g.#..P
+00003e90: 2c06 7c43 98b2 14bc a158 aacf e6de 119b  ,.|C.....X......
+00003ea0: 86e0 5c94 8448 5a3b ef86 c353 87e2 8a41  ..\..HZ;...S...A
+00003eb0: 90f1 96c9 31fc f01e 8296 553f 5ae2 f5c0  ....1.....U?Z...
+00003ec0: e929 7447 a272 47d2 bd69 8990 2a3b 3172  .)tG.rG..i..*;1r
+00003ed0: a43b 723a b037 7865 cbbe ebe0 15ce a4c1  .;r:.7xe........
+00003ee0: 444c 3ca8 1275 aebf c5b5 8e85 bf7f e950  DL<..u.........P
+00003ef0: 4c1e a58e cd79 4e0c 5f8f 0b83 3869 1bdc  L....yN._...8i..
+00003f00: 65af 0798 6049 742c 08e6 3a84 5ac9 756c  e...`It,..:.Z.ul
+00003f10: da52 6cc4 9be2 ba6e cdc2 c3e8 d65f 4646  .Rl....n....._FF
+00003f20: e15f 3ffb 3a96 5992 cfed c977 733f 131b  ._?.:.Y....ws?..
+00003f30: 9c29 3da8 c10a d26c 0974 0152 32c2 f704  .)=....l.t.R2...
+00003f40: fc9f 97ed 7d94 c40b e07f 4141 82e2 d922  ....}.....AA..."
+00003f50: 3466 7507 703f 59f0 e070 50da 5bf0 9495  4fu.p?Y..pP.[...
+00003f60: c878 6374 7c3d 3c07 272b a3c1 3e9a f8cb  .xct|=<.'+..>...
+00003f70: 349a 7d33 baf4 b696 e7c7 202e 55d1 40a9  4.}3...... .U.@.
+00003f80: 4749 13e0 8628 19b3 6e49 4ce5 dd24 7ed4  GI...(..nIL..$~.
+00003f90: a59e 7a8b 407f e640 2c5e 1482 4850 349c  ..z.@..@,^..HP4.
+00003fa0: 8223 7474 62c8 7e9a 84d7 b678 57c8 8b6d  .#ttb.~....xW..m
+00003fb0: b892 950d f616 516c a832 595a 3bdd cd20  ......Ql.2YZ;.. 
+00003fc0: eda6 6128 a933 4c93 3932 8633 4541 9018  ..a(.3L.92.3EA..
+00003fd0: ca0b 2f53 958e 0dfe db29 9bad abcc c02f  ../S.....)...../
+00003fe0: 8385 776d 1d92 7a64 b9b8 3555 cf72 905b  ..wm..zd..5U.r.[
+00003ff0: d64e b414 f0e2 906c dd28 46cb 389d a0d8  .N.....l.(F.8...
+00004000: 1083 1f4e acf8 1bbd 4bea aeed 4ed8 405a  ...N....K...N.@Z
+00004010: 4e49 d69d 31b1 aad6 566b d1dd b367 8d83  NI..1...Vk...g..
+00004020: baa6 69bf 0783 a2ad eb94 616a 087d 1766  ..i.......aj.}.f
+00004030: 9f69 5b37 8374 6093 5d83 282b aa2a c474  .i[7.t`.].(+.*.t
+00004040: a357 feb4 9f87 0ad8 33ef 5561 cbcd ce3c  .W......3.Ua...<
+00004050: 94a0 9dfd 922c 89da ea01 b65c ddbd 903b  .....,.....\...;
+00004060: 4e69 bbc2 3ac9 366f 9d43 89c4 2bd8 1f2f  Ni..:.6o.C..+../
+00004070: b87e a681 bb67 7bf6 5d4a 2b21 d43f da74  .~...g{.]J+!.?.t
+00004080: 98f7 8667 e2bc 442f f359 14cd c24f ffa2  ...g..D/.Y...O..
+00004090: 38ea 7fef fe01 0000 ffff 0300 504b 0304  8...........PK..
+000040a0: 1400 0600 0800 0000 2100 72a0 d0dc 5802  ........!.r...X.
+000040b0: 0000 c108 0000 1800 0000 786c 2f64 7261  ..........xl/dra
+000040c0: 7769 6e67 732f 6472 6177 696e 6731 2e78  wings/drawing1.x
+000040d0: 6d6c ec56 5d6f 9b30 147d 9fb4 ff60 f99d  ml.V]o.0.}...`..
+000040e0: 600c 230c 05aa e583 a9d2 d4f6 61fb 0196  `.#.........a...
+000040f0: 3101 0970 64bb 49aa aaff 7db6 3169 b625  1..pd.I...}.1i.%
+00004100: 6a53 ad0f 93c6 83b9 dccb bdd7 3ee7 1e92  jS..........>...
+00004110: d9d5 be6b c196 09d9 f03e 83c1 0441 c07a  ...k.....>...A.z
+00004120: cacb a65f 67f0 c7f7 c24b 2090 8af4 2569  ..._g....K ...%i
+00004130: 79cf 32f8 c024 bcca 3f7e 98ed 4b91 eee4  y.2..$..?~..K...
+00004140: 5200 5da0 97a9 7ecc 60ad d426 f57d 496b  R.]...~.`..&.}Ik
+00004150: d611 39e1 1bd6 eb68 c545 4794 7e14 6bbf  ..9....h.EG.~.k.
+00004160: 1464 a74b 77ad 8f11 8a7d b911 8c94 b266  .d.Kw....}.....f
+00004170: 4c2d 8708 74f5 c81b aa75 a4e9 616e 77a6  L-..t....u..anw.
+00004180: 767c c1da f64b 4f6b 2e06 5725 7837 5894  v|...KOk..W%x7X.
+00004190: b779 30f3 cd09 8c69 13b4 715b 55f9 34c6  .y0....i..q[U.4.
+000041a0: f121 621c 3628 f82e 0f92 c16f ecd1 695e  .!b.6(.....o..i^
+000041b0: c038 895d 8a0e d914 5bf9 b99d e247 6dd1  .8.]....[....Gm.
+000041c0: d9be e84c e330 bcac f1d8 6e2d c8a6 6e68  ...L.0....n-..nh
+000041d0: 2148 c740 47a8 e019 74e8 f4db af47 c13b  !H.@G...t....G.;
+000041e0: 0710 bdd9 de09 d094 190c 21e8 7556 0617  ..........!.uV..
+000041f0: 3511 0a60 9d46 52b6 57df a472 16b8 174d  5..`.FR.W..r...M
+00004200: 061f 8b02 cf3f ad8a c82b b4e5 4568 1e79  .....?...+..Eh.y
+00004210: f355 f4d9 2b70 98ac f0b4 58e0 307e 32d9  .U..+p....X.0~2.
+00004220: 419c 524d b5d2 5376 5d8e 1407 f11f 2477  A.RM..Sv].....$w
+00004230: 8dde a7e4 959a 50de f9bc aa1a cac6 a1d1  ......P.........
+00004240: 2313 44be 25d9 eef2 11b9 cbd3 f7c4 2cc8  #.D.%.........,.
+00004250: 4381 59cc 150e c127 e8e7 33df ee7e bcdb  C.Y....'..3..~..
+00004260: 530c ec9b 133b 726e 7ec3 c4a4 9909 398d  S....;rn~.....9.
+00004270: d5be 127a 9848 aa77 08f6 19d4 aa79 30ab  ...z.H.w.....y0.
+00004280: 4eb2 ad00 1d9c 74f4 da52 6392 63c6 bceb  N.....t..Rc.c...
+00004290: cc25 5164 80f4 6209 5143 9186 98a6 d672  .%Qd..b.QC.....r
+000042a0: d8d2 37c8 67a8 e40a bc4a cd03 3f4b 4eef  ..7.g....J..?KN.
+000042b0: 3bd6 ab41 d282 b596 6659 371b 0981 48cd  ;..A....fY7...H.
+000042c0: 4089 eb32 7044 1c9d d812 7200 c342 743c  @..2pD....r..Bt<
+000042d0: b48e 98b6 d1b5 0d40 2323 27b4 fdb2 dccf  .......@##'.....
+000042e0: e82e 8811 c2cf b157 293e 4cf4 901d 34f9  .......W)>L...4.
+000042f0: a2e2 a7a7 151f c551 72ae 7388 4f4b 3e40  .......Qr.s.OK>@
+00004300: 719c 9c6a fd17 341f fdaa f9f0 5fd4 7cf4  q..j..4....._.|.
+00004310: 5ff3 17fe 00bf afe6 f17b 69de 7e2b ccbf  _........{i.~+..
+00004320: 8ffc 2700 0000 ffff 0300 504b 0304 1400  ..'.......PK....
+00004330: 0600 0800 0000 2100 31b0 25e4 2609 0000  ......!.1.%.&...
+00004340: f433 0000 1400 0000 786c 2f63 6861 7274  .3......xl/chart
+00004350: 732f 6368 6172 7431 2e78 6d6c ec5b 5b6f  s/chart1.xml.[[o
+00004360: e3b8 157e 2fd0 ffa0 0a41 5f0a c7d6 c5d7  ...~/....A_.....
+00004370: 8eb3 b0e5 7831 6866 2798 64b7 408b 6241  ....x1hf'.d.@.bA
+00004380: 4bb4 a386 2235 2495 cb2c f607 f537 ece3  K..."5$..,...7..
+00004390: feb1 3dbc c896 1c67 9c38 4e9b 66e3 87c4  ..=....g.8N.f...
+000043a0: bc88 3a3c e7f0 f0fb 0ee9 77df dc64 c4b9  ..:<......w..d..
+000043b0: c25c a48c 0e5d efb0 e53a 98c6 2c49 e962  .\...]...:..,I.b
+000043c0: e87e 7f3e 6df4 5c47 4844 1344 18c5 43f7  .~.>m.\GHD.D..C.
+000043d0: 160b f79b a33f fee1 5d3c 882f 1097 6739  .....?..]<./..g9
+000043e0: 8ab1 0383 5031 8887 ee85 94f9 a0d9 14f1  ....P1..........
+000043f0: 05ce 9038 6439 a6d0 3667 3c43 128a 7cd1  ...8d9..6g<C..|.
+00004400: 4c38 ba86 c133 d2f4 5bad 4e53 0fe2 da01  L8...3..[.NS....
+00004410: d00e 0364 28a5 e5f3 fc21 cfb3 f93c 8df1  ...d(....!...<..
+00004420: 84c5 4586 a934 5270 4c90 040d 888b 3417  ..E..4RpL.....4.
+00004430: e568 b1d7 e1fe 9d11 b334 e64c b0b9 3c8c  .h.......4.L..<.
+00004440: 59d6 3483 9593 82c1 bc76 7339 ab23 5052  Y.4......vs9.#PR
+00004450: 8224 f6fa add0 b942 64e8 b6dc a6aa 2488  .$.....Bd.....$.
+00004460: 2e4c 05a6 8def cf4c 2567 054d 7012 314e  .L.....L%g.Mp.1N
+00004470: c11c 95fe 593c 1811 8939 85a1 2246 2548  ....Y<...9.."F%H
+00004480: 6df5 953d 48e3 19e2 9745 de00 7173 98e4  m..=H....E..qs..
+00004490: 2c25 a9bc d5d3 768f dec1 d8d1 0503 7d38  ,%....v.......}8
+000044a0: 9ff0 e722 e558 0cdd d80b 572a 081f ab80  ...".X....W*....
+000044b0: 56b7 d96b fad6 ae30 592f 1c08 794b b099  V..k...0Y/..yK..
+000044c0: 90d7 f2d5 6c9b cbf7 6a11 a688 9019 8a2f  ....l...j....../
+000044d0: 956e 2a9d 975d 57ed eac1 7565 a8a7 b41b  .n*..]W...ue....
+000044e0: a92f 3295 04eb 2f37 ea2f 4fe3 8ba3 7768  ./2.../7./O...wh
+000044f0: 3063 c9ed 2977 3893 ca08 8ec8 e369 ca85  0c..)w8......i..
+00004500: 3c41 429e 220e 7ee7 b96a 15c8 8ff0 674e  <AB.".~..j....gN
+00004510: d8f5 d0c5 8480 2fa4 e00d aa1e b4c0 f817  ....../.........
+00004520: d7b9 e628 1fba e273 8138 761d 4463 a806  ...(...s.8v.Dc..
+00004530: 8d49 5e16 2209 654f cd11 0d88 9067 6aea  .I^.".eO.....gj.
+00004540: ba90 ab9a fc94 ab7f 099e 7f02 69c4 17e8  ............i...
+00004550: 1ab6 409e 9996 2a35 b249 9e5e c24a a3ec  ..@...*5.I.^.J..
+00004560: 4c7f 739d 4bb0 3df4 84f5 a225 d7bd 6648  L.s.K.=....%..fH
+00004570: 6092 aa15 d902 33a2 8160 244d a629 21ba  `.....3..`$M.)!.
+00004580: a096 1f8e 0837 4a97 379e ee43 8aec 034b  .....7J.7..C...K
+00004590: 4c5d a7dd 82e1 8c98 45f6 713e 37d5 4159  L]......E.q>7.AY
+000045a0: dd84 21cb 51c0 5e6b 2f50 ab85 3af2 36c7  ..!.Q.^k/P..:.6.
+000045b0: 7358 fe43 f72f 196d 1069 86c3 68ad 0123  sX.C./.m.i..h..#
+000045c0: d310 8bb5 8658 685f 28f5 a15f 6335 a4d5  .....Xh_(.._c5..
+000045d0: c441 476a a90c dd39 6f4c 3f99 51e4 d139  .AGj...9oL?.Q..9
+000045e0: ce72 e160 e9c4 ecd7 5fa4 9323 b0eb afff  .r.`...._..#....
+000045f0: c961 f562 25a8 d4e3 c000 f01d 94de 2c9d  .a.b%.........,.
+00004600: 00be 48ed 130c 0c4a d06d 6d45 0afb 5eca  ..H....J.mmE..^.
+00004610: 940e 8d5a a852 65a5 2207 8799 2071 611e  ...Z.Re."... qa.
+00004620: d40a b7f2 13e8 0ac3 9b41 d47b 4a27 4485  .........A.{J'D.
+00004630: 64e7 aa30 c104 4b6c 756f a340 4e98 1c71  d..0..Kluo.@N..q
+00004640: 8c4c 44b8 6585 d4c1 6186 78a4 22ab aa86  .LD.e...a.x."...
+00004650: ef93 d45a 3166 c404 8a05 448a 1c42 a891  ...Z1f....D..B..
+00004660: 2326 8580 e080 13d3 7885 f86d c408 ab45  #&......x..m...E
+00004670: 1010 0d83 42e2 419a dcd4 a6cd 7882 edf0  ....B.A.....x...
+00004680: 5628 a322 21f9 273c 574f cc8f ce24 84ee  V(."!.'<WO...$..
+00004690: 3f1d 8c0e 0235 475d 09cd 1102 ef50 1d72  ?....5G].....P.r
+000046a0: 1941 e092 7679 1b21 72e9 c09b 8c6b c683  .A..vy.!r....k..
+000046b0: ab23 6704 2a47 0bec 2405 d771 568d 74a5  .#g.*G..$..qV.t.
+000046c0: 7596 2b73 a955 5f8e 680a faed 4b8b 95d6  u.+s.U_.h...K...
+000046d0: f99a 93a3 3886 c0a8 57de 1d6f ddd1 92a0  ....8...W..o....
+000046e0: 2faa 16ff fbf9 7778 0172 5fd9 2066 5595  /.....wx.r_. fU.
+000046f0: 9c6a 1bad ebf4 abcf cc8a d98c e060 b2d1  .j...........`..
+00004700: f9b6 ad61 1538 d717 e2ce 53c3 37f2 44e8  ...a.8....S.7.D.
+00004710: 09c0 37a7 e010 7c7e 8a82 a0d7 8aa2 b0d1  ..7...|~........
+00004720: 9e74 8e1b 61ab 1f35 c6c7 81df 38ee fa13  .t..a..5....8...
+00004730: bfdf 0dda 4114 fd5c d91e 1fbd 3986 957d  ....A..\....9..}
+00004740: a133 2868 fab9 c0ef edaa f809 0292 fa78  .3(h...........x
+00004750: 8d69 6f12 3642 f834 7ac7 41d8 087a 41d8  .io.6B.4z.A..zA.
+00004760: ed8c 47e3 91d7 fa59 afb8 7800 326b bf29  ..G....Y..x.2k.)
+00004770: 6701 ae62 cdb1 6e15 ed11 5b2c f924 abe8  g..b..n...[,.$..
+00004780: 485f 89ac 2a82 6e88 accb ea2d 91f5 f519  H_..*.n....-....
+00004790: 34d8 af41 352a d89f 41f9 62b6 dc28 43bf  4..A5*..A.b..(C.
+000047a0: d79e 8636 a8d7 56a3 8af0 bb6c 06da 535f  ...6..V....l..S_
+000047b0: e63a 6bef d72c 8109 fdfb 8a7e 55b3 4cfb  .:k..,.....~U.L.
+000047c0: d3f6 f1e8 7762 96ee 7ecd a2bd f979 56cb  ....wb..~....yV.
+000047d0: b41b f54c a4fb 1dec 4afd 279a e564 4684  ...L....J.'..dF.
+000047e0: a637 fb03 9a0a cf1a 3ef1 3cec 86bc a7c0  .7......>.<.....
+000047f0: 0683 9ea7 7887 d405 60b2 6d28 f06a cbac  ....x...`.m(.j..
+00004800: da72 3f23 d2bc 241f 0120 9ea6 0ae8 82cf  .r?#..$.. ......
+00004810: 18b1 1fca 94fa 8f23 4a4f 2548 ddcd 04c9  .......#JO%H....
+00004820: 7f21 0409 d344 1157 4523 d728 d292 f618  .!...D.WE#.(....
+00004830: ef00 6c7d c1ae 4ff0 029e f81b 5e63 3dd0  ..l}..O.....^c=.
+00004840: f203 82fc 8fca 4d58 a0a4 7a47 487e 87b2  ......MX..zGH~..
+00004850: 3ada 55f5 6798 6fac 3fc5 5c81 ef3a a885  :.U.g.o.?.\..:..
+00004860: fe63 8d76 cfd2 2f77 873a c108 a8c7 0930  .c.v../w.:.....0
+00004870: d86a aae3 9eed f2b8 d30e ba23 af31 e94c  .j.........#.1.L
+00004880: a346 38ef b41b fd49 df6b 747d 3f8c c27e  .F8....I.kt}?..~
+00004890: d8ee 8dc7 1558 da7e 342c ada6 2bda 565f  .....X.~4,..+.V_
+000048a0: 9bc4 0394 b909 7896 6b3b 461a 4f6f 204f  ......x.k;F.Oo O
+000048b0: e303 7f70 f0fe c0df 9941 212a ae21 2bf4  ...p.....A!*.!+.
+000048c0: cff4 5f87 8464 3f9a e2e1 bc20 e447 0a96  .._..d?.... .G..
+000048d0: 7a30 9fb2 2282 c155 30a2 45b6 4ef3 c607  z0.."..U0.E.N...
+000048e0: 8192 74c5 f5a0 cf92 eb99 3c5e c412 7cd4  ..t.......<^..|.
+000048f0: 5299 42e1 ea09 e9ec 9eae 5de7 83bd cd7c  R.B.......]....|
+00004900: b055 9757 9148 4318 559e 4231 c37b 3bf8  .U.W.HC.U.B1.{;.
+00004910: db3a 04db 3a84 db3a b4b7 75e8 6ceb d0dd  .:..:..:..u.l...
+00004920: dc01 bc67 a54c 5328 69ae b5c7 8be5 64a3  ...g.LS(i.....d.
+00004930: 1d77 3f9b 7648 96bb dfc3 4291 25d8 cf1e  .w?.vH....B.%...
+00004940: 8a14 6b2c 455b a0fc ef69 226d 7607 a2bc  ..k,E[...i"mv...
+00004950: 715d 7453 f2d3 20f0 dbbd 4ebb b3a1 a1db  q]tS.. ...N.....
+00004960: ed77 3b5e c772 d36a 0247 a5e8 96d9 9c7a  .w;^.r.j.G.....z
+00004970: e2c6 64d5 f9e3 f236 3648 57f2 36b6 e62b  ..d....66HW.6..+
+00004980: 799b f0e9 799b 9809 b963 ce86 5007 b2a9  y...y....c..P...
+00004990: 40ac ba6d d789 55f6 94d3 646b cad2 6473  @..m..U...dk..ds
+000049a0: 4c02 782d e571 4f1a 0e0d 7402 dd20 8b5a  L.x-.qO...t.. .Z
+000049b0: 422e 1ea8 0cb8 4980 89db 6cc6 ec86 47e1  B.....I...l...G.
+000049c0: 40c3 9a6c d561 e5aa 6f40 ed0d a8ed 2193  @..l.a..o@....!.
+000049d0: fd06 d4de 80da f300 b550 01b5 5570 bf1f  .........P..Up..
+000049e0: a829 e214 1fbc 61b5 d589 c30a 7176 5d67  .)....a.....qv]g
+000049f0: 856a e1c4 e210 92b7 7ffe 5c30 f957 e7c0  .j........\0.W..
+00004a00: fcdf 15cc 898c b112 4e58 ccf0 62f1 ddf8  ........NX..b...
+00004a10: f5e3 3bb3 c5d7 a9ee 5d0b ade0 9ed7 69f9  ..;.....].....i.
+00004a20: 5ed0 b98b 03bd beef b5ba 811f 1874 02a7  ^............t..
+00004a30: f955 8c07 046b a44f 19ef 058e 2246 f0c4  .U...k.O...."F..
+00004a40: 4211 1dc6 53a0 cdfa 44cc 0896 a5f4 03ba  B...S...D.......
+00004a50: b1a0 a4d2 31d1 c787 357e 8d6e 4e99 a5ce  ....1...5~.nN...
+00004a60: 3303 5521 004c 3359 73e7 6f31 dc25 4004  3.U!.L3Ys.o1.%@.
+00004a70: 981a 2b80 a203 ddbe c4c9 92ea 67e8 df8c  ..+.........g...
+00004a80: 9fa7 f1e5 07c0 4766 f012 1301 664a e9fd  ......Gf....fJ..
+00004a90: 8d12 1e02 e0bc 9480 8267 9f33 23c6 c6a3  .........g.3#...
+00004aa0: 5485 01fb 6dbf 8480 7338 4086 9894 e520  T...m...s8@.... 
+00004ab0: 8ca0 0b38 3c27 0b38 e256 e7e8 bb1c 667b  ...8<'.8.V....f{
+00004ac0: 9b73 35bd 87e5 6a76 0094 9b12 6f0d f015  .s5...jv....o...
+00004ad0: fd79 49d7 0bfe cb49 b317 7eab e011 584c  .yI....I..~...XL
+00004ae0: 5df2 1123 7b5a 1e04 1586 0797 4d54 5b99  ]..#{Z......MT[.
+00004af0: b752 47fc ffc0 dc3a bf2a d562 0c99 9111  .RG....:.*.b....
+00004b00: f8b6 3dab 07ff 3617 8066 04ae 5c08 b8c3  ..=...6..f..\...
+00004b10: 6052 6f65 94a1 ec43 4164 7a72 4560 7555  `Roe...CAdzrE`uU
+00004b20: 963b 10d5 6560 8127 ee46 989a 7cfb 8f30  .;..e`.'.F..|..0
+00004b30: f6e6 810e 18df f234 5121 af96 ce36 2cef  .......4Q!...6,.
+00004b40: d5ac 70d0 f7dd b96e 88af 0017 2c58 1016  ..p....n....,X..
+00004b50: 2cfc cf23 edae e794 6f21 6de8 fe1f 5e94  ,..#....o!m...^.
+00004b60: da3d a4d5 b259 5f09 69ba 698c e535 c636  .=...Y_.i.i..5.6
+00004b70: 8ccd 4cc1 c294 653c da00 7dd6 40d4 5303  ..L...e<..}.@.S.
+00004b80: 93cd 753d 0ff4 81fb 5726 38ef 8c7c 6a7b  ..u=....W&8..|j{
+00004b90: 461d 26be c04d 635d c0fd ef1a 76b3 db1c  F.&..Mc]....v...
+00004ba0: 3797 342b 2e79 d683 43e7 d32d b5c7 eb7e  7.4+.y..C..-...~
+00004bb0: 9b4f 61df c0e0 d07d a560 702d a6d5 2267  .Oa....}.`p-.."g
+00004bc0: 66c8 9b5d eddb 8326 e08c da2d 507d 4aab  f..]...&...-P}J.
+00004bd0: ef83 ea6f eb0c ef99 6fae 3ef7 8582 3d5c  ...o....o.>...=\
+00004be0: 977e e333 d55b d20f defc c1cf c8d2 b794  .~.3.[..........
+00004bf0: c7fd 908a 8f94 d8db 0076 5b4d 5291 8fe1  .........v[MR...
+00004c00: 32c1 a518 d9c4 029c 8959 4e0f e776 1375  2........YN..v.u
+00004c10: 52a6 eec7 4386 628d 9a94 d795 1f72 4f77  R...C.b......rOw
+00004c20: b6b8 e78e ee2b 4b11 e43c a5f2 0c4b b828  .....+K..<...K.(
+00004c30: bfd0 54e9 42df 7898 4252 1073 4d02 73b8  ..T.B.x.BR.sM.s.
+00004c40: 110d 9997 454a 85fe 01c0 a13a 2153 3f12  ....EJ.....:!S?.
+00004c50: 3984 a424 fc8a 40ff 57bf 57d0 0de6 7155  9..$..@.W.W...qU
+00004c60: 0a54 ca52 8d62 0acb b1e0 6545 aece bf20  .T.R.b....eE... 
+00004c70: a8d4 5fae e8e3 f2c7 3a47 bf01 0000 ffff  .._.....:G......
+00004c80: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00004c90: 767e a5b1 d307 0000 d926 0000 1400 0000  v~.......&......
+00004ca0: 786c 2f63 6861 7274 732f 6368 6172 7432  xl/charts/chart2
+00004cb0: 2e78 6d6c ec5a 6d6f db36 10fe 3e60 ff41  .xml.Zmo.6..>`.A
+00004cc0: 13b2 4f83 63c9 ef16 6a0f 8912 6fc3 d236  ..O.c...j...o..6
+00004cd0: 68ba 0dd8 300c 3445 db5c 2852 25a9 c4ee  h...0.4E.\(R%...
+00004ce0: b0ff bee3 8b1c cb71 dad4 6db1 2c4b 3e38  .......q..m.,K>8
+00004cf0: e28b 4ec7 e3dd c3bb 477a f6ed 3267 c115  ..N.....Gz..2g..
+00004d00: 918a 0a3e 0ae3 c328 0c08 c722 a37c 3e0a  ...>...(...".|>.
+00004d10: 7f7a 3d69 0cc2 4069 c433 c404 27a3 7045  .z=i..@i.3..'.pE
+00004d20: 54f8 edf8 cb2f 9ee1 042f 90d4 1705 c224  T..../.../.....$
+00004d30: 0021 5c25 7814 2eb4 2e92 6653 e105 c991  .!\%x.....fS....
+00004d40: 3a14 05e1 3036 1332 471a 9a72 decc 24ba  :...06.2G..r..$.
+00004d50: 06e1 396b b6a2 a8d7 b442 422f 00ed 2120  ..9k.....BB/..! 
+00004d60: 4794 57f7 cbfb dc2f 6633 8ac9 89c0 654e  G.W..../f3....eN
+00004d70: b876 5a48 c290 060b a805 2d54 250d c73d  .vZH......-T%..=
+00004d80: d9ba 2531 a758 0a25 66fa 108b bce9 8455  ..%1.X.%f......U
+00004d90: 8b02 6171 b7b9 5ed5 188c 9421 4de2 61d4  ..aq..^....!M.a.
+00004da0: 09ae 101b 8551 d834 9d0c f1b9 eb20 bcf1  .....Q.4..... ..
+00004db0: d385 eb94 a2e4 19c9 5221 396c c7c6 fc1c  ........R!9l....
+00004dc0: 2747 4c13 c941 542a b806 adbd bdf2 7b59  'GL..AT*......{Y
+00004dd0: 3c47 f2b2 2c1a a06e 018b 9c52 46f5 ca2e  <G..,..n...RF...
+00004de0: 3b1c 3f03 d9e9 4280 3d82 57e4 4d49 2551  ;.?...B.=.W.MI%Q
+00004df0: a310 c79d 1b13 743e d400 51bf 3968 b6fc  ......t>..Q.9h..
+00004e00: bec2 62e3 4ea2 f48a 11b7 a038 6a99 d536  ..b.N......8j..6
+00004e10: d7cf b52a 4c10 6353 842f 8d6d 3626 afa7  ...*L.cS./.m6&..
+00004e20: de8c 9b1b b78d 61ee b26e 642e 34d5 8cd8  ......a..nd.4...
+00004e30: 8ba5 f995 142f c6cf 5032 15d9 ea5c 0652  ...../..P2...\.R
+00004e40: 68b3 0981 2af0 844a a5cf 90d2 e748 82df  h...*..J.....H..
+00004e50: c5a1 8902 fd12 7e66 4c5c 8f42 c218 f802  ......~fL\.B....
+00004e60: 056f 30fd 6005 21df 86c1 b544 c528 546f  .o0.`.!....D.(To
+00004e70: 4a24 4918 208e a11b 2ca6 65d5 4835 b463  J$I. ...,.e.H5.c
+00004e80: b346 9430 a52f ccd2 6da3 303d c5b9 34ff  .F.0./..m.0=..4.
+00004e90: 3232 7b05 daa8 b730 b513 813e 53ab 1575  22{....0...>S..u
+00004ea0: ba69 492f 21d2 b8b8 b057 6170 097b 0f33  .iI/!....Wap.{.3
+00004eb0: 215e ace6 76d6 1429 c2a8 89c8 08b6 1125  !^..v..).......%
+00004ec0: 4a30 9a4d 2863 b661 c28f a44c 3aa3 eb65  J0.M(c.a...L:..e
+00004ed0: 6ce7 b032 7f2e 32d7 d7eb 4620 cea9 59e6  l..2..2...F ..Y.
+00004ee0: 2f67 33d7 ddae ba9b 20b2 9202 fbb5 f500  /g3..... .......
+00004ef0: 132d 3cd0 ab82 cc20 fc47 e137 396f 30ed  .-<.... .G.79o0.
+00004f00: c411 b435 4090 1bc0 6a6b 002b eb0b 953d  ...5@...jk.+...=
+00004f10: ec63 bc85 ac99 24d8 c884 ca28 9cc9 c6e4  .c....$....(....
+00004f20: 9593 a2c7 a710 4aa5 0b57 a398 b6f7 c10d  ......J..W......
+00004f30: 700d 466e 569b 0e17 dafa 8080 0d64 6855  p.FnV........dhU
+00004f40: 8b40 e59f c385 b199 3303 37a6 dbe8 28c0  .@......3.7...(.
+00004f50: 414e 905a b81b ad81 bdbe 0ca6 8278 27c4  AN.Z.........x'.
+00004f60: 3ca7 723a 546a f1da 344e 0823 9a78 5bfb  <.r:Tj..4N.#.x[.
+00004f70: a82f 98d0 4792 2087 002b 516a 0b06 5324  ./..G. ..+Qj..S$
+00004f80: 5383 a4a6 1bae 4fa8 df35 2c98 0386 3920  S.....O..5,...9 
+00004f90: 4301 90e9 f4c0 ac54 0006 2473 8357 48ae  C......T..$s.WH.
+00004fa0: 52c1 440d 3140 3502 06c1 09cd 96b5 650b  R.D.1@5.......e.
+00004fb0: 9911 2fde 2be5 4ca4 b47c 4566 e68e d9f8  ../.+.L..|Ef....
+00004fc0: 4203 547f 7570 74d0 376b b49d 309c 22f0  B.T.upt.7k..0.".
+00004fd0: 0633 a1d0 2900 95f6 e1ec 9428 7400 4f72  .3..)......(t.Or
+00004fe0: ae88 93ab f1f7 10cf a532 b75f 5943 1566  .........2._YC.f
+00004ff0: 8f4c 6857 625c c33e 72bd 4dd5 96bc cb93  .LhWb\.>r.M.....
+00005000: 11c6 807e 36bc 6eb9 e49e db07 46e2 26c2  ...~6.n.....F.&.
+00005010: 7f98 bd20 73f0 aa2b 8f54 de3e 18d9 8dd9  ... s..+.T.>....
+00005020: 61a0 e383 5672 3039 68ed 6d25 c4d5 3520  a...Vr09h.m%..5 
+00005030: fd6f f4f7 43c6 f23f 5cf3 7056 32f6 0747  .o..C..?\.pV2..G
+00005040: 39b9 b7f9 bc8a 1015 667f 7899 6f6f e5f1  9.......f.x.oo..
+00005050: c1c0 683a 586b 0a73 d6fb e9ce e654 6464  ..h:Xk.s.....Tdd
+00005060: 1c7d 6d67 d8c3 da76 6c6f 7777 f776 4775  .}mg...vloww.vGu
+00005070: 558d 8f38 7f30 b063 7ce0 ce09 adf7 4d68  U..8.0.c|.....Mh
+00005080: bf6f 4267 f704 f0aa 9b45 ba46 e56d de4e  .oBg.....E.F.m.N
+00005090: 64a9 cf94 dd5b b80a 4a09 e0fb 57da 6e0f  d....[..J...W.n.
+000050a0: a234 ed34 ba27 bdd3 4627 1aa6 8de3 d376  .4.4.'..F'.....v
+000050b0: ab71 da6f 9db4 86fd 76b7 9da6 7f6f a407  .q.o....v....o..
+000050c0: 1f9c 1c74 36ce c55e 5272 faa6 243f 7894  ...t6..^Rr..$?x.
+000050d0: f80b 00d9 fe35 a261 6fd8 e8c4 69da 189c  .....5.ao...i...
+000050e0: 7427 8d38 8a3a a7ad 56e7 b8d3 8afe b608  t'.8.:..V.......
+000050f0: 8413 d0d9 8654 b50a 1350 2ee4 b723 df06  .....T...P...#..
+00005100: 0b4e 3622 dff7 bc23 f287 7bfb f48b 291c  .N6"...#..{...).
+00005110: 8ad6 ad83 eba6 0816 9f17 085c 82b0 7d36  ...........\..}6
+00005120: 3d01 c1dd 4010 4706 0962 1b90 16da 9fa0  =...@.G..b......
+00005130: c006 d3c3 8482 f8e3 a020 3b9b 3265 73ea  ......... ;.2es.
+00005140: 85b8 3e23 73c2 b31f c956 1e04 233f 23a8  ..>#s....V..#?#.
+00005150: 0037 aa13 057d 29d2 2fe0 0cba d57f 41e4  .7...})./.....A.
+00005160: cefe 7322 cdc9 7c6b fe71 399d 3272 41df  ..s"..|k.q9.2rA.
+00005170: 6e8a 02b0 5aab 3647 c52f 34d3 3ec9 6ac5  n...Z.6G./4.>.j.
+00005180: 4377 c4a0 6505 8bdd c170 d0ef c7c3 db03  Cw..e....p......
+00005190: 5055 f5db 4337 0022 37f3 2893 19af 93aa  PU..C7."7.(.....
+000051a0: 7afe e48a 59f9 61e9 9305 9a1a 88fa 9e77  z...Y.a........w
+000051b0: 8068 1cef 8da2 4790 90a0 3909 1416 f2fe  .h....G...9.....
+000051c0: 7980 d7c5 67b6 8c07 50c5 b406 dd7e 370c  y...g...P....~7.
+000051d0: b0a9 5a24 cfde 5b2a b804 abed f3dc 5a2a  ..Z$..[*......Z*
+000051e0: 7647 3a8c 125b b89a a20e 2a9e cdc4 1827  vG:..[....*....'
+000051f0: a6f2 f4a7 d22a 9f0a ef66 1c88 047f 8cdd  .....*...f......
+00005200: 4c78 1c79 561c 5b78 bdd9 f927 7885 c424  Lx.yV.[x...'x..$
+00005210: 17a2 0a70 9f55 3fd8 e4ab f5f8 11d7 c55c  ...p.U?........\
+00005220: ad7e dbb1 431b 003c 6c03 d0f6 3b16 1470  .~..C..<l...;..p
+00005230: 7233 30e8 76e2 4eaf 37e8 fb60 ae81 2ec4  r30.v.N.7..`....
+00005240: f391 adbe ef44 7285 11dc 3137 e793 9014  .....Dr...17....
+00005250: 0e0f 5bd2 3bbd 72ca 9fa3 a597 bb31 31b3  ..[.;.r......11.
+00005260: 6575 ed94 41cb 73e1 d9b2 a93b 3b20 e626  eu..A.s....;; .&
+00005270: b90e 6e0a 9b51 f81d 014e 0d31 a04f 4409  ..n..Q...N.1.OD.
+00005280: 07d5 19e5 9724 f33c 8d81 a93f 857c 4df1  .....$.<...?.|M.
+00005290: e573 c02b 27bc c228 18a4 fcee 410d 37c1  .s.+'..(....A.7.
+000052a0: 21bb d680 8363 bf16 4e8d 9d14 83c1 e461  !....c..N......a
+000052b0: b755 41f2 0c88 1440 e7bc 0065 149f 0389  .UA....@...e....
+000052c0: c4e6 40f5 183e 691f 5227 de4d ea0c ee47  ..@..>i.R'.M...G
+000052d0: eaec 01f0 7ae9 08ad 4d7a add1 f375 cc43  ....z...Mz...u.C
+000052e0: a2d9 861f c6b2 3d72 760d 1241 c37a 1a0e  ......=rv..A.z..
+000052f0: 728b 5f5b 7368 6e67 8158 05b2 5b1d 7916  r._[shng.X..[.y.
+00005300: a9bb 9972 f931 e283 cf50 5fbf 12e9 9ddf  ...r.1...P_.....
+00005310: b46a 10c3 a6ec 087c db73 58e0 df8e 089f  .j.....|.sX.....
+00005320: 32a0 1e15 a9e8 2447 4942 ed2e 9e97 4cd3  2.....$GIB....L.
+00005330: b32b 06d1 b511 ee90 e6ad 8105 52d6 5b08  .+..........R.[.
+00005340: 53d7 efd3 238c 67e4 2c60 7c27 6966 20cf  S...#.g.,`|'if .
+00005350: 65d8 b5ac ebd1 4438 d8fb f65a 77e0 6bf4  e.....D8...Zw.k.
+00005360: f5bf 0fad fbb1 b786 247e c2b0 ffe0 1b82  ........$~......
+00005370: bd31 ac5e 4f5a 7cdb 8d61 76e8 98e8 6b42  .1.^OZ|..av...kB
+00005380: 3c6e 4d5d c3e7 256b 00da 95eb d493 a68f  <nM]..%k........
+00005390: 4522 4fd9 7d9e 5c07 5e44 3834 de3b d5a9  E"O.}.\.^D84.;..
+000053a0: 1d12 b5b4 f001 1e12 5bfa 7dfa 43c2 9f6d  ........[.}.C..m
+000053b0: 1f09 931f bf2b 9ff0 1dd7 134a 1a7e ecff  .....+.....J.~..
+000053c0: 8492 75fc aaa1 64ee 2a33 1fda ef07 4848  ..u...d.*3....HH
+000053d0: 226a af3e 2d11 695f 82da abed f2ed 33bf  "j.>-.i_......3.
+000053e0: aedd edca 0fea 9b80 a762 65f3 5380 7b1f  .........be.S.{.
+000053f0: f4e0 676c ed5b c6e3 7ea6 ea25 679e f0f6  ..gl.[..~..%g...
+00005400: 4768 4655 710c 45cf a53a f285 0b30 d0be  GhFUq.E..:...0..
+00005410: 6007 defb c450 e6e6 2310 a01f b6ea 8eea  `....P..#.......
+00005420: 1dfd 7dde 534f e777 bca3 7e64 f57f 2129  ..}.SO.w..~d..!)
+00005430: d717 44c3 d720 735b 072d 0882 2f0c 2640  ..D.. s[.-../.&@
+00005440: f811 692b bc02 786c a055 e694 2bfb 95cb  ..i+..xl.U..+...
+00005450: a1a1 a3cd 9750 87fd 3080 4f65 ec7f f351  .....P..0.Oe...Q
+00005460: 8e1d 70b7 9b56 3b04 02c7 4871 8db5 2c78  ..p..V;...Hq..,x
+00005470: 5859 18b2 1940 a5fe 7053 1bae bf48 1bff  XY...@..pS...H..
+00005480: 0300 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00005490: 0000 0021 003b 6d32 4bc1 0000 0042 0100  ...!.;m2K....B..
+000054a0: 0023 0000 0078 6c2f 776f 726b 7368 6565  .#...xl/workshee
+000054b0: 7473 2f5f 7265 6c73 2f73 6865 6574 312e  ts/_rels/sheet1.
+000054c0: 786d 6c2e 7265 6c73 848f c18a c230 1445  xml.rels.....0.E
+000054d0: f703 fe43 787b 93d6 850c 4353 3722 b855  ...Cx{....CS7".U
+000054e0: e703 62fa da06 db97 90f7 14fd 7bb3 1c65  ..b.........{..e
+000054f0: c0e5 e570 cfe5 369b fb3c a91b 660e 912c  ...p..6..<..f..,
+00005500: d4ba 0285 e463 1768 b0f0 7bda 2dbf 41b1  .....c.h..{.-.A.
+00005510: 38ea dc14 092d 3c90 61d3 2ebe 9a03 4e4e  8....-<.a.....NN
+00005520: 4a89 c790 5815 0bb1 8551 24fd 18c3 7ec4  J...X....Q$...~.
+00005530: d9b1 8e09 a990 3ee6 d949 8979 30c9 f98b  ......>..I.y0...
+00005540: 1bd0 acaa 6a6d f25f 07b4 2f4e b5ef 2ce4  ....jm._../N..,.
+00005550: 7d57 833a 3d52 59fe ec8e 7d1f 3c6e a3bf  }W.:=RY...}.<n..
+00005560: ce48 f2cf 8449 3990 603e a248 39c8 45ed  .H...I9.`>.H9.E.
+00005570: f280 6241 eb77 f69e 6b7d 0e04 a66d cccb  ..bA.w..k}...m..
+00005580: f3f6 0900 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00005590: 0008 0000 0021 0011 98ab c9db 0000 00d0  .....!..........
+000055a0: 0100 0023 0000 0078 6c2f 776f 726b 7368  ...#...xl/worksh
+000055b0: 6565 7473 2f5f 7265 6c73 2f73 6865 6574  eets/_rels/sheet
+000055c0: 322e 786d 6c2e 7265 6c73 ac91 cd4e c330  2.xml.rels...N.0
+000055d0: 0c80 ef48 bc43 e43b 49db 0342 68e9 2e68  ...H.C.;I..Bh..h
+000055e0: d2ae 301e 2024 6e1b d13a 51ec 017b 7bc2  ..0. $n..:Q..{{.
+000055f0: 6112 9d26 71e1 e61f f9f3 6779 b3fd 5a66  a..&q.....gy..Zf
+00005600: f581 8563 220b ad6e 4021 f914 228d 165e  ...c"..n@!.."..^
+00005610: 0fbb bb07 502c 8e82 9b13 a185 1332 6cfb  ....P,.......2l.
+00005620: db9b cd33 ce4e ea10 4f31 b3aa 1462 0b93  ...3.N..O1...b..
+00005630: 487e 3486 fd84 8b63 9d32 52ed 0ca9 2c4e  H~4....c.2R...,N
+00005640: 6a5a 4693 9d7f 7723 9aae 69ee 4df9 cd80  jZF...w#..i.M...
+00005650: 7ec5 54fb 60a1 ec43 07ea 70ca 75f3 dfec  ~.T.`..C..p.u...
+00005660: 340c d1e3 53f2 c705 49ae ac30 a1b8 cf7a  4...S...I..0...z
+00005670: 5945 ba32 a258 d0fa 5ce3 73d0 eaaa 0ce6  YE.2.X..\.s.....
+00005680: ba4d fb9f 36b9 4412 2c2f 2852 a578 6575  .M..6.D.,/(R.xeu
+00005690: d133 1779 a7df 22fd 489a d51f fa6f 0000  .3.y..".H....o..
+000056a0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+000056b0: 0021 0081 f1a0 3fc4 0000 00ad 0100 0023  .!....?........#
+000056c0: 0000 0078 6c2f 6472 6177 696e 6773 2f5f  ...xl/drawings/_
+000056d0: 7265 6c73 2f64 7261 7769 6e67 312e 786d  rels/drawing1.xm
+000056e0: 6c2e 7265 6c73 bc90 cf0a c230 0c87 ef82  l.rels.....0....
+000056f0: ef50 72b7 dd76 1011 bb5d 44d8 55f4 0142  .Pr..v...]D.U..B
+00005700: 97fd c1ad 2d4d 15f7 f616 4450 10bc 790a  ....-M....DP..y.
+00005710: 49c8 f7fb c8ae ba4f a3b8 51e0 c159 0db9  I......O..Q..Y..
+00005720: cc40 9035 ae19 6ca7 e17c 3aac 3620 38a2  .@.5..l..|:.6 8.
+00005730: 6d70 7496 34cc c450 95cb c5ee 4823 c674  mpt.4..P....H#.t
+00005740: c4fd e059 248a 650d 7d8c 7eab 149b 9e26  ...Y$.e.}.~....&
+00005750: 64e9 3cd9 b469 5d98 30a6 3674 caa3 b960  d.<..i].0.6t...`
+00005760: 47aa c8b2 b50a ef0c 283f 98a2 6e34 84ba  G.......(?..n4..
+00005770: 2940 9c66 9f92 7fb3 5ddb 0e86 f6ce 5c27  )@.f....].....\'
+00005780: b2f1 4b84 323d 8698 8018 3a8a 1aa4 7c4e  ..K.2=....:...|N
+00005790: f859 0a99 6441 7df7 c8ff e791 bf3c d4c7  .Y..dA}......<..
+000057a0: 93cb 0700 0000 ffff 0300 504b 0304 1400  ..........PK....
+000057b0: 0600 0800 0000 2100 9000 0db0 a601 0000  ......!.........
+000057c0: dd02 0000 0f00 0000 786c 2f6d 6574 6164  ........xl/metad
+000057d0: 6174 612e 786d 6c64 514b 4f1b 3110 be57  ata.xmldQKO.1..W
+000057e0: e23f 58be 6fbc 2114 42b4 bb28 02e5 4425  .?X.o.!.B..(..D%
+000057f0: 5428 ead5 b1c7 8955 bf64 7b69 5655 ff7b  T(.....U.d{iVU.{
+00005800: 67bd 8406 38d9 e319 7ff3 3d9a 9b83 35e4  g...8.....=...5.
+00005810: 0562 d2de b574 3eab 2901 27bc d46e d7d2  .b...t>.).'..n..
+00005820: 1f4f 9b6a 4949 cadc 496e bc83 960e 90e8  .O.jII..In......
+00005830: 4d77 f6a5 b190 b9e4 9913 0470 a9a5 fb9c  Mw.........p....
+00005840: c38a b124 f660 799a f900 0e3b ca47 cb33  ...$.`y....;.G.3
+00005850: 9671 c752 88c0 65da 0364 6bd8 795d 5f32  .q.R..e..dk.y]_2
+00005860: cbb5 a313 c2ea 20f9 2714 ab45 f4c9 ab3c  ...... .'..E...<
+00005870: 13de 32af 9416 f009 677e c5e4 e038 cef2  ..2.....g~...8..
+00005880: 18f9 40bb 376e 4f43 8044 84ef 5d46 6d1f  ..@.7nOC.D..]Fm.
+00005890: 1a04 bfa0 a09f f777 eb87 ef94 58ed 1efb  .......w....X...
+000058a0: 107c cc20 9fdf fc40 9635 5a22 7c18 4604  .|. ...@.5Z"|.F.
+000058b0: 1278 cab0 36e6 7ff1 cc4d 0fa8 1f9b 16e2  .x..6....M......
+000058c0: 0e11 f196 82d1 79a3 632a 7b49 f4bf 6fbd  ......y.c*{I..o.
+000058d0: 79dc 6b35 d5c2 008f 9bc9 9a32 5f1e 6ebd  y.k5.......2_.n.
+000058e0: b5e0 f284 c553 d2bb 3191 7139 4431 e10a  .....S..1.q9D1..
+000058f0: 30e6 1b1a 3fbe b3ae 61c7 108a d0ae 517d  0...?...a.....Q}
+00005900: ee23 8c03 2599 f702 4f6c d8fe ea1a 38e4  .#..%...Ol....8.
+00005910: fb94 cb49 faa8 5bfa 672b b7db a590 a252  ...I..[.g+.....R
+00005920: 7c0e d5c5 f525 547c f9f5 aa5a 8885 5ad4  |....%T|...Z..Z.
+00005930: a23e bf16 8bbf 6822 06b5 7a35 7c3d 1afe  .>....h"..z5|=..
+00005940: 1031 ec98 355a adee a620 0a6f 859a 0d0f  .1..5Z... .o....
+00005950: 0964 4beb 4217 7722 e9e3 6636 d260 ef39  .dK.B.w"..f6.`.9
+00005960: 77cd 5162 51f0 8173 1464 32f0 e588 5820  w.QbQ..s.d2...X 
+00005970: 4ebf 9c98 d2fd 0300 00ff ff03 0050 4b03  N............PK.
+00005980: 0414 0006 0008 0000 0021 0035 85fa 75af  .........!.5..u.
+00005990: 0100 003c 1000 0027 0000 0078 6c2f 7072  ...<...'...xl/pr
+000059a0: 696e 7465 7253 6574 7469 6e67 732f 7072  interSettings/pr
+000059b0: 696e 7465 7253 6574 7469 6e67 7331 2e62  interSettings1.b
+000059c0: 696e ec57 bd4a 0341 10fe ee12 21f1 02b1  in.W.J.A....!...
+000059d0: 4861 6111 2b1b 0b85 8096 9a68 a1a8 0731  Haa.+......h...1
+000059e0: 42ca 8811 1424 8a49 2f3e 839d e003 f80a  B....$.I/>......
+000059f0: be85 a520 d808 fa00 b612 e7cb 65c9 bab7  ... ........e...
+00005a00: 7729 5444 d959 26fb 33b3 33b3 5fbe 62ae  w)TD.Y&.3.3._.b.
+00005a10: 867d 7470 2a5a 4603 bb58 4205 0b32 cae8  .}tp*ZF..XB..2..
+00005a20: e210 e738 96df 2e92 c5cb 0685 47b4 8a99  ...8........G...
+00005a30: a7cb 8c87 3cae 834a ae0d 0f25 efbd efcb  ....<..J...%....
+00005a40: 0c51 0fab 12f5 fb85 d1fd 4106 6689 4bab  .Q........A.f.K.
+00005a50: 0854 37d7 b683 4264 9b09 8007 5952 95f0  .T7...Bd....YR..
+00005a60: 5eae 0e64 7bc0 bc6c 1aa2 ad10 783e 8bef  ^..d{..l....x>..
+00005a70: 4d3f fabe 59fc d5b9 8a67 fa35 fda6 3f8d  M?..Y....g.5..?.
+00005a80: 2aea 08b1 870d 6cc9 08b1 f303 088d 0fb9  *.....l.........
+00005a90: 8e03 1c0d 38d0 93ff fa44 46c4 850e ee84  ....8....DF.....
+00005aa0: 038b bf52 d357 934e cdfd c9b2 5dd1 0e01  ...R.W.N....]...
+00005ab0: 8780 43c0 21e0 1088 21c0 3e27 3354 1aa3  ..C.!...!.>'3T..
+00005ac0: deca 0694 3ff0 7310 3a04 4608 e4a5 331f  ....?.s.:.F...3.
+00005ad0: f187 5c32 252b 07ec 85c9 b192 2c38 536c  ..\2%+......,8Sl
+00005ae0: 7d35 cf69 57bd b7e9 d796 03e6 53fd 32ed  }5.iW.......S.2.
+00005af0: e65e d510 7d21 24e7 1996 812b b590 7965  .^..}!$....+..ye
+00005b00: 32f2 e7dd 59ed 5c5f d2d6 ef7f 36ca b598  2...Y.\_....6...
+00005b10: d8de 97f4 66fd 9d66 6c13 5315 2329 968e  ....f..fl.S.#)..
+00005b20: 0d7d 2e0c d573 71fd 2280 1bcf b1be 3cad  .}...sq.".....<.
+00005b30: f604 a852 31b1 61c6 5ac6 c984 e6a0 b0d1  ...R1.a.Z.......
+00005b40: f962 de7f 1dc6 b4e1 9684 2d39 ab44 f128  .b........-9.D.(
+00005b50: adae 34ae d970 637c 7279 5c4c daf5 5a94  ..4..pc|ry\L..Z.
+00005b60: 7fed 1f7f 5bdf 2fdf dc7e 0000 00ff ff03  ....[./..~......
+00005b70: 0050 4b03 0414 0006 0008 0000 0021 0035  .PK..........!.5
+00005b80: 85fa 75af 0100 003c 1000 0027 0000 0078  ..u....<...'...x
+00005b90: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+00005ba0: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+00005bb0: 7332 2e62 696e ec57 bd4a 0341 10fe ee12  s2.bin.W.J.A....
+00005bc0: 21f1 02b1 4861 6111 2b1b 0b85 8096 9a68  !...Haa.+......h
+00005bd0: a1a8 0731 42ca 8811 1424 8a49 2f3e 839d  ...1B....$.I/>..
+00005be0: e003 f80a be85 a520 d808 fa00 b612 e7cb  ....... ........
+00005bf0: 65c9 bab7 7729 5444 d959 26fb 33b3 33b3  e...w)TD.Y&.3.3.
+00005c00: 5fbe 62ae 867d 7470 2a5a 4603 bb58 4205  _.b..}tp*ZF..XB.
+00005c10: 0b32 cae8 e210 e738 96df 2e92 c5cb 0685  .2.....8........
+00005c20: 47b4 8a99 a7cb 8c87 3cae 834a ae0d 0f25  G.......<..J...%
+00005c30: efbd efcb 0c51 0fab 12f5 fb85 d1fd 4106  .....Q........A.
+00005c40: 6689 4bab 0854 37d7 b683 4264 9b09 8007  f.K..T7...Bd....
+00005c50: 5952 95f0 5eae 0e64 7bc0 bc6c 1aa2 ad10  YR..^..d{..l....
+00005c60: 783e 8bef 4d3f fabe 59fc d5b9 8a67 fa35  x>..M?..Y....g.5
+00005c70: fda6 3f8d 2aea 08b1 870d 6cc9 08b1 f303  ..?.*.....l.....
+00005c80: 088d 0fb9 8e03 1c0d 38d0 93ff fa44 46c4  ........8....DF.
+00005c90: 850e ee84 038b bf52 d357 934e cdfd c9b2  .......R.W.N....
+00005ca0: 5dd1 0e01 8780 43c0 21e0 1088 21c0 3e27  ].....C.!...!.>'
+00005cb0: 3354 1aa3 deca 0694 3ff0 7310 3a04 4608  3T......?.s.:.F.
+00005cc0: e4a5 331f f187 5c32 252b 07ec 85c9 b192  ..3...\2%+......
+00005cd0: 2c38 536c 7d35 cf69 57bd b7e9 d796 03e6  ,8Sl}5.iW.......
+00005ce0: 53fd 32ed e65e d510 7d21 24e7 1996 812b  S.2..^..}!$....+
+00005cf0: b590 7965 32f2 e7dd 59ed 5c5f d2d6 ef7f  ..ye2...Y.\_....
+00005d00: 36ca b598 d8de 97f4 66fd 9d66 6c13 5315  6.......f..fl.S.
+00005d10: 2329 968e 0d7d 2e0c d573 71fd 2280 1bcf  #)...}...sq."...
+00005d20: b1be 3cad f604 a852 31b1 61c6 5ac6 c984  ..<....R1.a.Z...
+00005d30: e6a0 b0d1 f962 de7f 1dc6 b4e1 9684 2d39  .....b........-9
+00005d40: ab44 f128 adae 34ae d970 637c 7279 5c4c  .D.(..4..pc|ry\L
+00005d50: daf5 5a94 7fed 1f7f 5bdf 2fdf dc7e 0000  ..Z.....[./..~..
+00005d60: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00005d70: 0021 00ec ff94 f080 0200 0062 0c00 0010  .!.........b....
+00005d80: 0000 0078 6c2f 6361 6c63 4368 6169 6e2e  ...xl/calcChain.
+00005d90: 786d 6c7c 57db 8adb 3010 7d2f f41f 8cde  xml|W...0.}/....
+00005da0: bb8e b2ed f642 92a5 bada b0ec 53fb 0126  .....B......S..&
+00005db0: 7137 01db 09b1 29ed df57 8d23 09cd 68fc  q7....)..W.#..h.
+00005dc0: 62c8 8c74 742e 2341 36cf 7ffa aef8 dd5e  b..tt.#A6......^
+00005dd0: c7d3 79d8 32fe b062 453b eccf 87d3 f0b6  ..y.2..bE;......
+00005de0: 653f 7f98 0f5f 5831 4ecd 7068 baf3 d06e  e?..._X1N.ph...n
+00005df0: d9df 7664 cfbb f7ef 36fb a6db cb63 731a  ..vd....6....cs.
+00005e00: 0a87 308c 5b76 9ca6 cbb7 b21c f7c7 b66f  ..0.[v.........o
+00005e10: c687 f3a5 1d5c e7d7 f9da 3793 fb79 7d2b  .....\....7..y}+
+00005e20: c7cb b56d 0ee3 b16d a7be 2bd7 abd5 53d9  ...m...m..+...S.
+00005e30: 3b00 b6db ec8b eb96 bd3e b2e2 e438 b0a2  ;........>...8..
+00005e40: fbff 2def 65c1 1d05 5777 dd5b bd68 88ae  ..-.e...Ww.[.h..
+00005e50: e310 77bd ac6f 9bdc f756 4e37 8166 3ce9  ..w..o...VN7.f<.
+00005e60: b33f 099c 11ea c919 827f f4eb 41fd e95e  .?..........A..^
+00005e70: f7c8 df53 36f1 c04f 70a1 53ef b47a da7e  ...S6..Op.S..z.~
+00005e80: 613d 971f 8329 5500 4cbc aa7d d96f b4a8  a=...)U.L..}.o..
+00005e90: 3053 cefb 62d3 a607 3110 c42c 8180 a607  0S..b...1..,....
+00005ea0: d110 442f 8180 a607 5110 442d 8180 a607  ..D/....Q.D-....
+00005eb0: 9110 442e 8180 6688 0e82 8825 10d0 f420  ..D...f....%... 
+00005ec0: af10 e4c5 c7ef 5754 f711 730b 93a0 2b3e  ......WT..s...+>
+00005ed0: 4f0e 1c94 2ab0 4826 3896 9341 adbe dea7  O...*.H&8..A....
+00005ee0: 2d1e e7ee 7f66 fe2a 3e4f f43a 0e20 9fef  -....f.*>O.:. ..
+00005ef0: 0422 c0a1 a68a cff7 1aaf 4462 c3c2 943c  ."........Db...<
+00005f00: b1df 1308 e4e7 7702 df1d 6f55 b84d 7067  ......w...oU.Mpg
+00005f10: 9d77 2d96 13d7 ea90 4900 cc13 aff3 c46b  .w-.....I......k
+00005f20: 6466 1d2c 8a17 1eda 5873 6857 cd7d 5871  df.,....XshW.}Xq
+00005f30: 1752 0613 aebd 49f1 0d82 b802 8288 bcb1  .R....I.........
+00005f40: 02e9 10c4 5008 3414 8218 0a01 f98a 2072  ....P.4....... r
+00005f50: 7ec8 03ed bce5 226f b97f a9e3 fc0a e202  ~....."o........
+00005f60: 4924 4a12 a224 1225 0951 128a 9284 2899  I$J..$.%.Q....(.
+00005f70: 1715 cbc9 1c4a 3487 9214 0533 9630 6399  .....J4....3.0c.
+00005f80: cf58 213b 1461 8742 7628 c20e 9557 19cb  .X!;.a.Bv(...W..
+00005f90: 894a 05cd 5384 790a d9a1 083b 14ba 4a0a  .J..S.y....;..J.
+00005fa0: daa1 f276 6848 4613 6434 22a3 0932 1a91  ...vhHF.d4"..2..
+00005fb0: d190 8c26 c8a0 6c34 918d 46d9 6822 1b9d  ...&..l4..F.h"..
+00005fc0: cf26 9693 6c0c b4c3 1076 1864 8721 ec30  .&..l....v.d.!.0
+00005fd0: c80e 03ed 3079 3b4c 9e7a 2ca7 d491 7986  ....0y;L.z,...y.
+00005fe0: 30cf 20f3 0c61 9e45 2a2d a1d2 2295 16aa  0. ..a.E*-.."...
+00005ff0: b479 9536 af32 9613 9516 a9b4 844a 8b54  .y.6.2.......J.T
+00006000: 5a4a 250c dde2 d0cb f0ef 60f7 0f00 00ff  ZJ%.......`.....
+00006010: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00006020: 009c e9d5 ff4d 0100 0069 0200 0011 0008  .....M...i......
+00006030: 0164 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
+00006040: 6d6c 20a2 0401 28a0 0001 0000 0000 0000  ml ...(.........
 00006050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000060a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000060b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000060c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000060d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000060e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000060f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006130: 0000 0000 0000 0000 0000 0000 007c 9251  .............|.Q
-00006140: 4f83 3014 85df 4dfc 0fa4 efd0 c2d8 740d  O.0...M.......t.
-00006150: b044 cd7c 7189 8918 8d6f 4d7b b711 a125  .D.|q....oM{...%
-00006160: 6d95 f1ef 2db0 213a e363 7bce fd7a ce4d  m...-.!:.c{..z.M
-00006170: 93d5 a12a bd4f d0a6 5032 4561 4090 0792  ...*.O..P2Ea@...
-00006180: 2b51 c85d 8a9e f3b5 7f8d 3c63 9914 ac54  +Q.]......<c...T
-00006190: 1252 d482 41ab ecf2 22e1 35e5 4ac3 a356  .R..A...".5.J..V
-000061a0: 3568 5b80 f11c 491a caeb 14ed adad 29c6  5h[...I.......).
-000061b0: 86ef a162 2670 0ee9 c4ad d215 b3ee a877  ...b&p.........w
-000061c0: b866 fc9d ed00 4784 2c70 0596 0966 19ee  .f....G.,p...f..
-000061d0: 807e 3d12 d111 29f8 88ac 3f74 d903 04c7  .~=...)...?t....
-000061e0: 5042 05d2 1a1c 0621 fef6 5ad0 95f9 73a0  PB.....!..Z...s.
-000061f0: 5726 ceaa b06d ed3a 1de3 4ed9 820f e2e8  W&...m.:..N.....
-00006200: 3e98 6234 364d 1334 b33e 86cb 1fe2 d7cd  >.b46M.4.>......
-00006210: c353 5fd5 2f64 b72b 0e28 4b04 a75c 03b3  .S_./d.+.(K..\..
-00006220: 4a67 f745 59ba fd6c 546b 20c1 13a1 5b62  Jg.EY..lTk ...[b
-00006230: c98c ddb8 7d6f 0b10 37ed 2fef b9ee b87d  ....}o..7./....}
-00006240: 8d01 0ec2 73c1 e850 e3a4 bccc 6eef f235  ....s..P....n..5
-00006250: ca22 12cd 7cb2 f4c9 551e 2e69 3ca7 71fc  ."..|...U..i<.q.
-00006260: d63d ff63 be0b 3a5c 54c7 10ff 1363 9fcc  .=.c..:\T....c..
-00006270: 7db2 c823 42c9 159d 4713 e209 9025 f8ec  }..#B...G....%..
-00006280: 7364 5f00 0000 ffff 0300 504b 0304 1400  sd_.......PK....
-00006290: 0600 0800 0000 2100 5c3f d894 2602 0000  ......!.\?..&...
-000062a0: a905 0000 1000 0801 646f 6350 726f 7073  ........docProps
-000062b0: 2f61 7070 2e78 6d6c 20a2 0401 28a0 0001  /app.xml ...(...
-000062c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006140: 0000 0000 0000 0000 0000 7c92 514f c320  ..........|.QO. 
+00006150: 1485 df4d fc0f 0def 2d65 eb74 236d 97a8  ...M....-e.t#m..
+00006160: 992f 2e31 b146 e31b 81bb adb1 4003 68d7  ./.1.F......@.h.
+00006170: 7f2f edb6 5a9d f111 ceb9 1fe7 dc90 2ef7  ./..Z...........
+00006180: b20a 3ec1 d852 ab0c 9128 4601 28ae 45a9  ..>..R...(F.(.E.
+00006190: b619 7a2e 56e1 1c05 d631 2558 a515 64a8  ..z.V....1%X..d.
+000061a0: 058b 96f9 e545 ca6b cab5 8147 a36b 30ae  .....E.k...G.k0.
+000061b0: 041b 7892 b294 d719 da39 5753 8c2d df81  ..x......9WS.-..
+000061c0: 6436 f20e e5c5 8d36 9239 7f34 5b5c 33fe  d6.....6.9.4[\3.
+000061d0: ceb6 8027 717c 8525 3826 9863 b803 86f5  ...'q|.%8&.c....
+000061e0: 4044 47a4 e003 b2fe 3055 0f10 1c43 0512  @DG.....0U...C..
+000061f0: 94b3 9844 047f 7b1d 1869 ff1c e895 9153  ...D..{..i.....S
+00006200: 96ae ad7d a763 dc31 5bf0 8338 b8f7 b61c  ...}.c.1[..8....
+00006210: 8c4d d344 cdb4 8fe1 f313 fcba 7e78 eaab  .M.D........~x..
+00006220: 86a5 ea76 c501 e5a9 e094 1b60 4e9b fcbe  ...v.......`N...
+00006230: ac2a bf9f b56e 2da4 7824 744b ac98 756b  .*...n-.x$tK..uk
+00006240: bfef 4d09 e2a6 fde5 3dd7 3db7 af71 8083  ..M.....=.=..q..
+00006250: 087c 307a a871 525e a6b7 77c5 0ae5 9378  .|0z.qR^..w....x
+00006260: 320d e345 185f 1764 4193 194d 92b7 eef9  2..E._.dA..M....
+00006270: 1ff3 5dd0 c385 3c86 f89f 9884 f12c 24a4  ..]...<......,$.
+00006280: 20d7 349e d384 8c88 2740 9ee2 b3cf 917f   .4.....'@......
+00006290: 0100 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+000062a0: 0000 0021 005c 3fd8 9426 0200 00a9 0500  ...!.\?..&......
+000062b0: 0010 0008 0164 6f63 5072 6f70 732f 6170  .....docProps/ap
+000062c0: 702e 786d 6c20 a204 0128 a000 0100 0000  p.xml ...(......
 000062d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000062e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000062f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1590,138 +1590,139 @@
 00006350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000063a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000063b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000063c0: 9c54 d16e 9b30 147d 9fb4 7f40 bc37 90b6  .T.n.0.}...@.7..
-000063d0: aaaa c8a1 a240 4754 0259 8054 da4b e4c1  .....@GT.Y.T.K..
-000063e0: 25b1 0a18 d96e 94ec eb67 8292 90d5 4cda  %....n...g....L.
-000063f0: deae efb9 3ef7 f8d8 bee8 695f 95da 0e18  ....>.....i_....
-00006400: 27b4 9eea e391 a96b 5067 3427 f566 aaa7  '......kPg4'.f..
-00006410: c9cb cda3 ae71 81eb 1c97 b486 a97e 00ae  .....q.......~..
-00006420: 3f59 5fbf a005 a30d 3041 806b 92a2 e653  ?Y_.....0A.k...S
-00006430: 7d2b 4433 310c 9e6d a1c2 7c24 e15a 2205  }+D31..m..|$.Z".
-00006440: 6515 1672 c936 062d 0a92 814b b38f 0a6a  e..r.6.-...K...j
-00006450: 61dc 9ae6 8301 7b01 750e f94d 7326 d43b  a.....{.u..Ms&.;
-00006460: c6c9 4efc 2f69 4eb3 561f 5f25 8746 0ab6  ..N./iN.V._%.F..
-00006470: 90dd 3425 c9b0 90a7 b4e6 2463 94d3 4268  ..4%......$c..Bh
-00006480: de3e 8312 197d 1049 7531 641f 8c88 8365  .>...}.Iu1d....e
-00006490: 22a3 bf44 7186 4b70 24b1 55e0 9203 322e  "..Dq.Kp$.U...2.
-000064a0: 09e4 036e 4d5b 60c2 b885 7662 b283 4c50  ...nM[`...vb..LP
-000064b0: a671 f24b da76 af6b 3f31 8756 ce54 df61  .q.K.v.k?1.V.T.a
-000064c0: 4670 2da4 acb6 ac5b 1ce3 b2e1 8259 6f94  Fp-....[.....Yo.
-000064d0: bdf3 2d80 e0c8 9005 5df2 18f6 6bfb 31b9  ..-.....]...k.1.
-000064e0: b7ee 8e05 32f8 6b61 c715 e20a 726d 89eb  ....2.ka....rm..
-000064f0: 0dfc 4b8b f1a3 ba47 2bb2 3bac 6c7e 6d43  ..K....G+.;.l~mC
-00006500: 4244 093c 2a16 9809 852b b7e3 be2d 4771  BD.<*....+...-Gq
-00006510: 9d29 9d4e 6fdf 488f 2f16 9ca3 58c8 17a5  .).No.H./...X...
-00006520: 4464 235c a9a1 e720 725e d7f1 ec87 a7dc  Dd#\... r^......
-00006530: e9f8 69f8 ba76 a240 8d46 71a2 04dc 7469  ..i..v.@.Fq...ti
-00006540: 27b3 2854 825e e8ae 5d3b 5137 f456 76b0  '.(T.^..];Q7.Vv.
-00006550: b6d3 2452 6f6d 513f 9ddb 6ae6 17db 4906  ..$RomQ?..j...I.
-00006560: c5fa 7610 a4b1 92d6 f76c d75b 0ebb 1004  ..v......l.[....
-00006570: f341 daf9 2c8e 67e1 3725 6ff8 bc6e 25a9  .A..,.g.7%o..n%.
-00006580: 9b4a 50f2 0e62 df53 2f6e 2d1c 2c58 466f  .JP..b.S/n-.,XFo
-00006590: 6aec b473 5072 9cd8 cbe4 d315 5c3d d83f  j..sPr......\=.?
-000065a0: 9e68 40ea 779e 3609 75b1 80d3 37bf 4ea2  .h@.w.6.u...7.N.
-000065b0: 788b 19e4 7232 9cc7 c039 817c f9c3 59d9  x...r2...9.|..Y.
-000065c0: 9238 dbf6 83e5 a79a cf40 3b94 56dd e4b5  .8.......@;.V...
-000065d0: c60f 23f3 ce94 f3a6 9743 c665 c65a bf01  ..#......C.e.Z..
-000065e0: 0000 ffff 0300 504b 0102 2d00 1400 0600  ......PK..-.....
-000065f0: 0800 0000 2100 f31e 96b1 bb01 0000 8708  ....!...........
-00006600: 0000 1300 0000 0000 0000 0000 0000 0000  ................
-00006610: 0000 0000 5b43 6f6e 7465 6e74 5f54 7970  ....[Content_Typ
-00006620: 6573 5d2e 786d 6c50 4b01 022d 0014 0006  es].xmlPK..-....
-00006630: 0008 0000 0021 00b5 5530 23f4 0000 004c  .....!..U0#....L
-00006640: 0200 000b 0000 0000 0000 0000 0000 0000  ................
-00006650: 00f4 0300 005f 7265 6c73 2f2e 7265 6c73  ....._rels/.rels
-00006660: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00006670: f0be 93b7 a904 0000 9c0d 0000 0f00 0000  ................
-00006680: 0000 0000 0000 0000 0000 1907 0000 786c  ..............xl
-00006690: 2f77 6f72 6b62 6f6f 6b2e 786d 6c50 4b01  /workbook.xmlPK.
-000066a0: 022d 0014 0006 0008 0000 0021 00a1 890e  .-.........!....
-000066b0: 7a25 0100 00e1 0400 001a 0000 0000 0000  z%..............
-000066c0: 0000 0000 0000 00ef 0b00 0078 6c2f 5f72  ...........xl/_r
-000066d0: 656c 732f 776f 726b 626f 6f6b 2e78 6d6c  els/workbook.xml
-000066e0: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
-000066f0: 0000 0021 0008 8108 7e62 1200 0062 aa00  ...!....~b...b..
-00006700: 0018 0000 0000 0000 0000 0000 0000 0054  ...............T
-00006710: 0e00 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00006720: 2f73 6865 6574 312e 786d 6c50 4b01 022d  /sheet1.xmlPK..-
-00006730: 0014 0006 0008 0000 0021 00d9 6ac7 56cc  .........!..j.V.
-00006740: 0a00 002e 4c00 0018 0000 0000 0000 0000  ....L...........
-00006750: 0000 0000 00ec 2000 0078 6c2f 776f 726b  ...... ..xl/work
-00006760: 7368 6565 7473 2f73 6865 6574 322e 786d  sheets/sheet2.xm
-00006770: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00006780: 00b5 902c ddb7 0400 0069 0f00 0018 0000  ...,.....i......
-00006790: 0000 0000 0000 0000 0000 00ee 2b00 0078  ............+..x
-000067a0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-000067b0: 6574 332e 786d 6c50 4b01 022d 0014 0006  et3.xmlPK..-....
-000067c0: 0008 0000 0021 00b1 450d ec5c 0700 0002  .....!..E..\....
-000067d0: 2100 0013 0000 0000 0000 0000 0000 0000  !...............
-000067e0: 00db 3000 0078 6c2f 7468 656d 652f 7468  ..0..xl/theme/th
-000067f0: 656d 6531 2e78 6d6c 504b 0102 2d00 1400  eme1.xmlPK..-...
-00006800: 0600 0800 0000 2100 d2e5 2255 4305 0000  ......!..."UC...
-00006810: 481a 0000 0d00 0000 0000 0000 0000 0000  H...............
-00006820: 0000 6838 0000 786c 2f73 7479 6c65 732e  ..h8..xl/styles.
-00006830: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-00006840: 0021 0011 52c1 0387 0200 002e 0800 0014  .!..R...........
-00006850: 0000 0000 0000 0000 0000 0000 00d6 3d00  ..............=.
-00006860: 0078 6c2f 7368 6172 6564 5374 7269 6e67  .xl/sharedString
-00006870: 732e 786d 6c50 4b01 022d 0014 0006 0008  s.xmlPK..-......
-00006880: 0000 0021 0072 a0d0 dc58 0200 00c1 0800  ...!.r...X......
-00006890: 0018 0000 0000 0000 0000 0000 0000 008f  ................
-000068a0: 4000 0078 6c2f 6472 6177 696e 6773 2f64  @..xl/drawings/d
-000068b0: 7261 7769 6e67 312e 786d 6c50 4b01 022d  rawing1.xmlPK..-
-000068c0: 0014 0006 0008 0000 0021 0031 b025 e426  .........!.1.%.&
-000068d0: 0900 00f4 3300 0014 0000 0000 0000 0000  ....3...........
-000068e0: 0000 0000 001d 4300 0078 6c2f 6368 6172  ......C..xl/char
-000068f0: 7473 2f63 6861 7274 312e 786d 6c50 4b01  ts/chart1.xmlPK.
-00006900: 022d 0014 0006 0008 0000 0021 0076 7ea5  .-.........!.v~.
-00006910: b1d3 0700 00d9 2600 0014 0000 0000 0000  ......&.........
-00006920: 0000 0000 0000 0075 4c00 0078 6c2f 6368  .......uL..xl/ch
-00006930: 6172 7473 2f63 6861 7274 322e 786d 6c50  arts/chart2.xmlP
-00006940: 4b01 022d 0014 0006 0008 0000 0021 003b  K..-.........!.;
-00006950: 6d32 4bc1 0000 0042 0100 0023 0000 0000  m2K....B...#....
-00006960: 0000 0000 0000 0000 007a 5400 0078 6c2f  .........zT..xl/
-00006970: 776f 726b 7368 6565 7473 2f5f 7265 6c73  worksheets/_rels
-00006980: 2f73 6865 6574 312e 786d 6c2e 7265 6c73  /sheet1.xml.rels
-00006990: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-000069a0: 1198 abc9 db00 0000 d001 0000 2300 0000  ............#...
-000069b0: 0000 0000 0000 0000 0000 7c55 0000 786c  ..........|U..xl
-000069c0: 2f77 6f72 6b73 6865 6574 732f 5f72 656c  /worksheets/_rel
-000069d0: 732f 7368 6565 7432 2e78 6d6c 2e72 656c  s/sheet2.xml.rel
-000069e0: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
-000069f0: 0081 f1a0 3fc4 0000 00ad 0100 0023 0000  ....?........#..
-00006a00: 0000 0000 0000 0000 0000 0098 5600 0078  ............V..x
-00006a10: 6c2f 6472 6177 696e 6773 2f5f 7265 6c73  l/drawings/_rels
-00006a20: 2f64 7261 7769 6e67 312e 786d 6c2e 7265  /drawing1.xml.re
-00006a30: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
-00006a40: 2100 9000 0db0 a601 0000 dd02 0000 0f00  !...............
-00006a50: 0000 0000 0000 0000 0000 0000 9d57 0000  .............W..
-00006a60: 786c 2f6d 6574 6164 6174 612e 786d 6c50  xl/metadata.xmlP
-00006a70: 4b01 022d 0014 0006 0008 0000 0021 0035  K..-.........!.5
-00006a80: 85fa 75af 0100 003c 1000 0027 0000 0000  ..u....<...'....
-00006a90: 0000 0000 0000 0000 0070 5900 0078 6c2f  .........pY..xl/
-00006aa0: 7072 696e 7465 7253 6574 7469 6e67 732f  printerSettings/
-00006ab0: 7072 696e 7465 7253 6574 7469 6e67 7331  printerSettings1
-00006ac0: 2e62 696e 504b 0102 2d00 1400 0600 0800  .binPK..-.......
-00006ad0: 0000 2100 3585 fa75 af01 0000 3c10 0000  ..!.5..u....<...
-00006ae0: 2700 0000 0000 0000 0000 0000 0000 645b  '.............d[
-00006af0: 0000 786c 2f70 7269 6e74 6572 5365 7474  ..xl/printerSett
-00006b00: 696e 6773 2f70 7269 6e74 6572 5365 7474  ings/printerSett
-00006b10: 696e 6773 322e 6269 6e50 4b01 022d 0014  ings2.binPK..-..
-00006b20: 0006 0008 0000 0021 00ec ff94 f080 0200  .......!........
-00006b30: 0062 0c00 0010 0000 0000 0000 0000 0000  .b..............
-00006b40: 0000 0058 5d00 0078 6c2f 6361 6c63 4368  ...X]..xl/calcCh
-00006b50: 6169 6e2e 786d 6c50 4b01 022d 0014 0006  ain.xmlPK..-....
-00006b60: 0008 0000 0021 0077 07ca 824d 0100 0069  .....!.w...M...i
-00006b70: 0200 0011 0000 0000 0000 0000 0000 0000  ................
-00006b80: 0006 6000 0064 6f63 5072 6f70 732f 636f  ..`..docProps/co
-00006b90: 7265 2e78 6d6c 504b 0102 2d00 1400 0600  re.xmlPK..-.....
-00006ba0: 0800 0000 2100 5c3f d894 2602 0000 a905  ....!.\?..&.....
-00006bb0: 0000 1000 0000 0000 0000 0000 0000 0000  ................
-00006bc0: 8a62 0000 646f 6350 726f 7073 2f61 7070  .b..docProps/app
-00006bd0: 2e78 6d6c 504b 0506 0000 0000 1600 1600  .xmlPK..........
-00006be0: ee05 0000 e665 0000 0000                 .....e....
+000063c0: 0000 0000 0000 0000 0000 0000 009c 54d1  ..............T.
+000063d0: 6e9b 3014 7d9f b47f 40bc 3790 b6aa aac8  n.0.}...@.7.....
+000063e0: a1a2 4047 5402 5980 54da 4be4 c125 b10a  ..@GT.Y.T.K..%..
+000063f0: 18d9 6e94 eceb 6782 9290 d54c dade aeef  ..n...g....L....
+00006400: b93e f7f8 d8be e869 5f95 da0e 1827 b49e  .>.....i_....'..
+00006410: eae3 91a9 6b50 6734 27f5 66aa a7c9 cbcd  ....kPg4'.f.....
+00006420: a3ae 7181 eb1c 97b4 86a9 7e00 ae3f 595f  ..q.......~..?Y_
+00006430: bfa0 05a3 0d30 4180 6b92 a2e6 537d 2b44  .....0A.k...S}+D
+00006440: 3331 0c9e 6da1 c27c 24e1 5a22 0565 1516  31..m..|$.Z".e..
+00006450: 72c9 3606 2d0a 9281 4bb3 8f0a 6a61 dc9a  r.6.-...K...ja..
+00006460: e683 017b 0175 0ef9 4d73 26d4 3bc6 c94e  ...{.u..Ms&.;..N
+00006470: fc2f 694e b356 1f5f 2587 460a b690 dd34  ./iN.V._%.F....4
+00006480: 25c9 b090 a7b4 e624 6394 d342 68de 3e83  %......$c..Bh.>.
+00006490: 1219 7d10 4975 3164 1f8c 8883 6522 a3bf  ..}.Iu1d....e"..
+000064a0: 4471 864b 7024 b155 e092 0332 2e09 e403  Dq.Kp$.U...2....
+000064b0: 6e4d 5b60 c2b8 8576 62b2 834c 50a6 71f2  nM[`...vb..LP.q.
+000064c0: 4bda 76af 6b3f 3187 56ce 54df 6146 702d  K.v.k?1.V.T.aFp-
+000064d0: a4ac b6ac 5b1c e3b2 e182 596f 94bd f32d  ....[.....Yo...-
+000064e0: 80e0 c890 055d f218 f66b fb31 b9b7 ee8e  .....]...k.1....
+000064f0: 0532 f86b 61c7 15e2 0a72 6d89 eb0d fc4b  .2.ka....rm....K
+00006500: 8bf1 a3ba 472b b23b ac6c 7e6d 4342 4409  ....G+.;.l~mCBD.
+00006510: 3c2a 1698 0985 2bb7 e3be 2d47 719d 299d  <*....+...-Gq.).
+00006520: 4e6f df48 8f2f 169c a358 c817 a544 6423  No.H./...X...Dd#
+00006530: 5ca9 a1e7 2072 5ed7 f1ec 87a7 dce9 f869  \... r^........i
+00006540: f8ba 76a2 408d 4671 a204 dc74 6927 b328  ..v.@.Fq...ti'.(
+00006550: 5482 5ee8 ae5d 3b51 37f4 5676 b0b6 d324  T.^..];Q7.Vv...$
+00006560: 526f 6d51 3f9d db6a e617 db49 06c5 fa76  RomQ?..j...I...v
+00006570: 10a4 b192 d6f7 6cd7 5b0e bb10 04f3 41da  ......l.[.....A.
+00006580: f92c 8e67 e137 256f f8bc 6e25 a99b 4a50  .,.g.7%o..n%..JP
+00006590: f20e 62df 532f 6e2d 1c2c 5846 6f6a ecb4  ..b.S/n-.,XFoj..
+000065a0: 7350 729c d8cb e4d3 155c 3dd8 3f9e 6840  sPr......\=.?.h@
+000065b0: ea77 9e36 0975 b180 d337 bf4e a278 8b19  .w.6.u...7.N.x..
+000065c0: e472 329c c7c0 3981 7cf9 c359 d992 38db  .r2...9.|..Y..8.
+000065d0: f683 e5a7 9acf 403b 9456 dde4 b5c6 0f23  ......@;.V.....#
+000065e0: f3ce 94f3 a697 43c6 65c6 5abf 0100 00ff  ......C.e.Z.....
+000065f0: ff03 0050 4b01 022d 0014 0006 0008 0000  ...PK..-........
+00006600: 0021 00f3 1e96 b1bb 0100 0087 0800 0013  .!..............
+00006610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006620: 005b 436f 6e74 656e 745f 5479 7065 735d  .[Content_Types]
+00006630: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00006640: 0000 2100 b555 3023 f400 0000 4c02 0000  ..!..U0#....L...
+00006650: 0b00 0000 0000 0000 0000 0000 0000 f403  ................
+00006660: 0000 5f72 656c 732f 2e72 656c 7350 4b01  .._rels/.relsPK.
+00006670: 022d 0014 0006 0008 0000 0021 005d f2ab  .-.........!.]..
+00006680: 8aa9 0400 0096 0d00 000f 0000 0000 0000  ................
+00006690: 0000 0000 0000 0019 0700 0078 6c2f 776f  ...........xl/wo
+000066a0: 726b 626f 6f6b 2e78 6d6c 504b 0102 2d00  rkbook.xmlPK..-.
+000066b0: 1400 0600 0800 0000 2100 a189 0e7a 2501  ........!....z%.
+000066c0: 0000 e104 0000 1a00 0000 0000 0000 0000  ................
+000066d0: 0000 0000 ef0b 0000 786c 2f5f 7265 6c73  ........xl/_rels
+000066e0: 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e 7265  /workbook.xml.re
+000066f0: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
+00006700: 2100 c712 3e03 6812 0000 6daa 0000 1800  !...>.h...m.....
+00006710: 0000 0000 0000 0000 0000 0000 540e 0000  ............T...
+00006720: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00006730: 6565 7431 2e78 6d6c 504b 0102 2d00 1400  eet1.xmlPK..-...
+00006740: 0600 0800 0000 2100 46d3 a5b7 d30a 0000  ......!.F.......
+00006750: 4b4c 0000 1800 0000 0000 0000 0000 0000  KL..............
+00006760: 0000 f220 0000 786c 2f77 6f72 6b73 6865  ... ..xl/workshe
+00006770: 6574 732f 7368 6565 7432 2e78 6d6c 504b  ets/sheet2.xmlPK
+00006780: 0102 2d00 1400 0600 0800 0000 2100 b590  ..-.........!...
+00006790: 2cdd b704 0000 690f 0000 1800 0000 0000  ,.....i.........
+000067a0: 0000 0000 0000 0000 fb2b 0000 786c 2f77  .........+..xl/w
+000067b0: 6f72 6b73 6865 6574 732f 7368 6565 7433  orksheets/sheet3
+000067c0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+000067d0: 0000 2100 b145 0dec 5c07 0000 0221 0000  ..!..E..\....!..
+000067e0: 1300 0000 0000 0000 0000 0000 0000 e830  ...............0
+000067f0: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
+00006800: 312e 786d 6c50 4b01 022d 0014 0006 0008  1.xmlPK..-......
+00006810: 0000 0021 00d2 e522 5543 0500 0048 1a00  ...!..."UC...H..
+00006820: 000d 0000 0000 0000 0000 0000 0000 0075  ...............u
+00006830: 3800 0078 6c2f 7374 796c 6573 2e78 6d6c  8..xl/styles.xml
+00006840: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00006850: 1152 c103 8702 0000 2e08 0000 1400 0000  .R..............
+00006860: 0000 0000 0000 0000 0000 e33d 0000 786c  ...........=..xl
+00006870: 2f73 6861 7265 6453 7472 696e 6773 2e78  /sharedStrings.x
+00006880: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00006890: 2100 72a0 d0dc 5802 0000 c108 0000 1800  !.r...X.........
+000068a0: 0000 0000 0000 0000 0000 0000 9c40 0000  .............@..
+000068b0: 786c 2f64 7261 7769 6e67 732f 6472 6177  xl/drawings/draw
+000068c0: 696e 6731 2e78 6d6c 504b 0102 2d00 1400  ing1.xmlPK..-...
+000068d0: 0600 0800 0000 2100 31b0 25e4 2609 0000  ......!.1.%.&...
+000068e0: f433 0000 1400 0000 0000 0000 0000 0000  .3..............
+000068f0: 0000 2a43 0000 786c 2f63 6861 7274 732f  ..*C..xl/charts/
+00006900: 6368 6172 7431 2e78 6d6c 504b 0102 2d00  chart1.xmlPK..-.
+00006910: 1400 0600 0800 0000 2100 767e a5b1 d307  ........!.v~....
+00006920: 0000 d926 0000 1400 0000 0000 0000 0000  ...&............
+00006930: 0000 0000 824c 0000 786c 2f63 6861 7274  .....L..xl/chart
+00006940: 732f 6368 6172 7432 2e78 6d6c 504b 0102  s/chart2.xmlPK..
+00006950: 2d00 1400 0600 0800 0000 2100 3b6d 324b  -.........!.;m2K
+00006960: c100 0000 4201 0000 2300 0000 0000 0000  ....B...#.......
+00006970: 0000 0000 0000 8754 0000 786c 2f77 6f72  .......T..xl/wor
+00006980: 6b73 6865 6574 732f 5f72 656c 732f 7368  ksheets/_rels/sh
+00006990: 6565 7431 2e78 6d6c 2e72 656c 7350 4b01  eet1.xml.relsPK.
+000069a0: 022d 0014 0006 0008 0000 0021 0011 98ab  .-.........!....
+000069b0: c9db 0000 00d0 0100 0023 0000 0000 0000  .........#......
+000069c0: 0000 0000 0000 0089 5500 0078 6c2f 776f  ........U..xl/wo
+000069d0: 726b 7368 6565 7473 2f5f 7265 6c73 2f73  rksheets/_rels/s
+000069e0: 6865 6574 322e 786d 6c2e 7265 6c73 504b  heet2.xml.relsPK
+000069f0: 0102 2d00 1400 0600 0800 0000 2100 81f1  ..-.........!...
+00006a00: a03f c400 0000 ad01 0000 2300 0000 0000  .?........#.....
+00006a10: 0000 0000 0000 0000 a556 0000 786c 2f64  .........V..xl/d
+00006a20: 7261 7769 6e67 732f 5f72 656c 732f 6472  rawings/_rels/dr
+00006a30: 6177 696e 6731 2e78 6d6c 2e72 656c 7350  awing1.xml.relsP
+00006a40: 4b01 022d 0014 0006 0008 0000 0021 0090  K..-.........!..
+00006a50: 000d b0a6 0100 00dd 0200 000f 0000 0000  ................
+00006a60: 0000 0000 0000 0000 00aa 5700 0078 6c2f  ..........W..xl/
+00006a70: 6d65 7461 6461 7461 2e78 6d6c 504b 0102  metadata.xmlPK..
+00006a80: 2d00 1400 0600 0800 0000 2100 3585 fa75  -.........!.5..u
+00006a90: af01 0000 3c10 0000 2700 0000 0000 0000  ....<...'.......
+00006aa0: 0000 0000 0000 7d59 0000 786c 2f70 7269  ......}Y..xl/pri
+00006ab0: 6e74 6572 5365 7474 696e 6773 2f70 7269  nterSettings/pri
+00006ac0: 6e74 6572 5365 7474 696e 6773 312e 6269  nterSettings1.bi
+00006ad0: 6e50 4b01 022d 0014 0006 0008 0000 0021  nPK..-.........!
+00006ae0: 0035 85fa 75af 0100 003c 1000 0027 0000  .5..u....<...'..
+00006af0: 0000 0000 0000 0000 0000 0071 5b00 0078  ...........q[..x
+00006b00: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+00006b10: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+00006b20: 7332 2e62 696e 504b 0102 2d00 1400 0600  s2.binPK..-.....
+00006b30: 0800 0000 2100 ecff 94f0 8002 0000 620c  ....!.........b.
+00006b40: 0000 1000 0000 0000 0000 0000 0000 0000  ................
+00006b50: 655d 0000 786c 2f63 616c 6343 6861 696e  e]..xl/calcChain
+00006b60: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00006b70: 0000 2100 9ce9 d5ff 4d01 0000 6902 0000  ..!.....M...i...
+00006b80: 1100 0000 0000 0000 0000 0000 0000 1360  ...............`
+00006b90: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
+00006ba0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+00006bb0: 0021 005c 3fd8 9426 0200 00a9 0500 0010  .!.\?..&........
+00006bc0: 0000 0000 0000 0000 0000 0000 0097 6200  ..............b.
+00006bd0: 0064 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
+00006be0: 6c50 4b05 0600 0000 0016 0016 00ee 0500  lPK.............
+00006bf0: 00f3 6500 0000 00                        ..e....
```

### Comparing `ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx` & `ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx` & `ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx` & `ragtime-0.0.33/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/tests/full_test.py` & `ragtime-0.0.33/tests/full_test.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/tests/run_tests.py` & `ragtime-0.0.33/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/tests/test_quest.json` & `ragtime-0.0.33/tests/test_quest.json`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/.gitignore` & `ragtime-0.0.33/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/LICENSE` & `ragtime-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/README.md` & `ragtime-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.32/pyproject.toml` & `ragtime-0.0.33/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ragtime"
-version = "0.0.32"
+version = "0.0.33"
 
 authors = [
   { name="Gilles Moyse", email="gilles@recital.ai" },
 ]
 maintainers = [
   { name="reciTAL", email="ragtime@recital.ai" },
 ]
```

### Comparing `ragtime-0.0.32/PKG-INFO` & `ragtime-0.0.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragtime
-Version: 0.0.32
+Version: 0.0.33
 Summary: Ragtime 🎹 is an LLMOps framework to automatically evaluate Retrieval Augmented Generation (RAG) systems and compare different RAGs / LLMs
 Project-URL: Homepage, https://github.com/recitalAI/ragtime-package
 Project-URL: Issues, https://github.com/recitalAI/ragtime-package/issues
 Author-email: Gilles Moyse <gilles@recital.ai>
 Maintainer-email: reciTAL <ragtime@recital.ai>
 License: MIT License
```

