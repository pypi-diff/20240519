# Comparing `tmp/verysimpletree-0.1.0b0.tar.gz` & `tmp/verysimpletree-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verysimpletree-0.1.0b0.tar", last modified: Sun May 12 13:06:33 2024, max compression
+gzip compressed data, was "verysimpletree-0.1.1b0.tar", last modified: Sun May 19 10:31:51 2024, max compression
```

## Comparing `verysimpletree-0.1.0b0.tar` & `verysimpletree-0.1.1b0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-12 13:06:33.988016 verysimpletree-0.1.0b0/
--rw-r--r--   0 aligorji   (501) staff       (20)      479 2024-05-12 13:06:33.987493 verysimpletree-0.1.0b0/PKG-INFO
--rw-r--r--   0 aligorji   (501) staff       (20)      101 2024-05-12 13:01:46.000000 verysimpletree-0.1.0b0/README.rst
--rw-r--r--   0 aligorji   (501) staff       (20)       38 2024-05-12 13:06:33.988118 verysimpletree-0.1.0b0/setup.cfg
--rw-r--r--   0 aligorji   (501) staff       (20)      694 2024-05-12 13:01:46.000000 verysimpletree-0.1.0b0/setup.py
-drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-12 13:06:33.983038 verysimpletree-0.1.0b0/verysimpletree/
--rw-r--r--   0 aligorji   (501) staff       (20)        0 2024-05-12 13:01:46.000000 verysimpletree-0.1.0b0/verysimpletree/__init__.py
--rw-r--r--   0 aligorji   (501) staff       (20)     5587 2024-05-12 13:01:46.000000 verysimpletree-0.1.0b0/verysimpletree/test_tree.py
--rw-r--r--   0 aligorji   (501) staff       (20)    12382 2024-05-12 13:01:46.000000 verysimpletree-0.1.0b0/verysimpletree/tree.py
-drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-12 13:06:33.986589 verysimpletree-0.1.0b0/verysimpletree.egg-info/
--rw-r--r--   0 aligorji   (501) staff       (20)      479 2024-05-12 13:06:33.000000 verysimpletree-0.1.0b0/verysimpletree.egg-info/PKG-INFO
--rw-r--r--   0 aligorji   (501) staff       (20)      249 2024-05-12 13:06:33.000000 verysimpletree-0.1.0b0/verysimpletree.egg-info/SOURCES.txt
--rw-r--r--   0 aligorji   (501) staff       (20)        1 2024-05-12 13:06:33.000000 verysimpletree-0.1.0b0/verysimpletree.egg-info/dependency_links.txt
--rw-r--r--   0 aligorji   (501) staff       (20)       15 2024-05-12 13:06:33.000000 verysimpletree-0.1.0b0/verysimpletree.egg-info/top_level.txt
+drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-19 10:31:51.862776 verysimpletree-0.1.1b0/
+-rw-r--r--   0 aligorji   (501) staff       (20)      479 2024-05-19 10:31:51.862172 verysimpletree-0.1.1b0/PKG-INFO
+-rw-r--r--   0 aligorji   (501) staff       (20)      101 2024-05-12 13:01:46.000000 verysimpletree-0.1.1b0/README.rst
+-rw-r--r--   0 aligorji   (501) staff       (20)       38 2024-05-19 10:31:51.862924 verysimpletree-0.1.1b0/setup.cfg
+-rw-r--r--   0 aligorji   (501) staff       (20)      694 2024-05-13 03:49:14.000000 verysimpletree-0.1.1b0/setup.py
+drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-19 10:31:51.858133 verysimpletree-0.1.1b0/verysimpletree/
+-rw-r--r--   0 aligorji   (501) staff       (20)        0 2024-05-12 13:01:46.000000 verysimpletree-0.1.1b0/verysimpletree/__init__.py
+-rw-r--r--   0 aligorji   (501) staff       (20)        0 2024-05-15 21:30:24.000000 verysimpletree-0.1.1b0/verysimpletree/py.typed
+-rw-r--r--   0 aligorji   (501) staff       (20)     6051 2024-05-19 10:29:30.000000 verysimpletree-0.1.1b0/verysimpletree/test_tree.py
+-rw-r--r--   0 aligorji   (501) staff       (20)    18762 2024-05-19 10:29:41.000000 verysimpletree-0.1.1b0/verysimpletree/tree.py
+drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-19 10:31:51.861339 verysimpletree-0.1.1b0/verysimpletree.egg-info/
+-rw-r--r--   0 aligorji   (501) staff       (20)      479 2024-05-19 10:31:51.000000 verysimpletree-0.1.1b0/verysimpletree.egg-info/PKG-INFO
+-rw-r--r--   0 aligorji   (501) staff       (20)      273 2024-05-19 10:31:51.000000 verysimpletree-0.1.1b0/verysimpletree.egg-info/SOURCES.txt
+-rw-r--r--   0 aligorji   (501) staff       (20)        1 2024-05-19 10:31:51.000000 verysimpletree-0.1.1b0/verysimpletree.egg-info/dependency_links.txt
+-rw-r--r--   0 aligorji   (501) staff       (20)       15 2024-05-19 10:31:51.000000 verysimpletree-0.1.1b0/verysimpletree.egg-info/top_level.txt
```

### Comparing `verysimpletree-0.1.0b0/setup.py` & `verysimpletree-0.1.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.rst").read_text()
 setuptools.setup(
     name="verysimpletree",
-    version="0.1.0beta",
+    version="0.1.1beta",
     author="Alex Gorji",
     author_email="aligorji@hotmail.com",
     description="lightweight tree data structure for musicxml and musicscore",
     url="https://github.com/alexgorji/verysimpletree.git",
     packages=setuptools.find_packages(),
     install_requires=[],
     classifiers=[
```

### Comparing `verysimpletree-0.1.0b0/verysimpletree/test_tree.py` & `verysimpletree-0.1.1b0/verysimpletree/test_tree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 
-from verysimpletree.tree import Tree, ChildNotFoundError
+from verysimpletree.tree import Tree, ChildNotFoundError, grandchild1
 
 
 class A(Tree):
     def __init__(self, name, parent=None, *args, **keyword):
         super().__init__(*args, **keyword)
         self._children = []
         self._parent = parent
@@ -33,14 +33,22 @@
         self.child3 = self.root.add_child('child3')
         self.child4 = self.root.add_child('child4')
         self.grandchild1 = self.child2.add_child('grandchild1')
         self.grandchild2 = self.child2.add_child('grandchild2')
         self.grandchild3 = self.child4.add_child('grandchild3')
         self.greatgrandchild1 = self.grandchild2.add_child('greatgrandchild1')
 
+    def test_is_last_child(self):
+        t = self.root
+        for node in t.traverse():
+            if node.name in ['root', 'child4', 'grandchild2', 'grandchild3', 'greatgrandchild1']:
+                assert node.is_last_child
+            else:
+                assert not node.is_last_child
+
     def test_get_root(self):
         assert self.greatgrandchild1.get_root() == self.root
         assert self.child4.get_root() == self.root
         assert self.root.get_root() == self.root
 
     def test_is_leaf(self):
         assert self.greatgrandchild1.is_leaf is True
@@ -52,49 +60,37 @@
                                               self.greatgrandchild1, self.child3, self.child4, self.grandchild3]
 
     def test_iterate_leaves(self):
         assert list(self.root.iterate_leaves()) == [self.child1, self.grandchild1, self.greatgrandchild1,
                                                     self.child3, self.grandchild3]
 
     def test_level(self):
-        assert [node.level for node in self.root.traverse()] == [0, 1, 1, 2, 2, 3, 1, 1, 2]
-        assert self.greatgrandchild1.level == 3
-        assert self.grandchild2.level == 2
-        assert self.child4.level == 1
-        assert self.root.level == 0
-
-    def test_tree_repr(self):
-        expected = """root
-    child1
-    child2
-        grandchild1
-        grandchild2
-            greatgrandchild1
-    child3
-    child4
-        grandchild3
-"""
-        assert self.root.tree_representation(lambda x: x.name) == expected
+        assert [node.get_level() for node in self.root.traverse()] == [0, 1, 1, 2, 2, 3, 1, 1, 2]
+        assert self.greatgrandchild1.get_level() == 3
+        assert self.grandchild2.get_level() == 2
+        assert self.child4.get_level() == 1
+        assert self.root.get_level() == 0
 
     def test_reversed_path_to_root(self):
-        assert list(self.greatgrandchild1.reversed_path_to_root()) == [self.greatgrandchild1, self.grandchild2, self.child2, self.root]
+        assert list(self.greatgrandchild1.get_reversed_path_to_root()) == [self.greatgrandchild1, self.grandchild2,
+                                                                           self.child2, self.root]
 
     def test_remove_child(self):
         with self.assertRaises(ChildNotFoundError):
             self.child2.remove(self.child1)
 
         self.child2.remove(self.grandchild2)
         assert self.child2.get_children() == [self.grandchild1]
         assert self.grandchild2.get_parent() is None
         assert self.greatgrandchild1.get_parent() == self.grandchild2
 
     def test_get_coordinates(self):
-        assert self.greatgrandchild1.get_coordinates_in_tree() == '2.2.1'
-        assert self.child2.get_coordinates_in_tree() == '2'
-        assert self.root.get_coordinates_in_tree() == '0'
+        assert self.greatgrandchild1.get_position_in_tree() == '2.2.1'
+        assert self.child2.get_position_in_tree() == '2'
+        assert self.root.get_position_in_tree() == '0'
 
     def test_replace_child(self):
         self.child2.replace_child(self.grandchild1, A(name='new_grand_child'))
         assert [ch.name for ch in self.child2.get_children()] == ['new_grand_child', 'grandchild2']
         self.child1.add_child('grandchild')
         self.child1.add_child('grandchild')
         new = A(name='other_new_grand_child')
@@ -115,22 +111,30 @@
     def test_next(self):
         assert self.child1.next == self.child2
         assert self.child2.next == self.child3
         assert self.child3.next == self.child4
         assert self.child4.next is None
 
     def test_get_leaves(self):
-        assert self.root.get_leaves(key=lambda x: x.name) == ['child1', ['grandchild1', ['greatgrandchild1']], 'child3', ['grandchild3']]
+        assert self.root.get_leaves(key=lambda x: x.name) == ['child1', ['grandchild1', ['greatgrandchild1']], 'child3',
+                                                              ['grandchild3']]
 
     def test_get_layer(self):
         assert self.root.get_layer(0) == [self.root]
         assert self.root.get_layer(1) == [self.child1, self.child2, self.child3, self.child4]
-        assert self.root.get_layer(2) == [self.child1, self.grandchild1, self.grandchild2, self.child3, self.grandchild3]
-        assert self.root.get_layer(3) == [self.child1, self.grandchild1, self.greatgrandchild1, self.child3, self.grandchild3]
-        assert self.root.get_layer(4) == [self.child1, self.grandchild1, self.greatgrandchild1, self.child3, self.grandchild3]
+        assert self.root.get_layer(2) == [self.child1, self.grandchild1, self.grandchild2, self.child3,
+                                          self.grandchild3]
+        assert self.root.get_layer(3) == [self.child1, self.grandchild1, self.greatgrandchild1, self.child3,
+                                          self.grandchild3]
+        assert self.root.get_layer(4) == [self.child1, self.grandchild1, self.greatgrandchild1, self.child3,
+                                          self.grandchild3]
+
+    def test_get_farthest_leaf(self):
+        pass
 
     def test_find_grandchild(self):
-        assert [n for n in self.root.traverse() if n.level == 2] == [self.grandchild1, self.grandchild2, self.grandchild3]
+        assert [n for n in self.root.traverse() if n.get_level() == 2] == [self.grandchild1, self.grandchild2,
+                                                                           self.grandchild3]
         for n in self.root.traverse():
-            if n.level == 2:
+            if n.get_level() == 2:
                 print(n)
-                break
+                break
```

