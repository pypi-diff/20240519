# Comparing `tmp/protein_turnover_website-0.3.12.tar.gz` & `tmp/protein_turnover_website-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protein_turnover_website-0.3.12.tar", max compression
+gzip compressed data, was "protein_turnover_website-0.4.0.tar", max compression
```

## Comparing `protein_turnover_website-0.3.12.tar` & `protein_turnover_website-0.4.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0     1068 2024-05-17 07:06:31.689753 protein_turnover_website-0.3.12/LICENSE
--rw-r--r--   0        0        0       54 2024-05-17 06:43:03.102172 protein_turnover_website-0.3.12/prerelease.md
--rw-r--r--   0        0        0        0 2022-07-26 04:07:22.266032 protein_turnover_website-0.3.12/protein_turnover_website/__init__.py
--rw-r--r--   0        0        0     2703 2024-04-30 05:50:34.065016 protein_turnover_website-0.3.12/protein_turnover_website/app.py
--rw-r--r--   0        0        0     3093 2023-11-02 07:02:15.299192 protein_turnover_website-0.3.12/protein_turnover_website/cdn.toml
--rw-r--r--   0        0        0     2348 2024-05-13 17:45:54.986841 protein_turnover_website-0.3.12/protein_turnover_website/commands.py
--rw-r--r--   0        0        0     2312 2024-05-14 02:02:03.612310 protein_turnover_website-0.3.12/protein_turnover_website/config.py
--rw-r--r--   0        0        0        0 2022-07-26 22:24:13.364615 protein_turnover_website-0.3.12/protein_turnover_website/explorer/__init__.py
--rw-r--r--   0        0        0    11047 2024-05-14 02:11:05.732768 protein_turnover_website-0.3.12/protein_turnover_website/explorer/explorer.py
--rw-r--r--   0        0        0     1973 2024-02-09 01:57:57.957617 protein_turnover_website-0.3.12/protein_turnover_website/explorer/explorer_view.py
--rw-r--r--   0        0        0     1402 2022-10-04 02:27:11.831477 protein_turnover_website-0.3.12/protein_turnover_website/explorer/templates/explorer-test.html
--rw-r--r--   0        0        0      684 2022-10-02 08:18:42.820693 protein_turnover_website-0.3.12/protein_turnover_website/explorer/templates/explorer.css
--rw-r--r--   0        0        0     2707 2024-02-09 05:14:34.573665 protein_turnover_website-0.3.12/protein_turnover_website/explorer/templates/explorer.html
--rw-r--r--   0        0        0     4743 2024-04-16 23:37:41.239415 protein_turnover_website-0.3.12/protein_turnover_website/explorer/templates/explorer.js
--rw-r--r--   0        0        0     5554 2024-02-09 02:01:08.107049 protein_turnover_website-0.3.12/protein_turnover_website/explorer/templates/explorer.ts
--rw-r--r--   0        0        0     4576 2024-04-27 04:12:34.414016 protein_turnover_website-0.3.12/protein_turnover_website/flask_utils.py
--rw-r--r--   0        0        0      618 2024-04-28 01:18:02.953935 protein_turnover_website-0.3.12/protein_turnover_website/index_view.py
--rw-r--r--   0        0        0    14385 2024-04-26 00:38:41.221557 protein_turnover_website-0.3.12/protein_turnover_website/inspect.py
--rw-r--r--   0        0        0     7864 2024-05-17 06:06:20.554503 protein_turnover_website-0.3.12/protein_turnover_website/inspect_view.py
--rw-r--r--   0        0        0     6712 2024-05-17 05:29:31.119348 protein_turnover_website-0.3.12/protein_turnover_website/jobs.py
--rw-r--r--   0        0        0     9514 2024-05-14 02:49:07.911976 protein_turnover_website-0.3.12/protein_turnover_website/jobs_view.py
--rw-r--r--   0        0        0    11705 2024-05-17 06:18:11.396851 protein_turnover_website-0.3.12/protein_turnover_website/jobsmanager.py
--rw-r--r--   0        0        0     2983 2024-04-26 07:44:15.310865 protein_turnover_website-0.3.12/protein_turnover_website/logger.py
--rw-r--r--   0        0        0        0 2022-08-17 09:28:39.309757 protein_turnover_website-0.3.12/protein_turnover_website/login/__init__.py
--rw-r--r--   0        0        0     4024 2024-04-16 00:47:38.985633 protein_turnover_website-0.3.12/protein_turnover_website/login/login_view.py
--rw-r--r--   0        0        0     1609 2022-10-04 02:27:11.839478 protein_turnover_website-0.3.12/protein_turnover_website/login/templates/login.html
--rw-r--r--   0        0        0      808 2024-04-16 23:37:41.243415 protein_turnover_website-0.3.12/protein_turnover_website/login/templates/login.js
--rw-r--r--   0        0        0      842 2023-11-02 07:02:15.299192 protein_turnover_website-0.3.12/protein_turnover_website/login/templates/login.ts
--rw-r--r--   0        0        0        0 2022-11-08 03:47:29.541934 protein_turnover_website-0.3.12/protein_turnover_website/sqla/__init__.py
--rw-r--r--   0        0        0     5659 2024-03-11 07:54:57.370123 protein_turnover_website-0.3.12/protein_turnover_website/sqla/export.py
--rw-r--r--   0        0        0      963 2024-03-11 07:57:30.587258 protein_turnover_website-0.3.12/protein_turnover_website/sqla/export.toml
--rw-r--r--   0        0        0    10772 2024-03-31 22:43:01.586988 protein_turnover_website-0.3.12/protein_turnover_website/sqla/inspect.py
--rw-r--r--   0        0        0      679 2024-03-28 12:14:06.794706 protein_turnover_website-0.3.12/protein_turnover_website/sqla/peptides.toml
--rw-r--r--   0        0        0      588 2023-11-13 22:21:06.788496 protein_turnover_website-0.3.12/protein_turnover_website/sqla/proteins.toml
--rw-r--r--   0        0        0    15025 2022-07-26 04:49:46.758869 protein_turnover_website-0.3.12/protein_turnover_website/static/img/UWA-Full-Hor-CMYK-wt-opt.svgz
--rw-r--r--   0        0        0    62042 2022-08-23 03:32:47.883547 protein_turnover_website-0.3.12/protein_turnover_website/static/img/about/eics.png
--rw-r--r--   0        0        0    43312 2022-08-23 03:28:30.649979 protein_turnover_website-0.3.12/protein_turnover_website/static/img/about/isotopeEnvelopes.png
--rw-r--r--   0        0        0     9576 2022-08-23 23:23:37.063505 protein_turnover_website-0.3.12/protein_turnover_website/static/img/about/labelledEnvelope.png
--rw-r--r--   0        0        0    32813 2023-03-14 02:49:15.755245 protein_turnover_website-0.3.12/protein_turnover_website/static/img/about/plotFittedEnvelopes.png
--rw-r--r--   0        0        0     2383 2022-07-26 04:50:41.527162 protein_turnover_website-0.3.12/protein_turnover_website/static/img/email-white.svgz
--rw-r--r--   0        0        0    32928 2022-08-12 06:39:23.045191 protein_turnover_website-0.3.12/protein_turnover_website/static/img/enrichment.png
--rw-r--r--   0        0        0    13430 2023-02-16 08:46:20.525798 protein_turnover_website-0.3.12/protein_turnover_website/static/img/nnls_residuals.png
--rw-r--r--   0        0        0    17346 2022-07-26 05:06:40.732228 protein_turnover_website-0.3.12/protein_turnover_website/static/img/turnover.png
--rw-r--r--   0        0        0   503303 2023-03-13 08:45:49.226525 protein_turnover_website-0.3.12/protein_turnover_website/static/img/wheat4.jpg
--rw-r--r--   0        0        0     9509 2024-05-13 18:00:04.667209 protein_turnover_website-0.3.12/protein_turnover_website/templates/about-frag.html
--rw-r--r--   0        0        0    14425 2024-05-13 12:39:23.043947 protein_turnover_website-0.3.12/protein_turnover_website/templates/about-orig.html
--rw-r--r--   0        0        0     1192 2024-05-13 17:57:38.180718 protein_turnover_website-0.3.12/protein_turnover_website/templates/about.html
--rw-r--r--   0        0        0     8911 2024-05-13 18:01:38.003934 protein_turnover_website-0.3.12/protein_turnover_website/templates/about.md.tplt
--rw-r--r--   0        0        0      291 2024-04-28 00:43:05.728911 protein_turnover_website-0.3.12/protein_turnover_website/templates/bad-file.html
--rw-r--r--   0        0        0     3571 2024-05-17 04:28:41.885275 protein_turnover_website-0.3.12/protein_turnover_website/templates/configuration.html
--rw-r--r--   0        0        0     1473 2024-04-28 00:40:29.487698 protein_turnover_website-0.3.12/protein_turnover_website/templates/errors/404.html
--rw-r--r--   0        0        0     5516 2024-04-08 03:50:35.047582 protein_turnover_website-0.3.12/protein_turnover_website/templates/filter-frag.html
--rw-r--r--   0        0        0      287 2023-11-03 03:27:24.219728 protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/beta.html
--rw-r--r--   0        0        0     7311 2022-07-26 04:16:32.500682 protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/email.svg
--rw-r--r--   0        0        0      485 2022-10-04 02:27:11.839478 protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/google.html
--rw-r--r--   0        0        0     1738 2023-11-03 22:30:22.219226 protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/macros.html
--rw-r--r--   0        0        0      885 2023-11-03 03:27:36.311873 protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/meta.html
--rw-r--r--   0        0        0      307 2022-07-26 04:16:32.500682 protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/offsite.svg
--rw-r--r--   0        0        0     3672 2024-02-14 06:31:18.938538 protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/range.css
--rw-r--r--   0        0        0      602 2024-02-14 07:36:27.479208 protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/range.html
--rw-r--r--   0        0        0     4011 2024-04-16 23:37:41.287415 protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/range.js
--rw-r--r--   0        0        0     4206 2024-02-20 02:42:42.591329 protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/range.ts
--rw-r--r--   0        0        0     1486 2022-10-04 02:27:11.835478 protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/theme.html
--rw-r--r--   0        0        0      446 2022-10-04 02:27:11.835478 protein_turnover_website-0.3.12/protein_turnover_website/templates/index.html
--rw-r--r--   0        0        0     2527 2024-04-16 23:37:41.247415 protein_turnover_website-0.3.12/protein_turnover_website/templates/inspect-download.js
--rw-r--r--   0        0        0     2755 2023-11-02 07:02:15.299192 protein_turnover_website-0.3.12/protein_turnover_website/templates/inspect-download.ts
--rw-r--r--   0        0        0     8373 2024-04-28 04:43:51.155619 protein_turnover_website-0.3.12/protein_turnover_website/templates/inspect.html
--rw-r--r--   0        0        0    12480 2024-04-16 23:37:41.263415 protein_turnover_website-0.3.12/protein_turnover_website/templates/inspect.js
--rw-r--r--   0        0        0    14315 2024-04-15 09:03:11.658937 protein_turnover_website-0.3.12/protein_turnover_website/templates/inspect.ts
--rw-r--r--   0        0        0     4665 2024-04-16 00:44:09.643261 protein_turnover_website-0.3.12/protein_turnover_website/templates/job-frag.html
--rw-r--r--   0        0        0     2801 2023-11-13 05:45:24.545353 protein_turnover_website-0.3.12/protein_turnover_website/templates/job-index.html
--rw-r--r--   0        0        0     3525 2024-04-16 23:37:41.267415 protein_turnover_website-0.3.12/protein_turnover_website/templates/job-index.js
--rw-r--r--   0        0        0     4153 2023-11-04 23:51:36.686589 protein_turnover_website-0.3.12/protein_turnover_website/templates/job-index.ts
--rw-r--r--   0        0        0    11736 2024-04-26 07:55:01.842002 protein_turnover_website-0.3.12/protein_turnover_website/templates/jobs.html
--rw-r--r--   0        0        0    12544 2024-04-16 23:37:41.279415 protein_turnover_website-0.3.12/protein_turnover_website/templates/jobs.js
--rw-r--r--   0        0        0    13944 2024-04-11 02:21:23.908714 protein_turnover_website-0.3.12/protein_turnover_website/templates/jobs.ts
--rw-r--r--   0        0        0     2517 2022-08-14 23:50:39.361001 protein_turnover_website-0.3.12/protein_turnover_website/templates/macros/spinner.html
--rw-r--r--   0        0        0      388 2024-04-29 01:16:09.377432 protein_turnover_website-0.3.12/protein_turnover_website/templates/print.css
--rw-r--r--   0        0        0    12753 2024-05-17 03:59:53.237173 protein_turnover_website-0.3.12/protein_turnover_website/templates/raw.html
--rw-r--r--   0        0        0     6508 2023-03-13 08:09:04.609138 protein_turnover_website-0.3.12/protein_turnover_website/templates/table_meta.html
--rw-r--r--   0        0        0      135 2024-04-29 00:49:29.828093 protein_turnover_website-0.3.12/protein_turnover_website/templates/view.html
--rw-r--r--   0        0        0     3945 2024-04-26 06:37:44.451865 protein_turnover_website-0.3.12/protein_turnover_website/utils.py
--rw-r--r--   0        0        0      261 2024-04-11 11:43:50.588696 protein_turnover_website-0.3.12/protein_turnover_website/wsgi.py
--rw-r--r--   0        0        0      123 2024-04-29 01:02:58.914559 protein_turnover_website-0.3.12/protein_turnover_website/wsgi_view.py
--rw-r--r--   0        0        0     1568 2024-05-17 07:11:41.683528 protein_turnover_website-0.3.12/pyproject.toml
--rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 protein_turnover_website-0.3.12/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-17 07:06:31.689753 protein_turnover_website-0.4.0/LICENSE
+-rw-r--r--   0        0        0       54 2024-05-17 06:43:03.102172 protein_turnover_website-0.4.0/prerelease.md
+-rw-r--r--   0        0        0        0 2022-07-26 04:07:22.266032 protein_turnover_website-0.4.0/protein_turnover_website/__init__.py
+-rw-r--r--   0        0        0     2703 2024-04-30 05:50:34.065016 protein_turnover_website-0.4.0/protein_turnover_website/app.py
+-rw-r--r--   0        0        0     3093 2023-11-02 07:02:15.299192 protein_turnover_website-0.4.0/protein_turnover_website/cdn.toml
+-rw-r--r--   0        0        0     2348 2024-05-13 17:45:54.986841 protein_turnover_website-0.4.0/protein_turnover_website/commands.py
+-rw-r--r--   0        0        0     2326 2024-05-19 05:48:07.744329 protein_turnover_website-0.4.0/protein_turnover_website/config.py
+-rw-r--r--   0        0        0        0 2022-07-26 22:24:13.364615 protein_turnover_website-0.4.0/protein_turnover_website/explorer/__init__.py
+-rw-r--r--   0        0        0    11154 2024-05-19 02:18:48.498784 protein_turnover_website-0.4.0/protein_turnover_website/explorer/explorer.py
+-rw-r--r--   0        0        0     1973 2024-02-09 01:57:57.957617 protein_turnover_website-0.4.0/protein_turnover_website/explorer/explorer_view.py
+-rw-r--r--   0        0        0     1402 2022-10-04 02:27:11.831477 protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer-test.html
+-rw-r--r--   0        0        0      684 2022-10-02 08:18:42.820693 protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.css
+-rw-r--r--   0        0        0     2707 2024-02-09 05:14:34.573665 protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.html
+-rw-r--r--   0        0        0     4743 2024-05-17 09:19:50.799202 protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.js
+-rw-r--r--   0        0        0     5554 2024-02-09 02:01:08.107049 protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.ts
+-rw-r--r--   0        0        0     5042 2024-05-19 03:27:01.503075 protein_turnover_website-0.4.0/protein_turnover_website/flask_utils.py
+-rw-r--r--   0        0        0      618 2024-04-28 01:18:02.953935 protein_turnover_website-0.4.0/protein_turnover_website/index_view.py
+-rw-r--r--   0        0        0    14385 2024-04-26 00:38:41.221557 protein_turnover_website-0.4.0/protein_turnover_website/inspect.py
+-rw-r--r--   0        0        0     7914 2024-05-18 20:07:47.125646 protein_turnover_website-0.4.0/protein_turnover_website/inspect_view.py
+-rw-r--r--   0        0        0     6632 2024-05-19 02:41:27.270572 protein_turnover_website-0.4.0/protein_turnover_website/jobs.py
+-rw-r--r--   0        0        0     9560 2024-05-19 02:41:18.226491 protein_turnover_website-0.4.0/protein_turnover_website/jobs_view.py
+-rw-r--r--   0        0        0    11506 2024-05-19 02:09:12.917842 protein_turnover_website-0.4.0/protein_turnover_website/jobsmanager.py
+-rw-r--r--   0        0        0     2982 2024-05-19 03:34:25.959094 protein_turnover_website-0.4.0/protein_turnover_website/logger.py
+-rw-r--r--   0        0        0        0 2022-08-17 09:28:39.309757 protein_turnover_website-0.4.0/protein_turnover_website/login/__init__.py
+-rw-r--r--   0        0        0     4024 2024-04-16 00:47:38.985633 protein_turnover_website-0.4.0/protein_turnover_website/login/login_view.py
+-rw-r--r--   0        0        0     1609 2022-10-04 02:27:11.839478 protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.html
+-rw-r--r--   0        0        0      808 2024-05-17 09:19:50.803202 protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.js
+-rw-r--r--   0        0        0      842 2023-11-02 07:02:15.299192 protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.ts
+-rw-r--r--   0        0        0        0 2022-11-08 03:47:29.541934 protein_turnover_website-0.4.0/protein_turnover_website/sqla/__init__.py
+-rw-r--r--   0        0        0     5657 2024-05-19 02:10:05.778296 protein_turnover_website-0.4.0/protein_turnover_website/sqla/export.py
+-rw-r--r--   0        0        0      963 2024-03-11 07:57:30.587258 protein_turnover_website-0.4.0/protein_turnover_website/sqla/export.toml
+-rw-r--r--   0        0        0    10772 2024-03-31 22:43:01.586988 protein_turnover_website-0.4.0/protein_turnover_website/sqla/inspect.py
+-rw-r--r--   0        0        0      679 2024-03-28 12:14:06.794706 protein_turnover_website-0.4.0/protein_turnover_website/sqla/peptides.toml
+-rw-r--r--   0        0        0      588 2023-11-13 22:21:06.788496 protein_turnover_website-0.4.0/protein_turnover_website/sqla/proteins.toml
+-rw-r--r--   0        0        0    15025 2022-07-26 04:49:46.758869 protein_turnover_website-0.4.0/protein_turnover_website/static/img/UWA-Full-Hor-CMYK-wt-opt.svgz
+-rw-r--r--   0        0        0    62042 2022-08-23 03:32:47.883547 protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/eics.png
+-rw-r--r--   0        0        0    43312 2022-08-23 03:28:30.649979 protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/isotopeEnvelopes.png
+-rw-r--r--   0        0        0     9576 2022-08-23 23:23:37.063505 protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/labelledEnvelope.png
+-rw-r--r--   0        0        0    32813 2023-03-14 02:49:15.755245 protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/plotFittedEnvelopes.png
+-rw-r--r--   0        0        0     2383 2022-07-26 04:50:41.527162 protein_turnover_website-0.4.0/protein_turnover_website/static/img/email-white.svgz
+-rw-r--r--   0        0        0    32928 2022-08-12 06:39:23.045191 protein_turnover_website-0.4.0/protein_turnover_website/static/img/enrichment.png
+-rw-r--r--   0        0        0    13430 2023-02-16 08:46:20.525798 protein_turnover_website-0.4.0/protein_turnover_website/static/img/nnls_residuals.png
+-rw-r--r--   0        0        0    17346 2022-07-26 05:06:40.732228 protein_turnover_website-0.4.0/protein_turnover_website/static/img/turnover.png
+-rw-r--r--   0        0        0   503303 2023-03-13 08:45:49.226525 protein_turnover_website-0.4.0/protein_turnover_website/static/img/wheat4.jpg
+-rw-r--r--   0        0        0     9509 2024-05-13 18:00:04.667209 protein_turnover_website-0.4.0/protein_turnover_website/templates/about-frag.html
+-rw-r--r--   0        0        0    14425 2024-05-13 12:39:23.043947 protein_turnover_website-0.4.0/protein_turnover_website/templates/about-orig.html
+-rw-r--r--   0        0        0     1192 2024-05-13 17:57:38.180718 protein_turnover_website-0.4.0/protein_turnover_website/templates/about.html
+-rw-r--r--   0        0        0     8911 2024-05-13 18:01:38.003934 protein_turnover_website-0.4.0/protein_turnover_website/templates/about.md.tplt
+-rw-r--r--   0        0        0      291 2024-04-28 00:43:05.728911 protein_turnover_website-0.4.0/protein_turnover_website/templates/bad-file.html
+-rw-r--r--   0        0        0     3571 2024-05-17 04:28:41.885275 protein_turnover_website-0.4.0/protein_turnover_website/templates/configuration.html
+-rw-r--r--   0        0        0     1473 2024-04-28 00:40:29.487698 protein_turnover_website-0.4.0/protein_turnover_website/templates/errors/404.html
+-rw-r--r--   0        0        0     5516 2024-04-08 03:50:35.047582 protein_turnover_website-0.4.0/protein_turnover_website/templates/filter-frag.html
+-rw-r--r--   0        0        0      287 2023-11-03 03:27:24.219728 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/beta.html
+-rw-r--r--   0        0        0     7311 2022-07-26 04:16:32.500682 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/email.svg
+-rw-r--r--   0        0        0      485 2022-10-04 02:27:11.839478 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/google.html
+-rw-r--r--   0        0        0     1738 2023-11-03 22:30:22.219226 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/macros.html
+-rw-r--r--   0        0        0      885 2023-11-03 03:27:36.311873 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/meta.html
+-rw-r--r--   0        0        0      307 2022-07-26 04:16:32.500682 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/offsite.svg
+-rw-r--r--   0        0        0     3672 2024-02-14 06:31:18.938538 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.css
+-rw-r--r--   0        0        0      602 2024-02-14 07:36:27.479208 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.html
+-rw-r--r--   0        0        0     4011 2024-05-17 09:19:50.839203 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.js
+-rw-r--r--   0        0        0     4206 2024-02-20 02:42:42.591329 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.ts
+-rw-r--r--   0        0        0     1486 2022-10-04 02:27:11.835478 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/theme.html
+-rw-r--r--   0        0        0      446 2022-10-04 02:27:11.835478 protein_turnover_website-0.4.0/protein_turnover_website/templates/index.html
+-rw-r--r--   0        0        0     2527 2024-05-17 09:19:50.807202 protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect-download.js
+-rw-r--r--   0        0        0     2755 2023-11-02 07:02:15.299192 protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect-download.ts
+-rw-r--r--   0        0        0     8373 2024-04-28 04:43:51.155619 protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.html
+-rw-r--r--   0        0        0    12482 2024-05-17 09:19:50.823202 protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.js
+-rw-r--r--   0        0        0    14319 2024-05-17 09:02:50.406196 protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.ts
+-rw-r--r--   0        0        0     4614 2024-05-19 02:36:25.783854 protein_turnover_website-0.4.0/protein_turnover_website/templates/job-frag.html
+-rw-r--r--   0        0        0     2789 2024-05-19 02:37:23.800371 protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.html
+-rw-r--r--   0        0        0     3525 2024-05-17 09:19:50.827202 protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.js
+-rw-r--r--   0        0        0     4153 2024-05-17 09:19:47.319160 protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.ts
+-rw-r--r--   0        0        0    11736 2024-04-26 07:55:01.842002 protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.html
+-rw-r--r--   0        0        0    12544 2024-05-17 09:19:50.835202 protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.js
+-rw-r--r--   0        0        0    13944 2024-04-11 02:21:23.908714 protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.ts
+-rw-r--r--   0        0        0     2517 2022-08-14 23:50:39.361001 protein_turnover_website-0.4.0/protein_turnover_website/templates/macros/spinner.html
+-rw-r--r--   0        0        0      388 2024-04-29 01:16:09.377432 protein_turnover_website-0.4.0/protein_turnover_website/templates/print.css
+-rw-r--r--   0        0        0    12753 2024-05-17 03:59:53.237173 protein_turnover_website-0.4.0/protein_turnover_website/templates/raw.html
+-rw-r--r--   0        0        0     6508 2023-03-13 08:09:04.609138 protein_turnover_website-0.4.0/protein_turnover_website/templates/table_meta.html
+-rw-r--r--   0        0        0      135 2024-04-29 00:49:29.828093 protein_turnover_website-0.4.0/protein_turnover_website/templates/view.html
+-rw-r--r--   0        0        0     3945 2024-04-26 06:37:44.451865 protein_turnover_website-0.4.0/protein_turnover_website/utils.py
+-rw-r--r--   0        0        0      261 2024-04-11 11:43:50.588696 protein_turnover_website-0.4.0/protein_turnover_website/wsgi.py
+-rw-r--r--   0        0        0      123 2024-04-29 01:02:58.914559 protein_turnover_website-0.4.0/protein_turnover_website/wsgi_view.py
+-rw-r--r--   0        0        0     1587 2024-05-19 09:01:03.011450 protein_turnover_website-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 protein_turnover_website-0.4.0/PKG-INFO
```

### Comparing `protein_turnover_website-0.3.12/LICENSE` & `protein_turnover_website-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/app.py` & `protein_turnover_website-0.4.0/protein_turnover_website/app.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/cdn.toml` & `protein_turnover_website-0.4.0/protein_turnover_website/cdn.toml`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/commands.py` & `protein_turnover_website-0.4.0/protein_turnover_website/commands.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/config.py` & `protein_turnover_website-0.4.0/protein_turnover_website/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 APP_NAME = "Protein Turnover"
 
 # only used with email logger
-# ADMINS = ['your.email@gmail.com']
+ADMINS: list[str] = []  # ['your.email@gmail.com']
 MAIL_SUBJECT = "turnover pipeline website"
-# where to send email to...
-MAIL_SERVER = "antivirus.uwa.edu.au"
+# where should logger send email to...
+MAIL_SERVER = "mailhost"
 
 
 # used for input placeholder
 MAIL_PLACEHOLDER = "your.name@uwa.edu.au"
 
 KILL_OK = True
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/explorer/explorer.py` & `protein_turnover_website-0.4.0/protein_turnover_website/explorer/explorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 from dataclasses import dataclass
 from datetime import datetime
 from itertools import chain
 from os import stat_result
 from pathlib import Path
 from typing import Any
+from typing import Sequence
 
 from flask import current_app
 from flask import Flask
 from flask import request
 from markupsafe import Markup
 from typing_extensions import TypedDict
 
@@ -368,19 +369,20 @@
     return mountpoints
 
 
 def init_mountpoints(app: Flask) -> None:
 
     MountPoint.ALLOW_LINKS = app.config.get("ALLOW_LINKS", False)
     mm = app.config.get("MOUNTPOINTS")
-
+    # NOTE: may come from a .toml file so will be
+    # a list of listss
     if (
-        not isinstance(mm, list)
+        not isinstance(mm, Sequence)
         or len(mm) == 0
-        or not all(isinstance(m, tuple) for m in mm)
+        or not all(isinstance(m, Sequence) for m in mm)
     ):
         raise ValueError("config.MOUNTPOINTS should be a list of tuples")
 
     mountpoints = [MountPoint(*m) for m in mm]
 
     if not sorted({m.label for m in mountpoints}) == sorted(
         m.label for m in mountpoints
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/explorer/explorer_view.py` & `protein_turnover_website-0.4.0/protein_turnover_website/explorer/explorer_view.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/explorer/templates/explorer-test.html` & `protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer-test.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/explorer/templates/explorer.css` & `protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.css`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/explorer/templates/explorer.html` & `protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/explorer/templates/explorer.js` & `protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/explorer/templates/explorer.ts` & `protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/flask_utils.py` & `protein_turnover_website-0.4.0/protein_turnover_website/flask_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 import gzip
+import os
 from itertools import chain
 from pathlib import Path
 from typing import Any
 
 import tomli as tomllib
+from flask import current_app
 from flask import Flask
 from flask import render_template
 from flask import Response
 from flask.config import Config
+from flask_login import current_user
 from jinja2 import FileSystemBytecodeCache
 from jinja2 import FileSystemLoader
 from jinja2 import TemplateNotFound
 from markupsafe import Markup
 
 from .utils import attrstr
 from .utils import human
@@ -23,19 +26,29 @@
 NAME = __name__.split(".", maxsplit=1)[0]
 
 
 def error_resp(msg: str, code: int) -> Response:
     return Response(msg, code, mimetype="text/plain")
 
 
+def oktokill() -> bool:
+    if current_user.is_authenticated:
+        return True
+    if current_app.config.get("WEBSITE_STATE", "multi_user") == "single_user":
+        return True
+    return current_app.config.get("KILL_OK", False)
+
+
 def config_app(config: Config) -> Config:
     config.from_object(f"{NAME}.config")
-    config.from_pyfile(f"{NAME}.cfg", silent=True)
+    config.from_pyfile("turnover-web.cfg", silent=True)
     # we are running in embbed mode...
-    config.from_envvar("TURNOVER_SETTINGS", silent=True)
+    # config.from_envvar("TURNOVER_SETTINGS", silent=True)
+    if "TURNOVER_SETTINGS" in os.environ:
+        config.from_file(os.environ["TURNOVER_SETTINGS"], load=tomllib.load, text=False)  # type: ignore
 
     return config
 
 
 def register_bytecode_cache(app: Flask, directory: str = "bytecode_cache") -> None:
     cache = Path(directory)
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/index_view.py` & `protein_turnover_website-0.4.0/protein_turnover_website/index_view.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/inspect.py` & `protein_turnover_website-0.4.0/protein_turnover_website/inspect.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/inspect_view.py` & `protein_turnover_website-0.4.0/protein_turnover_website/inspect_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,23 +185,23 @@
 def plot_url(dataid: str) -> Response:
     """Send plot as data: url"""
     plotio = mkplot(dataid, get_rowid(), fmt="png")
     url = encode_img(plotio, image_format="png")
     return jsonify({"image_url": url})
 
 
-@inspect.route("/enrichment_plot/<path:dataid>")
+@inspect.route("/enrichment_plot/<path:dataid>", methods=["POST", "GET"])
 def enrichment_plot(dataid: str) -> Response:
     p = make_enrichment_plot(dataid, column="enrichment")
     if p is None:
         abort(404)
     return jsonify({"enrichment_url": p})
 
 
-@inspect.route("/nnls_plot/<path:dataid>")
+@inspect.route("/nnls_plot/<path:dataid>", methods=["POST", "GET"])
 def nnls_plot(dataid: str) -> Response:
     p = make_nnls_plot(dataid, percent=0.01)
     if p is None:
         abort(404)
     return jsonify({"nnls_url": p})
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/jobs.py` & `protein_turnover_website-0.4.0/protein_turnover_website/jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,32 +7,29 @@
 from dataclasses import replace
 from pathlib import Path
 
 from flask import abort
 from flask import current_app
 from flask import Flask
 from flask import request
-from flask_login import current_user
 from protein_turnover.background import SimpleQueueClient
 from protein_turnover.jobs import PeptideSettings
 from protein_turnover.jobs import TurnoverJob
 
 from .explorer.explorer import find_mountpoint_for
 from .explorer.explorer import get_mountpoints
 from .explorer.explorer import logger
 from .explorer.explorer import safe_repr
+from .flask_utils import oktokill as oktokill
 from .jobsmanager import JobsManager
 from .jobsmanager import PersonalJobsManager
 
 
-def oktokill() -> None:
-    if current_user.is_authenticated:
-        return
-    ok = current_app.config.get("KILL_OK", False)
-    if not ok:
+def oktokill_abort() -> None:
+    if not oktokill():
         abort(404)
 
 
 def sanitize(job: TurnoverJob) -> TurnoverJob:
     mountpoints = get_mountpoints()
 
     def rep(p: str) -> str:
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/jobs_view.py` & `protein_turnover_website-0.4.0/protein_turnover_website/jobs_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 from flask import Blueprint
 from flask import current_app
 from flask import Flask
 from flask import jsonify
 from flask import render_template
 from flask import request
 from flask import Response
-from flask_login import current_user
 from protein_turnover.jobs import TurnoverJob
 from protein_turnover.pepxml import count_spectra
 from protein_turnover.pepxml import scan_pp_probability
 from protein_turnover.protxml import scan_proteins
 from protein_turnover.pymz import scan_mzml_spectra
 from protein_turnover.utils import atomicProperties
 from protein_turnover.utils import NAMES
 from protein_turnover.utils import PeptideSettings
 
 from .explorer.explorer import find_directory_from_request
 from .explorer.explorer import find_explorer
 from .explorer.explorer import get_mountpoints
+from .flask_utils import oktokill
 from .jobs import ensure_cachedir
 from .jobs import ensure_jobsdir
 from .jobs import File
 from .jobs import get_bg_client
 from .jobs import get_jobs_manager
 from .jobs import job_from_form
-from .jobs import oktokill
+from .jobs import oktokill_abort
 from .jobs import sanitize
 from .utils import read_log
 
 
 job = Blueprint("job", __name__)
 
 
@@ -59,25 +59,27 @@
 @job.route("/job-index")
 def index() -> str:
     """Jobs table"""
     return render_template(
         "job-index.html",
         is_running=get_bg_client().is_running(),
         **get_jobs_manager().find_jobs(),
+        oktokill=oktokill(),
     )
 
 
 @job.route("/refresh-jobs")
 def refresh_jobs() -> Response:
     """Refresh jobtables: returns json {table:html}"""
 
     jobs = get_jobs_manager().find_jobs()  # pylint: disable=redefined-outer-name
     e = current_app.jinja_env.get_template("job-frag.html")
     jobtable = e.module.jobtable  # type: ignore
-    jt = {k: jobtable(v, current_user) for k, v in jobs.items()}
+    ok = oktokill()
+    jt = {k: jobtable(v, ok) for k, v in jobs.items()}
     return jsonify(jt)
 
 
 @job.route("/meta")
 def find_metadata() -> str:
     """Find TurnoverJob file and return rendered HTML"""
 
@@ -165,15 +167,15 @@
         )
     jm = get_jobs_manager()
 
     # try to get a unique id starting with possible jobname
     jobid = jm.prefix_jobid(jobname)
 
     jobby = job_from_form(jobid)
-    jd = jm.locate(jobid, decode=False).locate_directory()
+    jd = jm.locate(jobid).locate_directory()
     try:
         jd.mkdir(exist_ok=True, parents=True)
     except OSError:
         current_app.logger.error("failed to make directory: %s", jd)
         return jsonify(
             JsonReply(status="failed", msg=f"can't create job {jobby.jobid}"),
         )
@@ -187,30 +189,30 @@
 
 @job.route("/kill")
 def kill_job() -> Response:
     dataid = request.values.get("dataid")
     if not dataid:
         abort(404)
 
-    oktokill()
+    oktokill_abort()
 
     msg = get_jobs_manager().locate(dataid).kill_pid()
     if msg is not None:
         return jsonify(JsonReply(status="failed", msg=msg))
 
     return jsonify(JsonReply(status="OK", msg=f"job {dataid} killed"))
 
 
 @job.route("/restart")
 def restart_job() -> Response:
     dataid = request.values.get("dataid")
     if not dataid:
         abort(404)
 
-    oktokill()
+    oktokill_abort()
 
     config = get_jobs_manager().locate(dataid).locate_config_file()
     if not config.exists():
         return jsonify(JsonReply(status="failed", msg=f"no job {dataid}!"))
 
     job = TurnoverJob.restore(config)  # pylint: disable=redefined-outer-name
     job = replace(job, status="pending")
@@ -223,15 +225,15 @@
 @job.route("/delete")
 def remove_job() -> Response:
 
     dataid = request.values.get("dataid")
     if not dataid:
         abort(404)
 
-    oktokill()
+    oktokill_abort()
 
     try:
         ok = get_jobs_manager().locate(dataid).remove()
 
         if not ok:
             return jsonify(JsonReply(status="failed", msg=f"no job {dataid}!"))
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/jobsmanager.py` & `protein_turnover_website-0.4.0/protein_turnover_website/jobsmanager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,36 @@
 from __future__ import annotations
 
 import os
 import random
 import shutil
 import signal
 import string
-from base64 import urlsafe_b64decode
-from base64 import urlsafe_b64encode
+import sys
 from datetime import datetime
 from os import walk
 from pathlib import Path
 from typing import Iterator
 from typing import NamedTuple
 from typing import TypedDict
 from uuid import uuid4
 
 from flask import abort
 from flask import current_app
-from protein_turnover.config import RESULT_EXT
+from protein_turnover.exts import RESULT_EXT
 from protein_turnover.jobs import slugify
 from protein_turnover.jobs import TurnoverJob
 
 
-def path_encode(path: str) -> str:
-    return urlsafe_b64encode(path.encode("ascii")).decode("ascii")
-
-
-def path_decode(path: str) -> str:
-    return urlsafe_b64decode(path.encode("ascii")).decode("ascii")
-
-
 class Locator:
     """Given a dataid and a root jobsdir locate all files for this dataid"""
 
-    def __init__(self, jobid: str, manager: JobsManager, decode: bool = False):
+    def __init__(self, jobid: str, manager: JobsManager):
         self.jobid = jobid
         self.manager = manager
-        self.decode = decode
 
     def stem(self) -> str:
         method = self.manager.method
         if method == -1:
             return "project"
         if method == 0:
             return self.jobid
@@ -103,43 +93,59 @@
             try:
                 f.unlink(missing_ok=True)
             except OSError:
                 pass
         return True
 
 
-def check_path(dataid: str, root: Path, decode: bool = True) -> tuple[Path, bool]:
+def check_path(dataid: str, root: Path) -> tuple[Path, bool]:
     """dataid is from the web, root is from us (so trusted)"""
-    if decode:
-        dataid = path_decode(dataid)
+
     dataid = dataid + ".toml"
     if ".." in dataid:
         return Path(dataid), False
     jobfile = Path(dataid)
     if jobfile.is_absolute():
         return jobfile, False
     jobfile = (root / jobfile).resolve()
     if not jobfile.relative_to(root):
         return jobfile, False
 
     return jobfile, True
 
 
+IS_WIN = sys.platform == "win32"
+
+
+def url_to_path(dataid: str) -> str:
+    # if IS_WIN:
+    #     return dataid.replace("/", "\\")
+    return dataid
+
+
+def path_to_url(path: str) -> str:
+    if IS_WIN:
+        return path.replace("\\", "/")
+    return path
+
+
 class SimpleLocator(Locator):
-    def __init__(self, dataid: str, manager: JobsManager, decode: bool = False):
+    def __init__(self, dataid: str, manager: JobsManager):
         """dataid is an encoded file path from the web (so untrustworth!)"""
-        jobfile, ok = check_path(dataid, manager.jobsdir, decode=decode)
+
+        # dataid = url_to_path(dataid)
+        jobfile, ok = check_path(dataid, manager.jobsdir)
         if not ok:
             self.bad_file(jobfile)
         if jobfile.exists():
             job = TurnoverJob.restore(jobfile)
             jobid = job.jobid
         else:
             jobid = dataid
-        super().__init__(jobid, manager, decode)
+        super().__init__(jobid, manager)
         self.jobfile = jobfile
 
     def bad_file(self, jobfile: Path) -> None:
         current_app.logger.error("bad dataid: %s", jobfile)
         abort(404)
 
     def locate_directory(self) -> Path:
@@ -180,15 +186,16 @@
     def dataid(self) -> str:
         return self.job.jobid
 
 
 class PersonalJobFiles(TurnoverJobFiles):
     @property
     def dataid(self) -> str:
-        return self.full_path
+        """Use full path as dataid"""
+        return path_to_url(self.full_path)
 
 
 class Jobs(TypedDict):
     running: list[TurnoverJobFiles]
     queued: list[TurnoverJobFiles]
     finished: list[TurnoverJobFiles]
 
@@ -292,46 +299,45 @@
         self.method = method
         self.sub_directories = sub_directories
         self.max_length = max_length
 
     def find_jobs(self) -> Jobs:
         return self.FinderClass().find_job_files(self.jobsdir)
 
-    def locate(self, dataid: str, *, decode: bool = False) -> Locator:
+    def locate(self, dataid: str) -> Locator:
         return self.LocatorClass(
             dataid,
             self,
-            decode=decode,
         )
 
     def new_jobid(self, possible_id: str | None = None) -> str:
         # find a unique job id based on user input first
         # the randomly generate new ones
         jobid = (
             self.create_jobid()
             if possible_id is None or not self.check_dir
             else slugify(possible_id)
         )
         if self.check_dir:
-            locate = self.locate(jobid, decode=False)
+            locate = self.locate(jobid)
             while locate.is_in_use():
                 jobid = self.create_jobid()
-                locate = self.locate(jobid, decode=False)
+                locate = self.locate(jobid)
         return jobid
 
     def prefix_jobid(self, prefix: str, ext: int = 6) -> str:
         prefix = chop(slugify(prefix), self.max_length)
         # pad out with random string
         # ext = self.max_length - len(prefix) + ext
         jobid = prefix + "-" + self.create_short_jobid(ext)
         if self.check_dir:
-            locate = self.locate(jobid, decode=False)
+            locate = self.locate(jobid)
             while locate.is_in_use():
                 jobid = prefix + "-" + self.create_short_jobid(ext)
-                locate = self.locate(jobid, decode=False)
+                locate = self.locate(jobid)
         return jobid
 
     def create_jobid(self) -> str:
         return create_jobid()
 
     def create_short_jobid(self, n: int = 8) -> str:
         return create_short_jobid(n)
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/logger.py` & `protein_turnover_website-0.4.0/protein_turnover_website/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     if not admins:
         return
     if isinstance(admins, str):
         admins = [admins]
 
     frm = admins[0].split("@")[-1]
     name = app.config.get("MAIL_SUBJECT", app.name)
-    mailhost = app.config.get("MAIL_SERVER", "localhost")
+    mailhost = app.config.get("MAIL_SERVER", "mailhost")
     if not mailhost:
         return
     if isinstance(mailhost, str) and ":" in mailhost:
         mailhost = mailhost.split(":")
         mailhost = (mailhost[0], int(mailhost[1]))
     mail_handler = Cls(
         mailhost,
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/login/login_view.py` & `protein_turnover_website-0.4.0/protein_turnover_website/login/login_view.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/login/templates/login.html` & `protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/login/templates/login.js` & `protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/login/templates/login.ts` & `protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/sqla/export.py` & `protein_turnover_website-0.4.0/protein_turnover_website/sqla/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pandas as pd
 from flask import abort
 from flask import current_app
 from flask import request
 from flask import Response
 from flask import send_file
-from protein_turnover.config import RESULT_EXT
+from protein_turnover.exts import RESULT_EXT
 from protein_turnover.sqla.query import Aggregate
 from protein_turnover.sqla.query import FormFilter
 from protein_turnover.sqla.query import RowFilter
 from typing_extensions import override
 from werkzeug.utils import secure_filename
 
 from ..inspect import Column
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/sqla/export.toml` & `protein_turnover_website-0.4.0/protein_turnover_website/sqla/export.toml`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/sqla/inspect.py` & `protein_turnover_website-0.4.0/protein_turnover_website/sqla/inspect.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/sqla/peptides.toml` & `protein_turnover_website-0.4.0/protein_turnover_website/sqla/peptides.toml`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/sqla/proteins.toml` & `protein_turnover_website-0.4.0/protein_turnover_website/sqla/proteins.toml`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/static/img/UWA-Full-Hor-CMYK-wt-opt.svgz` & `protein_turnover_website-0.4.0/protein_turnover_website/static/img/UWA-Full-Hor-CMYK-wt-opt.svgz`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/static/img/about/eics.png` & `protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/eics.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/static/img/about/isotopeEnvelopes.png` & `protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/isotopeEnvelopes.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/static/img/about/labelledEnvelope.png` & `protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/labelledEnvelope.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/static/img/about/plotFittedEnvelopes.png` & `protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/plotFittedEnvelopes.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/static/img/email-white.svgz` & `protein_turnover_website-0.4.0/protein_turnover_website/static/img/email-white.svgz`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/static/img/enrichment.png` & `protein_turnover_website-0.4.0/protein_turnover_website/static/img/enrichment.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/static/img/nnls_residuals.png` & `protein_turnover_website-0.4.0/protein_turnover_website/static/img/nnls_residuals.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/static/img/turnover.png` & `protein_turnover_website-0.4.0/protein_turnover_website/static/img/turnover.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/static/img/wheat4.jpg` & `protein_turnover_website-0.4.0/protein_turnover_website/static/img/wheat4.jpg`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/about-frag.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/about-frag.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/about-orig.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/about-orig.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/about.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/about.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/about.md.tplt` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/about.md.tplt`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/configuration.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/configuration.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/errors/404.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/errors/404.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/filter-frag.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/filter-frag.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/email.svg` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/email.svg`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/macros.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/macros.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/meta.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/meta.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/range.css` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.css`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/range.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/range.js` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/range.ts` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/fragments/theme.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/theme.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/inspect-download.js` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect-download.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/inspect-download.ts` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect-download.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/inspect.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/inspect.js` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -182,15 +182,15 @@
 
     function add_pep_filters(d) {
         d.filters = serializeForm(filterid);
         d.exclude = filter_peptides;
     }
 
     function make_url(url, rowid) {
-        return url + '?' + $.param({
+        return url + "?" + $.param({
             rowid
         });
         // return url.replace(/\/-1$/, `/${rowid}`)
     }
 
     function clear_datatable() {
         if (dt !== null) {
@@ -314,24 +314,24 @@
         return;
     }
 
     function refresh_enrichment() {
         const data = filter_peptides ? {
             filters: serializeForm(filterid)
         } : {};
-        return $.get(Config.enrichment_url, data).then((json) => {
+        return $.post(Config.enrichment_url, data).then((json) => {
             $enrichment_image.attr("src", json.enrichment_url);
         });
     }
 
     function refresh_nnls() {
         const data = filter_peptides ? {
             filters: serializeForm(filterid)
         } : {};
-        return $.get(Config.nnls_url, data).then((json) => {
+        return $.post(Config.nnls_url, data).then((json) => {
             $nnls_image.attr("src", json.nnls_url);
         });
     }
 
     function get_stats() {
         const $resid = $form.find('input[name="nnlsResidual"]');
         const $area = $form.find('input[name="maxPeakArea"]');
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/inspect.ts` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.ts`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
     }
     function add_pep_filters(d: any) {
         d.filters = serializeForm(filterid)
         d.exclude = filter_peptides
     }
 
     function make_url(url: string, rowid: string): string {
-        return url + '?' + $.param({rowid})
+        return url + "?" + $.param({ rowid })
         // return url.replace(/\/-1$/, `/${rowid}`)
     }
 
     function clear_datatable(): JQuery<HTMLElement> {
         if (dt !== null) {
             dt.destroy()
             dt = null
@@ -368,23 +368,23 @@
             dt!.search("").draw()
         }
         return
     }
 
     function refresh_enrichment() {
         const data = filter_peptides ? { filters: serializeForm(filterid) } : {}
-        return $.get(Config.enrichment_url, data).then((json) => {
+        return $.post(Config.enrichment_url, data).then((json) => {
             $enrichment_image.attr("src", json.enrichment_url)
         })
     }
 
     function refresh_nnls() {
         const data = filter_peptides ? { filters: serializeForm(filterid) } : {}
 
-        return $.get(Config.nnls_url, data).then((json) => {
+        return $.post(Config.nnls_url, data).then((json) => {
             $nnls_image.attr("src", json.nnls_url)
         })
     }
 
     function get_stats() {
         const $resid = $form.find('input[name="nnlsResidual"]')
         const $area = $form.find('input[name="maxPeakArea"]')
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/job-frag.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/job-frag.html`

 * *Files 3% similar despite different names*

```diff
@@ -62,19 +62,19 @@
 
         </div>
     </td>
 </tr>
 {% endmacro %}
 
 {# data:TurnoverJobFiles #}
-{% macro jobinfo(data, current_user) %}
+{% macro jobinfo(data, oktokill) %}
 <div class="btn-group">
     <button class="btn btn-sm btn-outline-info" data-view="true" title="show job info">Job</button>
     <button class="btn btn-sm btn-outline-secondary" data-log="true" title="show logs">Logs</button>
-    {% if config.KILL_OK or current_user.is_authenticated %}
+    {% if oktokill %}
         {% if data.is_running %}
         <button class="btn btn-sm btn-outline-danger" data-kill="true" title="stop this job"><i
                 class="fas fa-power-off"></i></button>
         {% elif data.status == 'killed' %}
         <button class="btn btn-sm btn-outline-success" data-restart="true" title="restart this job"><i
                 class="fas fa-redo"></i></button>
         <button class="btn btn-sm btn-outline-danger" data-remove="true" title="remove this job"><i
@@ -84,15 +84,15 @@
                 class="far fa-trash-alt"></i></button>
         {% endif %}
     {% endif %}
 </div>
 
 {% endmacro %}
 {# results:list[TurnoverJobFiles] #}
-{% macro jobtable(results, current_user) %}
+{% macro jobtable(results, oktokill) %}
 {% if results|length > 0 %}
 <table class="table">
     <thead>
         <tr>
             <th>has result</th>
             <th>job name</th>
             <th>status</th>
@@ -115,15 +115,15 @@
             <td>
                 <span class="{{data.status}}">{{data.status}}</span>
             </td>
             <td>
                 {{data.job.email or 'no email'}}
             </td>
             <td>
-                {{jobinfo(data, current_user)}}
+                {{jobinfo(data, oktokill)}}
             </td>
             <td>{{data.size|human}}</td>
             <td>{{data.mtime.strftime('%Y-%m-%d %H:%M:%S')}}</td>
         </tr>
         {% endfor %}
     </tbody>
 </table>
```

#### html2text {}

```diff
@@ -7,22 +7,20 @@
 {% endmacro %} {# type: loglist:list[LogRecord] #} {% macro showlog(loglist) %}
 Close {% if loglist %}
 ttiimmee                                       lleevveell         mmeessssaaggee
 {{rec.time.strftime('%Y-%m-%d %H:%M:%S')}} {{rec.level}} {{rec.msg}}
 {% else %}
 **** NNoo LLooggss ****
 {% endif %}
-{% endmacro %} {# data:TurnoverJobFiles #} {% macro jobinfo(data, current_user)
-%}
-Job Logs {% if config.KILL_OK or current_user.is_authenticated %} {% if
-data.is_running %} {% elif data.status == 'killed' %} {% elif data.status ==
-'failed' %} {% endif %} {% endif %}
+{% endmacro %} {# data:TurnoverJobFiles #} {% macro jobinfo(data, oktokill) %}
+Job Logs {% if oktokill %} {% if data.is_running %} {% elif data.status ==
+'killed' %} {% elif data.status == 'failed' %} {% endif %} {% endif %}
 {% endmacro %} {# results:list[TurnoverJobFiles] #} {% macro jobtable(results,
-current_user) %} {% if results|length > 0 %}
-hhaass rreessuulltt      jjoobb nnaammee             ssttaattuuss         eemmaaiill           iinnffoo            ssiizzee               llaasstt mmooddiiffiieedd
-{% if                                               {                                                  {
-data.has_result {                    {              {data.job.email {{jobinfo(data, {                  {data.mtime.strftime
-%} _v_i_e_w_ _r_e_s_u_l_t  {data.job.job_name}} {data.status}} or 'no email'}} current_user)}} {data.size|human}} ('%Y-%m-%d %H:%M:
-{% endif %}                                                                                            %S')}}
+oktokill) %} {% if results|length > 0 %}
+hhaass rreessuulltt      jjoobb nnaammee             ssttaattuuss         eemmaaiill           iinnffoo        ssiizzee               llaasstt mmooddiiffiieedd
+{% if                                               {               {{jobinfo                      {
+data.has_result {                    {              {data.job.email (data,      {                  {data.mtime.strftime
+%} _v_i_e_w_ _r_e_s_u_l_t  {data.job.job_name}} {data.status}} or 'no email'}} oktokill)}} {data.size|human}} ('%Y-%m-%d %H:%M:
+{% endif %}                                                                                        %S')}}
 {% else %} {#
 No jobs
 #} {% endif %} {% endmacro %}
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/job-index.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.html`

 * *Files 6% similar despite different names*

```diff
@@ -45,25 +45,25 @@
         if you are expecting your job
         to be running.</p>
     {% endif %}
 
     <h2>Jobs Running</h2>
     <hr />
     <div id="jobs-running" class="jobs-table">
-        {{ macros.jobtable(running, current_user) }}
+        {{ macros.jobtable(running, oktokill) }}
     </div>
     <h2>Jobs Queued</h2>
     <hr />
     <div id="jobs-queued" class="jobs-table">
-        {{ macros.jobtable(queued, current_user) }}
+        {{ macros.jobtable(queued, oktokill) }}
     </div>
     <h2>Jobs Done</h2>
     <hr />
     <div id="jobs-finished" class="jobs-table">
-        {{ macros.jobtable(finished, current_user) }}
+        {{ macros.jobtable(finished, oktokill) }}
     </div>
 </div>
 
 {% endblock content %}
 
 {% block js %}
 {{super()}}
```

#### html2text {}

```diff
@@ -9,18 +9,18 @@
 {% else %}
 The current job scheduler only wakes every 60 seconds to check for new jobs to
 run. Either refresh this page or press this button refresh if you are expecting
 your job to be running.
 {% endif %}
 ********** JJoobbss RRuunnnniinngg **********
 ===============================================================================
-{{ macros.jobtable(running, current_user) }}
+{{ macros.jobtable(running, oktokill) }}
 ********** JJoobbss QQuueeuueedd **********
 ===============================================================================
-{{ macros.jobtable(queued, current_user) }}
+{{ macros.jobtable(queued, oktokill) }}
 ********** JJoobbss DDoonnee **********
 ===============================================================================
-{{ macros.jobtable(finished, current_user) }}
+{{ macros.jobtable(finished, oktokill) }}
 {% endblock content %} {% block js %} {{super()}} {{cdn_js('datatables')}} {
 {cdn_js('datatables-select')}} {# https://datatables.net/reference/event/error
 #}
 {% endblock js %}
```

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/job-index.js` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/job-index.ts` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/jobs.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/jobs.js` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/jobs.ts` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/macros/spinner.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/macros/spinner.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/raw.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/raw.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/templates/table_meta.html` & `protein_turnover_website-0.4.0/protein_turnover_website/templates/table_meta.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/protein_turnover_website/utils.py` & `protein_turnover_website-0.4.0/protein_turnover_website/utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.3.12/pyproject.toml` & `protein_turnover_website-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protein-turnover-website"
-version = "0.3.12"
+version = "0.4.0"
 description = "Protein Turnover web pipeline"
 authors = ["Ian Castleden <ian.castleden@uwa.edu.au>"]
 license = "MIT"
 readme = "prerelease.md"
 exclude = ["tests/**"]
 packages = [{ include = "protein_turnover_website" }]
 repository = "https://github.com/arabidopsis/protein_turnover_website.git"
@@ -19,19 +19,20 @@
 Flask = "^3.0"
 python-dotenv = "^0.20.0"
 # For DataFrame.to_excel()
 openpyxl = ">=3.0.10"
 Flask-Login = ">=0.6"
 # for background job in protein_turnover
 psutil = ">=5.9"
+unidecode = "^1.3.8"
 
 # protein-turnover = { path = "../protein_turnover", develop = true }
 # poetry add git+ssh://git@github.com:arabidopsis/protein_turnover.git
 # protein-turnover = {git = "git@github.com:arabidopsis/protein_turnover.git"}
-protein-turnover = "^0.3.12"
+protein-turnover = "^0.4.0"
 typing-extensions = "^4.8"
 # these dependencies of protein_turnover
 tomli-w = ">=1.0.0"
 # for inspect
 tomli = ">=2.0.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `protein_turnover_website-0.3.12/PKG-INFO` & `protein_turnover_website-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-turnover-website
-Version: 0.3.12
+Version: 0.4.0
 Summary: Protein Turnover web pipeline
 Home-page: https://github.com/arabidopsis/protein_turnover_website.git
 License: MIT
 Author: Ian Castleden
 Author-email: ian.castleden@uwa.edu.au
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
@@ -15,20 +15,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: Flask (>=3.0,<4.0)
 Requires-Dist: Flask-Login (>=0.6)
 Requires-Dist: openpyxl (>=3.0.10)
-Requires-Dist: protein-turnover (>=0.3.12,<0.4.0)
+Requires-Dist: protein-turnover (>=0.4.0,<0.5.0)
 Requires-Dist: psutil (>=5.9)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: tomli (>=2.0.1)
 Requires-Dist: tomli-w (>=1.0.0)
 Requires-Dist: typing-extensions (>=4.8,<5.0)
+Requires-Dist: unidecode (>=1.3.8,<2.0.0)
 Project-URL: Repository, https://github.com/arabidopsis/protein_turnover_website.git
 Description-Content-Type: text/markdown
 
 # Protein Turnover Pipeline
 
 More documentation soon.
```

