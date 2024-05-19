# Comparing `tmp/mergemate-0.1.0.tar.gz` & `tmp/mergemate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergemate-0.1.0.tar", last modified: Sun May 19 10:08:34 2024, max compression
+gzip compressed data, was "mergemate-0.1.1.tar", last modified: Sun May 19 10:23:23 2024, max compression
```

## Comparing `mergemate-0.1.0.tar` & `mergemate-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:08:34.411554 mergemate-0.1.0/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     1070 2024-05-19 09:57:02.000000 mergemate-0.1.0/LICENSE
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     4517 2024-05-19 10:08:34.411320 mergemate-0.1.0/PKG-INFO
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     4123 2024-05-19 10:00:21.000000 mergemate-0.1.0/README.md
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:08:34.408974 mergemate-0.1.0/llmware/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:36.000000 mergemate-0.1.0/llmware/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     3305 2024-05-19 09:43:39.000000 mergemate-0.1.0/llmware/reviewer_agent.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:08:34.411045 mergemate-0.1.0/mergemate.egg-info/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     4517 2024-05-19 10:08:34.000000 mergemate-0.1.0/mergemate.egg-info/PKG-INFO
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      387 2024-05-19 10:08:34.000000 mergemate-0.1.0/mergemate.egg-info/SOURCES.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        1 2024-05-19 10:08:34.000000 mergemate-0.1.0/mergemate.egg-info/dependency_links.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       17 2024-05-19 10:08:34.000000 mergemate-0.1.0/mergemate.egg-info/requires.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       26 2024-05-19 10:08:34.000000 mergemate-0.1.0/mergemate.egg-info/top_level.txt
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:08:34.409869 mergemate-0.1.0/providers/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:40.000000 mergemate-0.1.0/providers/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     1623 2024-05-19 09:01:12.000000 mergemate-0.1.0/providers/github.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:08:34.410126 mergemate-0.1.0/scripts/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:46.000000 mergemate-0.1.0/scripts/__init__.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:08:34.410728 mergemate-0.1.0/scripts/github/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:46:00.000000 mergemate-0.1.0/scripts/github/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      985 2024-05-19 09:02:30.000000 mergemate-0.1.0/scripts/github/comment_handler.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      834 2024-05-19 08:45:56.000000 mergemate-0.1.0/scripts/github/pr_review.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       38 2024-05-19 10:08:34.411602 mergemate-0.1.0/setup.cfg
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      608 2024-05-19 10:08:26.000000 mergemate-0.1.0/setup.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.375730 mergemate-0.1.1/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     1070 2024-05-19 09:57:02.000000 mergemate-0.1.1/LICENSE
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     4812 2024-05-19 10:23:23.375454 mergemate-0.1.1/PKG-INFO
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     4418 2024-05-19 10:19:29.000000 mergemate-0.1.1/README.md
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.371776 mergemate-0.1.1/llmware/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:36.000000 mergemate-0.1.1/llmware/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     3307 2024-05-19 10:20:44.000000 mergemate-0.1.1/llmware/reviewer_agent.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.374731 mergemate-0.1.1/mergemate.egg-info/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     4812 2024-05-19 10:23:23.000000 mergemate-0.1.1/mergemate.egg-info/PKG-INFO
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      387 2024-05-19 10:23:23.000000 mergemate-0.1.1/mergemate.egg-info/SOURCES.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        1 2024-05-19 10:23:23.000000 mergemate-0.1.1/mergemate.egg-info/dependency_links.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       17 2024-05-19 10:23:23.000000 mergemate-0.1.1/mergemate.egg-info/requires.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       26 2024-05-19 10:23:23.000000 mergemate-0.1.1/mergemate.egg-info/top_level.txt
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.372907 mergemate-0.1.1/providers/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:40.000000 mergemate-0.1.1/providers/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     1623 2024-05-19 09:01:12.000000 mergemate-0.1.1/providers/github.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.373157 mergemate-0.1.1/scripts/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:46.000000 mergemate-0.1.1/scripts/__init__.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.374377 mergemate-0.1.1/scripts/github/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:46:00.000000 mergemate-0.1.1/scripts/github/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      985 2024-05-19 09:02:30.000000 mergemate-0.1.1/scripts/github/comment_handler.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      834 2024-05-19 08:45:56.000000 mergemate-0.1.1/scripts/github/pr_review.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       38 2024-05-19 10:23:23.376058 mergemate-0.1.1/setup.cfg
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      608 2024-05-19 10:21:30.000000 mergemate-0.1.1/setup.py
```

### Comparing `mergemate-0.1.0/LICENSE` & `mergemate-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.0/PKG-INFO` & `mergemate-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 Metadata-Version: 2.1
 Name: mergemate
-Version: 0.1.0
+Version: 0.1.1
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
 
+
 # MergeMate: Automated PR Review and Command Handling
 
-MergeMate is an advanced GitHub action designed to automate pull request reviews and handle command-based interactions within GitHub issues. It integrates state-of-the-art AI from OpenAI to provide insightful, context-aware responses to code reviews and comments directly within your GitHub workflow.
+MergeMate is a sophisticated tool crafted to automate pull request reviews and manage command-based interactions within GitHub issues. It harnesses LLMWare, a comprehensive development framework featuring tools and finely-tuned, to deliver insightful, context-aware responses directly within your git workflow.
 
 ## Features
 
-- **Automated PR Reviews**: Automatically generate detailed reviews for pull requests, including code suggestions and best practices.
-- **Command Handling**: Respond to commands in PR comments such as `/help`, `/explain`, `/status`, and `/ask` to facilitate more dynamic and interactive PR discussions.
-- **Markdown Support**: Enhances readability and user interaction by formatting responses in Markdown with customized headers and footers.
-- **Easy Integration**: Designed to work seamlessly as a GitHub action, allowing for straightforward integration into any project's CI/CD pipeline.
+- **Advanced Integration with LLMWare**: Leverages LLMWare to analyze code and manage interactions, utilizing the latest AI technologies for natural language understanding and decision-making.
+- **Automated PR Reviews**: Generates thorough reviews for pull requests automatically, including specific code suggestions and adherence to best practices.
+- **Command Handling**: Interprets and responds to commands in PR comments such as `/help`, `/explain`, `/status`, and `/ask`, enriching the interaction within PR discussions.
+- **Markdown Support**: Improves readability and interaction by utilizing Markdown for formatting responses, complete with custom headers and footers.
+- **Easy Integration**: Seamlessly integrates as a GitHub action, facilitating straightforward incorporation into any project's CI/CD pipeline.
+- **Future Expansion Plans**: Aimed at extending support to other repository management platforms like GitLab and Bitbucket, broadening the accessibility and utility of MergeMate across different development environments.
 
 ## Installation
 
-MergeMate can be easily installed via pip:
+Install MergeMate quickly and easily via pip at [mergemate](https://pypi.org/project/mergemate/):
 
 ```bash
 pip install mergemate
 ```
 
-This single command prepares your environment to leverage MergeMate's capabilities, streamlining your project's interaction paradigms.
+Deploying MergeMate prepares your environment to leverage advanced AI capabilities, streamlining project interactions and reviews.
 
 ## GitHub Action Setup
 
-MergeMate can be integrated into your GitHub workflows with the following configuration:
+Incorporate MergeMate into your GitHub workflows using this configuration:
 
 ### Workflow Definition
 
 ```yaml
 name: Automated PR Review and Command Handling
 
 on:
@@ -84,24 +87,22 @@
       - name: Handle Comment
         run: python -m mergemate.scripts.github.comment_handler
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
 ```
 
-This workflow automates PR reviews and handles specific commands in comments on pull requests. The configuration is optimized for GitHub actions, ensuring that the operations are only triggered under appropriate conditions to maintain efficiency and resource utilization.
-
 ## Documentation
 
-Comprehensive documentation is available within the package, detailing setup instructions, configuration options, and command details. This ensures that all potential users, from novices to seasoned developers, can effectively utilize and customize MergeMate according to their specific needs.
+Extensive documentation is included within the package, providing detailed setup instructions, configuration options, and command usage. This ensures that users ranging from beginners to experienced developers can effectively utilize and customize MergeMate.
 
-## Contribution
+## Contributing
 
-Contributions to MergeMate are welcomed. If you're interested in enhancing its capabilities or tailoring it to fit new use cases, please fork the repository and submit your pull requests. MergeMate is a living project, and contributions help it stay at the cutting edge of technology and usability.
+We warmly welcome contributions to MergeMate. If you are interested in enhancing its functionality or adapting it for additional use cases, please fork the repository and submit your pull requests. As an open-source project, MergeMate thrives on community involvement and contributions, which are crucial for its continuous evolution and enhancement.
 
 ## Licensing
 
-MergeMate is released under the MIT license, which provides great flexibility for both personal and commercial use, encouraging a broad adoption and diverse contributions from the community.
+MergeMate is proudly released under the MIT license. This permissive licensing fosters widespread adoption and significant contributions from the community, supporting both personal and commercial use.
 
 ---
 
-MergeMate represents a leap forward in automating interactions within GitHub's ecosystem, reflecting the ongoing evolution in development practices facilitated by advances in AI technology. As we continue to enhance its capabilities, your feedback and contributions are invaluable in shaping its future trajectory.
+MergeMate epitomizes the next step in automating interactions within GitHub's ecosystem, propelled by the ongoing advancement of AI-driven development tools. Your feedback and contributions are invaluable to us as we aim to continually expand and enhance MergeMate's capabilities, catering to a growing range of development environments and communities.
```

### Comparing `mergemate-0.1.0/README.md` & `mergemate-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+
 # MergeMate: Automated PR Review and Command Handling
 
-MergeMate is an advanced GitHub action designed to automate pull request reviews and handle command-based interactions within GitHub issues. It integrates state-of-the-art AI from OpenAI to provide insightful, context-aware responses to code reviews and comments directly within your GitHub workflow.
+MergeMate is a sophisticated tool crafted to automate pull request reviews and manage command-based interactions within GitHub issues. It harnesses LLMWare, a comprehensive development framework featuring tools and finely-tuned, to deliver insightful, context-aware responses directly within your git workflow.
 
 ## Features
 
-- **Automated PR Reviews**: Automatically generate detailed reviews for pull requests, including code suggestions and best practices.
-- **Command Handling**: Respond to commands in PR comments such as `/help`, `/explain`, `/status`, and `/ask` to facilitate more dynamic and interactive PR discussions.
-- **Markdown Support**: Enhances readability and user interaction by formatting responses in Markdown with customized headers and footers.
-- **Easy Integration**: Designed to work seamlessly as a GitHub action, allowing for straightforward integration into any project's CI/CD pipeline.
+- **Advanced Integration with LLMWare**: Leverages LLMWare to analyze code and manage interactions, utilizing the latest AI technologies for natural language understanding and decision-making.
+- **Automated PR Reviews**: Generates thorough reviews for pull requests automatically, including specific code suggestions and adherence to best practices.
+- **Command Handling**: Interprets and responds to commands in PR comments such as `/help`, `/explain`, `/status`, and `/ask`, enriching the interaction within PR discussions.
+- **Markdown Support**: Improves readability and interaction by utilizing Markdown for formatting responses, complete with custom headers and footers.
+- **Easy Integration**: Seamlessly integrates as a GitHub action, facilitating straightforward incorporation into any project's CI/CD pipeline.
+- **Future Expansion Plans**: Aimed at extending support to other repository management platforms like GitLab and Bitbucket, broadening the accessibility and utility of MergeMate across different development environments.
 
 ## Installation
 
-MergeMate can be easily installed via pip:
+Install MergeMate quickly and easily via pip at [mergemate](https://pypi.org/project/mergemate/):
 
 ```bash
 pip install mergemate
 ```
 
-This single command prepares your environment to leverage MergeMate's capabilities, streamlining your project's interaction paradigms.
+Deploying MergeMate prepares your environment to leverage advanced AI capabilities, streamlining project interactions and reviews.
 
 ## GitHub Action Setup
 
-MergeMate can be integrated into your GitHub workflows with the following configuration:
+Incorporate MergeMate into your GitHub workflows using this configuration:
 
 ### Workflow Definition
 
 ```yaml
 name: Automated PR Review and Command Handling
 
 on:
@@ -70,24 +73,22 @@
       - name: Handle Comment
         run: python -m mergemate.scripts.github.comment_handler
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
 ```
 
-This workflow automates PR reviews and handles specific commands in comments on pull requests. The configuration is optimized for GitHub actions, ensuring that the operations are only triggered under appropriate conditions to maintain efficiency and resource utilization.
-
 ## Documentation
 
-Comprehensive documentation is available within the package, detailing setup instructions, configuration options, and command details. This ensures that all potential users, from novices to seasoned developers, can effectively utilize and customize MergeMate according to their specific needs.
+Extensive documentation is included within the package, providing detailed setup instructions, configuration options, and command usage. This ensures that users ranging from beginners to experienced developers can effectively utilize and customize MergeMate.
 
-## Contribution
+## Contributing
 
-Contributions to MergeMate are welcomed. If you're interested in enhancing its capabilities or tailoring it to fit new use cases, please fork the repository and submit your pull requests. MergeMate is a living project, and contributions help it stay at the cutting edge of technology and usability.
+We warmly welcome contributions to MergeMate. If you are interested in enhancing its functionality or adapting it for additional use cases, please fork the repository and submit your pull requests. As an open-source project, MergeMate thrives on community involvement and contributions, which are crucial for its continuous evolution and enhancement.
 
 ## Licensing
 
-MergeMate is released under the MIT license, which provides great flexibility for both personal and commercial use, encouraging a broad adoption and diverse contributions from the community.
+MergeMate is proudly released under the MIT license. This permissive licensing fosters widespread adoption and significant contributions from the community, supporting both personal and commercial use.
 
 ---
 
-MergeMate represents a leap forward in automating interactions within GitHub's ecosystem, reflecting the ongoing evolution in development practices facilitated by advances in AI technology. As we continue to enhance its capabilities, your feedback and contributions are invaluable in shaping its future trajectory.
+MergeMate epitomizes the next step in automating interactions within GitHub's ecosystem, propelled by the ongoing advancement of AI-driven development tools. Your feedback and contributions are invaluable to us as we aim to continually expand and enhance MergeMate's capabilities, catering to a growing range of development environments and communities.
```

### Comparing `mergemate-0.1.0/llmware/reviewer_agent.py` & `mergemate-0.1.1/llmware/reviewer_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         )
         return self.return_response(response['llm_response'])
     
     def create_comment(self, comment, diff, status, comment_history, pr_title, pr_description):
         if comment.startswith('/'):
             command = comment.split(' ')[0]
             if command == '/help':
-                return self.return_response('\n'.join([f"{k}: {v}" for k, v in self.help_commands.items()]))
+                return self.return_response('\n'.join([f"`{k}`: {v}" for k, v in self.help_commands.items()]))
             elif command == '/explain':
                 return self.explain_code(diff)
             elif command == '/status':
                 return self.give_status(status)
             elif command == '/ask':
                 return self.ask(comment, diff, status, comment_history, pr_title, pr_description)    
             else:
```

### Comparing `mergemate-0.1.0/mergemate.egg-info/PKG-INFO` & `mergemate-0.1.1/mergemate.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 Metadata-Version: 2.1
 Name: mergemate
-Version: 0.1.0
+Version: 0.1.1
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
 
+
 # MergeMate: Automated PR Review and Command Handling
 
-MergeMate is an advanced GitHub action designed to automate pull request reviews and handle command-based interactions within GitHub issues. It integrates state-of-the-art AI from OpenAI to provide insightful, context-aware responses to code reviews and comments directly within your GitHub workflow.
+MergeMate is a sophisticated tool crafted to automate pull request reviews and manage command-based interactions within GitHub issues. It harnesses LLMWare, a comprehensive development framework featuring tools and finely-tuned, to deliver insightful, context-aware responses directly within your git workflow.
 
 ## Features
 
-- **Automated PR Reviews**: Automatically generate detailed reviews for pull requests, including code suggestions and best practices.
-- **Command Handling**: Respond to commands in PR comments such as `/help`, `/explain`, `/status`, and `/ask` to facilitate more dynamic and interactive PR discussions.
-- **Markdown Support**: Enhances readability and user interaction by formatting responses in Markdown with customized headers and footers.
-- **Easy Integration**: Designed to work seamlessly as a GitHub action, allowing for straightforward integration into any project's CI/CD pipeline.
+- **Advanced Integration with LLMWare**: Leverages LLMWare to analyze code and manage interactions, utilizing the latest AI technologies for natural language understanding and decision-making.
+- **Automated PR Reviews**: Generates thorough reviews for pull requests automatically, including specific code suggestions and adherence to best practices.
+- **Command Handling**: Interprets and responds to commands in PR comments such as `/help`, `/explain`, `/status`, and `/ask`, enriching the interaction within PR discussions.
+- **Markdown Support**: Improves readability and interaction by utilizing Markdown for formatting responses, complete with custom headers and footers.
+- **Easy Integration**: Seamlessly integrates as a GitHub action, facilitating straightforward incorporation into any project's CI/CD pipeline.
+- **Future Expansion Plans**: Aimed at extending support to other repository management platforms like GitLab and Bitbucket, broadening the accessibility and utility of MergeMate across different development environments.
 
 ## Installation
 
-MergeMate can be easily installed via pip:
+Install MergeMate quickly and easily via pip at [mergemate](https://pypi.org/project/mergemate/):
 
 ```bash
 pip install mergemate
 ```
 
-This single command prepares your environment to leverage MergeMate's capabilities, streamlining your project's interaction paradigms.
+Deploying MergeMate prepares your environment to leverage advanced AI capabilities, streamlining project interactions and reviews.
 
 ## GitHub Action Setup
 
-MergeMate can be integrated into your GitHub workflows with the following configuration:
+Incorporate MergeMate into your GitHub workflows using this configuration:
 
 ### Workflow Definition
 
 ```yaml
 name: Automated PR Review and Command Handling
 
 on:
@@ -84,24 +87,22 @@
       - name: Handle Comment
         run: python -m mergemate.scripts.github.comment_handler
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
 ```
 
-This workflow automates PR reviews and handles specific commands in comments on pull requests. The configuration is optimized for GitHub actions, ensuring that the operations are only triggered under appropriate conditions to maintain efficiency and resource utilization.
-
 ## Documentation
 
-Comprehensive documentation is available within the package, detailing setup instructions, configuration options, and command details. This ensures that all potential users, from novices to seasoned developers, can effectively utilize and customize MergeMate according to their specific needs.
+Extensive documentation is included within the package, providing detailed setup instructions, configuration options, and command usage. This ensures that users ranging from beginners to experienced developers can effectively utilize and customize MergeMate.
 
-## Contribution
+## Contributing
 
-Contributions to MergeMate are welcomed. If you're interested in enhancing its capabilities or tailoring it to fit new use cases, please fork the repository and submit your pull requests. MergeMate is a living project, and contributions help it stay at the cutting edge of technology and usability.
+We warmly welcome contributions to MergeMate. If you are interested in enhancing its functionality or adapting it for additional use cases, please fork the repository and submit your pull requests. As an open-source project, MergeMate thrives on community involvement and contributions, which are crucial for its continuous evolution and enhancement.
 
 ## Licensing
 
-MergeMate is released under the MIT license, which provides great flexibility for both personal and commercial use, encouraging a broad adoption and diverse contributions from the community.
+MergeMate is proudly released under the MIT license. This permissive licensing fosters widespread adoption and significant contributions from the community, supporting both personal and commercial use.
 
 ---
 
-MergeMate represents a leap forward in automating interactions within GitHub's ecosystem, reflecting the ongoing evolution in development practices facilitated by advances in AI technology. As we continue to enhance its capabilities, your feedback and contributions are invaluable in shaping its future trajectory.
+MergeMate epitomizes the next step in automating interactions within GitHub's ecosystem, propelled by the ongoing advancement of AI-driven development tools. Your feedback and contributions are invaluable to us as we aim to continually expand and enhance MergeMate's capabilities, catering to a growing range of development environments and communities.
```

### Comparing `mergemate-0.1.0/providers/github.py` & `mergemate-0.1.1/providers/github.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.0/scripts/github/comment_handler.py` & `mergemate-0.1.1/scripts/github/comment_handler.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.0/scripts/github/pr_review.py` & `mergemate-0.1.1/scripts/github/pr_review.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.0/setup.py` & `mergemate-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mergemate',
-    version='0.1.0',
+    version='0.1.1',
     author='Hardeep Singh',
     author_email='hardeep0khalsa122@gmail.com',
     packages=find_packages(),
     scripts=['scripts/github/comment_handler.py'],
     url='http://pypi.python.org/pypi/MergeMate/',
     license='LICENSE.txt',
     description='An automated tool to handle GitHub pull requests and comments.',
```

