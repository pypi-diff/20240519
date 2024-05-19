# Comparing `tmp/iec_api-0.2.8.tar.gz` & `tmp/iec_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iec_api-0.2.8.tar", max compression
+gzip compressed data, was "iec_api-0.3.0.tar", max compression
```

## Comparing `iec_api-0.2.8.tar` & `iec_api-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,41 @@
--rw-r--r--   0        0        0     1071 2024-03-05 13:13:52.455421 iec_api-0.2.8/LICENSE
--rw-r--r--   0        0        0      599 2024-03-05 13:13:52.455421 iec_api-0.2.8/README.md
--rw-r--r--   0        0        0        0 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/__init__.py
--rw-r--r--   0        0        0     6580 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/commons.py
--rw-r--r--   0        0        0     2024 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/const.py
--rw-r--r--   0        0        0     7729 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/data.py
--rw-r--r--   0        0        0    15414 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/iec_client.py
--rw-r--r--   0        0        0     8500 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/login.py
--rw-r--r--   0        0        0     1287 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/account.py
--rw-r--r--   0        0        0     2724 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/contract.py
--rw-r--r--   0        0        0     2157 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/customer.py
--rw-r--r--   0        0        0     2951 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/device.py
--rw-r--r--   0        0        0     1994 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/device_type.py
--rw-r--r--   0        0        0     1768 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/electric_bill.py
--rw-r--r--   0        0        0      639 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/exceptions.py
--rw-r--r--   0        0        0     4153 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/invoice.py
--rw-r--r--   0        0        0      265 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/jwt.py
--rw-r--r--   0        0        0     2532 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/meter_reading.py
--rw-r--r--   0        0        0      658 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/okta_errors.py
--rw-r--r--   0        0        0     3600 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/remote_reading.py
--rw-r--r--   0        0        0      971 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/response_descriptor.py
--rw-r--r--   0        0        0     1068 2024-03-05 13:13:52.455421 iec_api-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 iec_api-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-19 08:41:23.131713 iec_api-0.3.0/LICENSE
+-rw-r--r--   0        0        0      697 2024-05-19 08:41:23.131713 iec_api-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/__init__.py
+-rw-r--r--   0        0        0     8218 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/commons.py
+-rw-r--r--   0        0        0     2806 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/const.py
+-rw-r--r--   0        0        0    12026 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/data.py
+-rw-r--r--   0        0        0     1381 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/fault_portal_data.py
+-rw-r--r--   0        0        0      403 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/fault_portal_models/fault_portal_base.py
+-rw-r--r--   0        0        0     6048 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/fault_portal_models/outages.py
+-rw-r--r--   0        0        0     2627 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/fault_portal_models/user_profile.py
+-rw-r--r--   0        0        0    21447 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/iec_client.py
+-rw-r--r--   0        0        0     8527 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/login.py
+-rw-r--r--   0        0        0     1310 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/account.py
+-rw-r--r--   0        0        0     2724 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/contract.py
+-rw-r--r--   0        0        0     2312 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/contract_check.py
+-rw-r--r--   0        0        0     2173 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/customer.py
+-rw-r--r--   0        0        0     2951 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/device.py
+-rw-r--r--   0        0        0     1944 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/device_identity.py
+-rw-r--r--   0        0        0     1994 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/device_type.py
+-rw-r--r--   0        0        0     3016 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/efs.py
+-rw-r--r--   0        0        0     1768 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/electric_bill.py
+-rw-r--r--   0        0        0      528 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/error_response.py
+-rw-r--r--   0        0        0      639 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/exceptions.py
+-rw-r--r--   0        0        0      526 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/get_pdf.py
+-rw-r--r--   0        0        0     4280 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/invoice.py
+-rw-r--r--   0        0        0      265 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/jwt.py
+-rw-r--r--   0        0        0     2530 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/meter_reading.py
+-rw-r--r--   0        0        0      670 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/models_commons.py
+-rw-r--r--   0        0        0      658 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/okta_errors.py
+-rw-r--r--   0        0        0     6261 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/outages.py
+-rw-r--r--   0        0        0     3761 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/remote_reading.py
+-rw-r--r--   0        0        0      981 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/models/response_descriptor.py
+-rw-r--r--   0        0        0      536 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/static_data.py
+-rw-r--r--   0        0        0        0 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/usage_calculator/__init__.py
+-rw-r--r--   0        0        0     3291 2024-05-19 08:41:23.131713 iec_api-0.3.0/iec_api/usage_calculator/calculator.py
+-rw-r--r--   0        0        0      345 2024-05-19 08:41:23.135713 iec_api-0.3.0/iec_api/usage_calculator/consumption.py
+-rw-r--r--   0        0        0      908 2024-05-19 08:41:23.135713 iec_api-0.3.0/iec_api/usage_calculator/electric_device.py
+-rw-r--r--   0        0        0      518 2024-05-19 08:41:23.135713 iec_api-0.3.0/iec_api/usage_calculator/get_calculator_response.py
+-rw-r--r--   0        0        0      535 2024-05-19 08:41:23.135713 iec_api-0.3.0/iec_api/usage_calculator/rates.py
+-rw-r--r--   0        0        0     1050 2024-05-19 08:41:23.135713 iec_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 iec_api-0.3.0/PKG-INFO
```

### Comparing `iec_api-0.2.8/LICENSE` & `iec_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.8/iec_api/commons.py` & `iec_api-0.3.0/iec_api/commons.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import asyncio
 import http
+import logging
 import re
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from json import JSONDecodeError
 from typing import Any, Optional
 
+import aiohttp
 import pytz
-from aiohttp import ClientError, ClientResponse, ClientSession
-from loguru import logger
+from aiohttp import ClientError, ClientResponse, ClientSession, StreamReader
 
-from iec_api.const import TIMEZONE
+from iec_api.const import ERROR_FIELD_NAME, ERROR_SUMMARY_FIELD_NAME, TIMEZONE
+from iec_api.models.error_response import IecErrorResponse
 from iec_api.models.exceptions import IECError, IECLoginError
 from iec_api.models.okta_errors import OktaError
 from iec_api.models.response_descriptor import RESPONSE_DESCRIPTOR_FIELD, ErrorResponseDescriptor
 
+logger = logging.getLogger(__name__)
+
 
 def add_auth_bearer_to_headers(headers: dict[str, str], token: str) -> dict[str, str]:
     """
     Add JWT bearer token to the Authorization header.
     Args:
     headers (dict): The headers dictionary to be modified.
     token (str): The JWT token to be added to the headers.
@@ -77,15 +81,18 @@
     A function to parse error responses from IEC or Okta Server
     """
     logger.warning(f"Failed call: (Code {resp.status}): {resp.reason}")
     if len(json_resp) > 0:
         if json_resp.get(RESPONSE_DESCRIPTOR_FIELD) is not None:
             login_error_response = ErrorResponseDescriptor.from_dict(json_resp.get(RESPONSE_DESCRIPTOR_FIELD))
             raise IECError(login_error_response.code, login_error_response.error)
-        elif json_resp.get("errorSummary") is not None:
+        elif json_resp.get(ERROR_FIELD_NAME) is not None:
+            error_response = IecErrorResponse.from_dict(json_resp)
+            raise IECError(error_response.code, error_response.error)
+        elif json_resp.get(ERROR_SUMMARY_FIELD_NAME) is not None:
             login_error_response = OktaError.from_dict(json_resp)
             raise IECLoginError(resp.status, resp.reason + ": " + login_error_response.error_summary)
     raise IECError(resp.status, resp.reason)
 
 
 async def send_get_request(
     session: ClientSession, url: str, timeout: Optional[int] = 60, headers: Optional[dict] = None
@@ -93,25 +100,23 @@
     try:
         if not headers:
             headers = session.headers
 
         if not timeout:
             timeout = session.timeout
 
-        logger.debug(f"HTTP GET: {url}")
         resp = await session.get(url=url, headers=headers, timeout=timeout)
         json_resp: dict = await resp.json(content_type=None)
     except TimeoutError as ex:
         raise IECError(-1, f"Failed to communicate with IEC API due to time out: ({str(ex)})")
     except ClientError as ex:
         raise IECError(-1, f"Failed to communicate with IEC API due to ClientError: ({str(ex)})")
     except JSONDecodeError as ex:
         raise IECError(-1, f"Received invalid response from IEC API: {str(ex)}")
 
-    logger.debug(f"HTTP GET Response: {json_resp}")
     if resp.status != http.HTTPStatus.OK:
         parse_error_response(resp, json_resp)
 
     return json_resp
 
 
 async def send_non_json_get_request(
@@ -124,28 +129,23 @@
     try:
         if not headers:
             headers = session.headers
 
         if not timeout:
             timeout = session.timeout
 
-        logger.debug(
-            f"HTTP GET: {url}",
-        )
         resp = await session.get(url=url, headers=headers, timeout=timeout)
         resp_content = await resp.text(encoding=encoding)
     except TimeoutError as ex:
         raise IECError(-1, f"Failed to communicate with IEC API due to time out: ({str(ex)})")
     except ClientError as ex:
         raise IECError(-1, f"Failed to communicate with IEC API due to ClientError: ({str(ex)})")
     except JSONDecodeError as ex:
         raise IECError(-1, f"Received invalid response from IEC API: {str(ex)}")
 
-    logger.debug(f"HTTP GET Response: {resp_content}")
-
     return resp_content
 
 
 async def send_post_request(
     session: ClientSession,
     url: str,
     timeout: Optional[int] = 60,
@@ -154,43 +154,81 @@
     json_data: Optional[dict] = None,
 ) -> dict[str, Any]:
     try:
         if not headers:
             headers = session.headers
 
         if not timeout:
-            headers = session.timeout
-
-        logger.debug(f"HTTP POST: {url}")
-        logger.debug(f"HTTP Content: {data or json_data}")
+            timeout = session.timeout
 
         resp = await session.post(url=url, data=data, json=json_data, headers=headers, timeout=timeout)
 
         json_resp: dict = await resp.json(content_type=None)
     except TimeoutError as ex:
         raise IECError(-1, f"Failed to communicate with IEC API due to time out: ({str(ex)})")
     except ClientError as ex:
         raise IECError(-1, f"Failed to communicate with IEC API due to ClientError: ({str(ex)})")
     except JSONDecodeError as ex:
         raise IECError(-1, f"Received invalid response from IEC API: {str(ex)}")
 
-    logger.debug(f"HTTP POST Response: {json_resp}")
-
     if resp.status != http.HTTPStatus.OK:
         parse_error_response(resp, json_resp)
     return json_resp
 
 
+async def send_non_json_post_request(
+    session: ClientSession,
+    url: str,
+    timeout: Optional[int] = 60,
+    headers: Optional[dict] = None,
+    data: Optional[dict] = None,
+    json_data: Optional[dict] = None,
+) -> StreamReader:
+    try:
+        if not headers:
+            headers = session.headers
+
+        if not timeout:
+            headers = session.timeout
+
+        resp = await session.post(url=url, data=data, json=json_data, headers=headers, timeout=timeout)
+    except TimeoutError as ex:
+        raise IECError(-1, f"Failed to communicate with IEC API due to time out: ({str(ex)})")
+    except ClientError as ex:
+        raise IECError(-1, f"Failed to communicate with IEC API due to ClientError: ({str(ex)})")
+    except JSONDecodeError as ex:
+        raise IECError(-1, f"Received invalid response from IEC API: {str(ex)}")
+
+    if resp.status != http.HTTPStatus.OK:
+        raise IECError(resp.status, resp.reason)
+    return resp.content
+
+
 def convert_to_tz_aware_datetime(dt: Optional[datetime]) -> Optional[datetime]:
     """
     Convert a datetime object to a timezone aware datetime object.
     Args:
         dt (Optional[datetime]): The datetime object to be converted.
     Returns:
         Optional[datetime]: The timezone aware datetime object, or None if dt is None.
     """
     if dt is None:
         return None
     elif dt.year > 2000:  # Fix '0001-01-01T00:00:00' values
         return TIMEZONE.localize(dt)
     else:
         return dt.replace(tzinfo=pytz.utc)
+
+
+async def on_request_start_debug(session: aiohttp.ClientSession, context, params: aiohttp.TraceRequestStartParams):
+    logger.debug(f"HTTP {params.method}: {params.url}")
+
+
+async def on_request_chunk_sent_debug(
+    session: aiohttp.ClientSession, context, params: aiohttp.TraceRequestChunkSentParams
+):
+    if (params.method == "POST" or params.method == "PUT") and params.chunk:
+        logger.debug(f"HTTP Content {params.method}: {params.chunk}")
+
+
+async def on_request_end_debug(session: aiohttp.ClientSession, context, params: aiohttp.TraceRequestEndParams):
+    logger.debug(f"HTTP {params.method} Response <{params.response.status}>: {await params.response.text()}")
```

### Comparing `iec_api-0.2.8/iec_api/const.py` & `iec_api-0.3.0/iec_api/const.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,20 +21,33 @@
 
 HEADERS_WITH_AUTH = HEADERS_NO_AUTH.copy()  # Make a copy of the original dictionary
 HEADERS_WITH_AUTH["Authorization"] = "Bearer 1234"
 HEADERS_WITH_AUTH["Cookie"] = "ARRAffinity=?; " "ARRAffinitySameSite=?;" " GCLB=?"
 
 TIMEZONE = pytz.timezone("Asia/Jerusalem")
 IEC_API_BASE_URL = "https://iecapi.iec.co.il//api/"
+IEC_FAULT_PORTAL_API_URL = "https://masa-faultsportalapi.iec.co.il/api/"
+
 GET_ACCOUNTS_URL = IEC_API_BASE_URL + "outages/accounts"
 GET_CONSUMER_URL = IEC_API_BASE_URL + "customer"
 GET_REQUEST_READING_URL = IEC_API_BASE_URL + "Consumption/RemoteReadingRange/{contract_id}"
 GET_ELECTRIC_BILL_URL = IEC_API_BASE_URL + "ElectricBillsDrawers/ElectricBills/{contract_id}/{bp_number}"
 GET_CONTRACTS_URL = IEC_API_BASE_URL + "customer/contract/{bp_number}"
+GET_CHECK_CONTRACT_URL = IEC_API_BASE_URL + "customer/checkContract/{{contract_id}}/6"
+GET_EFS_MESSAGES_URL = IEC_API_BASE_URL + "customer/efs"
 GET_DEFAULT_CONTRACT_URL = GET_CONTRACTS_URL + "?count=1"
 GET_LAST_METER_READING_URL = IEC_API_BASE_URL + "Device/LastMeterReading/{contract_id}/{bp_number}"
 AUTHENTICATE_URL = IEC_API_BASE_URL + "Authentication/{id}/1/-1?customErrorPage=true"
 GET_DEVICES_URL = IEC_API_BASE_URL + "Device/{contract_id}"
+GET_TENANT_IDENTITY_URL = IEC_API_BASE_URL + "Tenant/Identify/{device_id}"
 GET_DEVICE_BY_DEVICE_ID_URL = GET_DEVICES_URL + "/{device_id}"
 GET_DEVICE_TYPE_URL = IEC_API_BASE_URL + "Device/type/{bp_number}/{contract_id}/false"
-GET_BILLING_INVOICES = IEC_API_BASE_URL + "billingCollection/invoices/{contract_id}/{bp_number}"
+GET_BILLING_INVOICES_URL = IEC_API_BASE_URL + "BillingCollection/invoices/{contract_id}/{bp_number}"
+GET_INVOICE_PDF_URL = IEC_API_BASE_URL + "BillingCollection/pdf"
 GET_KWH_TARIFF_URL = IEC_API_BASE_URL + "content/en-US/content/tariffs/contentpages/homeelectricitytariff"
+GET_CALCULATOR_GADGET_URL = IEC_API_BASE_URL + "content/en-US/calculators/gadget"
+GET_OUTAGES_URL = IEC_API_BASE_URL + "outages/transactions/{account_id}/2"
+
+GET_USER_PROFILE_FROM_FAULT_PORTAL_URL = IEC_FAULT_PORTAL_API_URL + "contacts/userprofile"
+GET_OUTAGES_FROM_FAULT_PORTAL_URL = IEC_FAULT_PORTAL_API_URL + "accounts/{account_id}/tranzactions/2"
+ERROR_FIELD_NAME = "Error"
+ERROR_SUMMARY_FIELD_NAME = "errorSummary"
```

### Comparing `iec_api-0.2.8/iec_api/data.py` & `iec_api-0.3.0/iec_api/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,65 @@
-import base64
+import logging
 from datetime import datetime
-from typing import Optional, TypeVar
+from typing import List, Optional, TypeVar
 
 from aiohttp import ClientSession
-from loguru import logger
 from mashumaro.codecs import BasicDecoder
 
 from iec_api import commons
 from iec_api.const import (
     GET_ACCOUNTS_URL,
-    GET_BILLING_INVOICES,
+    GET_BILLING_INVOICES_URL,
+    GET_CHECK_CONTRACT_URL,
     GET_CONSUMER_URL,
     GET_CONTRACTS_URL,
     GET_DEFAULT_CONTRACT_URL,
     GET_DEVICE_BY_DEVICE_ID_URL,
     GET_DEVICE_TYPE_URL,
     GET_DEVICES_URL,
+    GET_EFS_MESSAGES_URL,
     GET_ELECTRIC_BILL_URL,
-    GET_KWH_TARIFF_URL,
+    GET_INVOICE_PDF_URL,
     GET_LAST_METER_READING_URL,
+    GET_OUTAGES_URL,
     GET_REQUEST_READING_URL,
+    GET_TENANT_IDENTITY_URL,
     HEADERS_WITH_AUTH,
 )
 from iec_api.models.account import Account
 from iec_api.models.account import decoder as account_decoder
 from iec_api.models.contract import Contract, Contracts
 from iec_api.models.contract import decoder as contract_decoder
+from iec_api.models.contract_check import ContractCheck
+from iec_api.models.contract_check import decoder as contract_check_decoder
 from iec_api.models.customer import Customer
 from iec_api.models.device import Device, Devices
 from iec_api.models.device import decoder as devices_decoder
+from iec_api.models.device_identity import DeviceDetails, DeviceIdentity
+from iec_api.models.device_identity import decoder as device_identity_decoder
 from iec_api.models.device_type import DeviceType
 from iec_api.models.device_type import decoder as device_type_decoder
+from iec_api.models.efs import EfsMessage, EfsRequestAllServices, EfsRequestSingleService
+from iec_api.models.efs import decoder as efs_decoder
 from iec_api.models.electric_bill import ElectricBill
 from iec_api.models.electric_bill import decoder as electric_bill_decoder
 from iec_api.models.exceptions import IECError
+from iec_api.models.get_pdf import GetPdfRequest
 from iec_api.models.invoice import GetInvoicesBody
 from iec_api.models.invoice import decoder as invoice_decoder
 from iec_api.models.jwt import JWT
 from iec_api.models.meter_reading import MeterReadings
 from iec_api.models.meter_reading import decoder as meter_reading_decoder
+from iec_api.models.outages import Outage
+from iec_api.models.outages import decoder as outages_decoder
 from iec_api.models.remote_reading import ReadingResolution, RemoteReadingRequest, RemoteReadingResponse
 from iec_api.models.response_descriptor import ResponseWithDescriptor
 
 T = TypeVar("T")
+logger = logging.getLogger(__name__)
 
 
 async def _get_response_with_descriptor(
     session: ClientSession, jwt_token: JWT, request_url: str, decoder: BasicDecoder[ResponseWithDescriptor[T]]
 ) -> T:
     """
     A function to retrieve a response with a descriptor using a JWT token and a URL.
@@ -67,26 +80,56 @@
         raise IECError(
             response_with_descriptor.response_descriptor.code, response_with_descriptor.response_descriptor.description
         )
 
     return response_with_descriptor.data
 
 
-async def get_accounts(session: ClientSession, token: JWT) -> list[Account]:
+async def _post_response_with_descriptor(
+    session: ClientSession,
+    jwt_token: JWT,
+    request_url: str,
+    json_data: Optional[dict],
+    decoder: BasicDecoder[ResponseWithDescriptor[T]],
+) -> T:
+    """
+    A function to retrieve a response with a descriptor using a JWT token and a URL.
+
+    Args:
+        jwt_token (JWT): The JWT token used for authentication.
+        request_url (str): The URL to send the request to.
+        json_data (dict): POST content
+
+    Returns:
+        T: The response with a descriptor, with its type specified by the return type annotation.
+    """
+    headers = commons.add_auth_bearer_to_headers(HEADERS_WITH_AUTH, jwt_token.id_token)
+    response = await commons.send_post_request(session=session, url=request_url, headers=headers, json_data=json_data)
+
+    response_with_descriptor = decoder.decode(response)
+
+    if not response_with_descriptor.data and not response_with_descriptor.response_descriptor.is_success:
+        raise IECError(
+            response_with_descriptor.response_descriptor.code, response_with_descriptor.response_descriptor.description
+        )
+
+    return response_with_descriptor.data
+
+
+async def get_accounts(session: ClientSession, token: JWT) -> Optional[List[Account]]:
     """Get Accounts response from IEC API."""
     return await _get_response_with_descriptor(session, token, GET_ACCOUNTS_URL, account_decoder)
 
 
 async def get_customer(session: ClientSession, token: JWT) -> Optional[Customer]:
     """Get customer data response from IEC API."""
     headers = commons.add_auth_bearer_to_headers(HEADERS_WITH_AUTH, token.id_token)
     # sending get request and saving the response as response object
     response = await commons.send_get_request(session=session, url=GET_CONSUMER_URL, headers=headers)
 
-    logger.debug(f"Response: {response}")
     return Customer.from_dict(response)
 
 
 async def get_remote_reading(
     session: ClientSession,
     token: JWT,
     contract_id: str,
@@ -108,39 +151,64 @@
     headers = commons.add_auth_bearer_to_headers(HEADERS_WITH_AUTH, token.id_token)
 
     response = await commons.send_post_request(session=session, url=url, headers=headers, json_data=req.to_dict())
 
     return RemoteReadingResponse.from_dict(response)
 
 
-async def get_electric_bill(session: ClientSession, token: JWT, bp_number: str, contract_id: str) -> ElectricBill:
+async def get_efs_messages(
+    session: ClientSession, token: JWT, contract_id: str, service_code: Optional[int] = None
+) -> Optional[List[EfsMessage]]:
+    """Get EFS Messages response from IEC API."""
+    if service_code:
+        req = EfsRequestSingleService(contract_number=contract_id, process_type=1, service_code=f"EFS{service_code:03}")
+    else:
+        req = EfsRequestAllServices(contract_number=contract_id, process_type=1)
+
+    url = GET_EFS_MESSAGES_URL
+
+    return await _post_response_with_descriptor(session, token, url, json_data=req.to_dict(), decoder=efs_decoder)
+
+
+async def get_electric_bill(
+    session: ClientSession, token: JWT, bp_number: str, contract_id: str
+) -> Optional[ElectricBill]:
     """Get Electric Bill data response from IEC API."""
     return await _get_response_with_descriptor(
         session,
         token,
         GET_ELECTRIC_BILL_URL.format(contract_id=contract_id, bp_number=bp_number),
         electric_bill_decoder,
     )
 
 
-async def get_default_contract(session: ClientSession, token: JWT, bp_number: str) -> Contract:
+async def get_default_contract(session: ClientSession, token: JWT, bp_number: str) -> Optional[Contract]:
     """Get Contract data response from IEC API."""
     return await _get_response_with_descriptor(
         session, token, GET_DEFAULT_CONTRACT_URL.format(bp_number=bp_number), contract_decoder
     )
 
 
-async def get_contracts(session: ClientSession, token: JWT, bp_number: str) -> Contracts:
+async def get_contracts(session: ClientSession, token: JWT, bp_number: str) -> Optional[Contracts]:
     """Get all user's Contracts from IEC API."""
     return await _get_response_with_descriptor(
         session, token, GET_CONTRACTS_URL.format(bp_number=bp_number), contract_decoder
     )
 
 
-async def get_last_meter_reading(session: ClientSession, token: JWT, bp_number: str, contract_id: str) -> MeterReadings:
+async def get_contract_check(session: ClientSession, token: JWT, contract_id: str) -> Optional[ContractCheck]:
+    """Get Contract Check response from IEC API."""
+    return await _get_response_with_descriptor(
+        session, token, GET_CHECK_CONTRACT_URL.format(contract_id=contract_id), contract_check_decoder
+    )
+
+
+async def get_last_meter_reading(
+    session: ClientSession, token: JWT, bp_number: str, contract_id: str
+) -> Optional[MeterReadings]:
     """Get Last Meter Reading data response from IEC API."""
     return await _get_response_with_descriptor(
         session,
         token,
         GET_LAST_METER_READING_URL.format(contract_id=contract_id, bp_number=bp_number),
         meter_reading_decoder,
     )
@@ -150,42 +218,79 @@
     """Get Device data response from IEC API."""
     headers = commons.add_auth_bearer_to_headers(HEADERS_WITH_AUTH, token.id_token)
     # sending get request and saving the response as response object
     response = await commons.send_get_request(
         session=session, url=GET_DEVICES_URL.format(contract_id=contract_id), headers=headers
     )
 
-    logger.debug(f"Response: {response}")
     return [Device.from_dict(device) for device in response]
 
 
-async def get_device_by_device_id(session: ClientSession, token: JWT, contract_id: str, device_id: str) -> Devices:
+async def get_device_details(session: ClientSession, token: JWT, device_id: str) -> Optional[List[DeviceDetails]]:
+    """Get Device Details response from IEC API."""
+    device_identity: DeviceIdentity = await _get_response_with_descriptor(
+        session, token, GET_TENANT_IDENTITY_URL.format(device_id=device_id), device_identity_decoder
+    )
+
+    return device_identity.device_details if device_identity else None
+
+
+async def get_device_details_by_code(
+    session: ClientSession, token: JWT, device_id: str, device_code: str
+) -> Optional[DeviceDetails]:
+    """Get Device Details response from IEC API."""
+    devices = await get_device_details(session, token, device_id)
+
+    return next((device for device in devices if device.device_code == device_code), None)
+
+
+async def get_device_by_device_id(
+    session: ClientSession, token: JWT, contract_id: str, device_id: str
+) -> Optional[Devices]:
     """Get Device data response from IEC API."""
     return await _get_response_with_descriptor(
         session,
         token,
         GET_DEVICE_BY_DEVICE_ID_URL.format(device_id=device_id, contract_id=contract_id),
         devices_decoder,
     )
 
 
-async def get_device_type(session: ClientSession, token: JWT, bp_number: str, contract_id: str) -> DeviceType:
+async def get_device_type(session: ClientSession, token: JWT, bp_number: str, contract_id: str) -> Optional[DeviceType]:
     """Get Device Type data response from IEC API."""
     # sending get request and saving the response as response object
     return await _get_response_with_descriptor(
         session, token, GET_DEVICE_TYPE_URL.format(bp_number=bp_number, contract_id=contract_id), device_type_decoder
     )
 
 
-async def get_billing_invoices(session: ClientSession, token: JWT, bp_number: str, contract_id: str) -> GetInvoicesBody:
+async def get_billing_invoices(
+    session: ClientSession, token: JWT, bp_number: str, contract_id: str
+) -> Optional[GetInvoicesBody]:
     """Get Device Type data response from IEC API."""
     return await _get_response_with_descriptor(
-        session, token, GET_BILLING_INVOICES.format(bp_number=bp_number, contract_id=contract_id), invoice_decoder
+        session, token, GET_BILLING_INVOICES_URL.format(bp_number=bp_number, contract_id=contract_id), invoice_decoder
     )
 
 
-async def get_kwh_tariff(session: ClientSession) -> float:
-    """Get Device Type data response from IEC API."""
-    response = await commons.send_get_request(session=session, url=GET_KWH_TARIFF_URL)
-    kwh_tariff_str = response["components"][1]["table"][1][2]["value"]
+async def get_invoice_pdf(
+    session: ClientSession, token: JWT, bp_number: int | str, contract_id: int | str, invoice_number: int | str
+) -> bytes:
+    """Get Invoice PDF response from IEC API."""
+    headers = commons.add_auth_bearer_to_headers(HEADERS_WITH_AUTH, token.id_token)
+    headers = headers.copy()  # don't modify original headers
+    headers.update({"accept": "application/pdf", "content-type": "application/json"})
+
+    request = GetPdfRequest(
+        invoice_number=str(invoice_number), contract_id=str(contract_id), bp_number=str(bp_number)
+    ).to_dict()
+    response = await commons.send_non_json_post_request(
+        session, url=GET_INVOICE_PDF_URL, headers=headers, json_data=request
+    )
+    return await response.read()
+
 
-    return float(base64.b64decode(kwh_tariff_str).decode("utf-8"))
+async def get_outages_by_account(session: ClientSession, token: JWT, account_id: str) -> Optional[list[Outage]]:
+    """Get Device Type data response from IEC API."""
+    return await _get_response_with_descriptor(
+        session, token, GET_OUTAGES_URL.format(account_id=account_id), outages_decoder
+    )
```

### Comparing `iec_api-0.2.8/iec_api/iec_client.py` & `iec_api-0.3.0/iec_api/iec_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 import asyncio
 import atexit
-from datetime import datetime, timedelta
-from typing import Optional
+import logging
+from datetime import datetime
+from typing import List, Optional
 
+import aiofiles
 import aiohttp
 import jwt
 from aiohttp import ClientSession
-from loguru import logger
 
-from iec_api import data, login
-from iec_api.commons import is_valid_israeli_id
+from iec_api import commons, data, fault_portal_data, login, static_data
+from iec_api.fault_portal_models.outages import FaultPortalOutage
+from iec_api.fault_portal_models.user_profile import UserProfile
+from iec_api.models.account import Account
 from iec_api.models.contract import Contract
-from iec_api.models.customer import Account, Customer
+from iec_api.models.contract_check import ContractCheck
+from iec_api.models.customer import Customer
 from iec_api.models.device import Device, Devices
+from iec_api.models.device_identity import DeviceDetails
 from iec_api.models.device_type import DeviceType
+from iec_api.models.efs import EfsMessage
 from iec_api.models.electric_bill import ElectricBill
 from iec_api.models.exceptions import IECLoginError
 from iec_api.models.invoice import GetInvoicesBody
 from iec_api.models.jwt import JWT
 from iec_api.models.meter_reading import MeterReadings
+from iec_api.models.outages import Outage
 from iec_api.models.remote_reading import ReadingResolution, RemoteReadingResponse
+from iec_api.usage_calculator.calculator import UsageCalculator
+
+logger = logging.getLogger(__name__)
 
 
 class IecClient:
     """IEC API Client."""
 
     def __init__(self, user_id: str | int, session: Optional[ClientSession] = None):
         """
@@ -31,66 +41,75 @@
 
         Args:
         session (ClientSession): The aiohttp ClientSession object.
         user_id (str): The user ID (SSN) to be associated with the instance.
         automatically_login (bool): Whether to automatically log in the user. Default is False.
         """
 
-        self._kwh_tariff: Optional[float] = None
-        self._kwh_tariff_fetch_time: Optional[datetime.datetime] = None
-        if not is_valid_israeli_id(user_id):
+        if not commons.is_valid_israeli_id(user_id):
             raise ValueError("User ID must be a valid Israeli ID.")
 
+        # Custom Logger to the session
+        trace_config = aiohttp.TraceConfig()
+        trace_config.on_request_start.append(commons.on_request_start_debug)
+        trace_config.on_request_chunk_sent.append(commons.on_request_chunk_sent_debug)
+        trace_config.on_request_end.append(commons.on_request_end_debug)
+        trace_config.freeze()
+
         if not session:
-            session = aiohttp.ClientSession()
+            session = aiohttp.ClientSession(trace_configs=[trace_config])
             atexit.register(self._shutdown)
+        else:
+            session.trace_configs.append(trace_config)
 
         self._session = session
 
         self._state_token: Optional[str] = None  # Token for maintaining the state of the user's session
         self._factor_id: Optional[str] = None  # Factor ID for multifactor authentication
         self._session_token: Optional[str] = None  # Token for maintaining the user's session
         self.logged_in: bool = False  # Flag to indicate if the user is logged in
         self._token: JWT = JWT(
             access_token="", refresh_token="", token_type="", expires_in=0, scope="", id_token=""
         )  # Token for authentication
         self._user_id: str = str(user_id)  # User ID associated with the instance
         self._login_response: Optional[str] = None  # Response from the login attempt
         self._bp_number: Optional[str] = None  # BP Number associated with the instance
         self._contract_id: Optional[str] = None  # Contract ID associated with the instance
+        self._account_id: Optional[str] = None  # Account ID associated with the instance
 
     def _shutdown(self):
         if not self._session.closed:
             asyncio.run(self._session.close())
 
     # -------------
     # Data methods:
     # -------------
 
-    async def get_customer(self) -> Customer:
+    async def get_customer(self) -> Optional[Customer]:
         """
         Get consumer data response from IEC API.
         :return: Customer data
         """
         await self.check_token()
         customer = await data.get_customer(self._session, self._token)
         if customer:
             self._bp_number = customer.bp_number
         return customer
 
-    async def get_accounts(self) -> list[Account]:
+    async def get_accounts(self) -> Optional[List[Account]]:
         """
         Get consumer data response from IEC API.
         :return: Customer data
         """
         await self.check_token()
         accounts = await data.get_accounts(self._session, self._token)
 
-        if len(accounts) > 0:
+        if accounts and len(accounts) > 0:
             self._bp_number = accounts[0].account_number
+            self._account_id = accounts[0].id
 
         return accounts
 
     async def get_default_account(self) -> Account:
         """
         Get consumer data response from IEC API.
         :return: Customer data
@@ -109,15 +128,15 @@
 
         if not bp_number:
             bp_number = self._bp_number
 
         assert bp_number, "BP number must be provided"
 
         get_contract_response = await data.get_contracts(self._session, self._token, bp_number)
-        if get_contract_response and get_contract_response:
+        if get_contract_response:
             contracts = get_contract_response.contracts
             if contracts and len(contracts) > 0:
                 self._contract_id = contracts[0].contract_id
             return contracts[0]
         return None
 
     async def get_contracts(self, bp_number: str = None) -> list[Contract]:
@@ -138,14 +157,32 @@
         if get_contract_response:
             contracts = get_contract_response.contracts
             if contracts and len(contracts) > 0:
                 self._contract_id = contracts[0].contract_id
             return contracts
         return []
 
+    async def get_contract_check(self, contract_id: Optional[str] = None) -> Optional[ContractCheck]:
+        """
+        Get contract check for the contract
+        Args:
+            self: The instance of the class.
+            contract_id (str): The Contract ID of the meter.
+        Returns:
+            ContractCheck: a contract check
+        """
+        await self.check_token()
+
+        if not contract_id:
+            contract_id = self._contract_id
+
+        assert contract_id, "Contract Id must be provided"
+
+        return await data.get_contract_check(self._session, self._token, contract_id)
+
     async def get_last_meter_reading(
         self, bp_number: Optional[str] = None, contract_id: Optional[str] = None
     ) -> Optional[MeterReadings]:
         """
         Retrieves a last meter reading for a specific contract and user.
         Args:
             self: The instance of the class.
@@ -161,18 +198,15 @@
         assert bp_number, "BP number must be provided"
 
         if not contract_id:
             contract_id = self._contract_id
 
         assert contract_id, "Contract ID must be provided"
 
-        response = await data.get_last_meter_reading(self._session, self._token, bp_number, contract_id)
-        if response:
-            return response
-        return None
+        return await data.get_last_meter_reading(self._session, self._token, bp_number, contract_id)
 
     async def get_electric_bill(
         self, bp_number: Optional[str] = None, contract_id: Optional[str] = None
     ) -> Optional[ElectricBill]:
         """
         Retrieves a remote reading for a specific meter using the provided parameters.
         Args:
@@ -190,20 +224,50 @@
         assert bp_number, "BP number must be provided"
 
         if not contract_id:
             contract_id = self._contract_id
 
         assert contract_id, "Contract ID must be provided"
 
-        response = await data.get_electric_bill(self._session, self._token, bp_number, contract_id)
-        if response:
-            return response
-        return None
+        return await data.get_electric_bill(self._session, self._token, bp_number, contract_id)
 
-    async def get_devices(self, contract_id: Optional[str] = None) -> Optional[list[Device]]:
+    async def save_invoice_pdf_to_file(
+        self,
+        file_path: str,
+        invoice_number: str | int,
+        bp_number: Optional[str | int] = None,
+        contract_id: Optional[str | int] = None,
+    ):
+        """
+        Get PDF of invoice from IEC api
+        Args:
+            self: The instance of the class.
+            file_path (str): Path to save the bill to
+            invoice_number (str): The requested invoice number
+            bp_number (str): The BP number of the meter.
+            contract_id (str): The contract ID associated with the meter.
+        """
+        await self.check_token()
+
+        if not bp_number:
+            bp_number = self._bp_number
+
+        assert bp_number, "BP number must be provided"
+
+        if not contract_id:
+            contract_id = self._contract_id
+
+        assert contract_id, "Contract ID must be provided"
+
+        response_bytes = await data.get_invoice_pdf(self._session, self._token, bp_number, contract_id, invoice_number)
+        if response_bytes:
+            async with aiofiles.open(file_path, "wb") as f:
+                await f.write(response_bytes)
+
+    async def get_devices(self, contract_id: Optional[str] = None) -> Optional[List[Device]]:
         """
         Get a list of devices for the user
         Args:
             self: The instance of the class.
             contract_id (str): The Contract ID of the meter.
         Returns:
             list[Device]: List of devices
@@ -213,15 +277,15 @@
         if not contract_id:
             contract_id = self._contract_id
 
         assert contract_id, "Contract Id must be provided"
 
         return await data.get_devices(self._session, self._token, contract_id)
 
-    async def get_device_by_device_id(self, device_id: str, contract_id: Optional[str] = None) -> Devices:
+    async def get_device_by_device_id(self, device_id: str, contract_id: Optional[str] = None) -> Optional[Devices]:
         """
         Get a list of devices for the user
         Args:
             self: The instance of the class.
             device_id (str): The Device code.
             contract_id (str): The Contract ID of the user.
         Returns:
@@ -232,14 +296,43 @@
         if not contract_id:
             contract_id = self._contract_id
 
         assert contract_id, "Contract ID must be provided"
 
         return await data.get_device_by_device_id(self._session, self._token, contract_id, device_id)
 
+    async def get_device_details_by_device_id(self, device_id: str) -> Optional[List[DeviceDetails]]:
+        """
+        Get a list of devices for the user
+        Args:
+            self: The instance of the class.
+            device_id (str): The Device id.
+        Returns:
+            list[DeviceDetails]: List of device details or None
+        """
+        await self.check_token()
+
+        return await data.get_device_details(self._session, self._token, device_id)
+
+    async def get_device_details_by_device_id_and_code(
+        self, device_id: str, device_code: str
+    ) -> Optional[DeviceDetails]:
+        """
+        Get a list of devices for the user
+        Args:
+            self: The instance of the class.
+            device_id (str): The Device id.
+            device_code (str): The Device code.
+        Returns:
+            DeviceDetails: Device details or None
+        """
+        await self.check_token()
+
+        return await data.get_device_details_by_code(self._session, self._token, device_id, device_code)
+
     async def get_remote_reading(
         self,
         meter_serial_number: str,
         meter_code: int,
         last_invoice_date: datetime,
         from_date: datetime,
         resolution: ReadingResolution = ReadingResolution.DAILY,
@@ -269,15 +362,17 @@
             meter_serial_number,
             meter_code,
             last_invoice_date,
             from_date,
             resolution,
         )
 
-    async def get_device_type(self, bp_number: Optional[str] = None, contract_id: Optional[str] = None) -> DeviceType:
+    async def get_device_type(
+        self, bp_number: Optional[str] = None, contract_id: Optional[str] = None
+    ) -> Optional[DeviceType]:
         """
         Get a list of devices for the user
         Args:
             self: The instance of the class.
             bp_number (str): The BP number of the meter.
             contract_id (str: The Contract ID
         Returns:
@@ -295,15 +390,15 @@
 
         assert contract_id, "Contract ID must be provided"
 
         return await data.get_device_type(self._session, self._token, bp_number, contract_id)
 
     async def get_billing_invoices(
         self, bp_number: Optional[str] = None, contract_id: Optional[str] = None
-    ) -> GetInvoicesBody:
+    ) -> Optional[GetInvoicesBody]:
         """
         Get a list of devices for the user
         Args:
             self: The instance of the class.
             bp_number (str): The BP number of the meter.
             contract_id (str: The Contract ID
         Returns:
@@ -320,20 +415,95 @@
             contract_id = self._contract_id
 
         assert contract_id, "Contract ID must be provided"
 
         return await data.get_billing_invoices(self._session, self._token, bp_number, contract_id)
 
     async def get_kwh_tariff(self) -> float:
-        if not self._kwh_tariff or self._kwh_tariff_fetch_time < datetime.now() - timedelta(hours=1):
-            logger.debug("Tariff is missing or expired, fetching kwh tariff from IEC API")
-            self._kwh_tariff_fetch_time = datetime.now()
-            self._kwh_tariff = await data.get_kwh_tariff(self._session)
+        """Get kWh tariff"""
+        return await static_data.get_kwh_tariff(self._session)
+
+    async def get_usage_calculator(self) -> UsageCalculator:
+        """
+        Get Usage Calculator module
+        Returns:
+            UsageCalculator
+        """
+        return await static_data.get_usage_calculator(self._session)
+
+    async def get_efs_messages(
+        self, contract_id: Optional[str] = None, service_code: Optional[int] = None
+    ) -> Optional[List[EfsMessage]]:
+        """Get EFS Messages for the contract
+        Args:
+            self: The instance of the class.
+            contract_id (str): The Contract ID of the meter.
+            service_code (str): Specific EFS Service code
+        Returns:
+            list[EfsMessage]: List of EFS Messages
+        """
+        await self.check_token()
+
+        if not contract_id:
+            contract_id = self._contract_id
+
+        assert contract_id, "Contract Id must be provided"
+
+        return await data.get_efs_messages(self._session, self._token, contract_id, service_code)
+
+    async def get_outages_by_account(self, account_id: Optional[str] = None) -> Optional[List[Outage]]:
+        """Get Outages for the Account
+        Args:
+            self: The instance of the class.
+            account_id (str): The Account ID of the meter.
+        Returns:
+            list[Outage]: List of the Outages Messages
+        """
+        await self.check_token()
+
+        if not account_id:
+            account_id = self._account_id
+
+        assert account_id, "Account Id must be provided"
+
+        return await data.get_outages_by_account(self._session, self._token, account_id)
+
+    # ----------------
+    # Fault Portal Endpoints
+    # ----------------
+
+    async def get_fault_portal_user_profile(self) -> Optional[UserProfile]:
+        """Get User Profile for the Account from Fault Portal
+        Args:
+            self: The instance of the class.
+        Returns:
+            list[UserProfile]: The User Profile
+        """
+        await self.check_token()
+
+        return await fault_portal_data.get_user_profile(self._session, self._token)
+
+    async def get_fault_portal_outages_by_account(
+        self, account_id: Optional[str] = None
+    ) -> (Optional)[List[FaultPortalOutage]]:
+        """Get Outages for the Account from Fault Portal
+        Args:
+            self: The instance of the class.
+            account_id (str): The Account ID of the meter.
+        Returns:
+            list[Outage]: List of the Outages Messages
+        """
+        await self.check_token()
+
+        if not account_id:
+            account_id = self._account_id
+
+        assert account_id, "Account Id must be provided"
 
-        return self._kwh_tariff
+        return await fault_portal_data.get_outages_by_account(self._session, self._token, account_id)
 
     # ----------------
     # Login/Token Flow
     # ----------------
 
     async def login_with_id(self):
         """
```

### Comparing `iec_api-0.2.8/iec_api/login.py` & `iec_api-0.3.0/iec_api/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """ IEC Login Module. """
 import json
+import logging
 import random
 import re
 import string
 import time
 from typing import Optional, Tuple
 
 import aiofiles
 import jwt
 import pkce
 from aiohttp import ClientSession
-from loguru import logger
 
 from iec_api import commons
 from iec_api.models.exceptions import IECLoginError
 from iec_api.models.jwt import JWT
 
+logger = logging.getLogger(__name__)
+
 APP_CLIENT_ID = "0oaqf6zr7yEcQZqqt2p7"
 CODE_CHALLENGE_METHOD = "S256"
 APP_REDIRECT_URI = "com.iecrn:/"
 code_verifier, code_challenge = pkce.generate_pkce_pair()
 STATE = "".join(random.choice(string.digits + string.ascii_letters) for _ in range(12))
 IEC_OKTA_BASE_URL = "https://iec-ext.okta.com"
```

### Comparing `iec_api-0.2.8/iec_api/models/account.py` & `iec_api-0.3.0/iec_api/models/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass, field
 from typing import Optional
+from uuid import UUID
 
 from mashumaro import DataClassDictMixin, field_options
 from mashumaro.codecs import BasicDecoder
 
 from iec_api.models.response_descriptor import ResponseWithDescriptor
 
 # GET https://iecapi.iec.co.il//api/outages/accounts
@@ -30,15 +31,15 @@
 # }
 
 
 @dataclass
 class Account(DataClassDictMixin):
     account_number: str = field(metadata=field_options(alias="accountNumber"))
     account_type: int = field(metadata=field_options(alias="accountType"))
-    id: str
+    id: UUID
     email: Optional[str]
     telephone: Optional[str]
     government_number: str = field(metadata=field_options(alias="governmentNumber"))
     name: str
     view_type_code: int = field(metadata=field_options(alias="viewTypeCode"))
```

### Comparing `iec_api-0.2.8/iec_api/models/contract.py` & `iec_api-0.3.0/iec_api/models/contract.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 class Contract(DataClassDictMixin):
     address: str
     contract_id: str = field(metadata=field_options(alias="contractId"))
     due_date: date = field(metadata=field_options(alias="dueDate"))
     total_debt: float = field(metadata=field_options(alias="totalDebt"))
     frequency: int
     status: int
-    from_pativte_producer: bool = field(metadata=field_options(alias="fromPativteProducer"))
+    from_private_producer: bool = field(metadata=field_options(alias="fromPativteProducer"))
     city_code: str = field(metadata=field_options(alias="cityCode"))
     city_name: str = field(metadata=field_options(alias="cityName"))
     street_code: str = field(metadata=field_options(alias="streetCode"))
     street_name: str = field(metadata=field_options(alias="streetName"))
     house_number: str = field(metadata=field_options(alias="houseNumber"))
     debt_for_invoices_due_date_not_passed: float = field(
         metadata=field_options(alias="debtForInvoicesDueDateNotPassed")
```

### Comparing `iec_api-0.2.8/iec_api/models/customer.py` & `iec_api-0.3.0/iec_api/models/customer.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 from dataclasses import dataclass, field
 
 from mashumaro import DataClassDictMixin, field_options
 
 
 @dataclass
-class Account(DataClassDictMixin):
+class CustomerAccount(DataClassDictMixin):
     main_contract_id: str = field(metadata=field_options(alias="mainContractId"))
     main_contract_id_type: int = field(metadata=field_options(alias="mainContractIdType"))
     company_id: str = field(metadata=field_options(alias="companyId"))
     name: str
     last_name: str = field(metadata=field_options(alias="lastName"))
     bp_number: str = field(metadata=field_options(alias="bpNumber"))
     bp_type: int = field(metadata=field_options(alias="bpType"))
@@ -49,14 +49,14 @@
     account_type: int = field(metadata=field_options(alias="accountType"))
 
 
 @dataclass
 class Customer(DataClassDictMixin):
     bp_number: str = field(metadata=field_options(alias="bpNumber"))
     id_type: int = field(metadata=field_options(alias="idType"))
-    accounts: list[Account]
+    accounts: list[CustomerAccount]
     customer_status: int = field(metadata=field_options(alias="customerStatus"))
     id_number: str = field(metadata=field_options(alias="idNumber"))
     first_name: str = field(metadata=field_options(alias="firstName"))
     last_name: str = field(metadata=field_options(alias="lastName"))
     mobile_phone: str = field(metadata=field_options(alias="mobilePhone"))
     email: str
```

### Comparing `iec_api-0.2.8/iec_api/models/device.py` & `iec_api-0.3.0/iec_api/models/device.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.8/iec_api/models/device_type.py` & `iec_api-0.3.0/iec_api/models/device_type.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.8/iec_api/models/electric_bill.py` & `iec_api-0.3.0/iec_api/models/electric_bill.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.8/iec_api/models/exceptions.py` & `iec_api-0.3.0/iec_api/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.8/iec_api/models/invoice.py` & `iec_api-0.3.0/iec_api/models/invoice.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from dataclasses import dataclass, field
-from datetime import datetime
+from datetime import date, datetime
 from typing import Optional
 
 from mashumaro import DataClassDictMixin, field_options
 from mashumaro.codecs import BasicDecoder
 
 from iec_api.commons import convert_to_tz_aware_datetime
 from iec_api.models.meter_reading import MeterReading
+from iec_api.models.models_commons import FormattedDate
 from iec_api.models.response_descriptor import ResponseWithDescriptor
 
 # GET https://iecapi.iec.co.il//api/billingCollection/invoices/{bp_number}/{contract_number}
 #
 # {
 #     "data": {
 #         "property": {
@@ -63,15 +64,17 @@
     to_date: Optional[datetime] = field(metadata=field_options(alias="toDate"))
     amount_origin: float = field(metadata=field_options(alias="amountOrigin"))
     amount_to_pay: float = field(metadata=field_options(alias="amountToPay"))
     amount_paid: float = field(metadata=field_options(alias="amountPaid"))
     invoice_id: int = field(metadata=field_options(alias="invoiceId"))
     contract_number: int = field(metadata=field_options(alias="contractNumber"))
     order_number: int = field(metadata=field_options(alias="orderNumber"))
-    last_date: Optional[str] = field(metadata=field_options(alias="lastDate"))
+    last_date: Optional[date] = field(
+        metadata=field_options(alias="lastDate", serialization_strategy=FormattedDate("%d/%m/%Y"))
+    )
     invoice_payment_status: int = field(metadata=field_options(alias="invoicePaymentStatus"))
     document_id: str = field(metadata=field_options(alias="documentID"))
     days_period: str = field(metadata=field_options(alias="daysPeriod"))
     has_direct_debit: bool = field(metadata=field_options(alias="hasDirectDebit"))
     invoice_type: int = field(metadata=field_options(alias="invoiceType"))
 
     reading_code: int = field(metadata=field_options(alias="readingCode"), default=0)
```

### Comparing `iec_api-0.2.8/iec_api/models/meter_reading.py` & `iec_api-0.3.0/iec_api/models/meter_reading.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,25 +51,25 @@
     @classmethod
     def __post_deserialize__(cls, obj: "MeterReading") -> "MeterReading":
         obj.reading_date = convert_to_tz_aware_datetime(obj.reading_date)
         return obj
 
 
 @dataclass
-class LastMeters(DataClassDictMixin):
+class LastMeter(DataClassDictMixin):
     """Last Meters"""
 
     meter_readings: list[MeterReading] = field(metadata=field_options(alias="meterReadings"))
     serial_number: str = field(metadata=field_options(alias="serialNumber"))
     material_number: str = field(metadata=field_options(alias="materialNumber"))
     register_number: str = field(metadata=field_options(alias="registerNumber"))
 
 
 @dataclass
 class MeterReadings(DataClassDictMixin):
     """Meter Readings dataclass."""
 
     contract_account: str = field(metadata=field_options(alias="contractAccount"))
-    last_meters: list[LastMeters] = field(metadata=field_options(alias="lastMeters"))
+    last_meters: list[LastMeter] = field(metadata=field_options(alias="lastMeters"))
 
 
 decoder = BasicDecoder(ResponseWithDescriptor[MeterReadings])
```

### Comparing `iec_api-0.2.8/iec_api/models/okta_errors.py` & `iec_api-0.3.0/iec_api/models/okta_errors.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.8/iec_api/models/remote_reading.py` & `iec_api-0.3.0/iec_api/models/remote_reading.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 class RemoteReading(DataClassDictMixin):
     """Remote Reading Data dataclass."""
 
     status: int
     date: datetime
     value: float
 
+    def __hash__(self):
+        """Compute the hash value the remote reading, based on all fields."""
+        return hash((self.status, self.date, self.value))
+
     @classmethod
     def __post_deserialize__(cls, obj: "RemoteReading") -> "RemoteReading":
         obj.date = convert_to_tz_aware_datetime(obj.date)
         return obj
 
 
 @dataclass
```

### Comparing `iec_api-0.2.8/iec_api/models/response_descriptor.py` & `iec_api-0.3.0/iec_api/models/response_descriptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,9 +29,9 @@
 T = TypeVar("T")
 
 
 @dataclass
 class ResponseWithDescriptor(Generic[T], DataClassDictMixin):
     """Response With Descriptor"""
 
-    data: T
+    data: Optional[T]
     response_descriptor: ResponseDescriptor = field(metadata=field_options(alias=RESPONSE_DESCRIPTOR_FIELD))
```

### Comparing `iec_api-0.2.8/pyproject.toml` & `iec_api-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [tool.poetry]
 name = "iec-api"
-version = "0.2.8"
+version = "0.3.0"
 description = "A Python wrapper for Israel Electric Company API"
 authors = ["GuyKh"]
 license = "MIT"
 readme = "README.md"
 maintainers = [
     "Guy Khmelnitsky <guykhmel@gmail.com>",
 ]
 repository = "https://github.com/GuyKh/py-iec-api"
 keywords = ["python", "poetry", "api", "iec", "israel", "electric"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-mashumaro = "^3.12"
+mashumaro = "^3.13"
 pyjwt = "^2.8.0"
 requests = "^2.31.0"
 pkce = "^1.0.3"
 aiohttp = "^3.9.1"
 aiofiles = "^23.2.1"
-loguru = "^0.7.2"
 pytz = "^2024.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "8.1.0"
-pytest-cov = "^4.1.0"
-ruff = "^0.3.0"
+pytest = "8.2.0"
+pytest-cov = "^5.0.0"
+ruff = "^0.4.1"
 pre-commit = "^3.2.2"
 
 [tool.pytest.ini_options]
 testpaths = ["tests",]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `iec_api-0.2.8/PKG-INFO` & `iec_api-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iec-api
-Version: 0.2.8
+Version: 0.3.0
 Summary: A Python wrapper for Israel Electric Company API
 Home-page: https://github.com/GuyKh/py-iec-api
 License: MIT
 Keywords: python,poetry,api,iec,israel,electric
 Author: GuyKh
 Maintainer: Guy Khmelnitsky
 Maintainer-email: guykhmel@gmail.com
@@ -12,16 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
-Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: mashumaro (>=3.12,<4.0)
+Requires-Dist: mashumaro (>=3.13,<4.0)
 Requires-Dist: pkce (>=1.0.3,<2.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/GuyKh/py-iec-api
 Description-Content-Type: text/markdown
 
@@ -49,7 +48,10 @@
     print(contract)
 
 reading = await client.get_last_meter_reading(customer.bp_number, contracts[0].contract_id)
 print(reading)
 
 ```
 
+
+## Postman
+To use the API manually through Postman - read [Postman Collection Guide](POSTMAN.md)
```

