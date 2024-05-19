# Comparing `tmp/discord-disnake-2.3.0.2.tar.gz` & `tmp/discord_disnake-2.3.0.2.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\ezsh1\Documents\GitHub\discord-disnake\dist\tmp5lmcz53j\discord-disnake-2.3.0.2.tar", last modified: Sun Jan  2 22:27:25 2022, max compression
+gzip compressed data, was "C:\Users\ezsh1\Documents\GitHub\discord-disnake\dist\.tmp-1npccqdf\discord_disnake-2.3.0.2.post0.tar", last modified: Sun May 19 14:55:36 2024, max compression
```

## Comparing `discord-disnake-2.3.0.2.tar` & `discord_disnake-2.3.0.2.post0.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxrwxrwx   0        0        0        0 2022-01-02 22:27:25.188243 discord-disnake-2.3.0.2/
--rw-rw-rw-   0        0        0     1646 2022-01-02 22:27:25.188243 discord-disnake-2.3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      562 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-01-02 22:27:24.948967 discord-disnake-2.3.0.2/discord/
--rw-rw-rw-   0        0        0     1875 2022-01-02 22:25:16.000000 discord-disnake-2.3.0.2/discord/__init__.py
--rw-rw-rw-   0        0        0    10524 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/__main__.py
--rw-rw-rw-   0        0        0      732 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/abc.py
--rw-rw-rw-   0        0        0      445 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/activity.py
--rw-rw-rw-   0        0        0     1120 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/app_commands.py
--rw-rw-rw-   0        0        0      225 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/appinfo.py
--rw-rw-rw-   0        0        0      304 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/asset.py
--rw-rw-rw-   0        0        0      965 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/audit_logs.py
--rw-rw-rw-   0        0        0      185 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/backoff.py
--rw-rw-rw-   0        0        0     1067 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/channel.py
--rw-rw-rw-   0        0        0     1525 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/client.py
--rw-rw-rw-   0        0        0      175 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/colour.py
--rw-rw-rw-   0        0        0      449 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/components.py
--rw-rw-rw-   0        0        0      199 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/context_managers.py
--rw-rw-rw-   0        0        0      249 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/custom_warnings.py
--rw-rw-rw-   0        0        0      234 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/embeds.py
--rw-rw-rw-   0        0        0      252 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/emoji.py
--rw-rw-rw-   0        0        0     1949 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/enums.py
--rw-rw-rw-   0        0        0      977 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/errors.py
-drwxrwxrwx   0        0        0        0 2022-01-02 22:27:24.754722 discord-disnake-2.3.0.2/discord/ext/
-drwxrwxrwx   0        0        0        0 2022-01-02 22:27:25.004967 discord-disnake-2.3.0.2/discord/ext/commands/
--rw-rw-rw-   0        0        0      515 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/__init__.py
--rw-rw-rw-   0        0        0      166 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/_types.py
--rw-rw-rw-   0        0        0     1971 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/base_core.py
--rw-rw-rw-   0        0        0      548 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/bot.py
--rw-rw-rw-   0        0        0      502 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/bot_base.py
--rw-rw-rw-   0        0        0      406 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/cog.py
--rw-rw-rw-   0        0        0      279 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/common_bot_base.py
--rw-rw-rw-   0        0        0      251 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/context.py
--rw-rw-rw-   0        0        0     3036 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/converter.py
--rw-rw-rw-   0        0        0      462 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0     2915 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/core.py
--rw-rw-rw-   0        0        0     1829 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/ctx_menus_core.py
--rw-rw-rw-   0        0        0     3016 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/errors.py
--rw-rw-rw-   0        0        0      586 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/flags.py
--rw-rw-rw-   0        0        0      410 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/help.py
--rw-rw-rw-   0        0        0      789 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/interaction_bot_base.py
--rw-rw-rw-   0        0        0      938 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/params.py
--rw-rw-rw-   0        0        0     1929 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/slash_core.py
--rw-rw-rw-   0        0        0      295 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2022-01-02 22:27:25.004967 discord-disnake-2.3.0.2/discord/ext/tasks/
--rw-rw-rw-   0        0        0    27045 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0      148 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/file.py
--rw-rw-rw-   0        0        0      521 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/flags.py
--rw-rw-rw-   0        0        0      614 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/gateway.py
--rw-rw-rw-   0        0        0     1314 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/guild.py
--rw-rw-rw-   0        0        0      529 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/guild_scheduled_event.py
--rw-rw-rw-   0        0        0      412 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/http.py
--rw-rw-rw-   0        0        0      555 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/integrations.py
-drwxrwxrwx   0        0        0        0 2022-01-02 22:27:25.020984 discord-disnake-2.3.0.2/discord/interactions/
--rw-rw-rw-   0        0        0       81 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/interactions/__init__.py
--rw-rw-rw-   0        0        0     1255 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/interactions/application_command.py
--rw-rw-rw-   0        0        0      801 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/interactions/base.py
--rw-rw-rw-   0        0        0      413 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/interactions/message.py
--rw-rw-rw-   0        0        0      471 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/invite.py
--rw-rw-rw-   0        0        0      662 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/iterators.py
--rw-rw-rw-   0        0        0      397 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/member.py
--rw-rw-rw-   0        0        0      201 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/mentions.py
--rw-rw-rw-   0        0        0      879 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/message.py
--rw-rw-rw-   0        0        0      201 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/mixins.py
--rw-rw-rw-   0        0        0      173 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/object.py
--rw-rw-rw-   0        0        0      225 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/oggparse.py
--rw-rw-rw-   0        0        0      842 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/opus.py
--rw-rw-rw-   0        0        0      250 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/partial_emoji.py
--rw-rw-rw-   0        0        0      413 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/permissions.py
--rw-rw-rw-   0        0        0      542 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/player.py
--rw-rw-rw-   0        0        0      743 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/raw_models.py
--rw-rw-rw-   0        0        0      182 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/reaction.py
--rw-rw-rw-   0        0        0      379 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/role.py
--rw-rw-rw-   0        0        0      589 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/shard.py
--rw-rw-rw-   0        0        0      314 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/stage_instance.py
--rw-rw-rw-   0        0        0     1408 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/state.py
--rw-rw-rw-   0        0        0      555 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/sticker.py
--rw-rw-rw-   0        0        0      228 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/team.py
--rw-rw-rw-   0        0        0      332 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/template.py
--rw-rw-rw-   0        0        0      417 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/threads.py
-drwxrwxrwx   0        0        0        0 2022-01-02 22:27:25.109010 discord-disnake-2.3.0.2/discord/types/
--rw-rw-rw-   0        0        0      159 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/__init__.py
--rw-rw-rw-   0        0        0      458 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/activity.py
--rw-rw-rw-   0        0        0      240 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/appinfo.py
--rw-rw-rw-   0        0        0      861 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/audit_log.py
--rw-rw-rw-   0        0        0      616 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/channel.py
--rw-rw-rw-   0        0        0      328 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/components.py
--rw-rw-rw-   0        0        0      332 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/embed.py
--rw-rw-rw-   0        0        0      171 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/emoji.py
--rw-rw-rw-   0        0        0      177 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/gateway.py
--rw-rw-rw-   0        0        0      526 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/guild.py
--rw-rw-rw-   0        0        0      346 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/integration.py
--rw-rw-rw-   0        0        0     1412 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/interactions.py
--rw-rw-rw-   0        0        0      440 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/invite.py
--rw-rw-rw-   0        0        0      241 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/member.py
--rw-rw-rw-   0        0        0      504 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/message.py
--rw-rw-rw-   0        0        0      589 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/raw_models.py
--rw-rw-rw-   0        0        0      162 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/role.py
--rw-rw-rw-   0        0        0      143 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/snowflake.py
--rw-rw-rw-   0        0        0      389 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/sticker.py
--rw-rw-rw-   0        0        0      162 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/team.py
--rw-rw-rw-   0        0        0      178 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/template.py
--rw-rw-rw-   0        0        0      278 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/threads.py
--rw-rw-rw-   0        0        0      150 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/user.py
--rw-rw-rw-   0        0        0      329 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/voice.py
--rw-rw-rw-   0        0        0      323 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/webhook.py
--rw-rw-rw-   0        0        0      188 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/welcome_screen.py
--rw-rw-rw-   0        0        0      231 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/types/widget.py
-drwxrwxrwx   0        0        0        0 2022-01-02 22:27:25.125012 discord-disnake-2.3.0.2/discord/ui/
--rw-rw-rw-   0        0        0      253 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ui/__init__.py
--rw-rw-rw-   0        0        0      337 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ui/button.py
--rw-rw-rw-   0        0        0      201 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ui/item.py
--rw-rw-rw-   0        0        0      368 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ui/select.py
--rw-rw-rw-   0        0        0      395 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/ui/view.py
--rw-rw-rw-   0        0        0      358 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/user.py
--rw-rw-rw-   0        0        0     1760 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/utils.py
--rw-rw-rw-   0        0        0      510 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/voice_client.py
-drwxrwxrwx   0        0        0        0 2022-01-02 22:27:25.133002 discord-disnake-2.3.0.2/discord/webhook/
--rw-rw-rw-   0        0        0      195 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/webhook/__init__.py
--rw-rw-rw-   0        0        0      816 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/webhook/async_.py
--rw-rw-rw-   0        0        0      584 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/webhook/sync.py
--rw-rw-rw-   0        0        0      415 2022-01-02 19:55:51.000000 discord-disnake-2.3.0.2/discord/widget.py
-drwxrwxrwx   0        0        0        0 2022-01-02 22:27:25.180221 discord-disnake-2.3.0.2/discord_disnake.egg-info/
--rw-rw-rw-   0        0        0     1646 2022-01-02 22:27:24.000000 discord-disnake-2.3.0.2/discord_disnake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2891 2022-01-02 22:27:24.000000 discord-disnake-2.3.0.2/discord_disnake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-02 22:27:24.000000 discord-disnake-2.3.0.2/discord_disnake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-01-02 22:27:24.000000 discord-disnake-2.3.0.2/discord_disnake.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-01-02 22:27:24.000000 discord-disnake-2.3.0.2/discord_disnake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-02 22:27:25.188243 discord-disnake-2.3.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1946 2022-01-02 22:24:46.000000 discord-disnake-2.3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 14:55:36.911410 discord_disnake-2.3.0.2.post0/
+-rw-rw-rw-   0        0        0     1916 2024-05-19 14:55:36.908409 discord_disnake-2.3.0.2.post0/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2024-05-19 14:54:41.000000 discord_disnake-2.3.0.2.post0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 14:55:36.691396 discord_disnake-2.3.0.2.post0/discord/
+-rw-rw-rw-   0        0        0     2193 2024-05-19 14:54:41.000000 discord_disnake-2.3.0.2.post0/discord/__init__.py
+-rw-rw-rw-   0        0        0    10524 2022-01-02 19:55:51.000000 discord_disnake-2.3.0.2.post0/discord/__main__.py
+-rw-rw-rw-   0        0        0     1897 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/abc.py
+-rw-rw-rw-   0        0        0     1605 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/activity.py
+-rw-rw-rw-   0        0        0     1117 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/app_commands.py
+-rw-rw-rw-   0        0        0     1417 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/appinfo.py
+-rw-rw-rw-   0        0        0     1467 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/asset.py
+-rw-rw-rw-   0        0        0     2123 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/audit_logs.py
+-rw-rw-rw-   0        0        0     1341 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/backoff.py
+-rw-rw-rw-   0        0        0     2228 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/channel.py
+-rw-rw-rw-   0        0        0     2687 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/client.py
+-rw-rw-rw-   0        0        0     1332 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/colour.py
+-rw-rw-rw-   0        0        0     1607 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/components.py
+-rw-rw-rw-   0        0        0     1346 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/context_managers.py
+-rw-rw-rw-   0        0        0      264 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/custom_warnings.py
+-rw-rw-rw-   0        0        0     1437 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/embeds.py
+-rw-rw-rw-   0        0        0     1456 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/emoji.py
+-rw-rw-rw-   0        0        0     3112 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/enums.py
+-rw-rw-rw-   0        0        0     2139 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-19 14:55:36.515575 discord_disnake-2.3.0.2.post0/discord/ext/
+drwxrwxrwx   0        0        0        0 2024-05-19 14:55:36.743401 discord_disnake-2.3.0.2.post0/discord/ext/commands/
+-rw-rw-rw-   0        0        0      515 2022-01-02 19:55:51.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     1310 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/_types.py
+-rw-rw-rw-   0        0        0     1958 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/base_core.py
+-rw-rw-rw-   0        0        0     1700 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/bot.py
+-rw-rw-rw-   0        0        0     1649 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/bot_base.py
+-rw-rw-rw-   0        0        0     1558 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/cog.py
+-rw-rw-rw-   0        0        0     1455 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/common_bot_base.py
+-rw-rw-rw-   0        0        0     1445 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/context.py
+-rw-rw-rw-   0        0        0     4182 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/converter.py
+-rw-rw-rw-   0        0        0     1608 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0     4066 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/core.py
+-rw-rw-rw-   0        0        0     1811 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/ctx_menus_core.py
+-rw-rw-rw-   0        0        0     4165 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/errors.py
+-rw-rw-rw-   0        0        0     1736 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/flags.py
+-rw-rw-rw-   0        0        0     1561 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/help.py
+-rw-rw-rw-   0        0        0      765 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/interaction_bot_base.py
+-rw-rw-rw-   0        0        0      992 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/params.py
+-rw-rw-rw-   0        0        0     1915 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/slash_core.py
+-rw-rw-rw-   0        0        0     1446 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2024-05-19 14:55:36.745399 discord_disnake-2.3.0.2.post0/discord/ext/tasks/
+-rw-rw-rw-   0        0        0    27045 2022-01-02 19:55:51.000000 discord_disnake-2.3.0.2.post0/discord/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/file.py
+-rw-rw-rw-   0        0        0     1684 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/flags.py
+-rw-rw-rw-   0        0        0     1775 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/gateway.py
+-rw-rw-rw-   0        0        0     2477 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/guild.py
+-rw-rw-rw-   0        0        0     1644 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/guild_scheduled_event.py
+-rw-rw-rw-   0        0        0     1576 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/http.py
+-rw-rw-rw-   0        0        0     1711 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/integrations.py
+drwxrwxrwx   0        0        0        0 2024-05-19 14:55:36.755399 discord_disnake-2.3.0.2.post0/discord/interactions/
+-rw-rw-rw-   0        0        0       81 2022-01-02 19:55:51.000000 discord_disnake-2.3.0.2.post0/discord/interactions/__init__.py
+-rw-rw-rw-   0        0        0     1232 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/interactions/application_command.py
+-rw-rw-rw-   0        0        0     1952 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/interactions/base.py
+-rw-rw-rw-   0        0        0      402 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/interactions/message.py
+-rw-rw-rw-   0        0        0     1633 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/invite.py
+-rw-rw-rw-   0        0        0     1821 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/iterators.py
+-rw-rw-rw-   0        0        0     1559 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/member.py
+-rw-rw-rw-   0        0        0     1356 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/mentions.py
+-rw-rw-rw-   0        0        0     2040 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/message.py
+-rw-rw-rw-   0        0        0     1358 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/mixins.py
+-rw-rw-rw-   0        0        0     1330 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/object.py
+-rw-rw-rw-   0        0        0     1411 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/oggparse.py
+-rw-rw-rw-   0        0        0     2058 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/opus.py
+-rw-rw-rw-   0        0        0     1436 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/partial_emoji.py
+-rw-rw-rw-   0        0        0     1570 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/permissions.py
+-rw-rw-rw-   0        0        0     1704 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/player.py
+-rw-rw-rw-   0        0        0        0 2022-01-02 19:55:51.000000 discord_disnake-2.3.0.2.post0/discord/py.typed
+-rw-rw-rw-   0        0        0     1901 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/raw_models.py
+-rw-rw-rw-   0        0        0     1337 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/reaction.py
+-rw-rw-rw-   0        0        0     1543 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/role.py
+-rw-rw-rw-   0        0        0     1752 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/shard.py
+-rw-rw-rw-   0        0        0     1468 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/stage_instance.py
+-rw-rw-rw-   0        0        0     2571 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/state.py
+-rw-rw-rw-   0        0        0     1716 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/sticker.py
+-rw-rw-rw-   0        0        0     1433 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/team.py
+-rw-rw-rw-   0        0        0     1492 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/template.py
+-rw-rw-rw-   0        0        0     1578 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/threads.py
+drwxrwxrwx   0        0        0        0 2024-05-19 14:55:36.830404 discord_disnake-2.3.0.2.post0/discord/types/
+-rw-rw-rw-   0        0        0      159 2022-01-02 19:55:51.000000 discord_disnake-2.3.0.2.post0/discord/types/__init__.py
+-rw-rw-rw-   0        0        0     1612 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/activity.py
+-rw-rw-rw-   0        0        0     1426 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/appinfo.py
+-rw-rw-rw-   0        0        0     2014 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/audit_log.py
+-rw-rw-rw-   0        0        0     1771 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/channel.py
+-rw-rw-rw-   0        0        0     1480 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/components.py
+-rw-rw-rw-   0        0        0     1489 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/embed.py
+-rw-rw-rw-   0        0        0     1323 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/emoji.py
+-rw-rw-rw-   0        0        0     1353 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/gateway.py
+-rw-rw-rw-   0        0        0     1683 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/guild.py
+-rw-rw-rw-   0        0        0     1497 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/integration.py
+-rw-rw-rw-   0        0        0     2562 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/interactions.py
+-rw-rw-rw-   0        0        0     1596 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/invite.py
+-rw-rw-rw-   0        0        0     1428 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/member.py
+-rw-rw-rw-   0        0        0     1659 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/message.py
+-rw-rw-rw-   0        0        0     1741 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/raw_models.py
+-rw-rw-rw-   0        0        0     1315 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/role.py
+-rw-rw-rw-   0        0        0     1289 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/snowflake.py
+-rw-rw-rw-   0        0        0     1544 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/sticker.py
+-rw-rw-rw-   0        0        0     1315 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/team.py
+-rw-rw-rw-   0        0        0     1358 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/template.py
+-rw-rw-rw-   0        0        0     1433 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/threads.py
+-rw-rw-rw-   0        0        0     1303 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/user.py
+-rw-rw-rw-   0        0        0     1486 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/voice.py
+-rw-rw-rw-   0        0        0     1478 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/webhook.py
+-rw-rw-rw-   0        0        0     1352 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1418 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/types/widget.py
+drwxrwxrwx   0        0        0        0 2024-05-19 14:55:36.844406 discord_disnake-2.3.0.2.post0/discord/ui/
+-rw-rw-rw-   0        0        0      253 2022-01-02 19:55:51.000000 discord_disnake-2.3.0.2.post0/discord/ui/__init__.py
+-rw-rw-rw-   0        0        0     1496 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ui/button.py
+-rw-rw-rw-   0        0        0     1398 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ui/item.py
+-rw-rw-rw-   0        0        0     1527 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ui/select.py
+-rw-rw-rw-   0        0        0     1556 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/ui/view.py
+-rw-rw-rw-   0        0        0     1522 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/user.py
+-rw-rw-rw-   0        0        0     2923 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/utils.py
+-rw-rw-rw-   0        0        0     2466 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/voice_client.py
+drwxrwxrwx   0        0        0        0 2024-05-19 14:55:36.851405 discord_disnake-2.3.0.2.post0/discord/webhook/
+-rw-rw-rw-   0        0        0      195 2022-01-02 19:55:51.000000 discord_disnake-2.3.0.2.post0/discord/webhook/__init__.py
+-rw-rw-rw-   0        0        0     1970 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/webhook/async_.py
+-rw-rw-rw-   0        0        0     1740 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/webhook/sync.py
+-rw-rw-rw-   0        0        0     1577 2022-01-25 12:45:25.000000 discord_disnake-2.3.0.2.post0/discord/widget.py
+drwxrwxrwx   0        0        0        0 2024-05-19 14:55:36.905414 discord_disnake-2.3.0.2.post0/discord_disnake.egg-info/
+-rw-rw-rw-   0        0        0     1916 2024-05-19 14:55:36.000000 discord_disnake-2.3.0.2.post0/discord_disnake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2908 2024-05-19 14:55:36.000000 discord_disnake-2.3.0.2.post0/discord_disnake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 14:55:36.000000 discord_disnake-2.3.0.2.post0/discord_disnake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-19 14:55:36.000000 discord_disnake-2.3.0.2.post0/discord_disnake.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 14:55:36.000000 discord_disnake-2.3.0.2.post0/discord_disnake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 14:55:36.911410 discord_disnake-2.3.0.2.post0/setup.cfg
+-rw-rw-rw-   0        0        0     1937 2024-05-19 14:54:41.000000 discord_disnake-2.3.0.2.post0/setup.py
```

### Comparing `discord-disnake-2.3.0.2/PKG-INFO` & `discord_disnake-2.3.0.2.post0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 Metadata-Version: 2.1
 Name: discord-disnake
-Version: 2.3.0.2
+Version: 2.3.0.2.post0
 Summary: A shim for disnake (Python wrapper for the Discord API)
 Home-page: https://github.com/DisnakeDev/discord-disnake
 Author: Rapptz, EQUENOS
 License: MIT
 Project-URL: Documentation, https://docs.disnake.dev/en/latest
 Project-URL: Issue tracker, https://github.com/DisnakeDev/discord-disnake/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+Requires-Dist: disnake==2.3.0
+
+<p align="center">
+    <h3>⚠️⚠️⚠️ This package is deprecated and is no longer being maintained. ⚠️⚠️⚠️</h3>
+    Please migrate your project to use https://pypi.org/project/disnake directly.
+</p>
+
+<br/>
+<br/>
+
+---
+
+Original Readme:
 
 # This package is a shim
 
 This module allows to use [disnake](https://github.com/DisnakeDev/disnake) using `discord` namespace. This is not an independent library.
 
 # Installing
 
@@ -42,10 +54,8 @@
 py -3 -m pip install -U disnake[discord]
 ```
 
 # Links
 
 - [Documentation](https://docs.disnake.dev/en/latest)
 - [disnake GitHub](https://github.com/DisnakeDev/disnake)
-- [disnake Discord](https://discord.gg/gJDbCw8aQy)
-
-
+- [disnake Discord](https://discord.gg/disnake)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `discord-disnake-2.3.0.2/discord/__init__.py` & `discord_disnake-2.3.0.2.post0/discord/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,31 @@
 A basic wrapper for the Discord API.
 
 :copyright: (c) 2015-present Rapptz
 :license: MIT, see LICENSE for more details.
 
 """
 
+##### DEPRECATED #####
+import warnings
+warnings.warn(
+    "The discord-disnake compatibility shim is deprecated and is no longer being updated. Please migrate your project to use https://pypi.org/project/disnake directly.",
+    UserWarning,
+    stacklevel=2,
+)
+del warnings
+######################
+
+
+
 __title__ = "disnake"
 __author__ = "Rapptz, EQUENOS"
 __license__ = "MIT"
 __copyright__ = "Copyright 2015-present Rapptz, 2021-present EQUENOS"
-__version__ = "2.3.0.2"
+__version__ = "2.3.0.2.post0"
 
 __path__ = __import__("pkgutil").extend_path(__path__, __name__)
 
 import logging
 from typing import NamedTuple, Literal
 
 from .client import *
```

### Comparing `discord-disnake-2.3.0.2/discord/__main__.py` & `discord_disnake-2.3.0.2.post0/discord/__main__.py`

 * *Files identical despite different names*

### Comparing `discord-disnake-2.3.0.2/discord/app_commands.py` & `discord_disnake-2.3.0.2.post0/discord/app_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     PartialGuildAppCmdPerms,
     PartialGuildApplicationCommandPermissions,
     Role,
     SlashCommand,
     UnresolvedGuildApplicationCommandPermissions,
     User,
     UserCommand,
+    __dict__ as __original_dict__,
     _get_and_cast,
     _get_as_snowflake,
     application_command_factory,
     enum_if_int,
     try_enum,
     try_enum_to_int,
 )
@@ -36,9 +37,10 @@
     "ApplicationCommandPermissions",
     "GuildApplicationCommandPermissions",
     "PartialGuildApplicationCommandPermissions",
     "PartialGuildAppCmdPerms",
     "UnresolvedGuildApplicationCommandPermissions",
 )
 
-from disnake.app_commands import __dict__ as __original_dict__
 locals().update(__original_dict__)
+
+del __original_dict__
```

### Comparing `discord-disnake-2.3.0.2/discord/channel.py` & `discord_disnake-2.3.0.2.post0/discord/channel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,44 @@
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-2021 Rapptz
+Copyright (c) 2021-present Disnake Development
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
 from disnake.channel import (
+    DMC,
+    MISSING,
     ArchivedThreadIterator,
     Asset,
     CategoryChannel,
     ChannelType,
     ClientException,
-    DMC,
     DMChannel,
     GroupChannel,
     Hashable,
     InvalidArgument,
-    MISSING,
     NewsChannel,
     Object,
     PartialMessageable,
     PermissionOverwrite,
     Permissions,
     StageChannel,
     StageInstance,
@@ -21,14 +46,15 @@
     StoreChannel,
     TextChannel,
     Thread,
     VideoQualityMode,
     VocalGuildChannel,
     VoiceChannel,
     VoiceRegion,
+    __dict__ as __original_dict__,
     _channel_factory,
     _channel_type_factory,
     _guild_channel_factory,
     _single_delete_strategy,
     _threaded_channel_factory,
     _threaded_guild_channel_factory,
     try_enum,
@@ -44,9 +70,10 @@
     "CategoryChannel",
     "NewsChannel",
     "StoreChannel",
     "GroupChannel",
     "PartialMessageable",
 )
 
-from disnake.channel import __dict__ as __original_dict__
 locals().update(__original_dict__)
+
+del __original_dict__
```

### Comparing `discord-disnake-2.3.0.2/discord/ext/commands/__init__.py` & `discord_disnake-2.3.0.2.post0/discord/ext/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-disnake-2.3.0.2/discord/ext/commands/base_core.py` & `discord_disnake-2.3.0.2.post0/discord/ext/commands/base_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,36 +48,38 @@
     MessageNotFound,
     MissingAnyRole,
     MissingFlagArgument,
     MissingPermissions,
     MissingRequiredArgument,
     MissingRequiredFlag,
     MissingRole,
-    NSFWChannelRequired,
     NoEntryPointError,
     NoPrivateMessage,
     NotOwner,
+    NSFWChannelRequired,
     ObjectNotFound,
     P,
     PartialEmojiConversionFailure,
     PrivateMessageOnly,
     RoleNotFound,
     T,
     ThreadNotFound,
     TooManyArguments,
     TooManyFlags,
     UnexpectedQuoteError,
     UnresolvedGuildApplicationCommandPermissions,
     UserInputError,
     UserNotFound,
+    __dict__ as __original_dict__,
     _get_overridden_method,
     async_all,
     guild_permissions,
     maybe_coroutine,
     warn_deprecated,
     wrap_callback,
 )
 
 __all__ = ("InvokableApplicationCommand", "guild_permissions")
 
-from disnake.ext.commands.base_core import __dict__ as __original_dict__
 locals().update(__original_dict__)
+
+del __original_dict__
```

### Comparing `discord-disnake-2.3.0.2/discord/ext/commands/ctx_menus_core.py` & `discord_disnake-2.3.0.2.post0/discord/ext/commands/ctx_menus_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,32 +42,34 @@
     MessageNotFound,
     MissingAnyRole,
     MissingFlagArgument,
     MissingPermissions,
     MissingRequiredArgument,
     MissingRequiredFlag,
     MissingRole,
-    NSFWChannelRequired,
     NoEntryPointError,
     NoPrivateMessage,
     NotOwner,
+    NSFWChannelRequired,
     ObjectNotFound,
     PartialEmojiConversionFailure,
     PrivateMessageOnly,
     RoleNotFound,
     ThreadNotFound,
     TooManyArguments,
     TooManyFlags,
     UnexpectedQuoteError,
     UserCommand,
     UserInputError,
     UserNotFound,
+    __dict__ as __original_dict__,
     _get_overridden_method,
     message_command,
     safe_call,
     user_command,
 )
 
 __all__ = ("InvokableUserCommand", "InvokableMessageCommand", "user_command", "message_command")
 
-from disnake.ext.commands.ctx_menus_core import __dict__ as __original_dict__
 locals().update(__original_dict__)
+
+del __original_dict__
```

### Comparing `discord-disnake-2.3.0.2/discord/ext/commands/errors.py` & `discord_disnake-2.3.0.2.post0/discord/ext/commands/slash_core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from disnake.ext.commands.errors import (
+from disnake.ext.commands.slash_core import (
+    ApplicationCommandInteraction,
     ArgumentParsingError,
     BadArgument,
     BadBoolArgument,
     BadColorArgument,
     BadColourArgument,
     BadFlagArgument,
     BadInviteArgument,
@@ -11,114 +12,70 @@
     BotMissingAnyRole,
     BotMissingPermissions,
     BotMissingRole,
     ChannelNotFound,
     ChannelNotReadable,
     CheckAnyFailure,
     CheckFailure,
-    ClientException,
     CommandError,
     CommandInvokeError,
     CommandNotFound,
     CommandOnCooldown,
     CommandRegistrationError,
     ConversionError,
     DisabledCommand,
-    DiscordException,
     EmojiNotFound,
     ExpectedClosingQuoteError,
     ExtensionAlreadyLoaded,
     ExtensionError,
     ExtensionFailed,
     ExtensionNotFound,
     ExtensionNotLoaded,
     FlagError,
     GuildNotFound,
     GuildStickerNotFound,
     InvalidEndOfQuotedStringError,
+    InvokableApplicationCommand,
+    InvokableSlashCommand,
     MaxConcurrencyReached,
     MemberNotFound,
     MessageNotFound,
     MissingAnyRole,
     MissingFlagArgument,
     MissingPermissions,
     MissingRequiredArgument,
     MissingRequiredFlag,
     MissingRole,
-    NSFWChannelRequired,
     NoEntryPointError,
     NoPrivateMessage,
     NotOwner,
+    NSFWChannelRequired,
     ObjectNotFound,
+    Option,
+    OptionType,
     PartialEmojiConversionFailure,
     PrivateMessageOnly,
     RoleNotFound,
+    SlashCommand,
+    SubCommand,
+    SubCommandGroup,
     ThreadNotFound,
     TooManyArguments,
     TooManyFlags,
     UnexpectedQuoteError,
     UserInputError,
     UserNotFound,
+    __dict__ as __original_dict__,
+    _autocomplete,
+    _call_autocompleter,
+    _get_overridden_method,
+    call_param_func,
+    expand_params,
+    slash_command,
+    utils,
 )
 
-__all__ = (
-    "CommandError",
-    "MissingRequiredArgument",
-    "BadArgument",
-    "PrivateMessageOnly",
-    "NoPrivateMessage",
-    "CheckFailure",
-    "CheckAnyFailure",
-    "CommandNotFound",
-    "DisabledCommand",
-    "CommandInvokeError",
-    "TooManyArguments",
-    "UserInputError",
-    "CommandOnCooldown",
-    "MaxConcurrencyReached",
-    "NotOwner",
-    "MessageNotFound",
-    "ObjectNotFound",
-    "MemberNotFound",
-    "GuildNotFound",
-    "UserNotFound",
-    "ChannelNotFound",
-    "ThreadNotFound",
-    "ChannelNotReadable",
-    "BadColourArgument",
-    "BadColorArgument",
-    "RoleNotFound",
-    "BadInviteArgument",
-    "EmojiNotFound",
-    "GuildStickerNotFound",
-    "PartialEmojiConversionFailure",
-    "BadBoolArgument",
-    "MissingRole",
-    "BotMissingRole",
-    "MissingAnyRole",
-    "BotMissingAnyRole",
-    "MissingPermissions",
-    "BotMissingPermissions",
-    "NSFWChannelRequired",
-    "ConversionError",
-    "BadUnionArgument",
-    "BadLiteralArgument",
-    "ArgumentParsingError",
-    "UnexpectedQuoteError",
-    "InvalidEndOfQuotedStringError",
-    "ExpectedClosingQuoteError",
-    "ExtensionError",
-    "ExtensionAlreadyLoaded",
-    "ExtensionNotLoaded",
-    "NoEntryPointError",
-    "ExtensionFailed",
-    "ExtensionNotFound",
-    "CommandRegistrationError",
-    "FlagError",
-    "BadFlagArgument",
-    "MissingFlagArgument",
-    "TooManyFlags",
-    "MissingRequiredFlag",
-)
+__all__ = ("InvokableSlashCommand", "SubCommandGroup", "SubCommand", "slash_command")
 
-from disnake.ext.commands.errors import __dict__ as __original_dict__
 locals().update(__original_dict__)
+
+del __original_dict__
```

### Comparing `discord-disnake-2.3.0.2/discord/ext/commands/slash_core.py` & `discord_disnake-2.3.0.2.post0/discord/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,101 @@
-from disnake.ext.commands.slash_core import (
-    ApplicationCommandInteraction,
-    ArgumentParsingError,
-    BadArgument,
-    BadBoolArgument,
-    BadColorArgument,
-    BadColourArgument,
-    BadFlagArgument,
-    BadInviteArgument,
-    BadLiteralArgument,
-    BadUnionArgument,
-    BotMissingAnyRole,
-    BotMissingPermissions,
-    BotMissingRole,
-    ChannelNotFound,
-    ChannelNotReadable,
-    CheckAnyFailure,
-    CheckFailure,
-    CommandError,
-    CommandInvokeError,
-    CommandNotFound,
-    CommandOnCooldown,
-    CommandRegistrationError,
-    ConversionError,
-    DisabledCommand,
-    EmojiNotFound,
-    ExpectedClosingQuoteError,
-    ExtensionAlreadyLoaded,
-    ExtensionError,
-    ExtensionFailed,
-    ExtensionNotFound,
-    ExtensionNotLoaded,
-    FlagError,
-    GuildNotFound,
-    GuildStickerNotFound,
-    InvalidEndOfQuotedStringError,
-    InvokableApplicationCommand,
-    InvokableSlashCommand,
-    MaxConcurrencyReached,
-    MemberNotFound,
-    MessageNotFound,
-    MissingAnyRole,
-    MissingFlagArgument,
-    MissingPermissions,
-    MissingRequiredArgument,
-    MissingRequiredFlag,
-    MissingRole,
-    NSFWChannelRequired,
-    NoEntryPointError,
-    NoPrivateMessage,
-    NotOwner,
-    ObjectNotFound,
-    Option,
-    OptionType,
-    PartialEmojiConversionFailure,
-    PrivateMessageOnly,
-    RoleNotFound,
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-2021 Rapptz
+Copyright (c) 2021-present Disnake Development
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from disnake.client import (
+    MISSING,
+    AllowedMentions,
+    AppInfo,
+    ApplicationCommand,
+    ApplicationCommandType,
+    ApplicationFlags,
+    BaseActivity,
+    ChannelType,
+    Client,
+    ClientException,
+    ClientUser,
+    ConnectionClosed,
+    ConnectionState,
+    Coro,
+    DiscordException,
+    DiscordServerError,
+    DiscordVoiceWebSocket,
+    DiscordWebSocket,
+    Emoji,
+    ExponentialBackoff,
+    Forbidden,
+    GatewayNotFound,
+    Guild,
+    GuildApplicationCommandPermissions,
+    GuildIterator,
+    GuildSticker,
+    HTTPClient,
+    HTTPException,
+    Intents,
+    InteractionException,
+    InteractionNotResponded,
+    InteractionResponded,
+    InteractionTimedOut,
+    InvalidArgument,
+    InvalidData,
+    Invite,
+    KeepAliveHandler,
+    LoginFailure,
+    MessageCommand,
+    NoMoreItems,
+    NotFound,
+    Object,
+    PartialGuildApplicationCommandPermissions,
+    PartialMessageable,
+    PrivilegedIntentsRequired,
+    ReconnectWebSocket,
     SlashCommand,
-    SubCommand,
-    SubCommandGroup,
-    ThreadNotFound,
-    TooManyArguments,
-    TooManyFlags,
-    UnexpectedQuoteError,
-    UserInputError,
-    UserNotFound,
-    _autocomplete,
-    _call_autocompleter,
-    _get_overridden_method,
-    call_param_func,
-    expand_params,
-    slash_command,
+    StageInstance,
+    StandardSticker,
+    Status,
+    StickerPack,
+    Template,
+    Thread,
+    User,
+    UserCommand,
+    View,
+    VoiceClient,
+    VoiceKeepAliveHandler,
+    VoiceRegion,
+    Webhook,
+    Widget,
+    __dict__ as __original_dict__,
+    _cancel_tasks,
+    _cleanup_loop,
+    _sticker_factory,
+    _threaded_channel_factory,
+    create_activity,
     utils,
 )
 
-__all__ = ("InvokableSlashCommand", "SubCommandGroup", "SubCommand", "slash_command")
+__all__ = ("Client",)
 
-from disnake.ext.commands.slash_core import __dict__ as __original_dict__
 locals().update(__original_dict__)
+
+del __original_dict__
```

### Comparing `discord-disnake-2.3.0.2/discord/ext/tasks/__init__.py` & `discord_disnake-2.3.0.2.post0/discord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-disnake-2.3.0.2/discord/interactions/application_command.py` & `discord_disnake-2.3.0.2.post0/discord/interactions/application_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from disnake.interactions.application_command import (
+    MISSING,
     AppCmdDataOptionT,
     AppCmdInter,
     AppCommandInter,
     AppCommandInteraction,
     ApplicationCommandInteraction,
     ApplicationCommandInteractionData,
     ApplicationCommandInteractionDataOption,
@@ -11,22 +12,22 @@
     CmdInter,
     CmdInteraction,
     CommandInter,
     CommandInteraction,
     Guild,
     GuildCommandInteraction,
     Interaction,
-    MISSING,
     Member,
     Message,
     MessageCommandInteraction,
     OptionType,
     Role,
     User,
     UserCommandInteraction,
+    __dict__ as __original_dict__,
     _threaded_channel_factory,
     try_enum,
 )
 
 __all__ = (
     "ApplicationCommandInteraction",
     "GuildCommandInteraction",
@@ -40,9 +41,10 @@
     "CommandInter",
     "CmdInter",
     "AppCommandInteraction",
     "AppCommandInter",
     "AppCmdInter",
 )
 
-from disnake.interactions.application_command import __dict__ as __original_dict__
 locals().update(__original_dict__)
+
+del __original_dict__
```

### Comparing `discord-disnake-2.3.0.2/discord_disnake.egg-info/PKG-INFO` & `discord_disnake-2.3.0.2.post0/discord_disnake.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 Metadata-Version: 2.1
 Name: discord-disnake
-Version: 2.3.0.2
+Version: 2.3.0.2.post0
 Summary: A shim for disnake (Python wrapper for the Discord API)
 Home-page: https://github.com/DisnakeDev/discord-disnake
 Author: Rapptz, EQUENOS
 License: MIT
 Project-URL: Documentation, https://docs.disnake.dev/en/latest
 Project-URL: Issue tracker, https://github.com/DisnakeDev/discord-disnake/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+Requires-Dist: disnake==2.3.0
+
+<p align="center">
+    <h3>⚠️⚠️⚠️ This package is deprecated and is no longer being maintained. ⚠️⚠️⚠️</h3>
+    Please migrate your project to use https://pypi.org/project/disnake directly.
+</p>
+
+<br/>
+<br/>
+
+---
+
+Original Readme:
 
 # This package is a shim
 
 This module allows to use [disnake](https://github.com/DisnakeDev/disnake) using `discord` namespace. This is not an independent library.
 
 # Installing
 
@@ -42,10 +54,8 @@
 py -3 -m pip install -U disnake[discord]
 ```
 
 # Links
 
 - [Documentation](https://docs.disnake.dev/en/latest)
 - [disnake GitHub](https://github.com/DisnakeDev/disnake)
-- [disnake Discord](https://discord.gg/gJDbCw8aQy)
-
-
+- [disnake Discord](https://discord.gg/disnake)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `discord-disnake-2.3.0.2/discord_disnake.egg-info/SOURCES.txt` & `discord_disnake-2.3.0.2.post0/discord_disnake.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 discord/mixins.py
 discord/object.py
 discord/oggparse.py
 discord/opus.py
 discord/partial_emoji.py
 discord/permissions.py
 discord/player.py
+discord/py.typed
 discord/raw_models.py
 discord/reaction.py
 discord/role.py
 discord/shard.py
 discord/stage_instance.py
 discord/state.py
 discord/sticker.py
```

### Comparing `discord-disnake-2.3.0.2/setup.py` & `discord_disnake-2.3.0.2.post0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     description="A shim for disnake (Python wrapper for the Discord API)",
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=requirements,
     python_requires=">=3.8.0",
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 7 - Inactive",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

