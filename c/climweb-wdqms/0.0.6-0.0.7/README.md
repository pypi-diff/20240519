# Comparing `tmp/climweb_wdqms-0.0.6.tar.gz` & `tmp/climweb_wdqms-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climweb_wdqms-0.0.6.tar", last modified: Fri May 17 22:11:15 2024, max compression
+gzip compressed data, was "climweb_wdqms-0.0.7.tar", last modified: Sun May 19 21:39:09 2024, max compression
```

## Comparing `climweb_wdqms-0.0.6.tar` & `climweb_wdqms-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.021694 climweb_wdqms-0.0.6/climweb_wdqms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.021694 climweb_wdqms-0.0.6/climweb_wdqms/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/climweb_wdqms/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/management/commands/fetch_transmissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/climweb_wdqms/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-17 22:11:15.000000 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-17 22:11:15.000000 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:11:15.000000 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 22:11:15.000000 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 22:11:15.000000 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:39:09.004724 climweb_wdqms-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-19 21:39:09.004724 climweb_wdqms-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:39:09.000724 climweb_wdqms-0.0.7/climweb_wdqms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:39:09.000724 climweb_wdqms-0.0.7/climweb_wdqms/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:39:09.000724 climweb_wdqms-0.0.7/climweb_wdqms/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/management/commands/wdqms_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:39:09.000724 climweb_wdqms-0.0.7/climweb_wdqms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/climweb_wdqms/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:39:09.004724 climweb_wdqms-0.0.7/climweb_wdqms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-19 21:39:08.000000 climweb_wdqms-0.0.7/climweb_wdqms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-19 21:39:08.000000 climweb_wdqms-0.0.7/climweb_wdqms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:39:08.000000 climweb_wdqms-0.0.7/climweb_wdqms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-19 21:39:08.000000 climweb_wdqms-0.0.7/climweb_wdqms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 21:39:08.000000 climweb_wdqms-0.0.7/climweb_wdqms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-19 21:39:04.000000 climweb_wdqms-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-19 21:39:09.004724 climweb_wdqms-0.0.7/setup.cfg
```

### Comparing `climweb_wdqms-0.0.6/climweb_wdqms/management/commands/fetch_transmissions.py` & `climweb_wdqms-0.0.7/climweb_wdqms/management/commands/wdqms_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,117 +72,128 @@
     current_date = datetime.strptime(start_date, "%Y-%m-%d")
     while current_date <= datetime.strptime(end_date, "%Y-%m-%d"):
         dates.append(current_date.strftime('%Y-%m-%d'))
         current_date += timedelta(days=1)
     return dates
 
 
-def ingest_transmission_rates(start_date, end_date,variables, periods, centers, country_code):
+def ingest_transmission_rates(start_date, end_date, variable, periods, centers, country_code):
     dates = generate_date_range(start_date, end_date)
     baseline = "OSCAR" 
 
-    for variable in variables:
-        print(f"INGEST: Ingesting {variable.upper()}...")
-        variable = variable.lower()
-        for date in dates:
-            for period in periods:
-                trans_rates = download_transmission_rate_csv(date, period, variable, centers, baseline, country_code)
+    print(f"INGEST: Ingesting {variable.upper()}...")
+    variable = variable.lower()
+
+    for date in dates:
+        for period in periods:
+            trans_rates = download_transmission_rate_csv(date, period, variable, centers, baseline, country_code)
+
+            print(f"INGEST: Starting data ingestion for {date}-{period}")
+
+            # Create or update stations
+            stations_to_create = []
+            for _, row in trans_rates.iterrows():
+                station_data = {
+                    'wigos_id': row['wigosid'],
+                    'name': row['name'],
+                    'geom':Point(row['longitude'], row['latitude']),
+                    'in_oscar':row['in OSCAR']
+                }
+                
+                stations_to_create.append(Station(**station_data))
 
-                print(f"INGEST: Starting data ingestion for {date}-{period}")
 
-                # Create or update stations
-                stations_to_create = []
-                for _, row in trans_rates.iterrows():
-                    station_data = {
-                        'wigos_id': row['wigosid'],
-                        'name': row['name'],
-                        'geom':Point(row['longitude'], row['latitude']),
-                        'in_oscar':row['in OSCAR']
-                    }
-                    
-                    stations_to_create.append(Station(**station_data))
+            # Bulk create new stations
+            Station.objects.bulk_create(stations_to_create, ignore_conflicts=True)
 
+            # Create or update transmissions
+            transmissions_to_create = []
+            for _, row in trans_rates.iterrows():
 
-                # Bulk create new stations
-                Station.objects.bulk_create(stations_to_create, ignore_conflicts=True)
+                if Transmission.objects.filter(station=row['wigosid'], variable=row['variable'], received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')).exists():
+                    transmission_data = {
+                        'received_rate':row['received_rate'],
+                        'received':row['#received'],
+                        'expected':row['#expected'],
+                    }
+                    Transmission.objects.filter(station=row['wigosid'], variable=row['variable'], received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')).update(**transmission_data)
 
-                # Create or update transmissions
-                transmissions_to_create = []
-                for _, row in trans_rates.iterrows():
-
-                    if Transmission.objects.filter(station=row['wigosid'], variable=row['variable'], received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')).exists():
-                        transmission_data = {
-                            'received_rate':row['received_rate'],
-                            'received':row['#received'],
-                            'expected':row['#expected'],
-                        }
-                        Transmission.objects.filter(station=row['wigosid'], variable=row['variable'], received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')).update(**transmission_data)
-
-                    else:
-                        station = Station.objects.get(wigos_id=row['wigosid'])
-                        transmissions_to_create.append(Transmission(
-                            station=station,
-                            variable=row['variable'],
-                            received_rate=row['received_rate'],
-                            received=row['#received'],
-                            expected=row['#expected'],
-                            received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')
-                        ))
+                else:
+                    station = Station.objects.get(wigos_id=row['wigosid'])
+                    transmissions_to_create.append(Transmission(
+                        station=station,
+                        variable=row['variable'],
+                        received_rate=row['received_rate'],
+                        received=row['#received'],
+                        expected=row['#expected'],
+                        received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')
+                    ))
 
-                # Bulk create new transmissions
-                Transmission.objects.bulk_create(transmissions_to_create, ignore_conflicts=True)
-                
-                print(f"INGEST: Completed ingestion for {date}-{period}")
+            # Bulk create new transmissions
+            Transmission.objects.bulk_create(transmissions_to_create, ignore_conflicts=True)
+            
+            print(f"INGEST: Completed ingestion for {date}-{period}")
 
 
 
 class Command(BaseCommand):
     help = ('Fetch Country level transmission rate from WDQMS')
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def add_arguments(self, parser):
         parser.add_argument('-s', '--start_date', type=str, help='Start date of transmission. format YYYY-MM-DD') 
         parser.add_argument('-e', '--end_date', type=str, help='End date of transmission. format YYYY-MM-DD') 
-        parser.add_argument('-var', '--variables', nargs='+', type=str, help='List of variables e.g pressure,temperature, humidity, meridional_wind, zonal_wind') 
+        parser.add_argument('-var', '--variable', type=str, help='Accepted variables are e.g pressure,temperature, humidity, meridional_wind, zonal_wind') 
         parser.add_argument('-p', '--periods', nargs='+', type=str, help='List of synoptic hours e.g 00, 06, 12, 18') 
         parser.add_argument('-c', '--centers', nargs='+', type=str, help='List of monitoring centers e.g DWD, ECMWF, JMA, NCEP') 
 
         # Arguments are not added here since they will be parsed manually
         return
 
     def handle(self, *args, **kwargs):
 
-        latest_date = Transmission.objects.values_list('received_date__date').order_by('received_date__date').last()
+        transmissions = Transmission.objects.all()
         yesterday = datetime.now().date() - timedelta(days=1)
 
-        if kwargs['start_date'] is not None:
-            # check first cli params
-            start_date = kwargs['start_date']
-        elif latest_date:
-            # check latest date in db 
-            start_date = latest_date[0].strftime("%Y-%m-%d")
-        else:
-            # use earliest date in wdqms. usually means the db is empty 
-            start_date = "2019-01-01" 
-
 
+        latest_date = None
         end_date = kwargs['end_date'] if kwargs['end_date'] is not None else yesterday.strftime("%Y-%m-%d")
         periods = kwargs['periods'] if kwargs['periods'] is not None else ["00", "06", "12", "18"]
         centers = kwargs['centers'] if kwargs['centers'] is not None else ["DWD", "ECMWF", "JMA", "NCEP"]
-        variables = kwargs['variables'] if kwargs['variables'] is not None else ['pressure', 'temperature', 'humidity', 'meridional_wind' , 'zonal_wind']
+        variable = kwargs['variable'] if kwargs['variable'] is not None else ['pressure', 'temperature', 'humidity', 'meridional_wind' , 'zonal_wind']
 
         variables_ls = ['pressure', 'temperature', 'humidity', 'meridional_wind' , 'zonal_wind']
         period_ls = ["00", "06", "12", "18"]
         center_ls = ["DWD", "ECMWF", "JMA", "NCEP"]
 
+
         # Regular expression to match YYYY-MM-DD format
         date_pattern = re.compile(r'^\d{4}-\d{2}-\d{2}$')
 
+        if variable is not None:
+            if variable not in variables_ls:
+                self.stderr.write(self.style.ERROR(f"Accepeted variables include pressure,temperature, humidity, meridional_wind, zonal_wind"))
+                return  # Exit the command
+            else:
+                # check latest date for variable
+                latest_date = transmissions.filter(variable=variable).values_list('received_date__date').order_by('received_date__date').last()
+
+     
+        if kwargs['start_date'] is not None:
+            # check first cli params
+            start_date = kwargs['start_date']
+        elif latest_date:
+            # check latest date in db 
+            start_date = latest_date[0].strftime("%Y-%m-%d")
+        else:
+            # use earliest date in wdqms. usually means the db is empty 
+            start_date = "2023-01-01" 
+
         # Parsing the arguments manually
         if start_date is not None:
             if not date_pattern.match(start_date):
                 self.stderr.write(self.style.ERROR(f"Invalid format for 'start_date'. Use YYYY-MM-DD format."))
                 return  # Exit the command
 
         if end_date is not None:  
@@ -191,42 +202,36 @@
                 return  # Exit the command
             
         if datetime.strptime(start_date, "%Y-%m-%d") > datetime.strptime(end_date, "%Y-%m-%d"):
             self.stderr.write(self.style.ERROR(f"'End date' cannot come earlier than 'Start date'"))
             return  # Exit the command
 
 
-        if variables is not None:
-            for variable in variables:
-                if variable not in variables_ls:
-                    self.stderr.write(self.style.ERROR(f"Allowed variables include pressure,temperature, humidity, meridional_wind, zonal_wind"))
-                    return  # Exit the command
-
-            # Split the value by comma and append to list_arg
+               # Split the value by comma and append to list_arg
         if periods is not None:
             for period in periods:
                 if period not in period_ls:
                     self.stderr.write(self.style.ERROR(f"'{period}' is not a valid option. Choices are 00 06 12 18"))
                     return  # Exit the command
             
         if centers is not None:
             for center in centers:
                 if center.upper() not in center_ls:
                     self.stderr.write(self.style.ERROR(f"'{center}' is not a valid option. Choices are DWD ECMWF JMA NCEP"))
                     return  # Exit the command
                 
             
 
-        if start_date is not None and end_date is not None and variables is not None and centers is not None and periods is not None:
+        if start_date is not None and end_date is not None and variable is not None and centers is not None and periods is not None:
             for country in Country.objects.all():
                 if Country.objects.count() > 0:
                     # loop through all countries in boundary manager for data fetching and ingestion
                     self.stdout.write(f"FETCH: Requesting data for {country.country.name}")
 
-                    ingest_transmission_rates(start_date, end_date, variables, periods, centers, country.country.alpha3)
+                    ingest_transmission_rates(start_date, end_date, variable, periods, centers, country.country.alpha3)
                 else:
                     self.stderr.write(self.style.ERROR(f"Please select atleast one country in admin boundary settings first"))
```

### Comparing `climweb_wdqms-0.0.6/climweb_wdqms/migrations/0001_initial.py` & `climweb_wdqms-0.0.7/climweb_wdqms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.6/climweb_wdqms/models.py` & `climweb_wdqms-0.0.7/climweb_wdqms/models.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.6/climweb_wdqms/serializers.py` & `climweb_wdqms-0.0.7/climweb_wdqms/serializers.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.6/climweb_wdqms/urls.py` & `climweb_wdqms-0.0.7/climweb_wdqms/urls.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.6/climweb_wdqms/views.py` & `climweb_wdqms-0.0.7/climweb_wdqms/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 class SynopTransmissionView(APIView):
     filter_backends = [DjangoFilterBackend]
     filterset_fields = ["received_date", "station", "variable"]
     permission_classes = [IsAuthenticated | ReadOnly]
 
     def get(self, request):
         
-        queryset = Transmission.objects.all()
+        queryset = Transmission.objects.filter(received_date__year__gte = 2023)
         supported_params = ['station', 'frequency', 'received_date', 'variable']
         query_params = request.query_params
         
         validate = validate_params(query_params, supported_params)
 
         if validate:
             return Response(validate, status=400)  # Return a 400 Bad Request response
@@ -122,15 +122,15 @@
         return Response(result)
 
 
 class MonthlyTransmissionView(APIView):
 
     def get(self, request):
 
-        queryset = Transmission.objects.all()
+        queryset = Transmission.objects.filter(received_date__year__gte = 2023)
         result = []
 
         latest_year =  queryset.values_list('received_date__year').order_by('received_date__year').last()
         supported_params = ['station', 'year', 'variable']
 
         validate = validate_params(request.query_params, supported_params)
 
@@ -177,15 +177,15 @@
         return Response(result)
 
 
 class YearlyTransmissionView(APIView):
 
     def get(self, request):
 
-        queryset = Transmission.objects.all()
+        queryset = Transmission.objects.filter(received_date__year__gte = 2023)
         result = []
 
         supported_params = ['station', 'variable']
 
         validate = validate_params(request.query_params, supported_params)
 
         if validate:
```

### Comparing `climweb_wdqms-0.0.6/climweb_wdqms.egg-info/SOURCES.txt` & `climweb_wdqms-0.0.7/climweb_wdqms.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 MANIFEST.in
+README.md
 pyproject.toml
 setup.cfg
 climweb_wdqms/__init__.py
 climweb_wdqms/admin.py
 climweb_wdqms/apps.py
 climweb_wdqms/models.py
 climweb_wdqms/serializers.py
@@ -12,10 +13,10 @@
 climweb_wdqms.egg-info/PKG-INFO
 climweb_wdqms.egg-info/SOURCES.txt
 climweb_wdqms.egg-info/dependency_links.txt
 climweb_wdqms.egg-info/requires.txt
 climweb_wdqms.egg-info/top_level.txt
 climweb_wdqms/management/__init__.py
 climweb_wdqms/management/commands/__init__.py
-climweb_wdqms/management/commands/fetch_transmissions.py
+climweb_wdqms/management/commands/wdqms_stats.py
 climweb_wdqms/migrations/0001_initial.py
 climweb_wdqms/migrations/__init__.py
```

### Comparing `climweb_wdqms-0.0.6/setup.cfg` & `climweb_wdqms-0.0.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = climweb-wdqms
-version = 0.0.6
+version = 0.0.7
 description = National level WDQMS Summary tool
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/climweb-wdqms
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
```

