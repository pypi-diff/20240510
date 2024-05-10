# Comparing `tmp/mcc_api-1.1.1.tar.gz` & `tmp/mcc_api-1.1.2.tar.gz`

## Comparing `mcc_api-1.1.1.tar` & `mcc_api-1.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.1.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 mcc_api-1.1.1/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mcc_api-1.1.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 mcc_api-1.1.1/docs/conf.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mcc_api-1.1.1/docs/event.rst
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mcc_api-1.1.1/docs/index.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mcc_api-1.1.1/docs/island.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/__init__.py
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/event/__init__.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/event/enums.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/event/exceptions.py
--rw-r--r--   0        0        0    13133 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/event/responses.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/auth.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/directives.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/enums.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/scalars.py
--rw-r--r--   0        0        0    11084 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/types.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/run_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/test_event.py
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/test_halloffame.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/test_participants.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/test_rundown.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_event.json
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_halloffame.json
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_halloffame_game.json
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_participants.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_participants_team.json
--rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_rundown.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/404_halloffame_game.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/404_participants_team.json
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/404_rundown.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/429_ratelimit.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/island/__init__.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/island/test_schema.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.1.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mcc_api-1.1.1/LICENSE
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 mcc_api-1.1.1/README.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mcc_api-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 mcc_api-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.1.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 mcc_api-1.1.2/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mcc_api-1.1.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 mcc_api-1.1.2/docs/conf.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mcc_api-1.1.2/docs/event.rst
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mcc_api-1.1.2/docs/index.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mcc_api-1.1.2/docs/island.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/__init__.py
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/event/__init__.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/event/enums.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/event/exceptions.py
+-rw-r--r--   0        0        0    13133 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/event/responses.py
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/auth.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/directives.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/enums.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/scalars.py
+-rw-r--r--   0        0        0    15196 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/types.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/run_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/__init__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/test_event.py
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/test_halloffame.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/test_participants.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/test_rundown.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_event.json
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_halloffame.json
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_halloffame_game.json
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_participants.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_participants_team.json
+-rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_rundown.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/404_halloffame_game.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/404_participants_team.json
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/404_rundown.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/429_ratelimit.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/island/__init__.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/island/test_schema.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mcc_api-1.1.2/LICENSE
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 mcc_api-1.1.2/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mcc_api-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 mcc_api-1.1.2/PKG-INFO
```

### Comparing `mcc_api-1.1.1/.github/workflows/docs.yml` & `mcc_api-1.1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/.github/workflows/pypi_publish.yml` & `mcc_api-1.1.2/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/.github/workflows/tests.yml` & `mcc_api-1.1.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/docs/conf.py` & `mcc_api-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/docs/index.rst` & `mcc_api-1.1.2/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 .. image:: https://img.shields.io/pypi/v/mcc-api?label=🐍%20PyPI
    :alt: 🐍 PyPI
    :target: https://pypi.org/project/mcc-api/
 .. image:: https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.2-red
    :alt: 👑 Targeting Event API v1.3.2
    :target: https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.2
-.. image:: https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.02-aqua
-   :alt: 🏝️ Targeting Island API v24.05.02
-   :target: https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.02
+.. image:: https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.06-aqua
+   :alt: 🏝️ Targeting Island API v24.05.06
+   :target: https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.06
 
 A helper library for the `MC Championship <https://mcchampionship.com>`_ APIs
 (`Event <https://github.com/Noxcrew/mcchampionship-api>`_, inspired by `derNiklaas's <https://github.com/derNiklaas>`_
 `node-mcc-api <https://github.com/derNiklaas/node-mcc-api>`_ project, and
 `Island <https://github.com/Noxcrew/mccisland-api>`_).
 
 - Issues: `https://github.com/JamesMCo/python_mcc_api/issues <https://github.com/JamesMCo/python_mcc_api/issues>`_
```

### Comparing `mcc_api-1.1.1/mcc_api/event/__init__.py` & `mcc_api-1.1.2/mcc_api/event/__init__.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/mcc_api/event/enums.py` & `mcc_api-1.1.2/mcc_api/event/enums.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     MG_GRID_RUNNERS = auto()
     MG_MELTDOWN = auto()
     GLOBAL_STATISTICS = auto()
     LEGACY_STATISTICS = auto()
     MG_LOCKOUT_BINGO = auto()
     MG_FOOT_RACE = auto()
     MG_ROCKET_SPLEEF_OLD = auto()
+    MG_RAILROAD_RUSH = auto()
 
 
 class Team(UpperStrEnum):
     """Team identifiers accepted and returned by the MCC API."""
 
     RED = auto()
     ORANGE = auto()
```

### Comparing `mcc_api-1.1.1/mcc_api/event/exceptions.py` & `mcc_api-1.1.2/mcc_api/event/exceptions.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/mcc_api/event/responses.py` & `mcc_api-1.1.2/mcc_api/event/responses.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/mcc_api/island/__init__.py` & `mcc_api-1.1.2/mcc_api/island/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 schema = GraphQLSchema(
     query=query_type,
     directives=[*specified_directives, one_of_directive, spectaql_directive],
     types=[
         collections_type,
         crown_level_type,
         currency_type,
+        leaderboard_entry_type,
         party_type,
         player_type,
         progression_data_type,
         query_type,
         server_type,
         social_type,
         statistic_type,
@@ -31,14 +32,15 @@
         statistics_type,
         status_type,
         spectaqloption_type,
         trophy_data_type,
 
         game_enum,
         rank_enum,
+        rotation_enum,
         server_category_enum,
         trophy_category_enum,
     ]
 )
 
 _transport = RequestsHTTPTransport(
     url=__base_url,
```

### Comparing `mcc_api-1.1.1/mcc_api/island/auth.py` & `mcc_api-1.1.2/mcc_api/island/auth.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/mcc_api/island/directives.py` & `mcc_api-1.1.2/mcc_api/island/directives.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/mcc_api/island/enums.py` & `mcc_api-1.1.2/mcc_api/island/enums.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from graphql import GraphQLEnumType, GraphQLEnumValue
 
 
 __all__ = [
-    "game_enum", "rank_enum", "server_category_enum", "trophy_category_enum"
+    "game_enum", "rank_enum", "rotation_enum", "server_category_enum", "trophy_category_enum"
 ]
 
 game_enum = GraphQLEnumType(
     name="Game",
     description="A game.",
     values={
         "BATTLE_BOX": GraphQLEnumValue(
@@ -71,14 +71,42 @@
         "NOXCREW": GraphQLEnumValue(
             value="NOXCREW",
             description="The Noxcrew rank."
         )
     }
 )
 
+rotation_enum = GraphQLEnumType(
+    name="Rotation",
+    description="A rotation period.\n\n"
+                "Each period resets at 10AM UTC.",
+    values={
+        "DAILY": GraphQLEnumValue(
+            value="DAILY",
+            description="A daily rotation that resets."
+        ),
+        "WEEKLY": GraphQLEnumValue(
+            value="WEEKLY",
+            description="A weekly rotation that resets on Tuesdays."
+        ),
+        "MONTHLY": GraphQLEnumValue(
+            value="MONTHLY",
+            description="A monthly rotation that resets on the first day of every month."
+        ),
+        "YEARLY": GraphQLEnumValue(
+            value="YEARLY",
+            description="A yearly rotation that resets on the first day of every year."
+        ),
+        "LIFETIME": GraphQLEnumValue(
+            value="LIFETIME",
+            description="A lifetime rotation; a rotation period used to indicate something never rotates."
+        )
+    }
+)
+
 server_category_enum = GraphQLEnumType(
     name="ServerCategory",
     description="The category of a server.",
     values={
         "GAME": GraphQLEnumValue(
             value="GAME",
             description="A game server."
```

### Comparing `mcc_api-1.1.1/mcc_api/island/scalars.py` & `mcc_api-1.1.2/mcc_api/island/scalars.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/mcc_api/island/types.py` & `mcc_api-1.1.2/mcc_api/island/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 )
 
 
 __all__ = [
     "collections_type",
     "crown_level_type",
     "currency_type",
+    "leaderboard_entry_type",
     "party_type",
     "player_type",
     "progression_data_type",
     "query_type",
     "server_type",
     "social_type",
     "statistic_type",
@@ -88,14 +89,35 @@
         "silver": GraphQLField(
             GraphQLNonNull(GraphQLInt),
             description="The amount of silver the player currently has."
         )
     }
 )
 
+leaderboard_entry_type = GraphQLObjectType(
+    name="LeaderboardEntry",
+    description="An entry in a leaderboard.",
+    fields=lambda: {
+        "player": GraphQLField(
+            player_type,
+            description="The player who has this entry.\n\n"
+                        "This will be `null` if the player does not have the statistics enabled for the API.\n"
+                        "However, for Crown Level or Trophy count leaderboards, the player will not be `null`."
+        ),
+        "rank": GraphQLField(
+            GraphQLNonNull(GraphQLInt),
+            description="The rank for this entry."
+        ),
+        "value": GraphQLField(
+            GraphQLNonNull(GraphQLInt),
+            description="The value for this entry."
+        )
+    }
+)
+
 party_type = GraphQLObjectType(
     name="Party",
     description="A player's status within a party.",
     fields=lambda: {
         "active": GraphQLField(
             GraphQLNonNull(GraphQLBoolean),
             description="Whether the player is in an active party."
@@ -198,14 +220,45 @@
                     GraphQLNonNull(GraphQLString)
                 )
             }
         ),
         "statistics": GraphQLField(
             GraphQLNonNull(GraphQLList(GraphQLNonNull(statistic_type))),
             description="Returns a list of all known statistics."
+        ),
+        "statistic": GraphQLField(
+            statistic_type,
+            description="Returns a statistic by it's name.",
+            args={
+                "key": GraphQLArgument(
+                    GraphQLNonNull(GraphQLString)
+                )
+            }
+        ),
+        "nextRotation": GraphQLField(
+            GraphQLNonNull(datetime_scalar),
+            description="Returns when this rotation will next rotate.\n\n"
+                        "If the rotation is due the exact time this method is called, "
+                        "this method will return the next time that it will rotate.",
+            args={
+                "rotation": GraphQLArgument(
+                    GraphQLNonNull(rotation_enum)
+                )
+            }
+        ),
+        "previousRotation": GraphQLField(
+            GraphQLNonNull(datetime_scalar),
+            description="Returns when this rotation last rotated.\n\n"
+                        "If the rotation is due the exact time this method is called, "
+                        "this method will return the current time.",
+            args={
+                "rotation": GraphQLArgument(
+                    GraphQLNonNull(rotation_enum)
+                )
+            }
         )
     }
 )
 
 server_type = GraphQLObjectType(
     name="Server",
     description="A server on the network.",
@@ -247,14 +300,37 @@
         "forLeaderboard": GraphQLField(
             GraphQLNonNull(GraphQLBoolean),
             description="If this statistic generates leaderboards."
         ),
         "key": GraphQLField(
             GraphQLNonNull(GraphQLString),
             description="The key of the statistic."
+        ),
+        "leaderboard": GraphQLField(
+            GraphQLList(GraphQLNonNull(leaderboard_entry_type)),
+            description="Returns the leaderboard for this statistic in a given rotation.\n\n"
+                        "If this statistic does not generate leaderboards, "
+                        "or the statistic is not tracked for the provided rotation, this will return `null`.",
+            args={
+                "amount": GraphQLArgument(
+                    GraphQLNonNull(GraphQLInt),
+                    default_value=10
+                ),
+                "rotation": GraphQLArgument(
+                    GraphQLNonNull(rotation_enum),
+                    default_value=rotation_enum.values["LIFETIME"].value
+                )
+            }
+        ),
+        "rotations": GraphQLField(
+            GraphQLNonNull(GraphQLList(GraphQLNonNull(rotation_enum))),
+            description="The rotations for which this statistic is tracked.\n\n"
+                        "These are the rotations that can be used to generate leaderboards or fetch rotation values.\n"
+                        "Note that the `YEARLY` rotation never generates leaderboards, "
+                        "even if it is returned in this list."
         )
     }
 )
 
 statistic_value_result_type = GraphQLObjectType(
     name="StatisticValueResult",
     description="The result of fetching a value of a statistic.",
@@ -277,14 +353,31 @@
         "value": GraphQLField(
             statistic_value_result_type,
             description="Returns the raw value stored for this statistic.",
             args={
                 "statisticKey": GraphQLArgument(
                     GraphQLNonNull(GraphQLString)
                 )
+            },
+            deprecation_reason="This value is not backed by a rotation and will be removed. "
+                               "Use `rotationValue` instead."
+        ),
+        "rotationValue": GraphQLField(
+            GraphQLInt,
+            description="Returns the value stored for the given statistic in a rotation.\n\n"
+                        "The returned number will be `null` if the statistic does not track in the provided rotation, "
+                        "or if the statistic doesn't exist.",
+            args={
+                "rotation": GraphQLArgument(
+                    GraphQLNonNull(rotation_enum),
+                    default_value=rotation_enum.values["LIFETIME"].value
+                ),
+                "statisticKey": GraphQLArgument(
+                    GraphQLNonNull(GraphQLString)
+                )
             }
         )
     }
 )
 
 status_type = GraphQLObjectType(
     name="Status",
```

### Comparing `mcc_api-1.1.1/tests/run_tests.py` & `mcc_api-1.1.2/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/tests/event/test_event.py` & `mcc_api-1.1.2/tests/event/test_event.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/tests/event/test_halloffame.py` & `mcc_api-1.1.2/tests/event/test_halloffame.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/tests/event/test_participants.py` & `mcc_api-1.1.2/tests/event/test_participants.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/tests/event/test_rundown.py` & `mcc_api-1.1.2/tests/event/test_rundown.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/tests/event/mock_data/200_halloffame.json` & `mcc_api-1.1.2/tests/event/mock_data/200_halloffame.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/tests/event/mock_data/200_participants.json` & `mcc_api-1.1.2/tests/event/mock_data/200_participants.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/tests/event/mock_data/200_participants_team.json` & `mcc_api-1.1.2/tests/event/mock_data/200_participants_team.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/tests/event/mock_data/200_rundown.json` & `mcc_api-1.1.2/tests/event/mock_data/200_rundown.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/tests/island/test_schema.py` & `mcc_api-1.1.2/tests/island/test_schema.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/.gitignore` & `mcc_api-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/LICENSE` & `mcc_api-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/README.md` & `mcc_api-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Python MCC API
 
 [![🐍 PyPI](https://img.shields.io/pypi/v/mcc-api?label=🐍%20PyPI)](https://pypi.org/project/mcc-api/)
 [![👑 Targeting Event API v1.3.2](https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.2-red)](https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.2)
-[![🏝️ Targeting Island API v24.05.02](https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.02-aqua)](https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.02)
+[![🏝️ Targeting Island API v24.05.06](https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.06-aqua)](https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.06)
 
 A helper library for the [MC Championship](https://mcchampionship.com) APIs
 ([Event](https://github.com/Noxcrew/mcchampionship-api), inspired by [derNiklaas's](https://github.com/derNiklaas)
 [node-mcc-api](https://github.com/derNiklaas/node-mcc-api) project, and
 [Island](https://github.com/Noxcrew/mccisland-api)).
 
 - Issues: [https://github.com/JamesMCo/python_mcc_api/issues](https://github.com/JamesMCo/python_mcc_api/issues)
```

### Comparing `mcc_api-1.1.1/pyproject.toml` & `mcc_api-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.1/PKG-INFO` & `mcc_api-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mcc-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: Wrapper for the MC Championship API
 Project-URL: Repository, https://github.com/JamesMCo/python_mcc_api
 Project-URL: Issues, https://github.com/JamesMCo/python_mcc_api/issues
 Project-URL: Documentation, https://mrjamesco.uk/python_mcc_api
 Author-email: "James C." <james@cordon.click>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # Python MCC API
 
 [![🐍 PyPI](https://img.shields.io/pypi/v/mcc-api?label=🐍%20PyPI)](https://pypi.org/project/mcc-api/)
 [![👑 Targeting Event API v1.3.2](https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.2-red)](https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.2)
-[![🏝️ Targeting Island API v24.05.02](https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.02-aqua)](https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.02)
+[![🏝️ Targeting Island API v24.05.06](https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.06-aqua)](https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.06)
 
 A helper library for the [MC Championship](https://mcchampionship.com) APIs
 ([Event](https://github.com/Noxcrew/mcchampionship-api), inspired by [derNiklaas's](https://github.com/derNiklaas)
 [node-mcc-api](https://github.com/derNiklaas/node-mcc-api) project, and
 [Island](https://github.com/Noxcrew/mccisland-api)).
 
 - Issues: [https://github.com/JamesMCo/python_mcc_api/issues](https://github.com/JamesMCo/python_mcc_api/issues)
```

