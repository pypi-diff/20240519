# Comparing `tmp/gaiah_toolkit-0.3.13.tar.gz` & `tmp/gaiah_toolkit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaiah_toolkit-0.3.13.tar", last modified: Mon May 13 13:56:22 2024, max compression
+gzip compressed data, was "gaiah_toolkit-0.4.0.tar", last modified: Sun May 19 08:03:54 2024, max compression
```

## Comparing `gaiah_toolkit-0.3.13.tar` & `gaiah_toolkit-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:22.978658 gaiah_toolkit-0.3.13/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-05-13 13:56:22.978658 gaiah_toolkit-0.3.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:22.974658 gaiah_toolkit-0.3.13/gaiah/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/gaiah/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/gaiah/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7294 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/gaiah/gaiah.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:22.974658 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:56:22.978658 gaiah_toolkit-0.3.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:22.974658 gaiah_toolkit-0.3.13/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:03:54.038873 gaiah_toolkit-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-19 08:03:54.038873 gaiah_toolkit-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:03:54.034873 gaiah_toolkit-0.4.0/gaiah/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/gaiah.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/gaiah_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/gaiah_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/gaiah_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:03:54.034873 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:03:54.038873 gaiah_toolkit-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:03:54.034873 gaiah_toolkit-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/tests/test_main.py
```

### Comparing `gaiah_toolkit-0.3.13/LICENSE` & `gaiah_toolkit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaiah_toolkit-0.3.13/PKG-INFO` & `gaiah_toolkit-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiah_toolkit
-Version: 0.3.13
+Version: 0.4.0
 Home-page: https://github.com/your_username/gaiah
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gitpython
@@ -92,51 +92,60 @@
 
 特定のプロジェクトディレクトリでGaiahを使用する場合、以下のようにリポジトリの場所やコミットメッセージのファイルパスを指定できます:
 
 ```bash
 gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
 ```
 
-上記のコマンドでは、`--repo_dir`オプションでリポジトリのディレクトリを、`--commit_msg_path`オプションでコミットメッセージが記載されたMarkdownファイルのパスを指定しています。
+### リポジトリの初期化
 
-## 🤝 コミットメッセージの一括自動コミット
-
-Gaiahでは、LLMを用いて生成したコミットメッセージを一括自動コミットすることができます。以下の手順でコミットメッセージを生成し、コミットを行います:
-
-1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md)というフォーマットで、ステージング情報をLLMに渡します。
-
-2. LLMは以下のような形式でコミットメッセージを生成します:
-
-   ```
-   Commit Messages フォーマット
-
-   ## Commit 1
+```bash
+gaiah --create_repo --repo_name Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
+```
 
-   ### README.md
+## 処理フロー
 
-   ```commit-msg
-   📝 [docs] READMEに応用的な使い方セクションを追加
+```mermaid
 
-   - `README.md`ファイルに新たなセクションとして「応用的な使い方」を追加しました。これにより、ユーザーはGaiahを特定のプロジェクトディレクトリで使用する方法を具体的に学べるようになります。特に、リポジトリの指定やコミットメッセージのファイルパスを設定する具体的なコマンド例を示しています。  
-   ```
+graph TD
+   A[ユーザーがCLIを実行] --> B{コマンドライン引数を解析}
+   B --> C{Gaiahオブジェクトを作成}
+   C --> D{--create_repoオプションが指定されている?}
+   D -->|Yes| E[新しいリポジトリをGitHub上に作成]
+   E --> E1[.envファイルから環境変数を読み込む]
+   E1 --> E2[環境変数からアクセストークンを取得]
+   E2 --> E3[GitHubオブジェクトを作成]
+   E3 --> E4[リポジトリ名とパラメータを指定]
+   E4 --> E5[GitHub上に新しいリポジトリを作成]
+   E5 --> E6[リポジトリ作成完了のメッセージを表示]
+   E6 --> Q[処理完了]
+   D -->|No| F{--process_commitsオプションが指定されている?}
+   F -->|Yes| G[コミットメッセージファイルからコミットを処理]
+   G --> H[すべてのファイルをアンステージ]
+   H --> I{コミットセクションごとに処理}
+   I --> J{ファイル名とコミットメッセージを取得}
+   J --> K{ファイルを処理}
+   K --> L{ファイルをステージ}
+   L --> M{変更をコミット}
+   M --> N{次のコミットセクションがある?}
+   N -->|Yes| I
+   N -->|No| O[リモートリポジトリにプッシュ]
+   O --> P[処理完了]
+   F -->|No| Q[処理完了]
 
-   ## Commit 2
+```
 
-   ### gaiah/__init__.py
+## 開発用
 
-   ```commit-msg
-   🔖 [chore] Gaiahのバージョンを0.3.12に更新
+```bash
+gaiah --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits
+```
 
-   - `gaiah/__init__.py`でのバージョン番号を0.3.11から0.3.12へ更新しました。この更新は、最新の機能改善とバグ修正をユーザーに提供するためのものです。
-   ```
-   ```
 
-3. 生成されたコミットメッセージを`.Gaiah.md`ファイルに貼り付けます。このファイルは、初回に`gaiah`コマンドを実行した際に自動で生成されます。
 
-4. 再度`gaiah`コマンドを実行すると、`.Gaiah.md`ファイルからコミットメッセージが読み込まれ、自動的にコミットとプッシュが行われます。
 
 ## 🤝 貢献
 
 Gaiahをさらに良くするために、コミュニティからの貢献を歓迎します。アイデア、提案、バグ報告がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/Gaiah)で issue を開くか、プルリクエストを送信してください。
 
 ## 📄 ライセンス
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.3.13 Home-page: https://
+Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.4.0 Home-page: https://
 github.com/your_username/gaiah Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Version Control Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: gitpython Requires-Dist: python-dotenv Requires-
 Dist: PyGithub Requires-Dist: termcolor Requires-Dist: art
        [https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/
                                Gaiah_icon1.png]
@@ -46,35 +46,39 @@
 ``` 2. condaç°å¢ãã¢ã¯ãã£ãã¼ããã¾ã: ``` conda activate gaiah
 ``` 3. å¿è¦ãªä¾å­é¢ä¿ãã¤ã³ã¹ãã¼ã«ãã¾ã: ``` pip install
 gitpython python-dotenv PyGithub termcolor art ``` ## ð ä½¿ç¨æ¹æ³ ### CLI
 Gaiahã®CLIæ©è½ã«ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
 ```bash gaiah ``` ### å¿ç¨çãªä½¿ãæ¹
 ç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§Gaiahãä½¿ç¨ããå ´åãä»¥ä¸ã®ããã«ãªãã¸ããªã®å ´æãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãæå®ã§ãã¾ã:
 ```bash gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-``` ä¸è¨ã®ã³ãã³ãã§ã¯ã`--
-repo_dir`ãªãã·ã§ã³ã§ãªãã¸ããªã®ãã£ã¬ã¯ããªãã`--
-commit_msg_path`ãªãã·ã§ã³ã§ã³ãããã¡ãã»ã¼ã¸ãè¨è¼ãããMarkdownãã¡ã¤ã«ã®ãã¹ãæå®ãã¦ãã¾ãã
-## ð¤ ã³ãããã¡ãã»ã¼ã¸ã®ä¸æ¬èªåã³ããã
-Gaiahã§ã¯ãLLMãç¨ãã¦çæããã³ãããã¡ãã»ã¼ã¸ãä¸æ¬èªåã³ããããããã¨ãã§ãã¾ããä»¥ä¸ã®æé ã§ã³ãããã¡ãã»ã¼ã¸ãçæããã³ããããè¡ãã¾ã:
-1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://
-github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/
-STAGE_INFO_TEMPLATE_GAIAH.md)ã¨ãããã©ã¼ãããã§ãã¹ãã¼ã¸ã³ã°æå ±ãLLMã«æ¸¡ãã¾ãã
-2.
-LLMã¯ä»¥ä¸ã®ãããªå½¢å¼ã§ã³ãããã¡ãã»ã¼ã¸ãçæãã¾ã:
-``` Commit Messages ãã©ã¼ããã ## Commit 1 ### README.md ```commit-msg
-ð [docs] READMEã«å¿ç¨çãªä½¿ãæ¹ã»ã¯ã·ã§ã³ãè¿½å  -
-`README.md`ãã¡ã¤ã«ã«æ°ããªã»ã¯ã·ã§ã³ã¨ãã¦ãå¿ç¨çãªä½¿ãæ¹ããè¿½å ãã¾ãããããã«ãããã¦ã¼ã¶ã¼ã¯Gaiahãç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§ä½¿ç¨ããæ¹æ³ãå·ä½çã«å­¦ã¹ãããã«ãªãã¾ããç¹ã«ããªãã¸ããªã®æå®ãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãè¨­å®ããå·ä½çãªã³ãã³ãä¾ãç¤ºãã¦ãã¾ãã
-``` ## Commit 2 ### gaiah/__init__.py ```commit-msg ð [chore]
-Gaiahã®ãã¼ã¸ã§ã³ã0.3.12ã«æ´æ° - `gaiah/
-__init__.py`ã§ã®ãã¼ã¸ã§ã³çªå·ã0.3.11ãã0.3.12ã¸æ´æ°ãã¾ããããã®æ´æ°ã¯ãææ°ã®æ©è½æ¹åã¨ãã°ä¿®æ­£ãã¦ã¼ã¶ã¼ã«æä¾ããããã®ãã®ã§ãã
-``` ``` 3.
-çæãããã³ãããã¡ãã»ã¼ã¸ã`.Gaiah.md`ãã¡ã¤ã«ã«è²¼ãä»ãã¾ãããã®ãã¡ã¤ã«ã¯ãååã«`gaiah`ã³ãã³ããå®è¡ããéã«èªåã§çæããã¾ãã
-4.
-ååº¦`gaiah`ã³ãã³ããå®è¡ããã¨ã`.Gaiah.md`ãã¡ã¤ã«ããã³ãããã¡ãã»ã¼ã¸ãèª­ã¿è¾¼ã¾ããèªåçã«ã³ãããã¨ããã·ã¥ãè¡ããã¾ãã
-## ð¤ è²¢ç®
+``` ### ãªãã¸ããªã®åæå ```bash gaiah --create_repo --repo_name
+Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:
+\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
+``` ## å¦çãã­ã¼ ```mermaid graph TD A[ã¦ã¼ã¶ã¼ãCLIãå®è¡] --> B
+{ã³ãã³ãã©ã¤ã³å¼æ°ãè§£æ} B --> C
+{Gaiahãªãã¸ã§ã¯ããä½æ} C --> D{--
+create_repoãªãã·ã§ã³ãæå®ããã¦ãã?} D -->|Yes| E
+[æ°ãããªãã¸ããªãGitHubä¸ã«ä½æ] E --> E1
+[.envãã¡ã¤ã«ããç°å¢å¤æ°ãèª­ã¿è¾¼ã] E1 --> E2
+[ç°å¢å¤æ°ããã¢ã¯ã»ã¹ãã¼ã¯ã³ãåå¾] E2 --> E3
+[GitHubãªãã¸ã§ã¯ããä½æ] E3 --> E4
+[ãªãã¸ããªåã¨ãã©ã¡ã¼ã¿ãæå®] E4 --> E5
+[GitHubä¸ã«æ°ãããªãã¸ããªãä½æ] E5 --> E6
+[ãªãã¸ããªä½æå®äºã®ã¡ãã»ã¼ã¸ãè¡¨ç¤º] E6 --> Q[å¦çå®äº]
+D -->|No| F{--process_commitsãªãã·ã§ã³ãæå®ããã¦ãã?} F --
+>|Yes| G[ã³ãããã¡ãã»ã¼ã¸ãã¡ã¤ã«ããã³ããããå¦ç] G
+--> H[ãã¹ã¦ã®ãã¡ã¤ã«ãã¢ã³ã¹ãã¼ã¸] H --> I
+{ã³ãããã»ã¯ã·ã§ã³ãã¨ã«å¦ç} I --> J
+{ãã¡ã¤ã«åã¨ã³ãããã¡ãã»ã¼ã¸ãåå¾} J --> K
+{ãã¡ã¤ã«ãå¦ç} K --> L{ãã¡ã¤ã«ãã¹ãã¼ã¸} L --> M
+{å¤æ´ãã³ããã} M --> N{æ¬¡ã®ã³ãããã»ã¯ã·ã§ã³ããã?} N
+-->|Yes| I N -->|No| O[ãªã¢ã¼ããªãã¸ããªã«ããã·ã¥] O --> P
+[å¦çå®äº] F -->|No| Q[å¦çå®äº] ``` ## éçºç¨ ```bash gaiah --
+repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits ``` ## ð¤
+è²¢ç®
 Gaiahãããã«è¯ãããããã«ãã³ãã¥ããã£ããã®è²¢ç®ãæ­è¿ãã¾ããã¢ã¤ãã¢ãææ¡ããã°å ±åãããå ´åã¯ã
 [GitHubãªãã¸ããª](https://github.com/Sunwood-ai-labs/Gaiah)ã§ issue
 ãéããããã«ãªã¯ã¨ã¹ããéä¿¡ãã¦ãã ããã ## ð
 ã©ã¤ã»ã³ã¹ Gaiahã¯ã[MITã©ã¤ã»ã³ã¹](https://opensource.org/
 licenses/
 MIT)ã®ä¸ã§ãªãªã¼ã¹ããã¦ãããã©ã¤ãã©ãªã®èªç±ãã¤ãªã¼ãã³ã½ã¼ã¹ã§ã®ä½¿ç¨ãå¤æ´ãéå¸ãå¯è½ã§ãã
 ## ð è¬è¾
```

### Comparing `gaiah_toolkit-0.3.13/README.md` & `gaiah_toolkit-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -77,51 +77,60 @@
 
 特定のプロジェクトディレクトリでGaiahを使用する場合、以下のようにリポジトリの場所やコミットメッセージのファイルパスを指定できます:
 
 ```bash
 gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
 ```
 
-上記のコマンドでは、`--repo_dir`オプションでリポジトリのディレクトリを、`--commit_msg_path`オプションでコミットメッセージが記載されたMarkdownファイルのパスを指定しています。
+### リポジトリの初期化
 
-## 🤝 コミットメッセージの一括自動コミット
-
-Gaiahでは、LLMを用いて生成したコミットメッセージを一括自動コミットすることができます。以下の手順でコミットメッセージを生成し、コミットを行います:
-
-1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md)というフォーマットで、ステージング情報をLLMに渡します。
-
-2. LLMは以下のような形式でコミットメッセージを生成します:
-
-   ```
-   Commit Messages フォーマット
-
-   ## Commit 1
+```bash
+gaiah --create_repo --repo_name Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
+```
 
-   ### README.md
+## 処理フロー
 
-   ```commit-msg
-   📝 [docs] READMEに応用的な使い方セクションを追加
+```mermaid
 
-   - `README.md`ファイルに新たなセクションとして「応用的な使い方」を追加しました。これにより、ユーザーはGaiahを特定のプロジェクトディレクトリで使用する方法を具体的に学べるようになります。特に、リポジトリの指定やコミットメッセージのファイルパスを設定する具体的なコマンド例を示しています。  
-   ```
+graph TD
+   A[ユーザーがCLIを実行] --> B{コマンドライン引数を解析}
+   B --> C{Gaiahオブジェクトを作成}
+   C --> D{--create_repoオプションが指定されている?}
+   D -->|Yes| E[新しいリポジトリをGitHub上に作成]
+   E --> E1[.envファイルから環境変数を読み込む]
+   E1 --> E2[環境変数からアクセストークンを取得]
+   E2 --> E3[GitHubオブジェクトを作成]
+   E3 --> E4[リポジトリ名とパラメータを指定]
+   E4 --> E5[GitHub上に新しいリポジトリを作成]
+   E5 --> E6[リポジトリ作成完了のメッセージを表示]
+   E6 --> Q[処理完了]
+   D -->|No| F{--process_commitsオプションが指定されている?}
+   F -->|Yes| G[コミットメッセージファイルからコミットを処理]
+   G --> H[すべてのファイルをアンステージ]
+   H --> I{コミットセクションごとに処理}
+   I --> J{ファイル名とコミットメッセージを取得}
+   J --> K{ファイルを処理}
+   K --> L{ファイルをステージ}
+   L --> M{変更をコミット}
+   M --> N{次のコミットセクションがある?}
+   N -->|Yes| I
+   N -->|No| O[リモートリポジトリにプッシュ]
+   O --> P[処理完了]
+   F -->|No| Q[処理完了]
 
-   ## Commit 2
+```
 
-   ### gaiah/__init__.py
+## 開発用
 
-   ```commit-msg
-   🔖 [chore] Gaiahのバージョンを0.3.12に更新
+```bash
+gaiah --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits
+```
 
-   - `gaiah/__init__.py`でのバージョン番号を0.3.11から0.3.12へ更新しました。この更新は、最新の機能改善とバグ修正をユーザーに提供するためのものです。
-   ```
-   ```
 
-3. 生成されたコミットメッセージを`.Gaiah.md`ファイルに貼り付けます。このファイルは、初回に`gaiah`コマンドを実行した際に自動で生成されます。
 
-4. 再度`gaiah`コマンドを実行すると、`.Gaiah.md`ファイルからコミットメッセージが読み込まれ、自動的にコミットとプッシュが行われます。
 
 ## 🤝 貢献
 
 Gaiahをさらに良くするために、コミュニティからの貢献を歓迎します。アイデア、提案、バグ報告がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/Gaiah)で issue を開くか、プルリクエストを送信してください。
 
 ## 📄 ライセンス
```

#### html2text {}

```diff
@@ -40,35 +40,39 @@
 ``` 2. condaç°å¢ãã¢ã¯ãã£ãã¼ããã¾ã: ``` conda activate gaiah
 ``` 3. å¿è¦ãªä¾å­é¢ä¿ãã¤ã³ã¹ãã¼ã«ãã¾ã: ``` pip install
 gitpython python-dotenv PyGithub termcolor art ``` ## ð ä½¿ç¨æ¹æ³ ### CLI
 Gaiahã®CLIæ©è½ã«ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
 ```bash gaiah ``` ### å¿ç¨çãªä½¿ãæ¹
 ç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§Gaiahãä½¿ç¨ããå ´åãä»¥ä¸ã®ããã«ãªãã¸ããªã®å ´æãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãæå®ã§ãã¾ã:
 ```bash gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-``` ä¸è¨ã®ã³ãã³ãã§ã¯ã`--
-repo_dir`ãªãã·ã§ã³ã§ãªãã¸ããªã®ãã£ã¬ã¯ããªãã`--
-commit_msg_path`ãªãã·ã§ã³ã§ã³ãããã¡ãã»ã¼ã¸ãè¨è¼ãããMarkdownãã¡ã¤ã«ã®ãã¹ãæå®ãã¦ãã¾ãã
-## ð¤ ã³ãããã¡ãã»ã¼ã¸ã®ä¸æ¬èªåã³ããã
-Gaiahã§ã¯ãLLMãç¨ãã¦çæããã³ãããã¡ãã»ã¼ã¸ãä¸æ¬èªåã³ããããããã¨ãã§ãã¾ããä»¥ä¸ã®æé ã§ã³ãããã¡ãã»ã¼ã¸ãçæããã³ããããè¡ãã¾ã:
-1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://
-github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/
-STAGE_INFO_TEMPLATE_GAIAH.md)ã¨ãããã©ã¼ãããã§ãã¹ãã¼ã¸ã³ã°æå ±ãLLMã«æ¸¡ãã¾ãã
-2.
-LLMã¯ä»¥ä¸ã®ãããªå½¢å¼ã§ã³ãããã¡ãã»ã¼ã¸ãçæãã¾ã:
-``` Commit Messages ãã©ã¼ããã ## Commit 1 ### README.md ```commit-msg
-ð [docs] READMEã«å¿ç¨çãªä½¿ãæ¹ã»ã¯ã·ã§ã³ãè¿½å  -
-`README.md`ãã¡ã¤ã«ã«æ°ããªã»ã¯ã·ã§ã³ã¨ãã¦ãå¿ç¨çãªä½¿ãæ¹ããè¿½å ãã¾ãããããã«ãããã¦ã¼ã¶ã¼ã¯Gaiahãç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§ä½¿ç¨ããæ¹æ³ãå·ä½çã«å­¦ã¹ãããã«ãªãã¾ããç¹ã«ããªãã¸ããªã®æå®ãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãè¨­å®ããå·ä½çãªã³ãã³ãä¾ãç¤ºãã¦ãã¾ãã
-``` ## Commit 2 ### gaiah/__init__.py ```commit-msg ð [chore]
-Gaiahã®ãã¼ã¸ã§ã³ã0.3.12ã«æ´æ° - `gaiah/
-__init__.py`ã§ã®ãã¼ã¸ã§ã³çªå·ã0.3.11ãã0.3.12ã¸æ´æ°ãã¾ããããã®æ´æ°ã¯ãææ°ã®æ©è½æ¹åã¨ãã°ä¿®æ­£ãã¦ã¼ã¶ã¼ã«æä¾ããããã®ãã®ã§ãã
-``` ``` 3.
-çæãããã³ãããã¡ãã»ã¼ã¸ã`.Gaiah.md`ãã¡ã¤ã«ã«è²¼ãä»ãã¾ãããã®ãã¡ã¤ã«ã¯ãååã«`gaiah`ã³ãã³ããå®è¡ããéã«èªåã§çæããã¾ãã
-4.
-ååº¦`gaiah`ã³ãã³ããå®è¡ããã¨ã`.Gaiah.md`ãã¡ã¤ã«ããã³ãããã¡ãã»ã¼ã¸ãèª­ã¿è¾¼ã¾ããèªåçã«ã³ãããã¨ããã·ã¥ãè¡ããã¾ãã
-## ð¤ è²¢ç®
+``` ### ãªãã¸ããªã®åæå ```bash gaiah --create_repo --repo_name
+Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:
+\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
+``` ## å¦çãã­ã¼ ```mermaid graph TD A[ã¦ã¼ã¶ã¼ãCLIãå®è¡] --> B
+{ã³ãã³ãã©ã¤ã³å¼æ°ãè§£æ} B --> C
+{Gaiahãªãã¸ã§ã¯ããä½æ} C --> D{--
+create_repoãªãã·ã§ã³ãæå®ããã¦ãã?} D -->|Yes| E
+[æ°ãããªãã¸ããªãGitHubä¸ã«ä½æ] E --> E1
+[.envãã¡ã¤ã«ããç°å¢å¤æ°ãèª­ã¿è¾¼ã] E1 --> E2
+[ç°å¢å¤æ°ããã¢ã¯ã»ã¹ãã¼ã¯ã³ãåå¾] E2 --> E3
+[GitHubãªãã¸ã§ã¯ããä½æ] E3 --> E4
+[ãªãã¸ããªåã¨ãã©ã¡ã¼ã¿ãæå®] E4 --> E5
+[GitHubä¸ã«æ°ãããªãã¸ããªãä½æ] E5 --> E6
+[ãªãã¸ããªä½æå®äºã®ã¡ãã»ã¼ã¸ãè¡¨ç¤º] E6 --> Q[å¦çå®äº]
+D -->|No| F{--process_commitsãªãã·ã§ã³ãæå®ããã¦ãã?} F --
+>|Yes| G[ã³ãããã¡ãã»ã¼ã¸ãã¡ã¤ã«ããã³ããããå¦ç] G
+--> H[ãã¹ã¦ã®ãã¡ã¤ã«ãã¢ã³ã¹ãã¼ã¸] H --> I
+{ã³ãããã»ã¯ã·ã§ã³ãã¨ã«å¦ç} I --> J
+{ãã¡ã¤ã«åã¨ã³ãããã¡ãã»ã¼ã¸ãåå¾} J --> K
+{ãã¡ã¤ã«ãå¦ç} K --> L{ãã¡ã¤ã«ãã¹ãã¼ã¸} L --> M
+{å¤æ´ãã³ããã} M --> N{æ¬¡ã®ã³ãããã»ã¯ã·ã§ã³ããã?} N
+-->|Yes| I N -->|No| O[ãªã¢ã¼ããªãã¸ããªã«ããã·ã¥] O --> P
+[å¦çå®äº] F -->|No| Q[å¦çå®äº] ``` ## éçºç¨ ```bash gaiah --
+repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits ``` ## ð¤
+è²¢ç®
 Gaiahãããã«è¯ãããããã«ãã³ãã¥ããã£ããã®è²¢ç®ãæ­è¿ãã¾ããã¢ã¤ãã¢ãææ¡ããã°å ±åãããå ´åã¯ã
 [GitHubãªãã¸ããª](https://github.com/Sunwood-ai-labs/Gaiah)ã§ issue
 ãéããããã«ãªã¯ã¨ã¹ããéä¿¡ãã¦ãã ããã ## ð
 ã©ã¤ã»ã³ã¹ Gaiahã¯ã[MITã©ã¤ã»ã³ã¹](https://opensource.org/
 licenses/
 MIT)ã®ä¸ã§ãªãªã¼ã¹ããã¦ãããã©ã¤ãã©ãªã®èªç±ãã¤ãªã¼ãã³ã½ã¼ã¹ã§ã®ä½¿ç¨ãå¤æ´ãéå¸ãå¯è½ã§ãã
 ## ð è¬è¾
```

### Comparing `gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/PKG-INFO` & `gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiah_toolkit
-Version: 0.3.13
+Version: 0.4.0
 Home-page: https://github.com/your_username/gaiah
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gitpython
@@ -92,51 +92,60 @@
 
 特定のプロジェクトディレクトリでGaiahを使用する場合、以下のようにリポジトリの場所やコミットメッセージのファイルパスを指定できます:
 
 ```bash
 gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
 ```
 
-上記のコマンドでは、`--repo_dir`オプションでリポジトリのディレクトリを、`--commit_msg_path`オプションでコミットメッセージが記載されたMarkdownファイルのパスを指定しています。
+### リポジトリの初期化
 
-## 🤝 コミットメッセージの一括自動コミット
-
-Gaiahでは、LLMを用いて生成したコミットメッセージを一括自動コミットすることができます。以下の手順でコミットメッセージを生成し、コミットを行います:
-
-1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md)というフォーマットで、ステージング情報をLLMに渡します。
-
-2. LLMは以下のような形式でコミットメッセージを生成します:
-
-   ```
-   Commit Messages フォーマット
-
-   ## Commit 1
+```bash
+gaiah --create_repo --repo_name Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
+```
 
-   ### README.md
+## 処理フロー
 
-   ```commit-msg
-   📝 [docs] READMEに応用的な使い方セクションを追加
+```mermaid
 
-   - `README.md`ファイルに新たなセクションとして「応用的な使い方」を追加しました。これにより、ユーザーはGaiahを特定のプロジェクトディレクトリで使用する方法を具体的に学べるようになります。特に、リポジトリの指定やコミットメッセージのファイルパスを設定する具体的なコマンド例を示しています。  
-   ```
+graph TD
+   A[ユーザーがCLIを実行] --> B{コマンドライン引数を解析}
+   B --> C{Gaiahオブジェクトを作成}
+   C --> D{--create_repoオプションが指定されている?}
+   D -->|Yes| E[新しいリポジトリをGitHub上に作成]
+   E --> E1[.envファイルから環境変数を読み込む]
+   E1 --> E2[環境変数からアクセストークンを取得]
+   E2 --> E3[GitHubオブジェクトを作成]
+   E3 --> E4[リポジトリ名とパラメータを指定]
+   E4 --> E5[GitHub上に新しいリポジトリを作成]
+   E5 --> E6[リポジトリ作成完了のメッセージを表示]
+   E6 --> Q[処理完了]
+   D -->|No| F{--process_commitsオプションが指定されている?}
+   F -->|Yes| G[コミットメッセージファイルからコミットを処理]
+   G --> H[すべてのファイルをアンステージ]
+   H --> I{コミットセクションごとに処理}
+   I --> J{ファイル名とコミットメッセージを取得}
+   J --> K{ファイルを処理}
+   K --> L{ファイルをステージ}
+   L --> M{変更をコミット}
+   M --> N{次のコミットセクションがある?}
+   N -->|Yes| I
+   N -->|No| O[リモートリポジトリにプッシュ]
+   O --> P[処理完了]
+   F -->|No| Q[処理完了]
 
-   ## Commit 2
+```
 
-   ### gaiah/__init__.py
+## 開発用
 
-   ```commit-msg
-   🔖 [chore] Gaiahのバージョンを0.3.12に更新
+```bash
+gaiah --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits
+```
 
-   - `gaiah/__init__.py`でのバージョン番号を0.3.11から0.3.12へ更新しました。この更新は、最新の機能改善とバグ修正をユーザーに提供するためのものです。
-   ```
-   ```
 
-3. 生成されたコミットメッセージを`.Gaiah.md`ファイルに貼り付けます。このファイルは、初回に`gaiah`コマンドを実行した際に自動で生成されます。
 
-4. 再度`gaiah`コマンドを実行すると、`.Gaiah.md`ファイルからコミットメッセージが読み込まれ、自動的にコミットとプッシュが行われます。
 
 ## 🤝 貢献
 
 Gaiahをさらに良くするために、コミュニティからの貢献を歓迎します。アイデア、提案、バグ報告がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/Gaiah)で issue を開くか、プルリクエストを送信してください。
 
 ## 📄 ライセンス
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.3.13 Home-page: https://
+Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.4.0 Home-page: https://
 github.com/your_username/gaiah Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Version Control Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: gitpython Requires-Dist: python-dotenv Requires-
 Dist: PyGithub Requires-Dist: termcolor Requires-Dist: art
        [https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/
                                Gaiah_icon1.png]
@@ -46,35 +46,39 @@
 ``` 2. condaç°å¢ãã¢ã¯ãã£ãã¼ããã¾ã: ``` conda activate gaiah
 ``` 3. å¿è¦ãªä¾å­é¢ä¿ãã¤ã³ã¹ãã¼ã«ãã¾ã: ``` pip install
 gitpython python-dotenv PyGithub termcolor art ``` ## ð ä½¿ç¨æ¹æ³ ### CLI
 Gaiahã®CLIæ©è½ã«ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
 ```bash gaiah ``` ### å¿ç¨çãªä½¿ãæ¹
 ç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§Gaiahãä½¿ç¨ããå ´åãä»¥ä¸ã®ããã«ãªãã¸ããªã®å ´æãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãæå®ã§ãã¾ã:
 ```bash gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-``` ä¸è¨ã®ã³ãã³ãã§ã¯ã`--
-repo_dir`ãªãã·ã§ã³ã§ãªãã¸ããªã®ãã£ã¬ã¯ããªãã`--
-commit_msg_path`ãªãã·ã§ã³ã§ã³ãããã¡ãã»ã¼ã¸ãè¨è¼ãããMarkdownãã¡ã¤ã«ã®ãã¹ãæå®ãã¦ãã¾ãã
-## ð¤ ã³ãããã¡ãã»ã¼ã¸ã®ä¸æ¬èªåã³ããã
-Gaiahã§ã¯ãLLMãç¨ãã¦çæããã³ãããã¡ãã»ã¼ã¸ãä¸æ¬èªåã³ããããããã¨ãã§ãã¾ããä»¥ä¸ã®æé ã§ã³ãããã¡ãã»ã¼ã¸ãçæããã³ããããè¡ãã¾ã:
-1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://
-github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/
-STAGE_INFO_TEMPLATE_GAIAH.md)ã¨ãããã©ã¼ãããã§ãã¹ãã¼ã¸ã³ã°æå ±ãLLMã«æ¸¡ãã¾ãã
-2.
-LLMã¯ä»¥ä¸ã®ãããªå½¢å¼ã§ã³ãããã¡ãã»ã¼ã¸ãçæãã¾ã:
-``` Commit Messages ãã©ã¼ããã ## Commit 1 ### README.md ```commit-msg
-ð [docs] READMEã«å¿ç¨çãªä½¿ãæ¹ã»ã¯ã·ã§ã³ãè¿½å  -
-`README.md`ãã¡ã¤ã«ã«æ°ããªã»ã¯ã·ã§ã³ã¨ãã¦ãå¿ç¨çãªä½¿ãæ¹ããè¿½å ãã¾ãããããã«ãããã¦ã¼ã¶ã¼ã¯Gaiahãç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§ä½¿ç¨ããæ¹æ³ãå·ä½çã«å­¦ã¹ãããã«ãªãã¾ããç¹ã«ããªãã¸ããªã®æå®ãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãè¨­å®ããå·ä½çãªã³ãã³ãä¾ãç¤ºãã¦ãã¾ãã
-``` ## Commit 2 ### gaiah/__init__.py ```commit-msg ð [chore]
-Gaiahã®ãã¼ã¸ã§ã³ã0.3.12ã«æ´æ° - `gaiah/
-__init__.py`ã§ã®ãã¼ã¸ã§ã³çªå·ã0.3.11ãã0.3.12ã¸æ´æ°ãã¾ããããã®æ´æ°ã¯ãææ°ã®æ©è½æ¹åã¨ãã°ä¿®æ­£ãã¦ã¼ã¶ã¼ã«æä¾ããããã®ãã®ã§ãã
-``` ``` 3.
-çæãããã³ãããã¡ãã»ã¼ã¸ã`.Gaiah.md`ãã¡ã¤ã«ã«è²¼ãä»ãã¾ãããã®ãã¡ã¤ã«ã¯ãååã«`gaiah`ã³ãã³ããå®è¡ããéã«èªåã§çæããã¾ãã
-4.
-ååº¦`gaiah`ã³ãã³ããå®è¡ããã¨ã`.Gaiah.md`ãã¡ã¤ã«ããã³ãããã¡ãã»ã¼ã¸ãèª­ã¿è¾¼ã¾ããèªåçã«ã³ãããã¨ããã·ã¥ãè¡ããã¾ãã
-## ð¤ è²¢ç®
+``` ### ãªãã¸ããªã®åæå ```bash gaiah --create_repo --repo_name
+Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:
+\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
+``` ## å¦çãã­ã¼ ```mermaid graph TD A[ã¦ã¼ã¶ã¼ãCLIãå®è¡] --> B
+{ã³ãã³ãã©ã¤ã³å¼æ°ãè§£æ} B --> C
+{Gaiahãªãã¸ã§ã¯ããä½æ} C --> D{--
+create_repoãªãã·ã§ã³ãæå®ããã¦ãã?} D -->|Yes| E
+[æ°ãããªãã¸ããªãGitHubä¸ã«ä½æ] E --> E1
+[.envãã¡ã¤ã«ããç°å¢å¤æ°ãèª­ã¿è¾¼ã] E1 --> E2
+[ç°å¢å¤æ°ããã¢ã¯ã»ã¹ãã¼ã¯ã³ãåå¾] E2 --> E3
+[GitHubãªãã¸ã§ã¯ããä½æ] E3 --> E4
+[ãªãã¸ããªåã¨ãã©ã¡ã¼ã¿ãæå®] E4 --> E5
+[GitHubä¸ã«æ°ãããªãã¸ããªãä½æ] E5 --> E6
+[ãªãã¸ããªä½æå®äºã®ã¡ãã»ã¼ã¸ãè¡¨ç¤º] E6 --> Q[å¦çå®äº]
+D -->|No| F{--process_commitsãªãã·ã§ã³ãæå®ããã¦ãã?} F --
+>|Yes| G[ã³ãããã¡ãã»ã¼ã¸ãã¡ã¤ã«ããã³ããããå¦ç] G
+--> H[ãã¹ã¦ã®ãã¡ã¤ã«ãã¢ã³ã¹ãã¼ã¸] H --> I
+{ã³ãããã»ã¯ã·ã§ã³ãã¨ã«å¦ç} I --> J
+{ãã¡ã¤ã«åã¨ã³ãããã¡ãã»ã¼ã¸ãåå¾} J --> K
+{ãã¡ã¤ã«ãå¦ç} K --> L{ãã¡ã¤ã«ãã¹ãã¼ã¸} L --> M
+{å¤æ´ãã³ããã} M --> N{æ¬¡ã®ã³ãããã»ã¯ã·ã§ã³ããã?} N
+-->|Yes| I N -->|No| O[ãªã¢ã¼ããªãã¸ããªã«ããã·ã¥] O --> P
+[å¦çå®äº] F -->|No| Q[å¦çå®äº] ``` ## éçºç¨ ```bash gaiah --
+repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits ``` ## ð¤
+è²¢ç®
 Gaiahãããã«è¯ãããããã«ãã³ãã¥ããã£ããã®è²¢ç®ãæ­è¿ãã¾ããã¢ã¤ãã¢ãææ¡ããã°å ±åãããå ´åã¯ã
 [GitHubãªãã¸ããª](https://github.com/Sunwood-ai-labs/Gaiah)ã§ issue
 ãéããããã«ãªã¯ã¨ã¹ããéä¿¡ãã¦ãã ããã ## ð
 ã©ã¤ã»ã³ã¹ Gaiahã¯ã[MITã©ã¤ã»ã³ã¹](https://opensource.org/
 licenses/
 MIT)ã®ä¸ã§ãªãªã¼ã¹ããã¦ãããã©ã¤ãã©ãªã®èªç±ãã¤ãªã¼ãã³ã½ã¼ã¹ã§ã®ä½¿ç¨ãå¤æ´ãéå¸ãå¯è½ã§ãã
 ## ð è¬è¾
```

### Comparing `gaiah_toolkit-0.3.13/tests/test_cli.py` & `gaiah_toolkit-0.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gaiah_toolkit-0.3.13/tests/test_main.py` & `gaiah_toolkit-0.4.0/tests/test_main.py`

 * *Files identical despite different names*

