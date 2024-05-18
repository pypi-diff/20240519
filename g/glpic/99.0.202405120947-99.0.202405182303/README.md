# Comparing `tmp/glpic-99.0.202405120947.tar.gz` & `tmp/glpic-99.0.202405182303.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202405120947.tar", last modified: Sun May 12 09:47:53 2024, max compression
+gzip compressed data, was "glpic-99.0.202405182303.tar", last modified: Sat May 18 23:03:01 2024, max compression
```

## Comparing `glpic-99.0.202405120947.tar` & `glpic-99.0.202405182303.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:47:53.627880 glpic-99.0.202405120947/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-12 09:47:53.627880 glpic-99.0.202405120947/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-12 09:47:40.000000 glpic-99.0.202405120947/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:47:53.623880 glpic-99.0.202405120947/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10963 2024-05-12 09:47:40.000000 glpic-99.0.202405120947/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-12 09:47:40.000000 glpic-99.0.202405120947/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:47:53.627880 glpic-99.0.202405120947/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-12 09:47:53.000000 glpic-99.0.202405120947/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-12 09:47:53.000000 glpic-99.0.202405120947/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:47:53.000000 glpic-99.0.202405120947/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-12 09:47:53.000000 glpic-99.0.202405120947/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:47:53.000000 glpic-99.0.202405120947/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-12 09:47:53.000000 glpic-99.0.202405120947/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 09:47:53.000000 glpic-99.0.202405120947/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 09:47:53.627880 glpic-99.0.202405120947/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-12 09:47:53.000000 glpic-99.0.202405120947/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:03:01.810023 glpic-99.0.202405182303/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-18 23:03:01.810023 glpic-99.0.202405182303/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-18 23:02:51.000000 glpic-99.0.202405182303/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:03:01.810023 glpic-99.0.202405182303/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    11545 2024-05-18 23:02:51.000000 glpic-99.0.202405182303/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-18 23:02:51.000000 glpic-99.0.202405182303/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:03:01.810023 glpic-99.0.202405182303/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-18 23:03:01.000000 glpic-99.0.202405182303/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-18 23:03:01.000000 glpic-99.0.202405182303/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 23:03:01.000000 glpic-99.0.202405182303/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 23:03:01.000000 glpic-99.0.202405182303/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 23:03:01.000000 glpic-99.0.202405182303/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-18 23:03:01.000000 glpic-99.0.202405182303/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 23:03:01.000000 glpic-99.0.202405182303/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 23:03:01.810023 glpic-99.0.202405182303/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-18 23:03:01.000000 glpic-99.0.202405182303/setup.py
```

### Comparing `glpic-99.0.202405120947/README.md` & `glpic-99.0.202405182303/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405120947/glpic/__init__.py` & `glpic-99.0.202405182303/glpic/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -195,14 +195,27 @@
             if memory is not None and int(float(current_memory)) < int(memory):
                 continue
             results.append(computer)
             if number is not None and len(results) >= int(number):
                 break
         return results
 
+    def update_computer(self, computer, overrides):
+        info = self.info_computer({'computer': computer, 'uid': True})
+        if not info:
+            error(f"Computer {computer} not found")
+            return
+        computer_id = info[0]['Computer.id']
+        data = {'input': overrides}
+        if self.debug:
+            base_curl = curl_base(self.headers)
+            msg = f"{base_curl} -X POST -Lk {self.base_url}/Computer/{computer_id} -d '{json.dumps(data)}'"
+            print(msg)
+        return _put(f'{self.base_url}/Computer/{computer_id}', self.headers, data)
+
     def create_reservation(self, computer, overrides):
         overrides['begin'] = parse(str(datetime.now())).strftime('%Y-%m-%d %H:%M:%S')
         if 'end' not in overrides:
             overrides['end'] = date.today() + timedelta(days=30)
         user = overrides.get('user', self.user)
         if 'users_id' not in overrides:
             user_id = self.get_user(user)['id']
```

### Comparing `glpic-99.0.202405120947/glpic/cli.py` & `glpic-99.0.202405182303/glpic/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -108,14 +108,21 @@
         bmc = computer['Computer.PluginFieldsComputerbmcaddre.bmcaddressfield']
         model = computer['Computer.ComputerModel.name']
         entry = [name, group, serial, model, memory, bmc]
         computerstable.add_row(entry)
     print(computerstable)
 
 
+def update_computer(args):
+    glpic = Glpic(args.url, args.user, args.token, args.debug)
+    for computer in args.computers:
+        info(f"Updating computer {computer}")
+        glpic.update_computer(computer, overrides=handle_parameters(args.param))
+
+
 def list_reservations(args):
     glpic = Glpic(args.url, args.user, args.token, args.debug)
     reservationstable = PrettyTable(["Id", "Item", "Begin", "End", "Comment"])
     for reservation in glpic.list_reservations(overrides=handle_parameters(args.param)):
         _id, begin, end, comment = reservation['id'], reservation['begin'], reservation['end'], reservation['comment']
         comment = fill(comment, width=100)
         reservation_id = reservation['reservationitems_id']
@@ -207,14 +214,24 @@
     list_subparsers.add_parser('reservation', parents=[reservationlist_parser], description=reservationlist_desc,
                                help=reservationlist_desc, aliases=['reservations'])
 
     update_desc = 'Update Object'
     update_parser = subparsers.add_parser('update', description=update_desc, help=update_desc)
     update_subparsers = update_parser.add_subparsers(metavar='', dest='subcommand_update')
 
+    computerupdate_desc = 'Update Computer'
+    computerupdate_epilog = None
+    computerupdate_parser = update_subparsers.add_parser('computer', description=computerupdate_desc,
+                                                         help=computerupdate_desc,
+                                                         epilog=computerupdate_epilog, formatter_class=rawhelp,
+                                                         aliases=['computers'])
+    computerupdate_parser.add_argument('-P', '--param', action='append', help=PARAMHELP, metavar='PARAM')
+    computerupdate_parser.add_argument('computers', metavar='RESERVATIONS', nargs='*')
+    computerupdate_parser.set_defaults(func=update_computer)
+
     reservationupdate_desc = 'Update Reservation'
     reservationupdate_epilog = None
     reservationupdate_parser = update_subparsers.add_parser('reservation', description=reservationupdate_desc,
                                                             help=reservationupdate_desc,
                                                             epilog=reservationupdate_epilog, formatter_class=rawhelp,
                                                             aliases=['reservations'])
     reservationupdate_parser.add_argument('-P', '--param', action='append', help=PARAMHELP, metavar='PARAM')
```

### Comparing `glpic-99.0.202405120947/setup.py` & `glpic-99.0.202405182303/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202405120947',
+    version='99.0.202405182303',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

