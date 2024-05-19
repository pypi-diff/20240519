# Comparing `tmp/pass_operator-0.3.2.tar.gz` & `tmp/pass_operator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pass_operator-0.3.2.tar", max compression
+gzip compressed data, was "pass_operator-0.4.0.tar", max compression
```

## Comparing `pass_operator-0.3.2.tar` & `pass_operator-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    35140 2024-02-14 14:54:19.812250 pass_operator-0.3.2/LICENSE
--rw-r--r--   0        0        0     7082 2024-02-14 14:54:19.812250 pass_operator-0.3.2/README.md
--rw-r--r--   0        0        0     1523 2024-02-14 14:54:33.576265 pass_operator-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-14 14:54:19.820250 pass_operator-0.3.2/src/__init__.py
--rw-r--r--   0        0        0     1562 2024-02-14 14:54:19.820250 pass_operator-0.3.2/src/operator/__init__.py
--rw-r--r--   0        0        0    12291 2024-02-14 14:54:19.820250 pass_operator-0.3.2/src/operator/daemon.py
--rw-r--r--   0        0        0     2005 2024-02-14 14:54:19.820250 pass_operator-0.3.2/src/operator/git.py
--rw-r--r--   0        0        0     1218 2024-02-14 14:54:19.820250 pass_operator-0.3.2/src/operator/gpg.py
--rw-r--r--   0        0        0    10990 2024-02-14 14:54:19.820250 pass_operator-0.3.2/src/operator/secret.py
--rw-r--r--   0        0        0     1313 2024-02-14 14:54:19.820250 pass_operator-0.3.2/src/operator/utils.py
--rw-r--r--   0        0        0     7898 1970-01-01 00:00:00.000000 pass_operator-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35140 2024-05-19 14:56:44.759517 pass_operator-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7833 2024-05-19 14:56:44.759517 pass_operator-0.4.0/README.md
+-rw-r--r--   0        0        0     1606 2024-05-19 14:56:57.055595 pass_operator-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1562 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/__init__.py
+-rw-r--r--   0        0        0    14494 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/daemon.py
+-rw-r--r--   0        0        0     2017 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/git.py
+-rw-r--r--   0        0        0     1218 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/gpg.py
+-rw-r--r--   0        0        0     8500 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/secret.py
+-rw-r--r--   0        0        0     1313 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/utils.py
+-rw-r--r--   0        0        0     8770 1970-01-01 00:00:00.000000 pass_operator-0.4.0/PKG-INFO
```

### Comparing `pass_operator-0.3.2/LICENSE` & `pass_operator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pass_operator-0.3.2/README.md` & `pass_operator-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 metadata:
   name: mysecret
   namespace: pass-operator-test
 spec:
   encryptedData:
     mykey: premiscale/mydata
   managedSecret:
-    name: mysecret
-    namespace: pass-operator-test
+    metadata:
+      name: mysecret
+      namespace: pass-operator-test
     type: Opaque
     immutable: false
 ```
 
 The above `PassSecret` manifest translates to the following `Secret`.
 
 ```yaml
@@ -174,27 +175,40 @@
 
 ### Private SSH key
 
 Now add a remote git repository and watch as `pass insert`-commands create local commits automatically. Sync your local password store with the remote repo via `pass git push`.
 
 ## Development
 
-### Testing
+### Unit tests
 
 Run unit tests with
 
 ```shell
-poetry run pytest tests/unit
+yarn test:unit
 ```
 
-e2e tests against a live environment with
+### End-to-end tests
+
+Run e2e tests against a live (local) environment with
 
 ```shell
-poetry run pytest tests/e2e
+yarn test:e2e
 ```
 
-And coverage against the codebase with
+This command will
+
+1. Stand up a local 1-node minikube cluster with 4 cores, 4GiB memory and 30GiB storage. *(Modify [./scripts/minikube.sh](./scripts/minikube.sh) if these resources are unsuitable for your local development environment.)*
+2. Create a `localhost` docker registry redirect container.
+3. Build both e2e (hosts a git repository with encrypted pass secrets that match paths found in [./src/test/data/crd](./src/test/data/crd/)) and operator container images, as well as push these images to the local redirect for minikube to access.
+4. Installs both e2e and pass-operator Helm charts.
+5. Run e2e tests.
+6. Tear down the cluster and local registry, as well as cleans up locally-built artifacts.
+
+### Coverage
+
+Test coverage against the codebase with
 
 ```shell
 poetry run coverage run -m pytest
 poetry run coverage report -m pytest
 ```
```

### Comparing `pass_operator-0.3.2/pyproject.toml` & `pass_operator-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 [tool.poetry]
 name = "pass-operator"
-version = "v0.3.2"
+version = "v0.4.0"
 description = "A kubernetes operator that syncs and decrypts secrets from pass git repositories"
 authors = ["Emma Doyle <emma@premiscale.com>"]
 maintainers = ["Emma Doyle <emma@premiscale.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
-packages = [{include = "src"}]
+packages = [
+  { include = "passoperator", from = "src" }
+]
 include = [
   "LICENSE"
 ]
-exclude = [
-  "src/test"
-]
 keywords = [
     "python",
     "kubernetes",
     "secrets",
     "operator",
     "pass"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 kubernetes = "^29.0.0"
-kopf = "^1.36.2"
+kopf = "^1.37.2"
 python-gnupg = "^0.5.2"
-gitpython = "^3.1.41"
+gitpython = "^3.1.43"
+pyhumps = "^3.8.0"
+attrs = "^23.2.0"
+cattrs = "^23.2.3"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
-poetry = "^1.5.1"
-mypy = "^1.0.1"
-pylint = "^3.0.3"
-pytest = "^7.4.4"
-coverage = "^7.4.1"
-deepdiff = "^6.7.1"
+poetry = "^1.8.3"
+mypy = "^1.10.0"
+pylint = "^3.2.1"
+pytest = "^8.2.0"
+coverage = "^7.5.1"
+deepdiff = "^7.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-passoperator = "src.operator.daemon:main"
+passoperator = "passoperator.daemon:main"
 
 [tool.mypy]
 python_version = "3.10"
 strict_optional = "true"
 ignore_missing_imports = "true"
 
 [tool.coverage.run]
@@ -54,16 +56,16 @@
 
 [tool.coverage.report]
 fail_under = 60
 
 [tool.pytest.ini_options]
 addopts = "--junitxml=./junit_test_results.xml"
 testpaths = [
-  "tests"
+  "src/tests/"
 ]
 
 [tool.pylint."MESSAGES CONTROL"]
-disable = "invalid-name,wrong-import-order,superfluous-parens,line-too-long,missing-final-newline,logging-fstring-interpolation,too-many-instance-attributes,unused-argument,unused-import"
+disable = "too-many-arguments,invalid-name,wrong-import-order,superfluous-parens,line-too-long,missing-final-newline,logging-fstring-interpolation,too-many-instance-attributes,unused-argument,unused-import"
 fail-under = 9
 
 [tool.pylint.MASTER]
 init-hook = "import sys; sys.path.append('.')"
```

### Comparing `pass_operator-0.3.2/src/operator/__init__.py` & `pass_operator-0.4.0/src/passoperator/__init__.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.3.2/src/operator/daemon.py` & `pass_operator-0.4.0/src/passoperator/daemon.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 """
-A kubernetes operator that syncs and decrypts secrets from Linux password store (https://www.passwordstore.org/) git repositories
+A kubernetes operator that syncs and decrypts secrets from Linux password store (https://www.passwordstore.org/) git repositories.
 """
 
 
-from typing import Any
+from typing import Any, List
 from pathlib import Path
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from importlib import metadata
 from kubernetes import client, config
 from http import HTTPStatus
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
-from src.operator.git import pull, clone
-from src.operator.utils import LogLevel
-from src.operator.secret import PassSecret, ManagedSecret
-from src.operator import env
+from time import sleep
+
+from passoperator.git import pull, clone
+from passoperator.utils import LogLevel
+from passoperator.secret import PassSecret, ManagedSecret
+from passoperator import env
 
 import asyncio
 import logging
 import sys
 import kopf
 
 
 __version__ = metadata.version('pass-operator')
 
 log = logging.getLogger(__name__)
 
 
 @kopf.on.startup()
-def start(**_: Any) -> None:
+def start(settings: kopf.OperatorSettings, **_: Any) -> None:
     """
     Set up operator runtime.
     """
     log.info(f'Starting operator version {__version__}')
+    settings.persistence.finalizer = 'secrets.premiscale.com/finalizer'
+    settings.persistence.progress_storage = kopf.AnnotationsProgressStorage(prefix='secrets.premiscale.com')
 
 
 @kopf.timer(
     # Target PassSecret.secrets.premiscale.com/v1alpha1
     'secrets.premiscale.com', 'v1alpha1', 'passsecret',
     # Interval to check every instance of a PassSecret.
     interval=float(env['OPERATOR_INTERVAL']),
@@ -56,53 +60,89 @@
 
     # Ensure the GPG key ID in ~/.password-store/${PASS_DIRECTORY}/.gpg-id did not change with the git update.
     check_gpg_id(
         path=f'{env["PASS_DIRECTORY"]}/.gpg-id'
     )
 
     # Create a new PassSecret object with an up-to-date managedSecret decrypted value from the pass store.
-    passSecret = PassSecret.from_dict(
-        manifest=dict(body)
-    )
+    passSecretObj = PassSecret.from_kopf(body)
 
-    log.info(f'Reconciling PassSecret "{passSecret.name}" managed Secret "{passSecret.managedSecret.name}" in Namespace "{passSecret.managedSecret.namespace}" against password store.')
+    log.info(
+        f'Reconciling PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}" against password store.'
+    )
 
     v1 = client.CoreV1Api()
 
     try:
         secret = v1.read_namespaced_secret(
-            name=passSecret.managedSecret.name,
-            namespace=passSecret.managedSecret.namespace
+            name=passSecretObj.spec.managedSecret.metadata.name,
+            namespace=passSecretObj.spec.managedSecret.metadata.namespace
         )
 
-        _managedSecret = ManagedSecret.from_client_dict(secret.to_dict())
+        log.debug(secret)
+        _managedSecret = ManagedSecret.from_kopf(secret.to_dict())
 
         # If the managed secret data does not match what's in the newly-generated ManagedSecret object,
         # submit a patch request to update it.
-        if not _managedSecret.data_equals(passSecret.managedSecret):
+        if not _managedSecret.data_equals(passSecretObj.spec.managedSecret):
             if _managedSecret.immutable:
-                raise kopf.TemporaryError(f'PassSecret "{passSecret.name}" managed secret "{PassSecret.managedSecret.name}" is immutable. Ignoring data patch.')
+                raise kopf.TemporaryError(
+                    f'PassSecret "{passSecretObj.metadata.name}" managed secret "{passSecretObj.spec.managedSecret.metadata.name}" is immutable. Ignoring data patch.'
+                )
 
             v1.patch_namespaced_secret(
-                name=passSecret.managedSecret.name,
-                namespace=passSecret.managedSecret.namespace,
+                name=passSecretObj.spec.managedSecret.metadata.name,
+                namespace=passSecretObj.spec.managedSecret.metadata.namespace,
                 body=client.V1Secret(
-                    **passSecret.managedSecret.to_client_dict()
+                    **passSecretObj.spec.managedSecret.to_client_dict(finalizers=False)
                 )
             )
 
-            log.info(f'Reconciliation successfully updated Secret "{_managedSecret.name}".')
+            log.info(f'Reconciliation successfully updated Secret "{_managedSecret.metadata.name}".')
     except client.ApiException as e:
         raise kopf.PermanentError(e)
 
 
 # @kopf.on.cleanup()
 # def cleanup(**kwargs) -> None:
 #     pass
 
+# @kopf.on.resume()
+# def resume(**kwargs) -> None:
+#     pass
+
+
+def lookup_managing_passsecret(managedSecretName: str) -> PassSecret | None:
+    """
+    Look up a PassSecret object by name and namespace.
+
+    Args:
+        managedSecretName [str]: name of the managed Secret to look up a PassSecret by, if it exists.
+
+    Returns:
+        PassSecret | None: the PassSecret object if found, else None.
+    """
+    v1 = client.CustomObjectsApi()
+
+    try:
+        passSecrets = v1.list_namespaced_custom_object(
+            group='secrets.premiscale.com',
+            version='v1alpha1',
+            namespace=env['OPERATOR_NAMESPACE'],
+            plural='passsecrets'
+        )
+
+        for passSecret in passSecrets['items']:
+            if passSecret['spec']['managedSecret']['metadata']['name'] == managedSecretName:
+                return PassSecret.from_kopf(passSecret)
+        else:
+            return None
+    except client.ApiException as e:
+        raise kopf.PermanentError(e)
+
 
 @kopf.on.update('secrets.premiscale.com', 'v1alpha1', 'passsecret')
 def update(old: kopf.BodyEssence | Any, new: kopf.BodyEssence | Any, meta: kopf.Meta, **_: Any) -> None:
     """
     An update was received on the PassSecret object, so attempt to update the corresponding Secret.
 
     This method is pretty much identical to 'create'-type events.
@@ -117,141 +157,143 @@
             'name': meta['name'],
             'namespace': meta['namespace']
         }
     }
 
     # Parse the old PassSecret manifest.
     try:
-        oldPassSecret = PassSecret.from_dict(
-            manifest={
+        oldPassSecret = PassSecret.from_kopf(
+            {
                 **metadata,
                 **old
             }
         )
     except (ValueError, KeyError) as e:
         raise kopf.PermanentError(e)
 
     # Parse the new PassSecret manifest.
     try:
-        newPassSecret = PassSecret.from_dict(
-            manifest={
+        newPassSecret = PassSecret.from_kopf(
+            {
                 **metadata,
                 **new
             }
         )
     except (ValueError, KeyError) as e:
         raise kopf.PermanentError(e)
 
     v1 = client.CoreV1Api()
 
+    # Handle typically immutable field changes separately from the rest of the manifest on Secrets.
     try:
-        if newPassSecret.managedSecret.namespace != oldPassSecret.managedSecret.namespace:
-            # Namespace is different. Delete the former secret and create a new one in the new namespace.
+        if newPassSecret.spec.managedSecret.metadata.namespace != oldPassSecret.spec.managedSecret.metadata.namespace or newPassSecret.spec.managedSecret.metadata.name != oldPassSecret.spec.managedSecret.metadata.name:
+            # Name or namespace is different. Delete the former secret and create a new one in the new namespace.
             v1.delete_namespaced_secret(
-                name=oldPassSecret.managedSecret.name,
-                namespace=oldPassSecret.managedSecret.namespace
+                name=oldPassSecret.spec.managedSecret.metadata.name,
+                namespace=oldPassSecret.spec.managedSecret.metadata.namespace
             )
 
             v1.create_namespaced_secret(
-                namespace=newPassSecret.managedSecret.namespace,
+                namespace=newPassSecret.spec.managedSecret.metadata.namespace,
                 body=client.V1Secret(
-                    **newPassSecret.managedSecret.to_client_dict()
+                    **newPassSecret.spec.managedSecret.to_client_dict(finalizers=False)
                 )
             )
         else:
-            # Namespace is the same, secret's being updated in-place.
+            # Name and namespace are the same, but the secret's being updated in-place.
             v1.patch_namespaced_secret(
-                name=oldPassSecret.name,
-                namespace=oldPassSecret.namespace,
+                name=newPassSecret.metadata.name,
+                namespace=oldPassSecret.metadata.namespace,
                 body=client.V1Secret(
-                    **newPassSecret.managedSecret.to_client_dict()
+                    **newPassSecret.spec.managedSecret.to_client_dict(finalizers=False)
                 )
             )
 
-        log.info(f'Successfully updated PassSecret "{newPassSecret.name}" managed Secret {newPassSecret.managedSecret.name}.')
+        log.info(
+            f'Successfully updated PassSecret "{newPassSecret.metadata.name}" managed Secret "{newPassSecret.spec.managedSecret.metadata.name}".'
+        )
     except client.ApiException as e:
         raise kopf.PermanentError(e)
 
 
 @kopf.on.create('secrets.premiscale.com', 'v1alpha1', 'passsecret')
 def create(body: kopf.Body, **_: Any) -> None:
     """
     Create a new Secret with the spec of the newly-created PassSecret.
 
     Args:
         body [kopf.Body]: raw body of the created PassSecret.
     """
     try:
-        secret = PassSecret.from_dict(
-            manifest=dict(body)
-        )
+        passSecretObj = PassSecret.from_kopf(body)
     except (ValueError, KeyError) as e:
         raise kopf.PermanentError(e)
 
-    log.info(f'PassSecret "{secret.name}" created')
+    log.info(f'PassSecret "{passSecretObj.metadata.name}" created')
 
     v1 = client.CoreV1Api()
 
     try:
         v1.create_namespaced_secret(
-            namespace=secret.managedSecret.namespace,
+            namespace=passSecretObj.spec.managedSecret.metadata.namespace,
             body=client.V1Secret(
-                **secret.managedSecret.to_client_dict()
+                **passSecretObj.spec.managedSecret.to_client_dict(finalizers=False)
             )
         )
-        log.info(f'Created PassSecret "{secret.name}" managed Secret "{secret.managedSecret.name}" in Namespace "{secret.managedSecret.namespace}"')
+        log.info(
+            f'Created PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}"'
+        )
     except client.ApiException as e:
         if e.status == HTTPStatus.CONFLICT:
-            raise kopf.TemporaryError(f'Duplicate PassSecret "{secret.name}" managed Secret "{secret.managedSecret.name}" in Namespace "{secret.managedSecret.namespace}". Skipping.')
+            raise kopf.TemporaryError(f'Duplicate PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}". Skipping.')
         raise kopf.PermanentError(e)
 
 
 @kopf.on.delete('secrets.premiscale.com', 'v1alpha1', 'passsecret')
 def delete(body: kopf.Body, **_: Any) -> None:
     """
     Remove a managed secret, as the managing PassSecret has been deleted.
 
     Args:
         body [kopf.Body]: raw body of the deleted PassSecret.
     """
     try:
-        secret = PassSecret.from_dict(
-            manifest=dict(body)
-        )
+        passSecretObj = PassSecret.from_kopf(body)
     except (ValueError, KeyError) as e:
         raise kopf.PermanentError(e)
 
-    log.info(f'PassSecret "{secret.name}" deleted')
+    log.info(f'PassSecret "{passSecretObj.metadata.name}" deleted')
 
     v1 = client.CoreV1Api()
 
     try:
         v1.delete_namespaced_secret(
-            name=secret.managedSecret.name,
-            namespace=secret.managedSecret.namespace
+            name=passSecretObj.spec.managedSecret.metadata.name,
+            namespace=passSecretObj.spec.managedSecret.metadata.namespace
         )
-        log.info(f'Deleted PassSecret "{secret.name}" managed Secret "{secret.managedSecret.name}" in Namespace "{secret.managedSecret.namespace}"')
+        log.info(f'Deleted PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}"')
     except client.ApiException as e:
         if e.status == HTTPStatus.NOT_FOUND:
-            log.warning(f'PassSecret "{secret.name}" managed Secret "{secret.managedSecret.name}" was not found. Skipping.')
+            log.warning(f'PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" was not found. Skipping.')
         raise kopf.PermanentError(e)
 
 
 def check_gpg_id(path: Path | str, remove: bool =False) -> None:
     """
     Ensure the gpg ID exists (leftover from 'pass init' in the entrypoint, or a git clone) and its contents match PASS_GPG_KEY_ID.
 
     Args:
         path [Path]: Path-like object to the .gpg-id file.
         remove [bool]: indicate whether or not to remove this file, should it exist.
     """
     if Path(path).exists():
         with open(path, mode='r', encoding='utf-8') as gpg_id_f:
-            if gpg_id_f.read().rstrip() != env['PASS_GPG_KEY_ID']:
-                log.error(f'PASS_GPG_KEY_ID ({env["PASS_GPG_KEY_ID"]}) does not equal .gpg-id contained in {path}')
+            _gpg_id = gpg_id_f.read().rstrip()
+            if _gpg_id != env['PASS_GPG_KEY_ID']:
+                log.error(f'PASS_GPG_KEY_ID ({env["PASS_GPG_KEY_ID"]}) does not equal .gpg-id contained in {path}: {_gpg_id}')
                 sys.exit(1)
 
         if remove:
             Path(path).unlink(missing_ok=False)
     else:
         log.error(f'.gpg-id at "{path}" does not exist. pass init failure')
         sys.exit(1)
@@ -288,15 +330,15 @@
         '--log-file', default='/opt/pass-operator/runtime.log', type=str,
         help='Log file location (if log-stdout is not provided).'
     )
 
     args = parser.parse_args()
 
     if args.version:
-        print(f'passoperator v{__version__}')
+        print(f'passoperator v{__version__}', file=sys.stdout)
         sys.exit(0)
 
     config.load_incluster_config()
 
     if not env['PASS_GIT_URL']:
         log.error('Must provide a valid git URL (PASS_GIT_URL)')
         sys.exit(1)
```

### Comparing `pass_operator-0.3.2/src/operator/git.py` & `pass_operator-0.4.0/src/passoperator/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Methods to interact minimally with a Git repository.
 """
 
 
 from git import Repo
 from git.exc import CommandError
 from time import sleep
-from src.operator import env
+from passoperator import env
 
 import logging
 import sys
 
 
 log = logging.getLogger(__name__)
 
@@ -25,15 +25,15 @@
     )
 
     # if env['PASS_GIT_BRANCH'] not in repo.branches:
     #     log.error(f'Branch "{env["PASS_GIT_BRANCH"]}" not found in project at URL "{env["PASS_GIT_URL"]}"')
     #     sys.exit(1)
 
     if str(repo.active_branch) != env['PASS_GIT_BRANCH']:
-        repo.git.checkout(env['PASS_GIT_BRANCH'])
+        repo.git.checkout('origin/' + env['PASS_GIT_BRANCH'])
 
     log.info(f'Successfully cloned repo {env["PASS_GIT_URL"]} to password store {env["PASS_DIRECTORY"]}')
 
 
 def pull(daemon: bool =False, retry: bool =False) -> None:
     """
     Blocking function that optionally runs 'git pull' in the cloned repository, repeatedly. This said, the
```

### Comparing `pass_operator-0.3.2/src/operator/gpg.py` & `pass_operator-0.4.0/src/passoperator/gpg.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.3.2/src/operator/secret.py` & `pass_operator-0.4.0/src/passoperator/secret.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,173 +1,136 @@
 """
 Provide interfaces for interacting with PassSecret manifests and encrypted data in a clean, OO-way.
 """
 
 
 from __future__ import annotations
-from typing import Dict
-from dataclasses import dataclass, field
+from typing import Dict, Final, List
 from pathlib import Path
-from src.operator.gpg import decrypt
-from src.operator.utils import b64Dec, b64Enc
-from src.operator import env
+from attrs import define, asdict as to_dict
+from cattrs import structure as from_dict
+from humps import camelize
+from datetime import datetime
+
+from passoperator.gpg import decrypt
+from passoperator.utils import b64Dec, b64Enc
+from passoperator import env
 
+import kopf
 import logging
 
 
 log = logging.getLogger(__name__)
 
 
-@dataclass
+@define
+class Metadata:
+    """
+    Metadata is the schema for the metadata field of a K8s object.
+    """
+    name: str
+    namespace: str = 'default'
+    annotations: Dict[str, str] | None = None
+    labels: Dict[str, str] | None = None
+
+    def to_dict(self) -> Dict:
+        """
+        Output this object as a K8s manifest dictionary.
+
+        Returns:
+            Dict: this object as a dict.
+        """
+        return to_dict(
+            self,
+            filter=lambda a, v: v is not None
+        )
+
+
+@define
 class ManagedSecret:
     """
     Logic for interacting with managed Secret objects.
     """
-    name: str
+    metadata: Metadata
     data: Dict[str, str] | None = None
     stringData: Dict[str, str] | None = None
-    namespace: str ='default'
-    immutable: bool =False
-    secretType: str ='Opaque'
-    kind: str ='Secret'
-    apiGroup: str =''
-    apiVersion: str ='v1'
+    immutable: bool = False
+    type: str = 'Opaque'
+    kind: Final[str] = 'Secret'
+    apiVersion: Final[str] = 'v1'
+    finalizers: List[str] = []
 
-    def __post_init__(self) -> None:
+    def __attrs_post_init__(self) -> None:
         if not self.data and not self.stringData:
-            raise RuntimeError('ManagedSecret type expects at least one of \'data\', \'stringData\', to be set.')
+            return None
 
         # Propagate one field to the other, make sure they match despite b64 conversion.
         if self.stringData and self.data:
             # Ensure stringData and data contain the same keys & values by iterating over both if both are set independently.
             for key in self.stringData:
                 if key not in self.data:
                     self.data[key] = b64Enc(self.stringData[key])
                 else:
-                    assert b64Dec(self.data[key]) == self.stringData[key]
+                    assert self.data[key] == b64Enc(self.stringData[key])
             for key in self.data:
                 if key not in self.stringData:
                     self.stringData[key] = b64Dec(self.data[key])
                 else:
-                    assert b64Enc(self.stringData[key]) == self.data[key]
+                    assert self.stringData[key] == b64Dec(self.data[key])
 
         elif self.data and not self.stringData:
             self.stringData = {
                 key: b64Dec(value) for key, value in self.data.items()
             }
 
         elif self.stringData and not self.data:
             self.data = {
                 key: b64Enc(value) for key, value in self.stringData.items()
             }
 
-    @classmethod
-    def from_dict(cls, manifest: Dict) -> ManagedSecret:
-        """
-        Parse a k8s manifest into a ManagedSecret (Secret) dataclass.
+        # Ensure the managed secret is marked as managed and has a last-updated timestamp.
+        if self.metadata.annotations is None:
+            self.metadata.annotations = {}
 
-        Args:
-            manifest (Dict): a Secret manifest.
-
-        Returns:
-            ManagedSecret: a ManagedSecret created from parsing the contents of the manifest.
+        self.metadata.annotations['secrets.premiscale.com/managed'] = 'true'
+        self.metadata.annotations['secrets.premiscale.com/last-updated'] = datetime.now().isoformat()
 
-        Raises:
-            KeyError, ValueError: if expected keys are not present during dictionary unpacking.
-        """
-        # TODO: manage managed secrets' labels and annotations.
-        # if 'annotations' in manifest and len(manifest['annotations']):
-        #     annotations = manifest['annotations']
-        # else:
-        #     annotations = {}
-
-        # if 'labels' in manifest and len(manifest['labels']):
-        #     labels = manifest['labels']
-        # else:
-        #     labels = {}
-
-        return cls(
-            name=manifest['metadata']['name'],
-            namespace=manifest['metadata']['namespace'],
-            data=manifest['data'],
-            stringData=manifest['stringData'],
-            immutable=manifest['immutable'],
-            secretType=manifest['type']
-        )
+        return None
 
-    def to_dict(self) -> Dict:
+    def to_dict(self, export: bool = False) -> Dict:
         """
         Output this object as a k8s manifest dictionary.
 
+        Args:
+            export (bool): if True, export the object as a dict without the apiGroup and duplicate data keys.
+
         Returns:
             Dict: this object as a dict.
         """
-        return {
-            'apiVersion': self.apiVersion, # f'{self.apiGroup}/{self.apiVersion}' if self.apiGroup else self.apiVersion,
-            'kind': self.kind,
-            'metadata': {
-                'name': self.name,
-                'namespace': self.namespace
-                # TODO: labels and annotations, at a future date.
-            },
-            'data': self.data,
-            'immutable': self.immutable,
-            'type': self.secretType
-        }
-
-    @classmethod
-    def from_client_dict(cls, manifest: Dict) -> ManagedSecret:
-        """
-        Parse a k8s manifest from the kubernetes Python client package into a ManagedSecret (Secret)
-        dataclass. Primary difference is naming of the keys.
+        d = to_dict(self, filter=lambda a, v: v is not None and v is not False)
 
-        Args:
-            manifest (Dict): a Secret manifest.
+        if export:
+            d.pop('stringData')
 
-        Returns:
-            ManagedSecret: a ManagedSecret created from parsing the contents of the manifest.
+        return d
 
-        Raises:
-            KeyError, ValueError: if expected keys are not present during dictionary unpacking.
-        """
-        # TODO: manage managed secrets' labels and annotations.
-        # if 'annotations' in manifest and len(manifest['annotations']):
-        #     annotations = manifest['annotations']
-        # else:
-        #     annotations = {}
-
-        # if 'labels' in manifest and len(manifest['labels']):
-        #     labels = manifest['labels']
-        # else:
-        #     labels = {}
-
-        return cls(
-            name=manifest['metadata']['name'],
-            namespace=manifest['metadata']['namespace'],
-            data=manifest['data'],
-            stringData=manifest['string_data'],  # This is the only change from the method above, unfortunately.
-            immutable=manifest['immutable'],
-            secretType=manifest['type']
-        )
-
-    def to_client_dict(self) -> Dict:
+    def to_client_dict(self, finalizers: bool = False) -> Dict:
         """
         Output this secret to a dictionary with keys that match the arguments of kubernetes.client.V1Secret, for convenience.
+
+        Args:
+            finalizers (bool): if True, include the finalizers field in the output.
         """
-        return {
-            'api_version': f'{self.apiGroup}/{self.apiVersion}' if self.apiGroup else self.apiVersion,
-            'kind': self.kind,
-            'metadata': {
-                'name': self.name,
-                'namespace': self.namespace,
-            },
-            'string_data': self.stringData,
-            'type': self.secretType,
-            'immutable': self.immutable
-        }
+        d = dict(self.to_dict(export=True))
+        d.pop('data')
+        d.pop('apiVersion')
+        if not finalizers:
+            d.pop('finalizers')
+        d['string_data'] = self.stringData
+        return d
 
     def __eq__(self, __value: object) -> bool:
         """
         Compare two ManagedSecrets.
 
         Returns:
             bool: whether or not the ManagedSecrets as dictionaries equal one another.
@@ -184,138 +147,134 @@
             __value (ManagedSecret): another ManagedSecret object to compare against.
 
         Returns:
             bool: whether or not the ManagedSecrets' contained data are equal.
         """
         return self.data == __value.data
 
-
-@dataclass
-class PassSecret:
-    """
-    Manage PassSecret data in a clean, interoperable way.
-    """
-
-    # PassSecret objects require our set of environment variables because we need to decrypt the contents
-    # in order to instantiate a ManagedSecret object.
-    name: str
-    managedSecretName: str
-    encryptedData: Dict[str, str]
-    annotations: Dict[str, str] | None = None
-    labels: Dict[str, str] | None = None
-    namespace: str ='default'
-    kind: str ='PassSecret'
-    apiGroup: str ='secrets.premiscale.com'
-    apiVersion: str ='v1alpha1'
-
-    managedSecret: ManagedSecret = field(init=False)
-    managedSecretNamespace: str ='default'
-    managedSecretType: str ='Opaque'
-    managedSecretImmutable: bool =False
-
-    def __post_init__(self) -> None:
-        if (decryptedData := self._decrypt()) is None:
-            raise ValueError(f'Could not decrypt data on PassSecret {self.name}. Do you need to set a passphrase?')
-
-        self.managedSecret = ManagedSecret(
-            name=self.managedSecretName,
-            namespace=self.managedSecretNamespace,
-            stringData=decryptedData,
-            immutable=self.managedSecretImmutable,
-            secretType=self.managedSecretType
-        )
-
-    def to_dict(self) -> Dict:
-        """
-        Output this object as a K8s manifest dictionary.
-
-        Returns:
-            Dict: this object as a dict.
-        """
-        return {
-            'apiVersion': f'{self.apiGroup}/{self.apiVersion}',
-            'kind': self.kind,
-            'metadata': {
-                'name': self.name,
-                'namespace': self.namespace,
-                'annotations': self.annotations,
-                'labels': self.labels
-            },
-            'spec': {
-                'encryptedData': self.encryptedData,
-                'managedSecret': {
-                    'name': self.managedSecret.name,
-                    'namespace': self.managedSecret.namespace,
-                    'type': self.managedSecret.secretType,
-                    'immutable': self.managedSecret.immutable
-                }
-            }
-        }
-
     @classmethod
-    def from_dict(cls, manifest: Dict) -> PassSecret:
+    def from_kopf(cls, body: kopf.Body | Dict) -> ManagedSecret:
         """
-        Parse a k8s manifest into a PassSecret dataclass.
+        Create a ManagedSecret object from a K8s body dict.
 
         Args:
-            manifest (Dict): the PassSecret manifest dictionary to parse into the dataclass.
+            body (kopf.Body | Dict): the K8s manifest.
 
-        Raises:
-            KeyError, ValueError: if expected keys are not present during dictionary unpacking.
+        Returns:
+            ManagedSecret: the ManagedSecret object created from the manifest.
         """
-        if 'annotations' in manifest and len(manifest['annotations']):
-            annotations = manifest['annotations']
-        else:
-            annotations = {}
-
-        if 'labels' in manifest and len(manifest['labels']):
-            labels = manifest['labels']
-        else:
-            labels = {}
-
-        if 'immutable' not in manifest['spec']['managedSecret']:
-            manifest['spec']['managedSecret']['immutable'] = False
-
-        return cls(
-            name=manifest['metadata']['name'],
-            namespace=manifest['metadata']['namespace'],
-            encryptedData=manifest['spec']['encryptedData'],
-            labels=labels,
-            annotations=annotations,
-            # Parse out managed secret fields into arguments.
-            managedSecretName=manifest['spec']['managedSecret']['name'],
-            managedSecretNamespace=manifest['spec']['managedSecret']['namespace'],
-            managedSecretType=manifest['spec']['managedSecret']['type'],
-            managedSecretImmutable=manifest['spec']['managedSecret']['immutable'],
+
+        # Camelize the body to match the PassSecret object's fields, but keep the data fields as-is.
+        camelized_body = dict(camelize(dict(body)))
+        camelized_body['data'] = dict(body)['data']
+
+        return from_dict(
+            camelized_body,
+            cls
         )
 
-    def _decrypt(self) -> Dict[str, str] | None:
-        """
-        Decrypt the contents of this PassSecret's paths and store them on an attribute
 
-        Returns:
-            Optional[Dict[str, str]]: a dictionary of data keys and decrypted paths' values. If decryption was not possible, None.
+@define
+class PassSecretSpec:
+    """
+    PassSecretSpec is the schema for the spec field of a PassSecret object. It also handles decrypting the encrypted data on
+    the PassSecret object.
+    """
+    encryptedData: Dict[str, str]
+    managedSecret: ManagedSecret
+
+    def __attrs_post_init__(self) -> None:
+        # Post-process the managedSecret field to decrypt the contents of the managedSecret.
+        self.managedSecret = self.decrypt(self.managedSecret, self.encryptedData)
+
+    @staticmethod
+    def decrypt(ms: ManagedSecret, encryptedData: Dict[str, str]) -> ManagedSecret:
+        """
+        Decrypt the contents of this PassSecret's paths before returning the spec object.
         """
         stringData = {}
 
-        for secretKey in self.encryptedData:
-            secretPath = self.encryptedData[secretKey]
+        for secretKey in encryptedData:
+            secretPath = encryptedData[secretKey]
 
             decryptedSecret = decrypt(
                 Path(f'{env["PASS_DIRECTORY"]}/{secretPath}'),
                 passphrase=env['PASS_GPG_PASSPHRASE']
             )
 
             if decryptedSecret:
                 stringData[secretKey] = decryptedSecret
             else:
-                return None
+                log.error(f'Failed to decrypt secret at path: {secretPath}')
+                stringData[secretKey] = ''
+
+        return ManagedSecret(
+            metadata=ms.metadata,
+            stringData=stringData,
+            immutable=ms.immutable,
+            type=ms.type
+        )
 
-        return stringData
+    def to_dict(self) -> Dict:
+        """
+        Output this object as a K8s manifest dictionary.
+
+        Returns:
+            Dict: this object as a dict.
+        """
+        return {
+            'encryptedData': self.encryptedData,
+            'managedSecret': self.managedSecret.to_dict(export=True)
+        }
+
+
+@define
+class PassSecret:
+    """
+    Manage PassSecret data in a clean, interoperable way.
+    """
+    metadata: Metadata
+    spec: PassSecretSpec
+    kind: Final[str] = 'PassSecret'
+    apiVersion: Final[str] = 'secrets.premiscale.com/v1alpha1'
+
+    def to_dict(self) -> Dict:
+        """
+        Output this object as a K8s manifest dictionary.
+
+        Returns:
+            Dict: this object as a dict.
+        """
+        return {
+            'apiVersion': self.apiVersion,
+            'kind': self.kind,
+            'metadata': self.metadata.to_dict(),
+            'spec': self.spec.to_dict()
+        }
 
     def __eq__(self, __value: object) -> bool:
         """
         Compare two PassSecrets.
         """
         if isinstance(__value, PassSecret):
             return self.to_dict() == __value.to_dict()
-        return False
+        return False
+
+    @classmethod
+    def from_kopf(cls, body: kopf.Body | Dict) -> PassSecret:
+        """
+        Create a PassSecret object from a K8s body dict.
+
+        Args:
+            body (kopf.Body | Dict): the body of a K8s object.
+
+        Returns:
+            PassSecret: the PassSecret object created from the body.
+        """
+        # Camelize the body to match the PassSecret object's fields, but keep the encryptedData field as-is.
+        camelized_body = dict(camelize(dict(body)))
+        camelized_body['spec']['encryptedData'] = dict(body)['spec']['encryptedData']
+
+        return from_dict(
+            camelized_body,
+            cls
+        )
```

### Comparing `pass_operator-0.3.2/src/operator/utils.py` & `pass_operator-0.4.0/src/passoperator/utils.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.3.2/PKG-INFO` & `pass_operator-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: pass-operator
-Version: 0.3.2
+Version: 0.4.0
 Summary: A kubernetes operator that syncs and decrypts secrets from pass git repositories
 License: GPL-3.0-or-later
 Keywords: python,kubernetes,secrets,operator,pass
 Author: Emma Doyle
 Author-email: emma@premiscale.com
 Maintainer: Emma Doyle
 Maintainer-email: emma@premiscale.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: gitpython (>=3.1.41,<4.0.0)
-Requires-Dist: kopf (>=1.36.2,<2.0.0)
+Requires-Dist: attrs (>=23.2.0,<24.0.0)
+Requires-Dist: cattrs (>=23.2.3,<24.0.0)
+Requires-Dist: gitpython (>=3.1.43,<4.0.0)
+Requires-Dist: kopf (>=1.37.2,<2.0.0)
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0)
+Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: python-gnupg (>=0.5.2,<0.6.0)
 Description-Content-Type: text/markdown
 
 # `pass` secrets operator
 
 A Kubernetes operator to sync and decrypt secrets from a password store ([pass](https://www.passwordstore.org/)) Git repository. This operator is proposed as a proof-of-concept and shouldn't be used in any production capacity.
 
@@ -47,16 +50,17 @@
 metadata:
   name: mysecret
   namespace: pass-operator-test
 spec:
   encryptedData:
     mykey: premiscale/mydata
   managedSecret:
-    name: mysecret
-    namespace: pass-operator-test
+    metadata:
+      name: mysecret
+      namespace: pass-operator-test
     type: Opaque
     immutable: false
 ```
 
 The above `PassSecret` manifest translates to the following `Secret`.
 
 ```yaml
@@ -195,28 +199,41 @@
 
 ### Private SSH key
 
 Now add a remote git repository and watch as `pass insert`-commands create local commits automatically. Sync your local password store with the remote repo via `pass git push`.
 
 ## Development
 
-### Testing
+### Unit tests
 
 Run unit tests with
 
 ```shell
-poetry run pytest tests/unit
+yarn test:unit
 ```
 
-e2e tests against a live environment with
+### End-to-end tests
+
+Run e2e tests against a live (local) environment with
 
 ```shell
-poetry run pytest tests/e2e
+yarn test:e2e
 ```
 
-And coverage against the codebase with
+This command will
+
+1. Stand up a local 1-node minikube cluster with 4 cores, 4GiB memory and 30GiB storage. *(Modify [./scripts/minikube.sh](./scripts/minikube.sh) if these resources are unsuitable for your local development environment.)*
+2. Create a `localhost` docker registry redirect container.
+3. Build both e2e (hosts a git repository with encrypted pass secrets that match paths found in [./src/test/data/crd](./src/test/data/crd/)) and operator container images, as well as push these images to the local redirect for minikube to access.
+4. Installs both e2e and pass-operator Helm charts.
+5. Run e2e tests.
+6. Tear down the cluster and local registry, as well as cleans up locally-built artifacts.
+
+### Coverage
+
+Test coverage against the codebase with
 
 ```shell
 poetry run coverage run -m pytest
 poetry run coverage report -m pytest
 ```
```

