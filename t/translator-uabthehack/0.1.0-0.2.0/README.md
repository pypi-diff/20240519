# Comparing `tmp/translator_uabthehack-0.1.0.tar.gz` & `tmp/translator_uabthehack-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translator_uabthehack-0.1.0.tar", max compression
+gzip compressed data, was "translator_uabthehack-0.2.0.tar", max compression
```

## Comparing `translator_uabthehack-0.1.0.tar` & `translator_uabthehack-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-19 07:25:11.069376 translator_uabthehack-0.1.0/README.md
--rw-r--r--   0        0        0      313 2024-05-19 07:25:52.802709 translator_uabthehack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 07:25:46.106042 translator_uabthehack-0.1.0/translator_uabthehack/__init__.py
--rw-r--r--   0        0        0     4111 2024-05-19 07:25:46.106042 translator_uabthehack-0.1.0/translator_uabthehack/main.py
--rw-r--r--   0        0        0      728 2024-05-19 07:25:46.106042 translator_uabthehack-0.1.0/translator_uabthehack/traductor.py
--rw-r--r--   0        0        0     1078 2024-05-19 07:25:46.106042 translator_uabthehack-0.1.0/translator_uabthehack/variable_seeker.py
--rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 translator_uabthehack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-19 07:59:55.909363 translator_uabthehack-0.2.0/README.md
+-rw-r--r--   0        0        0      313 2024-05-19 08:00:57.829362 translator_uabthehack-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 07:59:57.622696 translator_uabthehack-0.2.0/translator_uabthehack/__init__.py
+-rw-r--r--   0        0        0     4116 2024-05-19 07:59:57.622696 translator_uabthehack-0.2.0/translator_uabthehack/main.py
+-rw-r--r--   0        0        0      728 2024-05-19 07:59:57.622696 translator_uabthehack-0.2.0/translator_uabthehack/traductor.py
+-rw-r--r--   0        0        0     1078 2024-05-19 07:59:57.622696 translator_uabthehack-0.2.0/translator_uabthehack/variable_seeker.py
+-rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 translator_uabthehack-0.2.0/PKG-INFO
```

### Comparing `translator_uabthehack-0.1.0/translator_uabthehack/main.py` & `translator_uabthehack-0.2.0/translator_uabthehack/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,18 +33,15 @@
             # Si està a les variables, la canviem
             new_word = '_'.join(literal_trns)
         else:
             new_word = word             # Si no, la deixem igual
         translated += new_word          # Afegim la nova paraula
     return translated                   # Retornem la traducció
 
-def main():
-    input_file = sys.argv[1]
-    trans_language=sys.argv[2]
-    output_file = sys.argv[3]
+def translate_code(input_file, trans_language, output_file):
 
 
     languages = {
     'af': 'Afrikaans', 'ar': 'Arabic', 'bg': 'Bulgarian', 'bn': 'Bengali', 'ca': 'Catalan', 'cs': 'Czech',
     'cy': 'Welsh', 'da': 'Danish', 'de': 'German', 'el': 'Greek', 'en': 'English', 'es': 'Spanish',
     'et': 'Estonian', 'fa': 'Persian (Farsi)', 'fi': 'Finnish', 'fr': 'French', 'gu': 'Gujarati', 'he': 'Hebrew',
     'hi': 'Hindi', 'hr': 'Croatian', 'hu': 'Hungarian', 'id': 'Indonesian', 'it': 'Italian', 'ja': 'Japanese',
@@ -86,8 +83,8 @@
                 if(text == "\"\"\"" or text == "\'\'\'"):
                     toggle = not toggle
                     output.write(text + "\n")
                 else:
                     process_line(text, toggle, traductor, output)
 
 if __name__=="__main__":    
-    main()
+    translate_code(sys.argv[1],sys.argv[2], sys.argv[3])
```

### Comparing `translator_uabthehack-0.1.0/translator_uabthehack/traductor.py` & `translator_uabthehack-0.2.0/translator_uabthehack/traductor.py`

 * *Files identical despite different names*

### Comparing `translator_uabthehack-0.1.0/translator_uabthehack/variable_seeker.py` & `translator_uabthehack-0.2.0/translator_uabthehack/variable_seeker.py`

 * *Files identical despite different names*

