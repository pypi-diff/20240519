# Comparing `tmp/trsolucoes-6.1.1.tar.gz` & `tmp/trsolucoes-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trsolucoes-6.1.1.tar", last modified: Fri May 17 14:03:58 2024, max compression
+gzip compressed data, was "trsolucoes-7.0.0.tar", last modified: Sun May 19 21:23:34 2024, max compression
```

## Comparing `trsolucoes-6.1.1.tar` & `trsolucoes-7.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:58.641626 trsolucoes-6.1.1/
--rw-rw-rw-   0        0        0     1088 2024-05-17 11:25:36.000000 trsolucoes-6.1.1/LICENCE
--rw-rw-rw-   0        0        0     2550 2024-05-17 14:03:58.639625 trsolucoes-6.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2224 2024-05-17 14:01:24.000000 trsolucoes-6.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:58.625595 trsolucoes-6.1.1/selenium_helper/
--rw-rw-rw-   0        0        0       43 2024-05-17 12:22:33.000000 trsolucoes-6.1.1/selenium_helper/__init__.py
--rw-rw-rw-   0        0        0    12924 2024-05-17 14:02:29.000000 trsolucoes-6.1.1/selenium_helper/selenium_helper.py
--rw-rw-rw-   0        0        0       42 2024-05-17 14:03:58.641626 trsolucoes-6.1.1/setup.cfg
--rw-rw-rw-   0        0        0      543 2024-05-17 14:03:55.000000 trsolucoes-6.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:03:58.638625 trsolucoes-6.1.1/trsolucoes.egg-info/
--rw-rw-rw-   0        0        0     2550 2024-05-17 14:03:58.000000 trsolucoes-6.1.1/trsolucoes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-17 14:03:58.000000 trsolucoes-6.1.1/trsolucoes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 14:03:58.000000 trsolucoes-6.1.1/trsolucoes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-17 14:03:58.000000 trsolucoes-6.1.1/trsolucoes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 21:23:34.612670 trsolucoes-7.0.0/
+-rw-rw-rw-   0        0        0     1088 2024-05-19 21:10:17.000000 trsolucoes-7.0.0/LICENCE
+-rw-rw-rw-   0        0        0     2550 2024-05-19 21:23:34.612670 trsolucoes-7.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2224 2024-05-19 21:10:17.000000 trsolucoes-7.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 21:23:34.609161 trsolucoes-7.0.0/selenium_helper/
+-rw-rw-rw-   0        0        0       43 2024-05-19 21:10:17.000000 trsolucoes-7.0.0/selenium_helper/__init__.py
+-rw-rw-rw-   0        0        0    13501 2024-05-19 21:17:39.000000 trsolucoes-7.0.0/selenium_helper/selenium_helper.py
+-rw-rw-rw-   0        0        0       42 2024-05-19 21:23:34.612670 trsolucoes-7.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      543 2024-05-19 21:19:24.000000 trsolucoes-7.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 21:23:34.611670 trsolucoes-7.0.0/trsolucoes.egg-info/
+-rw-rw-rw-   0        0        0     2550 2024-05-19 21:23:34.000000 trsolucoes-7.0.0/trsolucoes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-19 21:23:34.000000 trsolucoes-7.0.0/trsolucoes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 21:23:34.000000 trsolucoes-7.0.0/trsolucoes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-19 21:23:34.000000 trsolucoes-7.0.0/trsolucoes.egg-info/top_level.txt
```

### Comparing `trsolucoes-6.1.1/LICENCE` & `trsolucoes-7.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `trsolucoes-6.1.1/PKG-INFO` & `trsolucoes-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trsolucoes
-Version: 6.1.1
+Version: 7.0.0
 Summary: Um repositório não oficial de funções de auxilio para Selenium
 Author: Tainan Ramos
 Author-email: tainan@trsolucoes.com.br
 License: MIT License
 Keywords: trsolucoes
 Requires: selenium
 Description-Content-Type: text/markdown
```

### Comparing `trsolucoes-6.1.1/README.md` & `trsolucoes-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `trsolucoes-6.1.1/selenium_helper/selenium_helper.py` & `trsolucoes-7.0.0/selenium_helper/selenium_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,31 @@
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 from time import sleep
 
 
 class SeleniumHelper():
-    def wait_element(self, driver: WebDriver, locator: tuple[By, str], tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, return_element:bool = False, max_result:bool = False) -> bool | WebElement:
+    """
+    Classe SeleniumHelper.
+
+    Esta classe fornece métodos auxiliares para interagir com o navegador
+    utilizando o WebDriver do Selenium. A classe requer uma instância
+    de um driver do Selenium (como o ChromeDriver) para ser inicializada.
+    """
+    def __init__(self, driver: WebDriver) -> None:
+        """
+        Inicializa a classe SeleniumHelper com um WebDriver do Selenium.
+
+        Args:
+            * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
+        """
+        self.driver = driver
+    
+    def wait_element(self, locator: tuple[By, str], tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, return_element:bool = False, max_result:bool = False) -> bool | WebElement:
         """
         Aguarda a presença de um elemento na página, opcionalmente retornando o próprio elemento.
 
         Args:
             * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
             * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
             * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (attribute_name, attribute_value). Default é None.
@@ -26,28 +42,28 @@
         Returns:
             * bool | WebElement: Retorna o elemento WebElement se return_element for True e o elemento for encontrado. Caso contrário, retorna um booleano indicando se o elemento foi encontrado (True) ou não (False).
         """
         sleep(delay_before)
         checked: bool = False
         element: WebElement
         try:
-            element = _find_element(driver, locator, tag_filter, timeout, max_result)
+            element = _find_element(self.driver, locator, tag_filter, timeout, max_result)
             if(element):
                 checked = True
             else:
                 checked = False
         except:
             checked = False
         sleep(delay_after)
         if(return_element):
             return element
         else:
             return checked
 
-    def wait_and_send_keys(self, driver: WebDriver, locator: tuple[By, str], text: str, tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, clear_form: bool = True, click_before: bool = False, max_result:bool = False) -> None:
+    def wait_and_send_keys(self, locator: tuple[By, str], text: str, tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, clear_form: bool = True, click_before: bool = False, max_result:bool = False) -> None:
         """
         Aguarda a presença de um elemento na página e envia um texto para ele, com opções para limpar o campo e clicar no elemento antes de enviar o texto.
 
         Args:
             * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
             * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
             * text (str): Texto a ser enviado para o elemento.
@@ -57,42 +73,42 @@
             * delay_after (float, opcional): Tempo em segundos para esperar após enviar o texto para o elemento. Default é 0.3 segundos.
             * clear_form (bool, opcional): Se True, limpa o campo de texto antes de enviar o novo texto. Default é True.
             * click_before (bool, opcional): Se True, clica no elemento antes de enviar o texto. Default é False.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
-        element = _find_element(driver, locator, tag_filter, timeout, max_result)
+        element = _find_element(self.driver, locator, tag_filter, timeout, max_result)
         if(click_before):
-            self.wait_and_click(driver, locator, tag_filter)
+            self.wait_and_click(self.driver, locator, tag_filter)
         if(clear_form):
             element.clear()
         element.send_keys(text)
         sleep(delay_after)
 
-    def wait_and_click(self, driver: WebDriver, locator: tuple[By, str], tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, max_result: bool = False) -> None:
+    def wait_and_click(self, locator: tuple[By, str], tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, max_result: bool = False) -> None:
         """
         Aguarda a presença de um elemento na página e clica nele.
 
         Args:
             * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
             * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
             * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (attribute_name, attribute_value). Default é None.
             * timeout (int, opcional): Tempo máximo de espera pelo elemento em segundos. Default é 30 segundos.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelo elemento. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após clicar no elemento. Default é 0.3 segundos.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
-        element = _find_element(driver, locator, tag_filter, timeout, max_result)
+        element = _find_element(self.driver, locator, tag_filter, timeout, max_result)
         element.click()
         sleep(delay_after)
 
-    def wait_and_select(self, driver: WebDriver, locator: tuple[By, str], text: str, tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, max_result: bool = False) -> None:
+    def wait_and_select(self, locator: tuple[By, str], text: str, tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, max_result: bool = False) -> None:
         """
         Aguarda a presença de um elemento na página e seleciona uma opção por texto visível em um elemento <select>.
 
         Args:
             * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
             * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
             * text (str): Texto visível da opção a ser selecionada no elemento <select>.
@@ -100,55 +116,56 @@
             * timeout (int, opcional): Tempo máximo de espera pelo elemento em segundos. Default é 30 segundos.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelo elemento. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após selecionar a opção. Default é 0.3 segundos.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
-        element = _find_element(driver, locator, tag_filter, timeout, max_result)
+        element = _find_element(self.driver, locator, tag_filter, timeout, max_result)
         select_object = Select(element)
         select_object.select_by_visible_text(text)
         sleep(delay_after)
 
-    def wait_and_click_in_text(self, driver: WebDriver, locator: tuple[By, str], text: str, delay_before: float = 0.3, delay_after: float = 0.3) -> None:
+    def wait_and_click_in_text(self, locator: tuple[By, str], text: str, delay_before: float = 0.3, delay_after: float = 0.3) -> None:
         """
         Aguarda um breve período e clica em um elemento cujo texto corresponde ao texto fornecido.
 
         Args:
             * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
             * locator (tuple[By, str]): Localizador dos elementos na forma (By, value), onde By é a estratégia de localização e value é o seletor.
             * text (str): Texto a ser correspondido com o texto dos elementos encontrados.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelos elementos. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após clicar no elemento. Default é 0.3 segundos.
         """
         sleep(delay_before)
-        elements: list[WebElement] = driver.find_elements(locator[0], locator[1])
+
+        elements: list[WebElement] = self.driver.find_elements(locator[0], locator[1])
         for element in elements:
             if(text.lower() == element.text.lower()):
                 element.click()
                 break
         sleep(delay_after)
 
-    def wait_and_hover(self, driver: WebDriver, locator: tuple[By, str], tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, max_result: bool = False) -> None:
+    def wait_and_hover(self, locator: tuple[By, str], tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, max_result: bool = False) -> None:
         """
         Aguarda a presença de um elemento na página e passa o cursor do mouse sobre ele.
 
         Args:
             * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
             * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
             * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (attribute_name, attribute_value). Default é None.
             * timeout (int, opcional): Tempo máximo de espera pelo elemento em segundos. Default é 30 segundos.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelo elemento. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após passar o cursor sobre o elemento. Default é 0.3 segundos.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
-        element = _find_element(driver, locator, tag_filter, timeout, max_result)
-        actions = ActionChains(driver)
+        element = _find_element(self.driver, locator, tag_filter, timeout, max_result)
+        actions = ActionChains(self.driver)
         actions.move_to_element(element).perform()
         sleep(delay_after)
 
 def _find_element(driver: WebDriver, locator: tuple[By, str], tag_filter: list[tuple[str, str]], timeout: int, max_result: bool) -> WebElement:
         """
         Encontra um elemento na página e espera até que o elemento seja clicável.
 
@@ -160,15 +177,16 @@
             * max_result (bool): Se True, continua buscando até encontrar o elemento mais relevante baseado no filtro. Se False, retorna o primeiro elemento correspondente.
 
         Returns:
             * WebElement: O elemento WebElement encontrado que atende aos critérios, ou None se nenhum elemento for encontrado ou se ocorrer uma exceção.
         """
         element: WebElement = None
         try:
-            if(locator[0] == By.TAG_NAME):
+            if(tag_filter):
+                WebDriverWait(driver, timeout).until(EC.element_to_be_clickable(locator))
                 elements = driver.find_elements(locator[0], locator[1])
                 for el in elements:
                     for filter in tag_filter:
                         if (el.get_attribute(filter[0]) == filter[1]):
                             element = el    
                         else:
                             element = None
```

### Comparing `trsolucoes-6.1.1/setup.py` & `trsolucoes-7.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="UTF-8") as arq:
     readme = arq.read()
 
 setup(name="trsolucoes",
-      version="6.1.1",
+      version="7.0.0",
       license="MIT License",
       author="Tainan Ramos",
       long_description=readme,
       long_description_content_type="text/markdown",
       author_email="tainan@trsolucoes.com.br",
       keywords="trsolucoes",
       description="Um repositório não oficial de funções de auxilio para Selenium",
```

### Comparing `trsolucoes-6.1.1/trsolucoes.egg-info/PKG-INFO` & `trsolucoes-7.0.0/trsolucoes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trsolucoes
-Version: 6.1.1
+Version: 7.0.0
 Summary: Um repositório não oficial de funções de auxilio para Selenium
 Author: Tainan Ramos
 Author-email: tainan@trsolucoes.com.br
 License: MIT License
 Keywords: trsolucoes
 Requires: selenium
 Description-Content-Type: text/markdown
```

