# Comparing `tmp/chsu_schedule_api-1.2.1.tar.gz` & `tmp/chsu_schedule_api-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chsu_schedule_api-1.2.1.tar", max compression
+gzip compressed data, was "chsu_schedule_api-1.2.2.tar", max compression
```

## Comparing `chsu_schedule_api-1.2.1.tar` & `chsu_schedule_api-1.2.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      153 2024-03-28 22:56:25.487494 chsu_schedule_api-1.2.1/chsu_schedule_api/__init__.py
--rw-r--r--   0        0        0       86 2024-03-28 22:56:25.487494 chsu_schedule_api-1.2.1/chsu_schedule_api/api/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-16 12:26:44.074722 chsu_schedule_api-1.2.1/chsu_schedule_api/api/abc.py
--rw-r--r--   0        0        0     5980 2024-04-16 12:26:44.074722 chsu_schedule_api-1.2.1/chsu_schedule_api/api/api.py
--rw-r--r--   0        0        0      116 2024-03-28 22:56:25.488497 chsu_schedule_api-1.2.1/chsu_schedule_api/client/__init__.py
--rw-r--r--   0        0        0     1071 2024-03-28 22:56:25.488497 chsu_schedule_api-1.2.1/chsu_schedule_api/client/abc.py
--rw-r--r--   0        0        0     2065 2024-03-28 22:56:25.488497 chsu_schedule_api-1.2.1/chsu_schedule_api/client/aiohttp.py
--rw-r--r--   0        0        0      298 2024-03-28 22:56:25.488497 chsu_schedule_api-1.2.1/chsu_schedule_api/constants.py
--rw-r--r--   0        0        0      116 2024-03-28 22:56:25.488497 chsu_schedule_api-1.2.1/chsu_schedule_api/enums.py
--rw-r--r--   0        0        0      326 2024-04-16 12:26:44.076195 chsu_schedule_api-1.2.1/chsu_schedule_api/errors.py
--rw-r--r--   0        0        0      882 2024-04-16 12:26:44.076195 chsu_schedule_api-1.2.1/chsu_schedule_api/models/__init__.py
--rw-r--r--   0        0        0      302 2024-03-28 22:56:25.490518 chsu_schedule_api-1.2.1/chsu_schedule_api/models/auditorium.py
--rw-r--r--   0        0        0      208 2024-03-29 08:16:57.081988 chsu_schedule_api-1.2.1/chsu_schedule_api/models/base.py
--rw-r--r--   0        0        0      106 2024-03-28 22:56:25.490997 chsu_schedule_api-1.2.1/chsu_schedule_api/models/building.py
--rw-r--r--   0        0        0      411 2024-03-28 22:56:25.490997 chsu_schedule_api-1.2.1/chsu_schedule_api/models/department.py
--rw-r--r--   0        0        0      108 2024-03-28 22:56:25.491524 chsu_schedule_api-1.2.1/chsu_schedule_api/models/discipline.py
--rw-r--r--   0        0        0      356 2024-03-28 22:56:25.491524 chsu_schedule_api-1.2.1/chsu_schedule_api/models/student_group.py
--rw-r--r--   0        0        0      332 2024-03-28 22:56:25.491524 chsu_schedule_api-1.2.1/chsu_schedule_api/models/teacher.py
--rw-r--r--   0        0        0     2975 2024-04-16 12:36:49.734085 chsu_schedule_api-1.2.1/chsu_schedule_api/models/timetable.py
--rw-r--r--   0        0        0     1093 2024-03-28 22:56:25.486469 chsu_schedule_api-1.2.1/LICENSE
--rw-r--r--   0        0        0     1378 2024-04-16 12:40:58.517354 chsu_schedule_api-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2293 2024-04-16 12:26:44.073501 chsu_schedule_api-1.2.1/README.md
--rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 chsu_schedule_api-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      190 2024-05-09 23:11:38.332975 chsu_schedule_api-1.2.2/chsu_schedule_api/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-21 21:48:20.042901 chsu_schedule_api-1.2.2/chsu_schedule_api/api/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-21 21:48:20.042901 chsu_schedule_api-1.2.2/chsu_schedule_api/api/abc.py
+-rw-r--r--   0        0        0     6583 2024-05-01 14:24:54.808538 chsu_schedule_api-1.2.2/chsu_schedule_api/api/api.py
+-rw-r--r--   0        0        0      116 2024-04-21 21:48:20.043901 chsu_schedule_api-1.2.2/chsu_schedule_api/client/__init__.py
+-rw-r--r--   0        0        0     1071 2024-04-21 21:48:20.043901 chsu_schedule_api-1.2.2/chsu_schedule_api/client/abc.py
+-rw-r--r--   0        0        0     2065 2024-04-21 21:48:20.043901 chsu_schedule_api-1.2.2/chsu_schedule_api/client/aiohttp.py
+-rw-r--r--   0        0        0      298 2024-04-21 21:48:20.043901 chsu_schedule_api-1.2.2/chsu_schedule_api/constants.py
+-rw-r--r--   0        0        0      117 2024-04-30 20:48:12.729473 chsu_schedule_api-1.2.2/chsu_schedule_api/enums.py
+-rw-r--r--   0        0        0      326 2024-04-21 21:48:20.044901 chsu_schedule_api-1.2.2/chsu_schedule_api/errors.py
+-rw-r--r--   0        0        0      847 2024-05-09 22:41:10.334815 chsu_schedule_api-1.2.2/chsu_schedule_api/sync.py
+-rw-r--r--   0        0        0      882 2024-04-30 12:56:21.414625 chsu_schedule_api-1.2.2/chsu_schedule_api/types/__init__.py
+-rw-r--r--   0        0        0      449 2024-04-30 15:12:40.006923 chsu_schedule_api-1.2.2/chsu_schedule_api/types/auditorium.py
+-rw-r--r--   0        0        0      208 2024-04-21 21:48:20.044901 chsu_schedule_api-1.2.2/chsu_schedule_api/types/base.py
+-rw-r--r--   0        0        0      242 2024-04-30 13:27:56.379534 chsu_schedule_api-1.2.2/chsu_schedule_api/types/building.py
+-rw-r--r--   0        0        0      556 2024-04-30 15:09:39.999469 chsu_schedule_api-1.2.2/chsu_schedule_api/types/department.py
+-rw-r--r--   0        0        0      250 2024-04-30 15:10:00.610149 chsu_schedule_api-1.2.2/chsu_schedule_api/types/discipline.py
+-rw-r--r--   0        0        0      495 2024-04-30 15:09:42.737932 chsu_schedule_api-1.2.2/chsu_schedule_api/types/student_group.py
+-rw-r--r--   0        0        0      466 2024-04-30 15:11:29.469534 chsu_schedule_api-1.2.2/chsu_schedule_api/types/teacher.py
+-rw-r--r--   0        0        0     3710 2024-04-30 23:12:59.889989 chsu_schedule_api-1.2.2/chsu_schedule_api/types/timetable.py
+-rw-r--r--   0        0        0     1093 2024-04-21 21:48:20.041900 chsu_schedule_api-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1378 2024-05-09 23:50:52.169709 chsu_schedule_api-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2073 2024-05-09 23:47:23.246904 chsu_schedule_api-1.2.2/README.md
+-rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 chsu_schedule_api-1.2.2/PKG-INFO
```

### Comparing `chsu_schedule_api-1.2.1/chsu_schedule_api/api/abc.py` & `chsu_schedule_api-1.2.2/chsu_schedule_api/api/abc.py`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.2.1/chsu_schedule_api/api/api.py` & `chsu_schedule_api-1.2.2/chsu_schedule_api/api/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 )
 from chsu_schedule_api.enums import Methods
 from chsu_schedule_api.errors import (
     CHSUApiLookupError,
     CHSUApiResponseError,
     CHSUApiUnauthorizedError,
 )
-from chsu_schedule_api.models import (
+from chsu_schedule_api.types import (
     Auditorium,
     Building,
     Department,
     Discipline,
     Group,
     GroupId,
     Lecturer,
@@ -34,28 +34,32 @@
     TitleTimeTableType,
 )
 
 from .abc import ABCApi
 
 if TYPE_CHECKING:
     from chsu_schedule_api.client.abc import ABCHttpClient
-    from chsu_schedule_api.models import TimeTableType
+    from chsu_schedule_api.types import TimeTableType
 
 
 class CHSUApi(ABCApi):
     """CHSU API wrapper"""
 
     def __init__(
         self,
         username: str,
         password: str,
         client: "ABCHttpClient | None" = None,
     ) -> None:
         self._headers = {"User-Agent": "/"}
         self._auth_data = {"username": username, "password": password}
+        self._cache: dict[str, dict[str, "TimeTableType"]] = {
+            "lecturers": {},
+            "groups": {},
+        }
         super().__init__(client or AiohttpClient())
 
     async def auth_signin(self) -> bool:
         """
         Authorize
         Returns true on success
         """
@@ -153,30 +157,40 @@
         return [Teacher.model_validate(tch) for tch in resp]
 
     async def _get_id_by_title(
         self, title_tt: "TitleTimeTableType"
     ) -> "TimeTableType":
         """Get group or lecturer id"""
         if isinstance(title_tt, Group):
+            if title_tt.title in self._cache["groups"]:
+                return self._cache["groups"][title_tt.title]
             groups = await self.get_student_groups()
             for g in groups:
                 if g.title == title_tt.title:
-                    return GroupId(
+                    group = GroupId(
                         id=g.id,
                         from_date=title_tt.from_date,
                         to_date=title_tt.to_date,
                     )
+                    self._cache["groups"][title_tt.title] = group
+                    return group
             msg = f"Group {title_tt.title} not found"
             raise CHSUApiLookupError(msg)
+
         if isinstance(title_tt, Lecturer):
+            if title_tt.fullname in self._cache["lecturers"]:
+                return self._cache["lecturers"][title_tt.fullname]
             teachers = await self.get_teachers()
             for t in teachers:
                 if t.fio == title_tt.fullname:
-                    return LecturerId(
+                    lecturer = LecturerId(
                         id=t.id,
                         from_date=title_tt.from_date,
                         to_date=title_tt.to_date,
                     )
+                    self._cache["lecturers"][title_tt.fullname] = lecturer
+                    return lecturer
             msg = f"Lecturer {title_tt.fullname} not found"
             raise CHSUApiLookupError(msg)
+
         msg = f"Invalid time table type: {title_tt.__class__}"
         raise CHSUApiLookupError(msg)
```

### Comparing `chsu_schedule_api-1.2.1/chsu_schedule_api/client/abc.py` & `chsu_schedule_api-1.2.2/chsu_schedule_api/client/abc.py`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.2.1/chsu_schedule_api/client/aiohttp.py` & `chsu_schedule_api-1.2.2/chsu_schedule_api/client/aiohttp.py`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.2.1/chsu_schedule_api/models/__init__.py` & `chsu_schedule_api-1.2.2/chsu_schedule_api/types/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,29 @@
     TimeTableType,
     TitleTimeTableType,
     TTAuditory,
     TTStudentGroup,
 )
 
 __all__ = (
-    "Full",
-    "Group",
-    "GroupId",
-    "Lecturer",
     "Auditorium",
+    "Building",
     "CHSUModel",
     "CHSUResponseModel",
-    "Building",
+    "Chair",
     "Department",
-    "Node",
     "Discipline",
-    "Chair",
     "Faculty",
+    "Full",
+    "Group",
+    "GroupId",
+    "Lecturer",
+    "LecturerId",
+    "Node",
     "StudentGroup",
+    "TTAuditory",
+    "TTStudentGroup",
     "Teacher",
-    "LecturerId",
     "TimeTable",
     "TimeTableType",
     "TitleTimeTableType",
-    "TTAuditory",
-    "TTStudentGroup",
 )
```

### Comparing `chsu_schedule_api-1.2.1/chsu_schedule_api/models/timetable.py` & `chsu_schedule_api-1.2.2/chsu_schedule_api/types/timetable.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,89 @@
 from abc import abstractmethod
 from datetime import datetime, timedelta, timezone
 
-from pydantic import Field, validator
+from pydantic import Field, field_validator
 
-from chsu_schedule_api.models.building import Building
-from chsu_schedule_api.models.discipline import Discipline
-from chsu_schedule_api.models.teacher import Teacher
+from chsu_schedule_api.types.building import Building
+from chsu_schedule_api.types.discipline import Discipline
+from chsu_schedule_api.types.teacher import Teacher
 
 from .base import CHSUModel
 
 
 class TimeTableType(CHSUModel):
     """Base time table model"""
 
-    from_date: datetime | str
-    to_date: datetime | str
+    from_date: datetime | str | None = Field(default=None)
+    to_date: datetime | str | None = Field(default=None)
 
     @property
     @abstractmethod
     def path(self) -> str:
         """Time table path"""
 
-    def _dt_to_str(self) -> None:
+    def _prepare_date(self) -> None:
+        tz = timezone(timedelta(hours=3))
+        if self.from_date is None:
+            self.from_date = datetime.now(tz=tz)
+        if self.to_date is None:
+            self.to_date = self.from_date
         if isinstance(self.from_date, datetime):
             self.from_date = self.from_date.strftime("%d.%m.%Y")
         if isinstance(self.to_date, datetime):
             self.to_date = self.to_date.strftime("%d.%m.%Y")
 
 
 class TitleTimeTableType(CHSUModel):
     """
     Base model for time tables
     that require pre id definition
     """
 
-    from_date: datetime | str
-    to_date: datetime | str
+    from_date: datetime | str | None = Field(default=None)
+    to_date: datetime | str | None = Field(default=None)
 
 
 class LecturerId(TimeTableType):
     """Lecturer time table by id model"""
 
     id: int
 
     @property
     def path(self) -> str:
         """Time table path"""
-        super()._dt_to_str()
-        return f"/from/{self.from_date}/to/{self.to_date}/lecturerId/{self.id}"
+        super()._prepare_date()
+        return (
+            f"/from/{self.from_date}/to/"
+            f"{self.to_date or self.from_date}/lecturerId/{self.id}"
+        )
 
 
 class GroupId(TimeTableType):
     """Group time table by id model"""
 
     id: int
 
     @property
     def path(self) -> str:
         """Timetable path"""
-        super()._dt_to_str()
-        return f"/from/{self.from_date}/to/{self.to_date}/groupId/{self.id}"
+        super()._prepare_date()
+        return (
+            f"/from/{self.from_date}/to/"
+            f"{self.to_date or self.from_date}/groupId/{self.id}"
+        )
 
 
 class Full(TimeTableType):
     """Full time table model"""
 
     @property
     def path(self) -> str:
         """Timetable path"""
-        super()._dt_to_str()
+        super()._prepare_date()
         return f"/event/from/{self.from_date}/to/{self.to_date}"
 
 
 class Group(TitleTimeTableType):
     """Group time table by title model"""
 
     title: str
@@ -106,15 +117,22 @@
     lecturers: list[Teacher]  # can be empty
     abbrlessontype: str | None
     lessontype: str | None
     week: int
     weekday: int
     week_type: str = Field(alias="weekType")
     online_event: str | None = Field(alias="onlineEvent")
-    online: int
+    online: bool
+
+    def __str__(self) -> str:
+        """Return a string representation of the time table"""
+        return (
+            f"<TimeTable {self.date_event.strftime('%d.%m.%Y')} "
+            f"{self.discipline.title} ауд. {self.auditory.title}>"
+        )
 
-    @validator("date_event", pre=True)
+    @field_validator("date_event", mode="before")
     @classmethod
     def validate_datetime(cls, value: str) -> datetime:
         """Validate datetime"""
         tz = timezone(timedelta(hours=3))
         return datetime.strptime(value, "%d.%m.%Y").replace(tzinfo=tz)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `chsu_schedule_api-1.2.1/LICENSE` & `chsu_schedule_api-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.2.1/pyproject.toml` & `chsu_schedule_api-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chsu_schedule_api"
-version = "1.2.1"
+version = "1.2.2"
 description = "Asynchronous API wrapper for CHSU schedule API"
 authors = ["VoVcHiC <hello@chsutech.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/vovchic17/CHSUScheduleAPI"
 repository = "https://github.com/vovchic17/CHSUScheduleAPI"
 keywords = ["chsu", "schedule", "api"]
```

### Comparing `chsu_schedule_api-1.2.1/README.md` & `chsu_schedule_api-1.2.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # CHSUScheduleAPI
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
 [![Aiohttp](https://img.shields.io/badge/aiohttp-v3.9.3-2c5bb4?logo=aiohttp)](https://docs.aiohttp.org/en/stable/)
 [![Checked with mypy](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/vovchic17/static/main/src/badges/mypy.json)](https://mypy-lang.org/)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 
-Asynchronous API wrapper for [CHSU schedule API](api.chsu.ru)
+Asynchronous API wrapper for [CHSU schedule API](http://api.chsu.ru)
 
 ## Covered methods
 * Auth (validate token and sign in)
 * Building (get building list)
 * StudentGroup (get all the student groups)
 * Department (get list of departments and cathedras)
 * Auditorium (get auditorium list)
@@ -23,61 +23,50 @@
 
 Install via pip
 
 ```shell
 pip install chsu_schedule_api
 ```
 
-## Example
-Get building list
+## Synchronous example
+Get your schedule for today
 ```python
-import asyncio
-
 from chsu_schedule_api import CHSUApi
+from chsu_schedule_api.types import Group
 
 client = CHSUApi(username="USERNAME", password="PASSWORD")
 
-
-async def main() -> None:
-    await client.auth_signin()
-    buildings = await client.get_buildings()
-    print(buildings)
-
-
-if __name__ == "__main__":
-    asyncio.run(main())
+client.auth_signin()
+group_tt = client.get_time_table(
+    Group(title="1ИСб-01-1оп-22")
+)
+
+for tt in group_tt:
+    print(
+        tt.start_time,
+        tt.end_time,
+        tt.discipline.title,
+        tt.auditory.title
+    )
 ```
 
-## Example
-Get your group schedule
+## Asynchronous example
+Get building list
 ```python
 import asyncio
 
 from chsu_schedule_api import CHSUApi
-from chsu_schedule_api.models import Group
 
 client = CHSUApi(username="USERNAME", password="PASSWORD")
 
+
 async def main() -> None:
     await client.auth_signin()
-    group_tt = await client.get_time_table(
-        Group(
-            title="1ИСб-01-1оп-22",
-            from_date="03.04.2024",
-            to_date="03.04.2024",
-        )
-    )
-
-    for tt in group_tt:
-        print(
-            tt.start_time,
-            tt.end_time,
-            tt.discipline.title,
-            tt.auditory.title
-        )
+    buildings = await client.get_buildings()
+    print(buildings)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ## License
```

### Comparing `chsu_schedule_api-1.2.1/PKG-INFO` & `chsu_schedule_api-1.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chsu_schedule_api
-Version: 1.2.1
+Version: 1.2.2
 Summary: Asynchronous API wrapper for CHSU schedule API
 Home-page: https://github.com/vovchic17/CHSUScheduleAPI
 License: MIT
 Keywords: chsu,schedule,api
 Author: VoVcHiC
 Author-email: hello@chsutech.ru
 Requires-Python: >=3.12,<4.0
@@ -21,15 +21,15 @@
 
 # CHSUScheduleAPI
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
 [![Aiohttp](https://img.shields.io/badge/aiohttp-v3.9.3-2c5bb4?logo=aiohttp)](https://docs.aiohttp.org/en/stable/)
 [![Checked with mypy](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/vovchic17/static/main/src/badges/mypy.json)](https://mypy-lang.org/)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 
-Asynchronous API wrapper for [CHSU schedule API](api.chsu.ru)
+Asynchronous API wrapper for [CHSU schedule API](http://api.chsu.ru)
 
 ## Covered methods
 * Auth (validate token and sign in)
 * Building (get building list)
 * StudentGroup (get all the student groups)
 * Department (get list of departments and cathedras)
 * Auditorium (get auditorium list)
@@ -41,61 +41,50 @@
 
 Install via pip
 
 ```shell
 pip install chsu_schedule_api
 ```
 
-## Example
-Get building list
+## Synchronous example
+Get your schedule for today
 ```python
-import asyncio
-
 from chsu_schedule_api import CHSUApi
+from chsu_schedule_api.types import Group
 
 client = CHSUApi(username="USERNAME", password="PASSWORD")
 
-
-async def main() -> None:
-    await client.auth_signin()
-    buildings = await client.get_buildings()
-    print(buildings)
-
-
-if __name__ == "__main__":
-    asyncio.run(main())
+client.auth_signin()
+group_tt = client.get_time_table(
+    Group(title="1ИСб-01-1оп-22")
+)
+
+for tt in group_tt:
+    print(
+        tt.start_time,
+        tt.end_time,
+        tt.discipline.title,
+        tt.auditory.title
+    )
 ```
 
-## Example
-Get your group schedule
+## Asynchronous example
+Get building list
 ```python
 import asyncio
 
 from chsu_schedule_api import CHSUApi
-from chsu_schedule_api.models import Group
 
 client = CHSUApi(username="USERNAME", password="PASSWORD")
 
+
 async def main() -> None:
     await client.auth_signin()
-    group_tt = await client.get_time_table(
-        Group(
-            title="1ИСб-01-1оп-22",
-            from_date="03.04.2024",
-            to_date="03.04.2024",
-        )
-    )
-
-    for tt in group_tt:
-        print(
-            tt.start_time,
-            tt.end_time,
-            tt.discipline.title,
-            tt.auditory.title
-        )
+    buildings = await client.get_buildings()
+    print(buildings)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ## License
```

