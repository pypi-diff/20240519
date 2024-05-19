# Comparing `tmp/needto-0.0.4.tar.gz` & `tmp/needto-0.1.0.tar.gz`

## Comparing `needto-0.0.4.tar` & `needto-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.0.4/needto/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.0.4/needto/__init__.py
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 needto-0.0.4/needto/__main__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.0.4/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 needto-0.0.4/README.md
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 needto-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.1.0/needto/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.1.0/needto/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 needto-0.1.0/needto/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 needto-0.1.0/needto/src/__init__.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 needto-0.1.0/needto/src/ai_client.py
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 needto-0.1.0/needto/src/cli.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 needto-0.1.0/needto/src/config.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 needto-0.1.0/needto/src/utils.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 needto-0.1.0/README.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 needto-0.1.0/PKG-INFO
```

### Comparing `needto-0.0.4/needto/__main__.py` & `needto-0.1.0/needto/src/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,172 +1,85 @@
-import typing
 import os
 import click
-import json
 import sys
-import platform
-from simple_term_menu import TerminalMenu
 import typer
-import groq
 import rich.console
 import rich.prompt
 import subprocess
 from rich.markdown import Markdown
 
-try:
-    client = groq.Groq(
-        api_key=os.environ.get("GROQ_API_KEY"),
-    )
-except groq.GroqError:
-    print("Please set GROQ_API_KEY environment variable.")
-    sys.exit(1)
-
-app = typer.Typer()
-
-
-class AIClient:
-    def __init__(self, *, system_prompt: str, model_name: str = "llama3-70b-8192"):
-        console = rich.console.Console()
-        self.model_name = model_name
-        final_prompt = f"""{system_prompt}
-        System Info: OS: {platform.system()}, Arch: {platform.machine()}"""
-        messages = [
-            {"role": "system", "content": final_prompt.strip().replace("    ", "")},
-        ]
-        if stdin := "" if sys.stdin.isatty() else sys.stdin.read():
-            console.print("Got this from stdin:")
-            console.print(stdin)
-            messages.append(
-                {"role": "user", "content": f"Additional information:\n{stdin}"}
-            )
-        self.messages = messages
-
-    def ask(self, prompt: str, print_prompt=False, output_limit: int = 2000):
-        prompt = prompt.strip()[:output_limit]
-        console = rich.console.Console()
-        if print_prompt:
-            print()
-            console.print(prompt)
-            print()
-
-        self.messages.append({"role": "user", "content": prompt})
-        chat_completion = client.chat.completions.create(
-            messages=self.messages,
-            model=self.model_name,
-            response_format={"type": "json_object"},
-        )
-        answer = chat_completion.choices[0].message.content
-        self.messages.append({"role": "system", "content": answer})
-        try:
-            return json.loads(answer)
-        except json.decoder.JSONDecodeError:
-            with open("error.txt", "w") as fp:
-                fp.write(answer)
-
-
-def prompt_menu(
-    recommended_commands: list[str],
-    *,
-    ask_for_edit=False,
-    confirm_prompt="",
-    preview_command: None | str | typing.Callable[[str], str] = None,
-):
-    console = rich.console.Console()
-    NO_OP = "-- explain more --"
-    commands_to_prompt: list[str] = [NO_OP] + recommended_commands
-    menu_entry_index = TerminalMenu(
-        [command.replace("|", r"\|") for command in commands_to_prompt],
-        preview_command=preview_command,
-    ).show()
-    selected_command: str = commands_to_prompt[menu_entry_index]
-
-    print()
-    for command in recommended_commands:
-        if command == selected_command:
-            console.print(f"$ {command}", style="black on white")
-        else:
-            console.print(f"$ {command}")
-    print()
-
-    if selected_command == NO_OP:
-        return
+from .config import config_manager
+from .ai_client import AIClient
+from .utils import prompt_menu_and_print
 
-    if ask_for_edit and sys.stdin.isatty():
-        if edited_text := click.edit(text=selected_command):
-            selected_command = edited_text.strip()
+app = typer.Typer(no_args_is_help=True)
 
-    if selected_command.startswith("#"):
-        return
 
-    if not sys.stdin.isatty():
-        sys.stdin = open("/dev/tty")
-
-    if confirm_prompt and not rich.prompt.Confirm.ask(
-        f"{confirm_prompt} '{selected_command}'", default=False
-    ):
-        return
-
-    return selected_command
-
-
-@app.command()
-def find(prompt: str):
+@app.command(help="Find and run a command.")
+def do(prompt_list: list[str]):
+    prompt = " ".join(prompt_list)
     console = rich.console.Console()
     system_prompt = """
     You are a CLI code generator. User will search for a command, you respond with a list of CLI commands.
     Always answer in json in all your responses with these keys:
-    "description" (str), "warning" (str only if necessary), "commands" (list of str), needs_manual_change (bool).
+    "description" (str), "warning" (str only if necessary), "commands" (list of str).
     """
     console = rich.console.Console()
     ai_client = AIClient(system_prompt=system_prompt)
     parsed_answer = ai_client.ask(prompt)
 
     while True:
         console.print(parsed_answer["description"], style="bold blue")
+
         if warning := parsed_answer.get("warning"):
             console.print(warning, style="bold yellow")
 
-        if selected_command := prompt_menu(
+        if selected_command := prompt_menu_and_print(
             parsed_answer["commands"],
-            ask_for_edit=parsed_answer["needs_manual_change"],
-            confirm_prompt="Running",
+            ask_for_edit=True,
+            confirm_prompt="Run",
         ):
             try:
                 result = subprocess.run(selected_command, shell=True, check=True)
             except subprocess.CalledProcessError as e:
                 console.print(e)
                 sys.exit(e.returncode)
             else:
                 console.print(f"Successfully ran '{selected_command}'.")
                 sys.exit(result.returncode)
         else:
+            console.print("Leave blank to end conversation", style="blue bold")
             if user_prompt := input("> "):
                 print()
                 parsed_answer = ai_client.ask(user_prompt)
             else:
                 break
 
 
-@app.command()
-def ask(prompt: str):
+@app.command(help="Ask question, Send output of commands to AI to get help.")
+def ask(prompt_list: list[str]):
+    prompt = " ".join(prompt_list)
     system_prompt = """
     You are a AI assistant. User will ask you something and you will help him find their answer.
     You can ask user to run commands and send the output of commands to you, to help you answer their questions.
+    Don't recommend commands that can change the system state.
     Always answer in json in all your responses with these keys:
     "help" (markdown str), "commands_to_explore" (list of str only if necessary)
     """
     console = rich.console.Console()
     ai_client = AIClient(system_prompt=system_prompt)
     parsed_answer = ai_client.ask(prompt)
     while True:
         console.print(Markdown(parsed_answer["help"]))
         print()
 
         if commands := parsed_answer.get("commands_to_explore"):
-            if command := prompt_menu(commands):
+            if command := prompt_menu_and_print(
+                commands, confirm_prompt="Run and send output of", ask_for_edit=True
+            ):
                 try:
                     command_output = subprocess.run(
                         command, shell=True, capture_output=True
                     )
                 except subprocess.CalledProcessError as e:
                     parsed_answer = ai_client.ask(
                         f"Failed to run '{command}': {e}", print_prompt=True
@@ -179,55 +92,59 @@
                             f"stderr:\n{command_output.stderr.decode()}"
                             if command_output.stderr
                             else ""
                         ),
                         print_prompt=True,
                     )
             else:
+                console.print("Leave blank to end conversation", style="blue bold")
                 if user_prompt := input("> "):
                     print()
                     parsed_answer = ai_client.ask(user_prompt)
                 else:
                     break
         else:
             break
 
 
-@app.command()
-def write(prompt: str):
+@app.command(help="Write code.")
+def write(prompt_list: list[str]):
+    prompt = " ".join(prompt_list)
     system_prompt = """
     You are a AI assistant. User will ask you to write a code.
     You can ask user to clarify what they need and then run the code.
     Always answer in json in all your responses with these keys:
     "help" (markdown str), "files_to_save": (object with name to content)
     """
     console = rich.console.Console()
     ai_client = AIClient(system_prompt=system_prompt)
     parsed_answer = ai_client.ask(prompt)
     while True:
         console.print(Markdown(parsed_answer["help"]))
         files_to_save = parsed_answer.get("files_to_save", {})
         print()
         if files_to_save:
-            if selected_file_name := prompt_menu(
+            if selected_file_name := prompt_menu_and_print(
                 list(files_to_save.keys()),
                 preview_command=lambda file_name: files_to_save.get(file_name, ""),
             ):
                 file_content = files_to_save[selected_file_name]
                 while os.path.exists(selected_file_name):
-                    selected_file_name = rich.prompt.Prompt.ask(
+                    selected_file_name = console.print(
                         f"[bold red]'{selected_file_name}' already exists[/bold red]. Please enter a new name",
                     )
                 with open(selected_file_name, "w") as f:
                     f.write(file_content)
                 console.print(f"'{selected_file_name}' saved.", style="bold green")
                 break
 
-        if user_prompt := input("> "):
+        console.print("Leave blank to end conversation", style="blue bold")
+        if user_prompt := ("> ",):
             print()
             parsed_answer = ai_client.ask(user_prompt)
         else:
             break
 
 
-if __name__ == "__main__":
-    app()
+@app.command(help=f"Open editor for '{config_manager.config_path}'.")
+def config():
+    click.edit(filename=config_manager.config_path)
```

### Comparing `needto-0.0.4/.gitignore` & `needto-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `needto-0.0.4/LICENSE.txt` & `needto-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `needto-0.0.4/pyproject.toml` & `needto-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `needto-0.0.4/PKG-INFO` & `needto-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: needto
-Version: 0.0.4
+Version: 0.1.0
 Summary: Ask AI for help you in your terminal.
 Project-URL: Documentation, https://github.com/danialkeimasi/needto#readme
 Project-URL: Issues, https://github.com/danialkeimasi/needto/issues
 Project-URL: Source, https://github.com/danialkeimasi/needto
 Author-email: Danial Keimasi <danialkeimasi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

