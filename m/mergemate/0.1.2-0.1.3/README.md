# Comparing `tmp/mergemate-0.1.2.tar.gz` & `tmp/mergemate-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergemate-0.1.2.tar", last modified: Sun May 19 11:35:22 2024, max compression
+gzip compressed data, was "mergemate-0.1.3.tar", last modified: Sun May 19 12:11:53 2024, max compression
```

## Comparing `mergemate-0.1.2.tar` & `mergemate-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.027742 mergemate-0.1.2/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     1070 2024-05-19 09:57:02.000000 mergemate-0.1.2/LICENSE
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     4812 2024-05-19 11:35:22.027520 mergemate-0.1.2/PKG-INFO
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     4418 2024-05-19 10:19:29.000000 mergemate-0.1.2/README.md
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.024873 mergemate-0.1.2/mergemate/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:34:25.000000 mergemate-0.1.2/mergemate/__init__.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.025692 mergemate-0.1.2/mergemate/llmware/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:36.000000 mergemate-0.1.2/mergemate/llmware/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     3307 2024-05-19 10:20:44.000000 mergemate-0.1.2/mergemate/llmware/reviewer_agent.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.026293 mergemate-0.1.2/mergemate/providers/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:40.000000 mergemate-0.1.2/mergemate/providers/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     1623 2024-05-19 09:01:12.000000 mergemate-0.1.2/mergemate/providers/github.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.026424 mergemate-0.1.2/mergemate/scripts/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:46.000000 mergemate-0.1.2/mergemate/scripts/__init__.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.026986 mergemate-0.1.2/mergemate/scripts/github/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:46:00.000000 mergemate-0.1.2/mergemate/scripts/github/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      985 2024-05-19 09:02:30.000000 mergemate-0.1.2/mergemate/scripts/github/comment_handler.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      834 2024-05-19 08:45:56.000000 mergemate-0.1.2/mergemate/scripts/github/pr_review.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.027280 mergemate-0.1.2/mergemate.egg-info/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     4812 2024-05-19 11:35:21.000000 mergemate-0.1.2/mergemate.egg-info/PKG-INFO
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      489 2024-05-19 11:35:22.000000 mergemate-0.1.2/mergemate.egg-info/SOURCES.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        1 2024-05-19 11:35:21.000000 mergemate-0.1.2/mergemate.egg-info/dependency_links.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       17 2024-05-19 11:35:21.000000 mergemate-0.1.2/mergemate.egg-info/requires.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       10 2024-05-19 11:35:21.000000 mergemate-0.1.2/mergemate.egg-info/top_level.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       38 2024-05-19 11:35:22.027789 mergemate-0.1.2/setup.cfg
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      618 2024-05-19 11:35:01.000000 mergemate-0.1.2/setup.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.258167 mergemate-0.1.3/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     1070 2024-05-19 09:57:02.000000 mergemate-0.1.3/LICENSE
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     5366 2024-05-19 12:11:53.257958 mergemate-0.1.3/PKG-INFO
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     4973 2024-05-19 12:08:03.000000 mergemate-0.1.3/README.md
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.254401 mergemate-0.1.3/mergemate/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:34:25.000000 mergemate-0.1.3/mergemate/__init__.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.255199 mergemate-0.1.3/mergemate/llmware/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:36.000000 mergemate-0.1.3/mergemate/llmware/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     3017 2024-05-19 12:11:23.000000 mergemate-0.1.3/mergemate/llmware/reviewer_agent.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.255970 mergemate-0.1.3/mergemate/prompts/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:10:31.000000 mergemate-0.1.3/mergemate/prompts/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      632 2024-05-19 12:09:51.000000 mergemate-0.1.3/mergemate/prompts/answer_comment.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      644 2024-05-19 12:10:09.000000 mergemate-0.1.3/mergemate/prompts/create_review.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      360 2024-05-19 12:10:22.000000 mergemate-0.1.3/mergemate/prompts/explain_code.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.256708 mergemate-0.1.3/mergemate/providers/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:40.000000 mergemate-0.1.3/mergemate/providers/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     1623 2024-05-19 09:01:12.000000 mergemate-0.1.3/mergemate/providers/github.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.256822 mergemate-0.1.3/mergemate/scripts/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:46.000000 mergemate-0.1.3/mergemate/scripts/__init__.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.257356 mergemate-0.1.3/mergemate/scripts/github/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:46:00.000000 mergemate-0.1.3/mergemate/scripts/github/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      985 2024-05-19 09:02:30.000000 mergemate-0.1.3/mergemate/scripts/github/comment_handler.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      834 2024-05-19 08:45:56.000000 mergemate-0.1.3/mergemate/scripts/github/pr_review.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.257701 mergemate-0.1.3/mergemate.egg-info/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     5366 2024-05-19 12:11:53.000000 mergemate-0.1.3/mergemate.egg-info/PKG-INFO
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      624 2024-05-19 12:11:53.000000 mergemate-0.1.3/mergemate.egg-info/SOURCES.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        1 2024-05-19 12:11:53.000000 mergemate-0.1.3/mergemate.egg-info/dependency_links.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       17 2024-05-19 12:11:53.000000 mergemate-0.1.3/mergemate.egg-info/requires.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       10 2024-05-19 12:11:53.000000 mergemate-0.1.3/mergemate.egg-info/top_level.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       38 2024-05-19 12:11:53.258211 mergemate-0.1.3/setup.cfg
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      618 2024-05-19 12:11:36.000000 mergemate-0.1.3/setup.py
```

### Comparing `mergemate-0.1.2/LICENSE` & `mergemate-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.2/PKG-INFO` & `mergemate-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,14 @@
-Metadata-Version: 2.1
-Name: mergemate
-Version: 0.1.2
-Summary: An automated tool to handle GitHub pull requests and comments.
-Home-page: http://pypi.python.org/pypi/MergeMate/
-Author: Hardeep Singh
-Author-email: hardeep0khalsa122@gmail.com
-License: LICENSE.txt
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: llmware
-Requires-Dist: pygithub
-
 
 # MergeMate: Automated PR Review and Command Handling
+[![MIT License](https://img.shields.io/github/license/Hardeepsingh980/mergemate)](https://github.com/Hardeepsingh980/mergemate/blob/master/LICENSE)
+![coverage](https://img.shields.io/badge/coverage-80%25-yellowgreen)
+![version](https://img.shields.io/badge/version-0.1.2-blue)
+[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
+![commits](https://img.shields.io/github/commit-activity/m/Hardeepsingh980/mergemate)
 
 MergeMate is a sophisticated tool crafted to automate pull request reviews and manage command-based interactions within GitHub issues. It harnesses LLMWare, a comprehensive development framework featuring tools and finely-tuned, to deliver insightful, context-aware responses directly within your git workflow.
 
 ## Features
 
 - **Advanced Integration with LLMWare**: Leverages LLMWare to analyze code and manage interactions, utilizing the latest AI technologies for natural language understanding and decision-making.
 - **Automated PR Reviews**: Generates thorough reviews for pull requests automatically, including specific code suggestions and adherence to best practices.
@@ -38,14 +29,15 @@
 
 ## GitHub Action Setup
 
 Incorporate MergeMate into your GitHub workflows using this configuration:
 
 ### Workflow Definition
 
+Create the workflow file at `.github/workflows/mergemate.yml`.
 ```yaml
 name: Automated PR Review and Command Handling
 
 on:
   pull_request:
     types: [opened, synchronize]
   issue_comment:
@@ -86,14 +78,15 @@
         run: pip install mergemate
       - name: Handle Comment
         run: python -m mergemate.scripts.github.comment_handler
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
 ```
+`NOTE`: Do not forget to add `OPENAI_API_KEY` in Github Secrets.
 
 ## Documentation
 
 Extensive documentation is included within the package, providing detailed setup instructions, configuration options, and command usage. This ensures that users ranging from beginners to experienced developers can effectively utilize and customize MergeMate.
 
 ## Contributing
```

### Comparing `mergemate-0.1.2/README.md` & `mergemate-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,28 @@
+Metadata-Version: 2.1
+Name: mergemate
+Version: 0.1.3
+Summary: An automated tool to handle GitHub pull requests and comments.
+Home-page: http://pypi.python.org/pypi/MergeMate/
+Author: Hardeep Singh
+Author-email: hardeep0khalsa122@gmail.com
+License: LICENSE.txt
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: llmware
+Requires-Dist: pygithub
+
 
 # MergeMate: Automated PR Review and Command Handling
+[![MIT License](https://img.shields.io/github/license/Hardeepsingh980/mergemate)](https://github.com/Hardeepsingh980/mergemate/blob/master/LICENSE)
+![coverage](https://img.shields.io/badge/coverage-80%25-yellowgreen)
+![version](https://img.shields.io/badge/version-0.1.2-blue)
+[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
+![commits](https://img.shields.io/github/commit-activity/m/Hardeepsingh980/mergemate)
 
 MergeMate is a sophisticated tool crafted to automate pull request reviews and manage command-based interactions within GitHub issues. It harnesses LLMWare, a comprehensive development framework featuring tools and finely-tuned, to deliver insightful, context-aware responses directly within your git workflow.
 
 ## Features
 
 - **Advanced Integration with LLMWare**: Leverages LLMWare to analyze code and manage interactions, utilizing the latest AI technologies for natural language understanding and decision-making.
 - **Automated PR Reviews**: Generates thorough reviews for pull requests automatically, including specific code suggestions and adherence to best practices.
@@ -24,14 +43,15 @@
 
 ## GitHub Action Setup
 
 Incorporate MergeMate into your GitHub workflows using this configuration:
 
 ### Workflow Definition
 
+Create the workflow file at `.github/workflows/mergemate.yml`.
 ```yaml
 name: Automated PR Review and Command Handling
 
 on:
   pull_request:
     types: [opened, synchronize]
   issue_comment:
@@ -72,14 +92,15 @@
         run: pip install mergemate
       - name: Handle Comment
         run: python -m mergemate.scripts.github.comment_handler
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
 ```
+`NOTE`: Do not forget to add `OPENAI_API_KEY` in Github Secrets.
 
 ## Documentation
 
 Extensive documentation is included within the package, providing detailed setup instructions, configuration options, and command usage. This ensures that users ranging from beginners to experienced developers can effectively utilize and customize MergeMate.
 
 ## Contributing
 
@@ -87,8 +108,8 @@
 
 ## Licensing
 
 MergeMate is proudly released under the MIT license. This permissive licensing fosters widespread adoption and significant contributions from the community, supporting both personal and commercial use.
 
 ---
 
-MergeMate epitomizes the next step in automating interactions within GitHub's ecosystem, propelled by the ongoing advancement of AI-driven development tools. Your feedback and contributions are invaluable to us as we aim to continually expand and enhance MergeMate's capabilities, catering to a growing range of development environments and communities.
+MergeMate epitomizes the next step in automating interactions within GitHub's ecosystem, propelled by the ongoing advancement of AI-driven development tools. Your feedback and contributions are invaluable to us as we aim to continually expand and enhance MergeMate's capabilities, catering to a growing range of development environments and communities.
```

### Comparing `mergemate-0.1.2/mergemate/llmware/reviewer_agent.py` & `mergemate-0.1.3/mergemate/llmware/reviewer_agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 from llmware.prompts import Prompt
 import os
+from prompts import answer_comment, create_review, explain_code
 
 class ReviewerAgent:
     def __init__(self):
         self.prompt = Prompt().load_model('gpt-3.5-turbo', api_key=os.environ['OPENAI_API_KEY'])
         self.help_commands = {
             '/help': 'List all available commands.',
             '/explain': 'Explain the current code context',
             '/status': 'Get the current status of the PR.',
             '/ask': 'Ask a question about the the PR.'
         }
 
-        review_prompt = open('mergemate/prompts/create_review.txt', 'r')
-        self.review_prompt = review_prompt.read()
-        review_prompt.close()
-
-        explain_code_prompt = open('mergemate/prompts/explain_code.txt', 'r')
-        self.explain_code_prompt = explain_code_prompt.read()
-        explain_code_prompt.close()
-
-        answer_comment_prompt = open('mergemate/prompts/answer_comment.txt', 'r')
-        self.answer_comment_prompt = answer_comment_prompt.read()
-        answer_comment_prompt.close()
+        self.review_prompt = create_review.PROMPT
+        self.explain_code_prompt = explain_code.PROMPT
+        self.answer_comment_prompt = answer_comment.PROMPT
         
-
     def return_response(self, response):
         header = ":sparkles: **MergeMate Bot** :sparkles:\n\n"
         footer = "\n\n:bulb: *Use `/help` to list all available commands.* :bulb:"
         return header + response + footer
 
     def run(self, prompt, context=None):
         response = self.prompt.prompt_main(
```

### Comparing `mergemate-0.1.2/mergemate/providers/github.py` & `mergemate-0.1.3/mergemate/providers/github.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.2/mergemate/scripts/github/comment_handler.py` & `mergemate-0.1.3/mergemate/scripts/github/comment_handler.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.2/mergemate/scripts/github/pr_review.py` & `mergemate-0.1.3/mergemate/scripts/github/pr_review.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.2/mergemate.egg-info/PKG-INFO` & `mergemate-0.1.3/mergemate.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: mergemate
-Version: 0.1.2
+Version: 0.1.3
 Summary: An automated tool to handle GitHub pull requests and comments.
 Home-page: http://pypi.python.org/pypi/MergeMate/
 Author: Hardeep Singh
 Author-email: hardeep0khalsa122@gmail.com
 License: LICENSE.txt
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: llmware
 Requires-Dist: pygithub
 
 
 # MergeMate: Automated PR Review and Command Handling
+[![MIT License](https://img.shields.io/github/license/Hardeepsingh980/mergemate)](https://github.com/Hardeepsingh980/mergemate/blob/master/LICENSE)
+![coverage](https://img.shields.io/badge/coverage-80%25-yellowgreen)
+![version](https://img.shields.io/badge/version-0.1.2-blue)
+[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
+![commits](https://img.shields.io/github/commit-activity/m/Hardeepsingh980/mergemate)
 
 MergeMate is a sophisticated tool crafted to automate pull request reviews and manage command-based interactions within GitHub issues. It harnesses LLMWare, a comprehensive development framework featuring tools and finely-tuned, to deliver insightful, context-aware responses directly within your git workflow.
 
 ## Features
 
 - **Advanced Integration with LLMWare**: Leverages LLMWare to analyze code and manage interactions, utilizing the latest AI technologies for natural language understanding and decision-making.
 - **Automated PR Reviews**: Generates thorough reviews for pull requests automatically, including specific code suggestions and adherence to best practices.
@@ -38,14 +43,15 @@
 
 ## GitHub Action Setup
 
 Incorporate MergeMate into your GitHub workflows using this configuration:
 
 ### Workflow Definition
 
+Create the workflow file at `.github/workflows/mergemate.yml`.
 ```yaml
 name: Automated PR Review and Command Handling
 
 on:
   pull_request:
     types: [opened, synchronize]
   issue_comment:
@@ -86,14 +92,15 @@
         run: pip install mergemate
       - name: Handle Comment
         run: python -m mergemate.scripts.github.comment_handler
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
 ```
+`NOTE`: Do not forget to add `OPENAI_API_KEY` in Github Secrets.
 
 ## Documentation
 
 Extensive documentation is included within the package, providing detailed setup instructions, configuration options, and command usage. This ensures that users ranging from beginners to experienced developers can effectively utilize and customize MergeMate.
 
 ## Contributing
```

### Comparing `mergemate-0.1.2/setup.py` & `mergemate-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mergemate',
-    version='0.1.2',
+    version='0.1.3',
     author='Hardeep Singh',
     author_email='hardeep0khalsa122@gmail.com',
     packages=find_packages(),
     scripts=['mergemate/scripts/github/comment_handler.py'],
     url='http://pypi.python.org/pypi/MergeMate/',
     license='LICENSE.txt',
     description='An automated tool to handle GitHub pull requests and comments.',
```

