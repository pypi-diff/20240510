# Comparing `tmp/spond_classes-0.9.0.tar.gz` & `tmp/spond_classes-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spond_classes-0.9.0.tar", max compression
+gzip compressed data, was "spond_classes-0.9.1.tar", max compression
```

## Comparing `spond_classes-0.9.0.tar` & `spond_classes-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2065 2024-05-09 11:23:48.247557 spond_classes-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0    35823 2023-12-24 18:39:51.814809 spond_classes-0.9.0/LICENSE
--rw-r--r--   0        0        0     1958 2024-05-09 11:23:48.252828 spond_classes-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3005 2024-05-09 11:09:44.224321 spond_classes-0.9.0/README.md
--rw-r--r--   0        0        0      222 2024-05-09 11:09:45.384084 spond_classes-0.9.0/spond_classes/__init__.py
--rw-r--r--   0        0        0     1795 2024-05-09 10:55:24.781772 spond_classes-0.9.0/spond_classes/event.py
--rw-r--r--   0        0        0     3402 2024-05-09 10:55:24.905214 spond_classes-0.9.0/spond_classes/group.py
--rw-r--r--   0        0        0     2258 2024-05-09 10:55:24.880009 spond_classes-0.9.0/spond_classes/member.py
--rw-r--r--   0        0        0      192 2024-05-09 10:54:57.747925 spond_classes-0.9.0/spond_classes/profile.py
--rw-r--r--   0        0        0        0 2023-12-24 18:39:51.816809 spond_classes-0.9.0/spond_classes/py.typed
--rw-r--r--   0        0        0      586 2024-05-09 10:55:24.805315 spond_classes-0.9.0/spond_classes/role.py
--rw-r--r--   0        0        0      619 2024-05-09 10:55:24.829755 spond_classes-0.9.0/spond_classes/subgroup.py
--rw-r--r--   0        0        0     3678 1970-01-01 00:00:00.000000 spond_classes-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2347 2024-05-10 17:17:47.482196 spond_classes-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0    35823 2023-12-24 18:39:51.814809 spond_classes-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1958 2024-05-10 17:15:32.076119 spond_classes-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3050 2024-05-10 16:56:05.204081 spond_classes-0.9.1/README.md
+-rw-r--r--   0        0        0      336 2024-05-10 17:06:49.043290 spond_classes-0.9.1/spond_classes/__init__.py
+-rw-r--r--   0        0        0     1855 2024-05-10 16:56:05.205083 spond_classes-0.9.1/spond_classes/event.py
+-rw-r--r--   0        0        0     3571 2024-05-09 12:56:02.077461 spond_classes-0.9.1/spond_classes/group.py
+-rw-r--r--   0        0        0     2319 2024-05-09 12:56:02.060549 spond_classes-0.9.1/spond_classes/member.py
+-rw-r--r--   0        0        0      233 2024-05-09 12:56:02.055035 spond_classes-0.9.1/spond_classes/profile.py
+-rw-r--r--   0        0        0        0 2023-12-24 18:39:51.816809 spond_classes-0.9.1/spond_classes/py.typed
+-rw-r--r--   0        0        0      590 2024-05-09 12:56:02.067547 spond_classes-0.9.1/spond_classes/role.py
+-rw-r--r--   0        0        0      618 2024-05-09 12:56:02.072953 spond_classes-0.9.1/spond_classes/subgroup.py
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 spond_classes-0.9.1/PKG-INFO
```

### Comparing `spond_classes-0.9.0/CHANGELOG.md` & `spond_classes-0.9.1/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project tries to adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Historic and pre-release versions aren't necessarily included.
 
 
+## [0.9.1] - 2024-05-10
+
+### Changed
+
+- Docstring and README improvements
+
+### Fixed
+
+- `Member`, `Role`, `Subgroup` were removed from in top-level namespace
+
+- Docstring and README errors
+
+
 ## [0.9.0] - 2024-05-09
 
 ### Changed
 
 - BREAKING CHANGES: Significantly revised API - see README for details.
 
 - Rewritten from scratch using Pydantic; much closer to API data structure
@@ -79,12 +92,13 @@
 - Enforce linting with isort, black and ruff in CI using GitHub Actions
 
 ### Changed
 
 - Update dev/test dependencies: ruff
 
 
+[0.9.1]: https://github.com/elliot-100/Spond-classes/compare/v0.9.0...v0.9.1
 [0.9.0]: https://github.com/elliot-100/Spond-classes/compare/v0.8.1...v0.9.0
 [0.8.1]: https://github.com/elliot-100/Spond-classes/compare/v0.8.0...v0.8.1
 [0.8.0]: https://github.com/elliot-100/Spond-classes/compare/v0.7.3...v0.8.0
 [0.7.3]: https://github.com/elliot-100/Spond-classes/compare/v0.7.2...v0.7.3
 [0.7.2]: https://github.com/elliot-100/Spond-classes/compare/v0.7.1...v0.7.2
```

### Comparing `spond_classes-0.9.0/LICENSE` & `spond_classes-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spond_classes-0.9.0/pyproject.toml` & `spond_classes-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spond-classes"
-version = "0.9.0"
+version = "0.9.1"
 description = "Experimental Python class abstraction layer for `spond` package."
 authors = ["elliot-100 <3186037+elliot-100@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/elliot-100/Spond-classes"
 repository = "https://github.com/elliot-100/Spond-classes"
 packages = [{include = "spond_classes"}]
 include = ["CHANGELOG.md"]
```

### Comparing `spond_classes-0.9.0/README.md` & `spond_classes-0.9.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -57,19 +57,19 @@
     for member in group.members_by_subgroup(group.subgroup_by_id(subgroup_id))
         print(f"{member.full_name} is in the {subgroup.name} subgroup")
 
 asyncio.run(main())
 ```
 ## Key features
 
-* Create `Group` class instance from the dict returned by the corresponding `spond`
-  method:
+* Create `Group` instance from the dict returned from the API by the corresponding
+  `Spond` method:
 
 ```
-spond_classes.Group()
+spond_classes.Group(**dict)
 ```
 
 * Then access class instance attributes and methods:
 
 ```
 Group.uid: str
 Group.members: list[Member]
@@ -102,26 +102,26 @@
 Role.uid: str
 Role.name: str
 
 Subgroup.uid: str
 Subgroup.name: str
 ```
 
-* Create `Event` class instance from the dict returned by the corresponding `Spond`
-  method:
+* Create `Event` instance from the dict returned from the API by the corresponding
+  `Spond` method:
 
 ```
 spond_classes.Event(**dict)
 ```
 
 * Then access attributes:
 
 ```
 Event.uid: str
 Event.heading: str
 Event.start_time: datetime
-Event.Responses.accepted_uids: list
-Event.Responses.declined_uids: list
-Event.Responses.unanswered_uids: list
-Event.Responses.waiting_list_uids: list
-Event.Responses.unconfirmed_uids: list
+Event.Responses.accepted_uids: list[str]
+Event.Responses.declined_uids: list[str]
+Event.Responses.unanswered_uids: list[str]
+Event.Responses.waiting_list_uids: list[str]
+Event.Responses.unconfirmed_uids: list[str]
 ```
```

### Comparing `spond_classes-0.9.0/spond_classes/event.py` & `spond_classes-0.9.1/spond_classes/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,32 +27,34 @@
     waiting_list_uids: list[str] = Field(alias="waitinglistIds")
     unconfirmed_uids: list[str] = Field(alias="unconfirmedIds")
 
 
 class Event(BaseModel):
     """Represents an event in the Spond system.
 
+    Events are retrieved from the 'events' API endpoint.
+
     Attributes
     ----------
     uid : str
         id of the Event.
         `id` in API, but `id` is a reserved term and the `spond` package uses `uid`.
     heading : str
         Heading/name of the Event.
         `heading` in API.
+    responses : Responses
     start_time : datetime.
         Datetime at which the Event starts.
         `startTimestamp` in API, but returns a datetime instead of a string.
-    responses : Responses
     """
 
     uid: str = Field(alias="id")
     heading: str
-    start_time: datetime = Field(alias="startTimestamp")
     responses: Responses
+    start_time: datetime = Field(alias="startTimestamp")
 
     def __str__(self) -> str:
         """Return simple human-readable description.
 
         Date is included because heading is unlikely to be unique.
         """
         return f"Event '{self.heading}' on {self.start_time.date()}"
```

### Comparing `spond_classes-0.9.0/spond_classes/group.py` & `spond_classes-0.9.1/spond_classes/group.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 from .role import Role
 from .subgroup import Subgroup
 
 
 class Group(BaseModel):
     """Represents a group in the Spond system.
 
-    A Group has zero, one or more Members.
+    Groups are retrieved from the 'groups' API endpoint.
+
+    A Group has zero, one or more nested Members.
+    A Group has zero, one or more nested Roles.
+    A Group has zero, one or more nested Subgroups.
 
     Attributes
     ----------
     uid : str
         id of the Group.
         'id' in API, but 'id' is a reserved term and the `spond` package uses `uid`.
     members : list[Member]
```

### Comparing `spond_classes-0.9.0/spond_classes/member.py` & `spond_classes-0.9.1/spond_classes/member.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 from .profile import Profile
 
 
 class Member(BaseModel):
     """Represents a member in the Spond system.
 
-    A Member is an individual's record within a Group.
+    A Member is an individual's group-specific record.
+    A Member is nested within a Group.
     A Member may have a nested Profile.
 
     Attributes
     ----------
     uid : str
         id of the Member.
         'id' in API, but 'id' is a reserved term and the `spond` package uses `uid`.
@@ -22,19 +23,19 @@
         'createdTime' in API, but returns a datetime instead of a string.
     email : str
         'email' in API.
     first_name : str
         'firstName' in API.
     last_name : str
         'lastName' in API.
-    phone_number : str
+    phone_number : str | None
         'phoneNumber' in API.
-    profile : Profile
+    profile : Profile | None
         `profile` in API.
-    role_uids : list[str]
+    role_uids : list[str] | None
         `roles` in API, but aliased here to avoid confusion with `Group.Roles'
     subgroup_uids : list[str]
         `subGroups` in API, but aliased here to avoid confusion with `Group.Subgroups'
 
     Properties
     ----------
     full_name : str
```

### Comparing `spond_classes-0.9.0/spond_classes/role.py` & `spond_classes-0.9.1/spond_classes/role.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pydantic import BaseModel, Field
 
 
 class Role(BaseModel):
     """Represents a role in the Spond system.
 
-    A Role belongs to one Group.
+    A Role is nested within a Group.
 
     Attributes
     ----------
     uid : str
         id of the Role.
         'id' in API, but 'id' is a reserved term and the `spond` package uses `uid`.
     name : str
```

### Comparing `spond_classes-0.9.0/spond_classes/subgroup.py` & `spond_classes-0.9.1/spond_classes/subgroup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Subgroup class."""
 
 from pydantic import BaseModel, Field
 
 
 class Subgroup(BaseModel):
-    """Subgroup.
+    """Represents a subgroup in the Spond system.
 
-    Belongs to one Group.
-    May contain zero, one or more SpondMembers.
+    A Subgroup is nested within a Group.
 
     Attributes
     ----------
     uid : str
         id of the Subgroup.
         'id' in API, but 'id' is a reserved term and the `spond` package uses `uid`.
     name : str
```

### Comparing `spond_classes-0.9.0/PKG-INFO` & `spond_classes-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spond-classes
-Version: 0.9.0
+Version: 0.9.1
 Summary: Experimental Python class abstraction layer for `spond` package.
 Home-page: https://github.com/elliot-100/Spond-classes
 License: GPL 3.0
 Author: elliot-100
 Author-email: 3186037+elliot-100@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -77,19 +77,19 @@
     for member in group.members_by_subgroup(group.subgroup_by_id(subgroup_id))
         print(f"{member.full_name} is in the {subgroup.name} subgroup")
 
 asyncio.run(main())
 ```
 ## Key features
 
-* Create `Group` class instance from the dict returned by the corresponding `spond`
-  method:
+* Create `Group` instance from the dict returned from the API by the corresponding
+  `Spond` method:
 
 ```
-spond_classes.Group()
+spond_classes.Group(**dict)
 ```
 
 * Then access class instance attributes and methods:
 
 ```
 Group.uid: str
 Group.members: list[Member]
@@ -122,27 +122,27 @@
 Role.uid: str
 Role.name: str
 
 Subgroup.uid: str
 Subgroup.name: str
 ```
 
-* Create `Event` class instance from the dict returned by the corresponding `Spond`
-  method:
+* Create `Event` instance from the dict returned from the API by the corresponding
+  `Spond` method:
 
 ```
 spond_classes.Event(**dict)
 ```
 
 * Then access attributes:
 
 ```
 Event.uid: str
 Event.heading: str
 Event.start_time: datetime
-Event.Responses.accepted_uids: list
-Event.Responses.declined_uids: list
-Event.Responses.unanswered_uids: list
-Event.Responses.waiting_list_uids: list
-Event.Responses.unconfirmed_uids: list
+Event.Responses.accepted_uids: list[str]
+Event.Responses.declined_uids: list[str]
+Event.Responses.unanswered_uids: list[str]
+Event.Responses.waiting_list_uids: list[str]
+Event.Responses.unconfirmed_uids: list[str]
 ```
```

