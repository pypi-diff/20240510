# Comparing `tmp/profitpulse-1.6.0.tar.gz` & `tmp/profitpulse-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profitpulse-1.6.0.tar", max compression
+gzip compressed data, was "profitpulse-2.0.0.tar", max compression
```

## Comparing `profitpulse-1.6.0.tar` & `profitpulse-2.0.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
--rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-1.6.0/LICENSE
--rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-1.6.0/README.md
--rw-r--r--   0        0        0     1840 2024-05-06 20:10:40.253167 profitpulse-1.6.0/pyproject.toml
--rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-1.6.0/src/profitpulse/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-1.6.0/src/profitpulse/cli/__init__.py
--rw-r--r--   0        0        0     8292 2024-05-06 20:00:20.119273 profitpulse-1.6.0/src/profitpulse/cli/adapters.py
--rw-r--r--   0        0        0     5202 2024-05-06 17:27:14.195913 profitpulse-1.6.0/src/profitpulse/cli/main.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-1.6.0/src/profitpulse/data/__init__.py
--rw-r--r--   0        0        0     5989 2024-05-06 20:00:20.120217 profitpulse-1.6.0/src/profitpulse/data/accounts.py
--rw-r--r--   0        0        0     2855 2024-05-06 19:33:31.689142 profitpulse-1.6.0/src/profitpulse/data/accounts_test.py
--rw-r--r--   0        0        0     1894 2024-05-06 20:00:20.120854 profitpulse-1.6.0/src/profitpulse/data/pulse_view.py
--rw-r--r--   0        0        0     1630 2024-05-06 20:00:20.121528 profitpulse-1.6.0/src/profitpulse/data/pulse_view_test.py
--rw-r--r--   0        0        0     2007 2024-05-05 20:18:18.593519 profitpulse-1.6.0/src/profitpulse/data/transactions.py
--rw-r--r--   0        0        0     4677 2024-05-06 20:00:20.122106 profitpulse-1.6.0/src/profitpulse/data/views.py
--rw-r--r--   0        0        0     6833 2024-05-05 19:43:17.725626 profitpulse-1.6.0/src/profitpulse/data/views_test.py
--rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-1.6.0/src/profitpulse/gateways/__init__.py
--rw-r--r--   0        0        0     3188 2024-05-05 20:11:25.598621 profitpulse-1.6.0/src/profitpulse/gateways/cgdfile.py
--rw-r--r--   0        0        0     2030 2024-05-05 19:43:17.281923 profitpulse-1.6.0/src/profitpulse/gateways/cgdfile_test.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-1.6.0/src/profitpulse/infrastructure/__init__.py
--rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-1.6.0/src/profitpulse/infrastructure/migrations.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-1.6.0/src/profitpulse/lib/__init__.py
--rw-r--r--   0        0        0     1831 2024-05-06 19:33:31.689548 profitpulse-1.6.0/src/profitpulse/lib/account.py
--rw-r--r--   0        0        0      549 2024-04-27 17:48:38.578920 profitpulse-1.6.0/src/profitpulse/lib/account_name.py
--rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-1.6.0/src/profitpulse/lib/comment.py
--rw-r--r--   0        0        0      863 2024-05-05 19:54:59.624362 profitpulse-1.6.0/src/profitpulse/lib/money.py
--rw-r--r--   0        0        0      232 2024-05-04 22:12:33.559763 profitpulse-1.6.0/src/profitpulse/lib/transaction.py
--rw-r--r--   0        0        0      954 2024-05-05 19:49:14.366161 profitpulse-1.6.0/src/profitpulse/migrations/0001 - Initial.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-1.6.0/src/profitpulse/migrations/0002 - accounts.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-1.6.0/src/profitpulse/migrations/__init__.py
--rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-1.6.0/src/profitpulse/services/__init__.py
--rw-r--r--   0        0        0     1031 2024-05-06 19:33:31.690477 profitpulse-1.6.0/src/profitpulse/services/close_account.py
--rw-r--r--   0        0        0     1693 2024-05-06 19:33:31.691325 profitpulse-1.6.0/src/profitpulse/services/close_account_test.py
--rw-r--r--   0        0        0     1047 2024-05-06 19:33:31.692391 profitpulse-1.6.0/src/profitpulse/services/delete_account.py
--rw-r--r--   0        0        0     1559 2024-05-06 19:33:31.693279 profitpulse-1.6.0/src/profitpulse/services/delete_account_test.py
--rw-r--r--   0        0        0     1432 2024-05-06 19:33:31.694493 profitpulse-1.6.0/src/profitpulse/services/deposit_into_account.py
--rw-r--r--   0        0        0     2848 2024-05-06 19:33:31.695520 profitpulse-1.6.0/src/profitpulse/services/deposit_into_account_test.py
--rw-r--r--   0        0        0      303 2024-05-05 19:29:56.485862 profitpulse-1.6.0/src/profitpulse/services/errors.py
--rw-r--r--   0        0        0     1672 2024-05-06 19:33:31.696410 profitpulse-1.6.0/src/profitpulse/services/import_transactions.py
--rw-r--r--   0        0        0     2112 2024-05-06 19:33:31.697162 profitpulse-1.6.0/src/profitpulse/services/import_transactions_test.py
--rw-r--r--   0        0        0     1231 2024-05-06 19:33:31.697817 profitpulse-1.6.0/src/profitpulse/services/open_account.py
--rw-r--r--   0        0        0     1719 2024-05-06 19:33:31.698567 profitpulse-1.6.0/src/profitpulse/services/open_account_test.py
--rw-r--r--   0        0        0     1203 2024-05-06 19:33:31.699271 profitpulse-1.6.0/src/profitpulse/services/revalue.py
--rw-r--r--   0        0        0     1731 2024-05-06 19:33:31.700207 profitpulse-1.6.0/src/profitpulse/services/revalue_test.py
--rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-1.6.0/src/profitpulse/testrig/__init__.py
--rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-1.6.0/src/profitpulse/testrig/factory.py
--rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-1.6.0/src/profitpulse/testrig/fixtures.py
--rw-r--r--   0        0        0     4748 2024-05-06 19:58:30.761194 profitpulse-1.6.0/src/profitpulse/testrig/scenario.py
--rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-1.6.0/src/profitpulse/turbofan.py
--rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 profitpulse-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-2.0.0/README.md
+-rw-r--r--   0        0        0     1840 2024-05-10 11:36:35.784534 profitpulse-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-2.0.0/src/profitpulse/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-2.0.0/src/profitpulse/cli/__init__.py
+-rw-r--r--   0        0        0     8599 2024-05-10 06:54:12.881996 profitpulse-2.0.0/src/profitpulse/cli/adapters.py
+-rw-r--r--   0        0        0     5122 2024-05-10 11:11:53.203489 profitpulse-2.0.0/src/profitpulse/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-2.0.0/src/profitpulse/data/__init__.py
+-rw-r--r--   0        0        0     4533 2024-05-10 06:54:12.882781 profitpulse-2.0.0/src/profitpulse/data/assets.py
+-rw-r--r--   0        0        0     2409 2024-05-10 06:54:12.883293 profitpulse-2.0.0/src/profitpulse/data/assets_test.py
+-rw-r--r--   0        0        0      360 2024-05-10 06:54:12.884114 profitpulse-2.0.0/src/profitpulse/data/data.py
+-rw-r--r--   0        0        0     2149 2024-05-10 06:54:12.885295 profitpulse-2.0.0/src/profitpulse/data/pulse_view.py
+-rw-r--r--   0        0        0     3057 2024-05-10 06:54:12.885866 profitpulse-2.0.0/src/profitpulse/data/pulse_view_test.py
+-rw-r--r--   0        0        0     1951 2024-05-10 06:54:12.886478 profitpulse-2.0.0/src/profitpulse/data/transactions.py
+-rw-r--r--   0        0        0     4715 2024-05-10 06:54:12.887002 profitpulse-2.0.0/src/profitpulse/data/views.py
+-rw-r--r--   0        0        0     6779 2024-05-10 06:54:12.887503 profitpulse-2.0.0/src/profitpulse/data/views_test.py
+-rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-2.0.0/src/profitpulse/gateways/__init__.py
+-rw-r--r--   0        0        0     3188 2024-05-05 20:11:25.598621 profitpulse-2.0.0/src/profitpulse/gateways/cgdfile.py
+-rw-r--r--   0        0        0     2030 2024-05-05 19:43:17.281923 profitpulse-2.0.0/src/profitpulse/gateways/cgdfile_test.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-2.0.0/src/profitpulse/infrastructure/__init__.py
+-rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-2.0.0/src/profitpulse/infrastructure/migrations.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-2.0.0/src/profitpulse/lib/__init__.py
+-rw-r--r--   0        0        0     1962 2024-05-10 06:54:12.888068 profitpulse-2.0.0/src/profitpulse/lib/asset.py
+-rw-r--r--   0        0        0      541 2024-05-07 20:15:15.902011 profitpulse-2.0.0/src/profitpulse/lib/asset_name.py
+-rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-2.0.0/src/profitpulse/lib/comment.py
+-rw-r--r--   0        0        0      964 2024-05-10 06:54:12.889055 profitpulse-2.0.0/src/profitpulse/lib/money.py
+-rw-r--r--   0        0        0      232 2024-05-04 22:12:33.559763 profitpulse-2.0.0/src/profitpulse/lib/transaction.py
+-rw-r--r--   0        0        0      954 2024-05-05 19:49:14.366161 profitpulse-2.0.0/src/profitpulse/migrations/0001 - Initial.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-2.0.0/src/profitpulse/migrations/0002 - accounts.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-2.0.0/src/profitpulse/migrations/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-2.0.0/src/profitpulse/services/__init__.py
+-rw-r--r--   0        0        0     1468 2024-05-10 06:54:12.890186 profitpulse-2.0.0/src/profitpulse/services/acquire_asset.py
+-rw-r--r--   0        0        0     1636 2024-05-10 06:54:12.891286 profitpulse-2.0.0/src/profitpulse/services/acquire_asset_test.py
+-rw-r--r--   0        0        0     1298 2024-05-10 06:54:12.892139 profitpulse-2.0.0/src/profitpulse/services/delete_asset.py
+-rw-r--r--   0        0        0     1475 2024-05-10 06:54:12.892714 profitpulse-2.0.0/src/profitpulse/services/delete_asset_test.py
+-rw-r--r--   0        0        0     1888 2024-05-10 06:54:12.893192 profitpulse-2.0.0/src/profitpulse/services/deposit_into_asset.py
+-rw-r--r--   0        0        0     2680 2024-05-10 06:54:12.893995 profitpulse-2.0.0/src/profitpulse/services/deposit_into_asset_test.py
+-rw-r--r--   0        0        0     1428 2024-05-10 06:54:12.894591 profitpulse-2.0.0/src/profitpulse/services/divest_asset.py
+-rw-r--r--   0        0        0     1611 2024-05-10 06:54:12.895330 profitpulse-2.0.0/src/profitpulse/services/divest_asset_test.py
+-rw-r--r--   0        0        0      285 2024-05-07 20:15:15.913869 profitpulse-2.0.0/src/profitpulse/services/errors.py
+-rw-r--r--   0        0        0     2091 2024-05-10 06:54:12.895866 profitpulse-2.0.0/src/profitpulse/services/import_transactions.py
+-rw-r--r--   0        0        0     1967 2024-05-10 06:54:12.896440 profitpulse-2.0.0/src/profitpulse/services/import_transactions_test.py
+-rw-r--r--   0        0        0     1609 2024-05-10 06:54:12.896794 profitpulse-2.0.0/src/profitpulse/services/revalue_asset.py
+-rw-r--r--   0        0        0     1625 2024-05-10 06:54:12.897592 profitpulse-2.0.0/src/profitpulse/services/revalue_test.py
+-rw-r--r--   0        0        0     1049 2024-05-10 06:54:12.898087 profitpulse-2.0.0/src/profitpulse/services/services.py
+-rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-2.0.0/src/profitpulse/testrig/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-2.0.0/src/profitpulse/testrig/factory.py
+-rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-2.0.0/src/profitpulse/testrig/fixtures.py
+-rw-r--r--   0        0        0     4687 2024-05-08 17:37:21.761504 profitpulse-2.0.0/src/profitpulse/testrig/scenario.py
+-rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-2.0.0/src/profitpulse/turbofan.py
+-rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 profitpulse-2.0.0/PKG-INFO
```

### Comparing `profitpulse-1.6.0/LICENSE` & `profitpulse-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `profitpulse-1.6.0/README.md` & `profitpulse-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `profitpulse-1.6.0/pyproject.toml` & `profitpulse-2.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "profitpulse"
-version = "1.6.0"
+version = "2.0.0"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 maintainers = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/luistm/profitpulse"
 
@@ -51,15 +51,15 @@
 python = "^3.9"
 pendulum = "^3.0.0"
 rich = "^13.7.1"
 toml = "^0.10.2"
 turbofan = "^0.2.0"
 typer = "^0.12.3"
 gogotable = "^0.0.3"
-pastperfect = "^0.0.2"
+pastperfect = "^0.1.0"
 
 [tool.pytest.ini_options]
 markers = ["integration: tags a test as integration tests"]
 
 [tool.poetry.dev-dependencies.bandit]
 extras = ["toml"]
 version = "^1.7.8"
```

### Comparing `profitpulse-1.6.0/src/profitpulse/cli/adapters.py` & `profitpulse-2.0.0/src/profitpulse/cli/adapters.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,61 +4,59 @@
 """
 
 import logging
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
+import pastperfect
 from gogotable import gogotable
 from turbofan.database import Database, Session
 
-from profitpulse.data.accounts import Accounts
+from profitpulse.data.assets import Assets
 from profitpulse.data.pulse_view import PulseView
 from profitpulse.data.transactions import Transactions
-from profitpulse.data.views import AccountsView, TransactionsView
+from profitpulse.data.views import AssetsView, TransactionsView
 from profitpulse.gateways.cgdfile import GatewayCGDFile  # type: ignore
-from profitpulse.lib.account_name import AccountName
+from profitpulse.lib.asset_name import AssetName
 from profitpulse.lib.comment import Comment
 from profitpulse.lib.money import Money
-from profitpulse.services.close_account import (
-    CloseAccountRequester,
-    CloseAccountService,
+from profitpulse.services.acquire_asset import (
+    AcquireAssetService,
+    AssetAlreadyExistsError,
+    OpenAssetRequester,
 )
-from profitpulse.services.delete_account import (
-    DeleteAccountRequester,
-    DeleteAccountService,
-)
-from profitpulse.services.deposit_into_account import (
-    DepositIntoAccountRequester,
-    DepositIntoAccountService,
+from profitpulse.services.delete_asset import DeleteAssetRequester, DeleteAssetService
+from profitpulse.services.deposit_into_asset import (
+    DepositIntoAssetRequester,
+    DepositIntoAssetService,
 )
+from profitpulse.services.divest_asset import DivestAssetRequester, DivestAssetService
 from profitpulse.services.import_transactions import (
     ImportTransactionsRequester,
     ImportTransactionsService,
 )
-from profitpulse.services.open_account import (
-    AccountAlreadyExistsError,
-    OpenAccountRequester,
-    OpenAccountService,
+from profitpulse.services.revalue_asset import (
+    RevalueAssetRequester,
+    RevalueAssetService,
 )
-from profitpulse.services.revalue import RevalueAccountRequester, RevalueAccountService
 
 logging.basicConfig(level=logging.CRITICAL)
 logger = logging.getLogger(__name__)
 
 database_path = Path.home() / Path("Library/Application Support/Profitpulse")
 
 
 def report(
     seller: Optional[str],
     since: Optional[datetime] = None,
     on: Optional[datetime] = None,
 ) -> None:
     """
-    Shows a report of all transactions in all accounts given the provided
+    Shows a report of all transactions in all assets given the provided
      parameters:
      - seller: The provider or recipient of the value
      - since: The data from which the transactions should be shown
      - on: A specific date for which transactions should be shown
     """
 
     db = Database(database_path)
@@ -75,205 +73,215 @@
 
 
 def pulse() -> None:
     """
     Shows the current wealth status.
     """
 
-    headers = ["Account Name", "Status", "Invested", "Current", "Performance"]
+    headers = ["Asset Name", "Status", "Invested", "Current", "Performance"]
 
     db = Database(database_path)
     with Session(db.engine) as session:
         view = PulseView(session)
-        lines = gogotable(headers, view.data)
+        data = view.data
+        lines = gogotable(headers, data["assets"])  # {'assets': [], 'total': '0.00'}
         for line in lines:
             print(line)
+        print(f"Total: {data['total']}")
 
 
-class RevalueAccountRequest(RevalueAccountRequester):
-    def __init__(self, account_name: str, value: int) -> None:
-        self._account_name = account_name
+class RevalueAssetRequest(RevalueAssetRequester):
+    def __init__(self, asset_name: str, value: int) -> None:
+        self._asset_name = asset_name
         self._value = value
 
     @property
-    def account_name(self) -> AccountName:
-        return AccountName(self._account_name)
+    def asset_name(self) -> AssetName:
+        return AssetName(self._asset_name)
 
     @property
     def value(self) -> Money:
         return Money(self._value)
 
 
-def revalue(cent_amount: int, account_name: str) -> None:
+def revalue(cent_amount: int, asset_name: str) -> None:
     """
     Revalues an asset to reflect it's current worth.
     """
     db = Database(database_path)
     with Session(db.engine) as session:
-        request = RevalueAccountRequest(account_name, cent_amount)
-        accounts = Accounts(session)
-        service = RevalueAccountService(accounts)
+        request = RevalueAssetRequest(asset_name, cent_amount)
+        assets = Assets(session)
+        service = RevalueAssetService(assets, event_log=pastperfect.Events(session))
         service.execute(request)
         session.commit()
 
 
 def reset() -> None:
     """
     Resets the application by removing the database.
     """
     db = Database(database_path)
     db.remove()
 
 
 class RequestImportTransactions(ImportTransactionsRequester):
-    def __init__(self, account_name: str) -> None:
-        self._account_name = account_name
+    def __init__(self, asset_name: str) -> None:
+        self._asset_name = asset_name
 
     @property
-    def account_name(self) -> AccountName:
-        return AccountName(self._account_name)
+    def asset_name(self) -> AssetName:
+        return AssetName(self._asset_name)
 
 
-def import_file(file_path: Path, account_name: str) -> None:
+def import_file(file_path: Path, asset_name: str) -> None:
     """
     Imports a file with all the transactions for a specific asset.
     """
     db = Database(database_path)
     with Session(db.engine) as session:
         gateway_cgd = GatewayCGDFile(file_path)
         transactions = Transactions(session)
-        accounts = Accounts(session)
-        service = ImportTransactionsService(gateway_cgd, transactions, accounts)
-        request = RequestImportTransactions(account_name)
+        assets = Assets(session)
+        service = ImportTransactionsService(
+            gateway_cgd, transactions, assets, event_log=pastperfect.Events(session)
+        )
+        request = RequestImportTransactions(asset_name)
         service.execute(request)
         session.commit()
 
 
-class DepositRequest(DepositIntoAccountRequester):
+class DepositRequest(DepositIntoAssetRequester):
     def __init__(
-        self, cent_amount: int, account_name: str, comment: Optional[str] = None
+        self, cent_amount: int, asset_name: str, comment: Optional[str] = None
     ) -> None:
         self._cent_amount = cent_amount
-        self._account_name = account_name
+        self._asset_name = asset_name
         self._comment = comment
 
     @property
     def amount(self) -> Money:
         return Money(self._cent_amount)
 
     @property
     def comment(self) -> Optional[Comment]:
         return Comment(self._comment) if self._comment else None
 
     @property
-    def account_name(self) -> AccountName:
-        return AccountName(self._account_name)
+    def asset_name(self) -> AssetName:
+        return AssetName(self._asset_name)
 
 
-def deposit(cent_amount: int, account_name: str, comment: Optional[str] = None) -> None:
+def deposit(cent_amount: int, asset_name: str, comment: Optional[str] = None) -> None:
     """
     Appreciate an asset by increasing it's value.
     """
     with Session(Database(database_path).engine) as session:
-        accounts = Accounts(session)
-        request = DepositRequest(cent_amount, account_name, comment)
-        service = DepositIntoAccountService(accounts)
+        assets = Assets(session)
+        request = DepositRequest(cent_amount, asset_name, comment)
+        service = DepositIntoAssetService(assets, event_log=pastperfect.Events(session))
         service.execute(request)
 
         session.commit()
 
 
-def transfer(cent_amount: int, from_account_name: str, to_account_name: str) -> None:
+def transfer(cent_amount: int, from_asset_name: str, to_asset_name: str) -> None:
     """
     Transfers value from an asset to another asset.
     """
     with Session(Database(database_path).engine) as session:
-        accounts = Accounts(session)
-        request = DepositRequest(cent_amount, from_account_name)
-        service = DepositIntoAccountService(accounts)
+        assets = Assets(session)
+        request = DepositRequest(cent_amount, from_asset_name)
+        service = DepositIntoAssetService(assets, event_log=pastperfect.Events(session))
         service.execute(request)
 
-        request = DepositRequest(-cent_amount, to_account_name)
-        service = DepositIntoAccountService(accounts)
+        request = DepositRequest(-cent_amount, to_asset_name)
+        service = DepositIntoAssetService(assets, event_log=pastperfect.Events(session))
         service.execute(request)
 
         session.commit()
 
 
-def show_accounts() -> None:
+def show_assets() -> None:
     """
     Shows all assets and their current value.
     """
     with Session(Database(database_path).engine) as session:
-        data = AccountsView(session).data
+        data = AssetsView(session).data
         if not data:
             return
 
         headers = ["Name", "Balance", "Status", "Comment"]
         lines = gogotable(headers, data)
         for line in lines:
             print(line)
 
 
-class OpenAccountRequest(OpenAccountRequester):
+class OpenAssetRequest(OpenAssetRequester):
     def __init__(self, name: str) -> None:
-        self._name = AccountName(name)
+        self._name = AssetName(name)
 
     @property
-    def account_name(self) -> AccountName:
+    def asset_name(self) -> AssetName:
         return self._name
 
 
-def open_account(name: str) -> None:
+def open_asset(name: str) -> None:
     """
     Creates a new asset.
     """
     with Session(Database(database_path).engine) as session:
-        accounts = Accounts(session)
-        request = OpenAccountRequest(name)
+        assets = Assets(session)
+        request = OpenAssetRequest(name)
         try:
-            OpenAccountService(accounts).execute(request)
-        except AccountAlreadyExistsError as e:
+            AcquireAssetService(assets, event_log=pastperfect.Events(session)).execute(
+                request
+            )
+        except AssetAlreadyExistsError as e:
             print(str(e))
             return
 
         session.commit()
 
 
-class CloseAccountRequest(CloseAccountRequester):
-    def __init__(self, account_name: str) -> None:
-        self._account_name = account_name
+class DivestAssetRequest(DivestAssetRequester):
+    def __init__(self, asset_name: str) -> None:
+        self._asset_name = asset_name
 
     @property
-    def account_name(self) -> AccountName:
-        return AccountName(self._account_name)
+    def asset_name(self) -> AssetName:
+        return AssetName(self._asset_name)
 
 
-def close_account(name: str) -> None:
+def divest_asset(name: str) -> None:
     """
     Divests an asset from your wealth but the keeping it's history.
     """
     with Session(Database(database_path).engine) as session:
-        accounts = Accounts(session)
-        request = CloseAccountRequest(name)
-        CloseAccountService(accounts).execute(request)
+        assets = Assets(session)
+        request = DivestAssetRequest(name)
+        DivestAssetService(assets, event_log=pastperfect.Events(session)).execute(
+            request
+        )
         session.commit()
 
 
-class DeleteAccountRequest(DeleteAccountRequester):
-    def __init__(self, account_name: str) -> None:
-        self._account_name = account_name
+class DeleteAssetRequest(DeleteAssetRequester):
+    def __init__(self, asset_name: str) -> None:
+        self._asset_name = asset_name
 
     @property
-    def account_name(self) -> AccountName:
-        return AccountName(self._account_name)
+    def asset_name(self) -> AssetName:
+        return AssetName(self._asset_name)
 
 
-def delete_account(name: str) -> None:
+def delete_asset(name: str) -> None:
     """
     Completely deletes an asset.
     """
     with Session(Database(database_path).engine) as session:
-        accounts = Accounts(session)
-        request = DeleteAccountRequest(name)
-        DeleteAccountService(accounts).execute(request)
+        assets = Assets(session)
+        request = DeleteAssetRequest(name)
+        DeleteAssetService(assets, event_log=pastperfect.Events(session)).execute(
+            request
+        )
         session.commit()
```

### Comparing `profitpulse-1.6.0/src/profitpulse/cli/main.py` & `profitpulse-2.0.0/src/profitpulse/cli/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,40 +5,37 @@
 from datetime import datetime
 from importlib.metadata import version as get_version
 from pathlib import Path
 from typing import Optional
 
 import typer
 
-from profitpulse.cli.adapters import (
-    close_account,
+from profitpulse.cli.adapters import (  # delete_asset,; show_assets,; transfer,
     database_path,
-    delete_account,
     deposit,
+    divest_asset,
     import_file,
-    open_account,
+    open_asset,
     pulse,
     report,
     reset,
     revalue,
-    show_accounts,
-    transfer,
 )
 from profitpulse.infrastructure.migrations import migrate_database  # type: ignore
 
 profitpulse_app = typer.Typer(
     add_completion=False,
     help="Profitpulse helps you manage your personal finances.",
 )
 
-profitpulse_accounts_app = typer.Typer()
+profitpulse_assets_app = typer.Typer()
 profitpulse_app.add_typer(
-    profitpulse_accounts_app,
-    name="accounts",
-    help="Handles accounts",
+    profitpulse_assets_app,
+    name="assets",
+    help="Handles assets",
 )
 
 
 @profitpulse_app.command(name="version", help="Shows the current profitpulse version")
 def version() -> None:
     migrate_database(database_path)
     typer.echo(get_version("profitpulse"))
@@ -53,31 +50,31 @@
 @profitpulse_app.command(
     name="revalue", help="Revalues an asset to reflect it's current worth"
 )
 def revalue_(
     cent_amount: int = typer.Argument(
         0, help="Amount to deposit in cents", metavar="AMOUNT"
     ),
-    account_name: str = typer.Argument(
-        "", help="Name of the account", metavar='"ACCOUNT NAME"'
+    asset_name: str = typer.Argument(
+        "", help="Name of the asset", metavar='"ASSET NAME"'
     ),
 ) -> None:
     migrate_database(database_path)
-    revalue(cent_amount, account_name)
+    revalue(cent_amount, asset_name)
 
 
 @profitpulse_app.command(name="import", help="Import transactions for expense tracking")
 def import_(
     file_path: Path,
-    account_name: str = typer.Argument(
-        "", help="Name of the account", metavar='"ACCOUNT NAME"'
+    asset_name: str = typer.Argument(
+        "", help="Name of the asset", metavar='"ASSET NAME"'
     ),
 ) -> None:
     migrate_database(database_path)
-    import_file(file_path, account_name)
+    import_file(file_path, asset_name)
 
 
 @profitpulse_app.command(name="report", help="Builds reports according to filters")
 def report_(
     seller: Optional[str] = typer.Option(default="", help="Filters report by Seller"),
     since: Optional[datetime] = typer.Option(
         default=None, help="Show report since specified date"
@@ -98,86 +95,80 @@
     migrate_database(database_path)
     if not delete_information:
         raise typer.Abort()
 
     reset()
 
 
-@profitpulse_app.command(name="deposit", help="Deposits money into an account")
+@profitpulse_app.command(name="deposit", help="Deposits money into an asset")
 def deposit_(
     cent_amount: int = typer.Argument(
         0, help="Amount to deposit in cents", metavar="AMOUNT"
     ),
-    account_name: str = typer.Argument(
-        "", help="Name of the account", metavar='"ACCOUNT NAME"'
+    asset_name: str = typer.Argument(
+        "", help="Name of the asset", metavar='"ASSET NAME"'
     ),
     comment: Optional[str] = typer.Option(
         default=None, help="Comment to add to the transaction"
     ),
 ) -> None:
     migrate_database(database_path)
-    deposit(cent_amount, account_name, comment=comment)
+    deposit(cent_amount, asset_name, comment=comment)
 
 
-@profitpulse_app.command(name="withdraw", help="Withdraws money from an account")
-def withdraw_(
-    cent_amount: int = typer.Argument(
-        0, help="Amount to withdraw in cents", metavar="AMOUNT"
-    ),
-    account_name: str = typer.Argument(
-        "", help="Name of the account", metavar='"ACCOUNT NAME"'
-    ),
-) -> None:
-    migrate_database(database_path)
-    deposit(-cent_amount, account_name)
+# @profitpulse_app.command(name="withdraw", help="Withdraws money from an asset")
+# def withdraw_(
+#     cent_amount: int = typer.Argument(
+#         0, help="Amount to withdraw in cents", metavar="AMOUNT"
+#     ),
+#     asset_name: str = typer.Argument(
+#         "", help="Name of the asset", metavar='"ASSET NAME"'
+#     ),
+# ) -> None:
+#     migrate_database(database_path)
+#     deposit(-cent_amount, asset_name)
+
+
+# @profitpulse_app.command(name="transfer", help="Transfers money between assets")
+# def transfer_(
+#     cent_amount: int = typer.Argument(
+#         0, help="Amount to transfer in cents", metavar="AMOUNT"
+#     ),
+#     from_asset_name: str = typer.Argument(
+#         "", help="Name of the asset to transfer from", metavar='"ASSET NAME"'
+#     ),
+#     to_asset_name: str = typer.Argument(
+#         "", help="Name of the asset to transfer to", metavar='"ASSET NAME"'
+#     ),
+# ) -> None:
+#     migrate_database(database_path)
+#     transfer(cent_amount, from_asset_name, to_asset_name)
+
+
+# @profitpulse_assets_app.command(name="show", help="Shows existing assets")
+# def show() -> None:
+#     migrate_database(database_path)
+#     show_assets()
 
 
-@profitpulse_app.command(name="transfer", help="Transfers money between accounts")
-def transfer_(
-    cent_amount: int = typer.Argument(
-        0, help="Amount to transfer in cents", metavar="AMOUNT"
-    ),
-    from_account_name: str = typer.Argument(
-        "", help="Name of the account to transfer from", metavar='"ACCOUNT NAME"'
-    ),
-    to_account_name: str = typer.Argument(
-        "", help="Name of the account to transfer to", metavar='"ACCOUNT NAME"'
-    ),
-) -> None:
-    migrate_database(database_path)
-    transfer(cent_amount, from_account_name, to_account_name)
-
-
-@profitpulse_accounts_app.command(name="show", help="Shows existing accounts")
-def show() -> None:
-    migrate_database(database_path)
-    show_accounts()
-
-
-@profitpulse_accounts_app.command(name="open", help="Opens a new account")
+@profitpulse_assets_app.command(name="open", help="Opens a new asset")
 def open_(
-    name: str = typer.Argument(
-        "", help="Name of the account", metavar='"ACCOUNT NAME"'
-    ),
+    name: str = typer.Argument("", help="Name of the asset", metavar='"ASSET NAME"'),
 ) -> None:
     migrate_database(database_path)
-    open_account(name)
+    open_asset(name)
 
 
-@profitpulse_accounts_app.command(name="close", help="Closes an account")
-def close_(
-    name: str = typer.Argument(
-        "", help="Name of the account", metavar='"ACCOUNT NAME"'
-    ),
+@profitpulse_assets_app.command(name="divest", help="Divests an asset")
+def divest_(
+    name: str = typer.Argument("", help="Name of the asset", metavar='"ASSET NAME"'),
 ) -> None:
     migrate_database(database_path)
-    close_account(name)
+    divest_asset(name)
 
 
-@profitpulse_accounts_app.command(name="delete", help="Deletes an account")
-def delete_(
-    name: str = typer.Argument(
-        "", help="Name of the account", metavar='"ACCOUNT NAME"'
-    ),
-) -> None:
-    migrate_database(database_path)
-    delete_account(name)
+# @profitpulse_assets_app.command(name="delete", help="Deletes an asset")
+# def delete_(
+#     name: str = typer.Argument("", help="Name of the asset", metavar='"ASSET NAME"'),
+# ) -> None:
+#     migrate_database(database_path)
+#     delete_asset(name)
```

### Comparing `profitpulse-1.6.0/src/profitpulse/data/pulse_view.py` & `profitpulse-2.0.0/src/profitpulse/data/pulse_view.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 import typing
 
 import pastperfect
 from sqlalchemy import text
 
-from profitpulse.data.accounts import DIVESTED, PulseEvent, status_from_value
-from profitpulse.data.views import View
+from profitpulse.data.assets import DIVESTED, status_from_value
+from profitpulse.data.data import View
 from profitpulse.lib.money import Money
+from profitpulse.services.deposit_into_asset import ASSET_DEPOSITED
+from profitpulse.services.revalue_asset import ASSET_REVALUED
 
 
 class PulseView(View):
     def __init__(self, session: typing.Any):
         self._session = session
 
     @property
-    def data(self) -> typing.Any:
+    def data(self) -> typing.Any:  # noqa
         sql_stmt = """SELECT name, status as name FROM account ORDER BY id ASC"""
-        accounts = self._session.execute(text(sql_stmt))
+        assets = self._session.execute(text(sql_stmt))
 
         events = pastperfect.Events(self._session)
 
         results = []
-        for account in accounts:
-            account_name = account[0]
-            status = account[1]
-            account_details = ["n/a"] * 5
+        total = Money(0)
+        for asset in assets:
+            asset_name = asset[0]
+            status = asset[1]
+            asset_details = ["n/a"] * 5
             invested = Money(0)
             current = Money(0)
 
             has_events = False
             for event in events:
                 has_events = True
+
+                # Current
                 if (
-                    event.name == PulseEvent.ACCOUNT_REVALUE
-                    and event.data.get("name") == account_name
-                ):
-                    current = Money(event.data.get("balance"))
-                    continue
+                    event.name == ASSET_REVALUED or event.name == ASSET_DEPOSITED
+                ) and event.data.get("name") == asset_name:
+                    current = current + Money(event.data.get("balance"))
 
+                # Invested
                 if (
-                    event.name == PulseEvent.MONEY_DEPOSIT
-                    and event.data.get("name") == account_name
+                    event.name == ASSET_DEPOSITED
+                    and event.data.get("name") == asset_name
                 ):
-                    invested = invested + Money(event.data.get("balance"))
+                    invested = invested + Money(event.data.get("balance", 0))
 
-            account_details[0] = account_name
-            account_details[1] = status_from_value(status)
+            asset_details[0] = asset_name
+            asset_details[1] = status_from_value(status)
             if not has_events:
-                results.append(account_details)
+                results.append(asset_details)
                 continue
 
-            account_details[2] = str(invested)
-            account_details[3] = str(current)
+            asset_details[2] = str(invested)
+            asset_details[3] = str(current)
             if status == DIVESTED:
-                account_details[3] = "n/a"
-            account_details[4] = str(current - invested)
+                asset_details[3] = "n/a"  # TODO: presentation
+            else:
+                total = total + current
+            asset_details[4] = str(current - invested)
 
-            results.append(account_details)
+            results.append(asset_details)
 
-        return results
+        return {"total": str(total), "assets": results}
```

### Comparing `profitpulse-1.6.0/src/profitpulse/data/transactions.py` & `profitpulse-2.0.0/src/profitpulse/data/transactions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 import typing
 
 import pastperfect
 from turbofan.database import text
 
-from profitpulse.data.accounts import PulseEvent
-from profitpulse.lib.account_name import AccountName
+from profitpulse.lib.asset_name import AssetName
 from profitpulse.lib.transaction import Transaction
 from profitpulse.services.import_transactions import (
+    TRANSACTION_IMPORTED,
     ImportTransactionsTransactionCollector,
 )
 
 
 class Transactions(ImportTransactionsTransactionCollector):
     def __init__(self, session: typing.Any) -> None:
         self._session = session
 
-    def append(self, t: Transaction, account_name: AccountName) -> None:
+    def append(self, t: Transaction, asset_name: AssetName) -> None:
         """
         Append a transaction to the repository.
         """
 
-        # Get the account id by account name
+        # Get the asset id by asset name
         sql_statement = """
             SELECT id
               FROM account
              WHERE name = :name
         """
-        prepared_statement = text(sql_statement).bindparams(name=str(account_name))
+        prepared_statement = text(sql_statement).bindparams(name=str(asset_name))
         result = self._session.execute(prepared_statement)
-        account_id = result.fetchone()[0]
+        asset_id = result.fetchone()[0]
 
         # Insert the transaction
         sql_statement = """
             INSERT INTO balance (date_of_movement, description, value, origin, account_id)
-                 VALUES (:date_of_movement, :description, :value, :origin, :account_id)
+                 VALUES (:date_of_movement, :description, :value, :origin, :asset_id)
         """
         prepared_statement = text(sql_statement).bindparams(
             date_of_movement=str(t.date_of_movement),
             description=t.description,
             value=t.value,
             origin=t.origin,
-            account_id=account_id,
+            asset_id=asset_id,
         )
         self._session.execute(prepared_statement)
 
         events = pastperfect.Events(self._session)
         events.append(
             pastperfect.Event(
-                name=PulseEvent.TRANSACTION_IMPORTED,
+                name=TRANSACTION_IMPORTED,
                 data={
                     "value": int(str(t.value).replace(".", "")),
                     "date": str(
                         t.date_of_movement.date()
                     ),  # TODO: should not need date()
                     "description": t.description,
                 },
```

### Comparing `profitpulse-1.6.0/src/profitpulse/data/views.py` & `profitpulse-2.0.0/src/profitpulse/data/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,59 @@
-import abc
 import typing
 from datetime import datetime
 from typing import Any
 
 import pastperfect
 from turbofan.database import text
 
-from profitpulse.data import accounts as accounts_repository
-from profitpulse.data.accounts import PulseEvent
+from profitpulse.data import assets as assets_repository
+from profitpulse.data.data import View
 from profitpulse.lib.money import Money
+from profitpulse.services.deposit_into_asset import ASSET_DEPOSITED
+from profitpulse.services.import_transactions import TRANSACTION_IMPORTED
+from profitpulse.services.revalue_asset import ASSET_REVALUED
 
 
-class View(abc.ABC):
-    @property
-    @abc.abstractmethod
-    def data(self) -> Any: ...
-
-
-class AccountsView(View):
+class AssetsView(View):
     def __init__(self, session: typing.Any) -> None:
         self._session = session
 
     @property
     def data(self) -> Any:
         sql_stmt = """
           SELECT account.name as name,
                  account.status,
                  balance.description
             FROM account
        LEFT JOIN balance
               ON account.id = balance.account_id
         """
         rows = self._session.execute(text(sql_stmt))
-        accounts = list(rows)
+        assets = list(rows)
         events = pastperfect.Events(self._session)
 
         results = []
-        for account in accounts:
-            account_name = account[0]
-            account_details = [
-                account_name,
+        for asset in assets:
+            asset_name = asset[0]
+            asset_details = [
+                asset_name,
                 "0.00",
-                "Open" if account[1] == accounts_repository.ACTIVE else "Closed",
-                account[2] if account[2] else "",
+                "Open" if asset[1] == assets_repository.ACTIVE else "Closed",
+                asset[2] if asset[2] else "",
             ]
             total_balance = Money(0)
             for event in events:
                 if (
-                    event.name != PulseEvent.ACCOUNT_REVALUE
-                    or event.data.get("name") != account_name
-                ):
-                    continue
-
-                total_balance = Money(event.data.get("balance"))
+                    event.name == ASSET_DEPOSITED or event.name == ASSET_REVALUED
+                ) and event.data.get("name") == asset_name:
+                    total_balance = total_balance + Money(event.data.get("balance"))
 
-            account_details[1] = str(total_balance)
+            asset_details[1] = str(total_balance)
 
-            results.append(account_details)
+            results.append(asset_details)
 
         return results
 
 
 class TransactionsView(View):
     def __init__(
         self,
@@ -81,15 +74,15 @@
         """
 
         if not self._seller:
             events = pastperfect.Events(self._session)
             total_money = Money(0)
             transactions = []
             for event in events:
-                if event.name != PulseEvent.TRANSACTION_IMPORTED:
+                if event.name != TRANSACTION_IMPORTED:
                     continue
 
                 date_of_transaction = datetime.strptime(event.data["date"], "%Y-%m-%d")
                 if self._since:
                     if date_of_transaction < self._since:
                         continue
```

### Comparing `profitpulse-1.6.0/src/profitpulse/data/views_test.py` & `profitpulse-2.0.0/src/profitpulse/data/views_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 from datetime import datetime
 
 import pastperfect
 import pytest
 from turbofan.database import text
 
-from profitpulse.data.accounts import PulseEvent
-from profitpulse.data.views import AccountsView, TransactionsView
+from profitpulse.data.views import AssetsView, TransactionsView
 from profitpulse.lib.money import Money
+from profitpulse.services.import_transactions import TRANSACTION_IMPORTED
 
 
-class TestAccountsView:
+class TestAssetsView:
     @pytest.mark.integration
-    def test_return_no_data_when_no_accounts(self, tmp_db_session):
-        assert AccountsView(tmp_db_session).data == []  # nosec
+    def test_return_no_data_when_no_assets(self, tmp_db_session):
+        assert AssetsView(tmp_db_session).data == []  # nosec
 
     @pytest.mark.integration
-    def test_return_one_account_when_one_account_exists(self, tmp_db_session):
-        DatabaseScenario(tmp_db_session).open_account(name="TheAccountName")
-        assert AccountsView(tmp_db_session).data == [  # nosec
-            ["TheAccountName", str(Money(0)), "Closed", ""]
+    def test_return_one_asset_when_one_asset_exists(self, tmp_db_session):
+        DatabaseScenario(tmp_db_session).open_asset(name="TheAssetName")
+        assert AssetsView(tmp_db_session).data == [  # nosec
+            ["TheAssetName", str(Money(0)), "Closed", ""]
         ]
 
 
 class DatabaseScenario:
     def __init__(self, session):
         self.session = session
-        self.account_id = None
+        self.asset_id = None
 
-    def log_transaction(self, description, value, date_of_movement, origin, account_id):
+    def log_transaction(self, description, value, date_of_movement, origin, asset_id):
         sql_statement = """
             INSERT INTO balance (description, value, date_of_movement, origin, account_id)
                  VALUES (:description, :value, :date_of_movement, :origin, :account_id)
         """
 
         prepared_statement = text(sql_statement).bindparams(
             description=description,
             value=value,
             date_of_movement=date_of_movement,
             origin=origin,
-            account_id=account_id,
+            account_id=asset_id,
         )
 
         self.session.execute(prepared_statement)
 
         events = pastperfect.Events(self.session)
         events.append(
             pastperfect.Event(
-                name=PulseEvent.TRANSACTION_IMPORTED,
+                name=TRANSACTION_IMPORTED,
                 data={
                     "value": value,
                     "date": date_of_movement,
                     "description": description,
                 },
             )
         )
 
         return self
 
-    def open_account(self, name):
+    def open_asset(self, name):
         sql_statement = "INSERT INTO account (name)VALUES (:name)"
         prepared_statement = text(sql_statement).bindparams(name=name)
         result = self.session.execute(prepared_statement)
-        self.account_id = result.lastrowid
+        self.asset_id = result.lastrowid
         return self
 
 
 class TestTransactionsView:
     @pytest.mark.integration
     def test_shown_no_transactions_on_empty_database(self, tmp_db_session):
         transactions, total = TransactionsView(tmp_db_session).data
@@ -78,16 +78,16 @@
         """
         Given a database with one transaction
         When the view is executed
         Then the transaction is shown
         """
 
         scenario = DatabaseScenario(tmp_db_session)
-        scenario.open_account("TheAccountName")
-        scenario.log_transaction("foo", 1, "2020-01-01", "foo", scenario.account_id)
+        scenario.open_asset("TheAssetName")
+        scenario.log_transaction("foo", 1, "2020-01-01", "foo", scenario.asset_id)
 
         transactions, total = TransactionsView(tmp_db_session).data
 
         assert transactions == [{"description": "foo", "value": "0.01"}]  # nosec
         assert total == "0.01"  # nosec
 
     @pytest.mark.integration
@@ -97,28 +97,28 @@
         """
         Given a database with multiple transactions
         When the view is executed
         Then the transactions are shown
         """
 
         scenario = DatabaseScenario(tmp_db_session)
-        scenario.open_account("TheAccountName")
+        scenario.open_asset("TheAssetName")
         scenario = scenario.log_transaction(
             "foo",
             1,
             "2020-01-01",
             "foo",
-            scenario.account_id,
+            scenario.asset_id,
         )
         scenario.log_transaction(
             "bar",
             2,
             "2020-01-01",
             "foo",
-            scenario.account_id,
+            scenario.asset_id,
         )
 
         transactions, total = TransactionsView(tmp_db_session).data
 
         assert transactions == [  # nosec
             {"description": "foo", "value": "0.01"},
             {"description": "bar", "value": "0.02"},
@@ -130,28 +130,28 @@
         """
         Given a database with multiple transactions
         When the view is executed with a since date
         Then the transactions since the given date are shown
         """
 
         scenario = DatabaseScenario(tmp_db_session)
-        scenario.open_account("TheAccountName")
+        scenario.open_asset("TheAssetName")
         scenario = scenario.log_transaction(
             "foo",
             1,
             "2020-01-01",
             "foo",
-            scenario.account_id,
+            scenario.asset_id,
         )
         scenario.log_transaction(
             "bar",
             2,
             "2020-01-02",
             "foo",
-            scenario.account_id,
+            scenario.asset_id,
         )
 
         transactions, total = TransactionsView(
             tmp_db_session, since=datetime.strptime("2020-01-02", "%Y-%m-%d")
         ).data
 
         assert transactions == [{"description": "bar", "value": "0.02"}]  # nosec
@@ -162,28 +162,28 @@
         """
         Given a database with multiple transactions
         When the view is executed with a on date
         Then the transactions on the given date are shown
         """
 
         scenario = DatabaseScenario(tmp_db_session)
-        scenario.open_account("TheAccountName")
+        scenario.open_asset("TheAssetName")
         scenario = scenario.log_transaction(
             "foo",
             1,
             "2020-01-01",
             "foo",
-            scenario.account_id,
+            scenario.asset_id,
         )
         scenario.log_transaction(
             "bar",
             2,
             "2020-01-02",
             "foo",
-            scenario.account_id,
+            scenario.asset_id,
         )
 
         transactions, total = TransactionsView(
             tmp_db_session,
             on=datetime.strptime("2020-01-01", "%Y-%m-%d"),
         ).data
 
@@ -195,26 +195,26 @@
         """
         Given a database with multiple transactions
         When the view is executed with a seller
         Then the total for the given seller is shown
         """
 
         scenario = DatabaseScenario(tmp_db_session)
-        scenario.open_account("TheAccountName")
+        scenario.open_asset("TheAssetName")
         scenario = scenario.log_transaction(
             "foo",
             1,
             "2020-01-01",
             "foo",
-            scenario.account_id,
+            scenario.asset_id,
         )
         scenario.log_transaction(
             "bar",
             2,
             "2020-01-02",
             "foo",
-            scenario.account_id,
+            scenario.asset_id,
         )
 
         transactions, total = TransactionsView(tmp_db_session, seller="foo").data
 
         assert total == 1.0  # nosec
```

### Comparing `profitpulse-1.6.0/src/profitpulse/gateways/cgdfile.py` & `profitpulse-2.0.0/src/profitpulse/gateways/cgdfile.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.6.0/src/profitpulse/gateways/cgdfile_test.py` & `profitpulse-2.0.0/src/profitpulse/gateways/cgdfile_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.6.0/src/profitpulse/infrastructure/migrations.py` & `profitpulse-2.0.0/src/profitpulse/infrastructure/migrations.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.6.0/src/profitpulse/lib/account_name.py` & `profitpulse-2.0.0/src/profitpulse/lib/asset_name.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-class AccountName:
+class AssetName:
     def __init__(self, name: str) -> None:
         if not name:
-            raise ValueError("Account name cannot be empty")
+            raise ValueError("Asset name cannot be empty")
         self._name: str = name
 
     def __str__(self) -> str:
         return self._name
 
     def __repr__(self) -> str:
-        return f"AccountName({self._name})"
+        return f"AssetName({self._name})"
 
     def __eq__(self, __value: object) -> bool:
-        if not isinstance(__value, AccountName):
+        if not isinstance(__value, AssetName):
             return NotImplemented
         return self._name == __value._name
 
     def __hash__(self) -> int:
         return hash((self._name,))
```

### Comparing `profitpulse-1.6.0/src/profitpulse/lib/money.py` & `profitpulse-2.0.0/src/profitpulse/lib/money.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from __future__ import annotations
 
 
 class Money:
     def __init__(self, cents: int) -> None:
+        if not cents:
+            cents = 0
         self._cents = cents
 
     def __eq__(self, __value: object) -> bool:
         if not isinstance(__value, Money):
             return False
         return self._cents == __value._cents
 
     def __str__(self) -> str:
         return f"{self._cents / 100:.2f}"
 
+    def __int__(self) -> int:
+        return self.cents
+
     def __repr__(self) -> str:
         return f"Money({self._cents})"
 
     def __add__(self, other: Money) -> Money:
         return Money(self._cents + other._cents)
 
     def __sub__(self, other: Money) -> Money:
```

### Comparing `profitpulse-1.6.0/src/profitpulse/migrations/0001 - Initial.sql` & `profitpulse-2.0.0/src/profitpulse/migrations/0001 - Initial.sql`

 * *Files identical despite different names*

### Comparing `profitpulse-1.6.0/src/profitpulse/services/import_transactions_test.py` & `profitpulse-2.0.0/src/profitpulse/services/import_transactions_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,71 @@
 # type: ignore
 import pytest
 
-from profitpulse.lib.account import Account
-from profitpulse.lib.account_name import AccountName
-from profitpulse.services.deposit_into_account import AccountNotFoundError
+from profitpulse.lib.asset import Asset
+from profitpulse.lib.asset_name import AssetName
+from profitpulse.services.deposit_into_asset import AssetNotFoundError
 from profitpulse.services.import_transactions import ImportTransactionsService
 
 
-class AccountsStub:
-    def __getitem__(self, account_name: AccountName) -> Account:
-        return Account(account_name)
+class AssetsStub:
+    def __getitem__(self, asset_name: AssetName) -> Asset:
+        return Asset(asset_name)
 
 
 class RequestStub:
     @property
-    def account_name(self) -> AccountName:
-        return AccountName("TheAccountName")
+    def asset_name(self) -> AssetName:
+        return AssetName("TheAssetName")
 
 
 def test_append_zero_transactions_when_no_transactions_to_append() -> None:
     request = RequestStub()
-    accounts = AccountsStub()
+    assets = AssetsStub()
     source_transactions = []
     transactions = []
-    service = ImportTransactionsService(
-        source_transactions,
-        transactions,
-        accounts,
-    )
+    service = ImportTransactionsService(source_transactions, transactions, assets, [])
 
     service.execute(request)
 
     assert len(transactions) == 0  # nosec
 
 
 class TransactionsStub:
     def __init__(self) -> None:
         self._transactions = []  # type: ignore
 
-    def append(self, transaction, account_name: AccountName):
+    def append(self, transaction, asset_name: AssetName):
         self._transactions.append(transaction)
 
     def __len__(self):
         return len(self._transactions)
 
 
 def test_append_one_transaction_when_one_transaction_available_in_source():
     request = RequestStub()
-    accounts = AccountsStub()
+    assets = AssetsStub()
     source_transactions = [{}]
     transactions = TransactionsStub()
-    service = ImportTransactionsService(
-        source_transactions,
-        transactions,
-        accounts,
-    )
+    service = ImportTransactionsService(source_transactions, transactions, assets, [])
 
     service.execute(request)
 
     assert len(transactions) == 1  # nosec
 
 
-class AccountNotFounStub:
+class AssetNotFounStub:
     def __getitem__(self, _):
         raise KeyError
 
 
-def test_raise_error_if_account_not_found() -> None:
+def test_raise_error_if_asset_not_found() -> None:
     request = RequestStub()
-    accounts = AccountNotFounStub()
+    assets = AssetNotFounStub()
     transactions = []
     source_transactions = [{}]
-    service = ImportTransactionsService(
-        source_transactions,
-        transactions,
-        accounts,
-    )
+    service = ImportTransactionsService(source_transactions, transactions, assets, [])
     with pytest.raises(
-        AccountNotFoundError,
-        match="Could not find an account with name 'TheAccountName'",
+        AssetNotFoundError,
+        match="Could not find an asset with name 'TheAssetName'",
     ):
         service.execute(request)
```

### Comparing `profitpulse-1.6.0/src/profitpulse/testrig/fixtures.py` & `profitpulse-2.0.0/src/profitpulse/testrig/fixtures.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.6.0/src/profitpulse/testrig/scenario.py` & `profitpulse-2.0.0/src/profitpulse/testrig/scenario.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,96 +7,96 @@
 
 runner = CliRunner(mix_stderr=False)
 
 
 class CLIScenario:
     """
     Builds scenarios up on the tests can be run and evaluates the result taking
-    the context (CLI) into account.
+    the context (CLI) into asset.
     """
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}"
 
     def __init__(self, *_, **__) -> None:
         self._app = profitpulse_app
 
-    # Account management -----------------------------------------------------------------------------------------------
+    # Asset management -----------------------------------------------------------------------------------------------
 
-    def show_accounts(self):
+    def show_assets(self):
         """
-        Shows all the accounts and their current balance.
+        Shows all the assets and their current balance.
         """
-        result = runner.invoke(self._app, ["accounts", "show"], catch_exceptions=False)
+        result = runner.invoke(self._app, ["assets", "show"], catch_exceptions=False)
         assert result.exit_code == 0, result.stderr  # nosec
 
         return result.stdout
 
-    expect_accounts__first_usage = ""
+    expect_assets__first_usage = ""
 
-    def open_account(self, account_name):
+    def open_asset(self, asset_name):
         """
-        Opens a new account.
+        Opens a new asset.
         """
 
         result = runner.invoke(
-            self._app, ["accounts", "open", account_name], catch_exceptions=False
+            self._app, ["assets", "open", asset_name], catch_exceptions=False
         )
         assert result.exit_code == 0, result.stderr  # nosec
 
-    def divest(self, account_name: str) -> None:
+    def divest(self, asset_name: str) -> None:
         result = runner.invoke(
-            self._app, ["accounts", "close", account_name], catch_exceptions=False
+            self._app, ["assets", "divest", asset_name], catch_exceptions=False
         )
         assert result.exit_code == 0, result.stderr  # nosec
         assert result.stdout == "", result.stdout  # nosec
 
-    def delete_account(self, account_name: str) -> None:
+    def delete_asset(self, asset_name: str) -> None:
         """
-        Deletes an account.
+        Deletes an asset.
         """
         result = runner.invoke(
-            self._app, ["accounts", "delete", account_name], catch_exceptions=False
+            self._app, ["assets", "delete", asset_name], catch_exceptions=False
         )
         assert result.exit_code == 0, result.stderr  # nosec
 
     # Money transactions  ----------------------------------------------------------------------------------------------
 
     def deposit(
-        self, cent_amount: int, account_name: str, comment: Optional[str] = None
+        self, cent_amount: int, asset_name: str, comment: Optional[str] = None
     ) -> None:
-        args = ["deposit", str(cent_amount), account_name]
+        args = ["deposit", str(cent_amount), asset_name]
         if comment:
             args.append("--comment")
             args.append(comment)
         result = runner.invoke(self._app, args, catch_exceptions=False)
         assert result.exit_code == 0, result.stderr  # nosec
 
-    def withdraw(self, cent_amount: int, account_name: str) -> None:
+    def withdraw(self, cent_amount: int, asset_name: str) -> None:
         result = runner.invoke(
             self._app,
-            ["withdraw", str(cent_amount), account_name],
+            ["withdraw", str(cent_amount), asset_name],
             catch_exceptions=False,
         )
         assert result.exit_code == 0, result.stderr  # nosec
 
-    def transfer(self, amount: int, from_account: str, to_account: str):
+    def transfer(self, amount: int, from_asset: str, to_asset: str):
         result = runner.invoke(
             self._app,
-            ["transfer", str(amount), from_account, to_account],
+            ["transfer", str(amount), from_asset, to_asset],
             catch_exceptions=False,
         )
         assert result.exit_code == 0, result.stderr  # nosec
         return result.stdout
 
     # Reports ----------------------------------------------------------------------------------------------------------
 
-    def revalue(self, amount: int, account_name: str):
+    def revalue(self, amount: int, asset_name: str):
         result = runner.invoke(
-            self._app, ["revalue", str(amount), account_name], catch_exceptions=False
+            self._app, ["revalue", str(amount), asset_name], catch_exceptions=False
         )
         assert result.exit_code == 0, result.stderr  # nosec
         return result.stdout
 
     def pulse(self):
         """
         Shows a global view of the user finances.
@@ -127,15 +127,15 @@
     def current_month(self) -> str:
         """
         Returns the current month of the imported transactions.
         """
         # This is one of the months defined in the fixture file comprovativo_cgd.csv
         return "8"
 
-    def import_transactions(self, transactions_file: str, account_name: str):
+    def import_transactions(self, transactions_file: str, asset_name: str):
         result = runner.invoke(
             self._app,
-            ["import", str(transactions_file), account_name],
+            ["import", str(transactions_file), asset_name],
             catch_exceptions=False,
         )
         assert result.exit_code == 0, result.stderr  # nosec
         return result.stdout
```

### Comparing `profitpulse-1.6.0/PKG-INFO` & `profitpulse-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profitpulse
-Version: 1.6.0
+Version: 2.0.0
 Summary: Manage your personal finances
 Home-page: https://github.com/luistm/profitpulse
 License: MIT
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Maintainer: Luís Miranda
 Maintainer-email: luistm@gmail.com
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: gogotable (>=0.0.3,<0.0.4)
-Requires-Dist: pastperfect (>=0.0.2,<0.0.3)
+Requires-Dist: pastperfect (>=0.1.0,<0.2.0)
 Requires-Dist: pendulum (>=3.0.0,<4.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: turbofan (>=0.2.0,<0.3.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Repository, https://github.com/luistm/profitpulse
 Description-Content-Type: text/markdown
```

