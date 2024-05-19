# Comparing `tmp/gpt-pr-0.2.1.tar.gz` & `tmp/gpt-pr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/gpt-pr/gpt-pr/dist/.tmp-0849scsd/gpt-pr-0.2.1.tar", last modified: Fri Mar 15 21:44:35 2024, max compression
+gzip compressed data, was "/home/runner/work/gpt-pr/gpt-pr/dist/.tmp-ldna0n0d/gpt-pr-0.3.0.tar", last modified: Sun May 19 01:58:31 2024, max compression
```

## Comparing `gpt-pr-0.2.1.tar` & `gpt-pr-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-15 21:43:56.000000 gpt-pr-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-15 21:43:56.000000 gpt-pr-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/gpt_pr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/gpt_pr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/gpt_pr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/gpt_pr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/gpt_pr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/gpt_pr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/gpt_pr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/gpt_pr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/gptpr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 21:43:56.000000 gpt-pr-0.2.1/gptpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-15 21:43:56.000000 gpt-pr-0.2.1/gptpr/consolecolor.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-15 21:43:56.000000 gpt-pr-0.2.1/gptpr/gh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-03-15 21:43:56.000000 gpt-pr-0.2.1/gptpr/gitutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-15 21:43:56.000000 gpt-pr-0.2.1/gptpr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-03-15 21:43:56.000000 gpt-pr-0.2.1/gptpr/prdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-15 21:43:56.000000 gpt-pr-0.2.1/gptpr/test_prdata.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/gptpr/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-15 21:44:33.000000 gpt-pr-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-15 21:44:35.000000 gpt-pr-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-15 21:43:56.000000 gpt-pr-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 01:58:30.000000 gpt-pr-0.3.0/gpt_pr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gptpr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/consolecolor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/gh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/gitutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/prdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/test_prdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gptpr/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-19 01:58:29.000000 gpt-pr-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/setup.py
```

### Comparing `gpt-pr-0.2.1/README.md` & `gpt-pr-0.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 [![asciicast](https://asciinema.org/a/u0PwZlNjAGZcdXPPrjf84wj2A.svg)](https://asciinema.org/a/u0PwZlNjAGZcdXPPrjf84wj2A)
 
 ## Table of Contents
 
 - [Features](#features)
 - [Prerequisites](#prerequisites)
-- [Installation and Usage](#installation-and-usage)
-- [Authentication & API Keys](#authentication--api-keys)
+- [Installation](#installation)
+- [Configuration](#configuration)
+- [Usage](#usage)
 - [How to Contribute](#how-to-contribute)
 - [Roadmap](#roadmap)
 
 ## Features
 
 - Analyzes the diff changes of the current branch against the `main` branch.
 - Provides an option to exclude certain file changes from PR generation (for instance, you can ignore a `package.lock` file with 5k lines changed).
@@ -36,15 +37,15 @@
 
 ```bash
 pip install -U gpt-pr
 ```
 
 > Note: Use this command to **update** gpt-pr package to the latest version.
 
-2. Export API keys as environment variables ([Authentication & API Keys](#authentication--api-keys)).
+2. Setup API keys for GitHub and OpenAI, take a look at [Configuration](#configuration).
 
 3. Inside the Git repository you are working on, ensure you have pushed your branch to origin, then run:
 
 ```bash
 gpt-pr --help
 ```
 
@@ -59,78 +60,126 @@
 2. Navigate to the project directory and install dependencies:
 
 ```bash
 cd gpt-pr
 pipenv install
 ```
 
-After exporting api keys as environment variables ([Authentication & API Keys](#authentication--api-keys)), you can use GPT-PR within any git project directory. Suppose you've cloned **this project** to `~/workplace/gpt-pr`, here's how you can use it:
+After setting up API keys ([Configuration](#configuration)), you can use GPT-PR within any git project directory. Suppose you've cloned **this project** to `~/workplace/gpt-pr`, here's how you can use it:
 
 ```bash
 PYTHONPATH=~/workplace/gpt-pr/gpt-pr \
 PIPENV_PIPFILE=~/workplace/gpt-pr/Pipfile \
 pipenv run python ~/workplace/gpt-pr/gptpr/main.py --help
 ```
 
-## Usage
-
-### Generating Github Pull Requests
-
-To create a Pull request from your current branch commits to merge with `main` branch, just run:
-
-```
-gpt-pr
-```
-
-If you would like to compare with other base branch that is not `main`, just use `-b` param:
-
-```
-gpt-pr -b my-other-branch
-```
-
-### Usage help
-
-To show help commands:
-
-```
-gpt-pr -h
-```
-
-## Authentication & API Keys
+## Configuration
 
 ### Setting up GitHub Token (`GH_TOKEN`)
 
+GPT-PR tool will look for a `GH_TOKEN` in current shell env var OR in gpt-pr config file (at `~/.gpt-pr.ini`).
+
 To authenticate with GitHub, generate and export a GitHub Personal Access Token:
 
 1. Navigate to [GitHub's Personal Access Token page](https://github.com/settings/tokens).
 2. Click "Generate new token."
 3. Provide a description and select the required permissions `repo` for the token.
 4. Click "Generate token" at the bottom of the page.
 5. Copy the generated token.
-6. Export it as an environment variable:
+6. Set `gh_token` config running (supposing your gh token is `ghp_4Mb1QEr9gY5e8Lk3tN1KjPzX7W9z2V4HtJ2b`):
+
+```bash
+gpt-pr-config set gh_token ghp_4Mb1QEr9gY5e8Lk3tN1KjPzX7W9z2V4HtJ2b
+```
+
+Or just export it as an environment variable in your shell initializer:
 
 ```bash
 export GH_TOKEN=your_generated_token_here
 ```
 
 ### Setting up OpenAI API Key (`OPENAI_API_KEY`)
 
+GPT-PR tool will look for a `OPENAI_API_KEY` env var in current shell OR in gpt-pr config file (at `~/.gpt-pr.ini`).
+
 This project needs to interact with the ChatGPT API to generate the pull request description. So, you need to generate and export an OpenAI API Key:
 
 1. Navigate to [OpenAI's API Key page](https://platform.openai.com/signup).
 2. If you don't have an account, sign up and log in.
 3. Go to the API Keys section and click "Create new key."
 4. Provide a description and click "Create."
 5. Copy the generated API key.
-6. Export it as an environment variable:
+6. Set `openai_api_key` config running (supposing your openai_api_key is `QEr9gY5e8Lk3tN1KjPzX7W9z2V4Ht`):
+
+```bash
+gpt-pr-config set openai_api_key QEr9gY5e8Lk3tN1KjPzX7W9z2V4Ht
+```
+
+Or just export it as an environment variable in your shell initializer:
 
 ```bash
 export OPENAI_API_KEY=your_generated_api_key_here
 ```
 
+### Change OpenAI model
+
+To change OpenAI model, just run:
+
+```bash
+gpt-pr-config set openai_model gpt-3.5-turbo
+```
+
+To see a full list of available models, access [OpenAI Models Documentation](https://platform.openai.com/docs/models)
+
+### See all configs available
+
+To print all default configs and what is being used, just run:
+
+```bash
+gpt-pr-config print
+```
+
+### Reset config
+
+To reset any config to default value, just run:
+
+```bash
+gpt-pr-config reset config-name
+```
+
+Example:
+
+```bash
+gpt-pr-config reset openai_model
+```
+
+## Usage
+
+### Generating Github Pull Requests
+
+To create a Pull request from your current branch commits to merge with `main` branch, just run:
+
+```
+gpt-pr
+```
+
+If you would like to compare with other base branch that is not `main`, just use `-b` param:
+
+```
+gpt-pr -b my-other-branch
+```
+
+### Usage help
+
+To show help commands:
+
+```
+gpt-pr -h
+```
+
 Output:
 ![image](https://github.com/alissonperez/gpt-pr/assets/756802/cc6c0ca4-5759-44ce-ad35-e4e7305b3875)
 
 ## How to contribute?
 
 Please follow our [CONTRIBUTING](./CONTRIBUTING.md) guide.
```

### Comparing `gpt-pr-0.2.1/gpt_pr.egg-info/requires.txt` & `gpt-pr-0.3.0/gpt_pr.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 cffi==1.15.1
-cryptography==42.0.5
+cryptography==42.0.7
 fire==0.6.0
 pycparser==2.21
 wcwidth==0.2.13
 
 [:python_full_version >= "3.7.0"]
 charset-normalizer==3.3.2
 prompt-toolkit==3.0.43
 
 [:python_full_version >= "3.7.1"]
 openai==1.14.0
 
 [:python_version < "3.11"]
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
 
 [:python_version < "3.8"]
 cached-property==1.5.2
-typing-extensions==4.7.1
 
 [:python_version == "3.7"]
 importlib-metadata==6.7.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2"]
 six==1.16.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
 deprecated==1.2.14
 
 [:python_version >= "3.5"]
-idna==3.6
+idna==3.7
 
 [:python_version >= "3.6"]
 certifi==2024.2.2
 distro==1.9.0
 pynacl==1.5.0
 wrapt==1.16.0
 
@@ -48,14 +47,15 @@
 pydantic-core==2.14.6
 pygithub==2.2.0
 pyjwt[crypto]==2.8.0
 requests==2.31.0
 smmap==5.0.1
 sniffio==1.3.1
 termcolor==2.3.0
-tqdm==4.66.2
+tqdm==4.66.4
+typing-extensions==4.7.1
 urllib3==2.0.7
 zipp==3.15.0
 
 [:python_version >= "3.7" and python_version < "4.0"]
 inquirerpy==0.3.4
 pfzy==0.3.4
```

### Comparing `gpt-pr-0.2.1/gptpr/consolecolor.py` & `gpt-pr-0.3.0/gptpr/consolecolor.py`

 * *Files identical despite different names*

### Comparing `gpt-pr-0.2.1/gptpr/gh.py` & `gpt-pr-0.3.0/gptpr/gh.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 import os
 from github import Github
 from InquirerPy import inquirer
+from gptpr.config import config, config_command_example, CONFIG_README_SECTION
 
-GH_TOKEN = os.environ.get('GH_TOKEN')
 
-if not GH_TOKEN:
-    print("Please set GH_TOKEN environment variable")
-    exit(1)
+def _get_gh_token():
+    gh_token = config.get_user_config('GH_TOKEN')
+    if not gh_token:
+        gh_token = os.environ.get('GH_TOKEN')
 
-gh = Github(GH_TOKEN)
+    if not gh_token:
+        print('Please set "gh_token" config. Just run:',
+              config_command_example('gh_token', '[my gh token]'),
+              'more about at', CONFIG_README_SECTION)
+        exit(1)
+
+    return gh_token
+
+
+gh = Github(_get_gh_token())
 
 
 def create_pr(pr_data, yield_confirmation):
     repo = gh.get_repo(
         f'{pr_data.branch_info.owner}/{pr_data.branch_info.repo}')
 
     pr_confirmation = yield_confirmation or inquirer.confirm(
```

### Comparing `gpt-pr-0.2.1/gptpr/gitutil.py` & `gpt-pr-0.3.0/gptpr/gitutil.py`

 * *Files identical despite different names*

### Comparing `gpt-pr-0.2.1/gptpr/prdata.py` & `gpt-pr-0.3.0/gptpr/prdata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 import json
 import os
 from openai import OpenAI
 
 from gptpr.gitutil import BranchInfo
+from gptpr.config import config
 import gptpr.consolecolor as cc
 
 TOKENIZER_RATIO = 4
 MAX_TOKENS = 6000
 
 DEFAULT_PR_TEMPLATE = ('### Ref. [Link]\n\n## What was done?\n[Fill here]\n\n'
                        '## How was it done?\n[Fill here]\n\n'
@@ -33,14 +34,28 @@
                 print('Empty PR template at:', pr_template_file_path, 'using default template.')
     except Exception:
         print('PR template not found in .github dir. Using default template.')
 
     return pr_template
 
 
+def _get_open_ai_key():
+    api_key = config.get_user_config('OPENAI_API_KEY')
+
+    if not api_key:
+        api_key = os.environ.get('OPENAI_API_KEY')
+
+    if not api_key:
+        print('Please set "openai_api_key" config, just run:',
+              cc.yellow('gpt-pr-config set openai_api_key [open ai key]'))
+        exit(1)
+
+    return api_key
+
+
 @dataclass
 class PrData():
     branch_info: BranchInfo
     title: str
     body: str
 
     def to_display(self):
@@ -104,25 +119,22 @@
 
     total_length_with_diff = current_total_length + len(branch_info.diff)
     if total_length_with_diff / TOKENIZER_RATIO > MAX_TOKENS:
         print('Total content length (with diff) is too big.', cc.red('Skipping diff content...'))
     else:
         messages.append({'role': 'user', 'content': 'Diff changes:\n' + branch_info.diff})
 
-    openai_api_key = os.environ.get('OPENAI_API_KEY')
-
-    if not openai_api_key:
-        print("Please set OPENAI_API_KEY environment variable.")
-        exit(1)
+    client = OpenAI(api_key=_get_open_ai_key())
 
-    client = OpenAI(api_key=openai_api_key)
+    openai_model = config.get_user_config('OPENAI_MODEL')
+    print('Using OpenAI model:', cc.yellow(openai_model))
 
     chat_completion = client.chat.completions.create(
         messages=messages,
-        model='gpt-4-0613',
+        model=openai_model,
         functions=functions,
         function_call={'name': 'create_pr'},
         temperature=0,
         max_tokens=512,
         top_p=1,
         frequency_penalty=0,
         presence_penalty=0
```

### Comparing `gpt-pr-0.2.1/requirements.txt` & `gpt-pr-0.3.0/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 -i https://pypi.org/simple
 annotated-types==0.5.0; python_version >= '3.7'
 anyio==3.7.1; python_version >= '3.7'
 cached-property==1.5.2; python_version < '3.8'
 certifi==2024.2.2; python_version >= '3.6'
 cffi==1.15.1
 charset-normalizer==3.3.2; python_full_version >= '3.7.0'
-cryptography==42.0.5
+cryptography==42.0.7
 deprecated==1.2.14; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 distro==1.9.0; python_version >= '3.6'
-exceptiongroup==1.2.0; python_version < '3.11'
+exceptiongroup==1.2.1; python_version < '3.11'
 fire==0.6.0
 gitdb==4.0.11; python_version >= '3.7'
 gitpython==3.1.42; python_version >= '3.7'
 h11==0.14.0; python_version >= '3.7'
 httpcore==0.17.3; python_version >= '3.7'
 httpx==0.24.1; python_version >= '3.7'
-idna==3.6; python_version >= '3.5'
+idna==3.7; python_version >= '3.5'
 importlib-metadata==6.7.0; python_version == '3.7'
 inquirerpy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 openai==1.14.0; python_full_version >= '3.7.1'
 pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 prompt-toolkit==3.0.43; python_full_version >= '3.7.0'
 pycparser==2.21
 pydantic==2.5.3; python_version >= '3.7'
@@ -28,13 +28,13 @@
 pyjwt[crypto]==2.8.0; python_version >= '3.7'
 pynacl==1.5.0; python_version >= '3.6'
 requests==2.31.0; python_version >= '3.7'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'
 smmap==5.0.1; python_version >= '3.7'
 sniffio==1.3.1; python_version >= '3.7'
 termcolor==2.3.0; python_version >= '3.7'
-tqdm==4.66.2; python_version >= '3.7'
-typing-extensions==4.7.1; python_version < '3.8'
+tqdm==4.66.4; python_version >= '3.7'
+typing-extensions==4.7.1; python_version >= '3.7'
 urllib3==2.0.7; python_version >= '3.7'
 wcwidth==0.2.13
 wrapt==1.16.0; python_version >= '3.6'
 zipp==3.15.0; python_version >= '3.7'
```

### Comparing `gpt-pr-0.2.1/setup.py` & `gpt-pr-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,13 +35,16 @@
       description=('Automate your GitHub workflow with GPT-PR: '
                    'an OpenAI powered library for streamlined PR generation.'),
       url='http://github.com/alissonperez/gpt-pr',
       author='Alisson R. Perez',
       author_email='alissonperez@outlook.com',
       license='MIT',
       entry_points={
-          'console_scripts': ['gpt-pr=gptpr.main:main'],
+          'console_scripts': [
+              'gpt-pr=gptpr.main:main',
+              'gpt-pr-config=gptpr.main:run_config',
+          ],
       },
       packages=find_packages('.'),
       include_package_data=True,
       install_requires=get_requirements(),
       zip_safe=False)
```

