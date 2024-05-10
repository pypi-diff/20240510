# Comparing `tmp/startrek-1.2.0.tar.gz` & `tmp/startrek-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/startrek-1.2.0.tar", last modified: Tue Apr 23 09:02:34 2024, max compression
+gzip compressed data, was "dist/startrek-2.0.0.tar", last modified: Fri May 10 15:29:42 2024, max compression
```

## Comparing `startrek-1.2.0.tar` & `startrek-2.0.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/
--rw-r--r--   0 moky       (501) staff       (20)      449 2024-04-23 09:02:34.000000 startrek-1.2.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       25 2021-05-06 07:15:56.000000 startrek-1.2.0/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-23 09:02:34.000000 startrek-1.2.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      826 2024-04-23 08:26:41.000000 startrek-1.2.0/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/
--rw-r--r--   0 moky       (501) staff       (20)     2520 2023-01-13 11:45:48.000000 startrek-1.2.0/startrek/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5463 2024-03-06 13:31:40.000000 startrek-1.2.0/startrek/arrival.py
--rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-06 13:32:13.000000 startrek-1.2.0/startrek/departure.py
--rw-r--r--   0 moky       (501) staff       (20)     4960 2024-03-06 13:33:03.000000 startrek-1.2.0/startrek/dock.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/fsm/
--rw-r--r--   0 moky       (501) staff       (20)     2056 2023-01-13 04:48:09.000000 startrek-1.2.0/startrek/fsm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2301 2024-02-26 16:17:15.000000 startrek-1.2.0/startrek/fsm/auto.py
--rw-r--r--   0 moky       (501) staff       (20)     8897 2024-03-06 13:23:59.000000 startrek-1.2.0/startrek/fsm/base.py
--rw-r--r--   0 moky       (501) staff       (20)     5808 2024-03-06 10:33:56.000000 startrek-1.2.0/startrek/fsm/machine.py
--rw-r--r--   0 moky       (501) staff       (20)     5794 2024-04-23 08:23:46.000000 startrek-1.2.0/startrek/fsm/runner.py
--rw-r--r--   0 moky       (501) staff       (20)     4517 2024-04-23 08:26:09.000000 startrek-1.2.0/startrek/fsm/ticker.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/net/
--rw-r--r--   0 moky       (501) staff       (20)     3283 2023-01-13 11:39:06.000000 startrek-1.2.0/startrek/net/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8734 2024-03-13 09:27:10.000000 startrek-1.2.0/startrek/net/channel.py
--rw-r--r--   0 moky       (501) staff       (20)     3366 2024-03-13 09:14:10.000000 startrek-1.2.0/startrek/net/connection.py
--rw-r--r--   0 moky       (501) staff       (20)     3380 2024-03-06 08:44:28.000000 startrek-1.2.0/startrek/net/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     3867 2024-03-06 08:47:09.000000 startrek-1.2.0/startrek/net/hub.py
--rw-r--r--   0 moky       (501) staff       (20)    17022 2024-03-06 16:02:35.000000 startrek-1.2.0/startrek/net/state.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/port/
--rw-r--r--   0 moky       (501) staff       (20)     3722 2024-03-06 09:27:29.000000 startrek-1.2.0/startrek/port/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3100 2024-03-06 14:33:53.000000 startrek-1.2.0/startrek/port/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     4412 2024-03-13 09:17:53.000000 startrek-1.2.0/startrek/port/docker.py
--rw-r--r--   0 moky       (501) staff       (20)     2619 2024-01-26 17:39:19.000000 startrek-1.2.0/startrek/port/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     4127 2024-03-06 09:27:29.000000 startrek-1.2.0/startrek/port/ship.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/socket/
--rw-r--r--   0 moky       (501) staff       (20)     1899 2024-03-06 13:22:07.000000 startrek-1.2.0/startrek/socket/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4358 2024-04-23 08:25:49.000000 startrek-1.2.0/startrek/socket/active_conn.py
--rw-r--r--   0 moky       (501) staff       (20)    10666 2024-03-13 15:37:34.000000 startrek-1.2.0/startrek/socket/base_channel.py
--rw-r--r--   0 moky       (501) staff       (20)    10445 2024-03-13 14:50:15.000000 startrek-1.2.0/startrek/socket/base_conn.py
--rw-r--r--   0 moky       (501) staff       (20)     9754 2024-04-22 17:47:17.000000 startrek-1.2.0/startrek/socket/base_hub.py
--rw-r--r--   0 moky       (501) staff       (20)    10723 2024-03-13 14:50:40.000000 startrek-1.2.0/startrek/stardocker.py
--rw-r--r--   0 moky       (501) staff       (20)    11435 2024-04-22 17:47:32.000000 startrek-1.2.0/startrek/stargate.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/types/
--rw-r--r--   0 moky       (501) staff       (20)     1678 2024-03-06 07:44:45.000000 startrek-1.2.0/startrek/types/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7196 2024-03-06 10:36:46.000000 startrek-1.2.0/startrek/types/mapping.py
--rw-r--r--   0 moky       (501) staff       (20)     3721 2024-03-08 06:09:38.000000 startrek-1.2.0/startrek/types/pair.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      449 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      894 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)        9 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/
+-rw-r--r--   0 moky       (501) staff       (20)      449 2024-05-10 15:29:42.000000 startrek-2.0.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       25 2021-05-06 07:15:56.000000 startrek-2.0.0/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:29:42.000000 startrek-2.0.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      826 2024-05-10 15:28:44.000000 startrek-2.0.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/
+-rw-r--r--   0 moky       (501) staff       (20)     2520 2023-01-13 11:45:48.000000 startrek-2.0.0/startrek/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5463 2024-03-06 13:31:40.000000 startrek-2.0.0/startrek/arrival.py
+-rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-06 13:32:13.000000 startrek-2.0.0/startrek/departure.py
+-rw-r--r--   0 moky       (501) staff       (20)     4960 2024-03-06 13:33:03.000000 startrek-2.0.0/startrek/dock.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/fsm/
+-rw-r--r--   0 moky       (501) staff       (20)     2109 2024-05-09 18:37:27.000000 startrek-2.0.0/startrek/fsm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2349 2024-05-07 05:04:10.000000 startrek-2.0.0/startrek/fsm/auto.py
+-rw-r--r--   0 moky       (501) staff       (20)     8430 2024-05-07 05:02:58.000000 startrek-2.0.0/startrek/fsm/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     3845 2024-05-09 19:32:00.000000 startrek-2.0.0/startrek/fsm/daemon.py
+-rw-r--r--   0 moky       (501) staff       (20)     5880 2024-05-07 04:58:28.000000 startrek-2.0.0/startrek/fsm/machine.py
+-rw-r--r--   0 moky       (501) staff       (20)     4622 2024-05-09 18:45:29.000000 startrek-2.0.0/startrek/fsm/runner.py
+-rw-r--r--   0 moky       (501) staff       (20)     4495 2024-05-09 18:40:20.000000 startrek-2.0.0/startrek/fsm/ticker.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/net/
+-rw-r--r--   0 moky       (501) staff       (20)     3283 2023-01-13 11:39:06.000000 startrek-2.0.0/startrek/net/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9166 2024-05-07 05:08:01.000000 startrek-2.0.0/startrek/net/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)     3384 2024-05-07 05:08:54.000000 startrek-2.0.0/startrek/net/connection.py
+-rw-r--r--   0 moky       (501) staff       (20)     3416 2024-05-07 05:09:27.000000 startrek-2.0.0/startrek/net/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     3881 2024-05-07 15:28:01.000000 startrek-2.0.0/startrek/net/hub.py
+-rw-r--r--   0 moky       (501) staff       (20)    17046 2024-05-07 05:11:00.000000 startrek-2.0.0/startrek/net/state.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/port/
+-rw-r--r--   0 moky       (501) staff       (20)     3722 2024-03-06 09:27:29.000000 startrek-2.0.0/startrek/port/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3130 2024-05-07 05:12:48.000000 startrek-2.0.0/startrek/port/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     4442 2024-05-07 05:13:41.000000 startrek-2.0.0/startrek/port/docker.py
+-rw-r--r--   0 moky       (501) staff       (20)     2643 2024-05-07 05:12:04.000000 startrek-2.0.0/startrek/port/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     4127 2024-03-06 09:27:29.000000 startrek-2.0.0/startrek/port/ship.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/socket/
+-rw-r--r--   0 moky       (501) staff       (20)     1899 2024-03-06 13:22:07.000000 startrek-2.0.0/startrek/socket/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4446 2024-05-09 18:42:32.000000 startrek-2.0.0/startrek/socket/active_conn.py
+-rw-r--r--   0 moky       (501) staff       (20)    11374 2024-05-07 14:40:01.000000 startrek-2.0.0/startrek/socket/base_channel.py
+-rw-r--r--   0 moky       (501) staff       (20)    10668 2024-05-07 05:24:27.000000 startrek-2.0.0/startrek/socket/base_conn.py
+-rw-r--r--   0 moky       (501) staff       (20)    10165 2024-05-09 15:01:12.000000 startrek-2.0.0/startrek/socket/base_hub.py
+-rw-r--r--   0 moky       (501) staff       (20)    10900 2024-05-07 14:34:30.000000 startrek-2.0.0/startrek/stardocker.py
+-rw-r--r--   0 moky       (501) staff       (20)    11681 2024-05-09 15:01:24.000000 startrek-2.0.0/startrek/stargate.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/types/
+-rw-r--r--   0 moky       (501) staff       (20)     1678 2024-03-06 07:44:45.000000 startrek-2.0.0/startrek/types/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7196 2024-03-06 10:36:46.000000 startrek-2.0.0/startrek/types/mapping.py
+-rw-r--r--   0 moky       (501) staff       (20)     3721 2024-03-08 06:09:38.000000 startrek-2.0.0/startrek/types/pair.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      449 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      917 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)        9 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek.egg-info/top_level.txt
```

### Comparing `startrek-1.2.0/setup.py` & `startrek-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~~~~~~~
 
     Interstellar Transport
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '1.2.0'
+__version__ = '2.0.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
```

### Comparing `startrek-1.2.0/startrek/__init__.py` & `startrek-2.0.0/startrek/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.2.0/startrek/arrival.py` & `startrek-2.0.0/startrek/arrival.py`

 * *Files identical despite different names*

### Comparing `startrek-1.2.0/startrek/departure.py` & `startrek-2.0.0/startrek/departure.py`

 * *Files identical despite different names*

### Comparing `startrek-1.2.0/startrek/dock.py` & `startrek-2.0.0/startrek/dock.py`

 * *Files identical despite different names*

### Comparing `startrek-1.2.0/startrek/fsm/__init__.py` & `startrek-2.0.0/startrek/fsm/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,26 +30,28 @@
 
 """
     Finite State Machine
     ~~~~~~~~~~~~~~~~~~~~
 """
 
 from .ticker import Ticker, Metronome, PrimeMetronome, Singleton
-from .runner import Processor, Handler, Runnable, Runner, Daemon
+from .runner import Processor, Handler, Runnable, Runner
+from .daemon import Daemon, DaemonRunner
 from .machine import Context, Transition, State, Machine, Delegate
 from .base import BaseTransition, BaseState, BaseMachine
 from .auto import AutoMachine
 
 name = "FSM"
 
 __author__ = 'Albert Moky'
 
 __all__ = [
 
     'Ticker', 'Metronome', 'PrimeMetronome', 'Singleton',
 
-    'Processor', 'Handler', 'Runnable', 'Runner', 'Daemon',
+    'Processor', 'Handler', 'Runnable', 'Runner',
+    'Daemon', 'DaemonRunner',
 
     'Context', 'Transition', 'State', 'Machine', 'Delegate',
     'BaseTransition', 'BaseState', 'BaseMachine',
     'AutoMachine',
 ]
```

### Comparing `startrek-1.2.0/startrek/fsm/auto.py` & `startrek-2.0.0/startrek/fsm/auto.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,29 +41,29 @@
     # @property  # Override
     # @abstractmethod
     # def context(self) -> C:
     #     """ machine itself """
     #     raise NotImplemented
 
     # Override
-    def start(self):
-        super().start()
+    async def start(self):
+        await super().start()
         timer = PrimeMetronome()
         timer.add_ticker(ticker=self)
 
     # Override
-    def stop(self):
+    async def stop(self):
         timer = PrimeMetronome()
         timer.remove_ticker(ticker=self)
-        super().stop()
+        await super().stop()
 
     # Override
-    def pause(self):
+    async def pause(self):
         timer = PrimeMetronome()
         timer.remove_ticker(ticker=self)
-        super().pause()
+        await super().pause()
 
     # Override
-    def resume(self):
-        super().resume()
+    async def resume(self):
+        await super().resume()
         timer = PrimeMetronome()
         timer.add_ticker(ticker=self)
```

### Comparing `startrek-1.2.0/startrek/fsm/base.py` & `startrek-2.0.0/startrek/fsm/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -47,18 +47,14 @@
         self.__target = target
 
     @property
     def target(self) -> int:
         """ target state index """
         return self.__target
 
-    # @abstractmethod  # Override
-    # def evaluate(self, ctx: C, now: float) -> bool:
-    #     raise NotImplemented
-
 
 # noinspection PyAbstractClass
 class BaseState(State[C, T], ABC):
     """ State with transitions """
 
     def __init__(self, index: int):
         super().__init__()
@@ -76,30 +72,14 @@
     # Override
     def evaluate(self, ctx: C, now: float) -> Optional[T]:
         for trans in self.__transitions:
             if trans.evaluate(ctx, now=now):
                 # OK, get target state from this transition
                 return trans
 
-    # @abstractmethod  # Override
-    # def on_enter(self, old, ctx: C, now: float):
-    #     raise NotImplemented
-    #
-    # @abstractmethod  # Override
-    # def on_exit(self, new, ctx: C, now: float):
-    #     raise NotImplemented
-    #
-    # @abstractmethod  # Override
-    # def on_pause(self, ctx: C):
-    #     raise NotImplemented
-    #
-    # @abstractmethod  # Override
-    # def on_resume(self, ctx: C):
-    #     raise NotImplemented
-
 
 class MachineStatus(IntEnum):
     """ Machine Status """
     STOPPED = 0
     RUNNING = 1
     PAUSED = 2
 
@@ -166,15 +146,15 @@
         if 0 <= index:  # and index < len(self.__states):
             return self.__states[index]
 
     @current_state.setter  # private
     def current_state(self, state: BaseState[C, T]):
         self.__current = -1 if state is None else state.index
 
-    def __change_state(self, state: Optional[State[C, T]], now: float):
+    async def __change_state(self, state: Optional[State[C, T]], now: float):
         """
         Exit current state, and enter new state
 
         :param state:   next state
         :param now:     current time (seconds from Jan 1, 1970 UTC)
         """
         old = self.current_state
@@ -185,99 +165,99 @@
         delegate = self.delegate
         #
         #  Events before state changed
         #
         if delegate is not None:
             # prepare for changing current state to the new one,
             # the delegate can get old state via ctx if need
-            delegate.enter_state(state, machine, now=now)
+            await delegate.enter_state(state, machine, now=now)
         if old is not None:
-            old.on_exit(state, machine, now=now)
+            await old.on_exit(state, machine, now=now)
         #
         #  Change current state
         #
         self.current_state = state
         #
         #  Events after state changed
         #
         if state is not None:
-            state.on_enter(old, machine, now=now)
+            await state.on_enter(old, machine, now=now)
         if delegate is not None:
             # handle after the current state changed,
             # the delegate can get new state via ctx if need
-            delegate.exit_state(old, machine, now=now)
+            await delegate.exit_state(old, machine, now=now)
         return True
 
     #
     #   Actions
     #
 
     # Override
-    def start(self):
+    async def start(self):
         now = time.time()
-        ok = self.__change_state(state=self.default_state, now=now)
+        ok = await self.__change_state(state=self.default_state, now=now)
         assert ok, 'failed to change default state'
         self.__status = MachineStatus.RUNNING
 
     # Override
-    def stop(self):
+    async def stop(self):
         self.__status = MachineStatus.STOPPED
         now = time.time()
-        self.__change_state(state=None, now=now)  # force current state to None
+        await self.__change_state(state=None, now=now)  # force current state to None
 
     # Override
-    def pause(self):
+    async def pause(self):
         now = time.time()
         machine = self.context
         current = self.current_state
         #
         #  Events before state paused
         #
         if current is not None:
-            current.on_pause(machine, now=now)
+            await current.on_pause(machine, now=now)
         #
         #  Pause state
         #
         self.__status = MachineStatus.PAUSED
         #
         #  Events after state paused
         #
         delegate = self.delegate
         if delegate is not None:
-            delegate.pause_state(current, machine, now=now)
+            await delegate.pause_state(current, machine, now=now)
 
     # Override
-    def resume(self):
+    async def resume(self):
         now = time.time()
         machine = self.context
         current = self.current_state
         #
         #  Events before state resumed
         #
         delegate = self.delegate
         if delegate is not None:
-            delegate.resume_state(current, machine, now=now)
+            await delegate.resume_state(current, machine, now=now)
         #
         #  Resume state
         #
         self.__status = MachineStatus.RUNNING
         #
         #  Events after state resumed
         #
         if current is not None:
-            current.on_resume(machine, now=now)
+            await current.on_resume(machine, now=now)
 
     #
     #   Ticker
     #
 
     # Override
-    def tick(self, now: float, elapsed: float):
+    async def tick(self, now: float, elapsed: float):
         machine = self.context
         current = self.current_state
         if current is not None and self.__status == MachineStatus.RUNNING:
             trans = current.evaluate(machine, now=now)
             if trans is not None:
                 # assert isinstance(trans, BaseTransition), 'transition error: %s' % trans
                 target = self.get_target_state(transition=trans)
                 assert target is not None, 'target state error: %s' % trans.target
-                self.__change_state(state=target, now=now)
+                await self.__change_state(state=target, now=now)
```

### Comparing `startrek-1.2.0/startrek/fsm/machine.py` & `startrek-2.0.0/startrek/fsm/machine.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,107 +59,107 @@
         raise NotImplemented
 
 
 class State(ABC, Generic[C, T]):
     """ Finite State """
 
     @abstractmethod
-    def on_enter(self, old, ctx: C, now: float):
+    def evaluate(self, ctx: C, now: float) -> Optional[T]:
         """
-        Called after new state entered
+        Called by machine.tick() to evaluate each transitions
 
-        :param old:     previous state
         :param ctx:     context (machine)
         :param now:     current time (seconds from Jan 1, 1970 UTC)
+        :return success transition, or None to stay the current state
         """
         raise NotImplemented
 
     @abstractmethod
-    def on_exit(self, new, ctx: C, now: float):
+    async def on_enter(self, old, ctx: C, now: float):
         """
-        Called before old state exited
+        Called after new state entered
 
-        :param new:     next state
+        :param old:     previous state
         :param ctx:     context (machine)
         :param now:     current time (seconds from Jan 1, 1970 UTC)
         """
         raise NotImplemented
 
     @abstractmethod
-    def on_pause(self, ctx: C, now: float):
+    async def on_exit(self, new, ctx: C, now: float):
         """
-        Called before current state paused
+        Called before old state exited
 
+        :param new:     next state
         :param ctx:     context (machine)
         :param now:     current time (seconds from Jan 1, 1970 UTC)
         """
         raise NotImplemented
 
     @abstractmethod
-    def on_resume(self, ctx: C, now: float):
+    async def on_pause(self, ctx: C, now: float):
         """
-        Called after current state resumed
+        Called before current state paused
 
         :param ctx:     context (machine)
         :param now:     current time (seconds from Jan 1, 1970 UTC)
         """
         raise NotImplemented
 
     @abstractmethod
-    def evaluate(self, ctx: C, now: float) -> Optional[T]:
+    async def on_resume(self, ctx: C, now: float):
         """
-        Called by machine.tick() to evaluate each transitions
+        Called after current state resumed
 
         :param ctx:     context (machine)
         :param now:     current time (seconds from Jan 1, 1970 UTC)
-        :return success transition, or None to stay the current state
         """
         raise NotImplemented
 
 
 class Delegate(ABC, Generic[C, T, S]):
     """ State Machine Delegate """
 
     @abstractmethod
-    def enter_state(self, state: Optional[S], ctx: C, now: float):
+    async def enter_state(self, state: Optional[S], ctx: C, now: float):
         """
         Called before enter new state
         (get current state from context)
 
         :param state:   new state
         :param ctx:     context (machine)
         :param now:     current time (seconds from Jan 1, 1970 UTC)
         """
         raise NotImplemented
 
     @abstractmethod
-    def exit_state(self, state: Optional[S], ctx: C, now: float):
+    async def exit_state(self, state: Optional[S], ctx: C, now: float):
         """
         Called after exit old state
         (get current state from context)
 
         :param state:   old state
         :param ctx:     context (machine)
         :param now:     current time (seconds from Jan 1, 1970 UTC)
         """
         raise NotImplemented
 
     @abstractmethod
-    def pause_state(self, state: Optional[S], ctx: C, now: float):
+    async def pause_state(self, state: Optional[S], ctx: C, now: float):
         """
         Called after pause this state
 
         :param state:   current state
         :param ctx:     context (machine)
         :param now:     current time (seconds from Jan 1, 1970 UTC)
         """
         raise NotImplemented
 
     @abstractmethod
-    def resume_state(self, state: Optional[S], ctx: C, now: float):
+    async def resume_state(self, state: Optional[S], ctx: C, now: float):
         """
         Called before resume this state
 
         :param state:   current state
         :param ctx:     context (machine)
         :param now:     current time (seconds from Jan 1, 1970 UTC)
         """
@@ -171,25 +171,25 @@
 
     @property
     @abstractmethod
     def current_state(self) -> Optional[S]:
         raise NotImplemented
 
     @abstractmethod
-    def start(self):
+    async def start(self):
         """ Change current state to 'default' """
         raise NotImplemented
 
     @abstractmethod
-    def stop(self):
+    async def stop(self):
         """ Change current state to null """
         raise NotImplemented
 
     @abstractmethod
-    def pause(self):
+    async def pause(self):
         """ Pause machine, current state not change """
         raise NotImplemented
 
     @abstractmethod
-    def resume(self):
+    async def resume(self):
         """ Resume machine with current state """
         raise NotImplemented
```

### Comparing `startrek-1.2.0/startrek/fsm/runner.py` & `startrek-2.0.0/startrek/fsm/runner.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,65 +24,65 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-import time
-import weakref
+import asyncio
 from abc import ABC, abstractmethod
-from threading import Thread
-from typing import Optional
 
 
 class Processor(ABC):
 
     @abstractmethod
-    def process(self) -> bool:
+    async def process(self) -> bool:
         """
         Do the job
 
         :return: False on nothing to do
         """
         raise NotImplemented
 
 
 class Handler(ABC):
 
     @abstractmethod
-    def setup(self):
+    async def setup(self):
         """ Prepare for Handling """
         raise NotImplemented
     
     @abstractmethod
-    def handle(self):
+    async def handle(self):
         """ Handling run loop """
         raise NotImplemented
 
     @abstractmethod
-    def finish(self):
+    async def finish(self):
         """ Cleanup after handled """
         raise NotImplemented
 
 
 class Runnable(ABC):
 
     @abstractmethod
-    def run(self):
-        """ Run in a thread """
+    async def run(self):
+        """ Run in an async task """
         raise NotImplemented
 
 
+# noinspection PyAbstractClass
 class Runner(Runnable, Handler, Processor, ABC):
     """
         Runner
         ~~~~~~
 
-        @abstract method:
+        @abstract methods:
+            - setup()
+            - finish()
             - process()
     """
 
     # Frames Per Second
     # ~~~~~~~~~~~~~~~~~
     # (1) The human eye can process 10-12 still images per second,
     #     and the dynamic compensation function can also deceive us.
@@ -107,101 +107,50 @@
     def interval(self) -> float:
         return self.__interval
 
     @property
     def running(self) -> bool:
         return self.__running
 
-    def stop(self):
+    async def start(self):
+        self.__running = True
+
+    async def stop(self):
         self.__running = False
 
     # Override
-    def run(self):
-        self.setup()
+    async def run(self):
+        await self.setup()
         try:
-            self.handle()
+            await self.handle()
         finally:
-            self.finish()
-
-    # Override
-    def setup(self):
-        self.__running = True
+            await self.finish()
 
     # Override
-    def handle(self):
+    async def handle(self):
         while self.running:
-            if not self.process():
+            if await self.process():
+                # runner is busy, return True to go on.
+                pass
+            else:
                 # if nothing to do now, return False here
                 # to let the thread have a rest.
-                self._idle()
-
-    # Override
-    def finish(self):
-        self.__running = False
-
-    def _idle(self):
-        time.sleep(self.interval)
-
-    @abstractmethod
-    def process(self) -> bool:
-        raise NotImplemented
-
+                await self._idle()
 
-class Daemon:
-    """
-        Daemon Thread
-        ~~~~~~~~~~~~~
-        The main thread won't wait the daemon threads exit
-        when daemonic = True
-    """
+    # protected
+    async def _idle(self):
+        await self.sleep(seconds=self.interval)
+        # time.sleep(self.interval)
 
-    def __init__(self, target: Runnable, daemonic: bool = True):
-        super().__init__()
-        self.__target = weakref.ref(target)  # Callable
-        self.__daemon = daemonic
-        self.__thread: Optional[Thread] = None
-
-    @property  # private
-    def target(self) -> Optional[Runnable]:
-        ref = self.__target
-        if ref is not None:
-            return ref()
+    @classmethod
+    async def sleep(cls, seconds: float):
+        await asyncio.sleep(seconds)
 
-    @property
-    def alive(self) -> bool:
-        thr = self.__thread
-        if thr is not None:
-            return thr.is_alive()
-
-    def start(self):
-        self.__force_stop()
-        target = self.target
-        if target is not None:
-            thr = Thread(target=target.run, daemon=self.__daemon)
-            thr.start()
-            self.__thread = thr
-
-    def stop(self):
-        self.__force_stop()
-
-    def __del__(self):
-        self.__force_stop()
-
-    def __force_stop(self):
-        thr = self.__thread
-        if thr is not None:
-            self.__thread = None
-            self._join(thr=thr)
-
-    def _join(self, thr: Thread):
-        # Waits at most seconds for this thread to die.
-        # A timeout of 0 means to wait forever.
-        self.join(thr=thr, timeout=1.0)
+    @classmethod
+    def sync_run(cls, main):
+        """ Run main coroutine until complete """
+        asyncio.run(main)
 
     @classmethod
-    def join(cls, thr: Thread, timeout: float = None):
-        try:
-            if thr.is_alive():
-                thr.join(timeout=timeout)
-        except RuntimeError as error:
-            print('[ERROR] failed to join thread: %s, timeout: %d' % (error, timeout))
-            # traceback.print_exc()
+    def async_run(cls, coroutine) -> asyncio.Task:
+        """ Create an async task to run the coroutine """
+        return asyncio.create_task(coroutine)
```

### Comparing `startrek-1.2.0/startrek/fsm/ticker.py` & `startrek-2.0.0/startrek/fsm/ticker.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,95 +31,88 @@
 import threading
 import time
 import traceback
 from weakref import WeakSet
 from abc import ABC, abstractmethod
 from typing import Set
 
-from .runner import Runner, Daemon
+from .runner import Runner
+from .daemon import DaemonRunner
 
 
 class Ticker(ABC):
 
     @abstractmethod
-    def tick(self, now: float, elapsed: float):
+    async def tick(self, now: float, elapsed: float):
         """
         Drive current thread forward
 
         :param now:     current time (seconds from Jan 1, 1970 UTC)
         :param elapsed: seconds from previous tick
         """
         raise NotImplemented
 
 
-class Metronome(Runner):
+class Metronome(DaemonRunner):
 
     # at least wait 1/60 of a second
     MIN_INTERVAL = 1.0/60
 
     def __init__(self, interval: float):
         super().__init__(interval=interval)
         self.__last_time = 0
-        self.__daemon = Daemon(target=self)
         self.__lock = threading.Lock()
         self.__tickers = WeakSet()
 
     # Override
-    def setup(self):
-        super().setup()
+    async def setup(self):
+        await super().setup()
         self.__last_time = time.time()
 
     # Override
-    def process(self) -> bool:
+    async def process(self) -> bool:
         tickers = self.tickers
         if len(tickers) == 0:
             # nothing to do now,
             # return False to have a rest ^_^
             return False
         # 1. check time
         now = time.time()
         elapsed = now - self.__last_time
         waiting = self.interval - elapsed
         if waiting < self.MIN_INTERVAL:
             waiting = self.MIN_INTERVAL
-        time.sleep(waiting)
+        await self.sleep(seconds=waiting)
         now += waiting
         elapsed += waiting
         # 2. drive tickers
         for item in tickers:
             try:
-                item.tick(now=now, elapsed=elapsed)
+                await item.tick(now=now, elapsed=elapsed)
             except Exception as error:
                 print('[Metronome] drive ticker error: %s, %s' % (error, item))
                 traceback.print_exc()
         # 3. update last time
         self.__last_time = now
         return True
 
     @property  # private
     def tickers(self) -> Set[Ticker]:
+        """ get all tickers """
         with self.__lock:
             return set(self.__tickers)
 
     def add_ticker(self, ticker: Ticker):
         with self.__lock:
             self.__tickers.add(ticker)
 
     def remove_ticker(self, ticker: Ticker):
         with self.__lock:
             self.__tickers.discard(ticker)
 
-    def start(self):
-        self.__daemon.start()
-
-    # Override
-    def stop(self):
-        super().stop()
-        self.__daemon.stop()
-
 
 #
 #   Singleton for Prime Metronome
 #
 
 
 class Singleton(object):
@@ -141,16 +134,17 @@
         return getattr(self.__cls, key, None)
 
 
 @Singleton
 class PrimeMetronome:
 
     def __init__(self):
+        super().__init__()
         metronome = Metronome(interval=Runner.INTERVAL_SLOW)
-        metronome.start()
+        Runner.async_run(coroutine=metronome.start())
         self.__metronome = metronome
 
     def add_ticker(self, ticker: Ticker):
         self.__metronome.add_ticker(ticker=ticker)
 
     def remove_ticker(self, ticker: Ticker):
         self.__metronome.remove_ticker(ticker=ticker)
```

### Comparing `startrek-1.2.0/startrek/net/__init__.py` & `startrek-2.0.0/startrek/net/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.2.0/startrek/net/channel.py` & `startrek-2.0.0/startrek/net/channel.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,23 +27,38 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 import socket
 import traceback
 from abc import ABC, abstractmethod
+from enum import IntEnum
 from typing import Optional, Tuple
 
 from ..types import SocketAddress
 
 
+# protected
+class ChannelState(IntEnum):
+    """ Channel State Order """
+    INIT = 0    # initializing
+    OPEN = 1    # initialized
+    ALIVE = 2   # (not closed) and (connected or bound)
+    CLOSED = 3  # closed
+
+
 class Channel(ABC):
 
     @property
     @abstractmethod
+    def state(self) -> ChannelState:
+        raise NotImplemented
+
+    @property
+    @abstractmethod
     def closed(self) -> bool:
         """ not is_open() """
         raise NotImplemented
 
     @property
     @abstractmethod
     def bound(self) -> bool:
@@ -65,36 +80,36 @@
     @property
     @abstractmethod
     def vacant(self) -> bool:
         """ ready for writing """
         raise NotImplemented
 
     @abstractmethod
-    def close(self):
+    async def close(self):
         """ Close the channel """
         raise NotImplemented
 
     #
     #   Byte Channel
     #
 
     @abstractmethod
-    def read(self, max_len: int) -> Optional[bytes]:
+    async def read(self, max_len: int) -> Optional[bytes]:
         """
         Reads a sequence of bytes from this channel into the given buffer.
 
         :param max_len: max buffer length
         :return: The number of bytes read, possibly zero,
                  or -1 if the channel has reached end-of-stream
         :raise: socket.error
         """
         raise NotImplemented
 
     @abstractmethod
-    def write(self, data: bytes) -> int:
+    async def write(self, data: bytes) -> int:
         """
         Writes a sequence of bytes to this channel from the given buffer.
 
         :param data: outgo data
         :return: The number of bytes written, possibly zero
         :raise: socket.error
         """
@@ -122,16 +137,16 @@
         raise NotImplemented
 
     #
     #   Network Channel
     #
 
     @abstractmethod
-    def bind(self, address: Optional[SocketAddress] = None,
-             host: Optional[str] = '0.0.0.0', port: Optional[int] = 0):
+    async def bind(self, address: Optional[SocketAddress] = None,
+                   host: Optional[str] = '0.0.0.0', port: Optional[int] = 0):
         """
         Binds the channel's socket to a local address (host, port).
 
         :param address: local address
         :param host:    local host
         :param port:    local port
         :return: bound socket
@@ -157,16 +172,16 @@
     @property
     @abstractmethod
     def connected(self) -> bool:
         """ is_connected() """
         raise NotImplemented
 
     @abstractmethod
-    def connect(self, address: Optional[SocketAddress] = None,
-                host: Optional[str] = '127.0.0.1', port: Optional[int] = 0) -> socket.socket:
+    async def connect(self, address: Optional[SocketAddress] = None,
+                      host: Optional[str] = '127.0.0.1', port: Optional[int] = 0) -> socket.socket:
         """
         Connects this channel's socket.
 
         :param address: remote address
         :param host:    remote host
         :param port:    remote port
         :return: connected socket
@@ -185,36 +200,36 @@
         raise NotImplemented
 
     #
     #   Datagram Channel
     #
 
     @abstractmethod
-    def disconnect(self) -> Optional[socket.socket]:
+    async def disconnect(self) -> Optional[socket.socket]:
         """
         Disconnects this channel's socket.
 
         :return: inner socket
         :raise: socket.error
         """
         raise NotImplemented
 
     @abstractmethod
-    def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
+    async def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
         """
         Receives a data package via this channel.
 
         :param max_len: max buffer length
         :return: received data and remote address
         :raise: socket.error
         """
         raise NotImplemented
 
     @abstractmethod
-    def send(self, data: bytes, target: SocketAddress) -> int:
+    async def send(self, data: bytes, target: SocketAddress) -> int:
         """
         Sends a data package via this channel.
 
         :param data:   outgo data package
         :param target: remote address
         :return: The number of bytes sent, which will be either the number
                  of bytes that were remaining in the source buffer when this
@@ -258,42 +273,42 @@
     return get_local_address(sock=sock) is not None
 
 
 def is_closed(sock: socket.socket) -> bool:
     return getattr(sock, '_closed', False)
 
 
-def bind_socket(sock: socket.socket, local: SocketAddress) -> bool:
+async def bind_socket(sock: socket.socket, local: SocketAddress) -> bool:
     """ Bind to local address """
     try:
         sock.bind(local)
         return is_bound(sock=sock)
     except socket.error as error:
         print('[Socket] cannot bind to: %s, socket: %s, %s' % (local, sock, error))
         traceback.print_exc()
         return False
 
 
-def connect_socket(sock: socket.socket, remote: SocketAddress) -> bool:
+async def connect_socket(sock: socket.socket, remote: SocketAddress) -> bool:
     """ Connect to remote address """
     try:
         sock.connect(remote)
-        return is_bound(sock=sock)
+        return is_connected(sock=sock)
     except socket.error as error:
         print('[Socket] cannot connect to: %s, socket: %s, %s' % (remote, sock, error))
         traceback.print_exc()
         return False
 
 
-def disconnect_socket(sock: socket.socket) -> bool:
+async def disconnect_socket(sock: socket.socket) -> bool:
     """ Close socket """
     if is_closed(sock=sock) or not is_connected(sock=sock):
         return True
     try:
         # TODO: check for UDP socket
         # sock.shutdown(socket.SHUT_RDWR)
         sock.close()
-        return is_closed(sock=sock)
+        return not is_connected(sock=sock)
     except socket.error as error:
         print('[Socket] cannot close socket: %s, %s' % (sock, error))
         traceback.print_exc()
         return False
```

### Comparing `startrek-1.2.0/startrek/net/connection.py` & `startrek-2.0.0/startrek/net/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,29 +90,29 @@
     @property
     @abstractmethod
     def state(self):  # -> Optional[ConnectionState]:
         """ Get connection state """
         raise NotImplemented
 
     @abstractmethod
-    def send(self, data: bytes) -> int:
+    async def send(self, data: bytes) -> int:
         """
         Send data
 
         :param data: outgo data package
         :return: count of bytes sent, probably zero when it's non-blocking mode
         """
         raise NotImplemented
 
     @abstractmethod
-    def received(self, data: bytes):
+    async def received(self, data: bytes):
         """
         Call on received data for processing
 
         :param data: received data
         """
         raise NotImplemented
 
     @abstractmethod
-    def close(self):
+    async def close(self):
         """ Close the connection """
         raise NotImplemented
```

### Comparing `startrek-1.2.0/startrek/net/delegate.py` & `startrek-2.0.0/startrek/net/delegate.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,59 +36,59 @@
 from .state import ConnectionState
 
 
 class ConnectionDelegate(ABC):
     """ Connection Delegate """
 
     @abstractmethod
-    def connection_state_changed(self, previous: Optional[ConnectionState], current: Optional[ConnectionState],
-                                 connection: Connection):
+    async def connection_state_changed(self, previous: Optional[ConnectionState], current: Optional[ConnectionState],
+                                       connection: Connection):
         """
         Called when connection status is changed
 
         :param previous:   old state
         :param current:    new state
         :param connection: current connection
         """
         raise NotImplemented
 
     @abstractmethod
-    def connection_received(self, data: bytes, connection: Connection):
+    async def connection_received(self, data: bytes, connection: Connection):
         """
         Called when connection received data
 
         :param data:        received data package
         :param connection:  current connection
         """
         raise NotImplemented
 
     @abstractmethod
-    def connection_sent(self, sent: int, data: bytes, connection: Connection):
+    async def connection_sent(self, sent: int, data: bytes, connection: Connection):
         """
         Called after data sent via the connection
 
         :param sent:        length of sent bytes
         :param data:        sent data package
         :param connection:  current connection
         """
         raise NotImplemented
 
     @abstractmethod
-    def connection_failed(self, error: Union[IOError, socket.error], data: bytes, connection: Connection):
+    async def connection_failed(self, error: Union[IOError, socket.error], data: bytes, connection: Connection):
         """
         Called when failed to send data via the connection
 
         :param error:       connection error
         :param data:        outgoing data package
         :param connection:  current connection
         """
         raise NotImplemented
 
     @abstractmethod
-    def connection_error(self, error: Union[IOError, socket.error], connection: Connection):
+    async def connection_error(self, error: Union[IOError, socket.error], connection: Connection):
         """
         Called when connection (receiving) error
 
         :param error:       connection error
         :param connection:  current connection
         """
         raise NotImplemented
```

### Comparing `startrek-1.2.0/startrek/net/hub.py` & `startrek-2.0.0/startrek/net/hub.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,35 +31,35 @@
 import socket
 from abc import ABC, abstractmethod
 from typing import Optional, Iterable
 
 from ..types import SocketAddress
 from ..fsm import Processor
 
-from .channel import disconnect_socket
+from .channel import is_closed
 from .channel import Channel
 from .connection import Connection
 
 
 class Hub(Processor, ABC):
     """ Connections & Channels Container """
 
     @abstractmethod
-    def open(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
+    async def open(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
         """
         Open a channel with direction (remote, local)
 
         :param remote: remote address to connected
         :param local:  local address to bound
         :return: None on socket error
         """
         raise NotImplemented
 
     @abstractmethod
-    def connect(self, remote: SocketAddress, local: Optional[SocketAddress] = None) -> Optional[Connection]:
+    async def connect(self, remote: SocketAddress, local: Optional[SocketAddress] = None) -> Optional[Connection]:
         """
         Get connection with direction (remote, local)
 
         :param remote: remote address
         :param local:  local address
         :return: None on channel closed
         """
@@ -104,10 +104,10 @@
         sock = None
         try:
             sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             remote = ('8.8.8.8', 8888)
             sock.connect(remote)
             ip = sock.getsockname()[0]
         finally:
-            if sock is not None:
-                disconnect_socket(sock=sock)
+            if not (sock is None or is_closed(sock=sock)):
+                sock.close()
         return ip
```

### Comparing `startrek-1.2.0/startrek/net/state.py` & `startrek-2.0.0/startrek/net/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,27 +178,27 @@
             return self.index != other
         elif isinstance(other, str):
             return self.__name != other
         else:
             return True
 
     # Override
-    def on_enter(self, old, ctx: StateMachine, now: float):
+    async def on_enter(self, old, ctx: StateMachine, now: float):
         self.__time = now
 
     # Override
-    def on_exit(self, new, ctx: StateMachine, now: float):
+    async def on_exit(self, new, ctx: StateMachine, now: float):
         self.__time = 0
 
     # Override
-    def on_pause(self, ctx: StateMachine, now: float):
+    async def on_pause(self, ctx: StateMachine, now: float):
         pass
 
     # Override
-    def on_resume(self, ctx: StateMachine, now: float):
+    async def on_resume(self, ctx: StateMachine, now: float):
         pass
 
 
 class TimedConnection(ABC):
 
     @property
     @abstractmethod
```

### Comparing `startrek-1.2.0/startrek/port/__init__.py` & `startrek-2.0.0/startrek/port/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.2.0/startrek/port/delegate.py` & `startrek-2.0.0/startrek/port/delegate.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,57 +33,57 @@
 from .ship import Arrival, Departure
 from .docker import Docker, DockerStatus
 
 
 class DockerDelegate(ABC):
 
     @abstractmethod
-    def docker_received(self, ship: Arrival, docker: Docker):
+    async def docker_received(self, ship: Arrival, docker: Docker):
         """
         Callback when new package received
 
         :param ship:    income data package container
         :param docker:  connection docker
         """
         raise NotImplemented
 
     @abstractmethod
-    def docker_sent(self, ship: Departure, docker: Docker):
+    async def docker_sent(self, ship: Departure, docker: Docker):
         """
         Callback when package sent
 
         :param ship:    outgo data package container
         :param docker:  connection connection
         """
         raise NotImplemented
 
     @abstractmethod
-    def docker_failed(self, error: OSError, ship: Departure, docker: Docker):
+    async def docker_failed(self, error: OSError, ship: Departure, docker: Docker):
         """
         Callback when failed to send package
 
         :param error:   error message
         :param ship:    outgo data package container
         :param docker:  connection docker
         """
         raise NotImplemented
 
     @abstractmethod
-    def docker_error(self, error: OSError, ship: Departure, docker: Docker):
+    async def docker_error(self, error: OSError, ship: Departure, docker: Docker):
         """
         Callback when connection error
 
         :param error:   error message
         :param ship:    outgo data package container
         :param docker:  connection docker
         """
         raise NotImplemented
 
     @abstractmethod
-    def docker_status_changed(self, previous: DockerStatus, current: DockerStatus, docker: Docker):
+    async def docker_status_changed(self, previous: DockerStatus, current: DockerStatus, docker: Docker):
         """
         Callback when connection status changed
 
         :param previous: old status
         :param current:  new status
         :param docker:   connection docker
         """
```

### Comparing `startrek-1.2.0/startrek/port/docker.py` & `startrek-2.0.0/startrek/port/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,53 +104,53 @@
     @property
     @abstractmethod
     def local_address(self) -> Optional[SocketAddress]:
         """ Local address of connection """
         raise NotImplemented
 
     @abstractmethod
-    def send_data(self, payload: Union[bytes, bytearray]) -> bool:
+    async def send_data(self, payload: Union[bytes, bytearray]) -> bool:
         """
         Pack data to an outgo ship (with normal priority), and
         append to the waiting queue for sending out
 
         :param payload: data to be sent
         :return: False on error
         """
         raise NotImplemented
 
     @abstractmethod
-    def send_ship(self, ship: Departure) -> bool:
+    async def send_ship(self, ship: Departure) -> bool:
         """
         Append outgo ship (carrying data package, with priority)
         to the waiting queue for sending out
 
         :param ship: outgo ship carrying data package/fragment
         :return: False on duplicated
         """
         raise NotImplemented
 
     @abstractmethod
-    def process_received(self, data: bytes):
+    async def process_received(self, data: bytes):
         """
         Called when received data
 
         :param data: received data package
         """
         raise NotImplemented
 
     @abstractmethod
-    def heartbeat(self):
+    async def heartbeat(self):
         """
         Send 'PING' for keeping connection alive
         """
         raise NotImplemented
 
     @abstractmethod
     def purge(self, now: float) -> int:
         """ Clear all expired tasks """
         raise NotImplemented
 
     @abstractmethod
-    def close(self):
+    async def close(self):
         """ Close connection for this docker """
         raise NotImplemented
```

### Comparing `startrek-1.2.0/startrek/port/gate.py` & `startrek-2.0.0/startrek/port/gate.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,30 +40,30 @@
 class Gate(Processor, ABC):
     """
         Star Gate
         ~~~~~~~~~
     """
 
     @abstractmethod
-    def send_data(self, payload: Union[bytes, bytearray],
-                  remote: SocketAddress, local: Optional[SocketAddress]) -> bool:
+    async def send_data(self, payload: Union[bytes, bytearray],
+                        remote: SocketAddress, local: Optional[SocketAddress]) -> bool:
         """
         Pack data to an outgo ship (with normal priority), and
         append to the waiting queue of docker for remote address
 
         :param payload: data to be sent
         :param remote: remote address
         :param local:  local address
         :return: False on error
         """
         raise NotImplemented
 
     @abstractmethod
-    def send_ship(self, ship: Departure,
-                  remote: SocketAddress, local: Optional[SocketAddress]) -> bool:
+    async def send_ship(self, ship: Departure,
+                        remote: SocketAddress, local: Optional[SocketAddress]) -> bool:
         """
         Append outgo ship (carrying data package, with priority)
         to the waiting queue of docker for remote address
 
         :param ship:   departure ship
         :param remote: remote address
         :param local:  local address
```

### Comparing `startrek-1.2.0/startrek/port/ship.py` & `startrek-2.0.0/startrek/port/ship.py`

 * *Files identical despite different names*

### Comparing `startrek-1.2.0/startrek/socket/__init__.py` & `startrek-2.0.0/startrek/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.2.0/startrek/socket/active_conn.py` & `startrek-2.0.0/startrek/socket/active_conn.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,53 +29,54 @@
 # ==============================================================================
 
 import time
 import weakref
 from typing import Optional
 
 from ..types import SocketAddress
-from ..fsm import Daemon, Runnable
+from ..fsm import Runnable, Runner, Daemon
 from ..net import Hub
 
 from .base_conn import BaseConnection
 
 
 class ActiveConnection(BaseConnection, Runnable):
     """ Active connection for client """
 
     def __init__(self, remote: SocketAddress, local: Optional[SocketAddress]):
         super().__init__(remote=remote, local=local)
         self.__hub_ref = None
         self.__daemon = Daemon(target=self)
 
-    @property
+    @property  # protected
     def hub(self) -> Optional[Hub]:
         ref = self.__hub_ref
         if ref is not None:
             return ref()
 
     @property  # Override
     def closed(self) -> bool:
         return self.fsm is None
 
     # Override
-    def start(self, hub: Hub):
+    async def start(self, hub: Hub):
         self.__hub_ref = weakref.ref(hub)
         # 1. start state machine
-        self._start_machine()
-        # 2. start a background thread to check channel
+        await self._start_machine()
+        # 2. start an async task to check channel
         self.__daemon.start()
+        # await self.run()
 
     # Override
-    def run(self):
+    async def run(self):
         expired = 0
         last_time = 0
         interval = 8
         while not self.closed:
-            time.sleep(1.0)
+            await Runner.sleep(seconds=1.0)
             now = time.time()
             try:
                 sock = self.channel
                 if sock is None or sock.closed:
                     # first time to try connecting (last_time == 0)?
                     # or connection lost, then try to reconnect again.
                     # check time interval for the trying here
@@ -89,22 +90,22 @@
                     assert hub is not None, 'hub not found: %s -> %s' % (self.local_address, self.remote_address)
                     # try to open a new socket channel from the hub.
                     # the returned socket channel is opened for connecting,
                     # but maybe failed,
                     # so set an expired time to close it after timeout;
                     # if failed to open a new socket channel,
                     # then extend the time interval for next trying.
-                    sock = self._open_channel(hub=hub)
+                    sock = await self._open_channel(hub=hub)
                     if sock is not None:
                         # connect timeout after 2 minutes
                         expired = now + 128
                     elif interval < 128:
                         interval *= 2
                 elif sock.alive:
                     # socket channel is normal, reset the time interval here.
                     # this will work when the current connection lost
                     interval = 8
                 elif 0 < expired < now:
                     # connect timeout
-                    sock.close()
+                    await sock.close()
             except Exception as error:
                 print('[Socket] active connection error: %s' % error)
```

### Comparing `startrek-1.2.0/startrek/socket/base_channel.py` & `startrek-2.0.0/startrek/socket/base_channel.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,39 +34,40 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Tuple
 
 from ..types import SocketAddress, AddressPairObject
 
 from ..net.channel import is_blocking, is_closed, is_connected, is_bound
 from ..net.channel import bind_socket, connect_socket, disconnect_socket
+from ..net.channel import ChannelState
 from ..net import Channel
 
 
 class SocketReader(ABC):
 
     @abstractmethod
-    def read(self, max_len: int) -> Optional[bytes]:
+    async def read(self, max_len: int) -> Optional[bytes]:
         """ read data from socket """
         raise NotImplemented
 
     @abstractmethod
-    def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
+    async def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
         """ receive data via socket, and return it with remote address """
         raise NotImplemented
 
 
 class SocketWriter(ABC):
 
     @abstractmethod
-    def write(self, data: bytes) -> int:
+    async def write(self, data: bytes) -> int:
         """ write data into socket """
         raise NotImplemented
 
     @abstractmethod
-    def send(self, data: bytes, target: SocketAddress) -> int:
+    async def send(self, data: bytes, target: SocketAddress) -> int:
         """ send data via socket with remote address """
         raise NotImplemented
 
 
 class Controller:
     """ Socket Channel Controller """
 
@@ -97,43 +98,43 @@
             return channel.sock
 
 
 # noinspection PyAbstractClass
 class ChannelReader(Controller, SocketReader, ABC):
 
     # Override
-    def read(self, max_len: int) -> Optional[bytes]:
+    async def read(self, max_len: int) -> Optional[bytes]:
         sock = self.sock
         if sock is None or is_closed(sock=sock):
             raise ConnectionError('socket closed')
         else:
             return sock.recv(max_len)
 
     # @abstractmethod  # Override
-    # def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
+    # async def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
     #     """ receive data via socket, and return it with remote address """
     #     raise NotImplemented
 
 
 # noinspection PyAbstractClass
 class ChannelWriter(Controller, SocketWriter, ABC):
 
     # Override
-    def write(self, data: bytes) -> int:
+    async def write(self, data: bytes) -> int:
         """ Return the number of bytes sent;
             this may be less than len(data) if the network is busy. """
         # sent = sock.sendall(data)
         sock = self.sock
         if sock is None or is_closed(sock=sock):
             raise ConnectionError('socket closed')
         else:
             return sock.send(data)
 
     # @abstractmethod  # Override
-    # def send(self, data: bytes, target: SocketAddress) -> int:
+    # async def send(self, data: bytes, target: SocketAddress) -> int:
     #     """ send data via socket with remote address """
     #     raise NotImplemented
 
 
 class BaseChannel(AddressPairObject, Channel, ABC):
 
     def __init__(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]):
@@ -172,32 +173,48 @@
     #
 
     @property
     def sock(self) -> Optional[socket.socket]:
         """ inner socket """
         return self.__sock
 
-    def set_socket(self, sock: Optional[socket.socket]):
+    async def set_socket(self, sock: Optional[socket.socket]):
         """ set inner socket for this channel """
         # 1. replace with new socket
         old = self.__sock
         if sock is not None:
             self.__sock = sock
             self.__closed = False
         else:
             self.__sock = None
             self.__closed = True
         # 2. close old socket
         if old is not None and old is not sock:
-            disconnect_socket(sock=old)
+            await disconnect_socket(sock=old)
 
     #
-    #   Flags
+    #   States
     #
 
+    @property
+    def state(self) -> ChannelState:
+        if self.__closed is None:
+            # initializing
+            return ChannelState.INIT
+        sock = self.sock
+        if sock is None or is_closed(sock=sock):
+            # closed
+            return ChannelState.CLOSED
+        elif is_connected(sock=sock) or is_bound(sock=sock):
+            # normal
+            return ChannelState.ALIVE
+        else:
+            # opened
+            return ChannelState.OPEN
+
     @property  # Override
     def closed(self) -> bool:
         if self.__closed is None:
             # initializing
             return False
         sock = self.sock
         return sock is None or is_closed(sock=sock)
@@ -256,81 +273,81 @@
     # Override
     def configure_blocking(self, blocking: bool):
         sock = self.sock
         sock.setblocking(blocking)
         return sock
 
     # Override
-    def bind(self, address: Optional[SocketAddress] = None,
-             host: Optional[str] = '0.0.0.0', port: Optional[int] = 0):
+    async def bind(self, address: Optional[SocketAddress] = None,
+                   host: Optional[str] = '0.0.0.0', port: Optional[int] = 0):
         if address is None:
             if port > 0:
                 assert host is not None, 'host should not be empty'
                 address = (host, port)
             else:
                 address = self._local
                 assert address is not None, 'local address not set'
         sock = self.sock
-        ok = bind_socket(sock=sock, local=address)
+        ok = await bind_socket(sock=sock, local=address)
         assert ok, 'failed to bind socket: %s' % str(address)
         self._local = address
         return sock
 
     # Override
-    def connect(self, address: Optional[SocketAddress] = None,
-                host: Optional[str] = '127.0.0.1', port: Optional[int] = 0) -> socket.socket:
+    async def connect(self, address: Optional[SocketAddress] = None,
+                      host: Optional[str] = '127.0.0.1', port: Optional[int] = 0) -> socket.socket:
         if address is None:
             if port > 0:
                 assert host is not None, 'host should not be empty'
                 address = (host, port)
             else:
                 address = self._remote
                 assert address is not None, 'remote address not set'
         sock = self.sock
-        ok = connect_socket(sock=sock, remote=address)
+        ok = await connect_socket(sock=sock, remote=address)
         assert ok, 'failed to connect socket: %s' % str(address)
         self._remote = address
         return sock
 
     # Override
-    def disconnect(self) -> Optional[socket.socket]:
+    async def disconnect(self) -> Optional[socket.socket]:
         sock = self.__sock
         if sock is not None:
-            ok = disconnect_socket(sock=sock)
+            ok = await disconnect_socket(sock=sock)
             assert ok, 'failed to disconnect socket: %s' % sock
         return sock
 
     # Override
-    def close(self):
-        self.set_socket(sock=None)
+    async def close(self):
+        await self.set_socket(sock=None)
 
     # Override
-    def read(self, max_len: int) -> Optional[bytes]:
+    async def read(self, max_len: int) -> Optional[bytes]:
         try:
-            return self.reader.read(max_len=max_len)
+            return await self.reader.read(max_len=max_len)
         except socket.error as error:
-            self.close()
+            await self.close()
             raise error
 
     # Override
-    def write(self, data: bytes) -> int:
+    async def write(self, data: bytes) -> int:
         try:
-            return self.writer.write(data=data)
+            return await self.writer.write(data=data)
         except socket.error as error:
-            self.close()
+            await self.close()
             raise error
 
     # Override
-    def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
+    async def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
         try:
-            return self.reader.receive(max_len=max_len)
+            return await self.reader.receive(max_len=max_len)
         except socket.error as error:
-            self.close()
+            await self.close()
             raise error
 
     # Override
-    def send(self, data: bytes, target: SocketAddress) -> int:
+    async def send(self, data: bytes, target: SocketAddress) -> int:
         try:
-            return self.writer.send(data=data, target=target)
+            return await self.writer.send(data=data, target=target)
         except socket.error as error:
-            self.close()
+            await self.close()
             raise error
```

### Comparing `startrek-1.2.0/startrek/socket/base_conn.py` & `startrek-2.0.0/startrek/socket/base_conn.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,21 +77,21 @@
     #
 
     @property  # protected
     def fsm(self) -> Optional[StateMachine]:
         return self.__fsm
 
     # private
-    def _set_state_machine(self, fsm: Optional[StateMachine]):
+    async def _set_state_machine(self, fsm: Optional[StateMachine]):
         # 1. replace with new machine
         old = self.__fsm
         self.__fsm = fsm
         # 2. stop old machine
         if old is not None and old is not fsm:
-            old.stop()
+            await old.stop()
 
     def _create_state_machine(self) -> StateMachine:
         fsm = StateMachine(connection=self)
         fsm.delegate = self
         return fsm
 
     #
@@ -100,24 +100,24 @@
 
     @property
     def channel(self) -> Optional[Channel]:
         ref = self.__channel_ref
         if ref is not None:
             return ref()
 
-    def _set_channel(self, channel: Optional[Channel]):
+    async def _set_channel(self, channel: Optional[Channel]):
         # 1. replace with new channel
         old = self.channel
         if channel is not None:
             self.__channel_ref = weakref.ref(channel)
         # else:
         #     self.__channel_ref = None
         # 2. close old channel
         if old is not None and old is not channel:
-            old.close()
+            await old.close()
 
     #
     #   Flags
     #
 
     @property  # Override
     def closed(self) -> bool:
@@ -162,106 +162,107 @@
     def __repr__(self) -> str:
         mod = self.__module__
         cname = self.__class__.__name__
         return '<%s remote="%s" local="%s">\n%s\n</%s module="%s">'\
                % (cname, self._remote, self._local, self.channel, cname, mod)
 
     # Override
-    def close(self):
+    async def close(self):
         # stop state machine
-        self._set_state_machine(fsm=None)
+        await self._set_state_machine(fsm=None)
         # close channel
-        self._set_channel(channel=None)
+        await self._set_channel(channel=None)
 
-    def start(self, hub: Hub):
+    async def start(self, hub: Hub):
         """ Get channel from hub """
         # 1. get channel from hub
-        self._open_channel(hub=hub)
+        await self._open_channel(hub=hub)
         # 2. start state machine
-        self._start_machine()
+        await self._start_machine()
 
-    def _start_machine(self):
+    async def _start_machine(self):
         fsm = self._create_state_machine()
-        self._set_state_machine(fsm=fsm)
-        fsm.start()
+        await self._set_state_machine(fsm=fsm)
+        await fsm.start()
 
     # protected
-    def _open_channel(self, hub: Hub) -> Optional[Channel]:
-        sock = hub.open(remote=self.remote_address, local=self.local_address)
+    async def _open_channel(self, hub: Hub) -> Optional[Channel]:
+        sock = await hub.open(remote=self.remote_address, local=self.local_address)
         if sock is None:
             assert False, 'failed to open channel: remote=%s, local=%s' % (self.remote_address, self.local_address)
         else:
-            self._set_channel(channel=sock)
+            await self._set_channel(channel=sock)
         return sock
 
     #
     #   I/O
     #
 
     # Override
-    def received(self, data: bytes):
+    async def received(self, data: bytes):
         self.__last_received_time = time.time()  # update received time
         delegate = self.delegate
         if delegate is not None:
-            delegate.connection_received(data=data, connection=self)
+            await delegate.connection_received(data=data, connection=self)
 
-    def _send(self, data: bytes, target: Optional[SocketAddress]) -> int:
+    async def _send(self, data: bytes, target: Optional[SocketAddress]) -> int:
         channel = self.channel
         if channel is None or not channel.alive:
             # raise socket.error('socket channel lost: %s' % channel)
             return -1
         elif target is None:
             # assert False, 'target address empty'
             return -1
-        sent = channel.send(data=data, target=target)
+        sent = await channel.send(data=data, target=target)
         if sent > 0:
+            # update sent time
             self.__last_sent_time = time.time()
         return sent
 
     # Override
-    def send(self, data: bytes) -> int:
+    async def send(self, data: bytes) -> int:
         # try to send data
         error = None
         sent = -1
         try:
-            sent = self._send(data=data, target=self.remote_address)
+            sent = await self._send(data=data, target=self.remote_address)
             if sent < 0:  # == -1:
                 raise socket.error('failed to send: %d byte(s) to %s' % (len(data), self.remote_address))
         except socket.error as e:
             error = e
             # socket error, close current channel
-            self._set_channel(channel=None)
+            await self._set_channel(channel=None)
         # callback
         delegate = self.delegate
         if delegate is not None:
             if error is None:
-                delegate.connection_sent(sent=sent, data=data, connection=self)
+                await delegate.connection_sent(sent=sent, data=data, connection=self)
             else:
-                delegate.connection_failed(error=error, data=data, connection=self)
+                await delegate.connection_failed(error=error, data=data, connection=self)
         return sent
 
     #
     #   States
     #
 
     @property  # Override
     def state(self) -> Optional[ConnectionState]:
         fsm = self.fsm
         if fsm is not None:
             return fsm.current_state
 
     # Override
-    def tick(self, now: float, elapsed: float):
+    async def tick(self, now: float, elapsed: float):
         if self.__channel_ref is None:
             # not initialized
             return
         fsm = self.fsm
         if fsm is not None:
             # drive state machine forward
-            fsm.tick(now=now, elapsed=elapsed)
+            await fsm.tick(now=now, elapsed=elapsed)
 
     #
     #   Timed Connection
     #
 
     @property  # Override
     def last_sent_time(self) -> float:
@@ -284,19 +285,19 @@
         return now > self.__last_received_time + (self.EXPIRES << 3)
 
     #
     #   StateDelegate
     #
 
     # Override
-    def enter_state(self, state: Optional[ConnectionState], ctx: StateMachine, now: float):
+    async def enter_state(self, state: Optional[ConnectionState], ctx: StateMachine, now: float):
         pass
 
     # Override
-    def exit_state(self, state: Optional[ConnectionState], ctx: StateMachine, now: float):
+    async def exit_state(self, state: Optional[ConnectionState], ctx: StateMachine, now: float):
         current = ctx.current_state
         if isinstance(current, ConnectionState):
             index = current.index
         else:
             assert current is None, 'unknown connection state: %s' % current
             index = -1
         # if current == 'ready'
@@ -310,16 +311,16 @@
                 if self.__last_sent_time < timestamp:
                     self.__last_sent_time = timestamp
                 if self.__last_received_time < timestamp:
                     self.__last_received_time = timestamp
         # callback
         delegate = self.delegate
         if delegate is not None:
-            delegate.connection_state_changed(previous=state, current=current, connection=self)
+            await delegate.connection_state_changed(previous=state, current=current, connection=self)
 
     # Override
-    def pause_state(self, state: Optional[ConnectionState], ctx: StateMachine, now: float):
+    async def pause_state(self, state: Optional[ConnectionState], ctx: StateMachine, now: float):
         pass
 
     # Override
-    def resume_state(self, state: Optional[ConnectionState], ctx: StateMachine, now: float):
+    async def resume_state(self, state: Optional[ConnectionState], ctx: StateMachine, now: float):
         pass
```

### Comparing `startrek-1.2.0/startrek/socket/base_hub.py` & `startrek-2.0.0/startrek/socket/base_hub.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,41 +31,43 @@
 import socket
 import threading
 import time
 import weakref
 from abc import ABC, abstractmethod
 from typing import Optional, Iterable
 
+from ..fsm import Runner
 from ..types import SocketAddress, AddressPairMap
+from ..net.channel import ChannelState
 from ..net import Hub, Channel, Connection, ConnectionDelegate
 from .base_conn import BaseConnection
 
 
 class ConnectionPool(AddressPairMap[Connection]):
 
     # Override
     def set(self, item: Optional[Connection],
             remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Connection]:
         # 1. remove cached item
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
-            cached.close()
+            Runner.async_run(coroutine=cached.close())
         # 2. set new item
         old = super().set(item=item, remote=remote, local=local)
         assert old is None, 'should not happen: %s' % old
         return cached
 
     # Override
     def remove(self, item: Optional[Connection],
                remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Connection]:
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
-            cached.close()
+            Runner.async_run(coroutine=cached.close())
         if item is not None:
-            item.close()
+            Runner.async_run(coroutine=item.close())
         return cached
 
 
 class BaseHub(Hub, ABC):
 
     """
         Maximum Segment Size
@@ -149,82 +151,88 @@
 
     def _set_connection(self, connection: Connection,
                         remote: SocketAddress, local: Optional[SocketAddress]) -> Optional[Connection]:
         """ cache connection """
         return self.__connection_pool.set(item=connection, remote=remote, local=local)
 
     # Override
-    def connect(self, remote: SocketAddress, local: Optional[SocketAddress] = None) -> Optional[Connection]:
+    async def connect(self, remote: SocketAddress, local: Optional[SocketAddress] = None) -> Optional[Connection]:
         # try to get connection
         with self.__lock:
             old = self._get_connection(remote=remote, local=local)
             if old is None:
                 # create & cache connection
                 conn = self._create_connection(remote=remote, local=local)
                 self._set_connection(conn, remote=remote, local=local)
             else:
                 conn = old
         if old is None:
             assert isinstance(conn, BaseConnection), 'connection error: %s, %s' % (remote, conn)
             # try to open channel with direction (remote, local)
-            conn.start(hub=self)
+            await conn.start(hub=self)
         return conn
 
     #
     #   Process
     #
 
-    def _drive_channel(self, channel: Channel) -> bool:
-        if not channel.available:
-            # channel has no data to receive
+    async def _drive_channel(self, channel: Channel) -> bool:
+        cs = channel.state
+        if cs == ChannelState.INIT:
+            # preparing
             return False
-        # try to receive
+        elif cs == ChannelState.CLOSED:
+            # finished
+            return False
+        # cs == opened
+        # cs == alive
         try:
-            data, remote = channel.receive(max_len=self.MSS)
+            # try to receive
+            data, remote = await channel.receive(max_len=self.MSS)
         except socket.error as error:
             remote = channel.remote_address
             local = channel.local_address
             delegate = self.delegate
             if delegate is None or remote is None:
                 # UDP channel may not connected
                 # so no connection for it
                 self._remove_channel(channel=channel, remote=remote, local=local)
             else:
                 # remove channel and callback with connection
                 conn = self._get_connection(remote=remote, local=local)
                 self._remove_channel(channel=channel, remote=remote, local=local)
                 if conn is not None:
-                    delegate.connection_error(error=error, connection=conn)
+                    await delegate.connection_error(error=error, connection=conn)
             return False
-        if remote is None:
+        if remote is None or data is None or len(data) == 0:
             # received nothing
             return False
         else:
             local = channel.local_address
         # get connection for processing received data
-        conn = self.connect(remote=remote, local=local)
+        conn = await self.connect(remote=remote, local=local)
         if conn is not None:
-            conn.received(data=data)
+            await conn.received(data=data)
         return True
 
-    def _drive_channels(self, channels: Iterable[Channel]) -> int:
+    async def _drive_channels(self, channels: Iterable[Channel]) -> int:
         count = 0
         for sock in channels:
             # drive channel to receive data
-            if self._drive_channel(channel=sock):
+            if await self._drive_channel(channel=sock):
                 count += 1
         return count
 
     # noinspection PyMethodMayBeStatic
-    def _drive_connections(self, connections: Iterable[Connection]):
+    async def _drive_connections(self, connections: Iterable[Connection]):
         now = time.time()
         elapsed = now - self.__last_time_drive_connection
         for conn in connections:
             # drive connection to go on
-            conn.tick(now=now, elapsed=elapsed)
+            await conn.tick(now=now, elapsed=elapsed)
             # NOTICE: let the delegate to decide whether close an error connection
             #         or just remove it.
         self.__last_time_drive_connection = now
 
     def _cleanup_channels(self, channels: Iterable[Channel]):
         for sock in channels:
             if sock.closed:
@@ -238,18 +246,18 @@
             if conn.closed:
                 # if connection closed, remove it from the hub; notice that
                 # ActiveConnection can reconnect, it'll be not connected
                 # but still open, don't remove it in this situation.
                 self._remove_connection(connection=conn, remote=conn.remote_address, local=conn.local_address)
 
     # Override
-    def process(self) -> bool:
+    async def process(self) -> bool:
         # 1. drive all channels to receive data
         channels = self._all_channels()
-        count = self._drive_channels(channels=channels)
+        count = await self._drive_channels(channels=channels)
         # 2. drive all connections to move on
         connections = self._all_connections()
-        self._drive_connections(connections=connections)
+        await self._drive_connections(connections=connections)
         # 3. cleanup closed channels and connections
         self._cleanup_channels(channels=channels)
         self._cleanup_connections(connections=connections)
         return count > 0
```

### Comparing `startrek-1.2.0/startrek/stardocker.py` & `startrek-2.0.0/startrek/stardocker.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,25 +88,25 @@
 
     @property
     def connection(self) -> Optional[Connection]:
         ref = self.__conn_ref
         if ref is not None:
             return ref()
 
-    def set_connection(self, conn: Optional[Connection]):
+    async def set_connection(self, conn: Optional[Connection]):
         """ set connection for this docker """
         # 1. replace with new connection
         old = self.connection
         if conn is not None:
             self.__conn_ref = weakref.ref(conn)
         # else:
         #     self.__conn_ref = None
         # 2. close old connection
         if old is not None and old is not conn:
-            old.close()
+            await old.close()
 
     #
     #   Flags
     #
 
     @property  # Override
     def closed(self) -> bool:
@@ -136,70 +136,70 @@
     def __repr__(self) -> str:
         mod = self.__module__
         cname = self.__class__.__name__
         return '<%s remote="%s" local="%s" status="%s">\n%s\n</%s module="%s">'\
                % (cname, self._remote, self._local, self.status, self.connection, cname, mod)
 
     # Override
-    def send_ship(self, ship: Departure) -> bool:
+    async def send_ship(self, ship: Departure) -> bool:
         return self.__dock.add_departure(ship=ship)
 
     # Override
-    def process_received(self, data: bytes):
+    async def process_received(self, data: bytes):
         # 1. get income ship from received data
         ships = self._get_arrivals(data=data)
         if ships is None or len(ships) == 0:
             # waiting for more data
             return None
         delegate = self.delegate
         for income in ships:
             # 2. check income ship for response
-            income = self._check_arrival(ship=income)
+            income = await self._check_arrival(ship=income)
             if income is None:
                 # waiting for more fragment
                 continue
             # 3. callback for processing income ship with completed data package
             if delegate is not None:
-                delegate.docker_received(ship=income, docker=self)
+                await delegate.docker_received(ship=income, docker=self)
 
     @abstractmethod
     def _get_arrivals(self, data: bytes) -> List[Arrival]:
         """
         Get income ships from received data
 
         :param data: received data
         :return income ships carrying data package/fragments
         """
         raise NotImplemented
 
     @abstractmethod
-    def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
+    async def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
         """
         Check income ship for responding
 
         :param ship: income ship carrying data package/fragment/response
         :return income ship carrying completed data package
         """
         raise NotImplemented
 
-    def _check_response(self, ship: Arrival) -> Optional[Departure]:
+    async def _check_response(self, ship: Arrival) -> Optional[Departure]:
         """
         Check and remove linked departure ship with same SN (and page index for fragment)
 
         :param ship: income ship with SN
         """
         # check response for linked departure ship (same SN)
         linked = self.__dock.check_response(ship=ship)
         if linked is None:
             # linked departure task not found, or not finished yet
             return None
         # all fragments responded, task finished
         delegate = self.delegate
         if delegate is not None:
-            delegate.docker_sent(ship=linked, docker=self)
+            await delegate.docker_sent(ship=linked, docker=self)
         return linked
 
     def _assemble_arrival(self, ship: Arrival) -> Optional[Arrival]:
         """ Check received ship for completed package """
         return self.__dock.assemble_arrival(ship=ship)
 
     def _next_departure(self, now: float) -> Optional[Departure]:
@@ -207,23 +207,23 @@
         return self.__dock.next_departure(now=now)
 
     # Override
     def purge(self, now: float = 0) -> int:
         return self.__dock.purge(now=now)
 
     # Override
-    def close(self):
-        self.set_connection(conn=None)
+    async def close(self):
+        await self.set_connection(conn=None)
 
     #
     #  Processor
     #
 
     # Override
-    def process(self) -> bool:
+    async def process(self) -> bool:
         # 1. get connection which is ready for sending data
         conn = self.connection
         if conn is None:
             # waiting for connection
             return False
         elif not conn.vacant:
             # connection is not ready for sending data
@@ -243,30 +243,30 @@
                 # nothing to do now, return false to let the thread have a rest
                 return False
             elif outgo.get_status(now=now) == ShipStatus.FAILED:
                 delegate = self.delegate
                 if delegate is not None:
                     # callback for mission failed
                     error = TimeoutError('Request timeout')
-                    delegate.docker_failed(error=error, ship=outgo, docker=self)
+                    await delegate.docker_failed(error=error, ship=outgo, docker=self)
                 # task timeout, return True to process next one
                 return True
             else:
                 # get fragments from outgo task
                 fragments = outgo.fragments
                 if len(fragments) == 0:
                     # all fragments of this task have been sent already
                     # return True to process next one
                     return True
         # 3. process fragments of outgo task
         index = 0
         sent = 0
         try:
             for fra in fragments:
-                sent = conn.send(data=fra)
+                sent = await conn.send(data=fra)
                 if sent < len(fra):
                     # buffer overflow?
                     break
                 else:
                     # assert sent == len(fra), 'length of fragment error: %d, %d' % (sent, len(fra))
                     index += 1
                     sent = 0  # clear counter
@@ -279,15 +279,15 @@
                     # this task needs response,
                     # so we cannot call 'docker_sent()' immediately
                     # until the remote responded.
                     pass
                 else:
                     delegate = self.delegate
                     if delegate is not None:
-                        delegate.docker_sent(ship=outgo, docker=self)
+                        await delegate.docker_sent(ship=outgo, docker=self)
                 return True
         except Exception as e:
             # socket error, callback
             error = e
         # 4. remove sent fragments
         while index > 0:
             fragments.pop(0)
@@ -298,10 +298,11 @@
             fragments.insert(0, last[sent:])
         # 5. store remaining data
         self.__last_outgo = outgo
         self.__last_fragments = fragments
         # 6. callback for error
         delegate = self.delegate
         if delegate is not None:
-            delegate.docker_error(error=error, ship=outgo, docker=self)
+            # await delegate.docker_failed(error=error, ship=outgo, docker=self)
+            await delegate.docker_error(error=error, ship=outgo, docker=self)
         # task error
         return False
```

### Comparing `startrek-1.2.0/startrek/stargate.py` & `startrek-2.0.0/startrek/stargate.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import socket
 import threading
 import time
 import weakref
 from abc import ABC, abstractmethod
 from typing import Optional, List, Iterable, Union
 
+from .fsm import Runner
 from .types import SocketAddress, AddressPairMap
 from .net import Connection, ConnectionDelegate, ConnectionState
 from .net.state import StateOrder
 from .port import Departure, Gate
 from .port import Docker, DockerStatus, DockerDelegate
 from .port.docker import status_from_state
 from .stardocker import StarDocker
@@ -48,28 +49,28 @@
 
     # Override
     def set(self, item: Optional[Docker],
             remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Docker]:
         # 1. remove cached item
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
-            cached.close()
+            Runner.async_run(coroutine=cached.close())
         # 2. set new item
         old = super().set(item=item, remote=remote, local=local)
         assert old is None, 'should not happen: %s' % old
         return cached
 
     # Override
     def remove(self, item: Optional[Docker],
                remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Docker]:
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
-            cached.close()
+            Runner.async_run(coroutine=cached.close())
         if item is not None:
-            item.close()
+            Runner.async_run(coroutine=item.close())
         return cached
 
 
 class StarGate(Gate, ConnectionDelegate, ABC):
     """
         Star Gate
         ~~~~~~~~~
@@ -91,35 +92,35 @@
         return DockerPool()
 
     @property
     def delegate(self) -> Optional[DockerDelegate]:
         return self.__delegate_ref()
 
     # Override
-    def send_data(self, payload: Union[bytes, bytearray],
-                  remote: SocketAddress, local: Optional[SocketAddress]) -> bool:
+    async def send_data(self, payload: Union[bytes, bytearray],
+                        remote: SocketAddress, local: Optional[SocketAddress]) -> bool:
         worker = self._get_docker(remote=remote, local=local)
         if worker is None:
             # assert False, 'docker not found: %s -> %s' % (local, remote)
             return False
         elif not worker.alive:
             # assert False, 'docket not alive: %s -> %s' % (local, remote)
             return False
-        return worker.send_data(payload=payload)
+        return await worker.send_data(payload=payload)
 
     # Override
-    def send_ship(self, ship: Departure, remote: SocketAddress, local: Optional[SocketAddress]) -> bool:
+    async def send_ship(self, ship: Departure, remote: SocketAddress, local: Optional[SocketAddress]) -> bool:
         worker = self._get_docker(remote=remote, local=local)
         if worker is None:
             # assert False, 'docker not found: %s -> %s' % (local, remote)
             return False
         elif not worker.alive:
             # assert False, 'docket not alive: %s -> %s' % (local, remote)
             return False
-        return worker.send_ship(ship=ship)
+        return await worker.send_ship(ship=ship)
 
     #
     #   Docker
     #
 
     @abstractmethod
     def _create_docker(self, parties: List[bytes],
@@ -153,55 +154,55 @@
         return self.__docker_pool.set(item=docker, remote=remote, local=local)
 
     #
     #   Processor
     #
 
     # Override
-    def process(self) -> bool:
+    async def process(self) -> bool:
         dockers = self._all_dockers()
         # 1. drive all dockers to process
-        count = self._drive_dockers(dockers=dockers)
+        count = await self._drive_dockers(dockers=dockers)
         # 2. cleanup for dockers
         self._cleanup_dockers(dockers=dockers)
         return count > 0
 
     # noinspection PyMethodMayBeStatic
-    def _drive_dockers(self, dockers: Iterable[Docker]) -> int:
+    async def _drive_dockers(self, dockers: Iterable[Docker]) -> int:
         count = 0
         for worker in dockers:
-            if worker.process():
+            if await worker.process():
                 count += 1  # it's busy
         return count
 
     def _cleanup_dockers(self, dockers: Iterable[Docker]):
         now = time.time()
         for worker in dockers:
             if worker.closed:
                 # remove docker which connection lost
                 self._remove_docker(docker=worker, remote=worker.remote_address, local=worker.local_address)
             else:
                 # clear expired tasks
                 worker.purge(now=now)
 
-    def _heartbeat(self, connection: Connection):
+    async def _heartbeat(self, connection: Connection):
         """ Send a heartbeat package('PING') to remote address """
         remote = connection.remote_address
         local = connection.local_address
         worker = self._get_docker(remote=remote, local=local)
         if worker is not None:
-            worker.heartbeat()
+            await worker.heartbeat()
 
     #
     #   Connection Delegate
     #
 
     # Override
-    def connection_state_changed(self, previous: Optional[ConnectionState], current: Optional[ConnectionState],
-                                 connection: Connection):
+    async def connection_state_changed(self, previous: Optional[ConnectionState], current: Optional[ConnectionState],
+                                       connection: Connection):
         # convert status
         s1 = status_from_state(state=previous)
         s2 = status_from_state(state=current)
         # 1. callback when status changed
         if s1 != s2:
             remote = connection.remote_address
             local = connection.local_address
@@ -216,28 +217,28 @@
                     worker = self._create_docker([], remote=remote, local=local)
                     self._set_docker(worker, remote=remote, local=local)
                 else:
                     worker = old
             if old is None:
                 assert isinstance(worker, StarDocker), 'docker error: %s, %s' % (remote, worker)
                 # set connection for this docker
-                worker.set_connection(connection)
+                await worker.set_connection(connection)
             # NOTICE: if the previous state is null, the docker maybe not
             #         created yet, this situation means the docker status
             #         not changed too, so no need to callback here.
             delegate = self.delegate
             if delegate is not None:
-                delegate.docker_status_changed(previous=s1, current=s2, docker=worker)
+                await delegate.docker_status_changed(previous=s1, current=s2, docker=worker)
         # 2. heartbeat when connection expired
         index = -1 if current is None else current.index
         if index == StateOrder.EXPIRED:
-            self._heartbeat(connection=connection)
+            await self._heartbeat(connection=connection)
 
     # Override
-    def connection_received(self, data: bytes, connection: Connection):
+    async def connection_received(self, data: bytes, connection: Connection):
         remote = connection.remote_address
         local = connection.local_address
         # try to get docker
         with self.__lock:
             old = self._get_docker(remote=remote, local=local)
             if old is None:
                 # cache advance party for this connection
@@ -248,23 +249,23 @@
                 self._set_docker(worker, remote=remote, local=local)
             else:
                 party = []
                 worker = old
         if old is None:
             assert isinstance(worker, StarDocker), 'docker error: %s, %s' % (remote, worker)
             # set connection for this docker
-            worker.set_connection(connection)
+            await worker.set_connection(connection)
             # process advance parties one by one
             for item in party:
-                worker.process_received(data=item)
+                await worker.process_received(data=item)
             # remove advance party
             self._clear_advance_party(connection=connection)
         else:
             # docker exists, call docker.onReceived(data)
-            worker.process_received(data=data)
+            await worker.process_received(data=data)
 
     @abstractmethod
     def _cache_advance_party(self, data: bytes, connection: Connection) -> List[bytes]:
         """
         Cache the advance party before decide which docker to use
 
         :param data:        received data
@@ -279,20 +280,20 @@
         Clear all advance parties after docker created
 
         :param connection:  current connection
         """
         raise NotImplemented
 
     # Override
-    def connection_sent(self, sent: int, data: bytes, connection: Connection):
+    async def connection_sent(self, sent: int, data: bytes, connection: Connection):
         # ignore event for sending success
         pass
 
     # Override
-    def connection_failed(self, error: Union[IOError, socket.error], data: bytes, connection: Connection):
+    async def connection_failed(self, error: Union[IOError, socket.error], data: bytes, connection: Connection):
         # ignore event for sending failed
         pass
 
     # Override
-    def connection_error(self, error: Union[IOError, socket.error], connection: Connection):
+    async def connection_error(self, error: Union[IOError, socket.error], connection: Connection):
         # ignore event for receiving error
         pass
```

### Comparing `startrek-1.2.0/startrek/types/__init__.py` & `startrek-2.0.0/startrek/types/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.2.0/startrek/types/mapping.py` & `startrek-2.0.0/startrek/types/mapping.py`

 * *Files identical despite different names*

### Comparing `startrek-1.2.0/startrek/types/pair.py` & `startrek-2.0.0/startrek/types/pair.py`

 * *Files identical despite different names*

### Comparing `startrek-1.2.0/startrek.egg-info/SOURCES.txt` & `startrek-2.0.0/startrek.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 startrek.egg-info/PKG-INFO
 startrek.egg-info/SOURCES.txt
 startrek.egg-info/dependency_links.txt
 startrek.egg-info/top_level.txt
 startrek/fsm/__init__.py
 startrek/fsm/auto.py
 startrek/fsm/base.py
+startrek/fsm/daemon.py
 startrek/fsm/machine.py
 startrek/fsm/runner.py
 startrek/fsm/ticker.py
 startrek/net/__init__.py
 startrek/net/channel.py
 startrek/net/connection.py
 startrek/net/delegate.py
```

