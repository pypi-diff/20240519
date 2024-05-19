# Comparing `tmp/wttech_aem-0.9.0.tar.gz` & `tmp/wttech_aem-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wttech_aem-0.9.0.tar", last modified: Sun Apr  7 22:22:56 2024, max compression
+gzip compressed data, was "wttech_aem-0.9.1.tar", last modified: Sun Apr  7 23:33:01 2024, max compression
```

## Comparing `wttech_aem-0.9.0.tar` & `wttech_aem-0.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dominik.przybyl   (502) staff       (20)        0 2024-04-07 22:22:56.078823 wttech_aem-0.9.0/
--rw-r--r--   0 dominik.przybyl   (502) staff       (20)     5532 2024-04-07 22:22:56.077480 wttech_aem-0.9.0/PKG-INFO
--rw-r--r--   0 dominik.przybyl   (502) staff       (20)     5319 2024-04-07 22:22:54.000000 wttech_aem-0.9.0/README.md
--rw-r--r--   0 dominik.przybyl   (502) staff       (20)       38 2024-04-07 22:22:56.078951 wttech_aem-0.9.0/setup.cfg
--rw-------   0 dominik.przybyl   (502) staff       (20)     1002 2024-04-07 22:22:55.000000 wttech_aem-0.9.0/setup.py
-drwxr-xr-x   0 dominik.przybyl   (502) staff       (20)        0 2024-04-07 22:22:56.028384 wttech_aem-0.9.0/wttech_aem/
--rw-------   0 dominik.przybyl   (502) staff       (20)      786 2024-04-07 22:22:54.000000 wttech_aem-0.9.0/wttech_aem/__init__.py
--rw-------   0 dominik.przybyl   (502) staff       (20)     9269 2024-04-07 22:22:54.000000 wttech_aem-0.9.0/wttech_aem/_utilities.py
-drwxr-xr-x   0 dominik.przybyl   (502) staff       (20)        0 2024-04-07 22:22:56.072470 wttech_aem-0.9.0/wttech_aem/compose/
--rw-------   0 dominik.przybyl   (502) staff       (20)      320 2024-04-07 22:22:54.000000 wttech_aem-0.9.0/wttech_aem/compose/__init__.py
--rw-------   0 dominik.przybyl   (502) staff       (20)    14453 2024-04-07 22:22:54.000000 wttech_aem-0.9.0/wttech_aem/compose/_inputs.py
--rw-------   0 dominik.przybyl   (502) staff       (20)     9345 2024-04-07 22:22:54.000000 wttech_aem-0.9.0/wttech_aem/compose/instance.py
--rw-------   0 dominik.przybyl   (502) staff       (20)    13589 2024-04-07 22:22:54.000000 wttech_aem-0.9.0/wttech_aem/compose/outputs.py
--rw-------   0 dominik.przybyl   (502) staff       (20)     2723 2024-04-07 22:22:54.000000 wttech_aem-0.9.0/wttech_aem/provider.py
--rw-------   0 dominik.przybyl   (502) staff       (20)       97 2024-04-07 22:22:55.000000 wttech_aem-0.9.0/wttech_aem/pulumi-plugin.json
--rw-------   0 dominik.przybyl   (502) staff       (20)        0 2024-04-07 22:22:54.000000 wttech_aem-0.9.0/wttech_aem/py.typed
-drwxr-xr-x   0 dominik.przybyl   (502) staff       (20)        0 2024-04-07 22:22:56.075431 wttech_aem-0.9.0/wttech_aem.egg-info/
--rw-r--r--   0 dominik.przybyl   (502) staff       (20)     5532 2024-04-07 22:22:55.000000 wttech_aem-0.9.0/wttech_aem.egg-info/PKG-INFO
--rw-r--r--   0 dominik.przybyl   (502) staff       (20)      463 2024-04-07 22:22:56.000000 wttech_aem-0.9.0/wttech_aem.egg-info/SOURCES.txt
--rw-r--r--   0 dominik.przybyl   (502) staff       (20)        1 2024-04-07 22:22:55.000000 wttech_aem-0.9.0/wttech_aem.egg-info/dependency_links.txt
--rw-r--r--   0 dominik.przybyl   (502) staff       (20)        1 2024-04-07 22:22:55.000000 wttech_aem-0.9.0/wttech_aem.egg-info/not-zip-safe
--rw-r--r--   0 dominik.przybyl   (502) staff       (20)       50 2024-04-07 22:22:55.000000 wttech_aem-0.9.0/wttech_aem.egg-info/requires.txt
--rw-r--r--   0 dominik.przybyl   (502) staff       (20)       11 2024-04-07 22:22:55.000000 wttech_aem-0.9.0/wttech_aem.egg-info/top_level.txt
+drwxr-xr-x   0 dominik.przybyl   (502) staff       (20)        0 2024-04-07 23:33:01.351400 wttech_aem-0.9.1/
+-rw-r--r--   0 dominik.przybyl   (502) staff       (20)     6662 2024-04-07 23:33:01.350915 wttech_aem-0.9.1/PKG-INFO
+-rw-r--r--   0 dominik.przybyl   (502) staff       (20)     6449 2024-04-07 23:33:00.000000 wttech_aem-0.9.1/README.md
+-rw-r--r--   0 dominik.przybyl   (502) staff       (20)       38 2024-04-07 23:33:01.351465 wttech_aem-0.9.1/setup.cfg
+-rw-------   0 dominik.przybyl   (502) staff       (20)     1002 2024-04-07 23:33:01.000000 wttech_aem-0.9.1/setup.py
+drwxr-xr-x   0 dominik.przybyl   (502) staff       (20)        0 2024-04-07 23:33:01.321832 wttech_aem-0.9.1/wttech_aem/
+-rw-------   0 dominik.przybyl   (502) staff       (20)      786 2024-04-07 23:33:00.000000 wttech_aem-0.9.1/wttech_aem/__init__.py
+-rw-------   0 dominik.przybyl   (502) staff       (20)     9269 2024-04-07 23:33:00.000000 wttech_aem-0.9.1/wttech_aem/_utilities.py
+drwxr-xr-x   0 dominik.przybyl   (502) staff       (20)        0 2024-04-07 23:33:01.349304 wttech_aem-0.9.1/wttech_aem/compose/
+-rw-------   0 dominik.przybyl   (502) staff       (20)      320 2024-04-07 23:33:00.000000 wttech_aem-0.9.1/wttech_aem/compose/__init__.py
+-rw-------   0 dominik.przybyl   (502) staff       (20)    14453 2024-04-07 23:33:00.000000 wttech_aem-0.9.1/wttech_aem/compose/_inputs.py
+-rw-------   0 dominik.przybyl   (502) staff       (20)     9345 2024-04-07 23:33:00.000000 wttech_aem-0.9.1/wttech_aem/compose/instance.py
+-rw-------   0 dominik.przybyl   (502) staff       (20)    13589 2024-04-07 23:33:00.000000 wttech_aem-0.9.1/wttech_aem/compose/outputs.py
+-rw-------   0 dominik.przybyl   (502) staff       (20)     2723 2024-04-07 23:33:00.000000 wttech_aem-0.9.1/wttech_aem/provider.py
+-rw-------   0 dominik.przybyl   (502) staff       (20)       97 2024-04-07 23:33:01.000000 wttech_aem-0.9.1/wttech_aem/pulumi-plugin.json
+-rw-------   0 dominik.przybyl   (502) staff       (20)        0 2024-04-07 23:33:01.000000 wttech_aem-0.9.1/wttech_aem/py.typed
+drwxr-xr-x   0 dominik.przybyl   (502) staff       (20)        0 2024-04-07 23:33:01.350245 wttech_aem-0.9.1/wttech_aem.egg-info/
+-rw-r--r--   0 dominik.przybyl   (502) staff       (20)     6662 2024-04-07 23:33:01.000000 wttech_aem-0.9.1/wttech_aem.egg-info/PKG-INFO
+-rw-r--r--   0 dominik.przybyl   (502) staff       (20)      463 2024-04-07 23:33:01.000000 wttech_aem-0.9.1/wttech_aem.egg-info/SOURCES.txt
+-rw-r--r--   0 dominik.przybyl   (502) staff       (20)        1 2024-04-07 23:33:01.000000 wttech_aem-0.9.1/wttech_aem.egg-info/dependency_links.txt
+-rw-r--r--   0 dominik.przybyl   (502) staff       (20)        1 2024-04-07 23:33:01.000000 wttech_aem-0.9.1/wttech_aem.egg-info/not-zip-safe
+-rw-r--r--   0 dominik.przybyl   (502) staff       (20)       50 2024-04-07 23:33:01.000000 wttech_aem-0.9.1/wttech_aem.egg-info/requires.txt
+-rw-r--r--   0 dominik.przybyl   (502) staff       (20)       11 2024-04-07 23:33:01.000000 wttech_aem-0.9.1/wttech_aem.egg-info/top_level.txt
```

### Comparing `wttech_aem-0.9.0/PKG-INFO` & `wttech_aem-0.9.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,11 @@
-Metadata-Version: 2.1
-Name: wttech_aem
-Version: 0.9.0
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: parver>=0.2.1
-Requires-Dist: pulumi<4.0.0,>=3.56.0
-Requires-Dist: semver>=2.8.1
+[![AEM Compose Logo](https://github.com/wttech/pulumi-aem/raw/main/docs/logo-with-text.png)](https://github.com/wttech/aemc)
+[![WTT Logo](https://github.com/wttech/pulumi-aem/raw/main/docs/wtt-logo.png)](https://www.wundermanthompson.com/service/technology)
 
-![AEM Compose Logo](docs/logo-with-text.png)
-[![WTT Logo](docs/wtt-logo.png)](https://www.wundermanthompson.com/service/technology)
-
-[![Apache License, Version 2.0, January 2004](docs/apache-license-badge.svg)](http://www.apache.org/licenses/)
+[![Apache License, Version 2.0, January 2004](https://github.com/wttech/pulumi-aem/raw/main/docs/apache-license-badge.svg)](http://www.apache.org/licenses/)
 
 # AEM Compose - Pulumi Native Provider
 
 This provider allows development teams to easily set up [Adobe Experience Manager (AEM)](https://business.adobe.com/products/experience-manager/adobe-experience-manager.html) instances on virtual machines in the cloud (AWS, Azure, GCP, etc.) or bare metal machines.
 It's based on the [AEM Compose](https://github.com/wttech/aemc) tool and aims to simplify the process of creating AEM environments without requiring deep DevOps knowledge.
 
 Published in [Pulumi Registry](https://www.pulumi.com/registry/packages/aem/).
@@ -36,22 +27,28 @@
 - Based on the powerful [AEM Compose](https://github.com/wttech/aemc) tool
 
 ## Quickstart
 
 The easiest way to get started is to review, copy and adapt provided examples:
 
 1. AWS EC2 instance with private IP
-   * [Node.js](examples/nodejs_aws_ssm)
-   * [GoLang](examples/go_aws_ssm)
+   * [Go](https://github.com/wttech/pulumi-aem/tree/main/examples/go_aws_ssm)
+   * [NodeJS](https://github.com/wttech/pulumi-aem/tree/main/examples/nodejs_aws_ssm)
+   * [Python](https://github.com/wttech/pulumi-aem/tree/main/examples/python_aws_ssm)
+   * [.NET](https://github.com/wttech/pulumi-aem/tree/main/examples/dotnet_aws_ssm)
 2. AWS EC2 instance with public IP
-   * [Node.js](examples/nodejs_aws_ssh)
-   * [GoLang](examples/go_aws_ssh)
+   * [Go](https://github.com/wttech/pulumi-aem/tree/main/examples/go_aws_ssh)
+   * [NodeJS](https://github.com/wttech/pulumi-aem/tree/main/examples/nodejs_aws_ssh)
+   * [Python](https://github.com/wttech/pulumi-aem/tree/main/examples/python_aws_ssh)
+   * [.NET](https://github.com/wttech/pulumi-aem/tree/main/examples/dotnet_aws_ssh)
 3. Bare metal machine
-   * [Node.js](examples/nodejs_bare_metal)
-   * [GoLang](examples/go_bare_metal)
+   * [Go](https://github.com/wttech/pulumi-aem/tree/main/examples/go_bare_metal)
+   * [NodeJS](https://github.com/wttech/pulumi-aem/tree/main/examples/nodejs_bare_metal)
+   * [Python](https://github.com/wttech/pulumi-aem/tree/main/examples/python_bare_metal)
+   * [.NET](https://github.com/wttech/pulumi-aem/tree/main/examples/dotnet_bare_metal)
 
 - - -
 
 ## Development
 
 This repository is showing how to create and locally test a native Pulumi provider.
 
@@ -64,18 +61,20 @@
 #### Prerequisites
 
 Prerequisites for this repository are already satisfied by the [Pulumi Devcontainer](https://github.com/pulumi/devcontainer) if you are using Github Codespaces, or VSCode.
 
 If you are not using VSCode, you will need to ensure the following tools are installed and present in your `$PATH`:
 
 * [`pulumictl`](https://github.com/pulumi/pulumictl#installation)
-* [Go 1.21](https://golang.org/dl/) or 1.latest
+* [Go](https://golang.org/dl/) or 1.latest
 * [NodeJS](https://nodejs.org/en/) 14.x.  We recommend using [nvm](https://github.com/nvm-sh/nvm) to manage NodeJS installations.
 * [Yarn](https://yarnpkg.com/)
 * [TypeScript](https://www.typescriptlang.org/)
+* [Python](https://www.python.org/downloads/) (called as `python3`).  For recent versions of MacOS, the system-installed version is fine.
+* [.NET](https://dotnet.microsoft.com/download)
 
 
 #### Build & test the AEM provider
 
 1. Create a new Github CodeSpaces environment using this repository.
 1. Open a terminal in the CodeSpaces environment.
 1. Run `make build install` to build and install the provider.
@@ -84,24 +83,24 @@
 1. Run `make down` to tear down the example program.
 
 ##### Build the provider and install the plugin
 
    ```bash
    $ make build install
    ```
-   
+
 This will:
 
 1. Create the SDK codegen binary and place it in a `./bin` folder (gitignored)
 2. Create the provider binary and place it in the `./bin` folder (gitignored)
 3. Generate the dotnet, Go, Node, and Python SDKs and place them in the `./sdk` folder
 4. Install the provider on your machine.
 
 ##### Test against the example
-   
+
 ```bash
 $ cd examples/simple
 $ yarn link @wttech/aem
 $ yarn install
 $ pulumi stack init test
 $ pulumi up
 ```
```

### Comparing `wttech_aem-0.9.0/README.md` & `wttech_aem-0.9.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,20 @@
-![AEM Compose Logo](docs/logo-with-text.png)
-[![WTT Logo](docs/wtt-logo.png)](https://www.wundermanthompson.com/service/technology)
+Metadata-Version: 2.1
+Name: wttech_aem
+Version: 0.9.1
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: parver>=0.2.1
+Requires-Dist: pulumi<4.0.0,>=3.56.0
+Requires-Dist: semver>=2.8.1
 
-[![Apache License, Version 2.0, January 2004](docs/apache-license-badge.svg)](http://www.apache.org/licenses/)
+[![AEM Compose Logo](https://github.com/wttech/pulumi-aem/raw/main/docs/logo-with-text.png)](https://github.com/wttech/aemc)
+[![WTT Logo](https://github.com/wttech/pulumi-aem/raw/main/docs/wtt-logo.png)](https://www.wundermanthompson.com/service/technology)
+
+[![Apache License, Version 2.0, January 2004](https://github.com/wttech/pulumi-aem/raw/main/docs/apache-license-badge.svg)](http://www.apache.org/licenses/)
 
 # AEM Compose - Pulumi Native Provider
 
 This provider allows development teams to easily set up [Adobe Experience Manager (AEM)](https://business.adobe.com/products/experience-manager/adobe-experience-manager.html) instances on virtual machines in the cloud (AWS, Azure, GCP, etc.) or bare metal machines.
 It's based on the [AEM Compose](https://github.com/wttech/aemc) tool and aims to simplify the process of creating AEM environments without requiring deep DevOps knowledge.
 
 Published in [Pulumi Registry](https://www.pulumi.com/registry/packages/aem/).
@@ -27,22 +36,28 @@
 - Based on the powerful [AEM Compose](https://github.com/wttech/aemc) tool
 
 ## Quickstart
 
 The easiest way to get started is to review, copy and adapt provided examples:
 
 1. AWS EC2 instance with private IP
-   * [Node.js](examples/nodejs_aws_ssm)
-   * [GoLang](examples/go_aws_ssm)
+   * [Go](https://github.com/wttech/pulumi-aem/tree/main/examples/go_aws_ssm)
+   * [NodeJS](https://github.com/wttech/pulumi-aem/tree/main/examples/nodejs_aws_ssm)
+   * [Python](https://github.com/wttech/pulumi-aem/tree/main/examples/python_aws_ssm)
+   * [.NET](https://github.com/wttech/pulumi-aem/tree/main/examples/dotnet_aws_ssm)
 2. AWS EC2 instance with public IP
-   * [Node.js](examples/nodejs_aws_ssh)
-   * [GoLang](examples/go_aws_ssh)
+   * [Go](https://github.com/wttech/pulumi-aem/tree/main/examples/go_aws_ssh)
+   * [NodeJS](https://github.com/wttech/pulumi-aem/tree/main/examples/nodejs_aws_ssh)
+   * [Python](https://github.com/wttech/pulumi-aem/tree/main/examples/python_aws_ssh)
+   * [.NET](https://github.com/wttech/pulumi-aem/tree/main/examples/dotnet_aws_ssh)
 3. Bare metal machine
-   * [Node.js](examples/nodejs_bare_metal)
-   * [GoLang](examples/go_bare_metal)
+   * [Go](https://github.com/wttech/pulumi-aem/tree/main/examples/go_bare_metal)
+   * [NodeJS](https://github.com/wttech/pulumi-aem/tree/main/examples/nodejs_bare_metal)
+   * [Python](https://github.com/wttech/pulumi-aem/tree/main/examples/python_bare_metal)
+   * [.NET](https://github.com/wttech/pulumi-aem/tree/main/examples/dotnet_bare_metal)
 
 - - -
 
 ## Development
 
 This repository is showing how to create and locally test a native Pulumi provider.
 
@@ -55,18 +70,20 @@
 #### Prerequisites
 
 Prerequisites for this repository are already satisfied by the [Pulumi Devcontainer](https://github.com/pulumi/devcontainer) if you are using Github Codespaces, or VSCode.
 
 If you are not using VSCode, you will need to ensure the following tools are installed and present in your `$PATH`:
 
 * [`pulumictl`](https://github.com/pulumi/pulumictl#installation)
-* [Go 1.21](https://golang.org/dl/) or 1.latest
+* [Go](https://golang.org/dl/) or 1.latest
 * [NodeJS](https://nodejs.org/en/) 14.x.  We recommend using [nvm](https://github.com/nvm-sh/nvm) to manage NodeJS installations.
 * [Yarn](https://yarnpkg.com/)
 * [TypeScript](https://www.typescriptlang.org/)
+* [Python](https://www.python.org/downloads/) (called as `python3`).  For recent versions of MacOS, the system-installed version is fine.
+* [.NET](https://dotnet.microsoft.com/download)
 
 
 #### Build & test the AEM provider
 
 1. Create a new Github CodeSpaces environment using this repository.
 1. Open a terminal in the CodeSpaces environment.
 1. Run `make build install` to build and install the provider.
@@ -75,24 +92,24 @@
 1. Run `make down` to tear down the example program.
 
 ##### Build the provider and install the plugin
 
    ```bash
    $ make build install
    ```
-   
+
 This will:
 
 1. Create the SDK codegen binary and place it in a `./bin` folder (gitignored)
 2. Create the provider binary and place it in the `./bin` folder (gitignored)
 3. Generate the dotnet, Go, Node, and Python SDKs and place them in the `./sdk` folder
 4. Install the provider on your machine.
 
 ##### Test against the example
-   
+
 ```bash
 $ cd examples/simple
 $ yarn link @wttech/aem
 $ yarn install
 $ pulumi stack init test
 $ pulumi up
 ```
```

### Comparing `wttech_aem-0.9.0/setup.py` & `wttech_aem-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.9.0"
+VERSION = "0.9.1"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "aem Pulumi Package - Development Version"
```

### Comparing `wttech_aem-0.9.0/wttech_aem/__init__.py` & `wttech_aem-0.9.1/wttech_aem/__init__.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.9.0/wttech_aem/_utilities.py` & `wttech_aem-0.9.1/wttech_aem/_utilities.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.9.0/wttech_aem/compose/_inputs.py` & `wttech_aem-0.9.1/wttech_aem/compose/_inputs.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.9.0/wttech_aem/compose/instance.py` & `wttech_aem-0.9.1/wttech_aem/compose/instance.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.9.0/wttech_aem/compose/outputs.py` & `wttech_aem-0.9.1/wttech_aem/compose/outputs.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.9.0/wttech_aem/provider.py` & `wttech_aem-0.9.1/wttech_aem/provider.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.9.0/wttech_aem.egg-info/PKG-INFO` & `wttech_aem-0.9.1/wttech_aem.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: wttech_aem
-Version: 0.9.0
+Version: 0.9.1
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.56.0
 Requires-Dist: semver>=2.8.1
 
-![AEM Compose Logo](docs/logo-with-text.png)
-[![WTT Logo](docs/wtt-logo.png)](https://www.wundermanthompson.com/service/technology)
+[![AEM Compose Logo](https://github.com/wttech/pulumi-aem/raw/main/docs/logo-with-text.png)](https://github.com/wttech/aemc)
+[![WTT Logo](https://github.com/wttech/pulumi-aem/raw/main/docs/wtt-logo.png)](https://www.wundermanthompson.com/service/technology)
 
-[![Apache License, Version 2.0, January 2004](docs/apache-license-badge.svg)](http://www.apache.org/licenses/)
+[![Apache License, Version 2.0, January 2004](https://github.com/wttech/pulumi-aem/raw/main/docs/apache-license-badge.svg)](http://www.apache.org/licenses/)
 
 # AEM Compose - Pulumi Native Provider
 
 This provider allows development teams to easily set up [Adobe Experience Manager (AEM)](https://business.adobe.com/products/experience-manager/adobe-experience-manager.html) instances on virtual machines in the cloud (AWS, Azure, GCP, etc.) or bare metal machines.
 It's based on the [AEM Compose](https://github.com/wttech/aemc) tool and aims to simplify the process of creating AEM environments without requiring deep DevOps knowledge.
 
 Published in [Pulumi Registry](https://www.pulumi.com/registry/packages/aem/).
@@ -36,22 +36,28 @@
 - Based on the powerful [AEM Compose](https://github.com/wttech/aemc) tool
 
 ## Quickstart
 
 The easiest way to get started is to review, copy and adapt provided examples:
 
 1. AWS EC2 instance with private IP
-   * [Node.js](examples/nodejs_aws_ssm)
-   * [GoLang](examples/go_aws_ssm)
+   * [Go](https://github.com/wttech/pulumi-aem/tree/main/examples/go_aws_ssm)
+   * [NodeJS](https://github.com/wttech/pulumi-aem/tree/main/examples/nodejs_aws_ssm)
+   * [Python](https://github.com/wttech/pulumi-aem/tree/main/examples/python_aws_ssm)
+   * [.NET](https://github.com/wttech/pulumi-aem/tree/main/examples/dotnet_aws_ssm)
 2. AWS EC2 instance with public IP
-   * [Node.js](examples/nodejs_aws_ssh)
-   * [GoLang](examples/go_aws_ssh)
+   * [Go](https://github.com/wttech/pulumi-aem/tree/main/examples/go_aws_ssh)
+   * [NodeJS](https://github.com/wttech/pulumi-aem/tree/main/examples/nodejs_aws_ssh)
+   * [Python](https://github.com/wttech/pulumi-aem/tree/main/examples/python_aws_ssh)
+   * [.NET](https://github.com/wttech/pulumi-aem/tree/main/examples/dotnet_aws_ssh)
 3. Bare metal machine
-   * [Node.js](examples/nodejs_bare_metal)
-   * [GoLang](examples/go_bare_metal)
+   * [Go](https://github.com/wttech/pulumi-aem/tree/main/examples/go_bare_metal)
+   * [NodeJS](https://github.com/wttech/pulumi-aem/tree/main/examples/nodejs_bare_metal)
+   * [Python](https://github.com/wttech/pulumi-aem/tree/main/examples/python_bare_metal)
+   * [.NET](https://github.com/wttech/pulumi-aem/tree/main/examples/dotnet_bare_metal)
 
 - - -
 
 ## Development
 
 This repository is showing how to create and locally test a native Pulumi provider.
 
@@ -64,18 +70,20 @@
 #### Prerequisites
 
 Prerequisites for this repository are already satisfied by the [Pulumi Devcontainer](https://github.com/pulumi/devcontainer) if you are using Github Codespaces, or VSCode.
 
 If you are not using VSCode, you will need to ensure the following tools are installed and present in your `$PATH`:
 
 * [`pulumictl`](https://github.com/pulumi/pulumictl#installation)
-* [Go 1.21](https://golang.org/dl/) or 1.latest
+* [Go](https://golang.org/dl/) or 1.latest
 * [NodeJS](https://nodejs.org/en/) 14.x.  We recommend using [nvm](https://github.com/nvm-sh/nvm) to manage NodeJS installations.
 * [Yarn](https://yarnpkg.com/)
 * [TypeScript](https://www.typescriptlang.org/)
+* [Python](https://www.python.org/downloads/) (called as `python3`).  For recent versions of MacOS, the system-installed version is fine.
+* [.NET](https://dotnet.microsoft.com/download)
 
 
 #### Build & test the AEM provider
 
 1. Create a new Github CodeSpaces environment using this repository.
 1. Open a terminal in the CodeSpaces environment.
 1. Run `make build install` to build and install the provider.
@@ -84,24 +92,24 @@
 1. Run `make down` to tear down the example program.
 
 ##### Build the provider and install the plugin
 
    ```bash
    $ make build install
    ```
-   
+
 This will:
 
 1. Create the SDK codegen binary and place it in a `./bin` folder (gitignored)
 2. Create the provider binary and place it in the `./bin` folder (gitignored)
 3. Generate the dotnet, Go, Node, and Python SDKs and place them in the `./sdk` folder
 4. Install the provider on your machine.
 
 ##### Test against the example
-   
+
 ```bash
 $ cd examples/simple
 $ yarn link @wttech/aem
 $ yarn install
 $ pulumi stack init test
 $ pulumi up
 ```
```

