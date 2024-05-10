# Comparing `tmp/fastcrud-0.9.0.tar.gz` & `tmp/fastcrud-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastcrud-0.9.0.tar", max compression
+gzip compressed data, was "fastcrud-0.9.1.tar", max compression
```

## Comparing `fastcrud-0.9.0.tar` & `fastcrud-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1067 2024-01-09 01:09:38.763746 fastcrud-0.9.0/LICENSE
--rw-r--r--   0        0        0     8293 2024-03-14 21:30:08.730296 fastcrud-0.9.0/README.md
--rw-r--r--   0        0        0      246 2024-03-13 06:46:59.890132 fastcrud-0.9.0/fastcrud/__init__.py
--rw-r--r--   0        0        0        0 2024-01-09 01:15:05.380759 fastcrud-0.9.0/fastcrud/crud/__init__.py
--rw-r--r--   0        0        0    51447 2024-03-14 20:26:24.653351 fastcrud-0.9.0/fastcrud/crud/fast_crud.py
--rw-r--r--   0        0        0     4642 2024-03-13 06:15:04.807973 fastcrud-0.9.0/fastcrud/crud/helper.py
--rw-r--r--   0        0        0        0 2024-01-16 08:13:48.560647 fastcrud-0.9.0/fastcrud/endpoint/__init__.py
--rw-r--r--   0        0        0     9988 2024-03-04 19:02:47.172542 fastcrud-0.9.0/fastcrud/endpoint/crud_router.py
--rw-r--r--   0        0        0    21919 2024-03-04 19:02:47.172761 fastcrud-0.9.0/fastcrud/endpoint/endpoint_creator.py
--rw-r--r--   0        0        0     1616 2024-03-02 02:27:53.790165 fastcrud-0.9.0/fastcrud/endpoint/helper.py
--rw-r--r--   0        0        0       61 2024-02-11 22:05:59.357599 fastcrud-0.9.0/fastcrud/exceptions/__init__.py
--rw-r--r--   0        0        0     1791 2024-01-17 07:26:20.017811 fastcrud-0.9.0/fastcrud/exceptions/http_exceptions.py
--rw-r--r--   0        0        0      245 2024-03-02 02:27:53.790405 fastcrud-0.9.0/fastcrud/paginated/__init__.py
--rw-r--r--   0        0        0      794 2024-03-02 02:27:53.790764 fastcrud-0.9.0/fastcrud/paginated/helper.py
--rw-r--r--   0        0        0     1001 2024-03-02 02:27:53.791052 fastcrud-0.9.0/fastcrud/paginated/response.py
--rw-r--r--   0        0        0      381 2024-03-02 02:27:53.791362 fastcrud-0.9.0/fastcrud/paginated/schemas.py
--rw-r--r--   0        0        0        0 2024-01-31 12:56:26.941676 fastcrud-0.9.0/fastcrud/py.typed
--rw-r--r--   0        0        0     1363 2024-03-14 21:45:32.954087 fastcrud-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     9511 1970-01-01 00:00:00.000000 fastcrud-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-01-09 01:09:38.763746 fastcrud-0.9.1/LICENSE
+-rw-r--r--   0        0        0     8293 2024-03-14 22:11:48.965240 fastcrud-0.9.1/README.md
+-rw-r--r--   0        0        0      381 2024-03-18 06:58:48.815138 fastcrud-0.9.1/fastcrud/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-09 01:15:05.380759 fastcrud-0.9.1/fastcrud/crud/__init__.py
+-rw-r--r--   0        0        0    53363 2024-03-18 06:58:48.816538 fastcrud-0.9.1/fastcrud/crud/fast_crud.py
+-rw-r--r--   0        0        0     3720 2024-03-18 07:00:21.117320 fastcrud-0.9.1/fastcrud/crud/helper.py
+-rw-r--r--   0        0        0        0 2024-01-16 08:13:48.560647 fastcrud-0.9.1/fastcrud/endpoint/__init__.py
+-rw-r--r--   0        0        0     9988 2024-03-04 19:02:47.172542 fastcrud-0.9.1/fastcrud/endpoint/crud_router.py
+-rw-r--r--   0        0        0    21919 2024-03-04 19:02:47.172761 fastcrud-0.9.1/fastcrud/endpoint/endpoint_creator.py
+-rw-r--r--   0        0        0     1616 2024-03-02 02:27:53.790165 fastcrud-0.9.1/fastcrud/endpoint/helper.py
+-rw-r--r--   0        0        0       61 2024-02-11 22:05:59.357599 fastcrud-0.9.1/fastcrud/exceptions/__init__.py
+-rw-r--r--   0        0        0     1791 2024-01-17 07:26:20.017811 fastcrud-0.9.1/fastcrud/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0      245 2024-03-02 02:27:53.790405 fastcrud-0.9.1/fastcrud/paginated/__init__.py
+-rw-r--r--   0        0        0      794 2024-03-02 02:27:53.790764 fastcrud-0.9.1/fastcrud/paginated/helper.py
+-rw-r--r--   0        0        0     1001 2024-03-02 02:27:53.791052 fastcrud-0.9.1/fastcrud/paginated/response.py
+-rw-r--r--   0        0        0      381 2024-03-02 02:27:53.791362 fastcrud-0.9.1/fastcrud/paginated/schemas.py
+-rw-r--r--   0        0        0        0 2024-01-31 12:56:26.941676 fastcrud-0.9.1/fastcrud/py.typed
+-rw-r--r--   0        0        0     1363 2024-03-19 04:39:57.884338 fastcrud-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     9511 1970-01-01 00:00:00.000000 fastcrud-0.9.1/PKG-INFO
```

### Comparing `fastcrud-0.9.0/LICENSE` & `fastcrud-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastcrud-0.9.0/README.md` & `fastcrud-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `fastcrud-0.9.0/fastcrud/crud/fast_crud.py` & `fastcrud-0.9.1/fastcrud/crud/fast_crud.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from sqlalchemy import select, update, delete, func, inspect, asc, desc
 from sqlalchemy.exc import ArgumentError, MultipleResultsFound, NoResultFound
 
 from sqlalchemy.sql import Join
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.engine.row import Row
 from sqlalchemy.orm import DeclarativeBase
+from sqlalchemy.orm.util import AliasedClass
 from sqlalchemy.sql.elements import BinaryExpression
 from sqlalchemy.sql.selectable import Select
 
 from .helper import (
     _extract_matching_columns_from_schema,
     _auto_detect_join_condition,
-    _add_column_with_prefix,
     JoinConfig,
 )
 
 ModelType = TypeVar("ModelType", bound=DeclarativeBase)
 CreateSchemaType = TypeVar("CreateSchemaType", bound=BaseModel)
 UpdateSchemaType = TypeVar("UpdateSchemaType", bound=BaseModel)
 UpdateSchemaInternalType = TypeVar("UpdateSchemaInternalType", bound=BaseModel)
@@ -533,20 +533,21 @@
 
         total_count = await self.count(db=db, **kwargs)
         return {"data": data, "total_count": total_count}
 
     async def get_joined(
         self,
         db: AsyncSession,
+        schema_to_select: Optional[type[BaseModel]] = None,
         join_model: Optional[type[DeclarativeBase]] = None,
-        join_prefix: Optional[str] = None,
         join_on: Optional[Union[Join, BinaryExpression]] = None,
-        schema_to_select: Optional[type[BaseModel]] = None,
+        join_prefix: Optional[str] = None,
         join_schema_to_select: Optional[type[BaseModel]] = None,
         join_type: str = "left",
+        alias: Optional[AliasedClass] = None,
         joins_config: Optional[list[JoinConfig]] = None,
         **kwargs: Any,
     ) -> Optional[dict[str, Any]]:
         """
         Fetches a single record with one or multiple joins on other models. If 'join_on' is not provided, the method attempts
         to automatically detect the join condition using foreign key relationships. For multiple joins, use 'joins_config' to
         specify each join configuration. Advanced filters supported:
@@ -554,20 +555,21 @@
             '__lt' (less than),
             '__gte' (greater than or equal to),
             '__lte' (less than or equal to), and
             '__ne' (not equal).
 
         Args:
             db: The SQLAlchemy async session.
+            schema_to_select: Pydantic schema for selecting specific columns from the primary model. Required if `return_as_model` is True.
             join_model: The model to join with.
-            join_prefix: Optional prefix to be added to all columns of the joined model. If None, no prefix is added.
             join_on: SQLAlchemy Join object for specifying the ON clause of the join. If None, the join condition is auto-detected based on foreign keys.
-            schema_to_select: Pydantic schema for selecting specific columns from the primary model. Required if `return_as_model` is True.
+            join_prefix: Optional prefix to be added to all columns of the joined model. If None, no prefix is added.
             join_schema_to_select: Pydantic schema for selecting specific columns from the joined model.
             join_type: Specifies the type of join operation to perform. Can be "left" for a left outer join or "inner" for an inner join.
+            alias: An instance of `AliasedClass` for the join model, useful for self-joins or multiple joins on the same model. Result of `aliased(join_model)`.
             joins_config: A list of JoinConfig instances, each specifying a model to join with, join condition, optional prefix for column names, schema for selecting specific columns, and the type of join. This parameter enables support for multiple joins.
             **kwargs: Filters to apply to the primary model query, supporting advanced comparison operators for refined searching.
 
         Returns:
             A dictionary representing the joined record, or None if no record matches the criteria.
 
         Raises:
@@ -637,81 +639,86 @@
                         schema_to_select=DepartmentSchema,
                         join_type="inner",
                     )
                 ]
             )
             ```
 
-            Return example: prefix added, no schema_to_select or join_schema_to_select
+            Using `alias` for joining the same model multiple times:
             ```python
-            {
-                "id": 1,
-                "name": "John Doe",
-                "username": "john_doe",
-                "email": "johndoe@example.com",
-                "hashed_password": "hashed_password_example",
-                "profile_image_url": "https://profileimageurl.com/default.jpg",
-                "uuid": "123e4567-e89b-12d3-a456-426614174000",
-                "created_at": "2023-01-01T12:00:00",
-                "updated_at": "2023-01-02T12:00:00",
-                "deleted_at": null,
-                "is_deleted": false,
-                "is_superuser": false,
-                "tier_id": 2,
-                "tier_name": "Premium",
-                "tier_created_at": "2022-12-01T10:00:00",
-                "tier_updated_at": "2023-01-01T11:00:00"
-            }
+            from fastcrud import aliased
+
+            owner_alias = aliased(ModelTest, name="owner")
+            user_alias = aliased(ModelTest, name="user")
+
+            result = await crud.get_joined(
+                db=session,
+                schema_to_select=BookingSchema,
+                joins_config=[
+                    JoinConfig(
+                        model=ModelTest,
+                        join_on=BookingModel.owner_id == owner_alias.id,
+                        join_prefix="owner_",
+                        alias=owner_alias,
+                        schema_to_select=UserSchema
+                    ),
+                    JoinConfig(
+                        model=ModelTest,
+                        join_on=BookingModel.user_id == user_alias.id,
+                        join_prefix="user_",
+                        alias=user_alias,
+                        schema_to_select=UserSchema
+                    )
+                ],
+                id=1
+            )
             ```
         """
         if joins_config and (
-            join_model or join_prefix or join_on or join_schema_to_select
+            join_model or join_prefix or join_on or join_schema_to_select or alias
         ):
             raise ValueError(
-                "Cannot use both single join parameters and joinsConfig simultaneously."
+                "Cannot use both single join parameters and joins_config simultaneously."
             )
         elif not joins_config and not join_model:
-            raise ValueError(
-                "You need one of join_model or joins_config."
-            )
+            raise ValueError("You need one of join_model or joins_config.")
 
         primary_select = _extract_matching_columns_from_schema(
-            model=self.model, schema=schema_to_select
+            model=self.model,
+            schema=schema_to_select,
         )
-        stmt: Select = select(*primary_select)
+        stmt: Select = select(*primary_select).select_from(self.model)
 
         join_definitions = joins_config if joins_config else []
         if join_model:
             join_definitions.append(
                 JoinConfig(
                     model=join_model,
                     join_on=join_on,
                     join_prefix=join_prefix,
                     schema_to_select=join_schema_to_select,
                     join_type=join_type,
+                    alias=alias,
                 )
             )
 
         for join in join_definitions:
+            model = join.alias or join.model
+
             join_select = _extract_matching_columns_from_schema(
-                join.model, join.schema_to_select
+                model=join.model,
+                schema=join.schema_to_select,
+                prefix=join.join_prefix,
+                alias=join.alias,
             )
 
-            if join.join_prefix:
-                join_select = [
-                    _add_column_with_prefix(column, join.join_prefix)
-                    for column in join_select
-                ]
-
             if join.join_type == "left":
-                stmt = stmt.outerjoin(join.model, join.join_on).add_columns(
-                    *join_select
-                )
+                stmt = stmt.outerjoin(model, join.join_on).add_columns(*join_select)
             elif join.join_type == "inner":
-                stmt = stmt.join(join.model, join.join_on).add_columns(*join_select)
+                stmt = stmt.join(model, join.join_on).add_columns(*join_select)
             else:
                 raise ValueError(f"Unsupported join type: {join.join_type}.")
 
         filters = self._parse_filters(**kwargs)
         if filters:
             stmt = stmt.filter(*filters)
 
@@ -722,20 +729,21 @@
             return out
 
         return None
 
     async def get_multi_joined(
         self,
         db: AsyncSession,
+        schema_to_select: Optional[type[BaseModel]] = None,
         join_model: Optional[type[ModelType]] = None,
-        join_prefix: Optional[str] = None,
         join_on: Optional[Any] = None,
-        schema_to_select: Optional[type[BaseModel]] = None,
+        join_prefix: Optional[str] = None,
         join_schema_to_select: Optional[type[BaseModel]] = None,
         join_type: str = "left",
+        alias: Optional[str] = None,
         offset: int = 0,
         limit: int = 100,
         sort_columns: Optional[Union[str, list[str]]] = None,
         sort_orders: Optional[Union[str, list[str]]] = None,
         return_as_model: bool = False,
         joins_config: Optional[list[JoinConfig]] = None,
         **kwargs: Any,
@@ -747,33 +755,34 @@
             '__lt' (less than),
             '__gte' (greater than or equal to),
             '__lte' (less than or equal to), and
             '__ne' (not equal).
 
         Args:
             db: The SQLAlchemy async session.
+            schema_to_select: Pydantic schema for selecting specific columns from the primary model. Required if `return_as_model` is True.
             join_model: The model to join with.
-            join_prefix: Optional prefix to be added to all columns of the joined model. If None, no prefix is added.
             join_on: SQLAlchemy Join object for specifying the ON clause of the join. If None, the join condition is auto-detected based on foreign keys.
-            schema_to_select: Pydantic schema for selecting specific columns from the primary model. Required if `return_as_model` is True.
+            join_prefix: Optional prefix to be added to all columns of the joined model. If None, no prefix is added.
             join_schema_to_select: Pydantic schema for selecting specific columns from the joined model.
             join_type: Specifies the type of join operation to perform. Can be "left" for a left outer join or "inner" for an inner join.
+            alias: An instance of `AliasedClass` for the join model, useful for self-joins or multiple joins on the same model. Result of `aliased(join_model)`.
             offset: The offset (number of records to skip) for pagination.
             limit: The limit (maximum number of records to return) for pagination.
             sort_columns: A single column name or a list of column names on which to apply sorting.
             sort_orders: A single sort order ('asc' or 'desc') or a list of sort orders corresponding to the columns in sort_columns. If not provided, defaults to 'asc' for each column.
             return_as_model: If True, converts the fetched data to Pydantic models based on schema_to_select. Defaults to False.
             joins_config: List of JoinConfig instances for specifying multiple joins. Each instance defines a model to join with, join condition, optional prefix for column names, schema for selecting specific columns, and join type.
             **kwargs: Filters to apply to the primary query, including advanced comparison operators for refined searching.
 
         Returns:
             A dictionary containing the fetched rows under 'data' key and total count under 'total_count'.
 
         Raises:
-            ValueError: If limit or offset is negative, or if schema_to_select is required but not provided or invalid. 
+            ValueError: If limit or offset is negative, or if schema_to_select is required but not provided or invalid.
                         Also if both 'joins_config' and any of the single join parameters are provided or none of 'joins_config' and 'join_model' is provided.
 
         Examples:
             Fetching multiple User records joined with Tier records, using left join, returning raw data:
             ```python
             users = await crud_user.get_multi_joined(
                 db=session,
@@ -870,69 +879,97 @@
                 ],
                 offset=0,
                 limit=10,
                 sort_columns='username',
                 sort_orders='asc'
             )
             ```
+
+            Example using `alias` for multiple joins, with pagination, sorting, and model conversion:
+            ```python
+            from fastcrud import JoinConfig, FastCRUD, aliased
+
+            # Aliasing for self-joins or multiple joins on the same table
+            owner_alias = aliased(ModelTest, name="owner")
+            user_alias = aliased(ModelTest, name="user")
+
+            # Initialize your FastCRUD instance for BookingModel
+            crud = FastCRUD(BookingModel)
+
+            result = await crud.get_multi_joined(
+                db=session,
+                schema_to_select=BookingSchema,  # Primary model schema
+                joins_config=[
+                    JoinConfig(
+                        model=ModelTest,
+                        join_on=BookingModel.owner_id == owner_alias.id,
+                        join_prefix="owner_",
+                        alias=owner_alias,
+                        schema_to_select=UserSchema  # Schema for the joined model
+                    ),
+                    JoinConfig(
+                        model=ModelTest,
+                        join_on=BookingModel.user_id == user_alias.id,
+                        join_prefix="user_",
+                        alias=user_alias,
+                        schema_to_select=UserSchema
+                    )
+                ],
+                offset=10,  # Skip the first 10 records
+                limit=5,  # Fetch up to 5 records
+                sort_columns=['booking_date'],  # Sort by booking_date
+                sort_orders=['desc']  # In descending order
+            )
+            ```
         """
         if joins_config and (
-            join_model or join_prefix or join_on or join_schema_to_select
+            join_model or join_prefix or join_on or join_schema_to_select or alias
         ):
             raise ValueError(
-                "Cannot use both single join parameters and joinsConfig simultaneously."
+                "Cannot use both single join parameters and joins_config simultaneously."
             )
         elif not joins_config and not join_model:
-            raise ValueError(
-                "You need one of join_model or joins_config."
-            )
+            raise ValueError("You need one of join_model or joins_config.")
 
         if limit < 0 or offset < 0:
             raise ValueError("Limit and offset must be non-negative.")
 
-        joins: list[JoinConfig] = []
-        if join_model is not None:
-            joins.append(
+        primary_select = _extract_matching_columns_from_schema(
+            model=self.model, schema=schema_to_select
+        )
+        stmt: Select = select(*primary_select)
+
+        join_definitions = joins_config if joins_config else []
+        if join_model:
+            join_definitions.append(
                 JoinConfig(
                     model=join_model,
                     join_on=join_on
                     or _auto_detect_join_condition(self.model, join_model),
                     join_prefix=join_prefix,
                     schema_to_select=join_schema_to_select,
                     join_type=join_type,
+                    alias=alias,
                 )
             )
-        elif joins_config:
-            joins.extend(joins_config)
 
-        primary_select = _extract_matching_columns_from_schema(
-            model=self.model, schema=schema_to_select
-        )
-        stmt: Select = select(*primary_select)
-
-        for join in joins:
-            if join.schema_to_select:
-                join_select = _extract_matching_columns_from_schema(
-                    join.model, join.schema_to_select
-                )
-            else:
-                join_select = inspect(join.model).c
+        for join in join_definitions:
+            model = join.alias or join.model
 
-            if join.join_prefix:
-                join_select = [
-                    _add_column_with_prefix(column, join.join_prefix)
-                    for column in join_select
-                ]
+            join_select = _extract_matching_columns_from_schema(
+                model=join.model,
+                schema=join.schema_to_select,
+                prefix=join.join_prefix,
+                alias=join.alias,
+            )
 
             if join.join_type == "left":
-                stmt = stmt.outerjoin(join.model, join.join_on).add_columns(
-                    *join_select
-                )
+                stmt = stmt.outerjoin(model, join.join_on).add_columns(*join_select)
             elif join.join_type == "inner":
-                stmt = stmt.join(join.model, join.join_on).add_columns(*join_select)
+                stmt = stmt.join(model, join.join_on).add_columns(*join_select)
             else:
                 raise ValueError(f"Unsupported join type: {join.join_type}.")
 
         filters = self._parse_filters(**kwargs)
         if filters:
             stmt = stmt.filter(*filters)
```

### Comparing `fastcrud-0.9.0/fastcrud/endpoint/crud_router.py` & `fastcrud-0.9.1/fastcrud/endpoint/crud_router.py`

 * *Files identical despite different names*

### Comparing `fastcrud-0.9.0/fastcrud/endpoint/endpoint_creator.py` & `fastcrud-0.9.1/fastcrud/endpoint/endpoint_creator.py`

 * *Files identical despite different names*

### Comparing `fastcrud-0.9.0/fastcrud/endpoint/helper.py` & `fastcrud-0.9.1/fastcrud/endpoint/helper.py`

 * *Files identical despite different names*

### Comparing `fastcrud-0.9.0/fastcrud/exceptions/http_exceptions.py` & `fastcrud-0.9.1/fastcrud/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `fastcrud-0.9.0/fastcrud/paginated/helper.py` & `fastcrud-0.9.1/fastcrud/paginated/helper.py`

 * *Files identical despite different names*

### Comparing `fastcrud-0.9.0/fastcrud/paginated/response.py` & `fastcrud-0.9.1/fastcrud/paginated/response.py`

 * *Files identical despite different names*

### Comparing `fastcrud-0.9.0/pyproject.toml` & `fastcrud-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastcrud"
-version = "0.9.0"
+version = "0.9.1"
 description = "FastCRUD is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities."
 authors = ["Igor Benav <igor.magalhaes.r@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/igorbenav/fastcrud"
 include = [
     "LICENSE",
```

### Comparing `fastcrud-0.9.0/PKG-INFO` & `fastcrud-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcrud
-Version: 0.9.0
+Version: 0.9.1
 Summary: FastCRUD is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities.
 Home-page: https://github.com/igorbenav/fastcrud
 License: MIT
 Keywords: fastapi,crud,async,sqlalchemy,pydantic
 Author: Igor Benav
 Author-email: igor.magalhaes.r@gmail.com
 Requires-Python: >=3.9,<4.0
```

