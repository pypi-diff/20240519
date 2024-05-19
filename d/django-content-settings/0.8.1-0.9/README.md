# Comparing `tmp/django_content_settings-0.8.1.tar.gz` & `tmp/django_content_settings-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_content_settings-0.8.1.tar", max compression
+gzip compressed data, was "django_content_settings-0.9.tar", max compression
```

## Comparing `django_content_settings-0.8.1.tar` & `django_content_settings-0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     3010 2024-01-16 13:23:37.001345 django_content_settings-0.8.1/README_SHORT.md
--rw-r--r--   0        0        0    16974 2024-02-06 21:59:29.467075 django_content_settings-0.8.1/content_settings/admin.py
--rw-r--r--   0        0        0      294 2024-01-02 19:51:20.909422 django_content_settings-0.8.1/content_settings/apps.py
--rw-r--r--   0        0        0     9028 2024-01-26 14:55:00.837193 django_content_settings-0.8.1/content_settings/caching.py
--rw-r--r--   0        0        0     7896 2024-02-06 22:03:29.275922 django_content_settings-0.8.1/content_settings/conf.py
--rw-r--r--   0        0        0     3672 2024-01-26 14:56:14.321390 django_content_settings-0.8.1/content_settings/context_managers.py
--rw-r--r--   0        0        0      145 2024-01-02 19:51:20.912036 django_content_settings-0.8.1/content_settings/context_processors.py
--rw-r--r--   0        0        0      812 2024-01-02 19:51:20.912696 django_content_settings-0.8.1/content_settings/management/commands/static_content_set_new_values.py
--rw-r--r--   0        0        0     3945 2024-01-13 17:53:06.194497 django_content_settings-0.8.1/content_settings/migrations/0001_initial.py
--rw-r--r--   0        0        0     2656 2024-01-19 10:06:23.697155 django_content_settings-0.8.1/content_settings/migrations/0002_user_defined.py
--rw-r--r--   0        0        0        0 2024-01-02 19:51:20.913266 django_content_settings-0.8.1/content_settings/migrations/__init__.py
--rw-r--r--   0        0        0     4048 2024-01-28 09:01:26.188228 django_content_settings-0.8.1/content_settings/models.py
--rw-r--r--   0        0        0      645 2024-01-03 18:20:13.490442 django_content_settings-0.8.1/content_settings/permissions.py
--rw-r--r--   0        0        0     1845 2024-01-28 20:40:47.332355 django_content_settings-0.8.1/content_settings/settings.py
--rw-r--r--   0        0        0     3315 2024-01-31 11:40:37.857955 django_content_settings-0.8.1/content_settings/signals.py
--rw-r--r--   0        0        0      134 2024-01-28 20:40:47.256850 django_content_settings-0.8.1/content_settings/tags.py
--rw-r--r--   0        0        0     2874 2024-02-06 21:57:27.938551 django_content_settings-0.8.1/content_settings/templates/admin/content_settings/contentsetting/change_form.html
--rw-r--r--   0        0        0     6495 2024-02-06 21:57:07.008846 django_content_settings-0.8.1/content_settings/templates/admin/content_settings/contentsetting/change_list.html
--rw-r--r--   0        0        0      223 2024-01-02 19:51:20.918230 django_content_settings-0.8.1/content_settings/templates/admin/content_settings/contentsetting/context_tags.html
--rw-r--r--   0        0        0     1897 2024-01-18 19:45:58.439725 django_content_settings-0.8.1/content_settings/templates/admin/content_settings/contentsetting/object_history.html
--rw-r--r--   0        0        0        0 2024-01-02 19:51:20.918791 django_content_settings-0.8.1/content_settings/templatetags/__init__.py
--rw-r--r--   0        0        0      420 2024-01-02 19:51:20.919284 django_content_settings-0.8.1/content_settings/templatetags/content_settings_admin.py
--rw-r--r--   0        0        0      366 2024-01-02 19:51:20.920665 django_content_settings-0.8.1/content_settings/templatetags/content_settings_extras.py
--rw-r--r--   0        0        0      732 2024-01-30 11:18:42.799899 django_content_settings-0.8.1/content_settings/tests/test_all_settings.py
--rw-r--r--   0        0        0      243 2024-01-21 19:56:31.489111 django_content_settings-0.8.1/content_settings/types/__init__.py
--rw-r--r--   0        0        0    10266 2024-02-09 15:18:34.558436 django_content_settings-0.8.1/content_settings/types/array.py
--rw-r--r--   0        0        0    11390 2024-02-06 21:05:09.937400 django_content_settings-0.8.1/content_settings/types/basic.py
--rw-r--r--   0        0        0     2856 2024-01-30 12:16:59.143059 django_content_settings-0.8.1/content_settings/types/datetime.py
--rw-r--r--   0        0        0     5901 2024-02-08 15:37:14.964107 django_content_settings-0.8.1/content_settings/types/each.py
--rw-r--r--   0        0        0     1336 2024-01-07 22:21:58.186314 django_content_settings-0.8.1/content_settings/types/lazy.py
--rw-r--r--   0        0        0     3666 2024-02-06 18:06:43.726880 django_content_settings-0.8.1/content_settings/types/markup.py
--rw-r--r--   0        0        0     7397 2024-02-06 21:27:17.235105 django_content_settings-0.8.1/content_settings/types/mixins.py
--rw-r--r--   0        0        0     6867 2024-02-06 21:17:47.879456 django_content_settings-0.8.1/content_settings/types/template.py
--rw-r--r--   0        0        0      810 2024-01-06 12:08:35.122870 django_content_settings-0.8.1/content_settings/types/validators.py
--rw-r--r--   0        0        0      365 2024-01-07 22:32:02.247854 django_content_settings-0.8.1/content_settings/urls.py
--rw-r--r--   0        0        0     2400 2024-01-28 22:16:18.819797 django_content_settings-0.8.1/content_settings/views.py
--rw-r--r--   0        0        0     1376 2024-02-09 15:22:40.485540 django_content_settings-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4107 1970-01-01 00:00:00.000000 django_content_settings-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     3010 2024-01-16 13:23:37.001345 django_content_settings-0.9/README_SHORT.md
+-rw-r--r--   0        0        0    17696 2024-02-11 12:39:27.071948 django_content_settings-0.9/content_settings/admin.py
+-rw-r--r--   0        0        0      294 2024-01-02 19:51:20.909422 django_content_settings-0.9/content_settings/apps.py
+-rw-r--r--   0        0        0     9028 2024-02-09 16:45:28.990251 django_content_settings-0.9/content_settings/caching.py
+-rw-r--r--   0        0        0     7830 2024-02-11 11:52:41.313623 django_content_settings-0.9/content_settings/conf.py
+-rw-r--r--   0        0        0     3672 2024-01-26 14:56:14.321390 django_content_settings-0.9/content_settings/context_managers.py
+-rw-r--r--   0        0        0      145 2024-01-02 19:51:20.912036 django_content_settings-0.9/content_settings/context_processors.py
+-rw-r--r--   0        0        0      812 2024-01-02 19:51:20.912696 django_content_settings-0.9/content_settings/management/commands/static_content_set_new_values.py
+-rw-r--r--   0        0        0     3945 2024-01-13 17:53:06.194497 django_content_settings-0.9/content_settings/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2656 2024-01-19 10:06:23.697155 django_content_settings-0.9/content_settings/migrations/0002_user_defined.py
+-rw-r--r--   0        0        0        0 2024-01-02 19:51:20.913266 django_content_settings-0.9/content_settings/migrations/__init__.py
+-rw-r--r--   0        0        0     4048 2024-01-28 09:01:26.188228 django_content_settings-0.9/content_settings/models.py
+-rw-r--r--   0        0        0      645 2024-01-03 18:20:13.490442 django_content_settings-0.9/content_settings/permissions.py
+-rw-r--r--   0        0        0     1845 2024-01-28 20:40:47.332355 django_content_settings-0.9/content_settings/settings.py
+-rw-r--r--   0        0        0     3405 2024-02-11 12:12:48.335222 django_content_settings-0.9/content_settings/signals.py
+-rw-r--r--   0        0        0      134 2024-01-28 20:40:47.256850 django_content_settings-0.9/content_settings/tags.py
+-rw-r--r--   0        0        0     2944 2024-02-09 21:30:12.331322 django_content_settings-0.9/content_settings/templates/admin/content_settings/contentsetting/change_form.html
+-rw-r--r--   0        0        0     6549 2024-02-09 21:29:22.505452 django_content_settings-0.9/content_settings/templates/admin/content_settings/contentsetting/change_list.html
+-rw-r--r--   0        0        0      223 2024-01-02 19:51:20.918230 django_content_settings-0.9/content_settings/templates/admin/content_settings/contentsetting/context_tags.html
+-rw-r--r--   0        0        0     1897 2024-01-18 19:45:58.439725 django_content_settings-0.9/content_settings/templates/admin/content_settings/contentsetting/object_history.html
+-rw-r--r--   0        0        0        0 2024-01-02 19:51:20.918791 django_content_settings-0.9/content_settings/templatetags/__init__.py
+-rw-r--r--   0        0        0      420 2024-01-02 19:51:20.919284 django_content_settings-0.9/content_settings/templatetags/content_settings_admin.py
+-rw-r--r--   0        0        0      535 2024-02-11 12:39:26.304578 django_content_settings-0.9/content_settings/templatetags/content_settings_extras.py
+-rw-r--r--   0        0        0      732 2024-01-30 11:18:42.799899 django_content_settings-0.9/content_settings/tests/test_all_settings.py
+-rw-r--r--   0        0        0      340 2024-02-10 20:24:04.834510 django_content_settings-0.9/content_settings/types/__init__.py
+-rw-r--r--   0        0        0    10266 2024-02-09 15:18:34.558436 django_content_settings-0.9/content_settings/types/array.py
+-rw-r--r--   0        0        0    11283 2024-02-10 20:24:16.350897 django_content_settings-0.9/content_settings/types/basic.py
+-rw-r--r--   0        0        0     2882 2024-02-09 21:13:28.232955 django_content_settings-0.9/content_settings/types/datetime.py
+-rw-r--r--   0        0        0     8533 2024-02-11 12:39:26.779998 django_content_settings-0.9/content_settings/types/each.py
+-rw-r--r--   0        0        0     3583 2024-02-09 19:40:59.022296 django_content_settings-0.9/content_settings/types/lazy.py
+-rw-r--r--   0        0        0     3717 2024-02-09 21:16:34.754024 django_content_settings-0.9/content_settings/types/markup.py
+-rw-r--r--   0        0        0     7330 2024-02-11 12:39:26.771358 django_content_settings-0.9/content_settings/types/mixins.py
+-rw-r--r--   0        0        0     7465 2024-02-11 12:39:26.768489 django_content_settings-0.9/content_settings/types/template.py
+-rw-r--r--   0        0        0      810 2024-01-06 12:08:35.122870 django_content_settings-0.9/content_settings/types/validators.py
+-rw-r--r--   0        0        0      365 2024-01-07 22:32:02.247854 django_content_settings-0.9/content_settings/urls.py
+-rw-r--r--   0        0        0     2400 2024-02-11 11:54:43.621296 django_content_settings-0.9/content_settings/views.py
+-rw-r--r--   0        0        0     1374 2024-02-11 12:41:55.962819 django_content_settings-0.9/pyproject.toml
+-rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 django_content_settings-0.9/PKG-INFO
```

### Comparing `django_content_settings-0.8.1/README_SHORT.md` & `django_content_settings-0.9/README_SHORT.md`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/admin.py` & `django_content_settings-0.9/content_settings/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,35 +92,39 @@
             combine = Q()
             for tag in tags:
                 if tag in USER_TAGS:
                     continue
                 combine &= Q(tags__iregex=rf"(^|\n){tag}($|\n)")
 
             q = q.filter(combine)
-
         # This is terrable
         # But I don't know how to do it better
         # I need to filter out the names user don't have permissions to see
 
         names = list(q.values_list("name", flat=True))
         return q.filter(
             ~Q(
                 name__in=[
-                    name for name in names if not get_type_by_name(name).can_view(user)
+                    name
+                    for name in names
+                    if not get_type_by_name(name)
+                    or get_type_by_name(name).constant
+                    or not get_type_by_name(name).can_view(user)
                 ]
             )
         )
 
 
 class ContentSettinForm(ModelForm):
     def __init__(self, *args, **kwargs):
         super(ContentSettinForm, self).__init__(*args, **kwargs)
         if self.instance.name:
             cs_type = get_type_by_name(self.instance.name)
-            self.fields["value"] = cs_type.field
+            if cs_type:
+                self.fields["value"] = cs_type.field
         self.fields["value"].strip = False
 
         if "user_defined_type" in self.fields:
             self.fields["user_defined_type"].widget = forms.Select(
                 choices=[(v[0], v[2]) for v in USER_DEFINED_TYPES]
             )
 
@@ -191,18 +195,25 @@
 
     def context_tags(self, request):
         from .conf import get_type_by_name
 
         extra_context = {}
         selected_tags = get_selected_tags_from_params(request.GET)
 
+        if "q" in request.GET:
+            init_q = "?q=" + urllib.parse.quote(request.GET["q"]) + "&"
+        else:
+            init_q = "?"
+
         def q_tags(tags):
             if not tags:
-                return "?"
-            return "?" + TAGS_PARAM + "=" + urllib.parse.quote(TAGS_SPLITER.join(tags))
+                return init_q
+            return (
+                init_q + TAGS_PARAM + "=" + urllib.parse.quote(TAGS_SPLITER.join(tags))
+            )
 
         def q_add_tag(tag):
             return q_tags(selected_tags | set([tag]))
 
         def q_remove_tag(tag):
             return q_tags(selected_tags - set([tag]))
 
@@ -212,16 +223,18 @@
                 "url": q_remove_tag(tag),
             }
             for tag in sorted(selected_tags)
         ]
 
         tags_stat = defaultdict(int)
         user_settings = UserTagSetting.get_user_settings(request.user)
-        for cs in ContentSetting.objects.all():
-            if not get_type_by_name(cs.name).can_view(request.user):
+
+        for cs in self.get_changelist_instance(request).get_queryset(request):
+            cs_type = get_type_by_name(cs.name)
+            if not cs_type or not cs_type.can_view(request.user) or cs_type.constant:
                 continue
             val_tags = cs.tags_set | user_settings[cs.name]
             if selected_tags and (not val_tags or selected_tags - val_tags):
                 continue
 
             for tag in val_tags - selected_tags:
                 tags_stat[tag] += 1
@@ -251,15 +264,17 @@
             self.context_tags(request),
         )
 
     def change_view(self, request, object_id, *args, **kwargs):
         from .conf import get_type_by_name
 
         cs = ContentSetting.objects.filter(pk=object_id).first()
-        if cs and not get_type_by_name(cs.name).can_view(request.user):
+
+        cs_type = get_type_by_name(cs.name)
+        if cs and not cs_type or not cs_type.can_view(request.user) or cs_type.constant:
             raise PermissionDenied
 
         return super().change_view(request, object_id, *args, **kwargs)
 
     def history_view(self, request, object_id, extra_context=None):
         from .conf import get_type_by_name
 
@@ -267,17 +282,21 @@
         model = self.model
         obj = self.get_object(request, unquote(object_id))
         if obj is None:
             return self._get_obj_does_not_exist_redirect(
                 request, model._meta, object_id
             )
 
-        if not self.has_view_or_change_permission(request, obj) or not get_type_by_name(
-            obj.name
-        ).can_view_history(request.user):
+        cs_type = get_type_by_name(obj.name)
+        if (
+            not self.has_view_or_change_permission(request, obj)
+            or not cs_type
+            or not cs_type.can_view_history(request.user)
+            or cs_type.constant
+        ):
             raise PermissionDenied
 
         opts = model._meta
         app_label = opts.app_label
 
         context = {
             **self.admin_site.each_context(request),
@@ -317,15 +336,20 @@
             return True
         return user_able_to_update(request.user, obj.name)
 
     def setting_help(self, obj):
         cs_type = get_type_by_name(obj.name)
         if cs_type is None or cs_type.constant:
             return "(the setting is not using)"
-        return mark_safe(obj.help) + html_classes(obj.name)
+
+        if obj.user_defined_type:
+            help = cs_type.get_help()
+        else:
+            help = obj.help
+        return mark_safe(help + html_classes(obj.name))
 
     setting_help.short_description = "Help"
 
     def setting_tags(self, obj):
         cs_type = get_type_by_name(obj.name)
         if cs_type is None or cs_type.constant:
             return "(the setting is not using)"
```

### Comparing `django_content_settings-0.8.1/content_settings/caching.py` & `django_content_settings-0.9/content_settings/caching.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/conf.py` & `django_content_settings-0.9/content_settings/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,26 +86,27 @@
     try:
         content_settings = import_module(app + ".content_settings")
     except ImportError as e:
         if e.name != app + ".content_settings":
             raise
         continue
     for attr in dir(content_settings):
+        if not attr.isupper():
+            continue
+
         val = getattr(content_settings, attr)
+
         if not isinstance(val, BaseSetting):
             continue
 
         assert attr not in ALL, "Content Setting {} defined twice".format(attr)
 
         if attr in ALL and not ALL[attr].user_defined_slug:
             raise AssertionError("Overwriting content setting {}".format(attr))
 
-        if not attr.isupper():
-            raise AssertionError("content setting {} should be uppercase".format(attr))
-
         assert (
             not val.user_defined_slug
         ), "Do not set user_defined_slug in content_settings.py"
 
         ALL[attr] = val
```

### Comparing `django_content_settings-0.8.1/content_settings/context_managers.py` & `django_content_settings-0.9/content_settings/context_managers.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/management/commands/static_content_set_new_values.py` & `django_content_settings-0.9/content_settings/management/commands/static_content_set_new_values.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/migrations/0001_initial.py` & `django_content_settings-0.9/content_settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/migrations/0002_user_defined.py` & `django_content_settings-0.9/content_settings/migrations/0002_user_defined.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/models.py` & `django_content_settings-0.9/content_settings/models.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/permissions.py` & `django_content_settings-0.9/content_settings/permissions.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/settings.py` & `django_content_settings-0.9/content_settings/settings.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/signals.py` & `django_content_settings-0.9/content_settings/signals.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         from .conf import USER_DEFINED_TYPES_INITIAL
 
         if instance.user_defined_type not in USER_DEFINED_TYPES_INITIAL:
             return
         instance.version = USER_DEFINED_TYPES_INITIAL[
             instance.user_defined_type
         ].version
+        if instance.tags:
+            instance.tags = instance.tags.replace("\r\n", "\n")
 
 
 @receiver(post_delete, sender=ContentSetting)
 def create_history_settings_delete(sender, instance, **kwargs):
     HistoryContentSetting.objects.create(
         name=instance.name,
         value=instance.value,
```

### Comparing `django_content_settings-0.8.1/content_settings/templates/admin/content_settings/contentsetting/change_form.html` & `django_content_settings-0.9/content_settings/templates/admin/content_settings/contentsetting/change_form.html`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,18 @@
         text-decoration: underline;
         cursor: pointer;
     }
     .field-setting_help a {
         color: var(--link-fg);
         cursor: pointer;
     }
+    .field-py_data pre {
+        margin: 0;
+        padding: 0;
+    }
     div.subitem {
         margin-left: 10px;
     }
     </style>
 <script>
     (function($) {
         const objName = "{{original.name}}";
```

### Comparing `django_content_settings-0.8.1/content_settings/templates/admin/content_settings/contentsetting/change_list.html` & `django_content_settings-0.9/content_settings/templates/admin/content_settings/contentsetting/change_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,18 @@
     font-size: 18px;
 }
 .value_preview a{
     color: var(--link-fg);
     text-decoration: underline;
     cursor: pointer;
 }
+.value_preview pre {
+    margin: 0;
+    padding: 0;
+}
 .field-setting_help a {
     color: var(--link-fg);
     cursor: pointer;
 }
 div.subitem {
     margin-left: 10px;
 }
```

### Comparing `django_content_settings-0.8.1/content_settings/templates/admin/content_settings/contentsetting/object_history.html` & `django_content_settings-0.9/content_settings/templates/admin/content_settings/contentsetting/object_history.html`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/tests/test_all_settings.py` & `django_content_settings-0.9/content_settings/tests/test_all_settings.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/types/array.py` & `django_content_settings-0.9/content_settings/types/array.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/types/basic.py` & `django_content_settings-0.9/content_settings/types/basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     PREVIEW_ALL,
     PREVIEW_HTML,
     PREVIEW_TEXT,
     PREVIEW_PYTHON,
     PREVIEW_NONE,
     required,
     optional,
+    pre,
 )
 from content_settings.types.mixins import HTMLMixin
 from content_settings.permissions import none, staff
 
 
 class BaseSetting:
     pass
@@ -40,15 +41,14 @@
     - update_permission (Callable): Optional permission required to update the setting.
     - help_format (Optional[str]): Optional format string for the help text for the format (align to the type).
     - help (Optional[str]): Optional help text for the setting.
     - value_required (bool): Whether a value is required for the setting.
     - version (str): The version of the setting (using for caching).
     - tags (Optional[Iterable[str]]): Optional tags associated with the setting.
     - validators (Tuple[Callable]): Validators to apply to the setting value.
-    - empty_is_none (bool): Whether an empty value should be treated as None.
     - admin_preview_as (str): The format to use for the admin preview.
     - suffixes (Tuple[str]): Suffixes that can be appended to the setting value.
     - user_defined_slug (str): it contains a slug from db If the setting is defined in DB only (should not be set in content_settings)
     - overwrite_user_defined (bool): Whether the setting can overwrite a user defined setting.
     - default (str): The default value for the setting.
     """
 
@@ -62,15 +62,14 @@
     view_history_permission: Optional[Callable] = None
     help_format: str = "string"
     help: str = ""
     value_required: bool = False
     version: str = ""
     tags: Optional[Iterable[str]] = None
     validators: Tuple[Callable] = ()
-    empty_is_none: bool = False
     admin_preview_as: str = PREVIEW_NONE
     suffixes: Tuple[str] = ()
     user_defined_slug: Optional[str] = None
     overwrite_user_defined: bool = False
     default: Union[str, required, optional] = ""
     json_encoder = DjangoJSONEncoder
 
@@ -189,15 +188,15 @@
 
     def get_content_tags(self, value: str) -> Set[str]:
         from content_settings.conf import gen_tags
 
         return gen_tags(self, value)
 
     def get_validators(self) -> Tuple[Callable]:
-        return self.validators + tuple(self.cls_field.default_validators)
+        return tuple(self.validators) + tuple(self.cls_field.default_validators)
 
     def get_field(self) -> forms.Field:
         return self.cls_field(
             widget=self.get_widget(),
             validators=(self.validate_value,),
             required=self.value_required,
         )
@@ -208,25 +207,25 @@
         else:
             return self.widget
 
     def validate_raw_value(self, value: str) -> None:
         pass
 
     def validate_value(self, value: str) -> Any:
+        if self.value_required and not value:
+            raise ValidationError("This field is required")
         self.validate_raw_value(value)
         val = self.to_python(value)
         self.validate(val)
 
     def validate(self, value):
         for validator in self.get_validators():
             validator(value)
 
     def to_python(self, value: str) -> Any:
-        if self.empty_is_none and value.strip() == "":
-            return None
         return self.field.to_python(value)
 
     def json_view_value(self, value: Any, **kwargs) -> Any:
         return dumps(value, cls=self.json_encoder)
 
     def give_python_to_admin(self, value: str, name: str, **kwargs) -> Any:
         return self.to_python(value)
@@ -253,15 +252,15 @@
             return str(self.get_admin_preview_html(value, name, **kwargs))
 
         if self.get_admin_preview_as() == PREVIEW_TEXT:
             value = str(self.get_admin_preview_text(value, name, **kwargs))
         else:
             value = pformat(self.get_admin_preview_python(value, name, **kwargs))
 
-        return "<pre>{}</pre>".format(value.replace("<", "&lt;"))
+        return pre(value)
 
     def lazy_give(self, l_func: Callable, suffix=None) -> LazyObject:
         return LazyObject(l_func)
 
     def give(self, value, suffix: Optional[str] = None):
         return value
```

### Comparing `django_content_settings-0.8.1/content_settings/types/datetime.py` & `django_content_settings-0.9/content_settings/types/datetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import datetime, time, timedelta
 from django.core.exceptions import ValidationError
 from django.utils import formats
 
 from .basic import SimpleString, PREVIEW_PYTHON
+from .mixins import EmptyNoneMixin
 
 TIMEDELTA_FORMATS = {
     "s": "seconds",
     "m": "minutes",
     "h": "hours",
     "d": "days",
     "w": "weeks",
@@ -23,17 +24,16 @@
             delta_kwargs[TIMEDELTA_FORMATS[val_key]] = val
         except Exception as e:
             raise ValidationError(f"wrong format for {el}: {e}")
 
     return timedelta(**delta_kwargs)
 
 
-class DateTimeString(SimpleString):
+class DateTimeString(EmptyNoneMixin, SimpleString):
     input_formats = formats.get_format_lazy("DATETIME_INPUT_FORMATS")
-    empty_is_none = True
     admin_preview_as = PREVIEW_PYTHON
 
     def get_input_formats(self):
         if isinstance(self.input_formats, str):
             return [self.input_formats]
         return self.input_formats
```

### Comparing `django_content_settings-0.8.1/content_settings/types/each.py` & `django_content_settings-0.9/content_settings/types/each.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,86 @@
 from pprint import pformat
 
 from django.core.exceptions import ValidationError
 
-from . import required, optional, PREVIEW_HTML
+from . import required, optional, PREVIEW_HTML, pre
 
 
 class BaseEach:
-    pass
+    def is_each(self, value):
+        return True
+
+    def validate(self, value):
+        if not self.is_each(value):
+            return
+        self.each_validate(value)
+
+    def to_python(self, value):
+        if not self.is_each(value):
+            return value
+        return self.each_to_python(value)
+
+    def give(self, value, suffix=None):
+        if not self.is_each(value):
+            return value
+        return self.each_give(value, suffix)
+
+    def give_python_to_admin(self, value, name, **kwargs):
+        if not self.is_each(value):
+            return value
+        return self.each_give_python_to_admin(value, name, **kwargs)
+
+    def get_admin_preview_object(self, value, *args, **kwargs):
+        if not self.is_each(value):
+            return pre(value)
+        return self.each_get_admin_preview_object(value, *args, **kwargs)
 
 
 class Item(BaseEach):
     def __init__(self, cs_type):
         self.cs_type = cs_type
 
-    def validate(self, value):
+    def is_each(self, value):
+        return isinstance(value, (list, tuple))
+
+    def each_validate(self, value):
         for i, v in enumerate(value, start=1):
             try:
                 self.cs_type.validate(v)
             except ValidationError as e:
                 raise ValidationError(f"item #{i}: {e.message}")
 
-    def to_python(self, value):
+    def each_to_python(self, value):
         ret = []
         for i, v in enumerate(value, start=1):
             try:
                 ret.append(self.cs_type.to_python(v))
             except ValidationError as e:
                 raise ValidationError(f"item #{i}: {e.message}")
         return ret
 
-    def give_python_to_admin(self, value, name, **kwargs):
+    def each_give_python_to_admin(self, value, name, **kwargs):
         ret = []
         for i, v in enumerate(value, start=1):
             try:
                 ret.append(self.cs_type.give_python_to_admin(v, name, **kwargs))
             except ValidationError as e:
                 raise ValidationError(f"item #{i}: {e.message}")
         return ret
 
     def get_help_format(self):
         yield "A list of items. Each item should be: "
         yield "<div class='subitem'>"
         yield from self.cs_type.get_help_format()
         yield "</div>"
 
-    def give(self, value, suffix=None):
+    def each_give(self, value, suffix=None):
         return [self.cs_type.give(v, suffix) for v in value]
 
-    def get_admin_preview_object(self, value, *args, **kwargs):
+    def each_get_admin_preview_object(self, value, *args, **kwargs):
         return (
             "["
             + (
                 ",".join(
                     [
                         "<div class='subitem'>"
                         + self.cs_type.get_admin_preview_object(v, *args, **kwargs)
@@ -64,29 +93,32 @@
         )
 
 
 class Keys(BaseEach):
     def __init__(self, **kwargs):
         self.cs_types = kwargs
 
-    def validate(self, value):
+    def is_each(self, value):
+        return isinstance(value, dict)
+
+    def each_validate(self, value):
         for k, v in value.items():
             if k not in self.cs_types:
                 continue
             try:
                 self.cs_types[k].validate(v)
             except ValidationError as e:
                 raise ValidationError(f"key {k}: {e.message}")
 
         for k, v in self.cs_types.items():
             if k not in value:
                 if v.default == required:
                     raise ValidationError(f"Missing required key {k}")
 
-    def to_python(self, value):
+    def each_to_python(self, value):
         ret = {}
         for k, v in value.items():
             if k in self.cs_types:
                 try:
                     ret[k] = self.cs_types[k].to_python(v)
                 except ValidationError as e:
                     raise ValidationError(f"key {k}: {e.message}")
@@ -95,15 +127,15 @@
 
         for k, v in self.cs_types.items():
             if k not in ret and v.default not in (optional, required):
                 ret[k] = v.to_python(v.default)
 
         return ret
 
-    def give_python_to_admin(self, value, name, **kwargs):
+    def each_give_python_to_admin(self, value, name, **kwargs):
         ret = {}
         for k, v in value.items():
             if k in self.cs_types:
                 try:
                     ret[k] = self.cs_types[k].give_python_to_admin(v, name, **kwargs)
                 except ValidationError as e:
                     raise ValidationError(f"key {k}: {e.message}")
@@ -126,29 +158,84 @@
             elif v.default == optional:
                 yield "(optional) "
             else:
                 yield f"(default: {v.default if v.default else '<i>empty</i>'}) "
             yield from v.get_help_format()
             yield "</div>"
 
-    def give(self, value, suffix=None):
+    def each_give(self, value, suffix=None):
         return {
             k: self.cs_types[k].give(v, suffix) if k in self.cs_types else v
             for k, v in value.items()
         }
 
-    def get_admin_preview_object(self, value, *args, **kwargs):
-        def pre_format(val):
-            return "<pre>{}</pre>".format(pformat(value).replace("<", "&lt;"))
+    def each_get_admin_preview_object(self, value, *args, **kwargs):
+        return (
+            "{"
+            + ",".join(
+                [
+                    f"<div class='subitem'><i>{k}</i>: {self.cs_types[k].get_admin_preview_object(v, *args, **kwargs) if k in self.cs_types else pre(v)}</div>"
+                    for k, v in value.items()
+                ]
+            )
+            + "}"
+        )
+
+
+class Values(BaseEach):
+    def __init__(self, cs_type):
+        self.cs_type = cs_type
+
+    def is_each(self, value):
+        return isinstance(value, dict)
+
+    def each_validate(self, value):
+        for k, v in value.items():
+            try:
+                self.cs_type.validate(v)
+            except ValidationError as e:
+                raise ValidationError(f"key {k}: {e.message}")
+
+    def each_to_python(self, value):
+        ret = {}
+
+        for k, v in value.items():
+            try:
+                ret[k] = self.cs_type.to_python(v)
+            except ValidationError as e:
+                raise ValidationError(f"key {k}: {e.message}")
+
+        return ret
+
+    def each_give_python_to_admin(self, value, name, **kwargs):
+        ret = {}
+
+        for k, v in value.items():
+            try:
+                ret[k] = self.cs_type.give_python_to_admin(v, name, **kwargs)
+            except ValidationError as e:
+                raise ValidationError(f"key {k}: {e.message}")
+
+        return ret
+
+    def get_help_format(self):
+        yield "A dictionary. Each value should be: "
+        yield "<div class='subitem'>"
+        yield from self.cs_type.get_help_format()
+        yield "</div>"
+
+    def each_give(self, value, suffix=None):
+        return {k: self.cs_type.give(v, suffix) for k, v in value.items()}
 
+    def each_get_admin_preview_object(self, value, *args, **kwargs):
         return (
             "{"
             + ",".join(
                 [
-                    f"<div class='subitem'><i>{k}</i>: {self.cs_types[k].get_admin_preview_object(v, *args, **kwargs) if k in self.cs_types else pre_format(v)}</div>"
+                    f"<div class='subitem'><i>{k}</i>: {self.cs_type.get_admin_preview_object(v, *args, **kwargs)}</div>"
                     for k, v in value.items()
                 ]
             )
             + "}"
         )
```

### Comparing `django_content_settings-0.8.1/content_settings/types/markup.py` & `django_content_settings-0.9/content_settings/types/markup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections.abc import Iterable
 from functools import cached_property
 
 from django.core.exceptions import ValidationError
 
 from .basic import SimpleText, PREVIEW_PYTHON, SimpleString
 from .each import EachMixin, Keys, Item
+from .mixins import EmptyNoneMixin
 from . import required, optional
 
 
 class SimpleYAML(SimpleText):
     help_format = "Simple <a href='https://en.wikipedia.org/wiki/YAML' target='_blank'>YAML format</a>"
     admin_preview_as = PREVIEW_PYTHON
     yaml_loader = None
@@ -40,15 +41,15 @@
 
         try:
             return load(value, Loader=self.get_yaml_loader())
         except Exception as e:
             raise ValidationError(str(e))
 
 
-class SimpleJSON(SimpleText):
+class SimpleJSON(EmptyNoneMixin, SimpleText):
     help_format = "Simple <a href='https://en.wikipedia.org/wiki/JSON' target='_blank'>JSON format</a>"
     admin_preview_as = PREVIEW_PYTHON
     decoder_cls = None
     tags = {"json"}
 
     def get_decoder_cls(self):
         return self.decoder_cls
```

### Comparing `django_content_settings-0.8.1/content_settings/types/mixins.py` & `django_content_settings-0.9/content_settings/types/mixins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Optional
 from pprint import pformat
 
 from django.core.exceptions import ValidationError
 from django.utils.safestring import mark_safe
 
 from .validators import call_validator
-from . import PREVIEW_HTML
+from . import PREVIEW_HTML, pre, PREVIEW_TEXT, PREVIEW_PYTHON, PREVIEW_NONE
 
 
 def mix(*cls):
     return type("", cls, {})
 
 
 class MinMaxValidationMixin:
@@ -35,14 +35,23 @@
         if self.min_value is not None:
             yield f" from {self.min_value}"
 
         if self.max_value is not None:
             yield f" to {self.max_value}"
 
 
+class EmptyNoneMixin:
+    value_required = False
+
+    def to_python(self, value):
+        if value.strip() == "":
+            return None
+        return super().to_python(value)
+
+
 class HTMLMixin:
     admin_preview_as: str = PREVIEW_HTML
 
     def get_help_format(self):
         yield from super().get_help_format()
         yield " in HTML format"
 
@@ -52,24 +61,24 @@
 
 class PositiveValidationMixin(MinMaxValidationMixin):
     min_value = 0
 
 
 class CallToPythonMixin:
     call_func = None
-    preview_validators = None
-    admin_preview_call = True
 
     def prepare_python_call(self, value):
         return {"prepared": value}
 
     def get_preview_validators(self):
-        if self.preview_validators is None:
-            return ()
-        return self.preview_validators
+        return [
+            validator
+            for validator in self.get_validators()
+            if isinstance(validator, call_validator)
+        ]
 
     def get_call_func(self):
         return self.call_func
 
     def python_call(self, *args, **kwargs):
         return self.call_func(*args, **kwargs)
 
@@ -85,86 +94,72 @@
     def give_python_to_admin(self, value, name):
         try:
             value = self.to_python(value)
         except Exception as e:
             return [(None, e)]
         ret = []
         for validator in self.get_preview_validators():
-            str_validator = (
-                f"{name}({str(validator)})" if self.admin_preview_call else None
-            )
+            str_validator = f"{name}({str(validator)})"
             try:
                 ret.append((str_validator, validator(value)))
             except Exception as e:
                 ret.append((str_validator, e))
         return ret
 
-    def get_admin_preview_html(self, value, name, **kwargs):
-        if not value:
-            return "No preview (add at least one validator to preview_validators)"
-        html = ""
-        for validator, val in value:
-            if validator:
-                html += f"<div>{validator}</div>"
+    def get_admin_preview_object(self, value, name, **kwargs):
+        admin_preview_as = self.get_admin_preview_as()
+        if admin_preview_as == PREVIEW_NONE:
+            return ""
 
-            if isinstance(val, Exception):
-                val = f"ERROR!!! {val}"
+        if not value:
+            return "No preview (add at least one call_validator in validators)"
 
-            if not self.admin_preview_call and len(value) == 1:
-                html += str(val)
+        if len(value) == 1 and admin_preview_as in (PREVIEW_TEXT, PREVIEW_HTML):
+            value = value[0][1]
+            if isinstance(value, Exception):
+                return f"ERROR!!! {value}"
+            if admin_preview_as == PREVIEW_TEXT:
+                return pre(value)
             else:
-                html += f"<div>{val}</div>"
-
-        return html
-
-    def get_admin_preview_text(self, value, name, **kwargs):
-        if not value:
-            return "No preview (add at least one validator to preview_validators)"
+                return str(value)
 
         def _():
             for validator, val in value:
-                if validator:
-                    yield f">>> {validator}"
+                yield pre(f">>> {validator}")
 
                 if isinstance(val, Exception):
                     yield f"ERROR!!! {val}"
-                elif not self.admin_preview_call and len(value) == 1:
-                    yield str(val)
                 else:
-                    yield f"<<< {pformat(val)}"
+                    if admin_preview_as == PREVIEW_TEXT:
+                        yield pre(val)
+                    elif admin_preview_as == PREVIEW_HTML:
+                        yield str(val)
+                    else:
+                        yield pre("<<< " + pformat(val))
 
         return "\n".join(_())
 
-    def get_admin_preview_python(self, value, name, **kwargs):
-        if self.admin_preview_call:
-            return value
-
-        ret = [v for _, v in value]
-        if len(ret) == 1:
-            return ret[0]
-
-        return ret
-
 
 class GiveCallMixin:
     """
     for Template-like classes, when to_python should return a function,
     but as value you want to return not a function, but call it and return result
     """
 
-    admin_preview_call = False
-
     def get_suffixes(self):
         return ("call",) + super().get_suffixes()
 
     def get_validators(self):
         return (call_validator(),) + super().get_validators()
 
-    def get_preview_validators(self):
-        return (call_validator(),) + super().get_preview_validators()
+    def get_validators(self):
+        validators = super().get_validators()
+        if not validators:
+            return (call_validator(),)
+        return validators
 
     def give(self, value, suffix=None):
         if suffix is None:
             return value()
         if suffix == "call":
             return value
         return super().give(value, suffix)
```

### Comparing `django_content_settings-0.8.1/content_settings/types/template.py` & `django_content_settings-0.9/content_settings/types/template.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from itertools import zip_longest
 
 from django.core.exceptions import ValidationError
+from django.utils.safestring import mark_safe
 
 from .basic import SimpleText
 from .mixins import CallToPythonMixin, GiveCallMixin, HTMLMixin
 from .validators import call_validator
-from . import PREVIEW_TEXT, PREVIEW_PYTHON, required
+from . import PREVIEW_TEXT, PREVIEW_PYTHON, PREVIEW_HTML, required
 from ..permissions import superuser
+from .validators import call_validator
 
 
 class SimpleCallTemplate(CallToPythonMixin, SimpleText):
     admin_preview_as = PREVIEW_TEXT
     template_static_includes = ("CONTENT_SETTINGS", "SETTINGS")
     template_static_data = None
     template_args_default = None
@@ -30,14 +32,27 @@
     def get_template_static_data(self):
         if not self.template_static_data:
             return {}
         if callable(self.template_static_data):
             return self.template_static_data()
         return self.template_static_data
 
+    def get_validators(self):
+        validators = super().get_validators()
+        if validators:
+            return validators
+
+        has_required_args = any(
+            v == required for v in self.get_template_args_default().values()
+        )
+        if has_required_args:
+            return ()
+
+        return (call_validator(),)
+
     def get_help_format(self):
         yield self.help_format
         yield " Available objects:<ul>"
 
         for name, default in self.get_template_args_default().items():
             yield f"<li>{name}"
             if default == required:
@@ -87,46 +102,49 @@
             **ret,
             **self.get_template_static_data(),
         }
 
 
 class DjangoTemplate(SimpleCallTemplate):
     tags = {"template"}
+    admin_preview_as = PREVIEW_TEXT
 
     def prepare_python_call(self, value):
         from django.template import Template
 
         return {"template": Template(value.strip())}
 
     def python_call(self, *args, **kwargs):
         from django.template import Context
 
         template = kwargs.pop("template")
-        return template.render(
-            Context(
-                {
-                    **self.get_template_full_static_data(),
-                    **self.prepate_input_to_dict(*args, **kwargs),
-                }
+        return (
+            template.render(
+                Context(
+                    {
+                        **self.get_template_full_static_data(),
+                        **self.prepate_input_to_dict(*args, **kwargs),
+                    }
+                )
             )
-        )
+            + ""
+        )  # to avoid returning SafeText
 
 
 class DjangoTemplateNoArgs(GiveCallMixin, DjangoTemplate):
     pass
 
 
-class DjangoTemplateHTML(HTMLMixin, DjangoTemplate):
+class DjangoTemplateHTML(HTMLMixin, DjangoTemplateNoArgs):
     pass
 
 
 class DjangoModelTemplateMixin:
     model_queryset = None
     obj_name = "object"
-    admin_preview_call = False
 
     def get_template_args_default(self):
         return {
             self.obj_name: required,
             **super().get_template_args_default(),
         }
 
@@ -141,25 +159,25 @@
         first_validator = self.get_first_call_validator()
 
         if first_validator is not None:
             validators = (first_validator, *validators)
 
         return validators
 
-    def get_preview_validators(self):
-        first_validator = self.get_first_call_validator()
 
-        if first_validator is not None:
-            return (first_validator,)
+class DjangoModelTemplate(DjangoModelTemplateMixin, DjangoTemplate):
+    pass
 
-        return ()
 
+class DjangoModelTemplateHTML(DjangoModelTemplate):
+    admin_preview_as = PREVIEW_HTML
 
-class DjangoModelTemplate(DjangoModelTemplateMixin, DjangoTemplate):
-    pass
+    def give(self, value, suffix=None):
+        render_func = super().give(value, suffix)
+        return lambda *a, **k: mark_safe(render_func(*a, **k))
 
 
 class SimpleEval(SimpleCallTemplate):
     update_permission = staticmethod(superuser)
     help_format = "Python code that returns a value."
     tags = {"eval"}
     admin_preview_as = PREVIEW_PYTHON
```

### Comparing `django_content_settings-0.8.1/content_settings/types/validators.py` & `django_content_settings-0.9/content_settings/types/validators.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/content_settings/views.py` & `django_content_settings-0.9/content_settings/views.py`

 * *Files identical despite different names*

### Comparing `django_content_settings-0.8.1/pyproject.toml` & `django_content_settings-0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-content-settings"
-version = "0.8.1"
+version = "0.9"
 description = "Ability to easily create and manage editable variables directly from the Django admin panel"
 homepage = "https://django-content-settings.readthedocs.io/en/latest/"
 repository = "https://github.com/occipital/django-content-settings/"
 authors = ["oduvan <a.lyabah@checkio.org>"]
 keywords = ["Django", "settings"]
 readme = "README_SHORT.md"
 classifiers = [
```

### Comparing `django_content_settings-0.8.1/PKG-INFO` & `django_content_settings-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-content-settings
-Version: 0.8.1
+Version: 0.9
 Summary: Ability to easily create and manage editable variables directly from the Django admin panel
 Home-page: https://django-content-settings.readthedocs.io/en/latest/
 License: MIT
 Keywords: Django,settings
 Author: oduvan
 Author-email: a.lyabah@checkio.org
 Requires-Python: >=3.8,<=3.12
```

