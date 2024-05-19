# Comparing `tmp/schubmult-1.3.7.tar.gz` & `tmp/schubmult-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubmult-1.3.7.tar", last modified: Sun May 12 18:39:23 2024, max compression
+gzip compressed data, was "schubmult-1.3.8.tar", last modified: Sun May 19 21:32:16 2024, max compression
```

## Comparing `schubmult-1.3.7.tar` & `schubmult-1.3.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:23.882000 schubmult-1.3.7/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.7/LICENSE
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     5681 2024-05-12 18:39:23.831000 schubmult-1.3.7/PKG-INFO
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     5299 2024-05-12 18:38:20.000000 schubmult-1.3.7/README.md
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:21.540000 schubmult-1.3.7/schubmult/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2023-09-24 17:08:26.000000 schubmult-1.3.7/schubmult/__init__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)    17334 2024-05-12 18:35:24.000000 schubmult-1.3.7/schubmult/perm_lib.py
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:22.269000 schubmult-1.3.7/schubmult/schubmult_double/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       41 2023-09-25 01:39:08.000000 schubmult-1.3.7/schubmult/schubmult_double/__init__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       97 2023-09-26 17:55:50.000000 schubmult-1.3.7/schubmult/schubmult_double/__main__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     4773 2024-04-10 12:45:13.000000 schubmult-1.3.7/schubmult/schubmult_double/schubmult_double.py
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:22.570000 schubmult-1.3.7/schubmult/schubmult_py/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       36 2023-09-25 01:39:03.000000 schubmult-1.3.7/schubmult/schubmult_py/__init__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       94 2023-09-26 17:55:38.000000 schubmult-1.3.7/schubmult/schubmult_py/__main__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     4373 2024-04-10 12:45:06.000000 schubmult-1.3.7/schubmult/schubmult_py/schubmult_py.py
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:22.859000 schubmult-1.3.7/schubmult/schubmult_q/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       36 2024-04-03 15:35:41.000000 schubmult-1.3.7/schubmult/schubmult_q/__init__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       92 2024-04-03 15:28:43.000000 schubmult-1.3.7/schubmult/schubmult_q/__main__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     9034 2024-05-01 11:44:33.000000 schubmult-1.3.7/schubmult/schubmult_q/schubmult_q.py
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:23.144000 schubmult-1.3.7/schubmult/schubmult_q_double/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       33 2024-04-12 18:50:20.000000 schubmult-1.3.7/schubmult/schubmult_q_double/__init__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       99 2024-04-12 18:49:31.000000 schubmult-1.3.7/schubmult/schubmult_q_double/__main__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     3215 2024-04-15 14:01:00.000000 schubmult-1.3.7/schubmult/schubmult_q_double/schubmult_q_double.py
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:23.456000 schubmult-1.3.7/schubmult/schubmult_q_yz/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       29 2024-04-12 18:49:56.000000 schubmult-1.3.7/schubmult/schubmult_q_yz/__init__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       95 2024-04-12 18:49:43.000000 schubmult-1.3.7/schubmult/schubmult_q_yz/__main__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     9952 2024-05-12 18:35:10.000000 schubmult-1.3.7/schubmult/schubmult_q_yz/schubmult_q_yz.py
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:23.756000 schubmult-1.3.7/schubmult/schubmult_yz/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       27 2023-09-25 01:38:28.000000 schubmult-1.3.7/schubmult/schubmult_yz/__init__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       93 2023-09-26 17:55:32.000000 schubmult-1.3.7/schubmult/schubmult_yz/__main__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)    42460 2024-04-12 14:57:13.000000 schubmult-1.3.7/schubmult/schubmult_yz/schubmult_yz.py
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:21.962000 schubmult-1.3.7/schubmult.egg-info/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     5681 2024-05-12 18:39:19.000000 schubmult-1.3.7/schubmult.egg-info/PKG-INFO
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)      978 2024-05-12 18:39:20.000000 schubmult-1.3.7/schubmult.egg-info/SOURCES.txt
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        1 2024-05-12 18:39:19.000000 schubmult-1.3.7/schubmult.egg-info/dependency_links.txt
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)      353 2024-05-12 18:39:19.000000 schubmult-1.3.7/schubmult.egg-info/entry_points.txt
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       83 2024-05-12 18:39:19.000000 schubmult-1.3.7/schubmult.egg-info/requires.txt
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       10 2024-05-12 18:39:20.000000 schubmult-1.3.7/schubmult.egg-info/top_level.txt
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       79 2024-05-12 18:39:23.866000 schubmult-1.3.7/setup.cfg
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     1243 2024-05-12 18:36:25.000000 schubmult-1.3.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:16.890000 schubmult-1.3.8/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5681 2024-05-19 21:32:16.835000 schubmult-1.3.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5299 2024-05-12 18:38:20.000000 schubmult-1.3.8/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:14.482000 schubmult-1.3.8/schubmult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.8/schubmult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    18084 2024-05-18 15:28:41.000000 schubmult-1.3.8/schubmult/perm_lib.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:15.229000 schubmult-1.3.8/schubmult/schubmult_double/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.8/schubmult/schubmult_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.8/schubmult/schubmult_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5027 2024-05-17 15:39:33.000000 schubmult-1.3.8/schubmult/schubmult_double/schubmult_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:15.514000 schubmult-1.3.8/schubmult/schubmult_py/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.8/schubmult/schubmult_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.8/schubmult/schubmult_py/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5757 2024-05-17 15:05:46.000000 schubmult-1.3.8/schubmult/schubmult_py/schubmult_py.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:15.833000 schubmult-1.3.8/schubmult/schubmult_q/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.8/schubmult/schubmult_q/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.8/schubmult/schubmult_q/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10420 2024-05-17 14:57:50.000000 schubmult-1.3.8/schubmult/schubmult_q/schubmult_q.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:16.120000 schubmult-1.3.8/schubmult/schubmult_q_double/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.8/schubmult/schubmult_q_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.8/schubmult/schubmult_q_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3456 2024-05-17 15:40:28.000000 schubmult-1.3.8/schubmult/schubmult_q_double/schubmult_q_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:16.435000 schubmult-1.3.8/schubmult/schubmult_q_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.8/schubmult/schubmult_q_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.8/schubmult/schubmult_q_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11896 2024-05-19 18:52:48.000000 schubmult-1.3.8/schubmult/schubmult_q_yz/schubmult_q_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:16.762000 schubmult-1.3.8/schubmult/schubmult_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.8/schubmult/schubmult_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.8/schubmult/schubmult_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    47306 2024-05-19 18:33:48.000000 schubmult-1.3.8/schubmult/schubmult_yz/schubmult_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:14.937000 schubmult-1.3.8/schubmult.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5681 2024-05-19 21:32:12.000000 schubmult-1.3.8/schubmult.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      978 2024-05-19 21:32:13.000000 schubmult-1.3.8/schubmult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-19 21:32:12.000000 schubmult-1.3.8/schubmult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      353 2024-05-19 21:32:12.000000 schubmult-1.3.8/schubmult.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       83 2024-05-19 21:32:12.000000 schubmult-1.3.8/schubmult.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-05-19 21:32:12.000000 schubmult-1.3.8/schubmult.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2024-05-19 21:32:16.872000 schubmult-1.3.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1243 2024-05-19 21:31:58.000000 schubmult-1.3.8/setup.py
```

### Comparing `schubmult-1.3.7/LICENSE` & `schubmult-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.7/PKG-INFO` & `schubmult-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.7
+Version: 1.3.8
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.7/README.md` & `schubmult-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.7/schubmult/perm_lib.py` & `schubmult-1.3.8/schubmult/perm_lib.py`

 * *Files 9% similar despite different names*

```diff
@@ -135,14 +135,36 @@
 						else:
 							new_perm_add = tuple(new_perm)
 						perm_list += [(new_perm_add,up_perm2[j])]
 						total_list+=[(new_perm_add,pp+1)]
 		up_perm_list = perm_list
 	return total_list
 
+def elem_sym_perms_op(orig_perm,p,k):	
+	total_list = [(orig_perm,0)]
+	up_perm_list = [(orig_perm,k)]
+	for pp in range(p):
+		perm_list = []
+		for up_perm, last in up_perm_list:	
+			up_perm2 = [*up_perm]
+			if len(up_perm2) < k + 1:
+				up_perm2 += [i+1 for i in range(len(up_perm2),k+2)]
+			pos_list = [i for i in range(k) if up_perm2[i] == orig_perm[i]]
+			for j in range(last,len(up_perm2)):				
+				for i in pos_list:								
+					if has_bruhat_descent(up_perm2,i,j):
+						new_perm = [*up_perm2]
+						new_perm[i],new_perm[j] = new_perm[j],new_perm[i]
+						new_perm_add = tuple(permtrim(new_perm))
+						perm_list += [(new_perm_add,j)]
+						total_list+=[(new_perm_add,pp+1)]
+		up_perm_list = perm_list
+	return total_list
+
+
 def strict_theta(u):
 	ret = [*trimcode(u)]
 	did_one = True
 	while did_one:
 		did_one = False
 		for i in range(len(ret)-2,-1,-1):
 			if ret[i+1]!=0 and ret[i] <= ret[i+1]:
```

### Comparing `schubmult-1.3.7/schubmult/schubmult_double/schubmult_double.py` & `schubmult-1.3.8/schubmult/schubmult_double/schubmult_double.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,69 @@
 from symengine import *
 from functools import cache
 from itertools import chain
 from schubmult.perm_lib import *
-from schubmult.schubmult_yz import schubmult
+from schubmult.schubmult_yz import schubmult, mult_poly
 import sys
 
 n = 100
 
 var = symarray('x', n)
 var2 = symarray('y',n)
 var3 = var2
 var_r = symarray('r',n)
 
 var_q = Symbol("q")
 
 subs_dict = {}
 
 for i in range(1,n):
-	sm = var_r[0]
+	sm = var2[1]
 	for j in range(1,i):
 		sm += var_r[j]
 	subs_dict[var2[i]] = sm
 
 
 
 def main():
 	try:			
 		perms=[]
 		curperm = []
 		
 		pr = True
 		ascode = False
 		coprod = False
+		mult = False
+		mulstring = ""
 		try:
 			for s in sys.argv[1:]:
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
+				if mult:
+					mulstring+=s
+					continue
 				if s == "-code":
 					ascode = True
 					continue
 				if s == "-coprod":
 					coprod = True
 					continue
 				if s == "-":
 					perms += [curperm]
 					curperm = []
 					continue
+				if s == "-mult":
+					mult = True
+					continue
 				curperm += [int(s)]
 		except Exception:
 			print("**** schubmult_double ****")
 			print("Purpose: Compute products (and coproducts) of double Schubert polynomials in the same set of variables")
-			print("Usage: schubmult_double <-np|--no-print> <-code> perm1 - perm2 < - perm 3 ... >")
+			print("Usage: schubmult_double <-np|--no-print> <-code> perm1 - perm2 < - perm 3 ... > <-mult poly>")
 			print("Alternative usage: schubmult_double <-code> -coprod perm - indexlist")
 			exit(1)
 		
 		perms += [curperm]
 		
 		
 		if coprod:
@@ -141,15 +149,18 @@
 				for i in range(len(perms)):
 					perms[i] = uncode(perms[i])
 			
 			coeff_dict = {tuple(permtrim([*perms[0]])): 1}
 			
 			for perm in perms[1:]:
 				coeff_dict = schubmult(coeff_dict,tuple(permtrim([*perm])),var2,var2)
-				
+			if mult:
+				mul_exp = sympify(mulstring)
+				coeff_dict = mult_poly(coeff_dict,mul_exp)
+			
 			if pr:
 				if ascode:
 					width = max([len(str(trimcode(perm))) for perm in coeff_dict.keys()])
 				else:
 					width = max([len(str(perm)) for perm in coeff_dict.keys()])
 				
 				coeff_perms = list(coeff_dict.keys())
```

### Comparing `schubmult-1.3.7/schubmult/schubmult_py/schubmult_py.py` & `schubmult-1.3.8/schubmult/schubmult_py/schubmult_py.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,55 @@
 import sys
 from functools import cache
 from itertools import chain
 from schubmult.perm_lib import *
+from symengine import *
+
+var_x = symarray("x",100).tolist()
+
+def single_variable(coeff_dict,varnum):
+	ret = {}
+	for u in coeff_dict:
+		new_perms_k = elem_sym_perms(u,1,varnum)
+		new_perms_km1 = []
+		if varnum > 1:
+			new_perms_km1 = elem_sym_perms(u,1,varnum-1)
+		for perm, udiff in new_perms_k:
+			if udiff == 1:
+				ret[perm] = ret.get(perm,0) + coeff_dict[u]
+		for perm, udiff in new_perms_km1:
+			if udiff == 1:
+				ret[perm] = ret.get(perm,0) - coeff_dict[u]
+	return ret
+
+def mult_poly(coeff_dict,poly):
+	if poly in var_x:
+		return single_variable(coeff_dict,var_x.index(poly))
+	elif isinstance(poly,Mul):
+		ret = coeff_dict
+		for a in poly.args:
+			ret = mult_poly(ret,a)
+		return ret
+	elif isinstance(poly,Pow):
+		base = poly.args[0]
+		exponent = int(poly.args[1])
+		ret = coeff_dict
+		for i in range(int(exponent)):
+			ret = mult_poly(ret,base)
+		return ret
+	elif isinstance(poly,Add):
+		ret = {}
+		for a in poly.args:
+			ret = add_perm_dict(ret,mult_poly(coeff_dict,a))
+		return ret
+	else:
+		ret = {}
+		for perm in coeff_dict:
+			ret[perm] = poly*coeff_dict[perm]
+		return ret
 
 def schubmult(perm_dict,v):
 	vn1 = inverse(v)
 	th = theta(vn1)
 	if th[0]==0:
 		return perm_dict		
 	mu = permtrim(uncode(th))
@@ -54,31 +98,40 @@
 	try:
 		perms=[]
 		curperm = []
 		
 		pr = True
 		coprod = False
 		ascode = False
+		mult = False
+		mulstring = ""
 		
 		try:
 			for s in sys.argv[1:]:
+				if mult:
+					mulstring += s
+					continue
+				if s == "-mult":
+					mult = True
+					continue
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
 				if s == "-coprod":
 					coprod = True
 					continue
 				if s == "-code":
 					ascode = True
 					continue
 				if s == "-":
 					perms += [tuple(curperm)]
 					curperm = []
-					continue
-				curperm += [int(s)]
+					continue				
+				else:
+					curperm += [int(s)]
 		except Exception:
 			print("**** schubmult_py ****")
 			print("Purpose: Compute products (and coproducts) of ordinary Schubert polynomials")
 			print("Usage: schubmult_py <-np|--no-print> <-code> perm1 - perm2 <- perm3...>")
 			print("Alternative usage: schubmult_py -coprod <-np> <perm> - <index list>")
 			exit(1)
 		
@@ -134,19 +187,22 @@
 		else:
 			if ascode:
 				for i in range(len(perms)):
 					perms[i] = tuple(permtrim(uncode(perms[i])))
 		
 		
 			perms.sort(reverse=True,key=lambda x: sum(theta(inverse(x)))-inv(x))
-			
+					
 			coeff_dict = {tuple(permtrim([*perms[0]])): 1}
-			
+					
 			for perm in perms[1:]:
 				coeff_dict = schubmult(coeff_dict,tuple(permtrim([*perm])))
+			if mult:
+				mul_exp = sympify(mulstring)
+				coeff_dict = mult_poly(coeff_dict,mul_exp)
 				
 			if pr:
 				for perm, val in coeff_dict.items():
 					if val!= 0:
 						if ascode:						
 							print(f"{val}  {trimcode(perm)}")
 						else:
```

### Comparing `schubmult-1.3.7/schubmult/schubmult_q/schubmult_q.py` & `schubmult-1.3.8/schubmult/schubmult_q/schubmult_q.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,57 @@
 var3 = var2
 var_r = symarray('r',n)
 
 var_q = Symbol("q")
 
 subs_dict = {}
 
+var_x = symarray("x",100).tolist()
+
+def single_variable(coeff_dict,varnum):
+	ret = {}
+	for u in coeff_dict:
+		new_perms_k = elem_sym_perms_q(u,1,varnum)
+		new_perms_km1 = []
+		if varnum > 1:
+			new_perms_km1 = elem_sym_perms_q(u,1,varnum-1)
+		for perm, udiff, mul_val in new_perms_k:
+			if udiff == 1:
+				ret[perm] = ret.get(perm,0) + coeff_dict[u]*mul_val
+		for perm, udiff, mul_val in new_perms_km1:
+			if udiff == 1:
+				ret[perm] = ret.get(perm,0) - coeff_dict[u]*mul_val
+	return ret
+
+def mult_poly(coeff_dict,poly):
+	if poly in var_x:
+		return single_variable(coeff_dict,var_x.index(poly))
+	elif isinstance(poly,Mul):
+		ret = coeff_dict
+		for a in poly.args:
+			ret = mult_poly(ret,a)
+		return ret
+	elif isinstance(poly,Pow):
+		base = poly.args[0]
+		exponent = int(poly.args[1])
+		ret = coeff_dict
+		for i in range(int(exponent)):
+			ret = mult_poly(ret,base)
+		return ret
+	elif isinstance(poly,Add):
+		ret = {}
+		for a in poly.args:
+			ret = add_perm_dict(ret,mult_poly(coeff_dict,a))
+		return ret
+	else:
+		ret = {}
+		for perm in coeff_dict:
+			ret[perm] = poly*coeff_dict[perm]
+		return ret
+
 for i in range(1,n):
 	sm = var_r[0]
 	for j in range(1,i):
 		sm += var_r[j]
 	subs_dict[var2[i]] = sm
 
 def schubmult(perm_dict,v):
@@ -128,32 +171,41 @@
 		curperm = []
 		
 		pr = True
 		ascode = False
 		grass = False
 		grass_q_n = 0
 		equiv = False
+		mult = False
+		mulstring = ""
+		
 		try:
 			for s in sys.argv[1:]:
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
+				if mult:
+					mulstring += s
+					continue
 				if s == "-code":
 					ascode = True
 					continue
 				if s == "-grass":
 					grass = None
 					continue
 				if s == "-equiv":
 					equiv = True
 					continue
 				if grass is None:
 					grass = True
 					grass_q_n = int(s)
 					continue
+				if s == "-mult":
+					mult = True
+					continue
 				if s == "-":
 					perms += [curperm]
 					curperm = []
 					continue
 				curperm += [int(s)]
 		except Exception:
 			print("**** schubmult_q ****")
@@ -290,14 +342,18 @@
 				for i in range(len(perms)):
 					perms[i] = uncode(perms[i])
 		
 			coeff_dict = {tuple(permtrim([*perms[0]])): 1}
 			
 			for perm in perms[1:]:
 				coeff_dict = schubmult(coeff_dict,tuple(permtrim([*perm])))
+			
+			if mult:
+				mul_exp = sympify(mulstring)
+				coeff_dict = mult_poly(coeff_dict,mul_exp)
 				
 			if pr:
 				if ascode:
 					width = max([len(str(trimcode(perm))) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
 				else:
 					width = max([len(str(perm)) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
```

### Comparing `schubmult-1.3.7/schubmult/schubmult_q_double/schubmult_q_double.py` & `schubmult-1.3.8/schubmult/schubmult_q_double/schubmult_q_double.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from schubmult.perm_lib import *
-from schubmult.schubmult_q_yz import schubmult
+from schubmult.schubmult_q_yz import schubmult, mult_poly
 from symengine import *
 import sys
 
 
 q_var = symarray("q",100)
 
 var2 = symarray("y",100)
@@ -11,15 +11,15 @@
 
 var3 = var2
 var_r = symarray('r',100)
 
 subs_dict = {}
 
 for i in range(1,100):
-	sm = var_r[0]
+	sm = var2[1]
 	for j in range(1,i):
 		sm += var_r[j]
 	subs_dict[var2[i]] = sm
 	
 	
 
 def main():
@@ -32,19 +32,27 @@
 		
 		pr = True
 		display_positive = False
 		ascode = False
 		coprod = False
 		check = True
 		msg = False
+		mult = False
+		mulstring = ""
 		try:
 			for s in sys.argv[1:]:
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
+				if mult:
+					mulstring += s
+					continue
+				if s == "-mult":
+					mult = True
+					continue
 				if s == "-nocheck":
 					check = False
 					continue
 				if s == "--display-positive":
 					display_positive = True
 					continue
 				if s == "--optimizer-message":
@@ -85,14 +93,17 @@
 		
 		size = 0
 		L = len(perms)
 		
 		coeff_dict = {perms[0]: 1}
 		for perm in perms[1:]:
 			coeff_dict = schubmult(coeff_dict,perm,var2,var2)
+		if mult:
+			mul_exp = sympify(mulstring)
+			coeff_dict = mult_poly(coeff_dict,mul_exp)
 		
 		if pr:
 			if ascode:
 				width = max([len(str(trimcode(perm))) for perm in coeff_dict.keys() if expand(sympify(coeff_dict[perm]).subs(subs_dict))!=0])
 			else:
 				width = max([len(str(perm)) for perm in coeff_dict.keys() if expand(sympify(coeff_dict[perm]).subs(subs_dict))!=0])
```

### Comparing `schubmult-1.3.7/schubmult/schubmult_q_yz/schubmult_q_yz.py` & `schubmult-1.3.8/schubmult/schubmult_q_yz/schubmult_q_yz.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,67 @@
 from schubmult.schubmult_yz import compute_positive_rep, posify
 from symengine import *
 import sys
 
 var2 = symarray("y",100)
 var3 = symarray("z",100)
 
-var_x = symarray("x",100)
+var_y = var2.tolist()
+var_z = var3.tolist()
+var_x = symarray("x",100).tolist()
+
+def single_variable(coeff_dict,varnum):
+	ret = {}
+	for u in coeff_dict:
+		if varnum -1 < len(u):
+			ret[u] = ret.get(u,0) + var2[u[varnum-1]]*coeff_dict[u]
+		else:
+			ret[u] = ret.get(u,0) + var2[varnum]*coeff_dict[u]
+		new_perms_k = elem_sym_perms_q(u,1,varnum)
+		new_perms_km1 = []
+		if varnum > 1:
+			new_perms_km1 = elem_sym_perms_q(u,1,varnum-1)
+		for perm, udiff, mul_val in new_perms_k:
+			if udiff == 1:
+				ret[perm] = ret.get(perm,0) + coeff_dict[u]*mul_val
+		for perm, udiff, mul_val in new_perms_km1:
+			if udiff == 1:
+				ret[perm] = ret.get(perm,0) - coeff_dict[u]*mul_val
+	return ret
+
+def mult_poly(coeff_dict,poly):
+	if poly in var_x:
+		return single_variable(coeff_dict,var_x.index(poly))
+	elif isinstance(poly,Mul):
+		ret = coeff_dict
+		for a in poly.args:
+			ret = mult_poly(ret,a)
+		return ret
+	elif isinstance(poly,Pow):
+		base = poly.args[0]
+		exponent = int(poly.args[1])
+		ret = coeff_dict
+		for i in range(int(exponent)):
+			ret = mult_poly(ret,base)
+		return ret
+	elif isinstance(poly,Add):
+		ret = {}
+		for a in poly.args:
+			ret = add_perm_dict(ret,mult_poly(coeff_dict,a))
+		return ret
+	else:
+		ret = {}
+		for perm in coeff_dict:
+			ret[perm] = poly*coeff_dict[perm]
+		return ret
+		
 
 def nil_hecke(perm_dict,v,n,var2=var2,var3=var3):
+	if v == (1,2):
+		return perm_dict
 	th = strict_theta(inverse(v))
 	mu = permtrim(uncode(th))
 	vmu = permtrim(mulperm([*v],mu))
 	inv_vmu = inv(vmu)
 	inv_mu = inv(mu)
 	ret_dict = {}
 	vpaths = [([(vmu,0)],1)]
@@ -47,14 +97,16 @@
 		toget = tuple(vmu)
 		ret_dict = add_perm_dict({ep: vpathsums[ep].get(toget,0) for ep in vpathsums},ret_dict)
 	return ret_dict
 
 
 	
 def schubmult(perm_dict,v,var2=var2,var3=var3):
+	if v == (1,2):
+		return perm_dict
 	th = strict_theta(inverse(v))
 	mu = permtrim(uncode(th))
 	vmu = permtrim(mulperm([*v],mu))
 	inv_vmu = inv(vmu)
 	inv_mu = inv(mu)
 	ret_dict = {}
 	vpaths = [([(vmu,0)],1)]
@@ -185,15 +237,15 @@
 
 var2_t = tuple(var2.tolist())
 var3_t = tuple(var3.tolist())	
 
 def print_usage():
 	print("**** schubmult_q_yz ****")
 	print("Purpose: Compute Molev-Sagan coefficients of quantum double Schubert polynomials")
-	print("Usage: schubmult_q_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
+	print("Usage: schubmult_q_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. > <-mult poly_expression>")
 	print("       *** Computes products")
 	print("Alternative usage: schubmult_q_yz -nil-hecke n <-code> <--display-positive> perm")
 	print("       *** Computes nil-Hecke representation of quantum double Schubert polynomial, limiting to the group S_n")
 
 def main():
 	global var2
 	try:
@@ -206,26 +258,35 @@
 		display_positive = False
 		ascode = False
 		coprod = False
 		nilhecke = False
 		check = True
 		msg = False
 		just_nil = False
+		mult = False
 		
 		nil_N = 0
 		
+		mulstring = ""
+		
 		try:
 			for s in sys.argv[1:]:
 				if just_nil:
 					just_nil = False
 					nil_N = int(s)
 					continue
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
+				if mult:
+					mulstring += s
+					continue					
+				if s == "-mult":
+					mult = True
+					continue
 				if s == "-nocheck":
 					check = False
 					continue
 				if s == "--display-positive":
 					display_positive = True
 					continue
 				if s == "--optimizer-message":
@@ -239,19 +300,19 @@
 					print(f"Python version {sys.version}")
 					exit(0)
 				if s == "-code":
 					ascode = True
 					continue
 				if s == "--usage" or s == "--help":
 					print_usage()
-					exit(0)
+					exit(0)				
 				if s == "-":
 					perms += [curperm]
 					curperm = []
-					continue
+					continue				
 				curperm += [int(s)]
 		except Exception:
 			print_usage()
 			exit(1)
 				
 		perms += [curperm]
 		
@@ -264,19 +325,23 @@
 				perms[i] = tuple(permtrim([*perms[i]]))
 		
 		size = 0
 		L = len(perms)
 		
 		if nilhecke:
 			coeff_dict = nil_hecke({(1,2): 1},perms[0],nil_N)			
-			rep = ("y","x")
+			rep = ("y","x")		
 		else:
 			coeff_dict = {perms[0]: 1}
 			for perm in perms[1:]:
 				coeff_dict = schubmult(coeff_dict,perm)
+			if mult:
+				mul_exp = sympify(mulstring)
+				coeff_dict = mult_poly(coeff_dict,mul_exp)
+			rep = ("","")
 			rep = ("","")
 		
 		if pr:
 			if ascode:
 				width = max([len(str(trimcode(perm))) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
 			else:
 				width = max([len(str(perm)) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
@@ -297,37 +362,45 @@
 							q_dict = factor_out_q_keep_factored(val)
 							for q_part in q_dict:
 								#print(f"{q_part=} {q_dict[q_part]=}")
 								try:
 									val2 += q_part*int(q_dict[q_part])
 								except Exception:
 									try:
-										if len(perms) == 2 and q_part == 1:
+										if len(perms) == 2 and q_part == 1 and not mult:
 											u = permtrim([*perms[0]])
 											v = permtrim([*perms[1]])
 											val2 += posify(q_dict[q_part],tuple(u),tuple(v),perm,var2_t,var3_t,msg,False)
-										elif len(perms) == 2 and q_part in q_var2:
+										elif len(perms) == 2 and q_part in q_var2 and not mult:
 											i = q_var2.index(q_part)
 											u = permtrim([*perms[0]])
 											v = permtrim([*perms[1]])											
 											#print(f"{u=} {v=} {q_part=} {q_dict[q_part]=}")
 											if i<len(u) and i<len(v) and u[i-1]>u[i] and v[i-1]>v[i]:
 												u[i], u[i-1] = u[i-1], u[i]
 												v[i], v[i-1] = v[i-1], v[i]
 												#print(f"new {u=} {v=}")
 												val2 += q_part*posify(q_dict[q_part],tuple(permtrim(u)),tuple(permtrim(v)),perm,var2_t,var3_t,msg,False)
 										else:
 											val2 += q_part*compute_positive_rep(q_dict[q_part],var2_t,var3_t,msg,False)
 									except Exception as e:
-										print(f"error; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {coeff_dict.get(perm,0)=}")
-										print(f"Exception: {e}")
-										exit(1)
+										if mult:
+											print("warning; --display-positive is on but result is not positive",file=sys.stderr)
+											val2 = val
+											break
+										else:
+											print(f"error; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {coeff_dict.get(perm,0)=}")
+											print(f"Exception: {e}")
+											exit(1)
 							if check and expand(val - val2)!=0:
-								print(f"error: value not equal; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {coeff_dict.get(perm,0)=}")
-								exit(1)
+								if mult:
+									val2 = val
+								else:
+									print(f"error: value not equal; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {coeff_dict.get(perm,0)=}")
+									exit(1)
 							val = val2
 					if val!=0:
 						if ascode:
 							print(f"{str(trimcode(perm)):>{width}}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
 						else:
 							print(f"{str(perm):>{width}}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
 	except BrokenPipeError:
```

### Comparing `schubmult-1.3.7/schubmult/schubmult_yz/schubmult_yz.py` & `schubmult-1.3.8/schubmult/schubmult_yz/schubmult_yz.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,107 @@
 
 n = 100
 
 var = tuple(symarray('x',n).tolist())
 var2 = tuple(symarray('y',n).tolist())
 var3 = tuple(symarray('z',n).tolist())
 
+var_x = symarray("x",100).tolist()
+
+def single_variable(coeff_dict,varnum):
+	ret = {}
+	for u in coeff_dict:
+		if varnum -1 < len(u):
+			ret[u] = ret.get(u,0) + var2[u[varnum-1]]*coeff_dict[u]
+		else:
+			ret[u] = ret.get(u,0) + var2[varnum]*coeff_dict[u]
+		new_perms_k = elem_sym_perms(u,1,varnum)
+		new_perms_km1 = []
+		if varnum > 1:
+			new_perms_km1 = elem_sym_perms(u,1,varnum-1)
+		for perm, udiff in new_perms_k:
+			if udiff == 1:
+				ret[perm] = ret.get(perm,0) + coeff_dict[u]
+		for perm, udiff in new_perms_km1:
+			if udiff == 1:
+				ret[perm] = ret.get(perm,0) - coeff_dict[u]
+	return ret
+
+def single_variable_down(coeff_dict,varnum):
+	ret = {}
+	for u in coeff_dict:
+		if varnum -1 < len(u):
+			ret[u] = ret.get(u,0) + var2[u[varnum-1]]*coeff_dict[u]
+		else:
+			ret[u] = ret.get(u,0) + var2[varnum]*coeff_dict[u]
+		new_perms_k = elem_sym_perms_op(u,1,varnum)
+		new_perms_km1 = []
+		if varnum > 1:
+			new_perms_km1 = elem_sym_perms_op(u,1,varnum-1)
+		for perm, udiff in new_perms_k:
+			if udiff == 1:
+				ret[perm] = ret.get(perm,0) + coeff_dict[u]
+		for perm, udiff in new_perms_km1:
+			if udiff == 1:
+				ret[perm] = ret.get(perm,0) - coeff_dict[u]
+	return ret
+
+
+def mult_poly(coeff_dict,poly):
+	if poly in var_x:
+		return single_variable(coeff_dict,var_x.index(poly))
+	elif isinstance(poly,Mul):
+		ret = coeff_dict
+		for a in poly.args:
+			ret = mult_poly(ret,a)
+		return ret
+	elif isinstance(poly,Pow):
+		base = poly.args[0]
+		exponent = int(poly.args[1])
+		ret = coeff_dict
+		for i in range(int(exponent)):
+			ret = mult_poly(ret,base)
+		return ret
+	elif isinstance(poly,Add):
+		ret = {}
+		for a in poly.args:
+			ret = add_perm_dict(ret,mult_poly(coeff_dict,a))
+		return ret
+	else:
+		ret = {}
+		for perm in coeff_dict:
+			ret[perm] = poly*coeff_dict[perm]
+		return ret
+
+def mult_poly_down(coeff_dict,poly):
+	if poly in var_x:
+		return single_variable_down(coeff_dict,var_x.index(poly))
+	elif isinstance(poly,Mul):
+		ret = coeff_dict
+		for a in poly.args:
+			ret = mult_poly_down(ret,a)
+		return ret
+	elif isinstance(poly,Pow):
+		base = poly.args[0]
+		exponent = int(poly.args[1])
+		ret = coeff_dict
+		for i in range(int(exponent)):
+			ret = mult_poly_down(ret,base)
+		return ret
+	elif isinstance(poly,Add):
+		ret = {}
+		for a in poly.args:
+			ret = add_perm_dict(ret,mult_poly_down(coeff_dict,a))
+		return ret
+	else:
+		ret = {}
+		for perm in coeff_dict:
+			ret[perm] = poly*coeff_dict[perm]
+		return ret
+
 
 def forwardcoeff(u,v,perm,var2=var2,var3=var3):
 	th = theta(v)
 	muv = uncode(th)
 	vmun1 = mulperm(inverse([*v]),muv)
 	
 	w = mulperm([*perm],vmun1)	
@@ -156,14 +249,57 @@
 						for v2,vdiff,s in vpathdicts[index][v]:
 							newpathsums[up2][v2] = newpathsums[up2].get(v2,zero)+s*sumval*elem_sym_func(th[index],index+1,up,up2,v,v2,udiff,vdiff,var2,var3)
 			vpathsums = newpathsums
 		toget = tuple(vmu)
 		ret_dict = add_perm_dict({ep: vpathsums[ep].get(toget,0) for ep in vpathsums},ret_dict)
 	return ret_dict
 
+def schubmult_down(perm_dict,v,var2=var2,var3=var3):
+	vn1 = inverse(v)
+	th = theta(vn1)
+	if th[0]==0:
+		return perm_dict		
+	mu = permtrim(uncode(th))
+	vmu = permtrim(mulperm([*v],mu))
+	inv_vmu = inv(vmu)
+	inv_mu = inv(mu)
+	ret_dict = {}
+	vpaths = [([(vmu,0)],1)]
+	while th[-1] == 0:
+		th.pop()
+	thL = len(th)
+	vpathdicts = compute_vpathdicts(th,vmu,True)
+	for u,val in perm_dict.items():
+		inv_u = inv(u)
+		vpathsums = {u: {(1,2): val}}
+		for index in range(thL):			
+			mx_th = 0
+			for vp in vpathdicts[index]:
+				for v2,vdiff,s in vpathdicts[index][vp]:
+					if th[index]-vdiff > mx_th:
+						mx_th = th[index] - vdiff					
+			newpathsums = {}
+			for up in vpathsums:
+				inv_up = inv(up)
+				newperms = elem_sym_perms_op(up,mx_th,th[index])
+				for up2, udiff in newperms:
+					if up2 not in newpathsums:
+						newpathsums[up2]={}
+					for v in vpathdicts[index]:
+						sumval = vpathsums[up].get(v,zero)
+						if sumval == 0:
+							continue
+						for v2,vdiff,s in vpathdicts[index][v]:
+							newpathsums[up2][v2] = newpathsums[up2].get(v2,zero)+s*sumval*elem_sym_func(th[index],index+1,up2,up,v,v2,udiff,vdiff,var2,var3)
+			vpathsums = newpathsums
+		toget = tuple(vmu)
+		ret_dict = add_perm_dict({ep: vpathsums[ep].get(toget,0) for ep in vpathsums},ret_dict)
+	return ret_dict
+
+
 fvar = 0
 
 def poly_to_vec(poly,vec0=None):	
 	global dimen, monom_to_vec, base_vec
 	poly = expand(poly.xreplace({var3[1]: 0}))
 	
 	dc = poly.as_coefficients_dict()
@@ -1290,19 +1426,32 @@
 		
 		pr = True
 		display_positive = False
 		ascode = False
 		coprod = False
 		check = True
 		msg = False
+		mult = False
+		mulstring = ""
+		down = False
+		
 		try:
 			for s in sys.argv[1:]:
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
+				if mult:
+					mulstring += s
+					continue
+				if s == "-mult":
+					mult = True
+					continue
+				if s == "-down":
+					down = True
+					continue
 				if s == "-coprod":
 					coprod = True
 					continue
 				if s == "-nocheck":
 					check = False
 					continue
 				if s == "--display-positive":
@@ -1314,15 +1463,15 @@
 				if s == "--version":
 					print(f"Python version {sys.version}")
 					exit(0)
 				if s == "-code":
 					ascode = True
 					continue
 				if s == "--usage":
-					print("Usage: schubmult_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
+					print("Usage: schubmult_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. > <-mult poly_expression>")					
 					print("Alternative usage: schubmult_yz <-code> <--display-positive> -coprod perm - indexlist")
 					exit(0)
 				if s == "-":
 					perms += [curperm]
 					curperm = []
 					continue
 				curperm += [int(s)]
@@ -1458,30 +1607,43 @@
 			orig_perms = [*perms]
 			while len(perms) != size:
 				size = len(perms)
 				perms = split_perms(perms)
 			
 			coeff_dict = {perms[0]: 1}
 			check_coeff_dict = {perms[0]: 1}
-			for perm in orig_perms[1:]:
-				check_coeff_dict = schubmult(check_coeff_dict,perm)
-			if display_positive and len(perms)==2 and will_formula_work(perms[0],perms[1]):
+			
+			if down:
+				for perm in orig_perms[1:]:
+					check_coeff_dict = schubmult_down(check_coeff_dict,perm)
+				if mult:
+					mul_exp = sympify(mulstring)
+					check_coeff_dict = mult_poly_down(check_coeff_dict,mul_exp)				
+			else:
+				for perm in orig_perms[1:]:
+					check_coeff_dict = schubmult(check_coeff_dict,perm)
+				if mult:
+					mul_exp = sympify(mulstring)
+					check_coeff_dict = mult_poly(check_coeff_dict,mul_exp)
+			
+			
+			if display_positive and len(perms)==2 and will_formula_work(perms[0],perms[1]) and not mult and not down:
 				coeff_dict = {}
 				th = theta(perms[1])
 				muv = uncode(th)
 				muvn1v = mulperm(inverse(muv),perms[1])
 				coeff_dict2 = {perms[0]: 1}
 				coeff_dict2 = schubmult(coeff_dict2,muv)
 				for perm, val in coeff_dict2.items():					
 					w = mulperm([*perm],muvn1v)
 					if inv(w)+inv(muvn1v) == inv(perm):
 						coeff_dict[tuple(permtrim(w))] = val
 				posified = True
 				
-			if display_positive and len(perms)>2:
+			if display_positive and len(perms)>2 and not mult:
 				coeff_dict2 = dict(coeff_dict)
 				for perm in perms[1:]:					
 					coeff_dict3 = {}
 					for u in coeff_dict2:
 						coeff_dict4 = {u: 1}
 						coeff_dict4 = schubmult(coeff_dict4,perm)
 						for w in coeff_dict4:
@@ -1509,21 +1671,29 @@
 						try:
 							int(val)
 						except Exception:
 							notint = True
 						if notint and display_positive:
 							valu = val
 							try:
-								if len(perms) == 2 and not posified:
-									val = posify(val,perms[0],perms[1],perm,var2,var3,msg)							
-								elif not posified:								
+								if len(perms) == 2 and not posified and not mult:
+									if not down:
+										val = posify(val,perms[0],perms[1],perm,var2,var3,msg)							
+									else:
+										val = posify(val,perm,perms[1],perms[0],var2,var3,msg)
+								elif not posified and not mult:			
 									val = compute_positive_rep(val,var2,var3,msg)
-							except TypeError:
-								print(f"error; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {check_coeff_dict.get(perm,0)=}")
-								exit(1)
+								elif not posified:
+									val = compute_positive_rep(val,var2,var3,msg,do_pos_neg=False)
+							except Exception:
+								if mult:
+									print(f"warning; --display-positive is on but result is not positive",file=sys.stderr)
+								else:
+									print(f"error; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {check_coeff_dict.get(perm,0)=}")
+									exit(1)
 							if check and expand(val - check_coeff_dict.get(perm,0))!=0:
 								print(f"error; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {check_coeff_dict.get(perm,0)=}")
 								exit(1)
 						if val!=0:
 							if ascode:
 								print(f"{str(trimcode(perm)):>{width}}  {str(val).replace('**','^').replace('*',' ')}")	
 							else:
```

### Comparing `schubmult-1.3.7/schubmult.egg-info/PKG-INFO` & `schubmult-1.3.8/schubmult.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.7
+Version: 1.3.8
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.7/schubmult.egg-info/SOURCES.txt` & `schubmult-1.3.8/schubmult.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.7/setup.py` & `schubmult-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="schubmult",
-    version="1.3.7",
+    version="1.3.8",
     description="Computing Littlewood-Richardson coefficients of Schubert polynomials",
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url="https://github.com/matthematics/schubmult",
     author="Matt Samuel",
     author_email="schubmult@gmail.com",
     license="GNU",
```

