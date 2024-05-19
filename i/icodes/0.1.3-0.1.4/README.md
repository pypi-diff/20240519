# Comparing `tmp/icodes-0.1.3.tar.gz` & `tmp/icodes-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icodes-0.1.3.tar", max compression
+gzip compressed data, was "icodes-0.1.4.tar", max compression
```

## Comparing `icodes-0.1.3.tar` & `icodes-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     7048 2024-03-31 18:37:25.121754 icodes-0.1.3/LICENSE
--rw-r--r--   0        0        0     3198 2024-04-14 11:34:16.112163 icodes-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-06 19:55:00.301396 icodes-0.1.3/icds/__init__.py
--rw-r--r--   0        0        0     1935 2024-04-14 09:52:58.273822 icodes-0.1.3/icds/data.py
--rw-r--r--   0        0        0     1285 2024-04-14 09:43:58.775498 icodes-0.1.3/icds/git_helpers.py
--rw-r--r--   0        0        0     3124 2024-04-06 19:55:00.301396 icodes-0.1.3/icds/llm_interface.py
--rw-r--r--   0        0        0      797 2024-04-14 09:43:58.775498 icodes-0.1.3/icds/models.py
--rw-r--r--   0        0        0      236 2024-04-14 11:31:26.942217 icodes-0.1.3/icds/settings.py
--rw-r--r--   0        0        0     4520 2024-04-14 11:28:48.808145 icodes-0.1.3/icodes.py
--rw-r--r--   0        0        0     1145 2024-04-14 11:34:40.779865 icodes-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4256 1970-01-01 00:00:00.000000 icodes-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7048 2024-03-31 18:37:25.121754 icodes-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3687 2024-04-19 11:32:05.096609 icodes-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 19:55:00.301396 icodes-0.1.4/icds/__init__.py
+-rw-r--r--   0        0        0     2393 2024-05-19 15:27:23.586253 icodes-0.1.4/icds/data.py
+-rw-r--r--   0        0        0     2220 2024-04-19 11:32:05.096609 icodes-0.1.4/icds/git_helpers.py
+-rw-r--r--   0        0        0     3124 2024-04-06 19:55:00.301396 icodes-0.1.4/icds/llm_interface.py
+-rw-r--r--   0        0        0      797 2024-04-14 09:43:58.775498 icodes-0.1.4/icds/models.py
+-rw-r--r--   0        0        0      236 2024-04-14 11:31:26.942217 icodes-0.1.4/icds/settings.py
+-rw-r--r--   0        0        0     5500 2024-04-19 11:32:05.096609 icodes-0.1.4/icodes.py
+-rw-r--r--   0        0        0     1145 2024-05-19 15:29:24.089650 icodes-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4745 1970-01-01 00:00:00.000000 icodes-0.1.4/PKG-INFO
```

### Comparing `icodes-0.1.3/LICENSE` & `icodes-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `icodes-0.1.3/README.md` & `icodes-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 
 ### Inspecting a Repository
 
 To inspect a repository with iCODES, run:
 
     icodes inspect-repo /path/to/repo [--branch-name BRANCH_NAME]
 
-Replace /path/to/repo with the path to the Git repository you want to analyze. You can optionally specify a branch name using the --branch-name flag. If no branch is provided, iCODES will use the current branch for the repository.
+Replace /path/to/repo with the path to the Git repository you want to analyse. You can optionally specify a branch name using the --branch-name flag. If no branch is provided, iCODES will use the current branch for the repository.
 
-iCODES will analyze the latest commit on the specified branch and log the changes.
+iCODES will analyse the latest commit on the specified branch and log the changes.
 
 
 ### Building an Index
 
 To build an index for a Git repository with iCODES, run the following command:
 
     icodes build-index <path-to-repo>
@@ -63,15 +63,25 @@
 - `--author AUTHOR`: Filter commits by the specified author.
 - `--file FILE`: Filter commits that modified the specified file path.
 - `--start-date START_DATE`: Filter commits after the specified date (YYYY-MM-DD).
 - `--end-date END_DATE`: Filter commits before the specified date (YYYY-MM-DD).
 
 Example usage:
 
-    icodes search "bug fix" --author "John Doe" --file "src/main.py" --start-date "2023-01-01" --end-date "2023-12-31"
+    icodes search "bug fix" --author "Jane Doe" --file "src/main.py" --start-date "2023-01-01" --end-date "2023-12-31"
 
 This command will search for commits containing the phrase "bug fix" authored by "John Doe", modifying the file "src/main.py", between the dates "2023-01-01" and "2023-12-31".
 
+### Suggesting a commit for the currently staged changes
+
+You can now use the `suggest-commit-message` command to analyse the currently staged changes and suggest a commit message:
+
+    icodes suggest_commit_message /path/to/repo
+
+This command will retrieve the staged changes, format them into a commit-like format, and then use the LLM to analyse the changes and suggest a commit message.
+
+The suggested commit message and the detailed analysis will be displayed in the console output.
+
 
 ## Contributing
 
 We welcome contributions to iCODES!
```

### Comparing `icodes-0.1.3/icds/data.py` & `icodes-0.1.4/icds/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 
 def get_repo_by_name(db, name: str) -> DbRepo | None:
     statement = select(DbRepo).where(DbRepo.name == name)
     repo = db.exec(statement).first()
     return repo
 
 
+def list_repos(db, limit=None) -> list[DbRepo] | None:
+    statement = select(DbRepo)
+    if limit:
+        statement = statement.limit(limit)
+    repos = db.exec(statement).all()
+    return repos
+
+
 def get_or_create_db_repo(db, repo, repo_path) -> DbRepo:
     remote_url = repo.remotes.origin.url
     repo_name = remote_url.split("/")[-1].split(".")[0]
     db_repo = get_repo_by_name(db, repo_name)
     if not db_repo:
         logger.info(f"Creating a new repository record for repo '{repo_name}'")
         db_repo = DbRepo(
@@ -26,14 +34,22 @@
     return db_repo
 
 
 def get_repo_name_by_id(db, repo_id) -> str:
     return db.exec(select(DbRepo).where(DbRepo.id == repo_id)).first().name
 
 
+def list_commits(db, repo_id, limit=None) -> list[RepoCommit] | None:
+    statement = select(RepoCommit).where(RepoCommit.repo_id == repo_id)
+    if limit:
+        statement = statement.limit(limit)
+    commits = db.exec(statement).all()
+    return commits
+
+
 def search_commits(
     db, query, repo_name, file, author, start_date, end_date
 ) -> list[RepoCommit]:
     statement = select(RepoCommit)
     if repo_name:
         db_repo = get_repo_by_name(db, repo_name)
         if not db_repo:
```

### Comparing `icodes-0.1.3/icds/llm_interface.py` & `icodes-0.1.4/icds/llm_interface.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.3/icds/models.py` & `icodes-0.1.4/icds/models.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.3/icodes.py` & `icodes-0.1.4/icodes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typer import Typer, echo, Argument, Option
 from pathlib import Path
 
 from loguru import logger
 from git import Repo
 
-from icds.git_helpers import extract_commit_info
+from icds.git_helpers import extract_commit_info, get_staged_changes
 from icds.llm_interface import analyse_commit
 from icds.models import (
     create_db_and_tables,
     engine,
     RepoCommit,
     Session,
 )
@@ -21,15 +21,20 @@
 from icds.settings import settings
 
 app = Typer()
 
 
 @app.command()
 def inspect_repo(
-    repo_path: Path, branch_name: str = "", n_commits: int = 10, detailed: bool = False
+    repo_path: Path = Argument(..., help="Path to the git repository"),
+    branch_name: str = Option(
+        "", help="Branch name to inspect (default: current branch)"
+    ),
+    n_commits: int = Option(10, help="Number of commits to inspect (default: 10)"),
+    detailed: bool = Option(False, help="Show detailed analysis (default: False)"),
 ):
     """
     Inspect a git repository at a given path and branch. If no branch is provided, the current branch is used.
     Logs changes from the latest n_commits on the branch. If n_commits is not provided, a default maximum of 10
     commits are inspected.
     """
     repo = Repo(repo_path)
@@ -46,15 +51,21 @@
         echo(
             f"Summary of commit #{commit} by {commit.author} from {commit.authored_datetime}: \n"
         )
         echo("\t" + summary + "\n")
 
 
 @app.command()
-def build_index(repo_path: Path, branch_name: str = "", n_commits: int = 10):
+def build_index(
+    repo_path: Path = Argument(..., help="Path to the git repository"),
+    branch_name: str = Option(
+        "", help="Branch name to index (default: current branch)"
+    ),
+    n_commits: int = Option(10, help="Number of commits to index (default: 10)"),
+):
     """
     Build an index of the repository at the given path. If no branch is provided, the current branch is used.
     """
     repo = Repo(repo_path)
     if not branch_name:
         # Get the default branch configured for the repo
         branch_name = repo.active_branch.name
@@ -119,14 +130,31 @@
             echo(f"Author: {commit.author}")
             echo(f"Date: {commit.datetime}")
             echo(f"Summary: {commit.summary}")
             echo(f"Details: {commit.details}")
             echo("\n")
 
 
+@app.command()
+def suggest_commit_message(
+    repo_path: Path = Argument(..., help="Path to the git repository"),
+    detailed: bool = Option(False, help="Show detailed analysis (default: False)"),
+):
+    """
+    Analyse the currently staged changes and suggest a commit message.
+    """
+
+    repo = Repo(repo_path)
+    commit_info = get_staged_changes(repo)
+    analysis, summary = analyse_commit(commit_info)
+    if detailed:
+        echo(analysis + "\n\n")
+    echo(f"git commit -m '{summary}'")
+
+
 def main():
     create_db_and_tables()
     app()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `icodes-0.1.3/pyproject.toml` & `icodes-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "icodes"
-version = "0.1.3"
+version = "0.1.4"
 description = "LLM-powered Git archeology tool (a.k.a. Intelligent Commit Ontology Distiller and Enhanced Search)"
 authors = ["Jordan Dimov <jdimov@a115.co.uk>", "Bayo Ade <bayo.300@gmail.com>"]
 license = "CC0-1.0"
 readme = "README.md"
 packages = [
     { include = "icodes.py" },
     { include = "icds/**/*.py" },
```

### Comparing `icodes-0.1.3/PKG-INFO` & `icodes-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icodes
-Version: 0.1.3
+Version: 0.1.4
 Summary: LLM-powered Git archeology tool (a.k.a. Intelligent Commit Ontology Distiller and Enhanced Search)
 Home-page: https://github.com/a115/iCODES
 License: CC0-1.0
 Keywords: git,llm,archeology,commit,search
 Author: Jordan Dimov
 Author-email: jdimov@a115.co.uk
 Requires-Python: >=3.11,<4.0
@@ -62,17 +62,17 @@
 
 ### Inspecting a Repository
 
 To inspect a repository with iCODES, run:
 
     icodes inspect-repo /path/to/repo [--branch-name BRANCH_NAME]
 
-Replace /path/to/repo with the path to the Git repository you want to analyze. You can optionally specify a branch name using the --branch-name flag. If no branch is provided, iCODES will use the current branch for the repository.
+Replace /path/to/repo with the path to the Git repository you want to analyse. You can optionally specify a branch name using the --branch-name flag. If no branch is provided, iCODES will use the current branch for the repository.
 
-iCODES will analyze the latest commit on the specified branch and log the changes.
+iCODES will analyse the latest commit on the specified branch and log the changes.
 
 
 ### Building an Index
 
 To build an index for a Git repository with iCODES, run the following command:
 
     icodes build-index <path-to-repo>
@@ -89,16 +89,26 @@
 - `--author AUTHOR`: Filter commits by the specified author.
 - `--file FILE`: Filter commits that modified the specified file path.
 - `--start-date START_DATE`: Filter commits after the specified date (YYYY-MM-DD).
 - `--end-date END_DATE`: Filter commits before the specified date (YYYY-MM-DD).
 
 Example usage:
 
-    icodes search "bug fix" --author "John Doe" --file "src/main.py" --start-date "2023-01-01" --end-date "2023-12-31"
+    icodes search "bug fix" --author "Jane Doe" --file "src/main.py" --start-date "2023-01-01" --end-date "2023-12-31"
 
 This command will search for commits containing the phrase "bug fix" authored by "John Doe", modifying the file "src/main.py", between the dates "2023-01-01" and "2023-12-31".
 
+### Suggesting a commit for the currently staged changes
+
+You can now use the `suggest-commit-message` command to analyse the currently staged changes and suggest a commit message:
+
+    icodes suggest_commit_message /path/to/repo
+
+This command will retrieve the staged changes, format them into a commit-like format, and then use the LLM to analyse the changes and suggest a commit message.
+
+The suggested commit message and the detailed analysis will be displayed in the console output.
+
 
 ## Contributing
 
 We welcome contributions to iCODES!
```

