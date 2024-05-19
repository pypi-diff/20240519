# Comparing `tmp/aa_ledger-0.3.4.tar.gz` & `tmp/aa_ledger-0.3.5.tar.gz`

## Comparing `aa_ledger-0.3.4.tar` & `aa_ledger-0.3.5.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/admin.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/app_settings.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/apps.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/auth_hooks.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/decorators.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/errors.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/hooks.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/providers.py
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/tasks.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/urls.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/__init__.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/helpers.py
--rw-r--r--   0        0        0    21609 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/ledgermanager.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/schema.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/character/__init__.py
--rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/character/ledger.py
--rw-r--r--   0        0        0    15634 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/character/template.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/corporation/__init__.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/corporation/ledger.py
--rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/corporation/template.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/managers/charaudit_manager.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/managers/corpaudit_manager.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/managers/general_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/migrations/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/models/__init__.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/models/characteraudit.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/models/corporationaudit.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/models/events.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/models/general.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/css/billboards_dark.css
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/css/cards.css
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/css/custom.css
--rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-1.png
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-2.png
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-3.png
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0    22084 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/js/charledger.js
--rw-r--r--   0        0        0    18891 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/js/corpledger.js
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/js/img.js
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/task_helpers/__init__.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/task_helpers/char_helpers.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/task_helpers/core_helpers.py
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/task_helpers/corp_helpers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/task_helpers/etag_helpers.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/base.html
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/error.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/bundles/ledger-css.html
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/base.html
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/index.html
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/menu.html
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/char_ledger.html
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/month.html
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/year.html
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/corp_ledger.html
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/month.html
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/year.html
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/modals/modal-full.html
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/modals/modal-xl.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/modals/modal.html
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/modals/modal_dialog.html
--rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/modals/pve/view_character_content.html
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/view_helpers/__init__.py
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/view_helpers/core.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/__init__.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/pve.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/character/char_audit.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/corporation/corp_audit.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/corporation/corp_events.py
--rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/corporation/corp_tax.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/LICENSE
--rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/README.md
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/admin.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/app_settings.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/apps.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/auth_hooks.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/decorators.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/errors.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/hooks.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/providers.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/tasks.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/urls.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/api/__init__.py
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/api/helpers.py
+-rw-r--r--   0        0        0    21350 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/api/ledgermanager.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/api/schema.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/api/templatemanager.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/api/character/__init__.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/api/character/ledger.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/api/character/template.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/api/corporation/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/api/corporation/ledger.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/api/corporation/template.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/managers/charaudit_manager.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/managers/corpaudit_manager.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/managers/general_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/migrations/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/models/__init__.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/models/characteraudit.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/models/corporationaudit.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/models/events.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/models/general.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/static/ledger/css/billboards_dark.css
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/static/ledger/css/cards.css
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/static/ledger/css/custom.css
+-rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/static/ledger/guides/ledger-1.png
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/static/ledger/guides/ledger-2.png
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/static/ledger/guides/ledger-3.png
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/static/ledger/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/static/ledger/js/charledger.js
+-rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/static/ledger/js/corpledger.js
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/static/ledger/js/img.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/task_helpers/__init__.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/task_helpers/char_helpers.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/task_helpers/core_helpers.py
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/task_helpers/corp_helpers.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/task_helpers/etag_helpers.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/base.html
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/error.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/bundles/ledger-css.html
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/ledger/base.html
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/ledger/index.html
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/ledger/menu.html
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/ledger/charledger/char_ledger.html
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/ledger/charledger/month.html
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/ledger/charledger/year.html
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/ledger/corpledger/corp_ledger.html
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/ledger/corpledger/month.html
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/ledger/corpledger/year.html
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/modals/modal-full.html
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/modals/modal-xl.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/modals/modal.html
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/modals/modal_dialog.html
+-rw-r--r--   0        0        0    17661 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/templates/ledger/modals/pve/view_character_content.html
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/view_helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/view_helpers/core.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/views/__init__.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/views/pve.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/views/character/char_audit.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/views/corporation/corp_audit.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/views/corporation/corp_events.py
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/ledger/views/corporation/corp_tax.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/LICENSE
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/README.md
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 aa_ledger-0.3.5/PKG-INFO
```

### Comparing `aa_ledger-0.3.4/ledger/admin.py` & `aa_ledger-0.3.5/ledger/admin.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/app_settings.py` & `aa_ledger-0.3.5/ledger/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/auth_hooks.py` & `aa_ledger-0.3.5/ledger/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/decorators.py` & `aa_ledger-0.3.5/ledger/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/hooks.py` & `aa_ledger-0.3.5/ledger/hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/tasks.py` & `aa_ledger-0.3.5/ledger/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 @shared_task
 @when_esi_is_available
 def update_all_characters(runs: int = 0):
     characters = CharacterAudit.objects.select_related("character").all()
     for char in characters:
         update_character.apply_async(args=[char.character.character_id])
         runs = runs + 1
-    logger.info("Queued %s Audit Updates", runs)
+    logger.info("Queued %s Char Audit Updates", runs)
 
 
 @shared_task(bind=True, base=QueueOnce)
 def update_character(
     self, char_id, force_refresh=False
 ):  # pylint: disable=unused-argument
     character = (
```

### Comparing `aa_ledger-0.3.4/ledger/urls.py` & `aa_ledger-0.3.5/ledger/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     path("char/add/", add_char, name="ledger_add_char"),
     re_path(
         r"^char/fetch_memberaudit/", fetch_memberaudit, name="ledger_fetch_memberaudit"
     ),
     # -- Corporation Audit
     path("corporation/add/", add_corp, name="ledger_add_corp"),
     # -- PvE
-    path("ledger/index", ledger_index, name="ledger_index"),
+    path("index", ledger_index, name="ledger_index"),
     # -- -- Steuer
     path("steuer/index", index_steuer, name="steuer_index"),
     # -- -- Corporation Ledger
-    path("ledger/corp_index", ratting_index, name="ledger_corp_index"),
+    path("corp_index", ratting_index, name="ledger_corp_index"),
     # -- -- Char Ledger
-    path("ledger/char_index", ratting_char_index, name="ledger_char_index"),
+    path("char_index", ratting_char_index, name="ledger_char_index"),
     # -- -- Events
     path("events/", events_index, name="events_index"),
     path("events/admin/", events_admin, name="event_admin"),
     path("events/create/", create_event, name="create_event"),
     path("events/<int:event_id>/edit/", edit_event, name="edit_event"),
     path("events/<int:event_id>/delete/", delete_event, name="delete_event"),
     path("events/ajax/load_events", load_events, name="load_events"),
```

### Comparing `aa_ledger-0.3.4/ledger/api/__init__.py` & `aa_ledger-0.3.5/ledger/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/api/helpers.py` & `aa_ledger-0.3.5/ledger/api/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models import QuerySet
 
 from allianceauth.authentication.models import UserProfile
 from allianceauth.eveonline.models import EveCharacter
 
 from ledger import app_settings, models
-from ledger.hooks import get_extension_logger
 
 if app_settings.LEDGER_CORPSTATS_TWO:
     from corpstats.models import CorpMember
 else:
     from allianceauth.corputils.models import CorpMember
 
+from ledger.hooks import get_extension_logger
+
 logger = get_extension_logger(__name__)
 
 
 class Paginator(LimitOffsetPagination):
     class Input(Schema):
         limit: int = Field(30000, ge=1)
         offset: int = Field(0, ge=0)
@@ -35,14 +36,39 @@
         limit: int = pagination.limit
         return {
             "items": queryset[offset : offset + limit],
             "count": self._items_count(queryset),
         }
 
 
+# pylint: disable=import-outside-toplevel
+def get_models_and_string():
+    if app_settings.LEDGER_MEMBERAUDIT_USE:
+        from memberaudit.models import (
+            CharacterMiningLedgerEntry as CharacterMiningLedger,
+        )
+        from memberaudit.models import CharacterWalletJournalEntry
+
+        return (
+            CharacterMiningLedger,
+            CharacterWalletJournalEntry,
+            "character__character",
+        )
+    from ledger.models.characteraudit import (
+        CharacterMiningLedger,
+        CharacterWalletJournalEntry,
+    )
+
+    return (
+        CharacterMiningLedger,
+        CharacterWalletJournalEntry,
+        "character__eve_character",
+    )
+
+
 def get_main_character(request, character_id):
     perms = True
 
     main_char = EveCharacter.objects.select_related(
         "character_ownership",
         "character_ownership__user__profile",
         "character_ownership__user__profile__main_character",
```

### Comparing `aa_ledger-0.3.4/ledger/api/ledgermanager.py` & `aa_ledger-0.3.5/ledger/api/ledgermanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,34 +2,23 @@
 from datetime import datetime
 from decimal import Decimal
 
 from django.db.models import DecimalField, F, Q, Sum
 from django.db.models.functions import Coalesce
 
 from ledger import app_settings
-from ledger.models.corporationaudit import CorporationWalletJournalEntry
-
-if app_settings.LEDGER_MEMBERAUDIT_USE:
-    from memberaudit.models import CharacterMiningLedgerEntry as CharacterMiningLedger
-    from memberaudit.models import CharacterWalletJournalEntry
-
-    SR_CHAR = "character__character"
-else:
-    from ledger.models.characteraudit import (
-        CharacterMiningLedger,
-        CharacterWalletJournalEntry,
-    )
-
-    SR_CHAR = "character__eve_character"
-
+from ledger.api.helpers import get_models_and_string
 from ledger.hooks import get_extension_logger
+from ledger.models.corporationaudit import CorporationWalletJournalEntry
 from ledger.view_helpers.core import events_filter
 
 logger = get_extension_logger(__name__)
 
+CharacterMiningLedger, CharacterWalletJournalEntry, SR_CHAR = get_models_and_string()
+
 
 class LedgerDataCore:
     """LedgerDataCore class to store the core data."""
 
     def __init__(self, models):
         self.ess_entries, self.entries, self.mining_data = models
         self.total_bounty = 0
```

### Comparing `aa_ledger-0.3.4/ledger/api/schema.py` & `aa_ledger-0.3.5/ledger/api/schema.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/api/character/ledger.py` & `aa_ledger-0.3.5/ledger/api/character/ledger.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                         "reason": w.reason,
                     }
                 )
 
             return output
 
         @api.get(
-            "account/{character_id}/ledger/year/{year}/month/{month}",
+            "account/{character_id}/ledger/year/{year}/month/{month}/",
             response={200: List[schema.CharacterLedger], 403: str},
             tags=self.tags,
         )
         @paginate(Paginator)
         def get_character_ledger(request, character_id: int, year: int, month: int):
             if character_id == 0:
                 character_id = request.user.profile.main_character.character_id
```

### Comparing `aa_ledger-0.3.4/ledger/api/corporation/ledger.py` & `aa_ledger-0.3.5/ledger/api/corporation/ledger.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                         "reason": w.reason,
                     }
                 )
 
             return output
 
         @api.get(
-            "corporation/{corporation_id}/ledger/year/{year}/month/{month}",
+            "corporation/{corporation_id}/ledger/year/{year}/month/{month}/",
             response={200: List[schema.CorporationLedger], 403: str},
             tags=self.tags,
         )
         @paginate(Paginator)
         def get_corporation_ledger(request, corporation_id: int, year: int, month: int):
             perms = request.user.has_perm("ledger.basic_access")
```

### Comparing `aa_ledger-0.3.4/ledger/api/corporation/template.py` & `aa_ledger-0.3.5/ledger/task_helpers/char_helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,182 +1,211 @@
-from datetime import datetime
-from typing import List
+"""
+Character Helpers
+"""
+
+import time
+from datetime import timedelta
+
+from django.utils import timezone
+from esi.models import Token
+from eveuniverse.models import EveType
 
-from ninja import NinjaAPI
-
-from django.db.models import Q
-from django.shortcuts import render
-
-from ledger.api import schema
-from ledger.api.helpers import get_corporations, get_main_and_alts_all
+from ledger import providers
+from ledger.errors import TokenError
 from ledger.hooks import get_extension_logger
-from ledger.models.corporationaudit import CorporationWalletJournalEntry
-from ledger.view_helpers.core import (
-    calculate_days_year,
-    calculate_ess_stolen,
-    calculate_journal,
+from ledger.models.characteraudit import (
+    CharacterAudit,
+    CharacterMiningLedger,
+    CharacterWalletJournalEntry,
 )
+from ledger.models.general import EveEntity
+from ledger.task_helpers.etag_helpers import NotModifiedError, etag_results
 
 logger = get_extension_logger(__name__)
 
 
-# TODO Refactor this class
-# pylint: disable=too-many-locals, too-many-branches, too-many-statements
-class LedgerTemplateApiEndpoints:
-    tags = ["CorporationLedgerTemplate"]
-
-    def __init__(self, api: NinjaAPI):
-
-        @api.get(
-            "corporation/{main_id}/ledger/template/year/{year}/month/{month}",
-            response={200: List[schema.CharacterLedgerTemplate], 403: str},
-            tags=self.tags,
-        )
-        def get_corporation_ledger_template(
-            request, main_id: int, year: int, month: int
-        ):
-            overall_mode = False
-
-            perms = request.user.has_perm("ledger.basic_access")
-
-            if main_id == 0:
-                overall_mode = True
-
-            if not perms:
-                logger.error(
-                    "Permission Denied for %s to view corporation ledger template!",
-                    request.user,
+def get_token(character_id: int, scopes: list) -> "Token":
+    """
+    Helper method to get a valid token for a specific character with specific scopes.
+
+    Parameters
+    ----------
+    character_id: `int`
+    scopes: `int`
+
+    Returns
+    ----------
+    `class`: esi.models.Token or False
+
+    """
+    token = (
+        Token.objects.filter(character_id=character_id)
+        .require_scopes(scopes)
+        .require_valid()
+        .first()
+    )
+    if token:
+        return token
+    return False
+
+
+# pylint: disable=too-many-locals
+def update_character_wallet(character_id, force_refresh=False):
+    audit_char = CharacterAudit.objects.get(character__character_id=character_id)
+    logger.debug(
+        "Updating wallet transactions for: %s", audit_char.character.character_name
+    )
+
+    req_scopes = ["esi-wallet.read_character_wallet.v1"]
+
+    token = get_token(character_id, req_scopes)
+
+    if not token:
+        return "No Tokens"
+
+    try:
+        journal_items_ob = (
+            providers.esi.client.Wallet.get_characters_character_id_wallet_journal(
+                character_id=character_id
+            )
+        )
+
+        journal_items = etag_results(
+            journal_items_ob, token, force_refresh=force_refresh
+        )
+
+        _st = time.perf_counter()
+        _current_journal = CharacterWalletJournalEntry.objects.filter(
+            character=audit_char
+        ).values_list(
+            "entry_id", flat=True
+        )  # TODO add time filter
+        _current_eve_ids = list(
+            EveEntity.objects.all().values_list("eve_id", flat=True)
+        )
+
+        _new_names = []
+
+        items = []
+        for item in journal_items:
+            if item.get("id") not in _current_journal:
+                if item.get("second_party_id") not in _current_eve_ids:
+                    _new_names.append(item.get("second_party_id"))
+                    _current_eve_ids.append(item.get("second_party_id"))
+                if item.get("first_party_id") not in _current_eve_ids:
+                    _new_names.append(item.get("first_party_id"))
+                    _current_eve_ids.append(item.get("first_party_id"))
+
+                # pylint: disable=duplicate-code
+                asset_item = CharacterWalletJournalEntry(
+                    character=audit_char,
+                    amount=item.get("amount"),
+                    balance=item.get("balance"),
+                    context_id=item.get("context_id"),
+                    context_id_type=item.get("context_id_type"),
+                    date=item.get("date"),
+                    description=item.get("description"),
+                    first_party_id=item.get("first_party_id"),
+                    entry_id=item.get("id"),
+                    reason=item.get("reason"),
+                    ref_type=item.get("ref_type"),
+                    second_party_id=item.get("second_party_id"),
+                    tax=item.get("tax"),
+                    tax_receiver_id=item.get("tax_receiver_id"),
                 )
-                return 403, "Permission Denied!"
+                items.append(asset_item)
 
-            current_date = datetime.now()
+        created_names = EveEntity.objects.create_bulk_from_esi(_new_names)
 
-            total_amount = 0
-            total_amount_day = 0
-            total_amount_hour = 0
-            # ESS
-            total_amount_ess = 0
-            total_amount_day_ess = 0
-            total_amount_hour_ess = 0
-
-            current_date = current_date.replace(year=year)
-            if not month == 0:
-                current_date = current_date.replace(month=month)
-
-            current_day = calculate_days_year() if month == 0 else current_date.day
-
-            character_id = request.user.profile.main_character.character_id
-            corporations = get_corporations(request, character_id)
-
-            mains, chars = get_main_and_alts_all(corporations, char_ids=True)
-
-            filters = Q(second_party_id__in=chars)
-            filter_date = Q(date__year=current_date.year)
-            if not month == 0:
-                filter_date &= Q(date__month=current_date.month)
-
-            wallet_journal = (
-                CorporationWalletJournalEntry.objects.filter(filters, filter_date)
-                .select_related("first_party", "second_party", "division")
-                .values("amount", "date", "second_party_id", "ref_type")
-                .order_by("-date")
-            )
+        wallet_ballance = (
+            providers.esi.client.Wallet.get_characters_character_id_wallet(
+                character_id=character_id, token=token.valid_access_token()
+            ).result()
+        )
 
-            if overall_mode:
-                mains_data = mains
-            else:
-                mains_data = {main_id: mains.get(main_id, None)}
+        audit_char.balance = wallet_ballance
+        audit_char.save()
 
-            for _, mains_data in mains_data.items():
-                main = mains_data["main"]
-                alts = mains_data["alts"]
+        if created_names:
+            CharacterWalletJournalEntry.objects.bulk_create(items)
+        else:
+            raise TokenError("ESI Fail")
+        logger.debug(
+            "TIME: %s update_character_wallet %s",
+            time.perf_counter() - _st,
+            character_id,
+        )
+    except NotModifiedError:
+        logger.debug("No New wallet data for: %s", audit_char.character.character_name)
 
-                # Each Chars from a Main Character
-                chars = [alt.character_id for alt in alts] + [main.character_id]
+    audit_char.last_update_wallet = timezone.now()
+    audit_char.save()
+    audit_char.is_active()
 
-                char_name = main.character_name if not main_id == 0 else "Summary"
-                char_id = main.character_id if not main_id == 0 else 0
+    return ("Finished wallet transactions for: %s", audit_char.character.character_name)
 
-                my_filter = Q(second_party_id__in=chars)
-                my_filter_bounty = my_filter & Q(ref_type="bounty_prizes")
-                my_filter_ess_payout = my_filter & Q(ref_type="ess_escrow_transfer")
 
-                amount_ess = calculate_journal(wallet_journal, my_filter_ess_payout)
+def update_character_mining(character_id, force_refresh=False):
+    audit_char = CharacterAudit.objects.get(character__character_id=character_id)
+    logger.debug("Updating Mining for: %s", audit_char.character.character_name)
 
-                amount_bounty = calculate_journal(
-                    wallet_journal,
-                    my_filter_bounty,
-                )
+    req_scopes = ["esi-industry.read_character_mining.v1"]
 
-                # Berechne die Gesamtsumme für alle Charaktere
-                total_amount += amount_bounty["total_amount"]
-                total_amount_day += amount_bounty["total_amount_day"]
-                total_amount_hour += amount_bounty["total_amount_hour"]
-
-                # ESS
-                total_amount_ess += amount_ess["total_amount"]
-                total_amount_day_ess += amount_ess["total_amount_day"]
-                total_amount_hour_ess += amount_ess["total_amount_hour"]
-
-            stolen = 0
-            gain = 0
-
-            # If not 0 then add to Rattingledger
-            if total_amount > 0:
-                stolen, gain = calculate_ess_stolen(total_amount, total_amount_ess)
-
-            day_avg_isk = round(total_amount / current_day)
-            day_avg_ess = round(total_amount_ess / current_day)
-
-            hourly_avg_isk = round((total_amount / current_day) / 24)
-            hourly_avg_ess = round((total_amount_ess / current_day) / 24)
-
-            total_summary = total_amount + total_amount_ess
-            total_summary_day = total_amount_day + total_amount_day_ess
-            total_summary_hour = total_amount_hour + total_amount_hour_ess
-
-            # pylint: disable=duplicate-code
-            summary = {
-                "main_name": char_name,
-                "main_id": char_id,
-                "date": (
-                    str(current_date.year)
-                    if month == 0
-                    else current_date.strftime("%B")
-                ),
-                "summary_isk": total_amount,
-                "summary_ess": total_amount_ess,
-                "summary": total_summary,
-                "day_avg_isk": day_avg_isk,
-                "day_avg_ess": day_avg_ess,
-                "summary_day": total_summary_day,
-                "hourly_avg_isk": hourly_avg_isk,
-                "hourly_avg_ess": hourly_avg_ess,
-                "summary_hour": total_summary_hour,
-            }
-            if not overall_mode:
-                summary.update(
-                    {
-                        "day_isk": total_amount_day,
-                        "day_ess": total_amount_day_ess,
-                        "hourly_isk": total_amount_hour,
-                        "hourly_ess": total_amount_hour_ess,
-                    }
-                )
-            if stolen:
-                day_stolen = round(stolen / current_date.day)
-                hourly_stolen = round((stolen / current_date.day) / 24)
-
-                summary.update(
-                    {
-                        "gain": gain,
-                        "stolen": stolen,
-                        "day_stolen": day_stolen,
-                        "hourly_stolen": hourly_stolen,
-                    }
-                )
+    token = get_token(character_id, req_scopes)
+
+    if not token:
+        return "No Tokens"
+    try:
+        mining_op = providers.esi.client.Industry.get_characters_character_id_mining(
+            character_id=character_id
+        )
 
-            context = {"character": summary}
+        ledger = etag_results(mining_op, token, force_refresh=force_refresh)
 
-            return render(
-                request, "ledger/modals/pve/view_character_content.html", context
+        _st = time.perf_counter()
+        existings_pks = set(
+            CharacterMiningLedger.objects.filter(
+                character=audit_char, date__gte=timezone.now() - timedelta(days=30)
+            ).values_list("id", flat=True)
+        )
+        type_ids = set()
+        new_events = []
+        old_events = []
+        for event in ledger:
+
+            type_ids.add(event.get("type_id"))
+            pk = CharacterMiningLedger.create_primary_key(character_id, event)
+            _e = CharacterMiningLedger(
+                character=audit_char,
+                id=pk,
+                date=event.get("date"),
+                type_id=event.get("type_id"),
+                system_id=event.get("solar_system_id"),
+                quantity=event.get("quantity"),
             )
+            if pk in existings_pks:
+                old_events.append(_e)
+            else:
+                new_events.append(_e)
+
+        EveType.objects.bulk_get_or_create_esi(ids=list(type_ids))
+
+        if new_events:
+            CharacterMiningLedger.objects.bulk_create(new_events, ignore_conflicts=True)
+
+        if old_events:
+            CharacterMiningLedger.objects.bulk_update(old_events, fields=["quantity"])
+
+        logger.debug(
+            "TIME: %s update_character_mining %s",
+            time.perf_counter() - _st,
+            character_id,
+        )
+
+    except NotModifiedError:
+        logger.debug("No New Mining for: %s", audit_char.character.character_name)
+
+    audit_char.last_update_mining = timezone.now()
+    audit_char.save()
+    audit_char.is_active()
+
+    return f"Finished Mining for: {audit_char.character.character_name}"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_ledger-0.3.4/ledger/managers/charaudit_manager.py` & `aa_ledger-0.3.5/ledger/managers/charaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/managers/corpaudit_manager.py` & `aa_ledger-0.3.5/ledger/managers/corpaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/managers/general_manager.py` & `aa_ledger-0.3.5/ledger/managers/general_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/models/characteraudit.py` & `aa_ledger-0.3.5/ledger/models/characteraudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/models/corporationaudit.py` & `aa_ledger-0.3.5/ledger/models/corporationaudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/models/events.py` & `aa_ledger-0.3.5/ledger/models/events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/models/general.py` & `aa_ledger-0.3.5/ledger/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/static/ledger/css/billboards_dark.css` & `aa_ledger-0.3.5/ledger/static/ledger/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/static/ledger/css/cards.css` & `aa_ledger-0.3.5/ledger/static/ledger/css/cards.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/static/ledger/css/custom.css` & `aa_ledger-0.3.5/ledger/static/ledger/css/custom.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-1.png` & `aa_ledger-0.3.5/ledger/static/ledger/guides/ledger-1.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-2.png` & `aa_ledger-0.3.5/ledger/static/ledger/guides/ledger-2.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-3.png` & `aa_ledger-0.3.5/ledger/static/ledger/guides/ledger-3.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/static/ledger/images/Spinner-1s-64px-dark.gif` & `aa_ledger-0.3.5/ledger/static/ledger/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/static/ledger/images/Spinner-1s-64px-light.gif` & `aa_ledger-0.3.5/ledger/static/ledger/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/static/ledger/js/charledger.js` & `aa_ledger-0.3.5/ledger/static/ledger/js/charledger.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -14,15 +14,15 @@
 
     $('#monthDropdown').change(function() {
         selectedMonth = $(this).val(); // Ausgewählter Monat auslesen
         var selectedYear = currentYear; // Hier die Logik zum Auslesen des ausgewählten Jahres implementieren, falls nötig
         var monthText = getMonthName(selectedMonth);
 
         // URL für die Daten der ausgewählten Kombination von Jahr und Monat erstellen
-        var url = '/ledger/api/account/0/ledger/year/' + selectedYear + '/month/' + selectedMonth;
+        var url = '/ledger/api/account/0/ledger/year/' + selectedYear + '/month/' + selectedMonth + '/';
 
         // DataTable neu laden mit den Daten des ausgewählten Monats
         MonthTable.ajax.url(url).load();
         $('#currentMonthLink').text('Month - ' + monthText);
     });
 
     function getMonthName(monthNumber) {
@@ -54,15 +54,15 @@
         // Rückgabe des formatierten Strings mit Farbe und Einheit
         return '<span style="color: ' + color + ';">' + formattedValue + '</span> ISK';
     }
 
     // Initialize DataTable for current_month
     var MonthTable = $('#ratting').DataTable({
         ajax: {
-            url: '/ledger/api/account/0/ledger/year/' + currentYear + '/month/' + selectedMonth + '',
+            url: '/ledger/api/account/0/ledger/year/' + currentYear + '/month/' + selectedMonth + '/',
             dataSrc: function(data) {
                 // Zusätzliche Daten im DataTable-Objekt speichern
                 total_amount = data.items[0].total.total_amount;
                 total_amount_ess = data.items[0].total.total_amount_ess;
                 total_amount_others = data.items[0].total.total_amount_others;
                 total_amount_mining = data.items[0].total.total_amount_mining;
                 total_amount_combined = data.items[0].total.total_amount_all;
@@ -216,15 +216,15 @@
             {
                 data: 'col-total-action',
                 render: function(data, type, row) {
                     return '<button class="btn btn-sm btn-info btn-square" ' +
                         'data-bs-toggle="modal" ' +
                         'data-bs-target="#modalViewCharacterContainer" ' +
                         'aria-label="' + row.main_name + '" ' +
-                        'data-ajax_url="/ledger/api/account/' + row.main_id + '/ledger/template/year/' + currentYear + '/month/' + selectedMonth + '" ' +
+                        'data-ajax_url="/ledger/api/account/' + row.main_id + '/ledger/template/year/' + currentYear + '/month/' + selectedMonth + '/" ' +
                         'title="' + row.main_name + '">' +
                         '<span class="fas fa-info"></span>' +
                         '</button>';
                 }
             },
         ],
         order: [
@@ -244,29 +244,29 @@
             $('#foot .col-total-amount').html('' + formatAndColor(totalAmountAllChars) + '');
             $('#foot .col-total-ess').html('' + formatAndColor(totalEssAmountAllChars) + '');
             $('#foot .col-total-mining').html('' + formatAndColor(totalMiningAmountAllChars) + '');
             $('#foot .col-total-others').html('' + formatAndColor(totalOthersAmountAllChars) + '');
             $('#foot .col-total-gesamt').html('' + formatAndColor(totalCombinedAmountAllChars) + '');
             $('#foot .col-total-button').html('<button class="btn btn-sm btn-info btn-square" data-bs-toggle="modal" data-bs-target="#modalViewCharacterContainer"' +
                 'aria-label="{{ data.main_name }}"' +
-                'data-ajax_url="/ledger/api/account/0/ledger/template/year/' + currentYear + '/month/' + selectedMonth + '" ' +
+                'data-ajax_url="/ledger/api/account/0/ledger/template/year/' + currentYear + '/month/' + selectedMonth + '/" ' +
                 'title="{{ data.main_name }}"> <span class="fas fa-info"></span></button>');
         },
     });
 
     $('a[data-bs-toggle="tab"]').on('shown.bs.tab', function(e) {
         // Get the id of the tab that was clicked
         var targetTabId = $(e.target).attr('href');
 
         // Check if the clicked tab is the one containing the year DataTable
         if (targetTabId === '#tab-all_month' && !yearTableInitialized) {
             // Initialisiere DataTable für den Hauptinhalt
             var YearTable = $('#ratting_year').DataTable({
                 ajax: {
-                    url: '/ledger/api/account/0/ledger/year/' + currentYear + '/month/0',
+                    url: '/ledger/api/account/0/ledger/year/' + currentYear + '/month/0/',
                     dataSrc: function(data) {
                         // Zusätzliche Daten im DataTable-Objekt speichern
                         total_amount = data.items[0].total.total_amount;
                         total_amount_ess = data.items[0].total.total_amount_ess;
                         total_amount_mining = data.items[0].total.total_amount_mining;
                         total_amount_others = data.items[0].total.total_amount_others;
                         total_amount_combined = data.items[0].total.total_amount_all;
@@ -408,15 +408,15 @@
                     {
                         data: 'col-total-action',
                         render: function(data, type, row) {
                             return '<button class="btn btn-sm btn-info btn-square" ' +
                                 'data-bs-toggle="modal" ' +
                                 'data-bs-target="#modalViewCharacterContainer" ' +
                                 'aria-label="' + row.main_name + '" ' +
-                                'data-ajax_url="/ledger/api/account/' + row.main_id + '/ledger/template/year/' + currentYear + '/month/0" ' +
+                                'data-ajax_url="/ledger/api/account/' + row.main_id + '/ledger/template/year/' + currentYear + '/month/0/" ' +
                                 'title="' + row.main_name + '">' +
                                 '<span class="fas fa-info"></span>' +
                                 '</button>';
                         }
                     },
                 ],
                 order: [
@@ -437,15 +437,15 @@
                     $('#foot-year .col-total-amount').html('' + formatAndColor(totalAmountAllChars_year) + '');
                     $('#foot-year .col-total-ess').html('' + formatAndColor(totalEssAmountAllChars_year) + '');
                     $('#foot-year .col-total-mining').html('' + formatAndColor(totalMiningAmountAllChars_year) + '');
                     $('#foot-year .col-total-others').html('' + formatAndColor(totalOthersAmountAllChars_year) + '');
                     $('#foot-year .col-total-gesamt').html('' + formatAndColor(totalCombinedAmountAllChars_year) + '');
                     $('#foot-year .col-total-button').html('<button class="btn btn-sm btn-info btn-square" data-bs-toggle="modal" data-bs-target="#modalViewCharacterContainer"' +
                         'aria-label="{{ data.main_name }}"' +
-                        'data-ajax_url="/ledger/api/account/0/ledger/template/year/' + currentYear + '/month/0" ' +
+                        'data-ajax_url="/ledger/api/account/0/ledger/template/year/' + currentYear + '/month/0/" ' +
                         'title="{{ data.main_name }}"> <span class="fas fa-info"></span></button>');
                 },
             });
             yearTableInitialized = true;
         }
     });
 });
```

### Comparing `aa_ledger-0.3.4/ledger/static/ledger/js/corpledger.js` & `aa_ledger-0.3.5/ledger/static/ledger/js/corpledger.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -14,15 +14,15 @@
 
     $('#monthDropdown').change(function() {
         selectedMonth = $(this).val(); // Ausgewählter Monat auslesen
         var selectedYear = currentYear; // Hier die Logik zum Auslesen des ausgewählten Jahres implementieren, falls nötig
         var monthText = getMonthName(selectedMonth);
 
         // URL für die Daten der ausgewählten Kombination von Jahr und Monat erstellen
-        var url = '/ledger/api/corporation/0/ledger/year/' + selectedYear + '/month/' + selectedMonth;
+        var url = '/ledger/api/corporation/0/ledger/year/' + selectedYear + '/month/' + selectedMonth + '/';
 
         // DataTable neu laden mit den Daten des ausgewählten Monats
         MonthTable.ajax.url(url).load();
         $('#currentMonthLink').text('Month - ' + monthText);
     });
 
     function getMonthName(monthNumber) {
@@ -54,15 +54,15 @@
         // Rückgabe des formatierten Strings mit Farbe und Einheit
         return '<span style="color: ' + color + ';">' + formattedValue + '</span> ISK';
     }
 
     // Initialize DataTable for current_month
     var MonthTable = $('#ratting').DataTable({
         ajax: {
-            url: '/ledger/api/corporation/0/ledger/year/' + currentYear + '/month/' + selectedMonth + '',
+            url: '/ledger/api/corporation/0/ledger/year/' + currentYear + '/month/' + selectedMonth + '/',
             dataSrc: function(data) {
                 // Zusätzliche Daten im DataTable-Objekt speichern
                 total_amount = data.items[0].total.total_amount;
                 total_amount_ess = data.items[0].total.total_amount_ess;
                 total_amount_combined = data.items[0].total.total_amount_all;
 
                 // Billboard
@@ -179,15 +179,15 @@
             {
                 data: 'col-total-action',
                 render: function(data, type, row) {
                     return '<button class="btn btn-sm btn-info btn-square" ' +
                         'data-bs-toggle="modal" ' +
                         'data-bs-target="#modalViewCharacterContainer" ' +
                         'aria-label="' + row.main_name + '" ' +
-                        'data-ajax_url="/ledger/api/corporation/' + row.main_id + '/ledger/template/year/' + currentYear + '/month/' + selectedMonth + '" ' +
+                        'data-ajax_url="/ledger/api/corporation/' + row.main_id + '/ledger/template/year/' + currentYear + '/month/' + selectedMonth + '/" ' +
                         'title="' + row.main_name + '">' +
                         '<span class="fas fa-info"></span>' +
                         '</button>';
                 }
             },
         ],
         order: [
@@ -202,15 +202,15 @@
             var totalEssAmountAllChars = parseFloat(total_amount_ess);
             var totalCombinedAmountAllChars = parseFloat(total_amount_combined);
             $('#foot .col-total-amount').html('' + formatAndColor(totalAmountAllChars) + '');
             $('#foot .col-total-ess').html('' + formatAndColor(totalEssAmountAllChars) + '');
             $('#foot .col-total-gesamt').html('' + formatAndColor(totalCombinedAmountAllChars) + '');
             $('#foot .col-total-button').html('<button class="btn btn-sm btn-info btn-square" data-bs-toggle="modal" data-bs-target="#modalViewCharacterContainer"' +
                 'aria-label="{{ data.main_name }}"' +
-                'data-ajax_url="/ledger/api/corporation/0/ledger/template/year/' + currentYear + '/month/' + selectedMonth + '" ' +
+                'data-ajax_url="/ledger/api/corporation/0/ledger/template/year/' + currentYear + '/month/' + selectedMonth + '/" ' +
                 'title="{{ data.main_name }}"> <span class="fas fa-info"></span></button>');
         },
     });
 
     $('a[data-bs-toggle="tab"]').on('shown.bs.tab', function(e) {
         // Get the id of the tab that was clicked
         var targetTabId = $(e.target).attr('href');
@@ -218,15 +218,15 @@
         // Check if the clicked tab is the one containing the year DataTable
         if (targetTabId === '#tab-all_month' && !yearTableInitialized) {
 
             // Initialisiere DataTable für den Hauptinhalt
             // eslint-disable-next-line no-undef
             YearTable = $('#ratting_year').DataTable({
                 ajax: {
-                    url: '/ledger/api/corporation/0/ledger/year/' + currentYear + '/month/0',
+                    url: '/ledger/api/corporation/0/ledger/year/' + currentYear + '/month/0/',
                     dataSrc: function(data) {
                         // Zusätzliche Daten im DataTable-Objekt speichern
                         total_amount = data.items[0].total.total_amount;
                         total_amount_ess = data.items[0].total.total_amount_ess;
                         total_amount_combined = data.items[0].total.total_amount_all;
 
                         // Billboard
@@ -345,15 +345,15 @@
                     {
                         data: 'col-total-action',
                         render: function(data, type, row) {
                             return '<button class="btn btn-sm btn-info btn-square" ' +
                                 'data-bs-toggle="modal" ' +
                                 'data-bs-target="#modalViewCharacterContainer" ' +
                                 'aria-label="' + row.main_name + '" ' +
-                                'data-ajax_url="/voicesofwar/api/corporation/' + row.main_id + '/ledger/template/year/' + currentYear + '/month/' + selectedMonth + '" ' +
+                                'data-ajax_url="/ledger/api/corporation/' + row.main_id + '/ledger/template/year/' + currentYear + '/month/0/" ' +
                                 'title="' + row.main_name + '">' +
                                 '<span class="fas fa-info"></span>' +
                                 '</button>';
                         }
                     },
                 ],
                 order: [
@@ -368,15 +368,15 @@
                     var totalEssAmountAllChars = parseFloat(total_amount_ess);
                     var totalCombinedAmountAllChars = parseFloat(total_amount_combined);
                     $('#foot-year .col-total-amount').html('' + formatAndColor(totalAmountAllChars) + '');
                     $('#foot-year .col-total-ess').html('' + formatAndColor(totalEssAmountAllChars) + '');
                     $('#foot-year .col-total-gesamt').html('' + formatAndColor(totalCombinedAmountAllChars) + '');
                     $('#foot-year .col-total-button').html('<button class="btn btn-sm btn-info btn-square" data-bs-toggle="modal" data-bs-target="#modalViewCharacterContainer"' +
                         'aria-label="{{ data.main_name }}"' +
-                        'data-ajax_url="/voicesofwar/api/corporation/0/ledger/template/year/' + currentYear + '/month/' + selectedMonth + '" ' +
+                        'data-ajax_url="/ledger/api/corporation/0/ledger/template/year/' + currentYear + '/month/0/" ' +
                         'title="{{ data.main_name }}"> <span class="fas fa-info"></span></button>');
                 },
             });
 
             yearTableInitialized = true;
         }
     });
```

### Comparing `aa_ledger-0.3.4/ledger/static/ledger/js/img.js` & `aa_ledger-0.3.5/ledger/static/ledger/js/img.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/task_helpers/core_helpers.py` & `aa_ledger-0.3.5/ledger/task_helpers/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/task_helpers/corp_helpers.py` & `aa_ledger-0.3.5/ledger/task_helpers/corp_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/task_helpers/etag_helpers.py` & `aa_ledger-0.3.5/ledger/task_helpers/etag_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/base.html` & `aa_ledger-0.3.5/ledger/templates/ledger/base.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/error.html` & `aa_ledger-0.3.5/ledger/templates/ledger/error.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/ledger/base.html` & `aa_ledger-0.3.5/ledger/templates/ledger/ledger/base.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/ledger/index.html` & `aa_ledger-0.3.5/ledger/templates/ledger/ledger/index.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/ledger/menu.html` & `aa_ledger-0.3.5/ledger/templates/ledger/ledger/menu.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/char_ledger.html` & `aa_ledger-0.3.5/ledger/templates/ledger/ledger/charledger/char_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/month.html` & `aa_ledger-0.3.5/ledger/templates/ledger/ledger/charledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/year.html` & `aa_ledger-0.3.5/ledger/templates/ledger/ledger/charledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/corp_ledger.html` & `aa_ledger-0.3.5/ledger/templates/ledger/ledger/corpledger/corp_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/month.html` & `aa_ledger-0.3.5/ledger/templates/ledger/ledger/corpledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/year.html` & `aa_ledger-0.3.5/ledger/templates/ledger/ledger/corpledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/modals/modal-full.html` & `aa_ledger-0.3.5/ledger/templates/ledger/modals/modal-full.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/modals/modal-xl.html` & `aa_ledger-0.3.5/ledger/templates/ledger/modals/modal-xl.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/modals/modal.html` & `aa_ledger-0.3.5/ledger/templates/ledger/modals/modal.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/modals/modal_dialog.html` & `aa_ledger-0.3.5/ledger/templates/ledger/modals/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/templates/ledger/modals/pve/view_character_content.html` & `aa_ledger-0.3.5/ledger/templates/ledger/modals/pve/view_character_content.html`

 * *Files 4% similar despite different names*

```diff
@@ -25,253 +25,260 @@
                 </li>
             </ul>
             <div class="border border-secondary rounded-bottom tab-content px-2">
                 <div class="tab-pane panel panel-default active" id="tab-summary">
                     <div class="card-body modal-tab">
                         <div class="row description-row">
                             <div class="col-sm-6">Ratting:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.summary_isk|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount|format_currency }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">ESS:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.summary_ess|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount|format_currency }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Stolen ESS:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.stolen|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: red">{{ character.stolen.total_amount|format_currency }}</span> ISK</div>
                         </div>
                         {% if character.mining %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Mining:</div>
                             <div class='col-sm-6'><span style="color: green">{{ character.mining|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
-                        {% if character.trading %}
+                        {% if character.transaction %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Trading:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.trading|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.transaction.total_amount|format_currency }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Trading Cost:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.trading_cost|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: red">{{ character.market_cost.total_amount|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                         {% if character.contract %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Contracts:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.contract|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.contract.total_amount|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                         {% if character.donation %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Donations:<br>
                             <span style="color: #FFBF00"><!--<i class="fas fa-exclamation-triangle"></i> Excluded from summary <i class="fas fa-exclamation-triangle"></i>--></span>
                             </div>
                             <div class='col-sm-6'>
                                 <span style="color: green">
-                                    {{ character.donation|format_currency }}
+                                    {{ character.donation.total_amount|format_currency }}
                                 </span> ISK
                                     <br><span style="color: #3483eb"><!--<i class="fas fa-info-circle"></i> Exluded registered chars <i class="fas fa-info-circle"></i>--></span>
                             </div>
                         </div>
                         {% endif %}
                         {% if character.production_cost %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Production Cost:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.production_cost|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: red">{{ character.production_cost.total_amount|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Summary:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.summary|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount|format_currency }}</span> ISK</div>
                         </div>
                     </div>
                 </div>
                 <!--##############################DAILY#######################-->
                 <div class="tab-pane panel panel-default" id="tab-daily">
                     <div class="card-body modal-tab">
-                        {% if character.day_isk %}
+                        {% if character.bounty.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Ratting:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.day_isk|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Ratting per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.day_avg_isk|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_day|format_currency }}</span> ISK</div>
                         </div>
                         <hr>
 
-                        {% if character.day_ess %}
+                        {% if character.ess.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - ESS:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.day_ess|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount_day|format_currency }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Stolen ESS:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.day_stolen_ess|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. ESS per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.day_avg_ess|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.ess.average_day|format_currency }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Stolen per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.day_stolen|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|format_currency }}</span> ISK</div>
                         </div>
                         {% if character.mining %}
                         <hr>
-                        {% if character.mining_day %}
+                        {% if character.mining.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Mining:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.mining_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.mining.total_amount_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Mining per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.day_avg_mining|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.mining.average_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
 
-                        {% if character.trading %}
+                        {% if character.transaction %}
                         <hr>
-                        {% if character.trading_day %}
+                        {% if character.transaction.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Trading:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.trading_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.total_amount_day|format_currency }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Trading Cost:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.trading_cost_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.total_amount_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Trading per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.day_avg_trading|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_day|format_currency }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Trading Cost per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.day_avg_trading_cost|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.contract %}
                         <hr>
-                        {% if character.contract_day %}
+                        {% if character.contract.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Contracts:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.contract_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.contract.total_amount_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Contracts per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.day_avg_contract|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.donation %}
                         <hr>
-                        {% if character.donation_day %}
+                        {% if character.donation.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Donations:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.donation_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.donation.total_amount_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Donations per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.day_avg_donation|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.production_cost %}
                         <hr>
-                        {% if character.production_cost_day %}
+                        {% if character.production_cost.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Production Cost:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.total_amount_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Production Cost per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.day_avg_production_cost|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                         {% if character.date %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Summary Day</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.summary_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_day|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                     </div>
                 </div>
                 <!--############################## HOURLY #######################-->
                 <div class="tab-pane panel panel-default" id="tab-hourly">
                     <div class="card-body modal-tab">
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Ratting per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.hourly_avg_isk|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|format_currency }}</span> ISK</div>
                         </div>
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. ESS per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.hourly_avg_ess|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|format_currency }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Stolen per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.hourly_stolen|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_hour|format_currency }}</span> ISK</div>
                         </div>
 
                         {% if character.mining %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Mining per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.hourly_avg_mining|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.mining.average_hour|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
 
-                        {% if character.trading %}
+                        {% if character.transaction %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Trading per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.hourly_avg_trading|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_hour|format_currency }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Trading Cost per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.hourly_avg_trading_cost|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_hour|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.contract %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Contracts per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.hourly_avg_contract|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_hour|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.donation %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Donations per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.hourly_avg_donation|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_hour|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.production_cost %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Production Cost per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.hourly_avg_production_cost|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_hour|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        {% if character.date %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Summary Hour</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_hour|format_currency }}</span> ISK</div>
                         </div>
                         {% endif %}
                     </div>
                 </div>
             </div>
         </div>
         {% else %}
```

### Comparing `aa_ledger-0.3.4/ledger/view_helpers/core.py` & `aa_ledger-0.3.5/ledger/view_helpers/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 Core View Helper
 """
 
 from datetime import datetime
 from decimal import Decimal
 
 from django.core.cache import cache
-from django.db.models import DecimalField, F, Q, Sum
-from django.db.models.functions import Coalesce
+from django.db.models import Q
 
 from ledger.app_settings import STORAGE_BASE_KEY
 from ledger.decorators import custom_cache_timeout
 from ledger.hooks import get_extension_logger
 from ledger.models import Events
 
 logger = get_extension_logger(__name__)
@@ -72,53 +71,14 @@
         total_ess_stolen = int(ess_amount * (result / 100))
 
         total_ess_gain = format(result, ".2f")
 
     return total_ess_stolen, total_ess_gain
 
 
-def calculate_journal(entries, filter_data, exclude=False):
-    """
-    Berechnet den Gesamtbetrag (Summe) für Einträge in einem Journal.
-
-    :param entries: Eine Tabelle von Datenbankeinträgen (corporation journal oder character journal).
-    :type entries: QuerySet
-    :param filter_data: Ein Filter, der auf die Einträge angewendet wird.
-    :type filter_data: Q Filter
-    :return: Der Gesamtbetrag (Summe) der Einträge.
-    :rtype: float
-    """
-
-    current_date = datetime.now()
-
-    total_amount_entries = entries.filter(filter_data)
-
-    if exclude:
-        total_amount_entries = total_amount_entries.exclude(first_party__id__in=exclude)
-
-    total_amount_aggregated = total_amount_entries.aggregate(
-        total_amount=Coalesce(Sum(F("amount")), 0, output_field=DecimalField()),
-        total_amount_day=Coalesce(
-            Sum(F("amount"), filter=Q(date__day=current_date.day)),
-            0,
-            output_field=DecimalField(),
-        ),
-        total_amount_hour=Coalesce(
-            Sum(
-                F("amount"),
-                filter=Q(date__day=current_date.day, date__hour=current_date.hour),
-            ),
-            0,
-            output_field=DecimalField(),
-        ),
-    )
-
-    return total_amount_aggregated
-
-
 def _storage_key(identifier: str) -> str:
     return STORAGE_BASE_KEY + str(identifier)
 
 
 def get_cache_stale(key_name):
     data = cache.get(key=_storage_key(key_name))
     if not data:
```

### Comparing `aa_ledger-0.3.4/ledger/views/pve.py` & `aa_ledger-0.3.5/ledger/views/pve.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/views/character/char_audit.py` & `aa_ledger-0.3.5/ledger/views/character/char_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/views/corporation/corp_audit.py` & `aa_ledger-0.3.5/ledger/views/corporation/corp_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/views/corporation/corp_events.py` & `aa_ledger-0.3.5/ledger/views/corporation/corp_events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/ledger/views/corporation/corp_tax.py` & `aa_ledger-0.3.5/ledger/views/corporation/corp_tax.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/LICENSE` & `aa_ledger-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/README.md` & `aa_ledger-0.3.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 ## Upcoming<a name="upcoming"></a>
 
 - Corp Tax System (Tracks specific amount that transfer'd to specific division)
 - Events Calender
 
 ## Installation<a name="installation"></a>
 
+> \[!NOTE\]
+> AA Ledger needs at least Alliance Auth v4.0.0
+> Please make sure to update your Alliance Auth before you install this APP
+
 ### Step 1 - Install the Package<a name="step1"></a>
 
 Make sure you're in your virtual environment (venv) of your Alliance Auth then install the pakage.
 
 ```shell
 pip install aa-ledger
 ```
@@ -80,36 +84,40 @@
 | `char_audit_admin_access` | Can Manage Character Audit Module      | Can Manage Character Audit Module, Like Add Memeberaudit Chars, View Character Journals |
 | `corp_audit_admin_access` | Can Manage Corporation Audit Module    | Can Manage Corporation Audit Module, Like Add Corp, View Corporation Journals           |
 
 ### Step 6 - (Optional) Setting up Compatibilies<a name="step6"></a>
 
 The Following Settings can be setting up in the `local.py`
 
-- LEDGER_LOGGER_USE:        `True / False`
-- LEDGER_MEMBERAUDIT_USE:   `True / False`
-- LEDGER_CORPSTATS_TWO:     `True / False`
+- LEDGER_APP_NAME:          `"YOURNAME"`   - Set the name of the APP
+
+- LEDGER_LOGGER_USE:        `True / False` - Set to use own Logger File
+
+- LEDGER_MEMBERAUDIT_USE:   `True / False` - Set to use the Memberaudit Journal to Fetch Statistics
+
+- LEDGER_CORPSTATS_TWO:     `True / False` - Set to use Corp Stats Two APP to Fetch Members that are not registred
 
 If you set up LEDGER_LOGGER_USE to `True` you need to add the following code below:
 
 ```python
 LOGGING_LEDGER = {
     "handlers": {
         "ledger_file": {
-            "level": "DEBUG",
+            "level": "INFO",
             "class": "logging.handlers.RotatingFileHandler",
             "filename": os.path.join(BASE_DIR, "log/ledger.log"),
             "formatter": "verbose",
             "maxBytes": 1024 * 1024 * 5,
             "backupCount": 5,
         },
     },
     "loggers": {
         "ledger": {
             "handlers": ["ledger_file", "console"],
-            "level": "DEBUG",
+            "level": "INFO",
         },
     },
 }
 LOGGING["handlers"].update(LOGGING_LEDGER["handlers"])
 LOGGING["loggers"].update(LOGGING_LEDGER["loggers"])
 ```
```

### Comparing `aa_ledger-0.3.4/pyproject.toml` & `aa_ledger-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.4/PKG-INFO` & `aa_ledger-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-ledger
-Version: 0.3.4
+Version: 0.3.5
 Dynamic: Summary
 Project-URL: Changelog, https://github.com/Geuthur/aa-ledger/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/Geuthur/aa-ledger
 Project-URL: Source, https://github.com/Geuthur/aa-ledger
 Project-URL: Tracker, https://github.com/Geuthur/aa-ledger/issues
 Author-email: Geuthur <devgeuthur@gmail.com>
 License: MIT License
@@ -83,14 +83,18 @@
 ## Upcoming<a name="upcoming"></a>
 
 - Corp Tax System (Tracks specific amount that transfer'd to specific division)
 - Events Calender
 
 ## Installation<a name="installation"></a>
 
+> \[!NOTE\]
+> AA Ledger needs at least Alliance Auth v4.0.0
+> Please make sure to update your Alliance Auth before you install this APP
+
 ### Step 1 - Install the Package<a name="step1"></a>
 
 Make sure you're in your virtual environment (venv) of your Alliance Auth then install the pakage.
 
 ```shell
 pip install aa-ledger
 ```
@@ -137,36 +141,40 @@
 | `char_audit_admin_access` | Can Manage Character Audit Module      | Can Manage Character Audit Module, Like Add Memeberaudit Chars, View Character Journals |
 | `corp_audit_admin_access` | Can Manage Corporation Audit Module    | Can Manage Corporation Audit Module, Like Add Corp, View Corporation Journals           |
 
 ### Step 6 - (Optional) Setting up Compatibilies<a name="step6"></a>
 
 The Following Settings can be setting up in the `local.py`
 
-- LEDGER_LOGGER_USE:        `True / False`
-- LEDGER_MEMBERAUDIT_USE:   `True / False`
-- LEDGER_CORPSTATS_TWO:     `True / False`
+- LEDGER_APP_NAME:          `"YOURNAME"`   - Set the name of the APP
+
+- LEDGER_LOGGER_USE:        `True / False` - Set to use own Logger File
+
+- LEDGER_MEMBERAUDIT_USE:   `True / False` - Set to use the Memberaudit Journal to Fetch Statistics
+
+- LEDGER_CORPSTATS_TWO:     `True / False` - Set to use Corp Stats Two APP to Fetch Members that are not registred
 
 If you set up LEDGER_LOGGER_USE to `True` you need to add the following code below:
 
 ```python
 LOGGING_LEDGER = {
     "handlers": {
         "ledger_file": {
-            "level": "DEBUG",
+            "level": "INFO",
             "class": "logging.handlers.RotatingFileHandler",
             "filename": os.path.join(BASE_DIR, "log/ledger.log"),
             "formatter": "verbose",
             "maxBytes": 1024 * 1024 * 5,
             "backupCount": 5,
         },
     },
     "loggers": {
         "ledger": {
             "handlers": ["ledger_file", "console"],
-            "level": "DEBUG",
+            "level": "INFO",
         },
     },
 }
 LOGGING["handlers"].update(LOGGING_LEDGER["handlers"])
 LOGGING["loggers"].update(LOGGING_LEDGER["loggers"])
 ```
```

