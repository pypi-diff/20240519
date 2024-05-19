# Comparing `tmp/ops_py_azure_key_vault_alert-4.8.0.tar.gz` & `tmp/ops_py_azure_key_vault_alert-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_py_azure_key_vault_alert-4.8.0.tar", last modified: Wed May  1 08:13:58 2024, max compression
+gzip compressed data, was "ops_py_azure_key_vault_alert-5.0.0.tar", last modified: Sun May 19 13:02:41 2024, max compression
```

## Comparing `ops_py_azure_key_vault_alert-4.8.0.tar` & `ops_py_azure_key_vault_alert-5.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:13:58.161855 ops_py_azure_key_vault_alert-4.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-01 08:13:56.000000 ops_py_azure_key_vault_alert-4.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-01 08:13:58.161855 ops_py_azure_key_vault_alert-4.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:13:58.157855 ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-05-01 08:13:51.000000 ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11035 2024-05-01 08:13:51.000000 ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/azure_key_vault_alert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2531 2024-05-01 08:13:51.000000 ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/slack_post.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2281 2024-05-01 08:13:51.000000 ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/teams_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:13:58.161855 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-01 08:13:58.000000 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-01 08:13:58.000000 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:13:58.000000 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-01 08:13:58.000000 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 08:13:58.000000 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-01 08:13:56.000000 ops_py_azure_key_vault_alert-4.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-01 08:13:56.000000 ops_py_azure_key_vault_alert-4.8.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-01 08:13:51.000000 ops_py_azure_key_vault_alert-4.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 08:13:58.161855 ops_py_azure_key_vault_alert-4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 08:13:56.000000 ops_py_azure_key_vault_alert-4.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:02:41.188926 ops_py_azure_key_vault_alert-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-19 13:02:39.000000 ops_py_azure_key_vault_alert-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-05-19 13:02:41.188926 ops_py_azure_key_vault_alert-5.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:02:41.184926 ops_py_azure_key_vault_alert-5.0.0/azure_key_vault_alert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-05-19 13:02:36.000000 ops_py_azure_key_vault_alert-5.0.0/azure_key_vault_alert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11475 2024-05-19 13:02:36.000000 ops_py_azure_key_vault_alert-5.0.0/azure_key_vault_alert/azure_key_vault_alert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1298 2024-05-19 13:02:36.000000 ops_py_azure_key_vault_alert-5.0.0/azure_key_vault_alert/post_payloads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1537 2024-05-19 13:02:36.000000 ops_py_azure_key_vault_alert-5.0.0/azure_key_vault_alert/slack_workflow_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2284 2024-05-19 13:02:36.000000 ops_py_azure_key_vault_alert-5.0.0/azure_key_vault_alert/teams_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:02:41.184926 ops_py_azure_key_vault_alert-5.0.0/ops_py_azure_key_vault_alert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-05-19 13:02:41.000000 ops_py_azure_key_vault_alert-5.0.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-19 13:02:41.000000 ops_py_azure_key_vault_alert-5.0.0/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:02:41.000000 ops_py_azure_key_vault_alert-5.0.0/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-19 13:02:41.000000 ops_py_azure_key_vault_alert-5.0.0/ops_py_azure_key_vault_alert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 13:02:41.000000 ops_py_azure_key_vault_alert-5.0.0/ops_py_azure_key_vault_alert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-19 13:02:39.000000 ops_py_azure_key_vault_alert-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-05-19 13:02:39.000000 ops_py_azure_key_vault_alert-5.0.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-19 13:02:36.000000 ops_py_azure_key_vault_alert-5.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:02:41.188926 ops_py_azure_key_vault_alert-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-19 13:02:39.000000 ops_py_azure_key_vault_alert-5.0.0/setup.py
```

### Comparing `ops_py_azure_key_vault_alert-4.8.0/LICENSE` & `ops_py_azure_key_vault_alert-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_alert-4.8.0/PKG-INFO` & `ops_py_azure_key_vault_alert-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.8.0
+Version: 5.0.0
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -32,59 +32,62 @@
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: docutils==0.21.2
 Requires-Dist: idna==3.6
 Requires-Dist: importlib_metadata==7.1.0
 Requires-Dist: jaraco.classes==3.4.0
 Requires-Dist: jaraco.context==5.3.0
 Requires-Dist: jaraco.functools==4.0.1
-Requires-Dist: keyring==25.1.0
+Requires-Dist: keyring==25.2.1
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: nh3==0.2.17
-Requires-Dist: ops-py-azure-key-vault-report==5.0.5
+Requires-Dist: ops-py-azure-key-vault-report==6.0.0
 Requires-Dist: ops-py-generate-pyproject==2.2.3
 Requires-Dist: ops-py-message-handler==1.0.3
 Requires-Dist: packaging==24.0
 Requires-Dist: pip==24.0
 Requires-Dist: pkginfo==1.10.0
-Requires-Dist: Pygments==2.17.2
-Requires-Dist: pyproject_hooks==1.0.0
+Requires-Dist: Pygments==2.18.0
+Requires-Dist: pyproject_hooks==1.1.0
 Requires-Dist: readme_renderer==43.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: setuptools==69.1.0
-Requires-Dist: twine==5.0.0
+Requires-Dist: twine==5.1.0
 Requires-Dist: urllib3==2.2.0
 Requires-Dist: wheel==0.42.0
-Requires-Dist: zipp==3.18.1
+Requires-Dist: zipp==3.18.2
 
 # azure-key-vault-alert
 
 ## Description
 
 Uses the [ops-py-azure-key-vault-report](https://pypi.org/project/ops-py-azure-key-vault-report) tool to generate:
    
 ### Azure Key Vault reports  
 Which may be posted to a *Slack App* webhook, *Slack Workflow* webhook, or an *MS Teams* webhook.
 
 The output is formatted as a *Slack Code Block* when posted Slack. The content is output as a two plaintext Markdown tables:   
-the Summary and the Report.
+the Summary and the Report.  
+
+Long reports will be split into multiple parts. Part number will then be added to each part.   
 
 When posted to a MS Teams payload the Summary is formatted as *Facts*, followed by the Report as an HTML Table.
 
 ***OR***
 
 ### Azure Key Vault Slack alerts   
-Are only supported posted to a *Slack App* webhook.
-
 Each alert message is formatted as Slack Markdown.
 
+### Azure Key Vault MS Teams alerts
+Each alert message is formatted as `AdaptiveCard` with `TextBlock`s.
+
 
 ## Installation
 `pip install ops-py-azure-key-vault-alert`
 
 ## Usage
 
 ### Environment variables
@@ -213,15 +216,15 @@
 *The summary* will contain info about *every records parsed*, even if the record is not included to be output in the report.   
 **NOTE:** Only the *Record Types* specified will be included in the summary.   
 **NOTE:** If no records are included in the report (none expired and none expiring within the threshold), the summary will still be posted.  
 
 **For specified Key Vaults, alert if any records is about to expire within the next 14 days or if any record has expired with the last 14 days**   
 `python3 azure_key_vault_alert -v kv-dev kv--test kv-qa -c 14`
 
-**NOTE:** Each record will be alerted on in separate Slack messages.   
+**NOTE:** Each record will be alerted on in separate messages.   
 **NOTE:** E.g. if a record then has expired for 15 days or more, it will not be alerted on.  
 
 **Log all output**  
 A summary and a full report is always written to file. This may then be used to post to an Monitoring service API etc., e.g.:   
 ```
 curl --request POST \  
   --header 'Content-Type: application/json' \
```

### Comparing `ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/azure_key_vault_alert.py` & `ops_py_azure_key_vault_alert-5.0.0/azure_key_vault_alert/azure_key_vault_alert.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import logging
 import argparse
 import json
 import re
 from azure_key_vault_report import azure_key_vault_report
 from azure_key_vault_report import az_cmd
 from message_handler import message_handler
-from .slack_post import slack_post
-from .teams_alert import teams_alert
+from .slack_workflow_report import slack_workflow_report
+from .teams_report import teams_report
+from .post_payloads import post_payloads
 
 ########################################################################################################################
 
 
 def main():
     logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.INFO)
 
@@ -118,15 +119,15 @@
     kv_report = azure_key_vault_report.AzureKeyVaultReport(az_results)
     kv_report.parse_results()
     kv_report.add_summary()
     kv_report.add_report(expire_threshold=expire_threshold,
                          ignore_no_expiration=ignore_no_expiration,
                          include_all=include_all,
                          teams_json=teams_output,
-                         critical_threshold=alert_threshold)
+                         alert_threshold=alert_threshold)
 
     # Get the full report which will be written to file, and may be used for future references (logging / monitoring).
     # The name of the Workflow and Azure resource information are added to the json object.
     report_full = kv_report.get_report_full()
     if isinstance(report_full, dict):
         workflow_output_name = str(WORKFLOW_OUTPUT_NAME).strip().lower().replace(" ", "_")[:40]
         report_full["name"] = workflow_output_name
@@ -156,49 +157,64 @@
         print(report)
         return
 
     # Initializes the Message Handler
     if WEBHOOK_REPORT:
         msg_handler = message_handler.MessageHandler(WEBHOOK_REPORT)
 
-    # If the webhook is previously determined to be an MS Teams webhook, the teams_alert function is called
-    if teams_output:
-        success = teams_alert(title, kv_report, teams_max_chars, stdout_only=stdout_only, msg_handler=msg_handler)
+    # If to alert
+    if isinstance(alert_threshold, int):
+        payloads = None
+
+        # If the webhook is previously determined to be an MS Teams webhook, then get the teams alert payloads
+        if teams_output:
+            payloads = kv_report.get_teams_payloads(title, alert=True)
 
-    # If the webhook is previously determined NOT to be an MS Teams webhook
-    if msg_handler and not teams_output:
-
-        # If the webhook is previously determined to be a Slack App webhook
+        # If the webhook is previously determined to be a Slack App webhook, then get the slack alert payloads
         if slack_app:
-            if not isinstance(alert_threshold, int):
-                # If an 'alert_threshold' is NOT provided, Slack report payloads will be used
-                payloads = kv_report.get_slack_payloads(title, max_chars=slack_split_chars)
-            else:
-                # If an 'alert_threshold' is provided, Slack alert payloads will be used
-                payloads = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, md=True)
-
-            # If payloads, the slack_post function is called
-            if payloads:
-                success = slack_post(msg_handler, payloads=payloads)
-
-        # Proceed if the webhook is previously determined to NOT be a Slack App webhook (but a Slack Workflow webhook)
-        # and no 'alert_threshold' is specified (Slack Workflow is not supported for this) and
-        # that we do not post if we already have a success from an earlier post.
-        if not slack_app and not isinstance(alert_threshold, int) and not success:
-            posts = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, app=False)
-            if posts:
-                # The slack_post function is called
-                success = slack_post(msg_handler, posts=posts)
+            payloads = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, alert=True)
+
+        # If payloads, then post the payload by calling the post_payloads function
+        if payloads and msg_handler:
+            success = post_payloads(msg_handler, payloads)
+
+        # If no payloads, then just log
+        if (slack_app or teams_output) and not payloads and message_handler:
+            msg = "No records to alert on detected."
+            logging.error(msg)
 
-        # If the only option left is to post alert messages to a Slack Workflow (which is not supported),
-        # a message regarding info about not supported is posted instead.
-        if isinstance(alert_threshold, int) and not slack_app and not success:
+        # If alert and Slack Workflow, then log and post message about that is not supported
+        if not slack_app and not teams_output and not payloads and message_handler:
             error_msg = "Posting individual critical messages to Slack Workflow is not supported."
             logging.error(error_msg)
-            success = slack_post(msg_handler, posts=[(f"ERROR - {title}", error_msg)])
+            success = slack_workflow_report(msg_handler, posts=[(f"ERROR - {title}", error_msg)])
+
+    # if not alert, then report
+    else:
+        payloads = None
+
+        # If the webhook is previously determined to be an MS Teams webhook, the teams_report function is called
+        # which also will post the report message
+        if teams_output:
+            success = teams_report(title, kv_report, teams_max_chars, stdout_only=stdout_only, msg_handler=msg_handler)
+
+        # If the webhook is previously determined to be a Slack App webhook, then get the slack report payloads
+        if slack_app:
+            payloads = kv_report.get_slack_payloads(title, max_chars=slack_split_chars)
+
+        # If payloads, the slack_post function is called to post the report payloads
+        if payloads and msg_handler:
+            success = post_payloads(msg_handler, payloads)
+
+        # If Slack Workflow, then get the then get the slack report Workflow payloads
+        if not slack_app and not teams_output and msg_handler:
+            posts = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, app=False)
+            if posts:
+                # The slack_post function is called to post the Slack Workflow reports payloads
+                success = slack_workflow_report(msg_handler, posts=posts)
 
     # If success and 'WEBHOOK_NOTIFY' is provided
     # an additional notify will be posted to the 'WEBHOOK_NOTIFY' webhook
     if success and WEBHOOK_NOTIFY:
         logging.info(f"Trigger additional alert about new report message(s)...")
         alert = message_handler.MessageHandler(WEBHOOK_NOTIFY)
         alert.post_payload()
@@ -223,9 +239,8 @@
     GITHUB_REPOSITORY = os.getenv("GITHUB_REPOSITORY", "")
 
     # These Azure environment variables will be used in the full json logfile
     AZURE_CLIENT_ID = os.getenv("AZURE_CLIENT_ID")
     AZURE_SUBSCRIPTION_ID = os.getenv("AZURE_SUBSCRIPTION_ID")
     AZURE_TENANT_ID = os.getenv("AZURE_TENANT_ID")
 
-
     main()
```

### Comparing `ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/slack_post.py` & `ops_py_azure_key_vault_alert-5.0.0/azure_key_vault_alert/slack_workflow_report.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,31 @@
 #!/usr/bin/env python
 
 import logging
 
 
-def slack_post(msg_handler, payloads=None, posts=None):
+def slack_workflow_report(msg_handler, posts=None):
     """Calls the provided Message Handler object to build Slack payloads for a Slack Workflow.
     The payloads are built from the provided list of Slack Post (Tuples: "Title" / "Text").
-    OR
-    Processes the provided list of Slack App payloads.
 
     The payloads are posted by the Message Handler.
 
     Parameters
     ----------
     msg_handler : __init__.py
         A message_handler object
-    payloads : list
-        The list of Slack App payloads to post
     posts : list
         The list Tuples of Slack Workflow messages to post [(Title, Text)...]
 
     Returns
     -------
     True
         If response from one or more of the POSTs have return code 200
     """
 
-    # Proceed with the list of Slack App payloads if provided. The success counter is initially set to 0
-    if isinstance(payloads, list):
-        success_counter = 0
-        for p in payloads:
-            msg_handler.set_payload(p)
-            msg_handler.post_payload()
-
-            # If any of the payloads are sent it is considered a success
-            response_code = msg_handler.get_response_code()
-            if isinstance(response_code, int) and response_code == 200:
-                success_counter += 1
-            else:
-                logging.error(f"Failed to send message to Slack App. Response code {str(response_code)}.")
-
-        # Return True if success so that we know at least one message have been sent
-        if success_counter:
-            logging.info(f"{success_counter} messages posted to the Slack app.")
-            return True
-
     # Proceed with the list of Slack Workflow Post if provided. The success counter is initially set to 0
     if isinstance(posts, list):
         success_counter = 0
         for title_, text_ in posts:
             msg_handler.build_payload(Title=title_, Text=text_)
             msg_handler.post_payload()
```

### Comparing `ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/teams_alert.py` & `ops_py_azure_key_vault_alert-5.0.0/azure_key_vault_alert/teams_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 import logging
 
 
-def teams_alert(title, kv, max_chars, stdout_only=False, msg_handler=None):
+def teams_report(title, kv, max_chars, stdout_only=False, msg_handler=None):
     """Gets a payload from azure_key_vault_report object and push it to the msg_handler,
     or optionally just print to standard out.
 
     Parameters
     ----------
     title : str
         The title of the message
@@ -24,15 +24,15 @@
     Returns
     -------
     True
         If response from the POST has return code 200
     """
 
     # A payload with the report as html table is generated
-    payload = kv.get_teams_payload(title)
+    payload = kv.get_teams_payloads(title)
 
     # Return if no payload
     if not payload:
         logging.error("Unable to retrieve MS Teams payload")
         return
 
     # If stdout_only we print the payload to standard output only and then return
@@ -43,15 +43,15 @@
     # If payload is too large with the report as html, a new payload is generated.
     # A custom text is provided instead, which will be used instead of the html report.
     if len(payload) > max_chars:
         warning_msg = f"The {title} length is above the character limit count of {max_chars}"
         logging.warning(warning_msg)
         title = f"WARNING! {warning_msg}"
         text = "The html report have been omitted from the report due to size limits."
-        payload = kv.get_teams_payload(title, text=text)
+        payload = kv.get_teams_payloads(title, text=text)
 
     # The payload is set and ready to be posted
     logging.info(f"Using payload: {payload}")
 
     # Proceed with posting the payload to Message Handler if the 'msg_handler' was provided
     if msg_handler:
         msg_handler.set_payload(payload)
```

### Comparing `ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO` & `ops_py_azure_key_vault_alert-5.0.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.8.0
+Version: 5.0.0
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -32,59 +32,62 @@
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: docutils==0.21.2
 Requires-Dist: idna==3.6
 Requires-Dist: importlib_metadata==7.1.0
 Requires-Dist: jaraco.classes==3.4.0
 Requires-Dist: jaraco.context==5.3.0
 Requires-Dist: jaraco.functools==4.0.1
-Requires-Dist: keyring==25.1.0
+Requires-Dist: keyring==25.2.1
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: nh3==0.2.17
-Requires-Dist: ops-py-azure-key-vault-report==5.0.5
+Requires-Dist: ops-py-azure-key-vault-report==6.0.0
 Requires-Dist: ops-py-generate-pyproject==2.2.3
 Requires-Dist: ops-py-message-handler==1.0.3
 Requires-Dist: packaging==24.0
 Requires-Dist: pip==24.0
 Requires-Dist: pkginfo==1.10.0
-Requires-Dist: Pygments==2.17.2
-Requires-Dist: pyproject_hooks==1.0.0
+Requires-Dist: Pygments==2.18.0
+Requires-Dist: pyproject_hooks==1.1.0
 Requires-Dist: readme_renderer==43.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: setuptools==69.1.0
-Requires-Dist: twine==5.0.0
+Requires-Dist: twine==5.1.0
 Requires-Dist: urllib3==2.2.0
 Requires-Dist: wheel==0.42.0
-Requires-Dist: zipp==3.18.1
+Requires-Dist: zipp==3.18.2
 
 # azure-key-vault-alert
 
 ## Description
 
 Uses the [ops-py-azure-key-vault-report](https://pypi.org/project/ops-py-azure-key-vault-report) tool to generate:
    
 ### Azure Key Vault reports  
 Which may be posted to a *Slack App* webhook, *Slack Workflow* webhook, or an *MS Teams* webhook.
 
 The output is formatted as a *Slack Code Block* when posted Slack. The content is output as a two plaintext Markdown tables:   
-the Summary and the Report.
+the Summary and the Report.  
+
+Long reports will be split into multiple parts. Part number will then be added to each part.   
 
 When posted to a MS Teams payload the Summary is formatted as *Facts*, followed by the Report as an HTML Table.
 
 ***OR***
 
 ### Azure Key Vault Slack alerts   
-Are only supported posted to a *Slack App* webhook.
-
 Each alert message is formatted as Slack Markdown.
 
+### Azure Key Vault MS Teams alerts
+Each alert message is formatted as `AdaptiveCard` with `TextBlock`s.
+
 
 ## Installation
 `pip install ops-py-azure-key-vault-alert`
 
 ## Usage
 
 ### Environment variables
@@ -213,15 +216,15 @@
 *The summary* will contain info about *every records parsed*, even if the record is not included to be output in the report.   
 **NOTE:** Only the *Record Types* specified will be included in the summary.   
 **NOTE:** If no records are included in the report (none expired and none expiring within the threshold), the summary will still be posted.  
 
 **For specified Key Vaults, alert if any records is about to expire within the next 14 days or if any record has expired with the last 14 days**   
 `python3 azure_key_vault_alert -v kv-dev kv--test kv-qa -c 14`
 
-**NOTE:** Each record will be alerted on in separate Slack messages.   
+**NOTE:** Each record will be alerted on in separate messages.   
 **NOTE:** E.g. if a record then has expired for 15 days or more, it will not be alerted on.  
 
 **Log all output**  
 A summary and a full report is always written to file. This may then be used to post to an Monitoring service API etc., e.g.:   
 ```
 curl --request POST \  
   --header 'Content-Type: application/json' \
```

### Comparing `ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/requires.txt` & `ops_py_azure_key_vault_alert-5.0.0/ops_py_azure_key_vault_alert.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 charset-normalizer==3.3.2
 docutils==0.21.2
 idna==3.6
 importlib_metadata==7.1.0
 jaraco.classes==3.4.0
 jaraco.context==5.3.0
 jaraco.functools==4.0.1
-keyring==25.1.0
+keyring==25.2.1
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==10.2.0
 nh3==0.2.17
-ops-py-azure-key-vault-report==5.0.5
+ops-py-azure-key-vault-report==6.0.0
 ops-py-generate-pyproject==2.2.3
 ops-py-message-handler==1.0.3
 packaging==24.0
 pip==24.0
 pkginfo==1.10.0
-Pygments==2.17.2
-pyproject_hooks==1.0.0
+Pygments==2.18.0
+pyproject_hooks==1.1.0
 readme_renderer==43.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 setuptools==69.1.0
-twine==5.0.0
+twine==5.1.0
 urllib3==2.2.0
 wheel==0.42.0
-zipp==3.18.1
+zipp==3.18.2
```

### Comparing `ops_py_azure_key_vault_alert-4.8.0/readme.md` & `ops_py_azure_key_vault_alert-5.0.0/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 
 Uses the [ops-py-azure-key-vault-report](https://pypi.org/project/ops-py-azure-key-vault-report) tool to generate:
    
 ### Azure Key Vault reports  
 Which may be posted to a *Slack App* webhook, *Slack Workflow* webhook, or an *MS Teams* webhook.
 
 The output is formatted as a *Slack Code Block* when posted Slack. The content is output as a two plaintext Markdown tables:   
-the Summary and the Report.
+the Summary and the Report.  
+
+Long reports will be split into multiple parts. Part number will then be added to each part.   
 
 When posted to a MS Teams payload the Summary is formatted as *Facts*, followed by the Report as an HTML Table.
 
 ***OR***
 
 ### Azure Key Vault Slack alerts   
-Are only supported posted to a *Slack App* webhook.
-
 Each alert message is formatted as Slack Markdown.
 
+### Azure Key Vault MS Teams alerts
+Each alert message is formatted as `AdaptiveCard` with `TextBlock`s.
+
 
 ## Installation
 `pip install ops-py-azure-key-vault-alert`
 
 ## Usage
 
 ### Environment variables
@@ -151,15 +154,15 @@
 *The summary* will contain info about *every records parsed*, even if the record is not included to be output in the report.   
 **NOTE:** Only the *Record Types* specified will be included in the summary.   
 **NOTE:** If no records are included in the report (none expired and none expiring within the threshold), the summary will still be posted.  
 
 **For specified Key Vaults, alert if any records is about to expire within the next 14 days or if any record has expired with the last 14 days**   
 `python3 azure_key_vault_alert -v kv-dev kv--test kv-qa -c 14`
 
-**NOTE:** Each record will be alerted on in separate Slack messages.   
+**NOTE:** Each record will be alerted on in separate messages.   
 **NOTE:** E.g. if a record then has expired for 15 days or more, it will not be alerted on.  
 
 **Log all output**  
 A summary and a full report is always written to file. This may then be used to post to an Monitoring service API etc., e.g.:   
 ```
 curl --request POST \  
   --header 'Content-Type: application/json' \
```

### Comparing `ops_py_azure_key_vault_alert-4.8.0/requirements.txt` & `ops_py_azure_key_vault_alert-5.0.0/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 charset-normalizer==3.3.2
 docutils==0.21.2
 idna==3.6
 importlib_metadata==7.1.0
 jaraco.classes==3.4.0
 jaraco.context==5.3.0
 jaraco.functools==4.0.1
-keyring==25.1.0
+keyring==25.2.1
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==10.2.0
 nh3==0.2.17
-ops-py-azure-key-vault-report==5.0.5
+ops-py-azure-key-vault-report==6.0.0
 ops-py-generate-pyproject==2.2.3
 ops-py-message-handler==1.0.3
 packaging==24.0
 pip==24.0
 pkginfo==1.10.0
-Pygments==2.17.2
-pyproject_hooks==1.0.0
+Pygments==2.18.0
+pyproject_hooks==1.1.0
 readme_renderer==43.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 setuptools==69.1.0
-twine==5.0.0
+twine==5.1.0
 urllib3==2.2.0
 wheel==0.42.0
-zipp==3.18.1
+zipp==3.18.2
```

