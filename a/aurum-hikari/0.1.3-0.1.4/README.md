# Comparing `tmp/aurum_hikari-0.1.3.tar.gz` & `tmp/aurum_hikari-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurum_hikari-0.1.3.tar", max compression
+gzip compressed data, was "aurum_hikari-0.1.4.tar", max compression
```

## Comparing `aurum_hikari-0.1.3.tar` & `aurum_hikari-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,44 @@
--rw-r--r--   0        0        0     1080 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/LICENSE
--rw-r--r--   0        0        0     3213 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/README.md
--rw-r--r--   0        0        0      479 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/aurum/__init__.py
--rw-r--r--   0        0        0      382 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/aurum/_about.py
--rw-r--r--   0        0        0     5173 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/aurum/client.py
--rw-r--r--   0        0        0      316 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/aurum/commands/__init__.py
--rw-r--r--   0        0        0      198 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/aurum/commands/decorators/__init__.py
--rw-r--r--   0        0        0      664 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/aurum/commands/decorators/sub_command.py
--rw-r--r--   0        0        0     1408 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/aurum/commands/message_command.py
--rw-r--r--   0        0        0     8420 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/aurum/commands/slash_command.py
--rw-r--r--   0        0        0     2193 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/aurum/commands/sub_commands.py
--rw-r--r--   0        0        0     1491 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/aurum/commands/user_command.py
--rw-r--r--   0        0        0        0 2024-05-16 15:13:09.894233 aurum_hikari-0.1.3/aurum/enum/__init__.py
--rw-r--r--   0        0        0       94 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/enum/sync_commands.py
--rw-r--r--   0        0        0        0 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/ext/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/ext/plugins/__init__.py
--rw-r--r--   0        0        0      284 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/includable.py
--rw-r--r--   0        0        0      220 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/interactions/__init__.py
--rw-r--r--   0        0        0     3790 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/interactions/interaction_context.py
--rw-r--r--   0        0        0        0 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/internal/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/internal/commands/__init__.py
--rw-r--r--   0        0        0     3523 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/internal/commands/app_command.py
--rw-r--r--   0        0        0     4263 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/internal/commands/command_handler.py
--rw-r--r--   0        0        0     1898 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/internal/commands/context_menu_command.py
--rw-r--r--   0        0        0       69 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/internal/consts.py
--rw-r--r--   0        0        0      290 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/internal/exceptions/__init__.py
--rw-r--r--   0        0        0       67 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/internal/exceptions/base_exception.py
--rw-r--r--   0        0        0      407 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/internal/exceptions/commands_exceptions.py
--rw-r--r--   0        0        0     6548 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/internal/interaction_processor.py
--rw-r--r--   0        0        0      360 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/l10n/__init__.py
--rw-r--r--   0        0        0      494 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/l10n/localization_provider_interface.py
--rw-r--r--   0        0        0      387 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/l10n/types.py
--rw-r--r--   0        0        0      219 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/options/__init__.py
--rw-r--r--   0        0        0      257 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/options/choice.py
--rw-r--r--   0        0        0      892 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/options/option.py
--rw-r--r--   0        0        0        0 2024-05-16 15:13:09.898233 aurum_hikari-0.1.3/aurum/py.typed
--rw-r--r--   0        0        0     1741 2024-05-16 15:13:19.386152 aurum_hikari-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 aurum_hikari-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3082 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/README.md
+-rw-r--r--   0        0        0      479 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/__init__.py
+-rw-r--r--   0        0        0      382 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/_about.py
+-rw-r--r--   0        0        0     5346 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/client.py
+-rw-r--r--   0        0        0      316 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/decorators/__init__.py
+-rw-r--r--   0        0        0     1099 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/decorators/sub_command.py
+-rw-r--r--   0        0        0     2321 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/message_command.py
+-rw-r--r--   0        0        0     9023 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/slash_command.py
+-rw-r--r--   0        0        0     1671 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/sub_command.py
+-rw-r--r--   0        0        0     2402 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/user_command.py
+-rw-r--r--   0        0        0        0 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/enum/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/enum/sync_commands.py
+-rw-r--r--   0        0        0        0 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/ext/__init__.py
+-rw-r--r--   0        0        0      241 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/ext/plugins/__init__.py
+-rw-r--r--   0        0        0     4227 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/ext/plugins/plugin.py
+-rw-r--r--   0        0        0     3333 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/ext/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      292 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/includable.py
+-rw-r--r--   0        0        0      220 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/interactions/__init__.py
+-rw-r--r--   0        0        0     7214 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/interactions/interaction_context.py
+-rw-r--r--   0        0        0        0 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/commands/__init__.py
+-rw-r--r--   0        0        0     3035 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/commands/app_command.py
+-rw-r--r--   0        0        0     4014 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/commands/command_handler.py
+-rw-r--r--   0        0        0     1937 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/commands/context_menu_command.py
+-rw-r--r--   0        0        0       75 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/consts.py
+-rw-r--r--   0        0        0      290 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/exceptions/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/exceptions/base_exception.py
+-rw-r--r--   0        0        0      456 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/exceptions/commands_exceptions.py
+-rw-r--r--   0        0        0     6407 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/interaction_processor.py
+-rw-r--r--   0        0        0      401 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/__init__.py
+-rw-r--r--   0        0        0      147 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/locale.py
+-rw-r--r--   0        0        0     1223 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/localization_provider_interface.py
+-rw-r--r--   0        0        0      255 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/localized.py
+-rw-r--r--   0        0        0      529 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/pass_localization_provider.py
+-rw-r--r--   0        0        0      207 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/types.py
+-rw-r--r--   0        0        0      219 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/options/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/options/choice.py
+-rw-r--r--   0        0        0     1715 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/options/option.py
+-rw-r--r--   0        0        0        0 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/py.typed
+-rw-r--r--   0        0        0      147 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/types.py
+-rw-r--r--   0        0        0     1987 2024-05-18 23:01:19.581538 aurum_hikari-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 aurum_hikari-0.1.4/PKG-INFO
```

### Comparing `aurum_hikari-0.1.3/LICENSE` & `aurum_hikari-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.3/README.md` & `aurum_hikari-0.1.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         <a href="https://github.com/ShinshiDevs/aurum-hikari">
             <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/w/ShinshiDevs/aurum-hikari">
             <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues-closed/ShinshiDevs/aurum-hikari">
             <img alt="GitHub License" src="https://img.shields.io/github/license/ShinshiDevs/aurum-hikari">
         </a>
     </p>
     <p>
-        <a href="https://shinshidevs.github.io/aurum-hikari/docs/">Documentation</a>
+        <a href="https://shinshidevs.github.io/aurum-hikari/">Documentation</a>
         ·
         <a href="https://github.com/ShinshiDevs/aurum-hikari/releases">Releases</a>
         ·
         <a href="https://pypi.org/project/aurum-hikari/">PyPI</a>
         ·
         <a href="./LICENSE">License</a>
     </p>
@@ -36,19 +36,16 @@
         <text>
             Our goal is to provide you, as developers, with complete freedom of action and to highlight the benefits of Hikari.
         </text>
     </p>
 </div>
 
 # Installation
-> [!CAUTION]
-> This library is in the planning stage of development, it cannot be installed and used. Thanks!
-
 > [!NOTE]
-> This library requires Python version 3.10 or higher.
+> Aurum requires Python 3.10 or higher.
 
 Run command:
 ```md
 pip install aurum-hikari
 # Or
 python -m pip install aurum-hikari # for unix-type systems
 py -m pip install aurum-hikari # for windows
```

### Comparing `aurum_hikari-0.1.3/aurum/client.py` & `aurum_hikari-0.1.4/aurum/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,127 +3,125 @@
 import asyncio
 import typing
 from logging import getLogger
 
 from hikari.events import InteractionCreateEvent, StartedEvent, StartingEvent
 
 from aurum.enum.sync_commands import SyncCommandsFlag
-from aurum.includable import Includable
+from aurum.ext.plugins import PluginManager
 from aurum.internal.commands.app_command import AppCommand
 from aurum.internal.commands.command_handler import CommandHandler
+from aurum.internal.exceptions.base_exception import AurumException
 from aurum.internal.interaction_processor import InteractionProcessor
-from aurum.l10n import LocalizationProviderInterface
+from aurum.l10n.pass_localization_provider import PassLocalizationProvider
 
 if typing.TYPE_CHECKING:
     from collections.abc import Coroutine, Sequence
     from logging import Logger
 
-    from hikari.impl import GatewayBot
+    from aurum.includable import Includable
+    from aurum.l10n import LocalizationProviderInterface
+    from aurum.types import BotT
 
 __all__: Sequence[str] = ("Client",)
 
 
 class Client:
-    """
-    A wrapper class for the main bot class, designed to work with the Aurum framework and its features.
+    """A wrapper class for the main bot class, designed to work with the Aurum framework and its features.
 
-    At the moment, the wrapper only supports gateway connections.
+    Note:
+        At the moment, the wrapper only supports gateway connections.
 
     Attributes:
-        bot (GatewayBot): The bot instance.
         l10n (LocalizationProviderInterface): The localization provider instance for multi-language support.
             It is recommended to provide a localization provider if multi-language support is required.
-            You can use the our DefaultLocalizationProvider or create your own by inheriting from the LocalizationProviderInterface.
+        bot (BotT): The bot instance.
+        commands (CommandHandler): The command handler.
+        plugins (PluginManager): The plugin manager.
 
     Args:
-        bot: The bot instance that this client will interact with.
-        sync_commands: An optional SyncCommandsFlag enum value, indicating how to handle command synchronization.
-        l10n: Localization provider.
-            If a localization provider is not provided, an `EmptyLocalizationProvider` will be used, which will pass all functions and return the key.
-        ignore_l10n: An optional boolean flag. If `True`, the client will not emit a warning when a localization provider is not provided.
-        ignore_unknown_interactions: An optional boolean flag that, if set to `True`, will disable the warning message for unknown interactions.
-
-    Examples:
-        ```py
-        bot = hikari.GatewayBot("...")
-        l10n = MyCoolLocalizationProvider()
-        client = Client(bot, l10n=l10n)
-        ```
+        bot (BotT): The bot instance that this client will interact with.
+        sync_commands (SyncCommandFlag): An optional SyncCommandsFlag enum value, indicating how to handle command synchronization.
+        l10n (LocalizationProviderInterface): Localization provider.
+            If a localization provider is not provided, an `EmptyLocalizationProvider`
+            will be used, which will pass all functions and return the key.
+        ignore_l10n (bool): An optional flag. If `True`, the client will not emit a warning when a localization provider is not provided.
+        ignore_unknown_interactions (bool): An optional flag that, if set to `True`, will disable the warning message for unknown interactions.
     """
 
     __slots__: Sequence[str] = (
+        "l10n",
         "__logger",
         "_starting_tasks",
-        "_commands",
-        "_interaction_processor",
         "_sync_commands",
+        "_interaction_processor",
         "bot",
-        "l10n",
+        "commands",
+        "plugins",
     )
 
     def __init__(
         self,
-        bot: GatewayBot,
+        bot: BotT,
         *,
         sync_commands: SyncCommandsFlag = SyncCommandsFlag.SYNC,
         l10n: LocalizationProviderInterface | None = None,
         ignore_l10n: bool = False,
         ignore_unknown_interactions: bool = False,
     ) -> None:
         self.__logger: Logger = getLogger("aurum.client")
         self._starting_tasks: typing.List[Coroutine[None, None, typing.Any]] = []
-
-        self.bot: GatewayBot = bot
+        self._sync_commands: SyncCommandsFlag = sync_commands
 
         if not l10n and not ignore_l10n:
             self.__logger.warning(
-                "A localization provider has not been specified and localization will not be available. "
+                "a localization provider has not been specified and localization will not be available. "
                 "If you require localization, please use one of the available localization providers "
                 "or create your own implementation based on the LocalizationProviderInterface."
             )
-        self.l10n: LocalizationProviderInterface = l10n or EmptyLocalizationProvider()
+        self.l10n: LocalizationProviderInterface = l10n or PassLocalizationProvider()
         self.add_starting_task(self.l10n.start())
 
-        self._commands: CommandHandler = CommandHandler(bot, self.l10n)
+        self.bot: BotT = bot
+        self.commands: CommandHandler = CommandHandler(bot, self.l10n)
+        self.plugins: PluginManager = PluginManager(bot, self)
         self._interaction_processor: InteractionProcessor = InteractionProcessor(
             bot=bot,
             client=self,
             l10n=self.l10n,
-            commands=self._commands,
-            components=None,
+            commands=self.commands,
             ignore_unknown_interactions=ignore_unknown_interactions,
-            get_locale_func=self.l10n.get_locale_from_interaction,
+            get_locale_func=self.l10n.get_locale,
         )
-        self._sync_commands: SyncCommandsFlag = sync_commands
 
         for event, callback in {
             StartingEvent: self._on_starting,
             StartedEvent: self._on_started,
         }.items():
-            self.bot.event_manager.subscribe(event, callback)
+            self.bot.event_manager.subscribe(event, callback)  # type: ignore
 
     async def _on_starting(self, _: StartingEvent) -> None:
         try:
             await asyncio.gather(*self._starting_tasks)
-            self.__logger.debug("Completed all tasks")
+            self.__logger.debug("completed all tasks")
         except Exception as exception:
             self.__logger.warning(
-                "Some tasks weren't completed because of an exception", exc_info=exception
+                "some tasks weren't completed because of an exception", exc_info=exception
             )
 
     async def _on_started(self, _: StartedEvent) -> None:
         if self._sync_commands.value:
-            await self._commands.sync(debug=self._sync_commands == SyncCommandsFlag.DEBUG)
+            await self.commands.sync(debug=self._sync_commands == SyncCommandsFlag.DEBUG)
         self.bot.event_manager.subscribe(
             InteractionCreateEvent, self._interaction_processor.on_interaction
         )
 
     def add_starting_task(self, coro: Coroutine[None, None, typing.Any]) -> None:
         self._starting_tasks.append(coro)
 
     def include(self, includable: typing.Type[Includable]) -> None:
         if issubclass(includable, AppCommand):
-            instance: AppCommand = includable()  # type: ignore
-            self._commands.commands[instance.name] = instance
-
-
-class EmptyLocalizationProvider(LocalizationProviderInterface): ...
+            try:
+                instance: AppCommand = includable()  # type: ignore
+            except ValueError:
+                raise AurumException("`__init__` of base includable wasn't overrided")
+            self.commands.commands[instance.name] = instance
```

### Comparing `aurum_hikari-0.1.3/aurum/commands/decorators/sub_command.py` & `aurum_hikari-0.1.4/aurum/commands/decorators/sub_command.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,38 @@
 from __future__ import annotations
 
 import typing
 
-from aurum.commands.sub_commands import SubCommand
+from aurum.commands.sub_command import SubCommand
 
 if typing.TYPE_CHECKING:
     from collections.abc import Awaitable, Callable, Sequence
 
     from aurum.l10n import LocalizedOr
     from aurum.options import Option
 
 
 def sub_command(
     name: str,
     description: LocalizedOr[str] | None = None,
     options: Sequence[Option] = (),
 ) -> Callable[..., SubCommand]:
+    """Decorator for the sub-command.
+
+    Can be used only in a command class that inherits from `aurum.commands.slash_command.SlashCommand`.
+
+    Args:
+        name (str): The unique name for the sub-command.
+        description (LocalizedOr[str] | None): Optional description for the sub-command.
+        options (Sequence[Option]): Optional options of the sub-command.
+
+    Note:
+        The callback must be asynchronous.
+    """
+
     def decorator(func: Callable[..., Awaitable[None]]) -> SubCommand:
         return SubCommand(
             callback=func,
             name=name,
             description=description,
             options=options,
         )
```

### Comparing `aurum_hikari-0.1.3/aurum/commands/slash_command.py` & `aurum_hikari-0.1.4/aurum/commands/slash_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,101 +2,96 @@
 
 import typing
 
 from hikari.commands import CommandChoice, CommandOption, CommandType, OptionType
 from hikari.permissions import Permissions
 from hikari.undefined import UNDEFINED
 
-from aurum.commands.sub_commands import SubCommand
+from aurum.commands.sub_command import SubCommand
 from aurum.internal.commands.app_command import AppCommand
-from aurum.internal.consts import SUB_COMMANDS_VAR
+from aurum.internal.consts import SUB_COMMANDS_CONTAINER
 from aurum.l10n import Localized
 
 if typing.TYPE_CHECKING:
     from collections.abc import Callable, Sequence
 
     from hikari.api import SlashCommandBuilder
     from hikari.guilds import PartialGuild
     from hikari.snowflakes import SnowflakeishOr
     from hikari.undefined import UndefinedType
 
+    from aurum.interactions import InteractionContext
     from aurum.l10n import LocalizationProviderInterface, LocalizedOr
     from aurum.options import Option
 
 
 class SlashCommandMeta(type):
     def __new__(
         mcs: typing.Type[SlashCommandMeta],
         name: str,
         bases: typing.Tuple[type, ...],
         attrs: typing.Dict[str, typing.Any],
     ) -> SlashCommandMeta:
         cls: SlashCommandMeta = super().__new__(mcs, name, bases, attrs)
-        setattr(cls, SUB_COMMANDS_VAR, {})
+        setattr(cls, SUB_COMMANDS_CONTAINER, {})
         for name, obj in attrs.items():
             if isinstance(obj, SubCommand):
-                getattr(cls, SUB_COMMANDS_VAR)[obj.name] = obj
+                getattr(cls, SUB_COMMANDS_CONTAINER)[obj.name] = obj
         return cls
 
 
 class SlashCommand(AppCommand, metaclass=SlashCommandMeta):
-    """
-    Represents a slash-command.
-
-    Attributes:
-        _app (PartialCommand): Command application instance, available after sync.
-        command_type (CommandType): Type of the command.
-        name (str): The command name.
-        description (LocalizedOr[str] | None): Optional description of the command for help documentation.
-        guild (SnowflakeishOr[PartialGuild] | UndefinedType): Optional guild (server) where the command is available.
-        default_member_permissions (Permissions): The permissions a user must have to use the command by default.
-        dm_enabled (bool): Whether the command can be used in direct messages.
-        is_nsfw (bool): Indicates whether the command is age-restricted.
-        options (Sequence[Option]): Options to the command.
-        sub_commands (Dict[str, SubCommand]): Sub-commands of the command.
+    """Represents a slash-command.
 
     Args:
         name (str): The unique name of the command.
         description (LocalizedOr[str] | None): A description of command.
         guild (SnowflakeishOr[PartialGuild] | UndefinedType): The guild in which the command is available.
         default_member_permissions (Permissions): Permissions required to use the command, if any. Defaults to NONE.
-        dm_enabled (bool): Flag indicating whether the command is available in direct messages. Defaults to `False`.
+        is_dm_enabled (bool): Flag indicating whether the command is available in direct messages. Defaults to `False`.
         is_nsfw (bool): Flag indicating whether the command should only be available in NSFW channels. Defaults to `False`.
         options (Sequence[Option]): Options to the command.
 
-    Methods:
-        Inherited from AppCommand class.
-
-    Note:
-        If your command has sub-commands, the callback will not be executed.
+    Attributes:
+        options (Sequence[Option]): Options to the command.
+        sub_commands (Dict[str, SubCommand]): Sub-commands of the command.
 
     Example:
-        ```py
-        class HelloCommand(SlashCommand):
+        === "With callback"
+            ```py
+            class HelloCommand(SlashCommand):
             def __init__(self) -> None:
-                super().__init__(name="hello", description="Say hi to bot")
+                super().__init__(name="hello", description="Say hi to bot")  # (1)
 
             async def callback(self, context: InteractionContext) -> None:
                 await context.create_response(f"Hi, {context.user.mention}!")
-        ```
+            ```
+
+            1. Base information about your command: name, description, default member permissions and etc.
 
-    Example with sub-commands:
-        ```py
-        class ABCCommand(SlashCommand):
+        === "With sub-commands"
+            ```py
+            class ABCCommand(SlashCommand):  # (1)
             def __init__(self) -> None:
-                super().__init__(name="a")
+                super().__init__(name="a")  # (2)
 
-            @sub_command(name="b")
+            @sub_command(name="b")  # (3)
             async def b_command(self, context: InteractionContext) -> None:
-                ...
+                ...  # (4)
 
             @b_command.sub_command(name="c")
             async def b_c_command(self, context: InteractionContext) -> None:
                 ...
-        ```
+            ```
+
+            1. When command has a sub-commands, callback will be ignored.
+            2. Base information about your command: name, description, default member permissions and etc.
+            3. Base information about your sub-command.
+                The same fields with slash-command, but without guild, default member permissions, is nsfw, dm enabled flags.
+            4. If sub-command have another sub-command, callback of parent sub-command will be ignored too.
     """
 
     __slots__: Sequence[str] = (
         "_app",
         "command_type",
         "name",
         "description",
@@ -111,29 +106,42 @@
     def __init__(
         self,
         name: str,
         description: LocalizedOr[str] | None = None,
         *,
         guild: SnowflakeishOr[PartialGuild] | UndefinedType = UNDEFINED,
         default_member_permissions: Permissions = Permissions.NONE,
-        dm_enabled: bool = False,
+        is_dm_enabled: bool = False,
         is_nsfw: bool = False,
         options: Sequence[Option] = (),
     ) -> None:
         super().__init__(
             command_type=CommandType.SLASH,
             name=name,
             description=description,
             guild=guild,
             default_member_permissions=default_member_permissions,
-            dm_enabled=dm_enabled,
+            is_dm_enabled=is_dm_enabled,
             is_nsfw=is_nsfw,
         )
         self.options: Sequence[Option] = options
-        self.sub_commands: typing.Dict[str, SubCommand] = getattr(self, SUB_COMMANDS_VAR, {})
+        self.sub_commands: typing.Dict[str, SubCommand] = getattr(self, SUB_COMMANDS_CONTAINER, {})
+
+    async def callback(self, context: InteractionContext) -> None:
+        """A callback of the command.
+
+        Meant to override this method to set the callback to the command.
+
+        Warning:
+            This callback will be ignored if the command has a sub-commands.
+        """
+        # TODO: a callback decorator or something to fix this error
+        # Current problem is `Signature of "callback" incompatible with supertype "SlashCommand" - Mypy(override)`
+        # because `callback(self, context: InteractionContext)` != `callback(self, context: InteractionContext, arg_1, arg_2, etc)`
+        pass
 
     def __build_option(self, option: Option, l10n: LocalizationProviderInterface) -> CommandOption:
         choices: tuple[CommandChoice, ...] = tuple(
             CommandChoice(
                 name=str(choice.name),
                 name_localizations=(
                     l10n.build_localized(choice.name) if isinstance(choice.name, Localized) else {}
@@ -193,19 +201,21 @@
         )
 
     def get_builder(
         self,
         factory: Callable[[str, str], SlashCommandBuilder],
         l10n: LocalizationProviderInterface,
     ) -> SlashCommandBuilder:
-        description: str = str(self.description) if not self.sub_commands else self.name
+        description: str = (
+            str(self.description or "No description") if not self.sub_commands else self.name
+        )
         builder: SlashCommandBuilder = (
             factory(self.name, description)
             .set_default_member_permissions(self.default_member_permissions)
-            .set_is_dm_enabled(self.dm_enabled)
+            .set_is_dm_enabled(self.is_dm_enabled)
             .set_is_nsfw(self.is_nsfw)
         )
         if not self.sub_commands:
             if isinstance(self.description, Localized):
                 builder.set_description_localizations(l10n.build_localized(self.description))
         for command in self.sub_commands.values():
             if command.sub_commands:
```

### Comparing `aurum_hikari-0.1.3/aurum/commands/sub_commands.py` & `aurum_hikari-0.1.4/aurum/commands/message_command.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,67 @@
 from __future__ import annotations
 
 import typing
-from dataclasses import dataclass, field
 
-from aurum.options import Option
+from hikari.commands import CommandType
+from hikari.permissions import Permissions
+from hikari.undefined import UNDEFINED
 
-if typing.TYPE_CHECKING:
-    from collections.abc import Awaitable, Callable, Sequence
-
-    from aurum.l10n.types import LocalizedOr
-
-
-@dataclass(slots=True, kw_only=True)
-class SubCommand:
-    """
-    A class representing a sub-command.
-
-    Attributes:
-        callback (Callable[..., Awaitable[Any]]): A callback of sub-command.
-        name (str): The internal name of the command used for identification, display if `display_name` is not provided.
-        description (LocalizedOr[str] | None): Optional description of the command for help documentation.
-        display_name (LocalizedOr[str] | None): Optional localized display name of the command.
-        options (Sequence[Option]): Options to the command.
-        sub_commands (Dict[str, SubCommand]): Sub-commands of the sub-command.
+from aurum.internal.commands.context_menu_command import ContextMenuCommand
 
-    Methods:
-        sub_command: A decorator method used to add a new sub-command to this.
+if typing.TYPE_CHECKING:
+    from hikari.guilds import PartialGuild
+    from hikari.messages import Message
+    from hikari.snowflakes import SnowflakeishOr
+    from hikari.undefined import UndefinedType
+
+    from aurum.interactions import InteractionContext
+
+
+class MessageCommand(ContextMenuCommand):
+    """Represents an application command for message's context menu.
+
+    Args:
+        name (str): The unique name of the command.
+        guild (SnowflakeishOr[PartialGuild] | UndefinedType): Optional guild (server) where the command is available.
+        default_member_permissions (Permissions): The permissions a user must have to use the command by default.
+        is_dm_enabled (bool): Whether the command can be used in direct messages.
+        is_nsfw (bool): Indicates whether the command is age-restricted.
 
     Example:
         ```py
-        class ABCCommand(SlashCommand):
+        class ReverseTextCommand(MessageCommand):
             def __init__(self) -> None:
-                super().__init__(name="a")
+                super().__init__(name="Reverse", dm_enabled=True)
 
-            @sub_command(name="b")
-            async def b_command(self, context: InteractionContext) -> None:
-                ...
-
-            @b_command.sub_command(name="c")
-            async def b_c_command(self, context: InteractionContext) -> None:
-                ...
+            async def callback(self, context: InteractionContext, message: Message) -> None:
+                await context.create_response(message.content[::-1])
         ```
     """
 
-    callback: Callable[..., Awaitable[typing.Any]]
-
-    name: str
-    description: LocalizedOr[str] | None = None
-
-    options: Sequence[Option] = field(default_factory=tuple[Option])
-
-    sub_commands: typing.Dict[str, SubCommand] = field(default_factory=dict)
-
-    def sub_command(
+    def __init__(
         self,
         name: str,
-        description: LocalizedOr[str] | None = None,
-        options: Sequence[Option] = (),
-    ) -> Callable[..., None]:
-        def decorator(func: Callable[..., Awaitable[None]]) -> None:
-            self.sub_commands[name] = SubCommand(
-                callback=func,
-                name=name,
-                description=description,
-                options=options,
-            )
-
-        return decorator
+        *,
+        guild: SnowflakeishOr[PartialGuild] | UndefinedType = UNDEFINED,
+        default_member_permissions: Permissions = Permissions.NONE,
+        is_dm_enabled: bool = False,
+        is_nsfw: bool = False,
+    ) -> None:
+        super().__init__(
+            command_type=CommandType.MESSAGE,
+            name=name,
+            guild=guild,
+            default_member_permissions=default_member_permissions,
+            is_dm_enabled=is_dm_enabled,
+            is_nsfw=is_nsfw,
+        )
+
+    async def callback(self, context: InteractionContext, message: Message) -> None:
+        """A callback of the command.
+
+        Meant to override this method to set the callback to the command.
+
+        Raises:
+            NotImplementedError: If callback wasn't overrided.
+        """
+        raise NotImplementedError()
```

### Comparing `aurum_hikari-0.1.3/aurum/commands/user_command.py` & `aurum_hikari-0.1.4/aurum/internal/commands/context_menu_command.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,65 @@
 from __future__ import annotations
 
 import typing
 
-from hikari.commands import CommandType
 from hikari.permissions import Permissions
 from hikari.undefined import UNDEFINED
 
-from aurum.internal.commands.context_menu_command import ContextMenuCommand
+from aurum.internal.commands.app_command import AppCommand
 
 if typing.TYPE_CHECKING:
+    from collections.abc import Callable, Sequence
+
+    from hikari.api import ContextMenuCommandBuilder
+    from hikari.commands import CommandType
     from hikari.guilds import PartialGuild
-    from hikari.interactions import InteractionMember
     from hikari.snowflakes import SnowflakeishOr
     from hikari.undefined import UndefinedType
-    from hikari.users import PartialUser
-
-    from aurum.interactions import InteractionContext
 
+    from aurum.l10n import LocalizationProviderInterface
 
-class UserCommand(ContextMenuCommand):
-    """
-    Represents a user-command.
 
-    Raises:
-        NotImplementedError: This method should be overridden in a subclass and will raise an exception if called directly.
-    """
+class ContextMenuCommand(AppCommand):
+    __slots__: Sequence[str] = (
+        "_app",
+        "command_type",
+        "name",
+        "display_name",
+        "guild",
+        "default_member_permissions",
+        "dm_enabled",
+        "is_nsfw",
+    )
 
     def __init__(
         self,
+        command_type: CommandType,
         name: str,
         *,
         guild: SnowflakeishOr[PartialGuild] | UndefinedType = UNDEFINED,
         default_member_permissions: Permissions = Permissions.NONE,
-        dm_enabled: bool = False,
+        is_dm_enabled: bool = False,
         is_nsfw: bool = False,
     ) -> None:
         super().__init__(
-            command_type=CommandType.USER,
+            command_type=command_type,
             name=name,
+            description=None,
             guild=guild,
             default_member_permissions=default_member_permissions,
-            dm_enabled=dm_enabled,
+            is_dm_enabled=is_dm_enabled,
             is_nsfw=is_nsfw,
         )
 
-    async def callback(
-        self, context: InteractionContext, target: InteractionMember | PartialUser
-    ) -> None:
-        raise NotImplementedError()
+    def get_builder(
+        self,
+        factory: Callable[[CommandType | int, str], ContextMenuCommandBuilder],
+        l10n: LocalizationProviderInterface,  # type: ignore  # TODO: display name
+    ) -> ContextMenuCommandBuilder:
+        builder = (
+            factory(self.command_type, self.name)
+            .set_default_member_permissions(self.default_member_permissions)
+            .set_is_dm_enabled(self.is_dm_enabled)
+            .set_is_nsfw(self.is_nsfw)
+        )
+        return builder
```

### Comparing `aurum_hikari-0.1.3/aurum/internal/commands/command_handler.py` & `aurum_hikari-0.1.4/aurum/internal/commands/command_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,26 +27,14 @@
     """Handles command building and synchronization for a bot application.
 
     This class is responsible for application commands.
     It registers commands, synchronizes them with the Discord API.
 
     Attributes:
         commands (typing.Dict[str, AppCommand]): Dictionary that stores the actual AppCommand instances, keyed by their names.
-
-    Args:
-        bot (GatewayBot): A bot instance.
-
-    Methods:
-        sync: Sync commands with the Discord API.
-        get_command:
-            Get command.
-
-            Returns:
-                AppCommand
-                None: If command wasn't found
     """
 
     __slots__: Sequence[str] = (
         "__logger",
         "_app",
         "_bot",
         "_l10n",
@@ -62,16 +50,15 @@
         self._commands_builders: typing.Dict[
             SnowflakeishOr[PartialGuild] | UndefinedType, typing.Dict[str, CommandBuilder]
         ] = {}
 
         self.commands: typing.Dict[str, AppCommand] = {}
 
     async def sync(self, debug: bool = False) -> None:
-        """
-        Synchronizes the builders of commands with the Discord API for the bot application.
+        """Synchronizes the builders of commands with the Discord API for the bot application.
 
         This method will handle both global commands and guild-specific commands,
         ensuring they are up-to-date with the currently stored command builders.
 
         Args:
             debug: A boolean flag that, when set to True, enables more verbose logging
                    of the synchronization process for debugging purposes.
@@ -98,15 +85,15 @@
             self._app, list(self._commands_builders.pop(UNDEFINED).values())
         )
         for guild, commands_builders in self._commands_builders.items():
             synchronized[guild] = await self._bot.rest.set_application_commands(
                 self._app, list(commands_builders.values()), guild=guild
             )
         for entity, commands in synchronized.items():
-            for command in commands:
-                self.commands[command.name]._app = command
+            for partial_command in commands:
+                self.commands[command.name].set_app(partial_command)
             if debug:
                 self.__logger.debug(
                     "Set commands for %s: %s",
                     entity,
                     ", ".join(command.name for command in commands),
                 )
```

### Comparing `aurum_hikari-0.1.3/aurum/internal/commands/context_menu_command.py` & `aurum_hikari-0.1.4/aurum/internal/commands/app_command.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,90 @@
 from __future__ import annotations
 
 import typing
 
 from hikari.permissions import Permissions
 from hikari.undefined import UNDEFINED
 
-from aurum.internal.commands.app_command import AppCommand
+from aurum.includable import Includable
 
 if typing.TYPE_CHECKING:
-    from collections.abc import Callable, Sequence
+    from collections.abc import Sequence
 
-    from hikari.api import ContextMenuCommandBuilder
-    from hikari.commands import CommandType
+    from hikari.commands import CommandType, PartialCommand
     from hikari.guilds import PartialGuild
     from hikari.snowflakes import SnowflakeishOr
     from hikari.undefined import UndefinedType
 
-    from aurum.l10n import LocalizationProviderInterface, Localized
+    from aurum.l10n.types import LocalizedOr
 
 
-class ContextMenuCommand(AppCommand):
+class AppCommand(Includable):
+    """Represents an application command.
+
+    !!! This class is not suitable for use, please use the pre-existing implementations.
+
+    Attributes:
+        app (PartialCommand): Command application instance, available after sync.
+        command_type (CommandType): Type of the command.
+        name (str): The command name.
+        description (LocalizedOr[str] | None): An optional description of the command.
+        guild (SnowflakeishOr[PartialGuild] | UndefinedType): An optional guild (server) where the command is available.
+        default_member_permissions (Permissions): The permissions a user must have to use the command by default.
+        dm_enabled (bool): Whether the command can be used in direct messages.
+        is_nsfw (bool): Indicates whether the command is age-restricted.
+    """
+
     __slots__: Sequence[str] = (
-        "_app",
-        "command_type",
+        "app",
         "name",
         "display_name",
         "guild",
         "default_member_permissions",
-        "dm_enabled",
+        "is_dm_enabled",
         "is_nsfw",
+        "description",
+        "command_type",
     )
 
     def __init__(
         self,
         command_type: CommandType,
         name: str,
+        description: LocalizedOr[str] | None = None,
         *,
         guild: SnowflakeishOr[PartialGuild] | UndefinedType = UNDEFINED,
         default_member_permissions: Permissions = Permissions.NONE,
-        dm_enabled: bool = False,
+        is_dm_enabled: bool = False,
         is_nsfw: bool = False,
     ) -> None:
-        super().__init__(
-            command_type=command_type,
-            name=name,
-            description=None,
-            guild=guild,
-            default_member_permissions=default_member_permissions,
-            dm_enabled=dm_enabled,
-            is_nsfw=is_nsfw,
-        )
+        super().__init__(name=name)
+        self.app: PartialCommand | None = None
 
-    def get_builder(
-        self,
-        factory: Callable[[CommandType | int, str], ContextMenuCommandBuilder],
-        l10n: LocalizationProviderInterface,
-    ) -> ContextMenuCommandBuilder:
-        builder = (
-            factory(self.command_type, self.name)
-            .set_default_member_permissions(self.default_member_permissions)
-            .set_is_dm_enabled(self.dm_enabled)
-            .set_is_nsfw(self.is_nsfw)
-        )
-        return builder
+        self.guild: SnowflakeishOr[PartialGuild] | UndefinedType = guild
+
+        self.default_member_permissions: Permissions = default_member_permissions
+        self.is_dm_enabled: bool = is_dm_enabled
+        self.is_nsfw: bool = is_nsfw
+
+        self.description: LocalizedOr[str] | None = description
+        self.command_type: CommandType = command_type
+
+    def set_app(self, application: PartialCommand) -> AppCommand:
+        self.app = application
+        return self
+
+    def set_guild(self, guild: SnowflakeishOr[PartialGuild] | UndefinedType) -> AppCommand:
+        self.guild = guild
+        return self
+
+    def set_default_member_permissions(self, permissions: Permissions) -> AppCommand:
+        self.default_member_permissions = permissions
+        return self
+
+    def set_is_dm_enabled(self, dm_enabled: bool) -> AppCommand:
+        self.is_dm_enabled = dm_enabled
+        return self
+
+    def set_is_nsfw(self, nsfw: bool) -> AppCommand:
+        self.is_nsfw = nsfw
+        return self
```

### Comparing `aurum_hikari-0.1.3/aurum/internal/interaction_processor.py` & `aurum_hikari-0.1.4/aurum/internal/interaction_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,55 +20,52 @@
     from hikari.interactions import (
         CommandInteractionOption,
         ComponentInteraction,
         PartialInteraction,
     )
 
     from aurum.client import Client
-    from aurum.commands.sub_commands import SubCommand
+    from aurum.commands.sub_command import SubCommand
     from aurum.internal.commands.app_command import AppCommand
     from aurum.internal.commands.command_handler import CommandHandler
     from aurum.l10n import Locale, LocalizationProviderInterface
 
-type ComponentHandler = None  # TODO: Remove that, when ComponentHandler will appear
-
 
 class InteractionProcessor:
+    """Processor of interactions"""
+
     __slots__: Sequence[str] = (
         "bot",
         "client",
         "l10n",
         "commands",
-        "components",
         "ignore_unknown_interactions",
         "get_locale_func",
     )
 
     def __init__(
         self,
         bot: GatewayBot,
         client: Client,
         l10n: LocalizationProviderInterface,
         commands: CommandHandler,
-        components: ComponentHandler,
         ignore_unknown_interactions: bool,
-        get_locale_func: Callable[[CommandInteraction | ComponentInteraction], Locale],
+        get_locale_func: Callable[[str | CommandInteraction | ComponentInteraction], Locale | None],
     ) -> None:
         self.bot: GatewayBot = bot
         self.client: Client = client
         self.l10n: LocalizationProviderInterface = l10n
 
         self.commands: CommandHandler = commands
-        self.components: ComponentHandler = components
 
         self.ignore_unknown_interactions: bool = ignore_unknown_interactions
 
-        self.get_locale_func: Callable[[CommandInteraction | ComponentInteraction], Locale] = (
-            get_locale_func
-        )
+        self.get_locale_func: Callable[
+            [str | CommandInteraction | ComponentInteraction], Locale | None
+        ] = get_locale_func
 
     def create_interaction_context(
         self, interaction: ComponentInteraction | CommandInteraction
     ) -> InteractionContext:
         return InteractionContext(
             interaction=interaction,
             bot=self.bot,
```

### Comparing `aurum_hikari-0.1.3/aurum/options/option.py` & `aurum_hikari-0.1.4/aurum/options/option.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,23 +13,51 @@
     from hikari.commands import OptionType
 
     from aurum.l10n.types import LocalizedOr
 
 
 @dataclass(slots=True, kw_only=True)
 class Option:
-    type: OptionType
+    """Represents the command option."""
 
-    name: LocalizedOr[str]
+    type: OptionType
+    """The option type"""
+    name: str  # TODO: make a display_name soon
+    """The unique name of the option"""
     description: LocalizedOr[str]
-
+    """The description of the option"""
     is_required: bool = True
+    """An optional flag is the option is required.
+    
+    Default: True"""
     choices: Sequence[Choice] = field(default_factory=tuple[Choice])
-
+    """A list of choices to the option"""
     max_length: int | None = None
+    """An optional maximum length of the option value.
+
+    Note:
+        Available only for the string option type.
+    """
     min_length: int | None = None
-    """Only for string option"""
+    """An optional minimum length of the option value.
+
+    Note:
+        Available only for the string option type.
+    """
     max_value: int | None = None
+    """An optional maximum value of the option value.
+
+    Note:
+        Available only for the integer/float option type.
+    """
     min_value: int | None = None
-    """Only for integer/float option"""
+    """An optional minimum value of the option value.
+
+    Note:
+        Available only for the integer/float option type.
+    """
     channel_types: Sequence[ChannelType] = field(default_factory=tuple[ChannelType])
-    """Only for channel option"""
+    """An optional channel types are available for selection.
+
+    Note:
+        Available only for the channel option type.
+    """
```

### Comparing `aurum_hikari-0.1.3/pyproject.toml` & `aurum_hikari-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 
 # Package information
 [tool.poetry]
 packages = [{ include = "aurum" }]
 name = "aurum-hikari"
-version = "v0.1.3"
+version = "v0.1.4"
 license = "MIT"
 authors = ["stefanlight <64615032+stefanlight8@users.noreply.github.com>"]
 description = "A flexible command & component handler"
 keywords = [
     "discord",
     "hikari",
     "commands",
@@ -36,30 +36,39 @@
     "Typing :: Typed",
 ]
 readme = "README.md"
 
 
 [tool.poetry.urls]
 repository = "https://github.com/ShinshiDevs/aurum-hikari"
-documentation = "https://shinshidevs.github.io/aurum-hikari/docs/"
-"Bug Tracker" = "https://github.com/ShinshiDevs/aurum-hikari/issues"
+documentation = "https://shinshidevs.github.io/aurum-hikari/"
+"Issue Tracker" = "https://github.com/ShinshiDevs/aurum-hikari/issues"
 # TODO: Add discord later
 
 
 # Package dependencies
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
-hikari = ">2.0.0.dev120"
+hikari = ">2.0.0.dev122"
+
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = ">=1.5.3,<1.7"
+mkdocstrings-python = ">=1.8.0,<1.11"
+mkdocs-material = { version = "^9.5.23", extras = ["imaging"] }
+griffe-inherited-docstrings = "^1.0.0"
+mkdocs-material-extensions = "^1.3.1"
 
 
 # Developers stuff 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.10.0"
 ruff = "^0.4.3"
 
 # Developers stuff: Ruff settings
+
 [tool.ruff]
 line-length = 100
 target-version = "py310"
 
-[tool.ruff.per-file-ignores] # borrowed from hikari-lightbulb
+[tool.ruff.lint.per-file-ignores] # borrowed from hikari-lightbulb
 "__init__.py" = ["F401", "F403", "F405"]
```

### Comparing `aurum_hikari-0.1.3/PKG-INFO` & `aurum_hikari-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurum-hikari
-Version: 0.1.3
+Version: 0.1.4
 Summary: A flexible command & component handler
 License: MIT
 Keywords: discord,hikari,commands,components,command-handler,component-handler
 Author: stefanlight
 Author-email: 64615032+stefanlight8@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 3 - Alpha
@@ -17,17 +17,17 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: hikari (>2.0.0.dev120)
-Project-URL: Bug Tracker, https://github.com/ShinshiDevs/aurum-hikari/issues
-Project-URL: documentation, https://shinshidevs.github.io/aurum-hikari/docs/
+Requires-Dist: hikari (>2.0.0.dev122)
+Project-URL: Issue Tracker, https://github.com/ShinshiDevs/aurum-hikari/issues
+Project-URL: documentation, https://shinshidevs.github.io/aurum-hikari/
 Project-URL: repository, https://github.com/ShinshiDevs/aurum-hikari
 Description-Content-Type: text/markdown
 
 ![banner](static/banner.png)
 
 <div align="center">
     <h1>Aurum</h1>
@@ -43,15 +43,15 @@
         <a href="https://github.com/ShinshiDevs/aurum-hikari">
             <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/w/ShinshiDevs/aurum-hikari">
             <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues-closed/ShinshiDevs/aurum-hikari">
             <img alt="GitHub License" src="https://img.shields.io/github/license/ShinshiDevs/aurum-hikari">
         </a>
     </p>
     <p>
-        <a href="https://shinshidevs.github.io/aurum-hikari/docs/">Documentation</a>
+        <a href="https://shinshidevs.github.io/aurum-hikari/">Documentation</a>
         ·
         <a href="https://github.com/ShinshiDevs/aurum-hikari/releases">Releases</a>
         ·
         <a href="https://pypi.org/project/aurum-hikari/">PyPI</a>
         ·
         <a href="./LICENSE">License</a>
     </p>
@@ -65,19 +65,16 @@
         <text>
             Our goal is to provide you, as developers, with complete freedom of action and to highlight the benefits of Hikari.
         </text>
     </p>
 </div>
 
 # Installation
-> [!CAUTION]
-> This library is in the planning stage of development, it cannot be installed and used. Thanks!
-
 > [!NOTE]
-> This library requires Python version 3.10 or higher.
+> Aurum requires Python 3.10 or higher.
 
 Run command:
 ```md
 pip install aurum-hikari
 # Or
 python -m pip install aurum-hikari # for unix-type systems
 py -m pip install aurum-hikari # for windows
```

