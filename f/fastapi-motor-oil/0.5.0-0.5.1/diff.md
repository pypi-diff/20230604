# Comparing `tmp/fastapi_motor_oil-0.5.0.tar.gz` & `tmp/fastapi_motor_oil-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_motor_oil-0.5.0.tar", max compression
+gzip compressed data, was "fastapi_motor_oil-0.5.1.tar", max compression
```

## Comparing `fastapi_motor_oil-0.5.0.tar` & `fastapi_motor_oil-0.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-02-22 21:38:05.147034 fastapi_motor_oil-0.5.0/LICENSE
--rw-r--r--   0        0        0     9906 2023-03-03 14:53:38.016602 fastapi_motor_oil-0.5.0/README.md
--rw-r--r--   0        0        0     1103 2023-03-20 22:09:29.506455 fastapi_motor_oil-0.5.0/fastapi_motor_oil/__init__.py
--rw-r--r--   0        0        0     3103 2023-03-03 10:14:18.487006 fastapi_motor_oil-0.5.0/fastapi_motor_oil/bound_method_wrapper.py
--rw-r--r--   0        0        0     2551 2023-03-03 10:13:53.174943 fastapi_motor_oil-0.5.0/fastapi_motor_oil/delete_rule.py
--rw-r--r--   0        0        0     2550 2023-03-03 10:04:07.732907 fastapi_motor_oil-0.5.0/fastapi_motor_oil/model.py
--rw-r--r--   0        0        0        0 2023-02-24 18:46:38.693945 fastapi_motor_oil-0.5.0/fastapi_motor_oil/py.typed
--rw-r--r--   0        0        0    26121 2023-03-31 19:02:16.438341 fastapi_motor_oil-0.5.0/fastapi_motor_oil/service.py
--rw-r--r--   0        0        0     4902 2023-03-20 22:17:36.344965 fastapi_motor_oil-0.5.0/fastapi_motor_oil/typing.py
--rw-r--r--   0        0        0     1565 2023-03-01 12:30:19.133549 fastapi_motor_oil-0.5.0/fastapi_motor_oil/validator.py
--rw-r--r--   0        0        0     2234 2023-03-21 07:49:08.957996 fastapi_motor_oil-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    10998 1970-01-01 00:00:00.000000 fastapi_motor_oil-0.5.0/setup.py
--rw-r--r--   0        0        0    10468 1970-01-01 00:00:00.000000 fastapi_motor_oil-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-22 21:38:05.147034 fastapi_motor_oil-0.5.1/LICENSE
+-rw-r--r--   0        0        0     9954 2023-04-01 14:14:36.921182 fastapi_motor_oil-0.5.1/README.md
+-rw-r--r--   0        0        0     1631 2023-06-04 12:59:37.309187 fastapi_motor_oil-0.5.1/fastapi_motor_oil/__init__.py
+-rw-r--r--   0        0        0     3145 2023-06-04 12:09:52.899211 fastapi_motor_oil-0.5.1/fastapi_motor_oil/bound_method_wrapper.py
+-rw-r--r--   0        0        0     2641 2023-06-04 12:09:20.394794 fastapi_motor_oil-0.5.1/fastapi_motor_oil/delete_rule.py
+-rw-r--r--   0        0        0     2768 2023-06-04 12:12:44.073079 fastapi_motor_oil-0.5.1/fastapi_motor_oil/model.py
+-rw-r--r--   0        0        0        0 2023-02-24 18:46:38.693945 fastapi_motor_oil-0.5.1/fastapi_motor_oil/py.typed
+-rw-r--r--   0        0        0    26224 2023-06-04 12:34:04.571192 fastapi_motor_oil-0.5.1/fastapi_motor_oil/service.py
+-rw-r--r--   0        0        0     5225 2023-06-04 12:18:18.159592 fastapi_motor_oil-0.5.1/fastapi_motor_oil/typing.py
+-rw-r--r--   0        0        0     1636 2023-06-04 12:13:45.573637 fastapi_motor_oil-0.5.1/fastapi_motor_oil/validator.py
+-rw-r--r--   0        0        0     2702 2023-06-04 12:41:38.300297 fastapi_motor_oil-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    11047 1970-01-01 00:00:00.000000 fastapi_motor_oil-0.5.1/setup.py
+-rw-r--r--   0        0        0    10516 1970-01-01 00:00:00.000000 fastapi_motor_oil-0.5.1/PKG-INFO
```

### Comparing `fastapi_motor_oil-0.5.0/LICENSE` & `fastapi_motor_oil-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_motor_oil-0.5.0/README.md` & `fastapi_motor_oil-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 `FastAPI-motor-oil` is a collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a [FastAPI](https://fastapi.tiangolo.com/).
 
 Key features:
 
 - Database **model** design with `Pydantic`.
 - Relationship support and validation using async **validators and delete rules** with a declarative, decorator-based syntax.
+- Declarative **index** specification.
 - Typed **utilities** for convenient model and API creation.
-- A complete and customizable **async service layer** with **transaction support** that integrates all the above to keep your API and business logic clean, flexible, and easy to understand.
+- Ready to use, customizable **async service layer** with **transaction support** that integrates all the above to keep your API and business logic clean, flexible, and easy to understand.
 
-By providing a convenient, declarative middle layer between MongoDB and your API, `FastAPI-motor-oil` is halfway between an object document mapper (based on `Pydantic`) and a database driver (by wrapping the async `motor` driver).
+By providing a convenient, declarative middle layer between MongoDB and your API, `FastAPI-motor-oil` is halfway between an object document mapper (based on `Pydantic`) and a database driver (by wrapping the official, async `motor` driver).
 
 See the [full documentation here](https://volfpeter.github.io/fastapi-motor-oil/).
 
 ## Installation
 
 The library is available on PyPI and can be installed with:
```

### Comparing `fastapi_motor_oil-0.5.0/fastapi_motor_oil/bound_method_wrapper.py` & `fastapi_motor_oil-0.5.1/fastapi_motor_oil/bound_method_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from typing import Concatenate, Generic, ParamSpec, Type, TypeVar
 from collections.abc import Callable, Coroutine
+from typing import Concatenate, Generic, ParamSpec, Type, TypeVar
+
+__all__ = ("BoundMethodWrapper",)
 
 TOwner = TypeVar("TOwner")
 TParams = ParamSpec("TParams")
 TConfig = TypeVar("TConfig")
 
 
 class BoundMethodWrapper(Generic[TOwner, TParams, TConfig]):
@@ -85,8 +87,8 @@
             owner: The owner instance of the wrapper (the `self` argument of the wrapped instance method).
             *args: The wrapped method's positional arguments.
             *kwargs: The wrapped method's keyword arguments.
         """
         try:
             await self._func(owner, *args, **kwargs)
         except Exception as e:
-            raise e if self.exception is None else self.exception(f"Method failed: {self.name}")
+            raise e if self.exception is None else self.exception(f"Method failed: {self.name}") from e
```

### Comparing `fastapi_motor_oil-0.5.0/fastapi_motor_oil/delete_rule.py` & `fastapi_motor_oil-0.5.1/fastapi_motor_oil/delete_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from typing import Literal, TypeVar
-
 from collections.abc import Callable, Coroutine, Sequence
+from typing import Literal, TypeVar
 
 from bson.objectid import ObjectId
 from motor.core import AgnosticClientSession
 
 from .bound_method_wrapper import BoundMethodWrapper
 
+__all__ = (
+    "DeleteError",
+    "DeleteConfig",
+    "DeleteRule",
+    "delete_rule",
+)
+
 
 class DeleteError(Exception):
     ...
 
 
 TOwner = TypeVar("TOwner")
 DeleteConfig = Literal["deny", "pre", "post"]
```

### Comparing `fastapi_motor_oil-0.5.0/fastapi_motor_oil/model.py` & `fastapi_motor_oil-0.5.1/fastapi_motor_oil/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 from __future__ import annotations
-from typing import Any, Callable, Generator, Protocol
 
+from collections.abc import Callable, Generator
 from datetime import datetime, timezone
+from typing import Any, Protocol
 
 from bson import ObjectId
 from motor.core import AgnosticClient, AgnosticDatabase
 from pydantic import BaseModel, Field
 from pydantic.datetime_parse import parse_datetime
 
+__all__ = (
+    "AgnosticClient",
+    "AgnosticDatabase",
+    "ClientProvider",
+    "DatabaseProvider",
+    "UTCDatetime",
+    "StrObjectId",
+    "DocumentModel",
+    "DeleteResultModel",
+)
+
 
 class ClientProvider(Protocol):
     """
     Client provider protocol for FastAPI database dependencies.
     """
 
     def __call__(self) -> AgnosticClient:
```

### Comparing `fastapi_motor_oil-0.5.0/fastapi_motor_oil/service.py` & `fastapi_motor_oil-0.5.1/fastapi_motor_oil/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
-from typing import Any, Generator, Generic, TypeVar, TYPE_CHECKING
 
-from collections.abc import AsyncGenerator, Callable, Coroutine, Mapping, Sequence
-from contextlib import asynccontextmanager, nullcontext, AbstractAsyncContextManager
+from collections.abc import AsyncGenerator, Callable, Coroutine, Generator, Mapping, Sequence
+from contextlib import AbstractAsyncContextManager, asynccontextmanager, nullcontext
+from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
 from bson import ObjectId
 from pydantic import BaseModel
 from pymongo.results import DeleteResult, InsertOneResult, UpdateResult
 
 if TYPE_CHECKING:
     from motor.core import (
-        AgnosticClient,
         AgnosticClientSession,
-        AgnosticCollection,
         AgnosticCursor,
-        AgnosticDatabase,
         AgnosticLatentCommandCursor,
     )
 
+    from .model import AgnosticClient, AgnosticDatabase
     from .typing import (
+        AgnosticCollection,
         Collation,
         CollectionOptions,
         DeleteOptions,
         FindOptions,
         IndexData,
         InsertOneOptions,
         MongoProjection,
@@ -31,14 +30,20 @@
         UpdateObject,
         UpdateOneOptions,
     )
 
 from .delete_rule import DeleteRule
 from .validator import Validator
 
+__all__ = (
+    "MongoService",
+    "DeleteResult",
+    "InsertOneResult",
+    "UpdateResult",
+)
 
 TInsert = TypeVar("TInsert", bound=BaseModel)
 TUpdate = TypeVar("TUpdate", bound=BaseModel)
 
 
 class MongoService(Generic[TInsert, TUpdate]):
     """
```

### Comparing `fastapi_motor_oil-0.5.0/fastapi_motor_oil/typing.py` & `fastapi_motor_oil-0.5.1/fastapi_motor_oil/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,40 @@
 from __future__ import annotations
-from typing import Any, Mapping, Sequence, TypedDict, TYPE_CHECKING
 
+from collections.abc import Mapping, Sequence
 from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, Any, TypedDict
 
 from motor.core import AgnosticCollection
 from pymongo.collation import Collation as PMCollation
 
 if TYPE_CHECKING:
     from bson.codec_options import CodecOptions
     from pymongo.read_concern import ReadConcern
-    from pymongo.read_preferences import Primary, PrimaryPreferred, Secondary, SecondaryPreferred, Nearest
+    from pymongo.read_preferences import Nearest, Primary, PrimaryPreferred, Secondary, SecondaryPreferred
     from pymongo.write_concern import WriteConcern
 
 
+__all__ = (
+    "AgnosticCollection",
+    "MongoProjection",
+    "MongoQuery",
+    "UpdateObject",
+    "CollationDict",
+    "Collation",
+    "CollectionOptions",
+    "DeleteOptions",
+    "FindOptions",
+    "IndexData",
+    "InsertOneOptions",
+    "UpdateOneOptions",
+    "UpdateManyOptions",
+)
+
+
 MongoProjection = dict[str, Any]
 """
 MongoDB projection object.
 """
 
 
 MongoQuery = dict[str, Any]
```

### Comparing `fastapi_motor_oil-0.5.0/fastapi_motor_oil/validator.py` & `fastapi_motor_oil-0.5.1/fastapi_motor_oil/validator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-from typing import Literal, TypeVar
-
 from collections.abc import Callable, Coroutine
+from typing import Literal, TypeVar
 
 from .bound_method_wrapper import BoundMethodWrapper
 from .typing import MongoQuery
 
+__all__ = (
+    "ValidationError",
+    "Validator",
+    "validator",
+)
+
 
 class ValidationError(Exception):
     ...
 
 
 TOwner = TypeVar("TOwner")
 TInsertOrUpdate = TypeVar("TInsertOrUpdate")
```

### Comparing `fastapi_motor_oil-0.5.0/setup.py` & `fastapi_motor_oil-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['motor>=3.1.1,<4.0.0', 'pydantic>=1.10.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'fastapi-motor-oil',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'Collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a FastAPI.',
-    'long_description': '# FastAPI-motor-oil\n\n`FastAPI-motor-oil` is a collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a [FastAPI](https://fastapi.tiangolo.com/).\n\nKey features:\n\n- Database **model** design with `Pydantic`.\n- Relationship support and validation using async **validators and delete rules** with a declarative, decorator-based syntax.\n- Typed **utilities** for convenient model and API creation.\n- A complete and customizable **async service layer** with **transaction support** that integrates all the above to keep your API and business logic clean, flexible, and easy to understand.\n\nBy providing a convenient, declarative middle layer between MongoDB and your API, `FastAPI-motor-oil` is halfway between an object document mapper (based on `Pydantic`) and a database driver (by wrapping the async `motor` driver).\n\nSee the [full documentation here](https://volfpeter.github.io/fastapi-motor-oil/).\n\n## Installation\n\nThe library is available on PyPI and can be installed with:\n\n```console\n$ pip install fastapi-motor-oil\n```\n\n## Example\n\nPrerequisites:\n\n- MongoDB (e.g. the Community Edition) installed and running locally;\n- `fastapi` with all its dependencies (`pip install fastapi[all]`);\n- This library (`pip install fastapi-motor-oil`).\n\nIn this example we will create:\n\n- a simple `TreeNode` document model with a `name` and an optional reference to a `parent` node and some delete rules;\n- the services that are necessary to create, read, update, and delete documents;\n- a `fastapi` `APIRouter` factory that can be included in `fastapi` applications;\n- and the `fastapi` application itself.\n\nThe project layout under your root directory will be as follows:\n\n- `/tree_app`\n  - `__init__.py`\n  - `api.py`\n  - `main.py`\n  - `model.py`\n  - `service.py`\n\nModel definitions (in `model.py`):\n\n```python\nfrom fastapi_motor_oil import DocumentModel, StrObjectId, UTCDatetime\nfrom pydantic import BaseModel\n\nclass TreeNode(DocumentModel):\n    """\n    Tree node document model.\n    """\n\n    name: str\n    parent: StrObjectId | None\n    created_at: UTCDatetime\n\nclass TreeNodeCreate(BaseModel):\n    """\n    Tree node creation model.\n    """\n\n    name: str\n    parent: StrObjectId | None\n\nclass TreeNodeUpdate(BaseModel):\n    """\n    Tree node update model.\n    """\n\n    name: str | None\n    parent: StrObjectId | None\n\n```\n\nService implementation (in `service.py`):\n\n```python\nfrom typing import Any\nfrom collections.abc import Sequence\nfrom datetime import datetime, timezone\n\nfrom bson import ObjectId\nfrom fastapi_motor_oil import (\n    CollectionOptions,\n    MongoQuery,\n    MongoService,\n    delete_rule,\n    validator,\n)\nfrom motor.core import AgnosticClientSession\n\nfrom .model import TreeNodeCreate, TreeNodeUpdate\n\nclass TreeNodeService(MongoService[TreeNodeCreate, TreeNodeUpdate]):\n    """\n    Tree node database services.\n    """\n\n    __slots__ = ()\n\n    collection_name: str = "tree_nodes"\n\n    collection_options: CollectionOptions | None = None\n\n    @delete_rule("pre")  # Delete rule that remove the subtrees of deleted nodes.\n    async def dr_delete_subtree(\n        self, session: AgnosticClientSession, ids: Sequence[ObjectId]\n    ) -> None:\n        child_ids = await self.find_ids({"parent": {"$in": ids}}, session=session)\n        if len(child_ids) > 0:\n            # Recursion\n            await self.delete_many(\n                {"_id": {"$in": child_ids}}, options={"session": session}\n            )\n\n    @delete_rule("deny")  # Delete rule that prevents the removal of root nodes.\n    async def dr_deny_if_root(\n        self, session: AgnosticClientSession, ids: Sequence[ObjectId]\n    ) -> None:\n        root_cnt = await self.count_documents(\n            {"$and": [{"_id": {"$in": ids}}, {"parent": None}]},\n            options={"session": session},\n        )\n        if root_cnt > 0:\n            raise ValueError("Can not delete root nodes.")\n\n    @validator("insert-update")\n    async def v_parent_valid(\n        self, query: MongoQuery | None, data: TreeNodeCreate | TreeNodeUpdate\n    ) -> None:\n        if data.parent is None:  # No parent node is always fine\n            return\n\n        if not await self.exists(data.parent):  # Parent must exist.\n            raise ValueError("Parent does not exist.")\n\n        if isinstance(data, TreeNodeCreate):  # No more checks during creation.\n            return\n\n        matched_ids = (\n            (await self.find_ids(query)) if isinstance(data, TreeNodeUpdate) else []\n        )\n        if data.parent in matched_ids:  # Self reference is forbidden.\n            raise ValueError("Self-reference.")\n\n    async def _convert_for_insert(self, data: TreeNodeCreate) -> dict[str, Any]:\n        return {\n            **(await super()._convert_for_insert(data)),\n            "created_at": datetime.now(timezone.utc),\n        }\n```\n\nRouting implementation (in `api.py`):\n\n```python\nfrom typing import Any\n\nfrom fastapi import APIRouter, Depends, HTTPException, status\nfrom fastapi_motor_oil import (\n    AgnosticDatabase,\n    DatabaseProvider,\n    DeleteError,\n    DeleteResultModel,\n    StrObjectId,\n)\n\nfrom .model import TreeNode, TreeNodeCreate, TreeNodeUpdate\nfrom .service import TreeNodeService\n\ndef make_api(\n    *,\n    get_database: DatabaseProvider,\n    prefix: str = "/tree-node",\n) -> APIRouter:\n    """\n    Tree node `APIRouter` factory.\n\n    Arguments:\n        get_database: FastAPI dependency that returns the `AgnosticDatabase`\n                      database instance for the API.\n        prefix: The prefix for the created `APIRouter`.\n\n    Returns:\n        The created `APIRouter` instance.\n    """\n    api = APIRouter(prefix=prefix)\n\n    @api.get("/", response_model=list[TreeNode])\n    async def get_all(\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> list[dict[str, Any]]:\n        svc = TreeNodeService(database)\n        return [d async for d in svc.find()]\n\n    @api.post("/", response_model=TreeNode)\n    async def create(\n        data: TreeNodeCreate,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> dict[str, Any]:\n        svc = TreeNodeService(database)\n\n        try:\n            result = await svc.insert_one(data)\n        except Exception:\n            raise HTTPException(\n                status_code=status.HTTP_400_BAD_REQUEST, detail="Creation failed."\n            )\n\n        if (created := await svc.get_by_id(result.inserted_id)) is not None:\n            return created\n\n        raise HTTPException(status.HTTP_409_CONFLICT)\n\n    @api.get("/{id}", response_model=TreeNode)\n    async def get_by_id(\n        id: StrObjectId,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> dict[str, Any]:\n        svc = TreeNodeService(database)\n        if (result := await svc.get_by_id(id)) is not None:\n            return result\n\n        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=str(id))\n\n    @api.put("/{id}", response_model=TreeNode)\n    async def update_by_id(\n        id: StrObjectId,\n        data: TreeNodeUpdate,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> dict[str, Any]:\n        svc = TreeNodeService(database)\n\n        try:\n            result = await svc.update_by_id(id, data)\n        except Exception:\n            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=str(id))\n\n        if result.matched_count == 0:\n            raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))\n\n        if (updated := await svc.get_by_id(id)) is not None:\n            return updated\n\n        raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))\n\n    @api.delete("/{id}", response_model=DeleteResultModel)\n    async def delete_by_id(\n        id: StrObjectId,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> DeleteResultModel:\n        svc = TreeNodeService(database)\n        try:\n            result = await svc.delete_by_id(id)\n        except DeleteError:\n            raise HTTPException(status.HTTP_400_BAD_REQUEST, detail=str(id))\n        if result.deleted_count == 0:\n            raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))\n\n        return DeleteResultModel(delete_count=result.deleted_count)\n\n    return api\n```\n\nApplication (in `main.py`):\n\n```python\nfrom functools import lru_cache\n\nfrom fastapi import FastAPI\nfrom motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorDatabase\n\n@lru_cache(maxsize=1)\ndef get_database() -> AsyncIOMotorDatabase:\n    """Database provider dependency for the created API."""\n    mongo_connection_string = "mongodb://127.0.0.1:27017"\n    database_name = "tree-db"\n    client = AsyncIOMotorClient(mongo_connection_string)\n    return client[database_name]\n\ndef register_routes(app: FastAPI) -> None:\n    """Registers all routes of the application."""\n    from .api import make_api as make_tree_node_api\n\n    api_prefix = "/api/v1"\n\n    app.include_router(\n        make_tree_node_api(get_database=get_database),\n        prefix=api_prefix,\n    )\n\ndef create_app() -> FastAPI:\n    app = FastAPI()\n\n    register_routes(app)\n\n    return app\n```\n\nWith everything in place, you can serve the application by executing `uvicorn tree_app.main:create_app --reload --factory` in your root directory. Go to [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) in the browser to see and try the created REST API.\n\n## Requirements\n\nThe project depends on `motor` (the official asyncio MongoDB driver, which is built on top of `pymongo` and `bson`) and `pydantic`.\n\n`fastapi` is not an actual dependency, but the code was written with `fastapi` applications with a REST API in mind.\n\n## Development\n\nUse `black` for code formatting and `mypy` for static code analysis.\n\n## Contributing\n\nContributions are welcome.\n\n## License - MIT\n\nThe library is open-sourced under the conditions of the [MIT license](https://choosealicense.com/licenses/mit/).\n',
+    'long_description': '# FastAPI-motor-oil\n\n`FastAPI-motor-oil` is a collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a [FastAPI](https://fastapi.tiangolo.com/).\n\nKey features:\n\n- Database **model** design with `Pydantic`.\n- Relationship support and validation using async **validators and delete rules** with a declarative, decorator-based syntax.\n- Declarative **index** specification.\n- Typed **utilities** for convenient model and API creation.\n- Ready to use, customizable **async service layer** with **transaction support** that integrates all the above to keep your API and business logic clean, flexible, and easy to understand.\n\nBy providing a convenient, declarative middle layer between MongoDB and your API, `FastAPI-motor-oil` is halfway between an object document mapper (based on `Pydantic`) and a database driver (by wrapping the official, async `motor` driver).\n\nSee the [full documentation here](https://volfpeter.github.io/fastapi-motor-oil/).\n\n## Installation\n\nThe library is available on PyPI and can be installed with:\n\n```console\n$ pip install fastapi-motor-oil\n```\n\n## Example\n\nPrerequisites:\n\n- MongoDB (e.g. the Community Edition) installed and running locally;\n- `fastapi` with all its dependencies (`pip install fastapi[all]`);\n- This library (`pip install fastapi-motor-oil`).\n\nIn this example we will create:\n\n- a simple `TreeNode` document model with a `name` and an optional reference to a `parent` node and some delete rules;\n- the services that are necessary to create, read, update, and delete documents;\n- a `fastapi` `APIRouter` factory that can be included in `fastapi` applications;\n- and the `fastapi` application itself.\n\nThe project layout under your root directory will be as follows:\n\n- `/tree_app`\n  - `__init__.py`\n  - `api.py`\n  - `main.py`\n  - `model.py`\n  - `service.py`\n\nModel definitions (in `model.py`):\n\n```python\nfrom fastapi_motor_oil import DocumentModel, StrObjectId, UTCDatetime\nfrom pydantic import BaseModel\n\nclass TreeNode(DocumentModel):\n    """\n    Tree node document model.\n    """\n\n    name: str\n    parent: StrObjectId | None\n    created_at: UTCDatetime\n\nclass TreeNodeCreate(BaseModel):\n    """\n    Tree node creation model.\n    """\n\n    name: str\n    parent: StrObjectId | None\n\nclass TreeNodeUpdate(BaseModel):\n    """\n    Tree node update model.\n    """\n\n    name: str | None\n    parent: StrObjectId | None\n\n```\n\nService implementation (in `service.py`):\n\n```python\nfrom typing import Any\nfrom collections.abc import Sequence\nfrom datetime import datetime, timezone\n\nfrom bson import ObjectId\nfrom fastapi_motor_oil import (\n    CollectionOptions,\n    MongoQuery,\n    MongoService,\n    delete_rule,\n    validator,\n)\nfrom motor.core import AgnosticClientSession\n\nfrom .model import TreeNodeCreate, TreeNodeUpdate\n\nclass TreeNodeService(MongoService[TreeNodeCreate, TreeNodeUpdate]):\n    """\n    Tree node database services.\n    """\n\n    __slots__ = ()\n\n    collection_name: str = "tree_nodes"\n\n    collection_options: CollectionOptions | None = None\n\n    @delete_rule("pre")  # Delete rule that remove the subtrees of deleted nodes.\n    async def dr_delete_subtree(\n        self, session: AgnosticClientSession, ids: Sequence[ObjectId]\n    ) -> None:\n        child_ids = await self.find_ids({"parent": {"$in": ids}}, session=session)\n        if len(child_ids) > 0:\n            # Recursion\n            await self.delete_many(\n                {"_id": {"$in": child_ids}}, options={"session": session}\n            )\n\n    @delete_rule("deny")  # Delete rule that prevents the removal of root nodes.\n    async def dr_deny_if_root(\n        self, session: AgnosticClientSession, ids: Sequence[ObjectId]\n    ) -> None:\n        root_cnt = await self.count_documents(\n            {"$and": [{"_id": {"$in": ids}}, {"parent": None}]},\n            options={"session": session},\n        )\n        if root_cnt > 0:\n            raise ValueError("Can not delete root nodes.")\n\n    @validator("insert-update")\n    async def v_parent_valid(\n        self, query: MongoQuery | None, data: TreeNodeCreate | TreeNodeUpdate\n    ) -> None:\n        if data.parent is None:  # No parent node is always fine\n            return\n\n        if not await self.exists(data.parent):  # Parent must exist.\n            raise ValueError("Parent does not exist.")\n\n        if isinstance(data, TreeNodeCreate):  # No more checks during creation.\n            return\n\n        matched_ids = (\n            (await self.find_ids(query)) if isinstance(data, TreeNodeUpdate) else []\n        )\n        if data.parent in matched_ids:  # Self reference is forbidden.\n            raise ValueError("Self-reference.")\n\n    async def _convert_for_insert(self, data: TreeNodeCreate) -> dict[str, Any]:\n        return {\n            **(await super()._convert_for_insert(data)),\n            "created_at": datetime.now(timezone.utc),\n        }\n```\n\nRouting implementation (in `api.py`):\n\n```python\nfrom typing import Any\n\nfrom fastapi import APIRouter, Depends, HTTPException, status\nfrom fastapi_motor_oil import (\n    AgnosticDatabase,\n    DatabaseProvider,\n    DeleteError,\n    DeleteResultModel,\n    StrObjectId,\n)\n\nfrom .model import TreeNode, TreeNodeCreate, TreeNodeUpdate\nfrom .service import TreeNodeService\n\ndef make_api(\n    *,\n    get_database: DatabaseProvider,\n    prefix: str = "/tree-node",\n) -> APIRouter:\n    """\n    Tree node `APIRouter` factory.\n\n    Arguments:\n        get_database: FastAPI dependency that returns the `AgnosticDatabase`\n                      database instance for the API.\n        prefix: The prefix for the created `APIRouter`.\n\n    Returns:\n        The created `APIRouter` instance.\n    """\n    api = APIRouter(prefix=prefix)\n\n    @api.get("/", response_model=list[TreeNode])\n    async def get_all(\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> list[dict[str, Any]]:\n        svc = TreeNodeService(database)\n        return [d async for d in svc.find()]\n\n    @api.post("/", response_model=TreeNode)\n    async def create(\n        data: TreeNodeCreate,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> dict[str, Any]:\n        svc = TreeNodeService(database)\n\n        try:\n            result = await svc.insert_one(data)\n        except Exception:\n            raise HTTPException(\n                status_code=status.HTTP_400_BAD_REQUEST, detail="Creation failed."\n            )\n\n        if (created := await svc.get_by_id(result.inserted_id)) is not None:\n            return created\n\n        raise HTTPException(status.HTTP_409_CONFLICT)\n\n    @api.get("/{id}", response_model=TreeNode)\n    async def get_by_id(\n        id: StrObjectId,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> dict[str, Any]:\n        svc = TreeNodeService(database)\n        if (result := await svc.get_by_id(id)) is not None:\n            return result\n\n        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=str(id))\n\n    @api.put("/{id}", response_model=TreeNode)\n    async def update_by_id(\n        id: StrObjectId,\n        data: TreeNodeUpdate,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> dict[str, Any]:\n        svc = TreeNodeService(database)\n\n        try:\n            result = await svc.update_by_id(id, data)\n        except Exception:\n            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=str(id))\n\n        if result.matched_count == 0:\n            raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))\n\n        if (updated := await svc.get_by_id(id)) is not None:\n            return updated\n\n        raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))\n\n    @api.delete("/{id}", response_model=DeleteResultModel)\n    async def delete_by_id(\n        id: StrObjectId,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> DeleteResultModel:\n        svc = TreeNodeService(database)\n        try:\n            result = await svc.delete_by_id(id)\n        except DeleteError:\n            raise HTTPException(status.HTTP_400_BAD_REQUEST, detail=str(id))\n        if result.deleted_count == 0:\n            raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))\n\n        return DeleteResultModel(delete_count=result.deleted_count)\n\n    return api\n```\n\nApplication (in `main.py`):\n\n```python\nfrom functools import lru_cache\n\nfrom fastapi import FastAPI\nfrom motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorDatabase\n\n@lru_cache(maxsize=1)\ndef get_database() -> AsyncIOMotorDatabase:\n    """Database provider dependency for the created API."""\n    mongo_connection_string = "mongodb://127.0.0.1:27017"\n    database_name = "tree-db"\n    client = AsyncIOMotorClient(mongo_connection_string)\n    return client[database_name]\n\ndef register_routes(app: FastAPI) -> None:\n    """Registers all routes of the application."""\n    from .api import make_api as make_tree_node_api\n\n    api_prefix = "/api/v1"\n\n    app.include_router(\n        make_tree_node_api(get_database=get_database),\n        prefix=api_prefix,\n    )\n\ndef create_app() -> FastAPI:\n    app = FastAPI()\n\n    register_routes(app)\n\n    return app\n```\n\nWith everything in place, you can serve the application by executing `uvicorn tree_app.main:create_app --reload --factory` in your root directory. Go to [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) in the browser to see and try the created REST API.\n\n## Requirements\n\nThe project depends on `motor` (the official asyncio MongoDB driver, which is built on top of `pymongo` and `bson`) and `pydantic`.\n\n`fastapi` is not an actual dependency, but the code was written with `fastapi` applications with a REST API in mind.\n\n## Development\n\nUse `black` for code formatting and `mypy` for static code analysis.\n\n## Contributing\n\nContributions are welcome.\n\n## License - MIT\n\nThe library is open-sourced under the conditions of the [MIT license](https://choosealicense.com/licenses/mit/).\n',
     'author': 'Peter Volf',
     'author_email': 'do.volfp@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fastapi_motor_oil-0.5.0/PKG-INFO` & `fastapi_motor_oil-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-motor-oil
-Version: 0.5.0
+Version: 0.5.1
 Summary: Collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a FastAPI.
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,18 +16,19 @@
 
 `FastAPI-motor-oil` is a collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a [FastAPI](https://fastapi.tiangolo.com/).
 
 Key features:
 
 - Database **model** design with `Pydantic`.
 - Relationship support and validation using async **validators and delete rules** with a declarative, decorator-based syntax.
+- Declarative **index** specification.
 - Typed **utilities** for convenient model and API creation.
-- A complete and customizable **async service layer** with **transaction support** that integrates all the above to keep your API and business logic clean, flexible, and easy to understand.
+- Ready to use, customizable **async service layer** with **transaction support** that integrates all the above to keep your API and business logic clean, flexible, and easy to understand.
 
-By providing a convenient, declarative middle layer between MongoDB and your API, `FastAPI-motor-oil` is halfway between an object document mapper (based on `Pydantic`) and a database driver (by wrapping the async `motor` driver).
+By providing a convenient, declarative middle layer between MongoDB and your API, `FastAPI-motor-oil` is halfway between an object document mapper (based on `Pydantic`) and a database driver (by wrapping the official, async `motor` driver).
 
 See the [full documentation here](https://volfpeter.github.io/fastapi-motor-oil/).
 
 ## Installation
 
 The library is available on PyPI and can be installed with:
```

