# Comparing `tmp/perian_cli-0.1.4.tar.gz` & `tmp/perian_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perian_cli-0.1.4.tar", max compression
+gzip compressed data, was "perian_cli-0.1.5.tar", max compression
```

## Comparing `perian_cli-0.1.4.tar` & `perian_cli-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1220 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/__init__.py
--rw-r--r--   0        0        0     3607 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/accelerator_type.py
--rw-r--r--   0        0        0     1452 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/billing.py
--rw-r--r--   0        0        0     3200 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/instance_type.py
--rw-r--r--   0        0        0     3670 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/job.py
--rw-r--r--   0        0        0     1020 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/organization.py
--rw-r--r--   0        0        0     4950 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/cli.py
--rw-r--r--   0        0        0      133 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/colors.py
--rw-r--r--   0        0        0        0 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/__init__.py
--rw-r--r--   0        0        0     3036 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/accelerator_type.py
--rw-r--r--   0        0        0     1846 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/billing.py
--rw-r--r--   0        0        0      344 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/config.py
--rw-r--r--   0        0        0      898 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/currency.py
--rw-r--r--   0        0        0     3526 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/instance_type.py
--rw-r--r--   0        0        0     9529 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/job.py
--rw-r--r--   0        0        0     4523 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/registry.py
--rw-r--r--   0        0        0     5756 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/responses.py
--rw-r--r--   0        0        0      446 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/settings.py
--rw-r--r--   0        0        0     4452 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/__init__.py
--rw-r--r--   0        0        0     3688 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/currencies.py
--rw-r--r--   0        0        0     1086 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/db.py
--rw-r--r--   0        0        0    18983 2024-05-17 10:42:58.482600 perian_cli-0.1.4/pcli/util/formatter.py
--rw-r--r--   0        0        0      566 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/organization.py
--rw-r--r--   0        0        0    24293 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/rich_utils.py
--rw-r--r--   0        0        0     1185 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/setup.py
--rw-r--r--   0        0        0      633 2024-05-17 12:49:40.140266 perian_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 perian_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1344 2024-05-18 11:57:55.844602 perian_cli-0.1.5/pcli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/api/__init__.py
+-rw-r--r--   0        0        0     3607 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/api/accelerator_type.py
+-rw-r--r--   0        0        0     1452 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/api/billing.py
+-rw-r--r--   0        0        0     3200 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/api/instance_type.py
+-rw-r--r--   0        0        0     3670 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/api/job.py
+-rw-r--r--   0        0        0     1020 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/api/organization.py
+-rw-r--r--   0        0        0     4442 2024-05-19 13:38:57.638874 perian_cli-0.1.5/pcli/cli.py
+-rw-r--r--   0        0        0      133 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/colors.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/commands/__init__.py
+-rw-r--r--   0        0        0     3036 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/commands/accelerator_type.py
+-rw-r--r--   0        0        0     1816 2024-05-18 12:02:07.903485 perian_cli-0.1.5/pcli/commands/billing.py
+-rw-r--r--   0        0        0      344 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/commands/config.py
+-rw-r--r--   0        0        0      898 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/commands/currency.py
+-rw-r--r--   0        0        0     3721 2024-05-19 13:24:57.046228 perian_cli-0.1.5/pcli/commands/instance_type.py
+-rw-r--r--   0        0        0    10158 2024-05-19 13:26:11.102272 perian_cli-0.1.5/pcli/commands/job.py
+-rw-r--r--   0        0        0     4523 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/commands/registry.py
+-rw-r--r--   0        0        0     5758 2024-05-18 12:04:43.782364 perian_cli-0.1.5/pcli/responses.py
+-rw-r--r--   0        0        0      446 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/settings.py
+-rw-r--r--   0        0        0     5175 2024-05-19 13:37:17.971560 perian_cli-0.1.5/pcli/util/__init__.py
+-rw-r--r--   0        0        0     3688 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/util/currencies.py
+-rw-r--r--   0        0        0     1086 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/util/db.py
+-rw-r--r--   0        0        0    19553 2024-05-19 14:49:25.558316 perian_cli-0.1.5/pcli/util/formatter.py
+-rw-r--r--   0        0        0      566 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/util/organization.py
+-rw-r--r--   0        0        0    24293 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/util/rich_utils.py
+-rw-r--r--   0        0        0     1185 2024-05-16 14:06:00.296518 perian_cli-0.1.5/pcli/util/setup.py
+-rw-r--r--   0        0        0      633 2024-05-19 14:50:54.061998 perian_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 perian_cli-0.1.5/PKG-INFO
```

### Comparing `perian_cli-0.1.4/pcli/__init__.py` & `perian_cli-0.1.5/pcli/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from .util.db import DB
-
-db = DB()
+from typing import Callable
 
 from typer.main import TyperCommand, TyperGroup
+from typer.models import CommandFunctionType
 import click
 import rich
 import typer
 
 # overwriting typer default rich utils with perian branding
 from pcli.util import rich_utils as perian_branding
+from .util.db import DB
+
+
+db = DB()
 
 
 class PerianGroup(TyperGroup):
     def format_help(self, ctx: click.Context, formatter: click.HelpFormatter) -> None:
         if not rich:
             return super().format_help(ctx, formatter)
         return perian_branding.rich_format_help(
@@ -33,9 +36,10 @@
         )
 
 
 class PerianTyper(typer.Typer):
     def __init__(self, *args, cls=PerianGroup, **kwargs) -> None:
         super().__init__(*args, cls=cls, **kwargs)
 
-    def command(self, *args, cls=PerianCommand, **kwargs) -> typer.Typer.command:
+    def command(self, *args, cls=PerianCommand, **kwargs
+                ) -> Callable[[CommandFunctionType], CommandFunctionType]:
         return super().command(*args, cls=cls, **kwargs)
```

### Comparing `perian_cli-0.1.4/pcli/api/accelerator_type.py` & `perian_cli-0.1.5/pcli/api/accelerator_type.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/api/billing.py` & `perian_cli-0.1.5/pcli/api/billing.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/api/instance_type.py` & `perian_cli-0.1.5/pcli/api/instance_type.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/api/job.py` & `perian_cli-0.1.5/pcli/api/job.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/api/organization.py` & `perian_cli-0.1.5/pcli/api/organization.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/cli.py` & `perian_cli-0.1.5/pcli/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from time import sleep
-
-import validators
-from rich import print
+from rich import print as rich_print
 from rich.panel import Panel
 from rich.progress import SpinnerColumn, Progress
 from rich.prompt import Prompt, Confirm
 
 from pcli import PerianTyper
 from pcli import db
 from pcli.colors import PERIAN_LIME, PERIAN_PURPLE_LIGHT
@@ -57,34 +54,28 @@
 @handle_exception(InvalidMailException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(AbortedException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(DefaultApiException, exit=True, level=ExceptionLevel.ERROR)
 @handle_exception(OrganizationValidationException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(NoOrganizationException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(AuthenticationFailedException, exit=True, level=ExceptionLevel.WARNING)
 def login():
-    print(
+    rich_print(
         Panel.fit(
             "[bold "
             + PERIAN_PURPLE_LIGHT
             + "] Welcome to the Perian Sky Platform CLI [/bold "
             + PERIAN_PURPLE_LIGHT
             + "] \n\n"
             + MAGNIFYING_GLASS_EMOJI_UNICODE
             + "All login information can be found in your signup e-mail"
         )
     )
-    organization_name = Prompt.ask("Organization name")
-    contact_mail_address = Prompt.ask("Contact E-Mail Address")
+    organization_name = Prompt.ask("Account name")
     access_token = Prompt.ask("Access token")
 
-    if not validators.email(contact_mail_address):
-        raise InvalidMailException(
-            f"The provided e-mail '[bold underline]{contact_mail_address}[/bold underline]' is invalid."
-        )
-
     # getting stored organization data
     organization_data = db.get("organization")
 
     # warn user about override
     if organization_data:
         confirm_override = Confirm.ask(
             "An organization is already logged in and setting up a new one would override the data. Do you confirm?"
@@ -99,34 +90,30 @@
     ) as progress:
         progress.add_task(description="Validating with Sky Platform", total=None)
 
         # validating login information with backend
         perian_organization = get_organization({
             "name": organization_name,
             "token": access_token,
-            "email": contact_mail_address,
         })
 
         valid_name = perian_organization['organization']['name'] == organization_name
-        valid_mail = perian_organization['organization']['contact_email_address'] == contact_mail_address
         valid_token = perian_organization['organization']['access_token'] == access_token
 
-        if not valid_name or not valid_mail or not valid_token:
+        if not valid_name or not valid_token:
             raise OrganizationValidationException()
 
-
     db.set(
         "organization",
         {
             "name": organization_name,
             "token": access_token,
-            "email": contact_mail_address,
         },
     )
-    success(f"Login successful.")
+    success("Login successful.")
 
 
 @pcli.command("logout", rich_help_panel="Account")
 @handle_exception(NoOrganizationException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(AbortedException, exit=True, level=ExceptionLevel.WARNING)
 def logout():
     # getting stored organization data
@@ -138,8 +125,8 @@
     confirm_delete = Confirm.ask("Please confirm logout")
 
     if not confirm_delete:
         raise AbortedException()
 
     # deleting registry from db
     db.set("organization", None)
-    success(f"Logout successful.")
+    success("Logout successful.")
```

### Comparing `perian_cli-0.1.4/pcli/commands/accelerator_type.py` & `perian_cli-0.1.5/pcli/commands/accelerator_type.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/commands/billing.py` & `perian_cli-0.1.5/pcli/commands/billing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 from datetime import datetime, timezone
-from pcli import PerianTyper
 from typing import Annotated
 import typer
-from pcli.api.billing import generate_bill
-from decimal import Decimal
 
-from pcli.responses import DefaultApiException, handle_exception, ExceptionLevel, BillingTimeOrderException, BothBillingTimesNeededException
+from pcli import PerianTyper
+from pcli.api.billing import generate_bill
+from pcli.responses import (
+    BillingTimeOrderException,
+    BothBillingTimesNeededException,
+    DefaultApiException,
+    ExceptionLevel,
+    handle_exception,
+)
 from pcli.util.formatter import print_billing_information
 
 billing_command = PerianTyper(
     no_args_is_help=True,
     rich_markup_mode="rich",
     help="Managed and interact with billing information",
 )
 
 
 @billing_command.command("get", help="Get billing information for a given time")
 @handle_exception(DefaultApiException, exit=True, level=ExceptionLevel.ERROR)
 @handle_exception(BillingTimeOrderException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(BothBillingTimesNeededException, exit=True, level=ExceptionLevel.WARNING)
 def get_bill(
-    start_time: Annotated[datetime, typer.Option(help="Start time for the billing information. Defaults to the beginning of the last month")] = None,
-    end_time: Annotated[datetime, typer.Option(help="End time for the billing information. Defaults to the end of the last month")] = None,
+    start_time: Annotated[datetime, typer.Option(
+        help="Start time for the billing information. Defaults to the beginning of the last month")] = None,
+    end_time: Annotated[datetime, typer.Option(
+        help="End time for the billing information. Defaults to the end of the last month")] = None,
 ):
+    """Get billing information for a given time. If no time is provided, the billing information for the last month is returned."""
     if start_time and not end_time:
         raise BothBillingTimesNeededException()
 
     # adding timezone information to the datetime objects
     if start_time:
         if start_time.tzinfo is None:
             start_time = start_time.replace(tzinfo=timezone.utc)
     if end_time:
         if end_time.tzinfo is None:
             end_time = end_time.replace(tzinfo=timezone.utc)
 
     billing_information = generate_bill(start_time, end_time)
 
-    # adding perian margin to total price
-    billing_information.total_price = str(Decimal(billing_information.total_price) * Decimal(billing_information.margin_multiplier))
-
     print_billing_information(billing_information)
-
```

### Comparing `perian_cli-0.1.4/pcli/commands/currency.py` & `perian_cli-0.1.5/pcli/commands/currency.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/commands/instance_type.py` & `perian_cli-0.1.5/pcli/commands/instance_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Annotated
+from typing import Annotated, Optional
 from typing import Annotated
 from uuid import UUID
 
 import typer
 
 from pcli import PerianTyper
 from pcli.api.instance_type import get_by_id, get_by_requirements
@@ -37,36 +37,33 @@
 
 
 @instance_type_command.command("get", help="Get available instance types")
 @handle_exception(DefaultApiException, exit=True, level=ExceptionLevel.ERROR)
 @handle_exception(InstanceTypeApiException, exit=True, level=ExceptionLevel.ERROR)
 @handle_exception(NoOrganizationException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(InvalidInstanceTypeIdException, exit=True, level=ExceptionLevel.ERROR)
-@handle_exception(
-    InstanceTypeNotFoundException, exit=True, level=ExceptionLevel.WARNING
-)
-@handle_exception(
-    CurrencyAPIException, exit=True, level=ExceptionLevel.ERROR
-)
+@handle_exception(InstanceTypeNotFoundException, exit=True, level=ExceptionLevel.WARNING)
+@handle_exception(CurrencyAPIException, exit=True, level=ExceptionLevel.ERROR)
 @handle_exception(InvalidFilterCriteriaException, exit=True, level=ExceptionLevel.WARNING)
 def get_instance_type(
-    instance_type_id: Annotated[str, typer.Argument(help="ID of instance type")] = None,
-    cores: Annotated[int, typer.Option(help="Number of cpu cores")] = None,
-    memory: Annotated[int, typer.Option(help="Gigabyte of RAM")] = None,
-    accelerators: Annotated[int, typer.Option(help="Number of Accelerators")] = None,
+    instance_type_id: Annotated[Optional[str], typer.Argument(help="ID of instance type")] = None,
+    cores: Annotated[Optional[int], typer.Option(help="Number of cpu cores")] = None,
+    memory: Annotated[Optional[int], typer.Option(help="Gigabyte of RAM")] = None,
+    accelerators: Annotated[Optional[int], typer.Option(help="Number of Accelerators")] = None,
     accelerator_type: Annotated[
-        str,
+        Optional[str],
         typer.Option(
-            help="Name of accelerator type. See accelerator-type command for a list of all supported ones."
+            help="Name of accelerator type. See accelerator-type command for a list of all supported ones"
         ),
     ] = None,
+    country_code: Annotated[Optional[str], typer.Option(help="Country code (e.g. DE)")] = None,
     filters: Annotated[
-        str,
+        Optional[str],
         typer.Option(
-            help="Filter criteria to select instance types. A JSON string or the path to a JSON file is expected here."
+            help="Filter criteria to select instance types. A JSON string or the path to a JSON file is expected here"
         ),
     ] = None,
     limit: Annotated[
         int, typer.Option(help="Number of instance types to display")
     ] = 25,
 ):
     if instance_type_id:
@@ -85,14 +82,15 @@
             instance_type_filters = load_instance_type_filter_from_json(filters)
         else:
             instance_type_filters = load_instance_type_filter_from_values(
                 cores=cores,
                 memory=memory,
                 accelerators=accelerators,
                 accelerator_type=accelerator_type,
+                country_code=country_code,
             )
 
         # creating instance type query
         instance_type_query = InstanceTyperQueryView(**instance_type_filters)
 
         # calling API
         instance_types = get_by_requirements(instance_type_query, limit)
```

### Comparing `perian_cli-0.1.4/pcli/commands/job.py` & `perian_cli-0.1.5/pcli/commands/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,41 +7,45 @@
 
 from pcli import PerianTyper
 from pcli.api.instance_type import get_by_id as get_instance_type_by_id, \
     get_by_requirements as get_instance_type_by_requirements
 from pcli.api.job import get_by_id as get_job_by_id, get_all, cancel_job, create_job as api_create_job
 from pcli.colors import PERIAN_PURPLE_LIGHT
 from pcli.responses import (
+    InstanceTypeApiException,
+    InvalidFilterCriteriaException,
     handle_exception,
     ExceptionLevel,
     JobNotFoundException,
     DefaultApiException,
     JobAPIException,
     InvalidJobIdException,
     NoOrganizationException,
     success,
     JobAlreadyDoneException,
     InvalidJobManifestException,
     InvalidParametersException,
     InvalidInstanceTypeIdException,
-    InsufficientQuotaException
+    InsufficientQuotaException,
+    InstanceTypeNotFoundException
 )
 from pcli.util import load_instance_type_filter_from_values, load_job_manifest_from_json
 from pcli.util.formatter import print_jobs_list, print_job_description, format_instance_type_query
 from perian import InstanceTyperQueryView, CreateJobRequest
 from pcli import db
 from urllib.parse import urlparse
 from perian.models import DockerRegistryCredentials
 
 job_command = PerianTyper(
     no_args_is_help=True,
     rich_markup_mode="rich",
     help="Create and manage jobs"
 )
 
+
 def _parse_container_image_name(image_name) -> (str, Optional[str]):
     if not ":" in image_name:
         return image_name, None
     else:
         split_image = image_name.split(":")
         return split_image[0], split_image[1]
 
@@ -50,18 +54,20 @@
     if not "instance_type_id" in job_description:
         raise InvalidInstanceTypeIdException()
 
     if not "docker_run_parameters" in job_description or not "image_name" in job_description["docker_run_parameters"]:
         raise InvalidParametersException("Please provide a valid container image name.")
 
     if "requirements" in job_description:
-        job_description["requirements"] = format_instance_type_query(job_description["requirements"])
+        job_description["requirements"] = format_instance_type_query(
+            job_description["requirements"])
 
     return job_description
 
+
 def _inject_stored_registry(job_description: dict):
     # getting already stored registry data
     registry_data = db.get("registry")
 
     image_url = urlparse("https://" + job_description["docker_run_parameters"]["image_name"])
 
     if registry_data:
@@ -74,30 +80,34 @@
                     username=registry_data[registry_name]['username'],
                     password=registry_data[registry_name]['password']
                 )
     return job_description
 
 
 @job_command.command("create", help="Create a job")
+@handle_exception(DefaultApiException, exit=True, level=ExceptionLevel.ERROR)
+@handle_exception(InstanceTypeApiException, exit=True, level=ExceptionLevel.ERROR)
+@handle_exception(InstanceTypeNotFoundException, exit=True, level=ExceptionLevel.WARNING)
+@handle_exception(InsufficientQuotaException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(InvalidJobManifestException, exit=True, level=ExceptionLevel.WARNING)
+@handle_exception(InvalidFilterCriteriaException, exit=True, level=ExceptionLevel.WARNING)
+@handle_exception(InvalidInstanceTypeIdException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(InvalidParametersException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(JobAPIException, exit=True, level=ExceptionLevel.ERROR)
-@handle_exception(DefaultApiException, exit=True, level=ExceptionLevel.ERROR)
-@handle_exception(InvalidInstanceTypeIdException, exit=True, level=ExceptionLevel.WARNING)
-@handle_exception(InsufficientQuotaException, exit=True, level=ExceptionLevel.WARNING)
 def create_job(
-        image: Annotated[str, typer.Option(help="Container image name")] = None,
-        instance_type_id: Annotated[str, typer.Option(help="ID of instance type")] = None,
-        cores: Annotated[int, typer.Option(help="Number of cpu cores")] = None,
-        memory: Annotated[int, typer.Option(help="Gigabyte of RAM")] = None,
-        accelerators: Annotated[int, typer.Option(help="Number of Accelerators")] = None,
-        accelerator_type: Annotated[str, typer.Option(
-            help="Name of accelerator type. See accelerator-type command for a list of all supported ones.")] = None,
-        manifest: Annotated[str, typer.Option(
-            help="Job description manifest. A JSON string or the path to a JSON file is expected here.")] = None,
+        image: Annotated[Optional[str], typer.Option(help="Container image name")] = None,
+        instance_type_id: Annotated[Optional[str], typer.Option(help="ID of instance type")] = None,
+        cores: Annotated[Optional[int], typer.Option(help="Number of cpu cores")] = None,
+        memory: Annotated[Optional[int], typer.Option(help="Gigabyte of RAM")] = None,
+        accelerators: Annotated[Optional[int], typer.Option(help="Number of Accelerators")] = None,
+        accelerator_type: Annotated[Optional[str], typer.Option(
+            help="Name of accelerator type. See accelerator-type command for a list of all supported ones")] = None,
+        country_code: Annotated[Optional[str], typer.Option(help="Country code (e.g. DE)")] = None,
+        manifest: Annotated[Optional[str], typer.Option(
+            help="Job description manifest. A JSON string or the path to a JSON file is expected here")] = None,
 ):
     job_description = {}
 
     with (Progress(SpinnerColumn(style=PERIAN_PURPLE_LIGHT), TextColumn("[progress.description]{task.description}"), transient=True) as progress):
         # we can load the entire job description from file
         if manifest:
             job_description = load_job_manifest_from_json(manifest)
@@ -109,65 +119,71 @@
             _image_name, _tag = _parse_container_image_name(image)
             job_description['docker_run_parameters'] = {
                 "image_name": _image_name
             }
             if _tag:
                 job_description['docker_run_parameters']['image_tag'] = _tag
 
-            # handling instance type filter
-            if cores or memory or accelerators or accelerator_type:
-                instance_type_filters = load_instance_type_filter_from_values(
-                    cores=cores,
-                    memory=memory,
-                    accelerators=accelerators,
-                    accelerator_type=accelerator_type
-                )
-
-                # storing filters for later usage
-                job_description['requirements'] = instance_type_filters
-
             # handling instance type for job
             # user has provided a specific instance type id
             if instance_type_id:
                 try:
                     instance_type_id = UUID(instance_type_id)
                 except Exception:
                     raise InvalidInstanceTypeIdException()
                 job_description['instance_type_id'] = str(instance_type_id)
 
             # no specific instance type id, we need to find a suitable one first
             else:
-                selecting_instance_type_task = progress.add_task(description="Selecting optimal instance type",
-                                                                 total=None)
+                instance_type_filters = load_instance_type_filter_from_values(
+                    cores=cores,
+                    memory=memory,
+                    accelerators=accelerators,
+                    accelerator_type=accelerator_type,
+                    country_code=country_code,
+                )
+
+                # storing filters for later usage
+                job_description['requirements'] = instance_type_filters
+
+                selecting_instance_type_task = progress.add_task(
+                    description="Selecting optimal instance type", total=None)
 
                 # creating instance type query
                 instance_type_query = InstanceTyperQueryView(**instance_type_filters)
+
+                # querying for instance type
                 instance_types = get_instance_type_by_requirements(instance_type_query, 1)
+                if len(instance_types) == 0:
+                    raise InstanceTypeNotFoundException()
+
                 job_description['instance_type_id'] = instance_types[0].id
 
                 # this is just for the user experience and the progress spinner
                 time.sleep(0.3)
                 progress.remove_task(selecting_instance_type_task)
 
         # validating input before calling API
         job_description = _validate_job_description(job_description)
 
         # inject private registry previously saved via the CLI
         job_description = _inject_stored_registry(job_description)
 
         # creating job request and calling API
-        create_job_task = progress.add_task(description="Submitting job to Sky Platform", total=None)
+        create_job_task = progress.add_task(
+            description="Submitting job to Sky Platform", total=None)
         create_job_request = CreateJobRequest(**job_description)
         created_job = api_create_job(create_job_request)
 
         # this is just for the user experience and the progress spinner
         time.sleep(0.3)
         progress.remove_task(create_job_task)
 
-        success(f"Job with ID '[bold underline]{created_job.id}[/bold underline]' created successfully.")
+        success(
+            f"Job with ID '[bold underline]{created_job.id}[/bold underline]' created successfully.")
 
 
 @job_command.command("get", help="Get details about jobs")
 @handle_exception(JobNotFoundException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(DefaultApiException, exit=True, level=ExceptionLevel.ERROR)
 @handle_exception(JobAPIException, exit=True, level=ExceptionLevel.ERROR)
 @handle_exception(InvalidJobIdException, exit=True, level=ExceptionLevel.WARNING)
@@ -197,15 +213,16 @@
         jobs = get_all()
 
         if len(jobs) == 0:
             raise JobNotFoundException("No jobs found for your account.")
 
         print_jobs_list(jobs)
     else:
-        raise InvalidParametersException("Please provide a job ID or use '-all' option to get all jobs.")
+        raise InvalidParametersException(
+            "Please provide a job ID or use '-all' option to get all jobs.")
 
 
 @job_command.command("cancel", help="Cancel a job")
 @handle_exception(DefaultApiException, exit=True, level=ExceptionLevel.ERROR)
 @handle_exception(JobAPIException, exit=True, level=ExceptionLevel.ERROR)
 @handle_exception(InvalidJobIdException, exit=True, level=ExceptionLevel.WARNING)
 @handle_exception(JobAlreadyDoneException, exit=True, level=ExceptionLevel.WARNING)
```

### Comparing `perian_cli-0.1.4/pcli/commands/registry.py` & `perian_cli-0.1.5/pcli/commands/registry.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/responses.py` & `perian_cli-0.1.5/pcli/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pcli.colors import PERIAN_LIME, PERIAN_PURPLE_LIGHT
 
 CHECKMARK_EMOJI_UNICODE = "[green bold] :heavy_check_mark: [/green bold]"
 WARNING_EMOJI_UNICODE = ""
 CROSS_EMOJI_UNICODE = ""
 MAGNIFYING_GLASS_EMOJI_UNICODE = "\U0001F50D "
 
+
 class ExceptionLevel(str, Enum):
     ERROR = "Error"
     WARNING = "Warning"
     INFO = "Info"
 
 
 class DefaultException(Exception):
@@ -159,15 +160,15 @@
 
 
 class BillingTimeOrderException(DefaultException):
     detail: str = "Start date of billing time must be before end date. Please check the provided dates."
 
 
 class BothBillingTimesNeededException(DefaultException):
-    detail: str = "If you provide a start time for the billing period you must specify a end time as well."
+    detail: str = "If you provide a start time for the billing period you must specify an end time as well."
 
 
 class OrganizationValidationException(DefaultException):
     detail: str = "Account validation failed. Please check your login and account data."
 
 
 class AuthenticationFailedException(DefaultException):
```

### Comparing `perian_cli-0.1.4/pcli/util/__init__.py` & `perian_cli-0.1.5/pcli/util/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import os
 from json import JSONDecodeError
+from typing import Any, Dict, Optional
 
 import requests
 from requests.adapters import HTTPAdapter, Retry
 from requests.models import Response
 
 from pcli.responses import InvalidFilterCriteriaException, InvalidJobManifestException
 from pcli.util.formatter import (
@@ -48,20 +49,22 @@
     except JSONDecodeError:
         raise InvalidFilterCriteriaException(
             "Failed to load JSON file. The JSON seems to be malformed."
         )
 
 
 def load_instance_type_filter_from_values(
-    cores: int = None,
-    memory: int = None,
-    accelerators: int = None,
-    accelerator_type: str = None,
+    cores: Optional[int] = None,
+    memory: Optional[int] = None,
+    accelerators: Optional[int] = None,
+    accelerator_type: Optional[str] = None,
+    country_code: Optional[str] = None,
 ):
-    instance_type_filters = {}
+    """Create a filter query for instance types based on the provided values."""
+    instance_type_filters: Dict[str, Any] = {}
 
     if cores:
         instance_type_filters["cpu"] = {"cores": cores}
 
     if memory:
         instance_type_filters["ram"] = {"size": memory}
 
@@ -72,22 +75,35 @@
         if "accelerator" in instance_type_filters:
             instance_type_filters["accelerator"]["name"] = Name(accelerator_type)
         else:
             instance_type_filters["accelerator"] = {
                 "name": Name(accelerator_type)
             }
 
+    if country_code:
+        country_code = validate_and_format_country_code(country_code)
+        instance_type_filters["region"] = {"location": country_code}
+
     if len(instance_type_filters) == 0:
         raise InvalidFilterCriteriaException(
             "No valid filter criteria were provided. Please adjust your criteria."
         )
 
     return format_instance_type_query(instance_type_filters)
 
 
+def validate_and_format_country_code(country_code: str) -> str:
+    """Validate and convert the provided country code to uppercase."""
+    if len(country_code) != 2:
+        raise InvalidFilterCriteriaException(
+            "Invalid country code. Please provide a valid two-letter country code. (e.g. DE)"
+        )
+    return country_code.upper()
+
+
 def load_job_manifest_from_json(filters):
     job_manifest = None
     try:
         if ".json" in filters:
             full_path = os.path.join(os.path.dirname(__file__), filters)
 
             # the provided json file could be locally or provided as a full path
@@ -130,19 +146,15 @@
         raise InvalidFilterCriteriaException(
             "No valid filter criteria were provided. Please adjust your criteria."
         )
 
     return format_accelerator_type_query(accelerator_type_filters)
 
 
-
 def get_with_retry(url: str) -> Response:
     """Get a URL with retries on 5xx errors."""
     session = requests.Session()
     retries = Retry(total=5,
                     backoff_factor=0.1,
                     status_forcelist=[500, 502, 503, 504])
     session.mount(url, HTTPAdapter(max_retries=retries))
     return session.get(url)
-
-
-
```

### Comparing `perian_cli-0.1.4/pcli/util/currencies.py` & `perian_cli-0.1.5/pcli/util/currencies.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/util/db.py` & `perian_cli-0.1.5/pcli/util/db.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/util/formatter.py` & `perian_cli-0.1.5/pcli/util/formatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,57 @@
-import datetime
-from typing import Union
+from datetime import datetime
+from decimal import Decimal, getcontext
+from typing import List, Optional, Union
+
+from perian.models import (
+    BillingGranularity,
+    Currency,
+    InboundSpeed,
+    Name,
+    OutboundSpeed,
+    Size,
+    Speed,
+    UnitPrice,
+)
+from perian.models.job_status import JobStatus
+from perian.models.job_view import JobView
 from rich import box
 from rich import print as rprint
 from rich.columns import Columns
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 
 from pcli.colors import PERIAN_PURPLE_LIGHT, PERIAN_LIME
 from pcli.responses import CHECKMARK_EMOJI_UNICODE
-from perian.models import Speed, Size, InboundSpeed, OutboundSpeed, UnitPrice, BillingGranularity
-from perian.models.job_status import JobStatus
-from decimal import Decimal, getcontext
-from perian.models import Currency, BillingGranularity, Name
 from pcli.settings import cli_settings
 
 
 def _format_zone_name(zone_name: str):
     """Formats a provider zone name to a nice string. Especially for default zones."""
     if "DEFAULT" in zone_name:
         return "Default"
 
     return zone_name
 
+
 def _format_billing_granularity(billing_granularity: BillingGranularity):
     """Formats a billing granularity to a human-readable string."""
     if billing_granularity == BillingGranularity.PER_SECOND:
         return "Per Second"
     elif billing_granularity == BillingGranularity.PER_MINUTE:
         return "Per Minute"
     elif billing_granularity == BillingGranularity.PER_HOUR:
         return "Per Hour"
     elif billing_granularity == BillingGranularity.PER_10_MINUTES:
         return "Per 10 Minutes"
     else:
         return "Undefined"
 
+
 def _format_decimal(value: Union[Decimal, str], places: int = 3):
     """Formats a value that can either be a decimal or a string to a decimal with two decimal places that are not rounded."""
     # converting to decimal if the value is a string
     if type(value) is str:
         value = Decimal(value)
 
     # Setting the context precision high enough to handle the input
@@ -84,22 +96,31 @@
             + "[/bold "
             + PERIAN_LIME
             + " ]"
         )
     else:
         return str(status.value)
 
+
 def _get_currency_symbol(currency: Currency):
     if currency == Currency.EUR:
         return "€"
     elif currency == Currency.USD:
         return "$"
     if currency == Currency.CHF:
         return "CHF"
 
+
+def _format_datetime(dt: Optional[datetime]) -> str:
+    """Formats a datetime object to a string."""
+    if dt:
+        return dt.strftime("%d-%m-%Y %H:%M:%S %Z")
+    return "-"
+
+
 def print_instance_types_list(instance_types):
     table = Table(box=box.SIMPLE, safe_box=True)
 
     columns = [
         "ID",
         "Name",
         "Provider",
@@ -150,15 +171,16 @@
     no_accelerators = "-"
     accelerator_type = "-"
     total_accelerator_memory = "-"
 
     if instance_type.accelerator.no > 0:
         no_accelerators = str(instance_type.accelerator.no)
         accelerator_type = instance_type.accelerator.accelerator_types[0].display_name
-        total_accelerator_memory = str(_format_decimal(instance_type.accelerator.memory.size, 2)) + " GB"
+        total_accelerator_memory = str(_format_decimal(
+            instance_type.accelerator.memory.size, 2)) + " GB"
 
     if not as_panel:
         table = Table(box=box.SIMPLE)
 
         columns = [
             "CPU Cores",
             "RAM",
@@ -184,38 +206,39 @@
         console = Console()
         console.print(table)
 
     elif as_panel:
         Console().print(
             Panel.fit(
                 ("[bold underline]"
-                + "Instance Type"
-                + "[/bold underline]" if with_general_information else "")
+                 + "Instance Type"
+                 + "[/bold underline]" if with_general_information else "")
                 + ("[bold underline]"
-                 + "Hardware Profile"
-                 + "[/bold underline]" if not with_general_information else "")
+                   + "Hardware Profile"
+                   + "[/bold underline]" if not with_general_information else "")
                 + "\n\n"
                 + ("ID: "
-                + instance_type.id
-                + " \n"
-                + "Name: "
-                + instance_type.name
-                + " \n"
-                + "Type: "
-                + instance_type.type
-                + "\n\n"
-                + "Provider: "
-                + instance_type.provider.name
-                + " \n"
-                + "Region: "
-                + str(instance_type.region.location.value) + " (" + str(instance_type.region.city) + ")"
-                + " \n"
-                + "Availability Zone: "
-                + _format_zone_name(instance_type.zone.name)
-                + "\n\n" if with_general_information else "")
+                   + instance_type.id
+                   + " \n"
+                   + "Name: "
+                   + instance_type.name
+                   + " \n"
+                   + "Type: "
+                   + instance_type.type
+                   + "\n\n"
+                   + "Provider: "
+                   + instance_type.provider.name
+                   + " \n"
+                   + "Region: "
+                   + str(instance_type.region.location.value) +
+                   " (" + str(instance_type.region.city) + ")"
+                   + " \n"
+                   + "Availability Zone: "
+                   + _format_zone_name(instance_type.zone.name)
+                   + "\n\n" if with_general_information else "")
                 + "CPU Cores: "
                 + str(instance_type.cpu.cores)
                 + "\n"
                 + "RAM: "
                 + str(_format_decimal(instance_type.ram.size, 2))
                 + "\n"
                 + "No of Accelerators: "
@@ -275,33 +298,36 @@
             + " " + _get_currency_symbol(cli_settings.base_currency) + " \n"
             + "Billing Period: "
             + _format_billing_granularity(cli_settings.billing_granularity)
             + " \n"
         )
     )
     Console().print(Columns(first_section))
-    print_instance_type_hardware_profile(instance_type, as_panel=True, with_general_information=False)
+    print_instance_type_hardware_profile(
+        instance_type, as_panel=True, with_general_information=False)
 
 
-def print_jobs_list(jobs: list):
+def print_jobs_list(jobs: List[JobView]):
     table = Table(box=box.SIMPLE)
 
-    columns = ["ID", "Status", "Start Time", "Container Image"]
+    columns = ["ID", "Status", "Create Time", "Start Time", "End Time", "Container Image"]
 
     for column in columns:
         if column == "ID":
             table.add_column(column, no_wrap=True)
         else:
             table.add_column(column)
 
     for job in jobs:
         table.add_row(
             str(job.id),
             _format_job_status(job.status, only_positive=True),
-            str(job.started_at.strftime("%d-%m-%Y %H:%M:%S")) if job.started_at else "-",
+            _format_datetime(job.created_at),
+            _format_datetime(job.started_at),
+            _format_datetime(job.done_at),
             str(job.docker_metadata.docker_run_parameters.image_name),
         )
 
     console = Console()
     console.print(table)
 
 
@@ -315,16 +341,22 @@
             + "\n\n"
             + "Status: "
             + _format_job_status(job.status)
             + " \n"
             + "ID: "
             + str(job.id)
             + " \n"
+            + "Create Time: "
+            + _format_datetime(job.created_at)
+            + " \n"
             + "Start Time: "
-            + (str(job.started_at.strftime("%d-%m-%Y %H:%M:%S")) if job.started_at else "-")
+            + _format_datetime(job.started_at)
+            + " \n"
+            + "End Time: "
+            + _format_datetime(job.done_at)
         )
     )
 
     first_section.append(
         Panel.fit(
             "[bold underline]"
             + "Workload"
@@ -417,15 +449,16 @@
         if "per_hour" in instance_type_query["price"]:
             instance_type_query["price"]["per_hour"] = BillingGranularity(
                 str(instance_type_query["price"]["per_hour"])
             )
 
     if "accelerator" in instance_type_query:
         if "name" in instance_type_query['accelerator']:
-            instance_type_query['accelerator']['name'] = Name(instance_type_query['accelerator']['name'])
+            instance_type_query['accelerator']['name'] = Name(
+                instance_type_query['accelerator']['name'])
 
     return instance_type_query
 
 
 def format_accelerator_type_query(accelerator_type_query):
     if "memory" in accelerator_type_query:
         accelerator_type_query["memory"]["size"] = Size(
@@ -482,19 +515,18 @@
     columns = ["ID", "Name", "Vendor", "Memory (GB)"]
 
     for column in columns:
         if column == "ID":
             table.add_column(column, no_wrap=True)
         else:
             table.add_column(column)
-
     for accelerator_type in accelerator_types:
         table.add_row(
             str(accelerator_type.id),
-            _colorize_text(str(accelerator_type.display_name), PERIAN_PURPLE_LIGHT, "bold"),
+            _colorize_text(str(accelerator_type.name.value), PERIAN_PURPLE_LIGHT, "bold"),
             str(accelerator_type.vendor.value),
             str(_format_decimal(accelerator_type.memory.size, 2)),
         )
 
     console = Console()
     console.print(table)
 
@@ -521,21 +553,21 @@
 
 def print_registry_list(registries: dict):
     registry_table = Table(box=box.SIMPLE)
     registry_table.add_column("Registry Name")
     registry_table.add_column("Creation Time")
 
     for registry in registries:
-        creation_time = datetime.datetime.strptime(
+        creation_time = datetime.strptime(
             registries[registry]["created"], "%Y-%m-%d %H:%M:%S.%f"
         )
 
         registry_table.add_row(
             _colorize_text(registry, PERIAN_PURPLE_LIGHT, "bold"),
-            str(creation_time.strftime("%d-%m-%Y %H:%M:%S")),
+            _format_datetime(creation_time),
         )
 
     console = Console()
     console.print(registry_table)
 
 
 def print_currency_description(currency: Currency):
@@ -546,15 +578,14 @@
             + "[/bold underline]" +
             "\n\n" +
             str(currency.value)
         )
     )
 
 
-
 def print_billing_items_list(billing_items: list, limit: int = 25):
     display_overhang = False
     initial_length = 0
 
     table = Table(box=box.SIMPLE)
 
     columns = ["Job ID", "Price"]
@@ -569,41 +600,42 @@
         display_overhang = True
         initial_length = len(billing_items)
         billing_items = billing_items[:limit]
 
     for billing_item in billing_items:
         table.add_row(
             str(billing_item.job_id),
-            _format_decimal(billing_item.price)
+            _format_decimal(billing_item.price, 2)
         )
 
     if display_overhang:
         table.add_row(str(initial_length - limit) + " more ...", "")
 
     console = Console()
     console.print(table)
 
+
 def print_billing_information(billing_information):
     Console().print(
         Panel.fit(
             "[bold underline]"
             + "Billing Information"
             + "[/bold underline]" +
             "\n\n"
 
             + "Start Time: "
-            + billing_information.start_time.strftime("%d-%m-%Y %H:%M:%S")
+            + _format_datetime(billing_information.start_time)
             + "\n"
             + "End Time: "
-            + billing_information.end_time.strftime("%d-%m-%Y %H:%M:%S")
+            + _format_datetime(billing_information.end_time)
             + "\n\n"
             + "Total Amount: "
-            + _colorize_text(str(_format_decimal(billing_information.total_price)), PERIAN_PURPLE_LIGHT, "bold")
+            + _colorize_text(str(_format_decimal(billing_information.total_price, 2)),
+                             PERIAN_PURPLE_LIGHT, "bold")
             + " "
             + _get_currency_symbol(billing_information.currency)
         )
     )
 
     # displaying billing items
     if len(billing_information.items) > 0:
         print_billing_items_list(billing_information.items)
-
```

### Comparing `perian_cli-0.1.4/pcli/util/organization.py` & `perian_cli-0.1.5/pcli/util/organization.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/util/rich_utils.py` & `perian_cli-0.1.5/pcli/util/rich_utils.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pcli/util/setup.py` & `perian_cli-0.1.5/pcli/util/setup.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.4/pyproject.toml` & `perian_cli-0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perian-cli"
-version = "0.1.4"
+version = "0.1.5"
 description = "Perian Sky Platform CLI"
 authors = ["Perian <info@perian.io>"]
 homepage = "https://perian.io"
 documentation = "https://perian.io"
 packages = [{include = "pcli"}]
 
 [tool.poetry.scripts]
@@ -14,15 +14,15 @@
 python = "^3.10"
 typer = "0.12.3"
 validators = "0.28.1"
 pydantic = "2.7.0"
 click = "8.1.7"
 rich = "13.7.1"
 toml = "0.10.2"
-perian = "0.2.1"
+perian = "0.2.2"
 requests = "2.31.0"
 pydantic-settings = "2.2.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
```

### Comparing `perian_cli-0.1.4/PKG-INFO` & `perian_cli-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: perian-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Perian Sky Platform CLI
 Home-page: https://perian.io
 Author: Perian
 Author-email: info@perian.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (==8.1.7)
-Requires-Dist: perian (==0.2.1)
+Requires-Dist: perian (==0.2.2)
 Requires-Dist: pydantic (==2.7.0)
 Requires-Dist: pydantic-settings (==2.2.1)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rich (==13.7.1)
 Requires-Dist: toml (==0.10.2)
 Requires-Dist: typer (==0.12.3)
 Requires-Dist: validators (==0.28.1)
```

