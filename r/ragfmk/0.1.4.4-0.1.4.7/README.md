# Comparing `tmp/ragfmk-0.1.4.4-py3-none-any.whl.zip` & `tmp/ragfmk-0.1.4.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,41 +1,42 @@
-Zip file size: 32956 bytes, number of entries: 39
+Zip file size: 33559 bytes, number of entries: 40
 -rw-rw-rw-  2.0 fat     3657 b- defN 24-May-05 14:22 RagAdhocQueryDoc.py
 -rw-rw-rw-  2.0 fat     1731 b- defN 24-May-06 08:12 RagPrompt.py
 -rw-rw-rw-  2.0 fat     2239 b- defN 24-May-05 15:56 RagTest.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Dec-21 09:21 __init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Dec-21 09:21 ragfmk/__init__.py
--rw-rw-rw-  2.0 fat     9012 b- defN 24-May-06 08:12 ragfmk/rag.py
+-rw-rw-rw-  2.0 fat     9184 b- defN 24-May-08 08:07 ragfmk/rag.py
 -rw-rw-rw-  2.0 fat     2641 b- defN 24-May-06 08:12 ragfmk/ragChromaDB.py
 -rw-rw-rw-  2.0 fat     3716 b- defN 24-May-06 08:12 ragfmk/ragFAISS.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-25 16:16 ragfmk/elements/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Dec-21 09:21 ragfmk/elements/embeddings/__init__.py
--rw-rw-rw-  2.0 fat     3965 b- defN 24-May-06 08:12 ragfmk/elements/embeddings/embeddings.py
--rw-rw-rw-  2.0 fat     2236 b- defN 24-May-06 08:12 ragfmk/elements/embeddings/ollamaEmbeddings.py
--rw-rw-rw-  2.0 fat     1478 b- defN 24-May-06 08:12 ragfmk/elements/embeddings/stEmbeddings.py
+-rw-rw-rw-  2.0 fat     1586 b- defN 24-May-08 13:35 ragfmk/elements/embeddings/embedding.py
+-rw-rw-rw-  2.0 fat     3333 b- defN 24-May-08 16:07 ragfmk/elements/embeddings/embeddings.py
+-rw-rw-rw-  2.0 fat     2528 b- defN 24-May-08 15:44 ragfmk/elements/embeddings/ollamaEmbeddings.py
+-rw-rw-rw-  2.0 fat     1833 b- defN 24-May-08 14:39 ragfmk/elements/embeddings/stEmbeddings.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Dec-21 09:21 ragfmk/elements/llms/__init__.py
 -rw-rw-rw-  2.0 fat     1245 b- defN 24-Apr-27 09:28 ragfmk/elements/llms/ollama.py
--rw-rw-rw-  2.0 fat     3390 b- defN 24-May-06 08:12 ragfmk/elements/simsearchengines/ChromaDBWrapper.py
+-rw-rw-rw-  2.0 fat     3390 b- defN 24-May-08 16:02 ragfmk/elements/simsearchengines/ChromaDBWrapper.py
 -rw-rw-rw-  2.0 fat     4814 b- defN 24-May-06 08:12 ragfmk/elements/simsearchengines/FAISSWrapper.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-25 16:16 ragfmk/elements/simsearchengines/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Dec-21 09:21 ragfmk/elements/wrappers/__init__.py
--rw-rw-rw-  2.0 fat     3155 b- defN 24-May-06 08:12 ragfmk/elements/wrappers/chunks.py
+-rw-rw-rw-  2.0 fat     3203 b- defN 24-May-08 13:09 ragfmk/elements/wrappers/chunks.py
 -rw-rw-rw-  2.0 fat     7519 b- defN 24-May-06 08:12 ragfmk/elements/wrappers/document.py
 -rw-rw-rw-  2.0 fat     3128 b- defN 24-May-06 08:12 ragfmk/elements/wrappers/nearest.py
 -rw-rw-rw-  2.0 fat     1850 b- defN 24-May-06 08:12 ragfmk/elements/wrappers/prompt.py
 -rw-rw-rw-  2.0 fat      740 b- defN 24-May-01 15:19 ragfmk/interfaces/IChunks.py
 -rw-rw-rw-  2.0 fat      425 b- defN 24-May-01 15:19 ragfmk/interfaces/IDocument.py
--rw-rw-rw-  2.0 fat      748 b- defN 24-May-02 11:49 ragfmk/interfaces/IEmbeddings.py
+-rw-rw-rw-  2.0 fat      916 b- defN 24-May-08 16:07 ragfmk/interfaces/IEmbeddings.py
 -rw-rw-rw-  2.0 fat      895 b- defN 24-May-02 09:04 ragfmk/interfaces/INearest.py
 -rw-rw-rw-  2.0 fat      581 b- defN 24-May-01 15:19 ragfmk/interfaces/IPrompt.py
 -rw-rw-rw-  2.0 fat     1230 b- defN 24-May-01 15:19 ragfmk/interfaces/IRag.py
--rw-rw-rw-  2.0 fat     1844 b- defN 24-May-05 15:52 ragfmk/utils/CONST.py
+-rw-rw-rw-  2.0 fat     1842 b- defN 24-May-08 15:51 ragfmk/utils/CONST.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-25 16:16 ragfmk/utils/__init__.py
 -rw-rw-rw-  2.0 fat     1929 b- defN 24-May-06 08:12 ragfmk/utils/log.py
 -rw-rw-rw-  2.0 fat     1907 b- defN 24-Apr-22 13:53 ragfmk/utils/milestone.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-May-06 08:45 ragfmk-0.1.4.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     8593 b- defN 24-May-06 08:45 ragfmk-0.1.4.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-06 08:45 ragfmk-0.1.4.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       86 b- defN 24-May-06 08:45 ragfmk-0.1.4.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       51 b- defN 24-May-06 08:45 ragfmk-0.1.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3295 b- defN 24-May-06 08:45 ragfmk-0.1.4.4.dist-info/RECORD
-39 files, 79283 bytes uncompressed, 27648 bytes compressed:  65.1%
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-May-19 16:16 ragfmk-0.1.4.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     8713 b- defN 24-May-19 16:16 ragfmk-0.1.4.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-19 16:16 ragfmk-0.1.4.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       86 b- defN 24-May-19 16:16 ragfmk-0.1.4.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       51 b- defN 24-May-19 16:16 ragfmk-0.1.4.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3391 b- defN 24-May-19 16:16 ragfmk-0.1.4.7.dist-info/RECORD
+40 files, 81486 bytes uncompressed, 28097 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -24,14 +24,17 @@
 
 Filename: ragfmk/elements/__init__.py
 Comment: 
 
 Filename: ragfmk/elements/embeddings/__init__.py
 Comment: 
 
+Filename: ragfmk/elements/embeddings/embedding.py
+Comment: 
+
 Filename: ragfmk/elements/embeddings/embeddings.py
 Comment: 
 
 Filename: ragfmk/elements/embeddings/ollamaEmbeddings.py
 Comment: 
 
 Filename: ragfmk/elements/embeddings/stEmbeddings.py
@@ -93,26 +96,26 @@
 
 Filename: ragfmk/utils/log.py
 Comment: 
 
 Filename: ragfmk/utils/milestone.py
 Comment: 
 
-Filename: ragfmk-0.1.4.4.dist-info/LICENSE
+Filename: ragfmk-0.1.4.7.dist-info/LICENSE
 Comment: 
 
-Filename: ragfmk-0.1.4.4.dist-info/METADATA
+Filename: ragfmk-0.1.4.7.dist-info/METADATA
 Comment: 
 
-Filename: ragfmk-0.1.4.4.dist-info/WHEEL
+Filename: ragfmk-0.1.4.7.dist-info/WHEEL
 Comment: 
 
-Filename: ragfmk-0.1.4.4.dist-info/entry_points.txt
+Filename: ragfmk-0.1.4.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: ragfmk-0.1.4.4.dist-info/top_level.txt
+Filename: ragfmk-0.1.4.7.dist-info/top_level.txt
 Comment: 
 
-Filename: ragfmk-0.1.4.4.dist-info/RECORD
+Filename: ragfmk-0.1.4.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ragfmk/rag.py

```diff
@@ -2,14 +2,15 @@
 __email__ = "benoit@datacorner.fr"
 __license__ = "MIT"
 
 from ragfmk.elements.wrappers.document import document
 from ragfmk.elements.llms.ollama import ollama
 from ragfmk.elements.wrappers.prompt import prompt
 from ragfmk.utils.milestone import milestone
+from ragfmk.elements.embeddings.embeddings import embeddings
 from ragfmk.elements.embeddings.stEmbeddings import stEmbeddings
 from ragfmk.elements.wrappers.chunks import chunks
 from ragfmk.utils.log import log
 from ragfmk.interfaces.IRag import IRag
 import ragfmk.utils.CONST as C
 import os
 
@@ -66,15 +67,15 @@
                             level=self.__logLevel)
         return self.__myLog
 
     def addMilestone(self, name, description, *others):
         self.__milestones.add(name, description, others)
         self.log.info("Step {} -> {}".format(name, self.__fmtMsgForLog(description)))
 
-    def readTXT(self, txtfile) -> str:
+    def readTXT(self, txtfile):
         """ Reads a txt file
         Args:
             txtfile (str): text file path
         Returns:
             str: text read
         """
         try:
@@ -85,17 +86,17 @@
             if (len(doc.content) <= 0):
                 raise Exception("Error while reading the TXT document")
             self.addMilestone("PDF2TXT", "TXT file successfully loaded. Text length : {}".format(len(doc.content)))
             self.log.info("TXT file loaded successfully")
             return doc
         except Exception as e:
             self.log.error("Error while reading the TXT file: {}".format(str(e)))
-            return ""
+            return document()
 
-    def readPDF(self, pdffile, method = C.READER_VALPYPDF) -> str:
+    def readPDF(self, pdffile, method = C.READER_VALPYPDF):
         """ Reads a pdf file and converts it to Text
         Args:
             pdffile (str): pdf file path
             method (str, optional): Type of conversion. Defaults to C.READER_VALPYPDF.
         Returns:
             str: text converted
         """
@@ -110,15 +111,15 @@
             if (len(pdf.content) <= 0):
                 raise Exception("Error while converting the PDF document to text")
             self.addMilestone("PDF2TXT", "PDF converted to TEXT successfully. Text length : {}".format(len(pdf.content)))
             self.log.info("PDF file opened successfully")
             return pdf
         except Exception as e:
             self.log.error("Error while reading the PDF file: {}".format(str(e)))
-            return ""
+            return document()
             
     def charChunk(self, doc, separator, chunk_size, chunk_overlap) -> chunks:
         """ Document character chunking process
         Args:
             doc (elements.document): Text / document to chunk
             separator (str): Chunks separator
             chunk_size (str): chunk size
@@ -196,24 +197,24 @@
             self.addMilestone("LLMPT", "LLM Reponse\n {}\n".format(resp))
             self.log.info("Prompt managed successfully by the LLM.")
             return resp
         except Exception as e:
             self.log.error("Error while prompting the LLM {}".format(str(e)))
             return ""
     
-    def createEmbeddings(self, cks) -> stEmbeddings:
+    def createEmbeddings(self, cks, embds = stEmbeddings()) -> embeddings:
         """ create embeddings for a list of chunks
         Args:
-            cks (chunks): Chunks object
+            cks (chunks): Chunks object (list of texts)
+            embds (embeddings): embeddings object Factory by default stEmbeddings (Sentence Transformer)
         Returns:
             json: data and embeddings
         """
         try:
             self.log.info("Create embeddings for list of texts/chunks ...")
-            embds = stEmbeddings()
             if (not embds.create(cks)):
                 raise Exception("Error while creating the chunks embeddings")
             self.addMilestone("DOCEMBEDDGS", "Embeddings created from chunks successfully")
             self.log.info("Embeddings created successfully")
             return embds
         except Exception as e:
             self.log.error("Error while creating the list of texts/chunks embeddings {}".format(str(e)))
```

## ragfmk/elements/embeddings/embeddings.py

```diff
@@ -2,14 +2,15 @@
 __email__ = "benoit@datacorner.fr"
 __license__ = "MIT"
 
 import json
 from numpyencoder import NumpyEncoder
 from ragfmk.interfaces.IEmbeddings import IEmbeddings
 import ragfmk.utils.CONST as C
+from ragfmk.elements.embeddings.embedding import embedding
 
 """
         Embeddings and data are stored in Python list/JSON and used with the following format :
         {"0": {
                 'text': 'The prompt or text', 
                 'embedding': array([-6.65125623e-02,  
                                     ..., 
@@ -22,75 +23,57 @@
         ...,
         "x" : { ... }
         }
 """
 
 class embeddings(IEmbeddings):
     def __init__(self):
-        self.__content = {}
-
-    @property
-    def content(self) -> str: 
-        return self.__content
+        self.__embeddings = {}
     
     @property
     def jsonContent(self) -> str: 
-        return json.dumps(self.__content, cls=NumpyEncoder)
+        return json.dumps(self.content, cls=NumpyEncoder)
     @jsonContent.setter
-    def jsonContent(self, content):
-        try:
-            self.__content = json.loads(content)
-        except Exception as e:
-            self.items = {}
-            raise
+    def jsonContent(self, jsondata):
+        embsLoaded = json.loads(jsondata)
+        for key, value in embsLoaded.items():
+            emb = embedding()
+            emb.init(value[C.JST_TEXT], value[C.JST_EMBEDDINGS])
+            self.__embeddings[key] = emb
 
     @property
-    def size(self):
-        return len(self.__content)
+    def content(self): 
+        myJsonList = {}
+        for key, value in self.__embeddings.items():
+            myJsonList[key] = value.content
+        return myJsonList
+    
+    @property
+    def items(self):
+        return self.__embeddings
+    @items.setter
+    def items(self, it):
+        self.__embeddings = it
         
-    def encode(self, cks):
-        """ to surcharge with the embeddings class
-        Args:
-            cks ( array []): list of chunks to create embeddings for each  
-        Returns:
-            numpy.ndarray: vector embeddings
-        """
-        return None
-
-    def __wrap(self, vectAndData):
-        """ Wrap the Dataframe into a list (to have a json later)
-        The Dataframe contains 2 columns: 
-            1) text : with the data
-            2) embedding: with the vector/embeddings calculated (as a nparray)
+    def __getitem__(self, item):
+        """ Makes the Data column accessible via [] array
+            example: df['colName']
         Args:
-            vectAndData (Dataframe): Data and embeddings
+            item (str): attribute/column name
         Returns:
-            {}: list for a later JSON conversion
+            object: data
         """
-        self.__content = {}
-        for i, (chunk, vector) in enumerate(vectAndData):
-            line = {}
-            line[C.JST_TEXT] = chunk
-            line[C.JST_EMBEDDINGS] = vector
-            self.__content[i] = line
+        return self.__embeddings.__getitem__(item)
+    
+    @property
+    def size(self):
+        return len(self.__embeddings)
 
     def create(self, cks) -> bool:
-        """ Calculate the embeddings for list of chunks
-        Args:
-            cks (chunks):  chunks object
-        Returns:
-            str: json with data and embeddings for all chunks
-        """
-        try: 
-            vect = self.encode(cks)
-            vectAndData = zip(cks.items, vect)
-            self.__wrap(vectAndData)
-            return True
-        except Exception as e:
-            return False
+        return False
 
     def save(self, filename) -> bool:
         """ Save the chunks in a file.
         Args:
             filename (_type_): JSON chunks file
         Returns:
             bool: True if ok
@@ -102,24 +85,23 @@
         except Exception as e:
             return False
 
     def load(self, filename = "", content = "") -> bool:
         """ Load and build a chunk file (can be loaded from a json file or a json content). 
             Format required : Content = {"chunks": [..., ...] }
         Args:
-            filename (str, optional): JSON chunks file. Defaults to "".
-            content (str, optional): JSON chunks content. Defaults to "".
+            filename (str, optional): JSON embeddings file. Defaults to "".
+            content (str, optional): JSON embeddings content. Defaults to "".
         Returns:
             bool: True if ok
         """
         try:
-            self.__content = {}
-            if (len(filename) >0):
+            if (len(filename) > 0):
                 with open(filename, "r", encoding=C.ENCODING) as f:
-                    self.__content = json.load(f)
+                    self.jsonContent = f.read()
             elif (len(content) >0):
-                self.__content = content
+                self.jsonContent = content
             else:
                 return False
             return True
         except Exception as e:
             return False
```

## ragfmk/elements/embeddings/ollamaEmbeddings.py

```diff
@@ -3,14 +3,15 @@
 __license__ = "MIT"
 
 import requests
 import json
 
 import ragfmk.utils.CONST as C
 from ragfmk.elements.embeddings.embeddings import embeddings
+from ragfmk.elements.embeddings.embedding import embedding
 
 """
         Embeddings and data are stored in Python list/JSON and used with the following format :
         {"0": {
                 'text': 'The prompt or text', 
                 'embedding': array([-6.65125623e-02,  
                                     ..., 
@@ -41,33 +42,38 @@
     @property
     def urlbase(self) -> str: 
         return self.__urlbase
     @urlbase.setter
     def urlbase(self, url):
         self.__urlbase = url
 
-    def _getEmbeddings(self, prompt):
+    def __getEmbeddings(self, prompt) -> embedding:
         try:
             url = self.urlbase + "/embeddings"
             params = {"model": self.model,
                       "prompt": prompt}
             response = requests.post(url, json=params)
             if (response.status_code == 200):
                 response_text = response.text
                 data = json.loads(response_text)
-                return data["embedding"]
+                emb = embedding()
+                emb.init(prompt, data["embedding"])
+                return emb
             else:
                 raise Exception("Error while reaching out to the Web Service: {}", str(response.status_code, response.text))
         except Exception as e:
-            return str(e)
+            return None
 
-    def encode(self, cks):
+    def create(self, cks) -> bool:
         """ to surcharge with the embeddings class
         Args:
             cks (array []): list of chunks to create embeddings for each  
         Returns:
             numpy.ndarray: vector embeddings
         """
         try:
-            return self._getEmbeddings(cks.items)
+            self.items = {}
+            for i, item in enumerate(cks.items):
+                vect = self.__getEmbeddings(item) # cks.items[0]
+                self.items[str(i)] = vect
         except:
-            return None
+            return False
```

## ragfmk/elements/embeddings/stEmbeddings.py

```diff
@@ -1,14 +1,15 @@
 __author__ = "Benoit CAYLA"
 __email__ = "benoit@datacorner.fr"
 __license__ = "MIT"
 
 from sentence_transformers import SentenceTransformer
 import ragfmk.utils.CONST as C
 from ragfmk.elements.embeddings.embeddings import embeddings
+from ragfmk.elements.embeddings.embedding import embedding
 
 """
         Embeddings and data are stored in Python list/JSON and used with the following format :
         {"0": {
                 'text': 'The prompt or text', 
                 'embedding': array([-6.65125623e-02,  
                                     ..., 
@@ -31,19 +32,26 @@
     @property
     def model(self) -> str: 
         return self.__embeddingsModel
     @model.setter
     def model(self, model):
         self.__embeddingsModel = model
 
-    def encode(self, cks):
-        """ to surcharge with the embeddings class
+    def create(self, cks) -> bool:
+        """ Calculate the embeddings for list of chunks
         Args:
-            cks ( array []): list of chunks to create embeddings for each  
+            cks (chunks):  chunks object
         Returns:
-            numpy.ndarray: vector embeddings
+            str: json with data and embeddings for all chunks
         """
-        try:
+        try: 
             encoder = SentenceTransformer(self.__embeddingsModel)
-            return encoder.encode(cks.items)
-        except:
-            return None
+            vect = encoder.encode(cks.items)
+            vectAndData = zip(cks.items, vect)
+            self.items = {}
+            for i, (chunk, vector) in enumerate(vectAndData):
+                emb = embedding()
+                emb.init(chunk, vector)
+                self.items[str(i)] = emb
+            return True
+        except Exception as e:
+            return False
```

## ragfmk/elements/wrappers/chunks.py

```diff
@@ -90,15 +90,16 @@
             bool: True if ok
         """
         try:
             jsonEnv = ""
             if (len(filename) >0):
                 with open(filename, "r", encoding=C.ENCODING) as f:
                     jsonEnv = json.load(f)
+                self.items = jsonEnv[C.JST_CHUNKS]
             elif (len(content) >0):
                 jsonEnv = content
+                self.items.append(jsonEnv)
             else:
                 return False
-            self.items = jsonEnv[C.JST_CHUNKS]
             return True
         except Exception as e:
             return False
```

## ragfmk/interfaces/IEmbeddings.py

```diff
@@ -3,32 +3,41 @@
 __license__ = "MIT"
 
 from abc import ABC, abstractmethod
 
 class IEmbeddings(ABC):
     
     @property
-    def content(self): 
-        pass
-    
-    @property
     @abstractmethod
     def jsonContent(self):
         pass
     @jsonContent.setter
     def jsonContent(self, content):
         pass
     
     @property
     @abstractmethod
-    def size(self):
+    def content(self): 
+        pass
+        
+    @property
+    @abstractmethod
+    def items(self):
+        pass
+    @items.setter
+    def items(self, it):
         pass
     
     @abstractmethod
-    def encode(self, cks):
+    def __getitem__(self, item):
+        pass
+    
+    @property
+    @abstractmethod
+    def size(self):
         pass
     
     @abstractmethod
     def create(self, cks):
         pass
     
     @abstractmethod
```

## ragfmk/utils/CONST.py

```diff
@@ -44,15 +44,14 @@
 PROMPT_RAG_JINJA_TEMPLATE = "Question: {{question}}\n \
     Please answer the question based on the informations listed below: \n \
     {%- for item in nearestItems.items %} \
     Item: \n \
     {{ item }} \n \
     {% endfor %}"
 
-
 # Output status
 OUT_ERROR = "ERROR"
 OUT_SUCCESS = "SUCCESS"
 
 # Llamaparse
 LLAMAPARSE_API_URL = "https://api.cloud.llamaindex.ai/api/parsing"
 LLAMAPARSE_API_WAITSEC = 2
```

## Comparing `ragfmk-0.1.4.4.dist-info/LICENSE` & `ragfmk-0.1.4.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ragfmk-0.1.4.4.dist-info/RECORD` & `ragfmk-0.1.4.7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 RagAdhocQueryDoc.py,sha256=ncPLYMFoU9ky5jYaXPyJ-J0bi5v-mJXUIzbjBfEV2Yw,3657
 RagPrompt.py,sha256=WlBntCbi2iSZQeaNW_GzdSg65w24Lp3EpQwR40AulYI,1731
 RagTest.py,sha256=lOtSF1MOmkDc2fMIpcICHOowgEMROMCg_b-PS-B_ZC8,2239
 __init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ragfmk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ragfmk/rag.py,sha256=X8wtfcyY8CBxaLu8irBTCSC-JgJhq7JU5GQS844F0kY,9012
+ragfmk/rag.py,sha256=sMbJyuAY7aJbheNhZTPfAIfUlzsC51eRqXHd-RE6D0I,9184
 ragfmk/ragChromaDB.py,sha256=LSyPDjYeTyDsmEmHPKJ-8GT136qFJO5hz1wizr9CGDk,2641
 ragfmk/ragFAISS.py,sha256=meQFOPO_s1ke9jabnwnxXjLjGoUqUqTnmkQ34Mapvo4,3716
 ragfmk/elements/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ragfmk/elements/embeddings/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ragfmk/elements/embeddings/embeddings.py,sha256=By8UpEBqX4RaQZ394rdX20ZY6y4MLMZvI5BB6NGT9GU,3965
-ragfmk/elements/embeddings/ollamaEmbeddings.py,sha256=dsT45MQR8-wFjPvAB_sXLW_GSJJj_XUQ7vekjEcEi7w,2236
-ragfmk/elements/embeddings/stEmbeddings.py,sha256=Xn8jsHkk0wfGnC_gh4jLzEwA9KcLqQcj_usS6GxNLaU,1478
+ragfmk/elements/embeddings/embedding.py,sha256=cmVbqR1-8dwcktghdctmTDhEn8QeiId2EkBrB8Jyl5E,1586
+ragfmk/elements/embeddings/embeddings.py,sha256=8qrLKBOfdXqbbeyWEl2SK7_Ug_dBISGwjM5rCxfR9Lo,3333
+ragfmk/elements/embeddings/ollamaEmbeddings.py,sha256=z-Bxq6zKHPkUoQUVY4oo98EKCM3Yrf37O2vWextDx_8,2528
+ragfmk/elements/embeddings/stEmbeddings.py,sha256=ckR-gL2mHMKId9I8DfGPoWrQeLhNctaZJpMq6iDnhQA,1833
 ragfmk/elements/llms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ragfmk/elements/llms/ollama.py,sha256=q78U-2bh4qk-JuO1lM8reMsrA1SG12k6KRyWkrsf8dg,1245
 ragfmk/elements/simsearchengines/ChromaDBWrapper.py,sha256=mtNMIWED5V1aY36vIvGk4pnqo0gTQoMEN_dDzd3mv-Q,3390
 ragfmk/elements/simsearchengines/FAISSWrapper.py,sha256=CCRRVoFfturN4-QqC_vmBzZjrlkTj6GC1SBtx1ISKuc,4814
 ragfmk/elements/simsearchengines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ragfmk/elements/wrappers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ragfmk/elements/wrappers/chunks.py,sha256=BE09nzR2lwo8fmI59EsMhAnB6qn-go-2KCaWufy7iSY,3155
+ragfmk/elements/wrappers/chunks.py,sha256=uBiTw2LP6waZe_uEpIGIfkuZUubwVf2vX6JbaCZC-3k,3203
 ragfmk/elements/wrappers/document.py,sha256=94to3cUwiypdcLwlDHwEtcy1d4W6EdTDkOf79juWRUE,7519
 ragfmk/elements/wrappers/nearest.py,sha256=ZDsjrOTFwkleFVMBnRe0vclaiypzG4pNyqCaICXmkBM,3128
 ragfmk/elements/wrappers/prompt.py,sha256=tsOH_Z8XRxuHhz7EmzEmfJdYxuYd99D4Eo0EgBM2-kE,1850
 ragfmk/interfaces/IChunks.py,sha256=1dBqYCEXgWiNQAiteQHcG-ZQ_uCluUPaGXCyBSMXZto,740
 ragfmk/interfaces/IDocument.py,sha256=0KrP-0szl8qHDH1TyC5opBqxTJV1dAIe9nTeNetiUR0,425
-ragfmk/interfaces/IEmbeddings.py,sha256=nRpdaz6Ms1wJ48GHvK7rgUO_ict8zcAaFYYel6jgE-w,748
+ragfmk/interfaces/IEmbeddings.py,sha256=To1PGoNXFIplJf40CVrEUDoXcMRXkBNwtsYYlfI_nF4,916
 ragfmk/interfaces/INearest.py,sha256=DvPacdOW7lRzzX7MpdyvF3SlczjIlyxYrrQ-HcSV4bg,895
 ragfmk/interfaces/IPrompt.py,sha256=pZf8xQlKUw5s2Q4MSyxfpIQyNXGb6fjDwf9S1KAK9jg,581
 ragfmk/interfaces/IRag.py,sha256=-8OGjnOn_6G3kt5B_RP0x6oWQiPXo7Rdf9EJcNZ4YnI,1230
-ragfmk/utils/CONST.py,sha256=9Nz0_GTnGBCXiDoq2HNOEFVjH_pxlbBMnwzLC7GIfro,1844
+ragfmk/utils/CONST.py,sha256=ftYmVGuexCo7hF5_-llP2NBvZ_T_sFwpTPMiKhhPlYI,1842
 ragfmk/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ragfmk/utils/log.py,sha256=UlOwYPmCYK9N8Aim60egeT605uUoqoBqoswCpmsY6bk,1929
 ragfmk/utils/milestone.py,sha256=dA5T_0QVWtHv3HaAFVZkKCEdRDS2SQSJsi7g0e_glGw,1907
-ragfmk-0.1.4.4.dist-info/LICENSE,sha256=BvMmeujpLDerNqzsA1gOET7mphtef9ebt_u8-bp4bNA,1091
-ragfmk-0.1.4.4.dist-info/METADATA,sha256=FuzUT3yDLUKu4Gbl62BTD0O4kCekTQCRUNMSOQZPzjY,8593
-ragfmk-0.1.4.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ragfmk-0.1.4.4.dist-info/entry_points.txt,sha256=EDEdK3AmGTz0ZLfXx10aBUy50jxn6Uy3isBcmPkE3jg,86
-ragfmk-0.1.4.4.dist-info/top_level.txt,sha256=LlNlUm1ce3g4y9ARq9Q4C-19JnDcERKf-aDueiUfWG8,51
-ragfmk-0.1.4.4.dist-info/RECORD,,
+ragfmk-0.1.4.7.dist-info/LICENSE,sha256=BvMmeujpLDerNqzsA1gOET7mphtef9ebt_u8-bp4bNA,1091
+ragfmk-0.1.4.7.dist-info/METADATA,sha256=Ka_2T3k9H48puAzAFDjh464IfI8mmrlVX0TzStaEHdo,8713
+ragfmk-0.1.4.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ragfmk-0.1.4.7.dist-info/entry_points.txt,sha256=EDEdK3AmGTz0ZLfXx10aBUy50jxn6Uy3isBcmPkE3jg,86
+ragfmk-0.1.4.7.dist-info/top_level.txt,sha256=LlNlUm1ce3g4y9ARq9Q4C-19JnDcERKf-aDueiUfWG8,51
+ragfmk-0.1.4.7.dist-info/RECORD,,
```

