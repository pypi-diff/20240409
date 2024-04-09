# Comparing `tmp/educhain-0.1.4.tar.gz` & `tmp/educhain-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "educhain-0.1.4.tar", last modified: Sat Mar 30 21:01:30 2024, max compression
+gzip compressed data, was "educhain-0.1.6.tar", last modified: Tue Apr  9 08:15:45 2024, max compression
```

## Comparing `educhain-0.1.4.tar` & `educhain-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-03-30 21:01:30.542851 educhain-0.1.4/
--rw-r--r--   0 satvikp    (501) staff       (20)     1066 2024-03-22 08:48:24.000000 educhain-0.1.4/LICENSE
--rw-r--r--   0 satvikp    (501) staff       (20)     2309 2024-03-30 21:01:30.542643 educhain-0.1.4/PKG-INFO
--rw-r--r--   0 satvikp    (501) staff       (20)     1479 2024-03-29 11:07:39.000000 educhain-0.1.4/README.md
-drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-03-30 21:01:30.541546 educhain-0.1.4/educhain/
--rw-r--r--   0 satvikp    (501) staff       (20)       73 2024-03-11 17:35:12.000000 educhain-0.1.4/educhain/__init__.py
--rw-r--r--   0 satvikp    (501) staff       (20)      829 2024-03-29 15:25:05.000000 educhain-0.1.4/educhain/content_engine.py
--rw-r--r--   0 satvikp    (501) staff       (20)      670 2024-03-30 20:52:51.000000 educhain-0.1.4/educhain/models.py
--rw-r--r--   0 satvikp    (501) staff       (20)     1642 2024-03-29 15:12:13.000000 educhain-0.1.4/educhain/qna_engine.py
--rw-r--r--   0 satvikp    (501) staff       (20)      625 2024-03-27 15:00:18.000000 educhain-0.1.4/educhain/utils.py
-drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-03-30 21:01:30.542404 educhain-0.1.4/educhain.egg-info/
--rw-r--r--   0 satvikp    (501) staff       (20)     2309 2024-03-30 21:01:30.000000 educhain-0.1.4/educhain.egg-info/PKG-INFO
--rw-r--r--   0 satvikp    (501) staff       (20)      293 2024-03-30 21:01:30.000000 educhain-0.1.4/educhain.egg-info/SOURCES.txt
--rw-r--r--   0 satvikp    (501) staff       (20)        1 2024-03-30 21:01:30.000000 educhain-0.1.4/educhain.egg-info/dependency_links.txt
--rw-r--r--   0 satvikp    (501) staff       (20)       55 2024-03-30 21:01:30.000000 educhain-0.1.4/educhain.egg-info/requires.txt
--rw-r--r--   0 satvikp    (501) staff       (20)        9 2024-03-30 21:01:30.000000 educhain-0.1.4/educhain.egg-info/top_level.txt
--rw-r--r--   0 satvikp    (501) staff       (20)       38 2024-03-30 21:01:30.542895 educhain-0.1.4/setup.cfg
--rw-r--r--   0 satvikp    (501) staff       (20)      988 2024-03-30 21:01:00.000000 educhain-0.1.4/setup.py
+drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-04-09 08:15:45.873461 educhain-0.1.6/
+-rw-r--r--   0 satvikp    (501) staff       (20)     1066 2024-03-22 08:48:24.000000 educhain-0.1.6/LICENSE
+-rw-r--r--   0 satvikp    (501) staff       (20)     3824 2024-04-09 08:15:45.873175 educhain-0.1.6/PKG-INFO
+-rw-r--r--   0 satvikp    (501) staff       (20)     2934 2024-04-09 07:28:28.000000 educhain-0.1.6/README.md
+drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-04-09 08:15:45.870324 educhain-0.1.6/educhain/
+-rw-r--r--   0 satvikp    (501) staff       (20)      211 2024-04-09 07:28:28.000000 educhain-0.1.6/educhain/__init__.py
+-rw-r--r--   0 satvikp    (501) staff       (20)      857 2024-04-01 15:53:35.000000 educhain-0.1.6/educhain/content_engine.py
+-rw-r--r--   0 satvikp    (501) staff       (20)      668 2024-04-09 07:28:28.000000 educhain-0.1.6/educhain/models.py
+-rw-r--r--   0 satvikp    (501) staff       (20)     1518 2024-04-09 08:00:49.000000 educhain-0.1.6/educhain/qna_engine.py
+-rw-r--r--   0 satvikp    (501) staff       (20)     3047 2024-04-09 07:28:28.000000 educhain-0.1.6/educhain/utils.py
+drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-04-09 08:15:45.871692 educhain-0.1.6/educhain.egg-info/
+-rw-r--r--   0 satvikp    (501) staff       (20)     3824 2024-04-09 08:15:45.000000 educhain-0.1.6/educhain.egg-info/PKG-INFO
+-rw-r--r--   0 satvikp    (501) staff       (20)      293 2024-04-09 08:15:45.000000 educhain-0.1.6/educhain.egg-info/SOURCES.txt
+-rw-r--r--   0 satvikp    (501) staff       (20)        1 2024-04-09 08:15:45.000000 educhain-0.1.6/educhain.egg-info/dependency_links.txt
+-rw-r--r--   0 satvikp    (501) staff       (20)       85 2024-04-09 08:15:45.000000 educhain-0.1.6/educhain.egg-info/requires.txt
+-rw-r--r--   0 satvikp    (501) staff       (20)        9 2024-04-09 08:15:45.000000 educhain-0.1.6/educhain.egg-info/top_level.txt
+-rw-r--r--   0 satvikp    (501) staff       (20)       38 2024-04-09 08:15:45.873545 educhain-0.1.6/setup.cfg
+-rw-r--r--   0 satvikp    (501) staff       (20)     1040 2024-04-09 08:08:01.000000 educhain-0.1.6/setup.py
```

### Comparing `educhain-0.1.4/LICENSE` & `educhain-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `educhain-0.1.4/educhain/content_engine.py` & `educhain-0.1.6/educhain/content_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from langchain.chains import LLMChain
 
 def generate_lesson_plan(subject, level, llm=None):
 
     if llm:
         llm = llm
     else:
-        llm = ChatOpenAI()
+        llm = ChatOpenAI(model = 'gpt-3.5-turbo-0125')
 
     prompt = PromptTemplate(
         input_variables=["subject", "level"],
         template="""
     Generate a lesson plan for the given subject and level.
     Provide a detailed outline of the lesson, including an introduction, main activities, and a conclusion.
```

### Comparing `educhain-0.1.4/educhain/models.py` & `educhain-0.1.6/educhain/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     correct_answer: str
     
     def show(self):
         options_str = "\n".join(f"  {chr(65 + i)}. {option}" for i, option in enumerate(self.options))
         print(f"Question: {self.question}\nOptions:\n{options_str}\nCorrect Answer: {self.correct_answer}\n")
 
 
-
-
 class MCQList(BaseModel):
     questions: List[MCQ]
 
     def show(self):
         print("MCQs:\n")
         for i, mcq in enumerate(self.questions):
             print(f"Question {i + 1}:")
```

### Comparing `educhain-0.1.4/educhain/qna_engine.py` & `educhain-0.1.6/educhain/qna_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import json
-from .utils import to_csv  # Import the to_csv function from the utils module
+from .utils import to_csv, to_json, to_pdf  ###
 from langchain_openai import ChatOpenAI
 from langchain.prompts import PromptTemplate
 from langchain.chains import LLMChain
 from langchain.output_parsers import PydanticOutputParser
-from .models import MCQList, MCQ
-    
-def generate_mcq(topic, level = "Intermediate", num = 1, llm = None, file_name=None):
+from .models import MCQList ###
+
 
-    parser = PydanticOutputParser(pydantic_object=MCQList)
 
+def generate_mcq(topic, level, num=1, llm=None, prompt_template=None, **kwargs):
+    parser = PydanticOutputParser(pydantic_object=MCQList)
     format_instructions = parser.get_format_instructions()
 
-    MCQ_template = """
-    Generate {num} multiple-choice question (MCQ) based on the given topic and level.
-    provide the question, four answer options, and the correct answer.
-
-    Topic: {topic}
-    Level: {level}
-
-    The response should be in JSON format. \n {format_instructions}
-    """
-
-    MCQ_prompt = PromptTemplate(input_variables=["num", "topic", "level"],
-                                template=MCQ_template,
-                                partial_variables={"format_instructions": format_instructions}
-                                )
-    
+    if prompt_template is None:
+        prompt_template = """
+        Generate {num} multiple-choice question (MCQ) based on the given topic and level.
+        provide the question, four answer options, and the correct answer.
+
+        Topic: {topic}
+        Level: {level}
+        """
+
+    # Append the JSON format instruction line to the custom prompt template
+    prompt_template += "\nThe response should be in JSON format. \n {format_instructions}"
+
+    MCQ_prompt = PromptTemplate(
+        input_variables=["num", "topic", "level"],
+        template=prompt_template,
+        partial_variables={"format_instructions": format_instructions}
+    )
+
     if llm:
         llm = llm
     else:
-        llm = ChatOpenAI()
+        llm = ChatOpenAI(model="gpt-3.5-turbo-0125")
 
     MCQ_chain = LLMChain(llm=llm, prompt=MCQ_prompt)
-    results = MCQ_chain.invoke({"num": num,
-                                    "topic": topic,
-                                    "level": level
-                                    }, return_only_outputs=True)
+
+    results = MCQ_chain.invoke(
+        {"num": num, "topic": topic, "level": level, **kwargs},
+        return_only_outputs=True
+    )
 
     results = results["text"]
     structured_output = parser.parse(results)
-    
-    # Generate Csv file if file_name is provided
-    if file_name:
-        to_csv(structured_output, file_name)
-        
+
     return structured_output
+
```

### Comparing `educhain-0.1.4/setup.py` & `educhain-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="educhain",
-    version="0.1.4",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=[
         "langchain",
+        "langchain-community",
         "langchain-openai",
         "openai",
         "python-dotenv", 
-        "pandas"
+        "pandas",
+        "reportlab"
     ],
     author="Satvik Paramkusham",
     author_email="satvik@buildfastwithai.com",
     description="A Python package for generating educational content using Generative AI",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/satvik314/educhain",
```

