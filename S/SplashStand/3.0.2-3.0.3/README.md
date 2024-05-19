# Comparing `tmp/splashstand-3.0.2.tar.gz` & `tmp/splashstand-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splashstand-3.0.2.tar", last modified: Mon Mar  4 16:48:53 2024, max compression
+gzip compressed data, was "splashstand-3.0.3.tar", last modified: Sun May 19 18:44:53 2024, max compression
```

## Comparing `splashstand-3.0.2.tar` & `splashstand-3.0.3.tar`

### file list

```diff
@@ -1,204 +1,201 @@
--rw-r--r--   0        0        0     1497 2023-10-09 08:19:12.605666 splashstand-3.0.2/LICENSE
--rw-r--r--   0        0        0        0 2020-06-11 09:50:00.000000 splashstand-3.0.2/bin/__init__.py
--rw-r--r--   0        0        0      774 2024-01-07 08:40:43.345428 splashstand-3.0.2/bin/checkversions.py
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.087195 splashstand-3.0.2/bin/deploy/Dockerfile
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.091418 splashstand-3.0.2/bin/deploy/deploy.py
--rw-r--r--   0        0        0     3229 2023-10-09 12:31:07.524065 splashstand-3.0.2/bin/deploy/upgrade.py
--rw-r--r--   0        0        0     5728 2023-10-09 22:41:42.879511 splashstand-3.0.2/bin/startproject.py
--rw-r--r--   0        0        0     3843 2023-10-09 23:02:56.872038 splashstand-3.0.2/bin/upgradeproject.py
--rw-r--r--   0        0        0     3692 2024-03-04 16:48:53.861794 splashstand-3.0.2/pyproject.toml
--rw-r--r--   0        0        0      201 2023-10-08 07:49:18.355334 splashstand-3.0.2/splashstand/.dockerignore
--rw-r--r--   0        0        0      190 2023-10-08 07:49:18.360765 splashstand-3.0.2/splashstand/.gcloudignore
--rw-r--r--   0        0        0      189 2024-01-07 08:32:28.068168 splashstand-3.0.2/splashstand/.gitignore
--rw-r--r--   0        0        0        0 2024-02-08 15:34:19.647687 splashstand-3.0.2/splashstand/__init__.py
--rw-r--r--   0        0        0      282 2024-02-08 15:50:39.132974 splashstand-3.0.2/splashstand/__main__.py
--rw-r--r--   0        0        0       62 2024-01-16 17:26:09.447878 splashstand-3.0.2/splashstand/actions/__init__.py
--rw-r--r--   0        0        0        0 2024-02-08 15:44:34.530650 splashstand-3.0.2/splashstand/adapters/__init__.py
--rw-r--r--   0        0        0       62 2023-11-04 13:19:08.196866 splashstand-3.0.2/splashstand/adapters/admin/__init__.py
--rw-r--r--   0        0        0      146 2024-02-08 21:13:42.797239 splashstand-3.0.2/splashstand/adapters/admin/_base.py
--rw-r--r--   0        0        0     1243 2024-02-09 11:40:20.420816 splashstand-3.0.2/splashstand/adapters/admin/_manifest.py
--rw-r--r--   0        0        0    47070 2024-03-04 16:47:02.806219 splashstand-3.0.2/splashstand/adapters/admin/sqladmin.py
--rw-r--r--   0        0        0       66 2024-01-08 19:50:52.239671 splashstand-3.0.2/splashstand/adapters/analytics/__init__.py
--rw-r--r--   0        0        0      104 2024-02-05 06:27:27.240871 splashstand-3.0.2/splashstand/adapters/analytics/_base.py
--rw-r--r--   0        0        0      804 2024-01-27 07:27:46.673157 splashstand-3.0.2/splashstand/adapters/analytics/google.py
--rw-r--r--   0        0        0       60 2023-11-04 13:47:39.012562 splashstand-3.0.2/splashstand/adapters/app/__init__.py
--rw-r--r--   0        0        0      315 2024-02-24 10:37:18.252682 splashstand-3.0.2/splashstand/adapters/app/_base.py
--rw-r--r--   0        0        0     1883 2024-02-09 11:40:20.425409 splashstand-3.0.2/splashstand/adapters/app/_manifest.py
--rw-r--r--   0        0        0    11401 2024-02-09 12:53:06.009552 splashstand-3.0.2/splashstand/adapters/app/demo.py
--rw-r--r--   0        0        0     5318 2024-03-04 10:16:34.202188 splashstand-3.0.2/splashstand/adapters/app/main.py
--rw-r--r--   0        0        0       62 2024-01-24 11:56:36.687465 splashstand-3.0.2/splashstand/adapters/auth/__init__.py
--rw-r--r--   0        0        0     1727 2024-03-01 16:52:42.657450 splashstand-3.0.2/splashstand/adapters/auth/_base.py
--rw-r--r--   0        0        0     6532 2024-03-04 16:35:54.942259 splashstand-3.0.2/splashstand/adapters/auth/firebase.py
--rw-r--r--   0        0        0       66 2024-01-15 08:35:50.407500 splashstand-3.0.2/splashstand/adapters/captcha/__init__.py
--rw-r--r--   0        0        0      468 2024-02-09 11:38:05.704840 splashstand-3.0.2/splashstand/adapters/captcha/_base.py
--rw-r--r--   0        0        0     4369 2024-02-19 16:27:13.481012 splashstand-3.0.2/splashstand/adapters/captcha/google.py
--rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 splashstand-3.0.2/splashstand/adapters/mail/__init__.py
--rw-r--r--   0        0        0     5940 2023-07-07 13:49:10.956883 splashstand-3.0.2/splashstand/adapters/mail/mail.py
--rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 splashstand-3.0.2/splashstand/adapters/marketing/__init__.py
--rw-r--r--   0        0        0        0 2023-09-28 15:09:22.564270 splashstand-3.0.2/splashstand/adapters/marketing/mailchimp_.py
--rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 splashstand-3.0.2/splashstand/adapters/messaging/__init__.py
--rw-r--r--   0        0        0        0 2023-09-28 15:09:22.564270 splashstand-3.0.2/splashstand/adapters/messaging/firebase.py
--rw-r--r--   0        0        0       63 2024-02-07 20:56:24.207919 splashstand-3.0.2/splashstand/adapters/models/__init__.py
--rw-r--r--   0        0        0    16425 2024-03-01 09:40:13.085513 splashstand-3.0.2/splashstand/adapters/models/main.py
--rw-r--r--   0        0        0       60 2024-01-15 08:35:50.421574 splashstand-3.0.2/splashstand/adapters/pwa/__init__.py
--rw-r--r--   0        0        0       63 2024-02-07 11:18:36.653787 splashstand-3.0.2/splashstand/adapters/routes/__init__.py
--rw-r--r--   0        0        0      148 2024-02-07 21:14:30.088129 splashstand-3.0.2/splashstand/adapters/routes/_base.py
--rw-r--r--   0        0        0     2080 2024-03-02 16:37:25.712128 splashstand-3.0.2/splashstand/adapters/routes/main.py
--rw-r--r--   0        0        0       63 2024-01-15 08:52:24.049595 splashstand-3.0.2/splashstand/adapters/social/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.036675 splashstand-3.0.2/splashstand/adapters/social/facebook_.py
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.823043 splashstand-3.0.2/splashstand/migrations/alembic.ini
--rw-r--r--   0        0        0        0 2023-04-16 10:25:27.315716 splashstand-3.0.2/splashstand/migrations/env.py
--rw-r--r--   0        0        0        0 2023-04-16 10:25:27.275017 splashstand-3.0.2/splashstand/migrations/script.py.mako
--rw-r--r--   0        0        0      222 2024-01-28 11:37:37.164057 splashstand-3.0.2/splashstand/schemas/thing/_base.yml
--rw-r--r--   0        0        0      553 2024-01-29 10:55:29.082736 splashstand-3.0.2/splashstand/schemas/thing/creative_work/_base.yml
--rw-r--r--   0        0        0       53 2024-01-24 04:05:53.864155 splashstand-3.0.2/splashstand/schemas/thing/creative_work/_collection.yml
--rw-r--r--   0        0        0       62 2024-02-04 19:39:55.445764 splashstand-3.0.2/splashstand/schemas/thing/creative_work/_defined_term_set.yml
--rw-r--r--   0        0        0      194 2024-01-29 15:11:07.427995 splashstand-3.0.2/splashstand/schemas/thing/creative_work/article/_base.yml
--rw-r--r--   0        0        0       55 2024-02-04 19:39:55.430963 splashstand-3.0.2/splashstand/schemas/thing/creative_work/article/blog_posting.yml
--rw-r--r--   0        0        0       53 2024-01-22 11:40:24.546506 splashstand-3.0.2/splashstand/schemas/thing/creative_work/article/news_article.yml
--rw-r--r--   0        0        0        0 2024-01-22 11:40:24.550576 splashstand-3.0.2/splashstand/schemas/thing/creative_work/article/social_media_posting.yml
--rw-r--r--   0        0        0       47 2024-02-02 11:36:27.753070 splashstand-3.0.2/splashstand/schemas/thing/creative_work/blog.yml
--rw-r--r--   0        0        0      404 2024-01-28 11:29:46.708967 splashstand-3.0.2/splashstand/schemas/thing/creative_work/media_object/_base.yml
--rw-r--r--   0        0        0      194 2024-01-22 11:16:25.570379 splashstand-3.0.2/splashstand/schemas/thing/creative_work/media_object/audio_object.yml
--rw-r--r--   0        0        0      178 2024-01-22 11:16:25.546054 splashstand-3.0.2/splashstand/schemas/thing/creative_work/media_object/image_object.yml
--rw-r--r--   0        0        0      324 2024-02-04 19:39:55.443337 splashstand-3.0.2/splashstand/schemas/thing/creative_work/media_object/video_object.yml
--rw-r--r--   0        0        0      454 2024-01-28 11:13:09.049423 splashstand-3.0.2/splashstand/schemas/thing/creative_work/music_album.yml
--rw-r--r--   0        0        0       98 2024-01-28 11:13:09.055008 splashstand-3.0.2/splashstand/schemas/thing/creative_work/music_playlist.yml
--rw-r--r--   0        0        0      292 2024-01-29 14:39:41.433784 splashstand-3.0.2/splashstand/schemas/thing/creative_work/music_recording.yml
--rw-r--r--   0        0        0       12 2024-01-24 12:41:27.932026 splashstand-3.0.2/splashstand/schemas/thing/creative_work/poster.yml
--rw-r--r--   0        0        0      486 2024-01-29 09:12:15.709724 splashstand-3.0.2/splashstand/schemas/thing/event/_base.yml
--rw-r--r--   0        0        0       12 2024-01-22 11:16:25.578830 splashstand-3.0.2/splashstand/schemas/thing/event/music_event.yml
--rw-r--r--   0        0        0       95 2024-02-04 19:39:55.435562 splashstand-3.0.2/splashstand/schemas/thing/intangible/_defined_term.yml
--rw-r--r--   0        0        0       75 2024-01-23 22:25:16.758548 splashstand-3.0.2/splashstand/schemas/thing/intangible/category_code.yml
--rw-r--r--   0        0        0      310 2024-01-28 11:14:17.459275 splashstand-3.0.2/splashstand/schemas/thing/intangible/contact_point/_base.yml
--rw-r--r--   0        0        0      199 2024-01-28 11:15:36.772150 splashstand-3.0.2/splashstand/schemas/thing/intangible/contact_point/postal_address.yml
--rw-r--r--   0        0        0      112 2024-02-02 10:15:54.007731 splashstand-3.0.2/splashstand/schemas/thing/intangible/offer.yml
--rw-r--r--   0        0        0        0 2023-04-16 10:25:27.535462 splashstand-3.0.2/splashstand/schemas/thing/intangible/price_specification.yml
--rw-r--r--   0        0        0      128 2024-01-28 11:29:46.704013 splashstand-3.0.2/splashstand/schemas/thing/intangible/quantitative_value.yml
--rw-r--r--   0        0        0      625 2024-01-23 22:25:16.717752 splashstand-3.0.2/splashstand/schemas/thing/intangible/schedule.yml
--rw-r--r--   0        0        0      233 2024-01-29 08:22:15.686054 splashstand-3.0.2/splashstand/schemas/thing/intangible/type_and_quantity_node.yml
--rw-r--r--   0        0        0      150 2024-01-28 11:11:28.413128 splashstand-3.0.2/splashstand/schemas/thing/organization/_base.yml
--rw-r--r--   0        0        0        0 2024-01-22 10:54:15.859449 splashstand-3.0.2/splashstand/schemas/thing/organization/dance_group.yml
--rw-r--r--   0        0        0      119 2024-01-29 14:42:53.974389 splashstand-3.0.2/splashstand/schemas/thing/organization/music_group.yml
--rw-r--r--   0        0        0        0 2024-01-24 12:41:27.932506 splashstand-3.0.2/splashstand/schemas/thing/organization/performing_group.yml
--rw-r--r--   0        0        0        0 2024-01-24 12:41:27.953199 splashstand-3.0.2/splashstand/schemas/thing/organization/theater_group.yml
--rw-r--r--   0        0        0      578 2024-02-09 15:51:56.973911 splashstand-3.0.2/splashstand/schemas/thing/person/_base.yml
--rw-r--r--   0        0        0      457 2024-02-02 10:32:55.977099 splashstand-3.0.2/splashstand/schemas/thing/place/_base.yml
--rw-r--r--   0        0        0        0 2024-01-24 12:41:27.941123 splashstand-3.0.2/splashstand/schemas/thing/place/entertainment_business.yml
--rw-r--r--   0        0        0      139 2024-01-23 21:08:22.681995 splashstand-3.0.2/splashstand/schemas/thing/place/food_establishment.yml
--rw-r--r--   0        0        0      290 2024-01-23 21:08:22.676063 splashstand-3.0.2/splashstand/schemas/thing/place/lodging_business.yml
--rw-r--r--   0        0        0        0 2024-01-23 21:08:22.665060 splashstand-3.0.2/splashstand/schemas/thing/place/music_venue.yml
--rw-r--r--   0        0        0      226 2024-02-04 19:39:55.432246 splashstand-3.0.2/splashstand/schemas/thing/product/_base.yml
--rw-r--r--   0        0        0       89 2024-01-23 22:15:32.819070 splashstand-3.0.2/splashstand/schemas/thing/product/_product_collection.yml
--rw-r--r--   0        0        0      150 2024-02-04 19:39:55.451041 splashstand-3.0.2/splashstand/schemas/thing/product/_product_group.yml
--rw-r--r--   0        0        0       82 2024-01-28 11:22:23.616248 splashstand-3.0.2/splashstand/schemas/thing/product/_some_products.yml
--rw-r--r--   0        0        0      322 2024-03-04 16:47:05.529591 splashstand-3.0.2/splashstand/settings/adapters.yml
--rw-r--r--   0        0        0       83 2024-03-04 16:47:15.551059 splashstand-3.0.2/splashstand/settings/admin.yml
--rw-r--r--   0        0        0      110 2024-03-04 16:47:08.918497 splashstand-3.0.2/splashstand/settings/app.yml
--rw-r--r--   0        0        0      115 2024-03-04 16:47:06.559165 splashstand-3.0.2/splashstand/settings/auth.yml
--rw-r--r--   0        0        0      134 2024-03-04 16:47:06.134252 splashstand-3.0.2/splashstand/settings/cache.yml
--rw-r--r--   0        0        0      333 2024-03-04 16:47:05.019953 splashstand-3.0.2/splashstand/settings/debug.yml
--rw-r--r--   0        0        0       37 2024-03-04 16:47:05.144792 splashstand-3.0.2/splashstand/settings/logger.yml
--rw-r--r--   0        0        0       27 2024-03-04 16:47:07.057287 splashstand-3.0.2/splashstand/settings/models.yml
--rw-r--r--   0        0        0       32 2024-01-14 13:39:55.831734 splashstand-3.0.2/splashstand/settings/monitoring.yml
--rw-r--r--   0        0        0       16 2024-02-09 10:05:07.028234 splashstand-3.0.2/splashstand/settings/requests.yml
--rw-r--r--   0        0        0        3 2024-03-04 16:47:11.869686 splashstand-3.0.2/splashstand/settings/routes.yml
--rw-r--r--   0        0        0       37 2024-03-04 16:47:12.215987 splashstand-3.0.2/splashstand/settings/sql.yml
--rw-r--r--   0        0        0      164 2024-03-04 16:47:10.103381 splashstand-3.0.2/splashstand/settings/storage.yml
--rw-r--r--   0        0        0       59 2024-03-04 16:47:11.659327 splashstand-3.0.2/splashstand/settings/templates.yml
--rw-r--r--   0        0        0        0 2023-10-09 12:28:22.664820 splashstand-3.0.2/splashstand/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.468507 splashstand-3.0.2/splashstand/templates/admin/base/base.html.blah
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.465280 splashstand-3.0.2/splashstand/templates/admin/base/head.html.blah
--rw-r--r--   0        0        0     3132 2024-01-24 12:41:27.952900 splashstand-3.0.2/splashstand/templates/admin/base/js/serviceworker.js
--rw-r--r--   0        0        0     3362 2024-03-04 16:21:30.478428 splashstand-3.0.2/splashstand/templates/admin/base/tail.html.blah
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.430976 splashstand-3.0.2/splashstand/templates/admin/bulma/base.html.blah
--rw-r--r--   0        0        0      301 2024-03-04 16:21:30.470880 splashstand-3.0.2/splashstand/templates/admin/bulma/blocks/display_menu.html
--rw-r--r--   0        0        0     1127 2024-03-04 16:21:30.478801 splashstand-3.0.2/splashstand/templates/admin/bulma/blocks/menu_category.html
--rw-r--r--   0        0        0      422 2024-03-04 16:21:30.466542 splashstand-3.0.2/splashstand/templates/admin/bulma/blocks/menu_item.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.384215 splashstand-3.0.2/splashstand/templates/admin/bulma/create.html.blah
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.378407 splashstand-3.0.2/splashstand/templates/admin/bulma/delete.html.blah
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.365228 splashstand-3.0.2/splashstand/templates/admin/bulma/details.html.blah
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.424290 splashstand-3.0.2/splashstand/templates/admin/bulma/edit.html.blah
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.411254 splashstand-3.0.2/splashstand/templates/admin/bulma/error.html.blah
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.400973 splashstand-3.0.2/splashstand/templates/admin/bulma/index.html.blah
--rw-r--r--   0        0        0     2017 2024-03-04 16:21:30.465498 splashstand-3.0.2/splashstand/templates/admin/bulma/layout.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.417745 splashstand-3.0.2/splashstand/templates/admin/bulma/list.html.blah
--rw-r--r--   0        0        0     2022 2024-03-04 16:21:30.464316 splashstand-3.0.2/splashstand/templates/admin/bulma/login.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.446452 splashstand-3.0.2/splashstand/templates/admin/bulma/scss/admin.scss
--rw-r--r--   0        0        0    21368 2023-04-16 10:25:26.449863 splashstand-3.0.2/splashstand/templates/admin/bulma/scss/admin.yml
--rw-r--r--   0        0        0     1676 2023-10-08 07:49:18.349781 splashstand-3.0.2/splashstand/templates/admin/old/actions.html
--rw-r--r--   0        0        0     3670 2023-10-08 07:49:18.360195 splashstand-3.0.2/splashstand/templates/admin/old/analytics.html
--rw-r--r--   0        0        0     1614 2023-10-08 07:49:18.356792 splashstand-3.0.2/splashstand/templates/admin/old/content.html
--rw-r--r--   0        0        0     2401 2023-10-08 07:49:18.335133 splashstand-3.0.2/splashstand/templates/admin/old/details_modal.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.513578 splashstand-3.0.2/splashstand/templates/admin/old/edit_modal.html
--rw-r--r--   0        0        0      174 2023-10-08 07:49:18.359010 splashstand-3.0.2/splashstand/templates/admin/old/help.html
--rw-r--r--   0        0        0    12664 2023-04-29 15:04:31.101823 splashstand-3.0.2/splashstand/templates/admin/old/index.html
--rw-r--r--   0        0        0     2505 2023-10-08 07:49:18.355106 splashstand-3.0.2/splashstand/templates/admin/old/layout.html
--rw-r--r--   0        0        0    16475 2023-04-29 15:04:31.062084 splashstand-3.0.2/splashstand/templates/admin/old/lib.html
--rw-r--r--   0        0        0    10563 2023-10-08 07:49:18.337642 splashstand-3.0.2/splashstand/templates/admin/old/list.html
--rw-r--r--   0        0        0     2153 2023-10-08 07:49:18.329264 splashstand-3.0.2/splashstand/templates/admin/old/modal.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.530050 splashstand-3.0.2/splashstand/templates/admin/old/offline.html
--rw-r--r--   0        0        0      174 2023-04-16 10:25:26.526789 splashstand-3.0.2/splashstand/templates/admin/old/preview.html
--rw-r--r--   0        0        0      938 2023-10-08 07:49:18.337808 splashstand-3.0.2/splashstand/templates/admin/old/redis_console.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.485086 splashstand-3.0.2/splashstand/templates/admin/old/redis_response.html
--rw-r--r--   0        0        0     1974 2023-10-08 07:49:18.360424 splashstand-3.0.2/splashstand/templates/admin/old/row_actions.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.516813 splashstand-3.0.2/splashstand/templates/admin/old/site_edit.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.543476 splashstand-3.0.2/splashstand/templates/admin/old/static.html
--rw-r--r--   0        0        0    12313 2023-10-08 07:49:18.328464 splashstand-3.0.2/splashstand/templates/admin/old/storage_list.html
--rw-r--r--   0        0        0      146 2023-04-16 10:25:26.552654 splashstand-3.0.2/splashstand/templates/admin/old/store.html
--rw-r--r--   0        0        0      174 2023-10-08 07:49:18.355650 splashstand-3.0.2/splashstand/templates/admin/old/support.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.481539 splashstand-3.0.2/splashstand/templates/admin/old/theme_details_modal.html
--rw-r--r--   0        0        0     5691 2023-10-08 07:49:18.359164 splashstand-3.0.2/splashstand/templates/admin/old/theme_edit.html
--rw-r--r--   0        0        0     3774 2023-10-08 07:49:18.347873 splashstand-3.0.2/splashstand/templates/admin/old/theme_list.html
--rw-r--r--   0        0        0      760 2024-03-03 13:26:30.340077 splashstand-3.0.2/splashstand/templates/app/base/base.html
--rw-r--r--   0        0        0      211 2024-02-25 14:27:15.782831 splashstand-3.0.2/splashstand/templates/app/base/blocks/head.html
--rw-r--r--   0        0        0     1365 2023-10-08 07:49:18.341683 splashstand-3.0.2/splashstand/templates/app/base/blocks/tail.html
--rw-r--r--   0        0        0      102 2024-02-25 14:27:15.760110 splashstand-3.0.2/splashstand/templates/app/base/blocks/title.html
--rw-r--r--   0        0        0     3828 2023-10-08 07:49:18.328317 splashstand-3.0.2/splashstand/templates/app/base/js/serviceworker.js
--rw-r--r--   0        0        0      220 2023-04-16 10:25:26.330632 splashstand-3.0.2/splashstand/templates/app/base/robots.txt
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.325355 splashstand-3.0.2/splashstand/templates/app/base/sitemap.xml
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.319604 splashstand-3.0.2/splashstand/templates/app/base/sitemapindex.xml
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.686163 splashstand-3.0.2/splashstand/templates/app/bulma/about.html
--rw-r--r--   0        0        0      433 2023-10-08 07:49:18.360585 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/components.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.615759 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/construction.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.608494 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/contact_image.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.619053 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/contact_map.html
--rw-r--r--   0        0        0     4911 2023-10-08 07:49:18.355957 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/elements.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.636859 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/event_list.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.633950 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/event_past.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.630684 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/event_tile.html
--rw-r--r--   0        0        0     1003 2023-04-16 10:25:26.676673 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/footer.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.695120 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/form.html
--rw-r--r--   0        0        0     5353 2023-10-08 07:49:18.344167 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/header.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.669499 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/mailer.html
--rw-r--r--   0        0        0     2944 2023-10-08 07:49:18.334587 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/nav.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.652459 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/news_list.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.647547 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/news_tile.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.612249 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/project_list.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.626778 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/quote_tile.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.643223 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/user_tile.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.622339 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/venue_list.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.683136 splashstand-3.0.2/splashstand/templates/app/bulma/blocks/video.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.666348 splashstand-3.0.2/splashstand/templates/app/bulma/contact.html
--rw-r--r--   0        0        0       17 2024-02-25 14:27:15.758187 splashstand-3.0.2/splashstand/templates/app/bulma/events.html
--rw-r--r--   0        0        0       33 2024-02-24 08:12:48.452202 splashstand-3.0.2/splashstand/templates/app/bulma/home.html
--rw-r--r--   0        0        0      192 2024-02-25 14:27:15.739081 splashstand-3.0.2/splashstand/templates/app/bulma/index.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.663198 splashstand-3.0.2/splashstand/templates/app/bulma/offline.html
--rw-r--r--   0        0        0     6731 2023-10-08 07:49:18.357156 splashstand-3.0.2/splashstand/templates/app/bulma/privacy_policy.html
--rw-r--r--   0        0        0     6067 2024-02-24 08:12:48.459332 splashstand-3.0.2/splashstand/templates/app/bulma/service_terms.html
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.708359 splashstand-3.0.2/splashstand/templates/app/bulma/style/custom.scss
--rw-r--r--   0        0        0    22109 2023-04-16 10:25:26.715204 splashstand-3.0.2/splashstand/templates/app/bulma/style/custom.yml
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.705086 splashstand-3.0.2/splashstand/templates/app/bulma/style/fender.scss
--rw-r--r--   0        0        0    21435 2023-04-16 10:25:26.711727 splashstand-3.0.2/splashstand/templates/app/bulma/style/fender.yml
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.126798 splashstand-3.0.2/splashstand/tmp/migrations/README
--rw-r--r--   0        0        0        0 2023-04-16 10:25:26.130056 splashstand-3.0.2/splashstand/tmp/migrations/env.py
--rw-r--r--   0        0        0       43 2024-03-01 14:32:58.470182 splashstand-3.0.2/splashstand/tmp/secrets/app_secret_key
--rw-r--r--   0        0        0       90 2024-03-01 14:32:58.553550 splashstand-3.0.2/splashstand/tmp/secrets/app_secure_salt
--rw-r--r--   0        0        0       39 2024-03-01 14:33:00.066684 splashstand-3.0.2/splashstand/tmp/secrets/auth_api_key
--rw-r--r--   0        0        0        9 2024-03-01 14:32:59.642793 splashstand-3.0.2/splashstand/tmp/secrets/cache_host
--rw-r--r--   0        0        0       13 2024-03-01 14:32:59.719065 splashstand-3.0.2/splashstand/tmp/secrets/cache_password
--rw-r--r--   0        0        0        9 2024-03-01 14:33:04.722909 splashstand-3.0.2/splashstand/tmp/secrets/sql_host
--rw-r--r--   0        0        0       11 2024-03-01 14:33:04.846091 splashstand-3.0.2/splashstand/tmp/secrets/sql_password
--rw-r--r--   0        0        0        4 2024-03-01 14:33:04.792665 splashstand-3.0.2/splashstand/tmp/secrets/sql_user
--rw-r--r--   0        0        0        0 2020-05-30 12:35:52.000000 splashstand-3.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 splashstand-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-10-09 08:19:12.605666 splashstand-3.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-06-11 09:50:00.000000 splashstand-3.0.3/bin/__init__.py
+-rw-r--r--   0        0        0      774 2024-01-07 08:40:43.345428 splashstand-3.0.3/bin/checkversions.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.087195 splashstand-3.0.3/bin/deploy/Dockerfile
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.091418 splashstand-3.0.3/bin/deploy/deploy.py
+-rw-r--r--   0        0        0     3229 2023-10-09 12:31:07.524065 splashstand-3.0.3/bin/deploy/upgrade.py
+-rw-r--r--   0        0        0     5728 2023-10-09 22:41:42.879511 splashstand-3.0.3/bin/startproject.py
+-rw-r--r--   0        0        0     3843 2023-10-09 23:02:56.872038 splashstand-3.0.3/bin/upgradeproject.py
+-rw-r--r--   0        0        0     3774 2024-05-19 18:44:53.414105 splashstand-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0      201 2023-10-08 07:49:18.355334 splashstand-3.0.3/splashstand/.dockerignore
+-rw-r--r--   0        0        0      190 2023-10-08 07:49:18.360765 splashstand-3.0.3/splashstand/.gcloudignore
+-rw-r--r--   0        0        0      189 2024-01-07 08:32:28.068168 splashstand-3.0.3/splashstand/.gitignore
+-rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 splashstand-3.0.3/splashstand/Dockerfile
+-rw-r--r--   0        0        0        0 2024-02-08 15:34:19.647687 splashstand-3.0.3/splashstand/__init__.py
+-rw-r--r--   0        0        0      282 2024-02-08 15:50:39.132974 splashstand-3.0.3/splashstand/__main__.py
+-rw-r--r--   0        0        0       62 2024-01-16 17:26:09.447878 splashstand-3.0.3/splashstand/actions/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-08 15:44:34.530650 splashstand-3.0.3/splashstand/adapters/__init__.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:19:08.196866 splashstand-3.0.3/splashstand/adapters/admin/__init__.py
+-rw-r--r--   0        0        0      146 2024-02-08 21:13:42.797239 splashstand-3.0.3/splashstand/adapters/admin/_base.py
+-rw-r--r--   0        0        0     1243 2024-02-09 11:40:20.420816 splashstand-3.0.3/splashstand/adapters/admin/_manifest.py
+-rw-r--r--   0        0        0    46664 2024-05-19 18:35:21.672705 splashstand-3.0.3/splashstand/adapters/admin/sqladmin.py
+-rw-r--r--   0        0        0       66 2024-01-08 19:50:52.239671 splashstand-3.0.3/splashstand/adapters/analytics/__init__.py
+-rw-r--r--   0        0        0      104 2024-02-05 06:27:27.240871 splashstand-3.0.3/splashstand/adapters/analytics/_base.py
+-rw-r--r--   0        0        0      804 2024-01-27 07:27:46.673157 splashstand-3.0.3/splashstand/adapters/analytics/google.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:47:39.012562 splashstand-3.0.3/splashstand/adapters/app/__init__.py
+-rw-r--r--   0        0        0      315 2024-02-24 10:37:18.252682 splashstand-3.0.3/splashstand/adapters/app/_base.py
+-rw-r--r--   0        0        0     1883 2024-02-09 11:40:20.425409 splashstand-3.0.3/splashstand/adapters/app/_manifest.py
+-rw-r--r--   0        0        0    11401 2024-02-09 12:53:06.009552 splashstand-3.0.3/splashstand/adapters/app/demo.py
+-rw-r--r--   0        0        0     5918 2024-05-19 17:28:36.963051 splashstand-3.0.3/splashstand/adapters/app/main.py
+-rw-r--r--   0        0        0       62 2024-01-24 11:56:36.687465 splashstand-3.0.3/splashstand/adapters/auth/__init__.py
+-rw-r--r--   0        0        0     2011 2024-05-19 18:36:34.376096 splashstand-3.0.3/splashstand/adapters/auth/_base.py
+-rw-r--r--   0        0        0     6662 2024-05-19 18:39:02.039175 splashstand-3.0.3/splashstand/adapters/auth/firebase.py
+-rw-r--r--   0        0        0       66 2024-01-15 08:35:50.407500 splashstand-3.0.3/splashstand/adapters/captcha/__init__.py
+-rw-r--r--   0        0        0      468 2024-02-09 11:38:05.704840 splashstand-3.0.3/splashstand/adapters/captcha/_base.py
+-rw-r--r--   0        0        0     4369 2024-02-19 16:27:13.481012 splashstand-3.0.3/splashstand/adapters/captcha/google.py
+-rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 splashstand-3.0.3/splashstand/adapters/mail/__init__.py
+-rw-r--r--   0        0        0     5940 2023-07-07 13:49:10.956883 splashstand-3.0.3/splashstand/adapters/mail/mail.py
+-rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 splashstand-3.0.3/splashstand/adapters/marketing/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-28 15:09:22.564270 splashstand-3.0.3/splashstand/adapters/marketing/mailchimp_.py
+-rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 splashstand-3.0.3/splashstand/adapters/messaging/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-28 15:09:22.564270 splashstand-3.0.3/splashstand/adapters/messaging/firebase.py
+-rw-r--r--   0        0        0       60 2024-01-15 08:35:50.421574 splashstand-3.0.3/splashstand/adapters/pwa/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-01 17:17:55.263324 splashstand-3.0.3/splashstand/adapters/schemas/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-01 18:40:46.893221 splashstand-3.0.3/splashstand/adapters/schemas/_base.py
+-rw-r--r--   0        0        0     4266 2024-05-19 14:16:00.283144 splashstand-3.0.3/splashstand/adapters/schemas/_models/__init__.py
+-rw-r--r--   0        0        0     7246 2024-04-01 18:40:46.605991 splashstand-3.0.3/splashstand/adapters/schemas/_models/creative_work.py
+-rw-r--r--   0        0        0     2130 2024-04-01 18:40:46.866627 splashstand-3.0.3/splashstand/adapters/schemas/_models/event.py
+-rw-r--r--   0        0        0     1955 2024-04-01 18:40:46.854919 splashstand-3.0.3/splashstand/adapters/schemas/_models/organization.py
+-rw-r--r--   0        0        0     2575 2024-05-19 18:37:14.211228 splashstand-3.0.3/splashstand/adapters/schemas/_models/person.py
+-rw-r--r--   0        0        0     2258 2024-04-01 18:40:46.617208 splashstand-3.0.3/splashstand/adapters/schemas/_models/place.py
+-rw-r--r--   0        0        0     2751 2024-05-19 18:38:33.402181 splashstand-3.0.3/splashstand/adapters/schemas/schemaorg.py
+-rw-r--r--   0        0        0       63 2024-01-15 08:52:24.049595 splashstand-3.0.3/splashstand/adapters/social/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.036675 splashstand-3.0.3/splashstand/adapters/social/facebook_.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.823043 splashstand-3.0.3/splashstand/migrations/alembic.ini
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:27.315716 splashstand-3.0.3/splashstand/migrations/env.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:27.275017 splashstand-3.0.3/splashstand/migrations/script.py.mako
+-rw-r--r--   0        0        0        0 2024-04-01 16:43:35.281717 splashstand-3.0.3/splashstand/routes.py
+-rw-r--r--   0        0        0       53 2024-01-24 04:05:53.864155 splashstand-3.0.3/splashstand/scrap/_collection.yml
+-rw-r--r--   0        0        0       62 2024-03-25 14:47:12.935480 splashstand-3.0.3/splashstand/scrap/_defined_term_set.yml
+-rw-r--r--   0        0        0      194 2024-03-23 12:35:10.852462 splashstand-3.0.3/splashstand/scrap/audio_object.yml
+-rw-r--r--   0        0        0       12 2024-03-18 08:12:43.384753 splashstand-3.0.3/splashstand/scrap/blog.yml
+-rw-r--r--   0        0        0       85 2024-03-18 08:12:43.383892 splashstand-3.0.3/splashstand/scrap/blog_posting.yml
+-rw-r--r--   0        0        0        0 2024-01-22 10:54:15.859449 splashstand-3.0.3/splashstand/scrap/dance_group.yml
+-rw-r--r--   0        0        0        0 2024-01-24 12:41:27.941123 splashstand-3.0.3/splashstand/scrap/entertainment_business.yml
+-rw-r--r--   0        0        0      139 2024-01-23 21:08:22.681995 splashstand-3.0.3/splashstand/scrap/food_establishment.yml
+-rw-r--r--   0        0        0      178 2024-03-23 12:44:54.799064 splashstand-3.0.3/splashstand/scrap/image_object.yml
+-rw-r--r--   0        0        0       95 2024-02-04 19:39:55.435562 splashstand-3.0.3/splashstand/scrap/intangible/_defined_term.yml
+-rw-r--r--   0        0        0       75 2024-01-23 22:25:16.758548 splashstand-3.0.3/splashstand/scrap/intangible/category_code.yml
+-rw-r--r--   0        0        0      310 2024-01-28 11:14:17.459275 splashstand-3.0.3/splashstand/scrap/intangible/contact_point/_base.yml
+-rw-r--r--   0        0        0      199 2024-01-28 11:15:36.772150 splashstand-3.0.3/splashstand/scrap/intangible/contact_point/postal_address.yml
+-rw-r--r--   0        0        0      112 2024-02-02 10:15:54.007731 splashstand-3.0.3/splashstand/scrap/intangible/offer.yml
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:27.535462 splashstand-3.0.3/splashstand/scrap/intangible/price_specification.yml
+-rw-r--r--   0        0        0      128 2024-01-28 11:29:46.704013 splashstand-3.0.3/splashstand/scrap/intangible/quantitative_value.yml
+-rw-r--r--   0        0        0      625 2024-03-17 10:15:21.961766 splashstand-3.0.3/splashstand/scrap/intangible/schedule.yml
+-rw-r--r--   0        0        0      221 2024-03-17 10:15:28.105212 splashstand-3.0.3/splashstand/scrap/intangible/type_and_quantity_node.yml
+-rw-r--r--   0        0        0      290 2024-01-23 21:08:22.676063 splashstand-3.0.3/splashstand/scrap/lodging_business.yml
+-rw-r--r--   0        0        0      446 2024-03-16 12:10:03.074570 splashstand-3.0.3/splashstand/scrap/music_album.yml
+-rw-r--r--   0        0        0       12 2024-01-22 11:16:25.578830 splashstand-3.0.3/splashstand/scrap/music_event.yml
+-rw-r--r--   0        0        0       55 2024-03-18 08:12:43.387249 splashstand-3.0.3/splashstand/scrap/music_group.yml
+-rw-r--r--   0        0        0      194 2024-03-16 12:05:56.626542 splashstand-3.0.3/splashstand/scrap/music_playlist.yml
+-rw-r--r--   0        0        0      426 2024-03-16 09:46:20.886026 splashstand-3.0.3/splashstand/scrap/music_recording.yml
+-rw-r--r--   0        0        0        0 2024-01-23 21:08:22.665060 splashstand-3.0.3/splashstand/scrap/music_venue.yml
+-rw-r--r--   0        0        0        0 2024-01-24 12:41:27.932506 splashstand-3.0.3/splashstand/scrap/performing_group.yml
+-rw-r--r--   0        0        0       12 2024-01-24 12:41:27.932026 splashstand-3.0.3/splashstand/scrap/poster.yml
+-rw-r--r--   0        0        0      226 2024-02-04 19:39:55.432246 splashstand-3.0.3/splashstand/scrap/product/_base.yml
+-rw-r--r--   0        0        0       89 2024-01-23 22:15:32.819070 splashstand-3.0.3/splashstand/scrap/product/_product_collection.yml
+-rw-r--r--   0        0        0      150 2024-02-04 19:39:55.451041 splashstand-3.0.3/splashstand/scrap/product/_product_group.yml
+-rw-r--r--   0        0        0       82 2024-01-28 11:22:23.616248 splashstand-3.0.3/splashstand/scrap/product/_some_products.yml
+-rw-r--r--   0        0        0        0 2024-01-24 12:41:27.953199 splashstand-3.0.3/splashstand/scrap/theater_group.yml
+-rw-r--r--   0        0        0      329 2024-03-23 12:44:54.794787 splashstand-3.0.3/splashstand/scrap/video_object.yml
+-rw-r--r--   0        0        0      347 2024-05-19 18:39:05.642157 splashstand-3.0.3/splashstand/settings/adapters.yml
+-rw-r--r--   0        0        0       83 2024-05-19 18:39:32.020167 splashstand-3.0.3/splashstand/settings/admin.yml
+-rw-r--r--   0        0        0      126 2024-05-19 18:39:23.917780 splashstand-3.0.3/splashstand/settings/app.yml
+-rw-r--r--   0        0        0      115 2024-05-19 18:39:21.574574 splashstand-3.0.3/splashstand/settings/auth.yml
+-rw-r--r--   0        0        0      134 2024-05-19 18:39:08.360624 splashstand-3.0.3/splashstand/settings/cache.yml
+-rw-r--r--   0        0        0      346 2024-05-19 18:39:04.163362 splashstand-3.0.3/splashstand/settings/debug.yml
+-rw-r--r--   0        0        0       36 2024-05-19 18:39:04.661104 splashstand-3.0.3/splashstand/settings/logger.yml
+-rw-r--r--   0        0        0       27 2024-05-19 18:39:22.150700 splashstand-3.0.3/splashstand/settings/models.yml
+-rw-r--r--   0        0        0       32 2024-01-14 13:39:55.831734 splashstand-3.0.3/splashstand/settings/monitoring.yml
+-rw-r--r--   0        0        0       16 2024-02-09 10:05:07.028234 splashstand-3.0.3/splashstand/settings/requests.yml
+-rw-r--r--   0        0        0        3 2024-05-19 18:39:28.043259 splashstand-3.0.3/splashstand/settings/routes.yml
+-rw-r--r--   0        0        0        3 2024-05-19 18:39:09.045401 splashstand-3.0.3/splashstand/settings/schemas.yml
+-rw-r--r--   0        0        0       77 2024-05-19 18:39:28.551939 splashstand-3.0.3/splashstand/settings/sql.yml
+-rw-r--r--   0        0        0      164 2024-05-19 18:39:26.007689 splashstand-3.0.3/splashstand/settings/storage.yml
+-rw-r--r--   0        0        0       59 2024-05-19 18:39:27.727985 splashstand-3.0.3/splashstand/settings/templates.yml
+-rw-r--r--   0        0        0        0 2023-10-09 12:28:22.664820 splashstand-3.0.3/splashstand/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.468507 splashstand-3.0.3/splashstand/templates/admin/base/base.html.blah
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.465280 splashstand-3.0.3/splashstand/templates/admin/base/head.html.blah
+-rw-r--r--   0        0        0     3132 2024-01-24 12:41:27.952900 splashstand-3.0.3/splashstand/templates/admin/base/js/serviceworker.js
+-rw-r--r--   0        0        0     3362 2024-03-04 16:21:30.478428 splashstand-3.0.3/splashstand/templates/admin/base/tail.html.blah
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.430976 splashstand-3.0.3/splashstand/templates/admin/bulma/base.html.blah
+-rw-r--r--   0        0        0      301 2024-03-11 12:41:28.420083 splashstand-3.0.3/splashstand/templates/admin/bulma/blocks/display_menu.html
+-rw-r--r--   0        0        0     1127 2024-03-04 16:21:30.478801 splashstand-3.0.3/splashstand/templates/admin/bulma/blocks/menu_category.html
+-rw-r--r--   0        0        0      422 2024-03-04 16:21:30.466542 splashstand-3.0.3/splashstand/templates/admin/bulma/blocks/menu_item.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.384215 splashstand-3.0.3/splashstand/templates/admin/bulma/create.html.blah
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.378407 splashstand-3.0.3/splashstand/templates/admin/bulma/delete.html.blah
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.365228 splashstand-3.0.3/splashstand/templates/admin/bulma/details.html.blah
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.424290 splashstand-3.0.3/splashstand/templates/admin/bulma/edit.html.blah
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.411254 splashstand-3.0.3/splashstand/templates/admin/bulma/error.html.blah
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.400973 splashstand-3.0.3/splashstand/templates/admin/bulma/index.html.blah
+-rw-r--r--   0        0        0     1965 2024-04-15 14:32:35.783285 splashstand-3.0.3/splashstand/templates/admin/bulma/layout.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.417745 splashstand-3.0.3/splashstand/templates/admin/bulma/list.html.blah
+-rw-r--r--   0        0        0     2022 2024-03-04 16:21:30.464316 splashstand-3.0.3/splashstand/templates/admin/bulma/login.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.446452 splashstand-3.0.3/splashstand/templates/admin/bulma/scss/admin.scss
+-rw-r--r--   0        0        0    21368 2023-04-16 10:25:26.449863 splashstand-3.0.3/splashstand/templates/admin/bulma/scss/admin.yml
+-rw-r--r--   0        0        0     1676 2023-10-08 07:49:18.349781 splashstand-3.0.3/splashstand/templates/admin/old/actions.html
+-rw-r--r--   0        0        0     3670 2023-10-08 07:49:18.360195 splashstand-3.0.3/splashstand/templates/admin/old/analytics.html
+-rw-r--r--   0        0        0     1614 2023-10-08 07:49:18.356792 splashstand-3.0.3/splashstand/templates/admin/old/content.html
+-rw-r--r--   0        0        0     2401 2023-10-08 07:49:18.335133 splashstand-3.0.3/splashstand/templates/admin/old/details_modal.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.513578 splashstand-3.0.3/splashstand/templates/admin/old/edit_modal.html
+-rw-r--r--   0        0        0      174 2023-10-08 07:49:18.359010 splashstand-3.0.3/splashstand/templates/admin/old/help.html
+-rw-r--r--   0        0        0    12664 2023-04-29 15:04:31.101823 splashstand-3.0.3/splashstand/templates/admin/old/index.html
+-rw-r--r--   0        0        0     2505 2023-10-08 07:49:18.355106 splashstand-3.0.3/splashstand/templates/admin/old/layout.html
+-rw-r--r--   0        0        0    16475 2023-04-29 15:04:31.062084 splashstand-3.0.3/splashstand/templates/admin/old/lib.html
+-rw-r--r--   0        0        0    10563 2023-10-08 07:49:18.337642 splashstand-3.0.3/splashstand/templates/admin/old/list.html
+-rw-r--r--   0        0        0     2153 2023-10-08 07:49:18.329264 splashstand-3.0.3/splashstand/templates/admin/old/modal.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.530050 splashstand-3.0.3/splashstand/templates/admin/old/offline.html
+-rw-r--r--   0        0        0      174 2023-04-16 10:25:26.526789 splashstand-3.0.3/splashstand/templates/admin/old/preview.html
+-rw-r--r--   0        0        0      938 2023-10-08 07:49:18.337808 splashstand-3.0.3/splashstand/templates/admin/old/redis_console.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.485086 splashstand-3.0.3/splashstand/templates/admin/old/redis_response.html
+-rw-r--r--   0        0        0     1974 2023-10-08 07:49:18.360424 splashstand-3.0.3/splashstand/templates/admin/old/row_actions.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.516813 splashstand-3.0.3/splashstand/templates/admin/old/site_edit.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.543476 splashstand-3.0.3/splashstand/templates/admin/old/static.html
+-rw-r--r--   0        0        0    12313 2023-10-08 07:49:18.328464 splashstand-3.0.3/splashstand/templates/admin/old/storage_list.html
+-rw-r--r--   0        0        0      146 2023-04-16 10:25:26.552654 splashstand-3.0.3/splashstand/templates/admin/old/store.html
+-rw-r--r--   0        0        0      174 2023-10-08 07:49:18.355650 splashstand-3.0.3/splashstand/templates/admin/old/support.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.481539 splashstand-3.0.3/splashstand/templates/admin/old/theme_details_modal.html
+-rw-r--r--   0        0        0     5691 2023-10-08 07:49:18.359164 splashstand-3.0.3/splashstand/templates/admin/old/theme_edit.html
+-rw-r--r--   0        0        0     3774 2023-10-08 07:49:18.347873 splashstand-3.0.3/splashstand/templates/admin/old/theme_list.html
+-rw-r--r--   0        0        0      760 2024-03-03 13:26:30.340077 splashstand-3.0.3/splashstand/templates/app/base/base.html
+-rw-r--r--   0        0        0      211 2024-02-25 14:27:15.782831 splashstand-3.0.3/splashstand/templates/app/base/blocks/head.html
+-rw-r--r--   0        0        0     1365 2023-10-08 07:49:18.341683 splashstand-3.0.3/splashstand/templates/app/base/blocks/tail.html
+-rw-r--r--   0        0        0      102 2024-02-25 14:27:15.760110 splashstand-3.0.3/splashstand/templates/app/base/blocks/title.html
+-rw-r--r--   0        0        0     3828 2023-10-08 07:49:18.328317 splashstand-3.0.3/splashstand/templates/app/base/js/serviceworker.js
+-rw-r--r--   0        0        0      220 2023-04-16 10:25:26.330632 splashstand-3.0.3/splashstand/templates/app/base/robots.txt
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.325355 splashstand-3.0.3/splashstand/templates/app/base/sitemap.xml
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.319604 splashstand-3.0.3/splashstand/templates/app/base/sitemapindex.xml
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.686163 splashstand-3.0.3/splashstand/templates/app/bulma/about.html
+-rw-r--r--   0        0        0      433 2023-10-08 07:49:18.360585 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/components.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.615759 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/construction.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.608494 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/contact_image.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.619053 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/contact_map.html
+-rw-r--r--   0        0        0     4911 2023-10-08 07:49:18.355957 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/elements.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.636859 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/event_list.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.633950 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/event_past.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.630684 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/event_tile.html
+-rw-r--r--   0        0        0     1003 2023-04-16 10:25:26.676673 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/footer.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.695120 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/form.html
+-rw-r--r--   0        0        0     5353 2023-10-08 07:49:18.344167 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/header.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.669499 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/mailer.html
+-rw-r--r--   0        0        0     2944 2023-10-08 07:49:18.334587 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/nav.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.652459 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/news_list.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.647547 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/news_tile.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.612249 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/project_list.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.626778 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/quote_tile.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.643223 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/user_tile.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.622339 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/venue_list.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.683136 splashstand-3.0.3/splashstand/templates/app/bulma/blocks/video.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.666348 splashstand-3.0.3/splashstand/templates/app/bulma/contact.html
+-rw-r--r--   0        0        0       17 2024-02-25 14:27:15.758187 splashstand-3.0.3/splashstand/templates/app/bulma/events.html
+-rw-r--r--   0        0        0       33 2024-02-24 08:12:48.452202 splashstand-3.0.3/splashstand/templates/app/bulma/home.html
+-rw-r--r--   0        0        0      192 2024-02-25 14:27:15.739081 splashstand-3.0.3/splashstand/templates/app/bulma/index.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.663198 splashstand-3.0.3/splashstand/templates/app/bulma/offline.html
+-rw-r--r--   0        0        0     6731 2023-10-08 07:49:18.357156 splashstand-3.0.3/splashstand/templates/app/bulma/privacy_policy.html
+-rw-r--r--   0        0        0     6067 2024-02-24 08:12:48.459332 splashstand-3.0.3/splashstand/templates/app/bulma/service_terms.html
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.708359 splashstand-3.0.3/splashstand/templates/app/bulma/style/custom.scss
+-rw-r--r--   0        0        0    22109 2023-04-16 10:25:26.715204 splashstand-3.0.3/splashstand/templates/app/bulma/style/custom.yml
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.705086 splashstand-3.0.3/splashstand/templates/app/bulma/style/fender.scss
+-rw-r--r--   0        0        0    21435 2023-04-16 10:25:26.711727 splashstand-3.0.3/splashstand/templates/app/bulma/style/fender.yml
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.126798 splashstand-3.0.3/splashstand/tmp/migrations/README
+-rw-r--r--   0        0        0        0 2023-04-16 10:25:26.130056 splashstand-3.0.3/splashstand/tmp/migrations/env.py
+-rw-r--r--   0        0        0       43 2024-03-01 14:32:58.470182 splashstand-3.0.3/splashstand/tmp/secrets/app_secret_key
+-rw-r--r--   0        0        0       90 2024-03-01 14:32:58.553550 splashstand-3.0.3/splashstand/tmp/secrets/app_secure_salt
+-rw-r--r--   0        0        0       39 2024-03-01 14:33:00.066684 splashstand-3.0.3/splashstand/tmp/secrets/auth_api_key
+-rw-r--r--   0        0        0        9 2024-03-01 14:32:59.642793 splashstand-3.0.3/splashstand/tmp/secrets/cache_host
+-rw-r--r--   0        0        0       13 2024-03-01 14:32:59.719065 splashstand-3.0.3/splashstand/tmp/secrets/cache_password
+-rw-r--r--   0        0        0        9 2024-03-01 14:33:04.722909 splashstand-3.0.3/splashstand/tmp/secrets/sql_host
+-rw-r--r--   0        0        0       11 2024-03-01 14:33:04.846091 splashstand-3.0.3/splashstand/tmp/secrets/sql_password
+-rw-r--r--   0        0        0        4 2024-03-01 14:33:04.792665 splashstand-3.0.3/splashstand/tmp/secrets/sql_user
+-rw-r--r--   0        0        0        0 2020-05-30 12:35:52.000000 splashstand-3.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 splashstand-3.0.3/PKG-INFO
```

### Comparing `splashstand-3.0.2/LICENSE` & `splashstand-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/bin/checkversions.py` & `splashstand-3.0.3/bin/checkversions.py`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/bin/deploy/upgrade.py` & `splashstand-3.0.3/bin/deploy/upgrade.py`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/bin/startproject.py` & `splashstand-3.0.3/bin/startproject.py`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/bin/upgradeproject.py` & `splashstand-3.0.3/bin/upgradeproject.py`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/pyproject.toml` & `splashstand-3.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "SplashStand"
-version = "3.0.2"
+version = "3.0.3"
 description = ""
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
@@ -76,31 +76,36 @@
 config = [
     "python.use_venv",
     "true",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "crackerjack>=0.7.6",
     "watchfiles>=0.20.0",
     "ipython>=8.16.1",
     "-e file:///${PROJECT_ROOT}/../schemaorg-lite#egg=schemaorg-lite",
     "-e file:///${PROJECT_ROOT}/../fastblocks#egg=fastblocks[admin,auth,sitemap,style]",
     "-e file:///${PROJECT_ROOT}/../starlette-async-jinja#egg=starlette-async-jinja",
     "-e file:///${PROJECT_ROOT}/../jinja2-async-environment#egg=jinja2-async-environment",
     "-e file:///${PROJECT_ROOT}/../acb#egg=acb[cache,requests,secret,sql,storage]",
+    "-e file:///${PROJECT_ROOT}/../crackerjack#egg=Crackerjack",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py312"
 fix = true
 show-fixes = true
 output-format = "full"
 
+[tool.ruff.lint]
+ignore = [
+    "F821",
+]
+
 [tool.ruff.lint.isort]
 force-single-line = true
 
 [tool.ruff.lint.mccabe]
 max-complexity = 10
 
 [tool.ruff.lint.pydocstyle]
@@ -113,41 +118,41 @@
 
 [tool.creosote]
 paths = [
     "splashstand",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "pdm",
-    "phonenumbers",
-    "starlette-decorouter",
+    "pytest",
+    "pyfiglet",
     "libsass",
+    "starlette-decorouter",
+    "pdm",
+    "uuid-utils",
     "autotyping",
-    "pyfiglet",
-    "pytest",
-    "pdm-bump",
     "pre-commit",
-    "jinja2-inflection",
+    "pdm-bump",
     "jinja2-arrow",
-    "uuid-utils",
+    "phonenumbers",
+    "jinja2-inflection",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "splashstand",
 ]
 skips = [
-    "B403",
-    "B603",
     "B404",
     "B102",
     "B113",
+    "B603",
+    "B403",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "splashstand",
 ]
```

### Comparing `splashstand-3.0.2/splashstand/adapters/admin/_manifest.py` & `splashstand-3.0.3/splashstand/adapters/admin/_manifest.py`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/adapters/admin/sqladmin.py` & `splashstand-3.0.3/splashstand/adapters/admin/sqladmin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,56 @@
 import re
 import typing as t
 from contextlib import suppress
-from copy import deepcopy
 from datetime import datetime
 from datetime import timedelta
 
 import uuid_utils as uuid
 from acb.actions.encode import load
 from acb.adapters import import_adapter
 from acb.config import Config
 from acb.debug import debug
 from acb.depends import depends
 from aiopath import AsyncPath
-from fastblocks import current_user
-
-# from asgi_htmx import HtmxRequest
 from fastblocks import FastBlocks
 from google.oauth2.service_account import Credentials
 from inflection import camelize
 from inflection import pluralize
 from inflection import titleize
 from inflection import underscore
 from markupsafe import Markup
 from pydantic import AnyUrl
-from splashstand.adapters.models.main import schema_registry
+from pydantic import EmailStr
 from sqladmin import Admin as SqlAdmin
 from sqladmin import expose
 from sqladmin.authentication import login_required  # type: ignore
 from sqladmin.helpers import get_object_identifier  # type: ignore
 from sqladmin.models import ModelView  # type: ignore
 from sqlmodel import select
-
-# from sqlmodel import select  # type: ignore
 from sqlmodel import SQLModel
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.responses import RedirectResponse
 from starlette.responses import Response
 from starlette_async_jinja import AsyncJinja2Templates
 from starlette_async_jinja import JsonResponse
-from wtforms.validators import DataRequired  # type: ignore
 from ._base import AdminBase
 from ._base import AdminBaseSettings
 
 # from wtforms.fields import TextAreaField
 # from wtforms.widgets import TextArea
 # from wtforms.fields.datetime import DateTimeField
 
 
 Logger = import_adapter()
 Models = import_adapter()
 Templates = import_adapter()
 Storage = import_adapter()
+Schemas = import_adapter()
+Auth = import_adapter()
 Sql = import_adapter()
 
 
 class AdminSettings(AdminBaseSettings):
     title: str = "SplashStand Dashboard"
     style: str = "bulma"
     theme: str = "light"
@@ -129,38 +124,51 @@
 
 
 class Admin(AdminBase, SqlAdmin):  # type: ignore
     def __init__(self, app: Starlette = FastBlocks(), **kwargs: t.Any) -> None:
         super().__init__(app, **kwargs)
 
     @depends.inject
-    async def init(
+    async def create_user(
         self,
+        name: str,
+        gmail: EmailStr,
+        is_superuser: bool = False,
+        role: str = "user",
         models: Models = depends(),  # type: ignore
+        **kwargs: str,
     ) -> None:
-        try:
-            person = models.Person
-            admin_user = await person.query()
-            if not len(admin_user):
-                self.logger.debug("Creating admin superuser...")
-                await models.create_user(
-                    gmail=self.config.admin.gmail,
-                    is_superuser=True,
-                    role="admin",
+        user = getattr(models.sql, "Person")(
+            name=name, gmail=gmail, is_superuser=is_superuser, role=role, **kwargs
+        )
+        debug(user)
+        await user.save()
+
+    @depends.inject
+    async def init(self, models: Models = depends()) -> None:  # type: ignore
+        admin_user = (
+            await models.sql.Person.query(
+                "Person.role == 'admin'", f"Person.gmail == '{self.config.admin.gmail}'"
+            )
+        ).first()
+        if admin_user is None:
+            self.logger.debug("Creating admin superuser...")
+            await self.create_user(
+                name="Default Admin",
+                gmail=self.config.admin.gmail,
+                is_superuser=True,
+                role="admin",
+            )
+            admin_user = (
+                await models.sql.Person.query(
+                    "Person.role == 'admin'",
+                    f"Person.gmail == '{self.config.admin.gmail}'",
                 )
-                admin_user = await person.query()
-            for k, v in vars(admin_user[0]).items():
-                debug(k, v)
-        except Exception as e:
-            self.logger.exception(e)
-
-        for model in [m for m in vars(models).values() if issubclass(m, SQLModel)]:
-            debug(model)
-            # self.add_view(await self.create_view(model))
-            self.logger.debug(f"Created {model.__name__} admin view")
+            ).one()
+        debug(admin_user)
 
     @depends.inject
     @t.override
     def init_templating_engine(
         self, templates: Templates = depends()  # type: ignore
     ) -> AsyncJinja2Templates:
         admin_templates = templates.admin
@@ -170,14 +178,18 @@
             admin=self,
             is_list=lambda x: isinstance(x, list),  # type: ignore
             get_object_identifier=get_object_identifier,
         )
         admin_templates.env.globals.update(admin_templates_env_globals)
         return admin_templates
 
+    @login_required
+    async def index(self, request: Request) -> Response:
+        return await self.templates.TemplateResponse(request, "index.html")
+
     @t.override
     async def login(  # type: ignore
         self, request: Request
     ) -> t.Coroutine[t.Any, t.Any, t.Any] | RedirectResponse | None:
         if self.authentication_backend:
             context = {}
             ok = await self.authentication_backend.login(request)
@@ -273,256 +285,271 @@
         resp = JsonResponse(
             content=admin_manifest.model_dump_json(), media_type="application/xml"
         )
         resp.headers["Content-Type"] = "application/json"
         resp.headers["Cache-Control"] = "max-age=4200, no-cache, must-revalidate"
         return resp
 
-    @depends.inject
-    def get_file_input(
-        self, field: t.Any, storage: Storage = depends()  # type: ignore
-    ) -> str:
-        if field.data and isinstance(field.data, str):
-            cloud_fn = storage.media.get_url(field.data)
-            # unique_id = field.data.split('.')[0]
-            # if field.name == "image":
-            #     cloud_fn = stor.media.get_url(resize(field.data, "240x", fit=1))
-            html = (
-                '<input id="{0}" name="{0}" type="file" '
-                'class="file-upload-input" value="{1}" src="{2}"/>'.format(
-                    field.name, field.data, cloud_fn
-                )
-            )
-        else:
-            html = (
-                '<input id="{0}" name="{0}" '
-                'class="file-upload-input" type="file">'.format(field.name)
-            )
-        return Markup(html)
 
-    @depends.inject
-    def _list_video_thumbnail(
-        self, model: SQLModel, storage: Storage = depends()  # type: ignore
-    ) -> Markup | str:
-        if model.video:
-            input_id = model.video.split(".")[0]
-            video_type = model.video.split(".")[1]
-            return Markup(
-                '<video width="" height="" controls>'
-                '<source src="{}" type="video/{}" '
-                'preload="metadata" id="video-{}">'
-                "Your browser does not support the video tag."
-                "</video>".format(
-                    storage.media.get_url(model.video), video_type, input_id
-                )
+depends.set(Admin)
+
+
+@depends.inject
+def get_file_input(field: t.Any, storage: Storage = depends()) -> str:  # type: ignore
+    if field.data and isinstance(field.data, str):
+        cloud_fn = storage.media.get_url(field.data)
+        # unique_id = field.data.split('.')[0]
+        # if field.name == "image":
+        #     cloud_fn = stor.media.get_url(resize(field.data, "240x", fit=1))
+        html = (
+            '<input id="{0}" name="{0}" type="file" '
+            'class="file-upload-input" value="{1}" src="{2}"/>'.format(
+                field.name, field.data, cloud_fn
             )
-        elif "youtube_id" in vars(model):
-            if model.youtube_id and not model.video:
-                return Markup(
-                    '<div class="youtube-iframe" '
-                    'style="position:relative;padding-top:56.25%;">'
-                    '<iframe width="" height="" '
-                    'src="https://www.youtube.com/embed/{0}" '
-                    'frameborder="0" allowfullscreen '
-                    'style="position:absolute;top:0;left:0;width:100%;height:100%;" '
-                    'id="youtube-{0}">'
-                    "</iframe>"
-                    "</div>"
-                ).format(model.youtube_id)
-        return ""
+        )
+    else:
+        html = (
+            '<input id="{0}" name="{0}" '
+            'class="file-upload-input" type="file">'.format(field.name)
+        )
+    return Markup(html)
 
-    def _list_image_thumbnail(self, model: SQLModel) -> str | Markup:
-        image = None
-        try:
-            image = model.image
-        except AttributeError:
-            try:
-                image = model.photo
-            except AttributeError:
-                with suppress(AttributeError):
-                    image = model.picture
-        if not image:
-            if "video" in vars(model):
-                return self._list_video_thumbnail(model)
-            return ""
-        input_id = image.split(".")[0]
-        # thumb = resize(image, "x240", fit=1)
+
+@depends.inject
+def _list_video_thumbnail(
+    model: SQLModel, storage: Storage = depends()  # type: ignore
+) -> Markup | str:
+    if model.video:
+        input_id = model.video.split(".")[0]
+        video_type = model.video.split(".")[1]
         return Markup(
-            '<a class="image-popup-link" href="{}"><img '
-            'id="image-{}" class="list-image" src="{}" />'
-            "</a>".format(model.image.url, input_id, model.image.thumbnail_url)
+            '<video width="" height="" controls>'
+            '<source src="{}" type="video/{}" '
+            'preload="metadata" id="video-{}">'
+            "Your browser does not support the video tag."
+            "</video>".format(storage.media.get_url(model.video), video_type, input_id)
         )
+    elif (
+        "youtube_id" in vars(model) and getattr(model, "youtube_id") and not model.video
+    ):
+        return Markup(
+            '<div class="youtube-iframe" '
+            'style="position:relative;padding-top:56.25%;">'
+            '<iframe width="" height="" '
+            'src="https://www.youtube.com/embed/{0}" '
+            'frameborder="0" allowfullscreen '
+            'style="position:absolute;top:0;left:0;width:100%;height:100%;" '
+            'id="youtube-{0}">'
+            "</iframe>"
+            "</div>"
+        ).format(model.youtube_id)
+    return ""
+
+
+def _list_image_thumbnail(model: SQLModel) -> str | Markup:
+    image = None
+    try:
+        image = model.image
+    except AttributeError:
+        try:
+            image = model.photo
+        except AttributeError:
+            with suppress(AttributeError):
+                image = model.picture
+    if not image:
+        if "video" in vars(model):
+            return _list_video_thumbnail(model)
+        return ""
+    input_id = image.split(".")[0]
+    # thumb = resize(image, "x240", fit=1)
+    return Markup(
+        '<a class="image-popup-link" href="{}"><img '
+        'id="image-{}" class="list-image" src="{}" />'
+        "</a>".format(model.image.url, input_id, model.image.thumbnail_url)
+    )
 
-    @depends.inject
-    async def create_view(
-        self,
-        app_model: type[SQLModel],
-        config: Config = depends(),  # type: ignore
-    ) -> t.Any:  # type: ignore
-        last_fields = [
-            "visible",
-            "maintainer",
-            "editor",
-            "date_created",
-            "date_modified",
-        ]
 
-        first_fields = [
+@depends.inject
+async def create_view(
+    app_model: type[SQLModel],
+    schemas: Schemas = depends(),  # type: ignore
+    config: Config = depends(),  # type: ignore
+) -> t.Any:  # type: ignore
+
+    last_fields = ["visible", "maintainer", "editor", "date_created", "date_modified"]
+
+    schema = getattr(schemas, underscore(app_model.__name__))
+
+    first_fields = [f for f in app_model.model_fields if f in schemas.thing._properties]
+
+    _fields = app_model.model_fields | app_model.__sqlmodel_relationships__
+    debug(schema._properties)
+    debug(len(schema._properties))
+    debug(schema._types)
+    # debug(schema._fields)
+    # debug(len(schema._fields))
+    clip = getattr(schema, "clip", None)
+    if clip:
+        debug(clip._fields)
+
+    class cls(ModelView, model=app_model):  # type: ignore
+        form_columns = [
             f
-            for f in list(schema_registry.get()["thing"].fields.keys())
-            if f != "visible"
+            for f in _fields
+            if f in schema._properties
+            and f not in first_fields
+            and f not in last_fields
         ]
 
-        class cls(ModelView, model=app_model):  # type: ignore
-            _fields: dict[str, t.Any] = app_model.__model_fields__
+        column_details_list = first_fields + form_columns + last_fields
 
-            def is_accessible(self, request: Request) -> bool:
-                return current_user.get().is_superuser
+        form_columns = first_fields + form_columns + [last_fields[0]]
 
-            def is_visible(self, request: Request) -> bool:
-                return True
-
-            @depends.inject
-            async def get_entries(
-                self, model: SQLModel, sql: Sql = depends()  # type: ignore
-            ) -> list[t.Any]:
-                async with sql.async_session() as session:
-                    entries_query = select(model)  # type: ignore
-                    result = await session.execute(entries_query)
-                    return result.all()
-
-            async def after_model_change(
-                self,
-                data: dict[str, t.Any],
-                model: t.Any,
-                is_created: bool,
-                request: Request,
-            ) -> None:
-                if is_created:
-                    entries = await self.get_entries(model)
-                    with suppress(AttributeError):
-                        for entry in entries:
-                            if entry.position == 99999:
-                                entry.position = 1
-                            else:
-                                entry.position = entry.position + 1
-                            entry.save()
-
-            async def after_model_delete(self, model: t.Any, request: Request) -> None:
+        @depends.inject
+        def is_accessible(
+            self, request: Request, auth: Auth = depends()  # type: ignore
+        ) -> bool:  # type: ignore
+            return auth.current_user.is_authenticated
+
+        def is_visible(self, request: Request) -> bool:
+            return True
+
+        @depends.inject
+        async def get_entries(
+            self, model: SQLModel, sql: Sql = depends()  # type: ignore
+        ) -> list[t.Any]:
+            async with sql.async_session() as session:
+                entries_query = select(model)  # type: ignore
+                result = await session.execute(entries_query)
+                return result.all()
+
+        async def after_model_change(
+            self,
+            data: dict[str, t.Any],
+            model: t.Any,
+            is_created: bool,
+            request: Request,
+        ) -> None:
+            if is_created:
+                entries = await self.get_entries(model)
                 with suppress(AttributeError):
-                    rm_position = model.position
-                    entries = await self.get_entries(model)
                     for entry in entries:
-                        if entry.position > rm_position:
-                            entry.position = entry.position - 1
-                            # entry.save()
-
-            async def on_model_change(
-                self,
-                data: dict[str, t.Any],
-                model: t.Any,
-                is_created: bool,
-                request: Request,
-            ) -> None:
-                if "youtube_id" in vars(model) and model.youtube_id:
-                    for prefix in (
-                        "https://youtu.be/",
-                        "http://youtu.be/",
-                        "https://www.youtube.com/watch?v=",
-                        "http://www.youtube.com/watch?v=",
-                    ):
-                        model.youtube_id = model.youtube_id.lstrip(prefix)
-                    pattern = r"[&,?]t=(\d+)"
-                    start = re.search(pattern, model.youtube_id)
-                    if start and ((not model.start) or model.start == "00:00:00"):
-                        model.start = timedelta(seconds=int(start.group(1)))
-                    pattern = r"[&,?]t=(\d+).*"
-                    model.youtube_id = re.sub(pattern, "", model.youtube_id)
-                if "spotify_id" in vars(model) and model.spotify_id:
-                    ...
-                if "archive_id" in vars(model) and model.archive_id:
-                    ...
-                if "soundcloud_id" in vars(model) and model.soundcloud_id:
-                    ...
-                if "bandcamp_id" in vars(model) and model.bandcamp_id:
-                    ...
-
-            @staticmethod
-            def _datetime_format(value: datetime) -> str:
-                # return value.strftime('%m-%d-%Y %I:%M %p')
-                # return value.strftime('%a %b %w, %Y - %I:%M %p')
-                return value.strftime("%a %b %d, %Y - %I:%M %p")
-                # return value.strftime('%a %b %d, %Y')
-
-            # column_type_formatters: dict[str, t.Any] = dict(
-            #     ModelView.column_type_formatters, date=_datetime_format
-            # )
-
-            column_formatters = {  # type: ignore
-                app_model.image: self._list_image_thumbnail,
-                app_model.picture: self._list_image_thumbnail,
-                app_model.photo: self._list_image_thumbnail,
-                app_model.video: self._list_video_thumbnail,
-            }
-
-            page_size = 25
-            page_size_options = [25, 50, 100, 200]
-            can_delete = True
-            details_template = "details.html"
-            list_template = "list.html"
-            form_include_pk = False
-            form_args = {}
-            form_columns = list(_fields.keys())
-            form_columns.remove("id")
-            form_columns = [
-                f for f in form_columns if f not in last_fields + first_fields
-            ]
-            form_columns = first_fields + form_columns
-            column_details_list = deepcopy(form_columns)
-            form_columns.append("visible")
-            # form_widget_args = dict(uid=dict(readonly=True))
-            # if not current_user.get().has_role(
-            #     "admin"
-            # ) or not current_user.get().has_role("owner"):
-            #     form_widget_args.gmail = dict(readonly=True)
-            for name, field in _fields.items():  # noqa: FURB135
-                if field.alias != field.name:
-                    key_name = name.removesuffix("_pk")
-                form_kwargs = dict(label=titleize(field.alias.removesuffix("_pk")))
-                if field.required:
-                    form_kwargs["validators"] = [DataRequired()]  # type: ignore
-                form_args[name] = form_kwargs
-            column_list = ["name"]
-            if "position" in list(_fields.keys()):
-                column_list.remove("position")
-                column_default_sort = "position"
-                column_sortable_list = ["position"]
-                column_list.append("position")
-            elif "published" in _fields:
-                column_default_sort = ("published", True)
-            elif "date" in _fields:
-                column_default_sort = "date"
-            else:
-                column_default_sort = "name"
-                column_sortable_list = ["name"]
-            column_details_list.extend(last_fields)
-
-        cls.__name__ = f"{app_model.__name__}Admin"
-        cls.name = titleize(app_model._alias or cls.name)
-        cls.name_plural = pluralize(cls.name)
-        cls.icon = f"fa-solid fa-{config.admin.icons[underscore(cls.name)]}"
-        debug(cls.__name__)
-        debug(vars(cls))
-        debug(cls.column_list)
-        debug(cls.form_columns)
-        debug(cls.column_details_list)
-        return cls
+                        if entry.position == 99999:
+                            entry.position = 1
+                        else:
+                            entry.position = entry.position + 1
+                        entry.save()
+
+        async def after_model_delete(self, model: t.Any, request: Request) -> None:
+            with suppress(AttributeError):
+                rm_position = model.position
+                entries = await self.get_entries(model)
+                for entry in entries:
+                    if entry.position > rm_position:
+                        entry.position = entry.position - 1
+                        entry.save()
+
+        async def on_model_change(
+            self,
+            data: dict[str, t.Any],
+            model: t.Any,
+            is_created: bool,
+            request: Request,
+        ) -> None:
+            if "youtube_id" in vars(model) and model.youtube_id:
+                for prefix in (
+                    "https://youtu.be/",
+                    "http://youtu.be/",
+                    "https://www.youtube.com/watch?v=",
+                    "http://www.youtube.com/watch?v=",
+                ):
+                    model.youtube_id = model.youtube_id.lstrip(prefix)
+                pattern = r"[&,?]t=(\d+)"
+                start = re.search(pattern, model.youtube_id)
+                if start and ((not model.start) or model.start == "00:00:00"):
+                    model.start = timedelta(seconds=int(start.group(1)))
+                pattern = r"[&,?]t=(\d+).*"
+                model.youtube_id = re.sub(pattern, "", model.youtube_id)
+            if "spotify_id" in vars(model) and model.spotify_id:
+                ...
+            if "archive_id" in vars(model) and model.archive_id:
+                ...
+            if "soundcloud_id" in vars(model) and model.soundcloud_id:
+                ...
+            if "bandcamp_id" in vars(model) and model.bandcamp_id:
+                ...
+
+        @staticmethod
+        def _datetime_format(value: datetime) -> str:
+            return value.strftime("%a %b %d, %Y - %I:%M %p")
+
+        column_type_formatters = dict(
+            date=_datetime_format,
+            image=_list_image_thumbnail,
+            picture=_list_image_thumbnail,
+            photo=_list_image_thumbnail,
+            video=_list_video_thumbnail,
+        )
 
+        is_async = True
+        page_size = 25
+        page_size_options = [25, 50, 100, 200]
+        can_delete = True
+        details_template = "details.html"
+        list_template = "list.html"
+
+        form_widget_args = dict(
+            google_uid=dict(readonly=True), picture=dict(readonly=True)
+        )
+
+        # if not current_user().has_role("admin") or not current_user().has_role("owner"):
+        #     form_widget_args.gmail = dict(readonly=True)
+        #     form_widget_args.role = dict(readonly=True)
+
+        form_args = {}
+
+        # column_details_list = deepcopy(form_columns)
+
+        # for name, field in _fields.items():  # noqa: FURB135
+        #     form_kwargs = dict(
+        #         label=titleize(
+        #             field.alias or name.removesuffix("_id").removesuffix("_object")
+        #         )
+        #     )
+        #     if hasattr(field, "required"):
+        #         form_kwargs["validators"] = [DataRequired()]  # type: ignore
+        #     form_args[name] = form_kwargs
+        column_list = ["name"]
+        if "position" in _fields:
+            column_list.remove("position")
+            column_default_sort = "position"
+            column_sortable_list = ["position"]
+            column_list.append("position")
+        elif "published" in _fields:
+            column_default_sort = ("published", True)
+        elif "date" in _fields:
+            column_default_sort = "date"
+        else:
+            column_default_sort = "name"
+            column_sortable_list = ["name"]
+        # column_details_list.extend(last_fields)
+
+    cls.__name__ = f"{app_model.__name__}Admin"
+    # cls.name = titleize(app_model.alias or app_model.__name__)
+    cls.name = titleize(app_model.__name__)
+    cls.name_plural = pluralize(cls.name)
+    # cls.icon = f"fa-solid fa-{config.admin.icons[underscore(cls.name)]}"
+    debug(cls.__name__)
+    debug(cls.name)
+    debug(cls.name_plural)
+    debug(cls.form_columns)
+    debug(cls.column_list)
+    debug(cls.column_details_list)
+    return cls
 
-depends.set(Admin)
 
 #
 #
 # class CustomView(BaseView):
 #     name = "Custom Page"
 #     icon = "fa-chart-line"
 #
```

### Comparing `splashstand-3.0.2/splashstand/adapters/analytics/google.py` & `splashstand-3.0.3/splashstand/adapters/analytics/google.py`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/adapters/app/_manifest.py` & `splashstand-3.0.3/splashstand/adapters/app/_manifest.py`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/adapters/app/demo.py` & `splashstand-3.0.3/splashstand/adapters/app/demo.py`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/adapters/app/main.py` & `splashstand-3.0.3/splashstand/adapters/app/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,41 +4,40 @@
 
 from acb.adapters import get_adapter
 from acb.adapters import import_adapter
 from acb.config import Config
 from acb.debug import debug
 from acb.depends import depends
 from fastblocks.applications import FastBlocks
+from sqlmodel import SQLModel
 from ._base import AppBase
 from ._base import AppBaseSettings
 
 main_start = perf_counter()
 
 Logger = import_adapter()
 Cache = import_adapter()
+Schemas = import_adapter()
 Auth = import_adapter()
+Models = import_adapter()
 
 
 class AppSettings(AppBaseSettings):
     pwa_name: str = "SplashStand"
     store_enabled: bool = False
     fontawesome_pro: bool = True
     ios_id: t.Optional[str] = None
     datetime_format: str = "MM-DD-YYYY h:mm A"
     about: str = (
         "SplashStand is a fast, simple, safe, and secure content management system."
     )
     social_media: list[str] = []
     favicon: str = "favicon.ico"
     icon: str = "icon.png"
-    contact: dict[str, str] = dict(
-        email="",
-        phone="",
-        address="",
-    )
+    contact: dict[str, str] = dict(email="", phone="", address="")
     copyright: t.Optional[str] = None
     theme_color: str = "fff"
     bgcolor: str = "fff"
     permanent_session_lifetime: int = 2_678_400
     wtf_csrf_time_limit: int = 172_800
     roles: list[str] = ["admin", "owner", "contributor", "user"]
     media_types: list[str] = ["image", "video", "audio"]
@@ -75,16 +74,15 @@
             ("2048x2732", "1024", "1366", "2"),
             ("1668x2388", "834", "1194", "2"),
             ("1668x2224", "834", "1112", "2"),
             ("1536x2048", "768", "1024", "2"),
         ),
     )
     header: dict[str, tuple[str]] = dict(
-        dimensions=("1920x1080",),
-        logo_dimensions=("1024x240",),
+        dimensions=("1920x1080",), logo_dimensions=("1024x240",)
     )
     notification_icons: dict[str, str] = dict(
         info="info-circle",
         success="check-circle",
         danger="exclamation-circle",
         warning="exclamation-triangle",
     )
@@ -108,35 +106,49 @@
     @asynccontextmanager
     @depends.inject
     async def lifespan(
         self,
         app: FastBlocks,
         cache: Cache = depends(),  # type: ignore
         auth: Auth = depends(),  # type: ignore
+        models: Models = depends(),  # type: ignore
     ) -> t.AsyncGenerator[None, None]:
-        if not self.config.deployed and not self.config.debug.production:
+        if (
+            not self.config.deployed
+            and self.config.debug.cache
+            and not self.config.debug.production
+        ):
             await cache.delete_match("*")
 
         if get_adapter("admin").enabled:
             admin = depends.get(import_adapter("admin"))
             admin.__init__(
                 app,
                 engine=depends.get(import_adapter("sql")).engine,
                 title=self.config.admin.title,
                 debug=self.config.debug.admin,
                 base_url=self.config.admin.url,
                 logo_url=self.config.admin.logo_url,
                 authentication_backend=auth,
             )
-            for v in admin.templates.env.loader.searchpath:
-                debug(v)
+            # for v in admin.templates.env.loader.searchpath:
+            #     debug(v)
+            debug([v for v in vars(models.sql).values() if issubclass(v, SQLModel)])
+            from ..admin.sqladmin import create_view
+
+            for model in [
+                m for m in vars(models.sql).values() if issubclass(m, SQLModel)
+            ]:
+                debug(model)
+                admin.add_view(await create_view(model))
+                self.logger.debug(f"Created {model.__name__} admin view")
             self.router.routes.insert(0, self.router.routes.pop())
 
-        for route in self.routes:
-            debug(route)
+        # for route in self.routes:
+        #     debug(route)
 
         async def post_startup() -> None:
             if not self.config.deployed:
                 from aioconsole import aprint
                 from pyfiglet import Figlet
 
                 fig = Figlet(font="slant", width=90, justify="center")
```

### Comparing `splashstand-3.0.2/splashstand/adapters/auth/_base.py` & `splashstand-3.0.3/splashstand/adapters/auth/_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 import typing as t
 from abc import ABC
 from abc import abstractmethod
+from contextvars import ContextVar
 
 from acb.config import Settings
 from pydantic import EmailStr
 from acb.adapters import AdapterBase
 from pydantic import SecretStr
 from sqlmodel import SQLModel
 from starlette.requests import Request
+from starlette.authentication import UnauthenticatedUser
 
 
 class AuthBaseSettings(Settings):
     token_id: t.Optional[str] = None
     session_cookie: t.Optional[str] = None
 
 
 class AuthBase(AdapterBase, ABC):
-    @staticmethod
+    _current_user: ContextVar[t.Any] = ContextVar(
+        "current_user", default=UnauthenticatedUser()
+    )
+
+    @property
+    def current_user(self) -> t.Any:
+        return self._current_user.get()
+
     @abstractmethod
-    async def authenticate(request: Request) -> bool:
+    async def authenticate(self, request: Request) -> bool:
         raise NotImplementedError
 
     @abstractmethod
     def __init__(self, secret_key: SecretStr, user_model: SQLModel) -> None:
         raise NotImplementedError
 
     @abstractmethod
```

### Comparing `splashstand-3.0.2/splashstand/adapters/auth/firebase.py` & `splashstand-3.0.3/splashstand/adapters/auth/firebase.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from datetime import timedelta
 from time import time
 
 from acb.adapters import import_adapter
 from acb.config import Config
 from acb.debug import debug
 from acb.depends import depends
-from fastblocks import current_user
 from firebase_admin import auth
 from firebase_admin import initialize_app
 from google.auth.transport import requests as google_requests
 from pydantic import EmailStr
 from pydantic import SecretStr
 from sqlmodel import select  # type: ignore
 from sqlmodel import SQLModel
@@ -23,25 +22,28 @@
 from ._base import AuthBaseSettings
 from ._base import AuthBaseUser
 
 firebase_request_adapter: google_requests.Request = google_requests.Request()
 firebase_app: t.Any = None
 
 
+@depends.inject
+def get_token(config: Config = depends()) -> str:
+    return f"_ss_{b64encode(config.app.name.encode()).decode().rstrip('=')}"
+
+
 class AuthSettings(AuthBaseSettings):
     api_key: SecretStr = SecretStr("")
     app_id: str = ""
     messaging_sender_id: str = ""
 
     @depends.inject
     def __init__(self, config: Config = depends(), **data: t.Any) -> None:
         super().__init__(**data)
-        self.token_id = (
-            f"_ss_{b64encode(config.app.name.encode()).decode().rstrip('=')}"
-        )
+        self.token_id = get_token()
 
 
 class CurrentUser(AuthBaseUser):
     user_data: t.Any = {}
 
     def has_role(self, role: str) -> str:
         return self.user_data.custom_claims.get(role)
@@ -70,110 +72,108 @@
         self, request: Request | None, config: Config = depends()
     ) -> bool | str:
         if request:
             with suppress(
                 auth.ExpiredIdTokenError,
                 auth.RevokedIdTokenError,
                 auth.InvalidIdTokenError,
+                auth.ExpiredSessionCookieError,
             ):
                 session_cookie = request.session.get(config.auth.token_id)
                 if session_cookie:
                     self.user_data = auth.verify_session_cookie(
                         session_cookie, check_revoked=True
                     )
         return self.identity or False
 
 
-current_user.set(CurrentUser())
-
-
 class Auth(AuthBase):
     @depends.inject
     def __init__(
         self,
         secret_key: t.Optional[SecretStr] = None,
         user_model: t.Optional[SQLModel] = None,
     ) -> None:
         self.secret_key = secret_key or self.config.app.secret_key
         self.middlewares = [
             Middleware(
                 SessionMiddleware,  # type: ignore
                 secret_key=self.secret_key.get_secret_value(),
-                session_cookie=f"{self.config.app.name}_dash",
+                session_cookie=f"{get_token()}_admin",
                 https_only=True if self.config.deployed else False,
             )
         ]
         self.name = "firebase"
         self.user_model = user_model
+        self._current_user.set(CurrentUser())
 
     async def init(self) -> None:
         global firebase_app
         firebase_options: dict[str, str] = dict(projectId=self.config.app.project)
         firebase_app = initialize_app(options=firebase_options.copy())
 
     async def login(self, request: Request) -> bool:
         id_token = request.cookies.get(self.config.auth.token_id)
         if id_token:
-            if current_user.get().is_authenticated(request):
+            if self.current_user.is_authenticated(request):
                 return True
             user_data = None
             with suppress(
                 auth.ExpiredIdTokenError,
                 auth.RevokedIdTokenError,
                 auth.InvalidIdTokenError,
             ):
                 user_data = auth.verify_id_token(id_token, check_revoked=True)
             if user_data:
-                self.user_model = depends.get(import_adapter("models")).Person
+                self.user_model = depends.get(import_adapter("models")).sql.Person
                 sql = depends.get(import_adapter("sql"))
                 async with sql.session as session:
                     user_query = select(self.user_model).where(  # type: ignore
                         self.user_model.gmail == user_data["email"]  # type: ignore
                         and self.user_model.is_active  # type: ignore
                         and self.user_model.is_superuser  # type: ignore
                     )
                     result = await session.execute(user_query)
                     enabled_user = result.one_or_none()
                 if enabled_user and (time() - user_data["auth_time"] < 5 * 6):
                     enabled_user = enabled_user[0]
                     auth.set_custom_user_claims(
                         user_data["uid"], {enabled_user.role: True}
                     )
-                    enabled_user.name = (user_data["name"],)
-                    enabled_user.uid = (user_data["uid"],)
-                    enabled_user.image = (user_data["picture"],)
+                    enabled_user.name = user_data["name"]
+                    debug(user_data["uid"], type(user_data["uid"]))
+                    enabled_user.google_uid = user_data["uid"]
+                    enabled_user.picture = user_data["picture"]
                     await enabled_user.save()
                     expires_in = timedelta(days=14)
                     session_cookie = auth.create_session_cookie(
                         id_token, expires_in=expires_in
                     )
                     self.config.auth.session_cookie = session_cookie
                     request.session.update({self.config.auth.token_id: session_cookie})
                     debug(request.session.keys())
                     return True
-                else:
-                    auth.revoke_refresh_tokens(user_data["uid"])
+                auth.revoke_refresh_tokens(user_data["uid"])
         request.session.pop(self.config.auth.token_id, None)
-        current_user.get().user_data = {}
+        self.current_user.user_data = {}
         return False
 
     async def logout(self, request: Request) -> bool:
         request.session.pop(self.config.auth.token_id, None)
         with suppress(
             auth.ExpiredIdTokenError,
             auth.RevokedIdTokenError,
             auth.InvalidIdTokenError,
+            auth.ExpiredSessionCookieError,
             ValueError,
         ):
             id_token = request.cookies.get(self.config.auth.token_id)
             user_data = auth.verify_id_token(id_token, check_revoked=True)
             auth.revoke_refresh_tokens(user_data["uid"])
-            current_user.get().user_data = {}
-            return True
-        return False
+        self.current_user().user_data = {}
+        return True
 
-    @staticmethod
-    async def authenticate(request: Request) -> bool:
-        return current_user.get().is_authenticated(request)
+    async def authenticate(self, request: Request) -> bool:
+        return self.current_user.is_authenticated(request)
 
 
 depends.set(Auth)
```

### Comparing `splashstand-3.0.2/splashstand/adapters/captcha/google.py` & `splashstand-3.0.3/splashstand/adapters/captcha/google.py`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/adapters/mail/mail.py` & `splashstand-3.0.3/splashstand/adapters/mail/mail.py`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/schemas/thing/intangible/schedule.yml` & `splashstand-3.0.3/splashstand/scrap/intangible/schedule.yml`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/base/js/serviceworker.js` & `splashstand-3.0.3/splashstand/templates/admin/base/js/serviceworker.js`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/base/tail.html.blah` & `splashstand-3.0.3/splashstand/templates/admin/base/tail.html.blah`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/bulma/blocks/menu_category.html` & `splashstand-3.0.3/splashstand/templates/admin/bulma/blocks/menu_category.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/bulma/layout.html` & `splashstand-3.0.3/splashstand/templates/admin/bulma/layout.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 [% extends "base.html" %]
-[# [% from '_macros.html' import display_menu %] #]
 [% block body %]
 <div class="wrapper">
   <aside class="navbar navbar-expand-lg navbar-vertical navbar-expand-md navbar-dark">
     <div class="container-fluid">
       <h1 class="navbar-brand navbar-brand-autodark">
         <a href="[[ url_for('admin:index') ]]">
           [% if admin.logo_url %]
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-[% extends "base.html" %] [# [% from '_macros.html' import display_menu %] #]
-[% block body %]
+[% extends "base.html" %] [% block body %]
 _[[_%%_ _ii_ff_ _aa_dd_mm_ii_nn_.._ll_oo_gg_oo____uu_rr_ll_ _%%_]]_ _[[_AA_dd_mm_ii_nn_]]_[[_%%_ _ee_ll_ss_ee_ _%%_]]
 _**_**_**_**_ _[[_[[_ _aa_dd_mm_ii_nn_.._tt_ii_tt_ll_ee_ _]]_]]_ _**_**_**_**
 _[[_%%_ _ee_nn_dd_ii_ff_ _%%_]]
 [[ render_block('display_menu.html', menu=admin._menu, request=request) ]]
 [% if admin.authentication_backend %]
 _L_o_g_o_u_t
 [% endif %]
```

### Comparing `splashstand-3.0.2/splashstand/templates/admin/bulma/login.html` & `splashstand-3.0.3/splashstand/templates/admin/bulma/login.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/bulma/scss/admin.yml` & `splashstand-3.0.3/splashstand/templates/admin/bulma/scss/admin.yml`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/actions.html` & `splashstand-3.0.3/splashstand/templates/admin/old/actions.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/analytics.html` & `splashstand-3.0.3/splashstand/templates/admin/old/analytics.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/content.html` & `splashstand-3.0.3/splashstand/templates/admin/old/content.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/details_modal.html` & `splashstand-3.0.3/splashstand/templates/admin/old/details_modal.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/index.html` & `splashstand-3.0.3/splashstand/templates/admin/old/index.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/layout.html` & `splashstand-3.0.3/splashstand/templates/admin/old/layout.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/lib.html` & `splashstand-3.0.3/splashstand/templates/admin/old/lib.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/list.html` & `splashstand-3.0.3/splashstand/templates/admin/old/list.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/modal.html` & `splashstand-3.0.3/splashstand/templates/admin/old/modal.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/redis_console.html` & `splashstand-3.0.3/splashstand/templates/admin/old/redis_console.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/row_actions.html` & `splashstand-3.0.3/splashstand/templates/admin/old/row_actions.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/storage_list.html` & `splashstand-3.0.3/splashstand/templates/admin/old/storage_list.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/theme_edit.html` & `splashstand-3.0.3/splashstand/templates/admin/old/theme_edit.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/admin/old/theme_list.html` & `splashstand-3.0.3/splashstand/templates/admin/old/theme_list.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/app/base/base.html` & `splashstand-3.0.3/splashstand/templates/app/base/base.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/app/base/blocks/tail.html` & `splashstand-3.0.3/splashstand/templates/app/base/blocks/tail.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/app/base/js/serviceworker.js` & `splashstand-3.0.3/splashstand/templates/app/base/js/serviceworker.js`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/app/bulma/blocks/elements.html` & `splashstand-3.0.3/splashstand/templates/app/bulma/blocks/elements.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/app/bulma/blocks/footer.html` & `splashstand-3.0.3/splashstand/templates/app/bulma/blocks/footer.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/app/bulma/blocks/header.html` & `splashstand-3.0.3/splashstand/templates/app/bulma/blocks/header.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/app/bulma/blocks/nav.html` & `splashstand-3.0.3/splashstand/templates/app/bulma/blocks/nav.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/app/bulma/privacy_policy.html` & `splashstand-3.0.3/splashstand/templates/app/bulma/privacy_policy.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/app/bulma/service_terms.html` & `splashstand-3.0.3/splashstand/templates/app/bulma/service_terms.html`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/app/bulma/style/custom.yml` & `splashstand-3.0.3/splashstand/templates/app/bulma/style/custom.yml`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/splashstand/templates/app/bulma/style/fender.yml` & `splashstand-3.0.3/splashstand/templates/app/bulma/style/fender.yml`

 * *Files identical despite different names*

### Comparing `splashstand-3.0.2/PKG-INFO` & `splashstand-3.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: SplashStand
-Version: 3.0.2
-Keywords: starlette htmx jinja httpx fastapi sqladmin sqlmodel pydantic
+Version: 3.0.3
+Keywords: starlette,htmx,jinja,httpx,fastapi,sqladmin,sqlmodel,pydantic
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
```

