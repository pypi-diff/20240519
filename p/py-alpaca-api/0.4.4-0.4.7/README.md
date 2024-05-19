# Comparing `tmp/py_alpaca_api-0.4.4.tar.gz` & `tmp/py_alpaca_api-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.4.4.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.4.7.tar", max compression
```

## Comparing `py_alpaca_api-0.4.4.tar` & `py_alpaca_api-0.4.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.4.4/LICENSE
--rw-r--r--   0        0        0    17299 2024-05-15 03:25:08.684820 py_alpaca_api-0.4.4/README.md
--rw-r--r--   0        0        0        0 2024-05-18 07:55:50.214840 py_alpaca_api-0.4.4/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2460 2024-05-18 15:10:11.299597 py_alpaca_api-0.4.4/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-18 07:55:40.234842 py_alpaca_api-0.4.4/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     3025 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     3711 2024-05-18 15:10:11.299597 py_alpaca_api-0.4.4/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    20501 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.4/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     7736 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     2102 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    18665 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0    14954 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0     6403 2024-05-18 15:10:11.299597 py_alpaca_api-0.4.4/py_alpaca_api/src/screener.py
--rw-r--r--   0        0        0    21192 2024-05-18 07:47:00.164957 py_alpaca_api-0.4.4/py_alpaca_api/src/watchlist.py
--rw-r--r--   0        0        0     1279 2024-05-18 15:10:11.299597 py_alpaca_api-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    18060 1970-01-01 00:00:00.000000 py_alpaca_api-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-19 01:27:26.322892 py_alpaca_api-0.4.7/LICENSE
+-rw-r--r--   0        0        0    16791 2024-05-19 11:02:34.884010 py_alpaca_api-0.4.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.4.7/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2513 2024-05-19 04:10:18.598262 py_alpaca_api-0.4.7/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.4.7/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     6009 2024-05-19 04:10:18.608262 py_alpaca_api-0.4.7/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     3750 2024-05-19 04:10:18.608262 py_alpaca_api-0.4.7/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    21161 2024-05-19 04:10:18.608262 py_alpaca_api-0.4.7/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     7736 2024-05-19 02:32:34.142337 py_alpaca_api-0.4.7/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2102 2024-05-19 02:32:34.112337 py_alpaca_api-0.4.7/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    18665 2024-05-19 02:32:34.172337 py_alpaca_api-0.4.7/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0    14954 2024-05-19 02:32:34.172337 py_alpaca_api-0.4.7/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     7359 2024-05-19 12:31:17.233892 py_alpaca_api-0.4.7/py_alpaca_api/src/screener.py
+-rw-r--r--   0        0        0    21397 2024-05-19 04:10:18.608262 py_alpaca_api-0.4.7/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1324 2024-05-19 12:31:17.233892 py_alpaca_api-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.4.7/PKG-INFO
```

### Comparing `py_alpaca_api-0.4.4/LICENSE` & `py_alpaca_api-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.4/README.md` & `py_alpaca_api-0.4.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,163 +1,138 @@
+Metadata-Version: 2.1
+Name: py-alpaca-api
+Version: 0.4.7
+Summary: Python package, for communicating with Alpaca Markets REST API.
+Home-page: https://github.com/TexasCoding/py-alpaca-api
+License: MIT
+Keywords: alpaca,python
+Author: TexasCoding
+Author-email: jeff10278@me.com
+Requires-Python: >=3.12,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: pendulum (>=3.0.0,<4.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Documentation, https://py-alpaca-api.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/TexasCoding/py-alpaca-api
+Description-Content-Type: text/markdown
+
 <p align="center">
   <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" alt="project-logo">
 </p>
 <p align="center">
     <h1 align="center">PY-ALPACA-API</h1>
 </p>
 <p align="center">
-    <em>Empowering traders with precision and control.</em>
+    <em>Empowering Alpaca Trading API with Python</em>
 </p>
 <p align="center">
 <img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/TexasCoding/py-alpaca-api/.github%2Fworkflows%2Ftest-package.yml?logo=github">
 	<img src="https://img.shields.io/github/license/TexasCoding/py-alpaca-api?style=default&logo=opensourceinitiative&logoColor=white&color=0080ff" alt="license">
 	<img src="https://img.shields.io/github/last-commit/TexasCoding/py-alpaca-api?style=default&logo=git&logoColor=white&color=0080ff" alt="last-commit">
 	<img src="https://img.shields.io/github/languages/top/TexasCoding/py-alpaca-api?style=default&color=0080ff" alt="repo-top-language">
 	<img src="https://img.shields.io/github/languages/count/TexasCoding/py-alpaca-api?style=default&color=0080ff" alt="repo-language-count">
 <p>
 <p align="center">
 	<!-- default option, no dependency badges. -->
+   <img alt="Python" src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">
+   <img alt="Poetry" src="https://img.shields.io/badge/Poetry-%233B82F6.svg?style=for-the-badge&logo=poetry&logoColor=0B3D8D">
+
 </p>
 
 <br><!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary><br>
 
-- [Overview](#overview)
-- [Features](#features)
-- [Repository Structure](#repository-structure)
-- [Modules](#modules)
-- [Getting Started](#getting-started)
-  - [Installation](#installation)
-  - [Usage](#usage)
-  - [Tests](#tests)
-- [Project Roadmap](#project-roadmap)
-- [Contributing](#contributing)
-- [License](#license)
-- [Acknowledgments](#acknowledgments)
+- [ Overview](#-overview)
+- [ Features](#-features)
+- [ Repository Structure](#-repository-structure)
+- [ Modules](#-modules)
+- [ Getting Started](#-getting-started)
+  - [ Installation](#-installation)
+  - [ Usage](#-usage)
+  - [ Tests](#-tests)
+- [ Project Roadmap](#-project-roadmap)
+- [ Contributing](#-contributing)
+- [ License](#-license)
+- [ Acknowledgments](#-acknowledgments)
 </details>
 <hr>
 
 ##  Overview
 
-Py-alpaca-api is a robust Python library facilitating seamless interaction with the Alpaca Markets REST API. It empowers developers to manage accounts, assets, market data, orders, and positions efficiently. By leveraging key modules like position, order, and history, users can access historical market data, analyze trends, and make informed trading decisions. With a focus on modularity and ease of use, this open-source project delivers essential functionalities for enhancing trading platforms and enabling strategic decision-making within the financial realm.
+The py-alpaca-api project facilitates seamless interaction with the Alpaca Markets REST API, offering a comprehensive suite of functionalities for trading and investment purposes. Key components include asset retrieval, market analysis, order management, and real-time market monitoring. By providing structured classes and methods, such as watchlist and screener functionalities, the project enhances the efficiency of utilizing Alpacas services. With a focus on modular design and data manipulation capabilities, py-alpaca-api empowers users to access vital trading insights and make informed investment decisions.
 
 ---
 
 ##  Features
 
 |    |   Feature         | Description |
 |----|-------------------|---------------------------------------------------------------|
-| ⚙️  | **Architecture**  | The project follows a modular architecture design, allowing for separate components such as Account, Asset, Market, and Order handling. It initializes with API Key, Secret, and Paper Trading options. |
-| 🔩 | **Code Quality**  | The codebase maintains good code quality with consistent style and formatting. It integrates tools like Black for code formatting and Flake8 for linting. |
-| 📄 | **Documentation** | The project has extensive documentation covering various modules such as Account, Asset, and History. It provides detailed explanations of methods, parameters, and usage instructions. |
-| 🔌 | **Integrations**  | Key integrations include requests for HTTP requests, pandas for data manipulation, and pytest for testing. It also leverages Alpaca Markets REST API for financial data interaction. |
-| 🧩 | **Modularity**    | The codebase is highly modular, with separate modules for different functionalities like Position, Order, and Market data retrieval. This promotes code reusability and maintainability. |
-| 🧪 | **Testing**       | The project utilizes pytest for unit testing and requests-mock for mocking HTTP requests. GitHub Actions automate testing workflows for ensuring code integrity. |
-| ⚡️  | **Performance**   | The codebase efficiently handles data retrieval and processing, ensuring smooth interaction with the Alpaca API endpoints. Performance optimizations are achieved through streamlined historical data retrieval and market status updates. |
-| 🛡️ | **Security**      | Security measures include handling authentication securely through API Key and Secret. The project emphasizes data protection and access control by managing account and asset information securely. |
-| 📦 | **Dependencies**  | Key external libraries and dependencies include requests, pandas, numpy for data manipulation, and pytest for testing. Additional tools like pre-commit and poetry enhance development workflows. |
+| ⚙️  | **Architecture**  | The project follows a structured architecture using classes like PyAlpacaApi, Watchlist, Screener, Position, Order, Market, and others for specific API interactions. This modular design enhances functionality and maintainability. |
+| 🔩 | **Code Quality**  | The codebase maintains good quality with clear variable naming, proper commenting, and adherence to PEP8 style guidelines. The use of tools like Black and pre-commit ensures consistent code formatting. |
+| 📄 | **Documentation** | Extensive documentation is provided through files like requirements.txt, pyproject.toml, and inline comments. Detailed descriptions help users understand functions and classes efficiently. Proper metadata and dependencies are also outlined. |
+| 🔌 | **Integrations**  | Key dependencies include python-dateutil, requests, pandas, pytest, numpy, and others necessary for data manipulation, HTTP requests, and testing. GitHub Actions are used for CI/CD processes. |
+| 🧩 | **Modularity**    | The codebase exhibits high modularity with separate modules for various functionalities like account management, asset handling, market analysis, etc. This modular approach enhances reusability and facilitates easy maintenance and updates. |
+| 🧪 | **Testing**       | Testing frameworks like pytest are used along with tools like requests-mock and pytest-mock for mocking API responses. Test automation is enforced through GitHub Actions for continuous testing. |
+| ⚡️  | **Performance**   | The project shows efficient resource usage and speed when interacting with the Alpaca Markets REST API. Data retrieval and processing are optimized, ensuring smooth functionality even under high load. |
+| 🛡️ | **Security**      | Measures are taken to handle data protection and access control, though specific details are not explicitly mentioned in the codebase. Security best practices must be ensured when handling sensitive trading data. |
+| 📦 | **Dependencies**  | Key external libraries and dependencies include requests, pandas, numpy, and others crucial for data manipulation and API interactions. Poetry is used for dependency management. |
 
 ---
 
 ##  Repository Structure
 
 ```sh
-└── py-alpaca-api/
-    ├── .github
-    │   ├── ISSUE_TEMPLATE
-    │   │   ├── bug_report.md
-    │   │   ├── custom.md
-    │   │   └── feature_request.md
-    │   └── workflows
-    │       └── test-package.yml
-    ├── CODE_OF_CONDUCT.md
-    ├── CONTRIBUTING.md
-    ├── LICENSE
-    ├── README.md
-    ├── SECURITY.md
-    ├── docs
-    │   ├── Makefile
-    │   ├── make.bat
-    │   ├── rtd_requirements.txt
-    │   └── source
-    │       ├── conf.py
-    │       ├── index.md
-    │       └── notebooks
-    ├── poetry.lock
-    ├── py_alpaca_api
-    │   ├── __init__.py
-    │   ├── alpaca.py
-    │   └── src
-    │       ├── __init__.py
-    │       ├── account.py
-    │       ├── asset.py
-    │       ├── data_classes.py
-    │       ├── history.py
-    │       ├── market.py
-    │       ├── order.py
-    │       └── position.py
-    ├── pyproject.toml
-    ├── requirements.txt
-    └── tests
-        ├── __init__.py
-        ├── test_account.py
-        ├── test_alpaca.py
-        ├── test_asset.py
-        ├── test_historical_data.py
-        ├── test_market.py
-        ├── test_orders.py
-        └── test_positions.py
+   py_alpaca_api
+   ├── alpaca.py
+   └── src
+       ├── __init__.py
+       ├── account.py
+       ├── asset.py
+       ├── data_classes.py
+       ├── history.py
+       ├── market.py
+       ├── order.py
+       ├── position.py
+       ├── screener.py
+       └── watchlist.py
 ```
 
 ---
 
 ##  Modules
 
-<details closed><summary>.</summary>
-
-| File                                                                                          | Summary                                                                                                                                                                                                                |
-| ---                                                                                           | ---                                                                                                                                                                                                                    |
-| [requirements.txt](https://github.com/TexasCoding/py-alpaca-api/blob/master/requirements.txt) | Ensures Python dependencies are managed for the repository, restricting versions to specific ranges. Facilitates compatibility and stable functioning by defining required packages for the Alpaca API project.        |
-| [pyproject.toml](https://github.com/TexasCoding/py-alpaca-api/blob/master/pyproject.toml)     | Enables interaction with Alpaca Markets REST API. Manages account, asset, market data, orders, and positions. Supports Python 3.12, pandas, requests, and numpy. Integrates testing, linting, and documentation tools. |
-
-</details>
-
 <details closed><summary>py_alpaca_api</summary>
 
-| File                                                                                          | Summary                                                                                                                                                                                                                                         |
-| ---                                                                                           | ---                                                                                                                                                                                                                                             |
-| [alpaca.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/alpaca.py) | Defines PyAlpacaApi class, initializing with API Key, Secret, and Paper Trading option. Sets URLs based on trading mode and initializes Account, Asset, History, Position, Order, and Market objects for interacting with Alpaca API endpoints. |
+| File                                                                                          | Summary                                                                                                                                                                                                                              |
+| ---                                                                                           | ---                                                                                                                                                                                                                                  |
+| [alpaca.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/alpaca.py) | Defines PyAlpacaApi class initializing with API credentials for Alpaca trading. Sets URL based on trading type. Instantiates account, asset, history, position, order, market, watchlist, and screener objects for API interactions. |
 
 </details>
 
 <details closed><summary>py_alpaca_api.src</summary>
 
-| File                                                                                                          | Summary                                                                                                                                                                                                                                                                                                                                                                                                          |
-| ---                                                                                                           | ---                                                                                                                                                                                                                                                                                                                                                                                                              |
-| [position.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/position.py)         | Retrieves and processes account positions from Alpaca API. Includes functions to get all positions as a DataFrame, retrieve a specific position, close all positions, and close a specific position by symbol or ID.                                                                                                                                                                                             |
-| [order.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/order.py)               | SummaryThis code file, `history.py`, plays a crucial role in the `py-alpaca-api` repository by providing essential functionalities related to historical market data retrieval and analysis within the Alpaca API ecosystem. By leveraging this module, developers can efficiently access and process historical data for strategic decision-making, enhancing the overall capabilities of the trading platform. |
-| [market.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/market.py)             | Retrieves market clock status via HTTP GET request, handling successful and failed responses. Integrated with Alpaca API for real-time market data.                                                                                                                                                                                                                                                              |
-| [history.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/history.py)           | Retrieve historical stock data from Alpaca API based on specified parameters. Validates asset information, handles timeframe conversions, sends API request with required parameters, and converts response to a structured DataFrame. Ensures error handling for data availability, asset validation, and API response.                                                                                         |
-| [data_classes.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/data_classes.py) | This code file, `data_classes.py`, plays a critical role in defining the data structures and classes essential for modeling various financial assets and market data within the `py-alpaca-api` repository. By encapsulating the core data elements and relationships, this module sets the foundation for consistent and organized representation of data throughout the project.                               |
-| [asset.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/asset.py)               | Retrieves asset information from the Alpaca API based on the provided symbol. Parses the response into an AssetClass object containing essential details like ID, exchange, status, and more. Signals errors if retrieval fails.                                                                                                                                                                                 |
-| [account.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/account.py)           | Retrieves account information from Alpaca API, mapping it to an AccountClass object in JSON format. Handles successful and failed responses gracefully within the repositorys modular architecture.                                                                                                                                                                                                              |
-
-</details>
-
-<details closed><summary>.github.workflows</summary>
-
-| File                                                                                                            | Summary                                                                                                                                                                                                                                              |
-| ---                                                                                                             | ---                                                                                                                                                                                                                                                  |
-| [test-package.yml](https://github.com/TexasCoding/py-alpaca-api/blob/master/.github/workflows/test-package.yml) | Tests package dependencies and ensures code integrity through automated workflows. Orchestrates testing for account, asset, historical data, market, orders, and positions modules. Facilitates CI/CD integration for robust repository maintenance. |
+| File                                                                                                          | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| ---                                                                                                           | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| [watchlist.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/watchlist.py)       | This code file within the `py-alpaca-api` repository serves the critical purpose of providing a comprehensive set of classes and functions to interact with the Alpaca API effectively. It encapsulates functionalities related to account management, asset handling, data retrieval, market analysis, order execution, portfolio positions, stock screening, and watchlist management. By offering a structured and modular approach to utilizing Alpacas services, this code file significantly enhances the parent repositorys architecture and functionality.                          |
+| [screener.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/screener.py)         | Defines methods to retrieve top gainers and losers in the stock market by analyzing price, volume, and trade count. Implements a data aggregation function to generate results based on specified criteria.                                                                                                                                                                                                                                                                                                                                                                                 |
+| [position.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/position.py)         | Retrieves, formats, and manages position data from the Alpaca Trade API, enabling actions like fetching all positions, getting specific positions, closing all positions, and closing a specific position. Enhances trading insights with customized data organization and closing capabilities.                                                                                                                                                                                                                                                                                            |
+| [order.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/order.py)               | This code file, `screener.py`, within the `py-alpaca-api` repository, plays a vital role in the parent repositorys architecture. It focuses on providing functionalities related to screening stocks based on defined criteria. By leveraging this code, users can easily filter and identify stocks that match specific attributes, enhancing their investment decision-making process. This feature adds significant value to the overall offering of the `py-alpaca-api` repository, making it a comprehensive tool for individuals seeking to interact with the Alpaca API efficiently. |
+| [market.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/market.py)             | Defines Market class with clock method to retrieve market status from Alpaca API. Handles API requests and responses to provide real-time market clock data for trading. Impactful feature for real-time market monitoring within the PyAlpacaApi repository structure.                                                                                                                                                                                                                                                                                                                     |
+| [history.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/history.py)           | Retrieves historical stock data from Alpaca API based on specified parameters. Validates asset as a stock and fetches data utilizing URL formation and API requests. Transforms JSON response into a structured DataFrame for further analysis within the repositorys architecture.                                                                                                                                                                                                                                                                                                         |
+| [data_classes.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/data_classes.py) | This code file in the py-alpaca-api repository serves as a comprehensive interface for interacting with Alpacas API services. It offers functionalities for managing accounts, assets, market data, order placements, positions, screeners, and watchlists. The code encapsulates critical features enabling seamless integration with Alpacas services for trading and investment purposes within the parent repository's architecture.                                                                                                                                                    |
+| [asset.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/asset.py)               | Retrieves asset information from Alpaca API using provided trade URL and headers. Supports fetching all assets based on status, asset class, and exchange. Implements error handling for unsuccessful requests.                                                                                                                                                                                                                                                                                                                                                                             |
+| [account.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/account.py)           | Retrieves account information from Alpaca API using provided URL and headers. Implements a method to return account details as an object. Handles successful and unsuccessful responses appropriately.                                                                                                                                                                                                                                                                                                                                                                                      |
 
 </details>
 
----
-
 ##  Getting Started
 
 **System Requirements:**
 
 * **Python**: `version x.y.z`
 
 ###  Installation
@@ -181,38 +156,25 @@
 > ```
 
 ###  Usage
 
 <h4>From <code>source</code></h4>
 
 > Run py-alpaca-api using the command below:
-> ```python
-> from py_alpaca_api import PyAlpacaApi
-> api = PyAlpacaApi(api_key='YOUR_KEY', api_secret='YOUR_SECRET', api_paper=True)
-> positions = api.position.get_all()
-> orders = api.order.get_all()
-> # Create new order
-> order = api.order.market(symbol='AAPL', qty=1.034, side='buy')
+> ```console
+> $ python main.py
 > ```
 
 ###  Tests
 
 > Run the test suite using the command below:
 > ```console
 > $ pytest
 > ```
 
----
-
-##  Project Roadmap
-
-- [X] `► Create functionality for all Alpaca API resources`
-
----
-
 ##  Contributing
 
 Contributions are welcome! Here are several ways you can contribute:
 
 - **[Report Issues](https://github.com/TexasCoding/py-alpaca-api/issues)**: Submit bugs found or log feature requests for the `py-alpaca-api` project.
 - **[Submit Pull Requests](https://github.com/TexasCoding/py-alpaca-api/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
 - **[Join the Discussions](https://github.com/TexasCoding/py-alpaca-api/discussions)**: Share your insights, provide feedback, or ask questions.
@@ -263,7 +225,8 @@
 ##  Acknowledgments
 
 - List any resources, contributors, inspiration, etc. here.
 
 [**Return**](#-overview)
 
 ---
+
```

### Comparing `py_alpaca_api-0.4.4/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.4.7/py_alpaca_api/alpaca.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             ValueError if API Secret is not provided
 
         Example:
         --------
         >>> PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
         PyAlpacaApi()
         """  # noqa
+
         # Check if API Key and Secret are provided
         if not api_key:
             raise ValueError("API Key is required")
         if not api_secret:
             raise ValueError("API Secret is required")
         # Set the API Key and Secret
         self.headers = {
@@ -54,12 +55,16 @@
             self.trade_url = "https://api.alpaca.markets/v2"
 
         self.data_url = "https://data.alpaca.markets/v2"
 
         self.account = Account(trade_url=self.trade_url, headers=self.headers)
         self.asset = Asset(trade_url=self.trade_url, headers=self.headers)
         self.history = History(data_url=self.data_url, headers=self.headers, asset=self.asset)
-        self.position = Position(trade_url=self.trade_url, headers=self.headers, account=self.account)
+        self.position = Position(
+            trade_url=self.trade_url,
+            headers=self.headers,
+            account=self.account,
+        )
         self.order = Order(trade_url=self.trade_url, headers=self.headers)
         self.market = Market(trade_url=self.trade_url, headers=self.headers)
         self.watchlist = Watchlist(trade_url=self.trade_url, headers=self.headers)
         self.screener = Screener(data_url=self.data_url, headers=self.headers, asset=self.asset)
```

### Comparing `py_alpaca_api-0.4.4/py_alpaca_api/src/asset.py` & `py_alpaca_api-0.4.7/py_alpaca_api/src/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,20 @@
 
         ValueError: If headers are not provided
         """  # noqa
 
         self.trade_url = trade_url
         self.headers = headers
 
-    def get_all(self, status: str = "active", asset_class: str = "us_equity", exchange: str = "") -> pd.DataFrame:
+    def get_all(
+        self,
+        status: str = "active",
+        asset_class: str = "us_equity",
+        exchange: str = "",
+    ) -> pd.DataFrame:
         # Alpaca API URL for asset information
         url = f"{self.trade_url}/assets"
 
         params = {
             "status": status,
             "asset_class": asset_class,
             "exchange": exchange,
```

### Comparing `py_alpaca_api-0.4.4/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.4.7/py_alpaca_api/src/data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,25 +303,31 @@
 
 
 def watchlist_class_from_dict(data_dict: dict) -> WatchlistClass:
     return WatchlistClass(
         id=str(data_dict["id"] if data_dict["id"] else ""),
         account_id=str(data_dict["account_id"] if data_dict["account_id"] else ""),
         created_at=(
-            datetime.strptime(data_dict["created_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["created_at"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["created_at"]
             else datetime.date(0, 0, 0)
         ),
         updated_at=(
-            datetime.strptime(data_dict["updated_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["updated_at"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["updated_at"]
             else datetime.date(0, 0, 0)
         ),
         name=str(data_dict["name"] if data_dict["name"] else ""),
-        assets=[asset_class_from_dict(sym) for sym in data_dict["assets"] if len(data_dict["assets"]) > 0] if data_dict["assets"] else None,
+        assets=([asset_class_from_dict(sym) for sym in data_dict["assets"] if len(data_dict["assets"]) > 0] if data_dict["assets"] else None),
     )
 
 
 ############################################
 # Data Class Clock Conversion Functions
 ############################################
 def clock_class_from_dict(data_dict: dict) -> ClockClass:
@@ -335,26 +341,35 @@
     Returns:
     --------
     ClockClass
         A ClockClass object.
     """  # noqa
     return ClockClass(
         market_time=(
-            datetime.strptime(data_dict["timestamp"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["timestamp"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["timestamp"]
             else datetime.date(0, 0, 0)
         ),
         is_open=bool(data_dict["is_open"]),
         next_open=(
-            datetime.strptime(data_dict["next_open"].replace("T", " ").replace("-04:00", ""), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["next_open"].replace("T", " ").replace("-04:00", ""),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["next_open"]
             else datetime.date(0, 0, 0)
         ),
         next_close=(
-            datetime.strptime(data_dict["next_close"].replace("-04:00", "").replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["next_close"].replace("-04:00", "").replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["next_close"]
             else datetime.date(0, 0, 0)
         ),
     )
 
 
 ############################################
@@ -433,15 +448,18 @@
         pending_transfer_in=float(data_dict["pending_transfer_in"] if data_dict["pending_transfer_in"] else 0),
         portfolio_value=float(data_dict["portfolio_value"] if data_dict["portfolio_value"] else 0),
         pattern_day_trader=bool(data_dict["pattern_day_trader"]),
         trading_blocked=bool(data_dict["trading_blocked"]),
         transfers_blocked=bool(data_dict["transfers_blocked"]),
         account_blocked=bool(data_dict["account_blocked"]),
         created_at=(
-            datetime.strptime(data_dict["created_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["created_at"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["created_at"]
             else datetime.date(0, 0, 0)
         ),
         trade_suspended_by_user=bool(data_dict["trade_suspended_by_user"]),
         multiplier=int(data_dict["multiplier"] if data_dict["multiplier"] else 0),
         shorting_enabled=bool(data_dict["shorting_enabled"]),
         equity=float(data_dict["equity"] if data_dict["equity"] else 0),
@@ -509,50 +527,74 @@
     OrderClass
         An OrderClass object.
     """  # noqa
     return OrderClass(
         id=str(data_dict["id"] if data_dict["id"] else ""),
         client_order_id=str(data_dict["client_order_id"]),
         created_at=(
-            datetime.strptime(data_dict["created_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["created_at"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["created_at"]
             else datetime(1, 1, 1, 0, 0)
         ),
         updated_at=(
-            datetime.strptime(data_dict["updated_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["updated_at"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["updated_at"]
             else datetime(1, 1, 1, 0, 0)
         ),
         submitted_at=(
-            datetime.strptime(data_dict["submitted_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["submitted_at"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["submitted_at"]
             else datetime(1, 1, 1, 0, 0)
         ),
         filled_at=(
-            datetime.strptime(data_dict["filled_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["filled_at"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["filled_at"]
             else datetime(1, 1, 1, 0, 0)
         ),
         expired_at=(
-            datetime.strptime(data_dict["expired_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["expired_at"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["expired_at"]
             else datetime(1, 1, 1, 0, 0)
         ),
         canceled_at=(
-            datetime.strptime(data_dict["canceled_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["canceled_at"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["canceled_at"]
             else datetime(1, 1, 1, 0, 0)
         ),
         failed_at=(
-            datetime.strptime(data_dict["failed_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["failed_at"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["failed_at"]
             else datetime(1, 1, 1, 0, 0)
         ),
         replaced_at=(
-            datetime.strptime(data_dict["replaced_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            datetime.strptime(
+                data_dict["replaced_at"].split(".")[0].replace("T", " "),
+                "%Y-%m-%d %H:%M:%S",
+            )
             if data_dict["replaced_at"]
             else datetime(1, 1, 1, 0, 0)
         ),
         replaced_by=str(data_dict["replaced_by"] if data_dict["replaced_by"] else ""),
         replaces=str(data_dict["replaces"] if data_dict["replaces"] else ""),
         asset_id=str(data_dict["asset_id"] if data_dict["asset_id"] else ""),
         symbol=str(data_dict["symbol"] if data_dict["symbol"] else ""),
```

### Comparing `py_alpaca_api-0.4.4/py_alpaca_api/src/history.py` & `py_alpaca_api-0.4.7/py_alpaca_api/src/history.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.4/py_alpaca_api/src/market.py` & `py_alpaca_api-0.4.7/py_alpaca_api/src/market.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.4/py_alpaca_api/src/order.py` & `py_alpaca_api-0.4.7/py_alpaca_api/src/order.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.4/py_alpaca_api/src/position.py` & `py_alpaca_api-0.4.7/py_alpaca_api/src/position.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.4.4/py_alpaca_api/src/screener.py` & `py_alpaca_api-0.4.7/py_alpaca_api/src/screener.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import json
-from datetime import datetime, timedelta
 
 import pandas as pd
+import pendulum
 import requests
-from pytz import timezone
 
 from .asset import Asset
 
-tz = timezone("US/Eastern")
-ctime = datetime.now(tz)
-close = (ctime - timedelta(days=1)).strftime("%Y-%m-%d")
-prev_close = (ctime - timedelta(days=2)).strftime("%Y-%m-%d")
+# This keeps the date in sync with the market
+# If it's a weekend, it will return the previous Friday
+# If it's a weekday, it will return the previous day, other than Monday
+# If it's Monday, it will return the previous Friday
+today = pendulum.now(tz="America/New_York")
+yesterday = today.subtract(days=1).strftime("%Y-%m-%d")
+if today.day_of_week == (pendulum.SUNDAY or pendulum.MONDAY):
+    yesterday = today.previous(pendulum.FRIDAY).strftime("%Y-%m-%d")
+######################################################################
 
 
 class Screener:
     def __init__(self, data_url: str, headers: object, asset: Asset) -> None:
         """Initialize Screener class3
 
         Parameters:
@@ -123,21 +127,41 @@
 
         gainers_df = gainers_df[gainers_df["price"] > price_greater_than]
         gainers_df = gainers_df[gainers_df["change"] > change_greater_than]
         gainers_df = gainers_df[gainers_df["volume"] > volume_greater_than]
         gainers_df = gainers_df[gainers_df["trades"] > trade_count_greater_than]
         return gainers_df.sort_values(by="change", ascending=False).reset_index(drop=True).head(total_gainers_returned)
 
-    def _get_percentages(self, timeframe: str = "1Day", start: str = prev_close, end: str = close) -> pd.DataFrame:
-        """Get top gainers for the day
+    def _get_percentages(
+        self,
+        timeframe: str = "1Day",
+        start: str = yesterday,
+        end: str = yesterday,
+    ) -> pd.DataFrame:
+        """Get percentage changes for the previous day
+
+        Parameters:
+        ___________
+        timeframe: str
+                Timeframe optional, default is 1Day
+
+        start: str
+                Start date optional, default is yesterday
+
+        end: str
+                End date optional, default is yesterday
 
         Returns:
         _______
-        pd.DataFrame: Top gainers for the day
-        """
+        pd.DataFrame: Percentage changes for the previous day
+
+        Raises:
+        _______
+        ValueError: If failed to get top gainers
+        """  # noqa
         url = f"{self.data_url}/stocks/bars"
 
         params = {
             "symbols": ",".join(self.asset.get_all()["symbol"].tolist()),
             "limit": 10000,
             "timeframe": timeframe,
             "start": start,
@@ -156,38 +180,50 @@
             bars_df = pd.DataFrame.from_dict(res["bars"], orient="index")
             page_token = res["next_page_token"]
 
             while page_token:
                 params["page_token"] = page_token
                 response = requests.get(url, headers=self.headers, params=params)
                 res = json.loads(response.text)
-                bars_df = pd.concat([bars_df, pd.DataFrame.from_dict(res["bars"], orient="index")])
+                bars_df = pd.concat(
+                    [
+                        bars_df,
+                        pd.DataFrame.from_dict(res["bars"], orient="index"),
+                    ]
+                )
                 page_token = res["next_page_token"]
 
             bars_df.reset_index()
 
             gainer_df = pd.DataFrame()
 
             for bar in bars_df.iterrows():
                 # bar[0] is symbol
                 # bar[1][1] is current bar
                 # bar[1][0] is previous bar
                 # bar[1][1]["c"] is current close
                 # bar[1][0]["c"] is previous close
                 # ((current close - previous close) / previous close) * 100
+                # print(bar[1][0])
                 try:
-                    change = round(((bar[1][1]["c"] - bar[1][0]["c"]) / bar[1][0]["c"]) * 100, 2)
+                    change = round(
+                        ((bar[1][0]["c"] - bar[1][0]["o"]) / bar[1][0]["o"]) * 100,
+                        2,
+                    )
+
                     symbol = bar[0]
+
                     sym_data = {
                         "symbol": symbol,
                         "change": change,
-                        "price": bar[1][1]["c"],
-                        "volume": bar[1][1]["v"],
-                        "trades": bar[1][1]["n"],
+                        "price": bar[1][0]["c"],
+                        "volume": bar[1][0]["v"],
+                        "trades": bar[1][0]["n"],
                     }
                     gainer_df = pd.concat([gainer_df, pd.DataFrame([sym_data])])
+
                 except Exception:
                     pass
             gainer_df.reset_index(drop=True, inplace=True)
             return gainer_df
         else:
             raise ValueError(f"Failed to get top gainers. Response: {response.text}")
```

### Comparing `py_alpaca_api-0.4.4/py_alpaca_api/src/watchlist.py` & `py_alpaca_api-0.4.7/py_alpaca_api/src/watchlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,21 @@
         # Otherwise raise an exception
         else:
             raise Exception(response.text)
 
     ########################################################
     # ///////////// Update a watchlist ////////////////////#
     ########################################################
-    def update(self, watchlist_id: str = None, watchlist_name: str = None, name: str = "", symbols: str = "") -> WatchlistClass:
+    def update(
+        self,
+        watchlist_id: str = None,
+        watchlist_name: str = None,
+        name: str = "",
+        symbols: str = "",
+    ) -> WatchlistClass:
         """Update a watchlist
 
         Parameters:
         -----------
         watchlist_id: str
             Watchlist ID (default: None) optional
 
@@ -286,15 +292,20 @@
             symbols = symbols.replace(" ", "").split(",")
         else:
             symbols = ",".join([o.symbol for o in watchlist.assets])
 
         # Create the payload
         payload = {"name": name, "symbols": symbols}
         # Send the request, if 200 return the WatchlistClass object
-        response = requests.put(url, headers=self.headers, json=payload, params={"name": watchlist_name} if watchlist_name else None)
+        response = requests.put(
+            url,
+            headers=self.headers,
+            json=payload,
+            params={"name": watchlist_name} if watchlist_name else None,
+        )
 
         res = json.loads(response.text)
 
         if response.status_code == 200:
             return watchlist_class_from_dict(res)
         else:
             raise Exception(response.text)
@@ -343,15 +354,20 @@
             return f"Watchlist {watchlist_id if watchlist_id else watchlist_name} deleted successfully."
         else:
             raise Exception(response.text)
 
     ########################################################
     # ///////////// Add Asset to  watchlist ///////////////#
     ########################################################
-    def add_asset(self, watchlist_id: str = None, watchlist_name: str = None, symbol: str = "") -> WatchlistClass:
+    def add_asset(
+        self,
+        watchlist_id: str = None,
+        watchlist_name: str = None,
+        symbol: str = "",
+    ) -> WatchlistClass:
         """Add a Asset to a watchlist
 
         Parameters:
         -----------
         watchlist_id: str
             Watchlist ID (default: None) optional
 
@@ -430,15 +446,20 @@
             return watchlist_class_from_dict(res)
         else:
             raise Exception(response.text)
 
     ########################################################
     # /////////// Remove a Asset from  watchlist //////////#
     ########################################################
-    def remove_asset(self, watchlist_id: str = None, watchlist_name: str = None, symbol: str = "") -> WatchlistClass:
+    def remove_asset(
+        self,
+        watchlist_id: str = None,
+        watchlist_name: str = None,
+        symbol: str = "",
+    ) -> WatchlistClass:
         """Remove a Asset from a watchlist
 
         Parameters:
         -----------
         watchlist_id: str
             Watchlist ID (default: None) optional
```

### Comparing `py_alpaca_api-0.4.4/pyproject.toml` & `py_alpaca_api-0.4.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.4.4"
+version = "0.4.7"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
 keywords = ["alpaca", "python"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pandas = "^2.2.2"
 requests = "^2.31.0"
 numpy = "^1.26.4"
+pendulum = "^3.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 requests-mock = "^1.12.1"
 black = "^24.4.2"
 isort = "^5.13.2"
 pre-commit = "^3.7.1"
 ipykernel = "^6.29.4"
 pytest-mock = "^3.14.0"
 pytest-mock-server = "^0.3.0"
+python-dotenv = "^1.0.1"
 
 
 [tool.poetry.group.test.dependencies]
 flake8 = "^7.0.0"
 
 
 [tool.poetry.group.doc.dependencies]
```

### Comparing `py_alpaca_api-0.4.4/PKG-INFO` & `py_alpaca_api-0.4.7/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,183 +1,117 @@
-Metadata-Version: 2.1
-Name: py-alpaca-api
-Version: 0.4.4
-Summary: Python package, for communicating with Alpaca Markets REST API.
-Home-page: https://github.com/TexasCoding/py-alpaca-api
-License: MIT
-Keywords: alpaca,python
-Author: TexasCoding
-Author-email: jeff10278@me.com
-Requires-Python: >=3.12,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Project-URL: Documentation, https://py-alpaca-api.readthedocs.io/en/latest/
-Project-URL: Repository, https://github.com/TexasCoding/py-alpaca-api
-Description-Content-Type: text/markdown
-
 <p align="center">
   <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" alt="project-logo">
 </p>
 <p align="center">
     <h1 align="center">PY-ALPACA-API</h1>
 </p>
 <p align="center">
-    <em>Empowering traders with precision and control.</em>
+    <em>Empowering Alpaca Trading API with Python</em>
 </p>
 <p align="center">
 <img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/TexasCoding/py-alpaca-api/.github%2Fworkflows%2Ftest-package.yml?logo=github">
 	<img src="https://img.shields.io/github/license/TexasCoding/py-alpaca-api?style=default&logo=opensourceinitiative&logoColor=white&color=0080ff" alt="license">
 	<img src="https://img.shields.io/github/last-commit/TexasCoding/py-alpaca-api?style=default&logo=git&logoColor=white&color=0080ff" alt="last-commit">
 	<img src="https://img.shields.io/github/languages/top/TexasCoding/py-alpaca-api?style=default&color=0080ff" alt="repo-top-language">
 	<img src="https://img.shields.io/github/languages/count/TexasCoding/py-alpaca-api?style=default&color=0080ff" alt="repo-language-count">
 <p>
 <p align="center">
 	<!-- default option, no dependency badges. -->
+   <img alt="Python" src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">
+   <img alt="Poetry" src="https://img.shields.io/badge/Poetry-%233B82F6.svg?style=for-the-badge&logo=poetry&logoColor=0B3D8D">
+
 </p>
 
 <br><!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary><br>
 
-- [Overview](#overview)
-- [Features](#features)
-- [Repository Structure](#repository-structure)
-- [Modules](#modules)
-- [Getting Started](#getting-started)
-  - [Installation](#installation)
-  - [Usage](#usage)
-  - [Tests](#tests)
-- [Project Roadmap](#project-roadmap)
-- [Contributing](#contributing)
-- [License](#license)
-- [Acknowledgments](#acknowledgments)
+- [ Overview](#-overview)
+- [ Features](#-features)
+- [ Repository Structure](#-repository-structure)
+- [ Modules](#-modules)
+- [ Getting Started](#-getting-started)
+  - [ Installation](#-installation)
+  - [ Usage](#-usage)
+  - [ Tests](#-tests)
+- [ Project Roadmap](#-project-roadmap)
+- [ Contributing](#-contributing)
+- [ License](#-license)
+- [ Acknowledgments](#-acknowledgments)
 </details>
 <hr>
 
 ##  Overview
 
-Py-alpaca-api is a robust Python library facilitating seamless interaction with the Alpaca Markets REST API. It empowers developers to manage accounts, assets, market data, orders, and positions efficiently. By leveraging key modules like position, order, and history, users can access historical market data, analyze trends, and make informed trading decisions. With a focus on modularity and ease of use, this open-source project delivers essential functionalities for enhancing trading platforms and enabling strategic decision-making within the financial realm.
+The py-alpaca-api project facilitates seamless interaction with the Alpaca Markets REST API, offering a comprehensive suite of functionalities for trading and investment purposes. Key components include asset retrieval, market analysis, order management, and real-time market monitoring. By providing structured classes and methods, such as watchlist and screener functionalities, the project enhances the efficiency of utilizing Alpacas services. With a focus on modular design and data manipulation capabilities, py-alpaca-api empowers users to access vital trading insights and make informed investment decisions.
 
 ---
 
 ##  Features
 
 |    |   Feature         | Description |
 |----|-------------------|---------------------------------------------------------------|
-| ⚙️  | **Architecture**  | The project follows a modular architecture design, allowing for separate components such as Account, Asset, Market, and Order handling. It initializes with API Key, Secret, and Paper Trading options. |
-| 🔩 | **Code Quality**  | The codebase maintains good code quality with consistent style and formatting. It integrates tools like Black for code formatting and Flake8 for linting. |
-| 📄 | **Documentation** | The project has extensive documentation covering various modules such as Account, Asset, and History. It provides detailed explanations of methods, parameters, and usage instructions. |
-| 🔌 | **Integrations**  | Key integrations include requests for HTTP requests, pandas for data manipulation, and pytest for testing. It also leverages Alpaca Markets REST API for financial data interaction. |
-| 🧩 | **Modularity**    | The codebase is highly modular, with separate modules for different functionalities like Position, Order, and Market data retrieval. This promotes code reusability and maintainability. |
-| 🧪 | **Testing**       | The project utilizes pytest for unit testing and requests-mock for mocking HTTP requests. GitHub Actions automate testing workflows for ensuring code integrity. |
-| ⚡️  | **Performance**   | The codebase efficiently handles data retrieval and processing, ensuring smooth interaction with the Alpaca API endpoints. Performance optimizations are achieved through streamlined historical data retrieval and market status updates. |
-| 🛡️ | **Security**      | Security measures include handling authentication securely through API Key and Secret. The project emphasizes data protection and access control by managing account and asset information securely. |
-| 📦 | **Dependencies**  | Key external libraries and dependencies include requests, pandas, numpy for data manipulation, and pytest for testing. Additional tools like pre-commit and poetry enhance development workflows. |
+| ⚙️  | **Architecture**  | The project follows a structured architecture using classes like PyAlpacaApi, Watchlist, Screener, Position, Order, Market, and others for specific API interactions. This modular design enhances functionality and maintainability. |
+| 🔩 | **Code Quality**  | The codebase maintains good quality with clear variable naming, proper commenting, and adherence to PEP8 style guidelines. The use of tools like Black and pre-commit ensures consistent code formatting. |
+| 📄 | **Documentation** | Extensive documentation is provided through files like requirements.txt, pyproject.toml, and inline comments. Detailed descriptions help users understand functions and classes efficiently. Proper metadata and dependencies are also outlined. |
+| 🔌 | **Integrations**  | Key dependencies include python-dateutil, requests, pandas, pytest, numpy, and others necessary for data manipulation, HTTP requests, and testing. GitHub Actions are used for CI/CD processes. |
+| 🧩 | **Modularity**    | The codebase exhibits high modularity with separate modules for various functionalities like account management, asset handling, market analysis, etc. This modular approach enhances reusability and facilitates easy maintenance and updates. |
+| 🧪 | **Testing**       | Testing frameworks like pytest are used along with tools like requests-mock and pytest-mock for mocking API responses. Test automation is enforced through GitHub Actions for continuous testing. |
+| ⚡️  | **Performance**   | The project shows efficient resource usage and speed when interacting with the Alpaca Markets REST API. Data retrieval and processing are optimized, ensuring smooth functionality even under high load. |
+| 🛡️ | **Security**      | Measures are taken to handle data protection and access control, though specific details are not explicitly mentioned in the codebase. Security best practices must be ensured when handling sensitive trading data. |
+| 📦 | **Dependencies**  | Key external libraries and dependencies include requests, pandas, numpy, and others crucial for data manipulation and API interactions. Poetry is used for dependency management. |
 
 ---
 
 ##  Repository Structure
 
 ```sh
-└── py-alpaca-api/
-    ├── .github
-    │   ├── ISSUE_TEMPLATE
-    │   │   ├── bug_report.md
-    │   │   ├── custom.md
-    │   │   └── feature_request.md
-    │   └── workflows
-    │       └── test-package.yml
-    ├── CODE_OF_CONDUCT.md
-    ├── CONTRIBUTING.md
-    ├── LICENSE
-    ├── README.md
-    ├── SECURITY.md
-    ├── docs
-    │   ├── Makefile
-    │   ├── make.bat
-    │   ├── rtd_requirements.txt
-    │   └── source
-    │       ├── conf.py
-    │       ├── index.md
-    │       └── notebooks
-    ├── poetry.lock
-    ├── py_alpaca_api
-    │   ├── __init__.py
-    │   ├── alpaca.py
-    │   └── src
-    │       ├── __init__.py
-    │       ├── account.py
-    │       ├── asset.py
-    │       ├── data_classes.py
-    │       ├── history.py
-    │       ├── market.py
-    │       ├── order.py
-    │       └── position.py
-    ├── pyproject.toml
-    ├── requirements.txt
-    └── tests
-        ├── __init__.py
-        ├── test_account.py
-        ├── test_alpaca.py
-        ├── test_asset.py
-        ├── test_historical_data.py
-        ├── test_market.py
-        ├── test_orders.py
-        └── test_positions.py
+   py_alpaca_api
+   ├── alpaca.py
+   └── src
+       ├── __init__.py
+       ├── account.py
+       ├── asset.py
+       ├── data_classes.py
+       ├── history.py
+       ├── market.py
+       ├── order.py
+       ├── position.py
+       ├── screener.py
+       └── watchlist.py
 ```
 
 ---
 
 ##  Modules
 
-<details closed><summary>.</summary>
-
-| File                                                                                          | Summary                                                                                                                                                                                                                |
-| ---                                                                                           | ---                                                                                                                                                                                                                    |
-| [requirements.txt](https://github.com/TexasCoding/py-alpaca-api/blob/master/requirements.txt) | Ensures Python dependencies are managed for the repository, restricting versions to specific ranges. Facilitates compatibility and stable functioning by defining required packages for the Alpaca API project.        |
-| [pyproject.toml](https://github.com/TexasCoding/py-alpaca-api/blob/master/pyproject.toml)     | Enables interaction with Alpaca Markets REST API. Manages account, asset, market data, orders, and positions. Supports Python 3.12, pandas, requests, and numpy. Integrates testing, linting, and documentation tools. |
-
-</details>
-
 <details closed><summary>py_alpaca_api</summary>
 
-| File                                                                                          | Summary                                                                                                                                                                                                                                         |
-| ---                                                                                           | ---                                                                                                                                                                                                                                             |
-| [alpaca.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/alpaca.py) | Defines PyAlpacaApi class, initializing with API Key, Secret, and Paper Trading option. Sets URLs based on trading mode and initializes Account, Asset, History, Position, Order, and Market objects for interacting with Alpaca API endpoints. |
+| File                                                                                          | Summary                                                                                                                                                                                                                              |
+| ---                                                                                           | ---                                                                                                                                                                                                                                  |
+| [alpaca.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/alpaca.py) | Defines PyAlpacaApi class initializing with API credentials for Alpaca trading. Sets URL based on trading type. Instantiates account, asset, history, position, order, market, watchlist, and screener objects for API interactions. |
 
 </details>
 
 <details closed><summary>py_alpaca_api.src</summary>
 
-| File                                                                                                          | Summary                                                                                                                                                                                                                                                                                                                                                                                                          |
-| ---                                                                                                           | ---                                                                                                                                                                                                                                                                                                                                                                                                              |
-| [position.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/position.py)         | Retrieves and processes account positions from Alpaca API. Includes functions to get all positions as a DataFrame, retrieve a specific position, close all positions, and close a specific position by symbol or ID.                                                                                                                                                                                             |
-| [order.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/order.py)               | SummaryThis code file, `history.py`, plays a crucial role in the `py-alpaca-api` repository by providing essential functionalities related to historical market data retrieval and analysis within the Alpaca API ecosystem. By leveraging this module, developers can efficiently access and process historical data for strategic decision-making, enhancing the overall capabilities of the trading platform. |
-| [market.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/market.py)             | Retrieves market clock status via HTTP GET request, handling successful and failed responses. Integrated with Alpaca API for real-time market data.                                                                                                                                                                                                                                                              |
-| [history.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/history.py)           | Retrieve historical stock data from Alpaca API based on specified parameters. Validates asset information, handles timeframe conversions, sends API request with required parameters, and converts response to a structured DataFrame. Ensures error handling for data availability, asset validation, and API response.                                                                                         |
-| [data_classes.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/data_classes.py) | This code file, `data_classes.py`, plays a critical role in defining the data structures and classes essential for modeling various financial assets and market data within the `py-alpaca-api` repository. By encapsulating the core data elements and relationships, this module sets the foundation for consistent and organized representation of data throughout the project.                               |
-| [asset.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/asset.py)               | Retrieves asset information from the Alpaca API based on the provided symbol. Parses the response into an AssetClass object containing essential details like ID, exchange, status, and more. Signals errors if retrieval fails.                                                                                                                                                                                 |
-| [account.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/account.py)           | Retrieves account information from Alpaca API, mapping it to an AccountClass object in JSON format. Handles successful and failed responses gracefully within the repositorys modular architecture.                                                                                                                                                                                                              |
-
-</details>
-
-<details closed><summary>.github.workflows</summary>
-
-| File                                                                                                            | Summary                                                                                                                                                                                                                                              |
-| ---                                                                                                             | ---                                                                                                                                                                                                                                                  |
-| [test-package.yml](https://github.com/TexasCoding/py-alpaca-api/blob/master/.github/workflows/test-package.yml) | Tests package dependencies and ensures code integrity through automated workflows. Orchestrates testing for account, asset, historical data, market, orders, and positions modules. Facilitates CI/CD integration for robust repository maintenance. |
+| File                                                                                                          | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| ---                                                                                                           | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| [watchlist.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/watchlist.py)       | This code file within the `py-alpaca-api` repository serves the critical purpose of providing a comprehensive set of classes and functions to interact with the Alpaca API effectively. It encapsulates functionalities related to account management, asset handling, data retrieval, market analysis, order execution, portfolio positions, stock screening, and watchlist management. By offering a structured and modular approach to utilizing Alpacas services, this code file significantly enhances the parent repositorys architecture and functionality.                          |
+| [screener.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/screener.py)         | Defines methods to retrieve top gainers and losers in the stock market by analyzing price, volume, and trade count. Implements a data aggregation function to generate results based on specified criteria.                                                                                                                                                                                                                                                                                                                                                                                 |
+| [position.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/position.py)         | Retrieves, formats, and manages position data from the Alpaca Trade API, enabling actions like fetching all positions, getting specific positions, closing all positions, and closing a specific position. Enhances trading insights with customized data organization and closing capabilities.                                                                                                                                                                                                                                                                                            |
+| [order.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/order.py)               | This code file, `screener.py`, within the `py-alpaca-api` repository, plays a vital role in the parent repositorys architecture. It focuses on providing functionalities related to screening stocks based on defined criteria. By leveraging this code, users can easily filter and identify stocks that match specific attributes, enhancing their investment decision-making process. This feature adds significant value to the overall offering of the `py-alpaca-api` repository, making it a comprehensive tool for individuals seeking to interact with the Alpaca API efficiently. |
+| [market.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/market.py)             | Defines Market class with clock method to retrieve market status from Alpaca API. Handles API requests and responses to provide real-time market clock data for trading. Impactful feature for real-time market monitoring within the PyAlpacaApi repository structure.                                                                                                                                                                                                                                                                                                                     |
+| [history.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/history.py)           | Retrieves historical stock data from Alpaca API based on specified parameters. Validates asset as a stock and fetches data utilizing URL formation and API requests. Transforms JSON response into a structured DataFrame for further analysis within the repositorys architecture.                                                                                                                                                                                                                                                                                                         |
+| [data_classes.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/data_classes.py) | This code file in the py-alpaca-api repository serves as a comprehensive interface for interacting with Alpacas API services. It offers functionalities for managing accounts, assets, market data, order placements, positions, screeners, and watchlists. The code encapsulates critical features enabling seamless integration with Alpacas services for trading and investment purposes within the parent repository's architecture.                                                                                                                                                    |
+| [asset.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/asset.py)               | Retrieves asset information from Alpaca API using provided trade URL and headers. Supports fetching all assets based on status, asset class, and exchange. Implements error handling for unsuccessful requests.                                                                                                                                                                                                                                                                                                                                                                             |
+| [account.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/account.py)           | Retrieves account information from Alpaca API using provided URL and headers. Implements a method to return account details as an object. Handles successful and unsuccessful responses appropriately.                                                                                                                                                                                                                                                                                                                                                                                      |
 
 </details>
 
----
-
 ##  Getting Started
 
 **System Requirements:**
 
 * **Python**: `version x.y.z`
 
 ###  Installation
@@ -201,38 +135,25 @@
 > ```
 
 ###  Usage
 
 <h4>From <code>source</code></h4>
 
 > Run py-alpaca-api using the command below:
-> ```python
-> from py_alpaca_api import PyAlpacaApi
-> api = PyAlpacaApi(api_key='YOUR_KEY', api_secret='YOUR_SECRET', api_paper=True)
-> positions = api.position.get_all()
-> orders = api.order.get_all()
-> # Create new order
-> order = api.order.market(symbol='AAPL', qty=1.034, side='buy')
+> ```console
+> $ python main.py
 > ```
 
 ###  Tests
 
 > Run the test suite using the command below:
 > ```console
 > $ pytest
 > ```
 
----
-
-##  Project Roadmap
-
-- [X] `► Create functionality for all Alpaca API resources`
-
----
-
 ##  Contributing
 
 Contributions are welcome! Here are several ways you can contribute:
 
 - **[Report Issues](https://github.com/TexasCoding/py-alpaca-api/issues)**: Submit bugs found or log feature requests for the `py-alpaca-api` project.
 - **[Submit Pull Requests](https://github.com/TexasCoding/py-alpaca-api/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
 - **[Join the Discussions](https://github.com/TexasCoding/py-alpaca-api/discussions)**: Share your insights, provide feedback, or ask questions.
@@ -283,8 +204,7 @@
 ##  Acknowledgments
 
 - List any resources, contributors, inspiration, etc. here.
 
 [**Return**](#-overview)
 
 ---
-
```

