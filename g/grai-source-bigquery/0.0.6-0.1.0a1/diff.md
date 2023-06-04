# Comparing `tmp/grai_source_bigquery-0.0.6.tar.gz` & `tmp/grai_source_bigquery-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_bigquery-0.0.6.tar", max compression
+gzip compressed data, was "grai_source_bigquery-0.1.0a1.tar", max compression
```

## Comparing `grai_source_bigquery-0.0.6.tar` & `grai_source_bigquery-0.1.0a1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      141 2023-04-30 17:49:45.930311 grai_source_bigquery-0.0.6/README.md
--rw-r--r--   0        0        0      932 2023-05-18 16:41:43.962977 grai_source_bigquery-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      145 2023-02-13 20:16:22.712224 grai_source_bigquery-0.0.6/src/grai_source_bigquery/__init__.py
--rw-r--r--   0        0        0     6659 2023-04-29 00:19:10.365235 grai_source_bigquery-0.0.6/src/grai_source_bigquery/adapters.py
--rw-r--r--   0        0        0     1192 2023-02-13 20:16:22.712633 grai_source_bigquery-0.0.6/src/grai_source_bigquery/base.py
--rw-r--r--   0        0        0     5672 2023-05-18 17:01:19.338830 grai_source_bigquery-0.0.6/src/grai_source_bigquery/loader.py
--rw-r--r--   0        0        0     4814 2023-05-18 16:40:46.483832 grai_source_bigquery-0.0.6/src/grai_source_bigquery/models.py
--rw-r--r--   0        0        0      186 2023-02-13 20:16:22.713174 grai_source_bigquery-0.0.6/src/grai_source_bigquery/package_definitions.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.6/setup.py
--rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-02 08:01:59.695304 grai_source_bigquery-0.1.0a1/README.md
+-rw-r--r--   0        0        0      971 2023-06-04 15:51:10.689502 grai_source_bigquery-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-02-14 12:06:39.088033 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/__init__.py
+-rw-r--r--   0        0        0     8578 2023-06-02 08:26:06.787907 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/adapters.py
+-rw-r--r--   0        0        0     2124 2023-06-04 15:50:44.843872 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/base.py
+-rw-r--r--   0        0        0    12864 2023-06-04 15:50:44.997687 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/loader.py
+-rw-r--r--   0        0        0     6120 2023-06-04 15:50:44.919123 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/models.py
+-rw-r--r--   0        0        0      199 2023-06-02 08:26:06.789100 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/package_definitions.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 grai_source_bigquery-0.1.0a1/PKG-INFO
```

### Comparing `grai_source_bigquery-0.0.6/pyproject.toml` & `grai_source_bigquery-0.1.0a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_bigquery"
-version = "0.0.6"
+version = "0.1.0-alpha1"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_bigquery", from = "src" },
 ]
 readme = "README.md"
@@ -16,14 +16,15 @@
 python = "^3.8"
 pydantic = "^1.9.1"
 grai-client = "^0.2.0"
 multimethod = "^1.8"
 grai-schemas = "^0.1.9"
 google-cloud-bigquery = "^3.5.0"
 setuptools = "^67.1.0"
+google-cloud-logging = "^3.5.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.10.1"
 pytest = "^7.2.0"
 python-dotenv = "^0.21.1"
```

### Comparing `grai_source_bigquery-0.0.6/src/grai_source_bigquery/adapters.py` & `grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/adapters.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,19 +25,41 @@
     TableID,
 )
 from grai_source_bigquery.package_definitions import config
 
 
 @multimethod
 def build_grai_metadata(current: Any, desired: Any) -> BaseModel:
+    """
+
+    Args:
+        current (Any):
+        desired (Any):
+
+    Returns:
+
+    Raises:
+
+    """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_grai_metadata.register
 def build_grai_metadata_from_column(current: Column, version: Literal["v1"] = "v1") -> ColumnMetadata:
+    """
+
+    Args:
+        current (Column):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
     default_value = current.default_value
     if current.default_value is not None:
         default_value = DefaultValue(
             has_default_value=True,
             default_value=current.default_value,
             data_type=current.data_type,
         )
@@ -55,26 +77,48 @@
         "tags": [config.metadata_id],
     }
     return ColumnMetadata(**data)
 
 
 @build_grai_metadata.register
 def build_grai_metadata_from_table(current: Table, version: Literal["v1"] = "v1") -> TableMetadata:
+    """
+
+    Args:
+        current (Table):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
     data = {
         "version": version,
         "node_type": NodeTypeLabels.table.value,
         "node_attributes": {},
         "tags": [config.metadata_id],
     }
 
     return TableMetadata(**data)
 
 
 @build_grai_metadata.register
 def build_grai_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> GenericEdgeMetadataV1:
+    """
+
+    Args:
+        current (Edge):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
     data = {"version": version, "tags": [config.metadata_id]}
 
     if isinstance(current.source, TableID):
         if isinstance(current.destination, ColumnID):
             data["edge_type"] = EdgeTypeLabels.table_to_column.value
             return TableToColumnMetadata(**data)
         elif isinstance(current.destination, TableID):
@@ -90,80 +134,168 @@
 
 
 # ---
 
 
 @multimethod
 def build_app_metadata(current: Any, desired: Any) -> None:
+    """
+
+    Args:
+        current (Any):
+        desired (Any):
+
+    Returns:
+
+    Raises:
+
+    """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_app_metadata.register
 def build_metadata_from_column(current: Column, version: Literal["v1"] = "v1") -> Dict:
+    """
+
+    Args:
+        current (Column):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
     data = {
         "table_name": current.table,
         "schema": current.column_schema,
     }
 
     return data
 
 
 @build_app_metadata.register
 def build_metadata_from_table(current: Table, version: Literal["v1"] = "v1") -> Dict:
+    """
+
+    Args:
+        current (Table):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
     data = {
         "schema": current.table_schema,
         "table_type": current.table_type.value,
     }
     return data
 
 
 @build_app_metadata.register
 def build_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> Dict:
+    """
+
+    Args:
+        current (Edge):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
     data = {
         "definition": current.definition,
         "constraint_type": current.constraint_type.value,
     }
     data |= current.metadata if current.metadata is not None else {}
 
     return data
 
 
 # ---
 
 
 def build_metadata(obj, version):
+    """
+
+    Args:
+        obj:
+        version:
+
+    Returns:
+
+    Raises:
+
+    """
     integration_meta = build_app_metadata(obj, version)
     base_metadata = build_grai_metadata(obj, version)
     integration_meta["grai"] = base_metadata
 
     return {
         base_config.metadata_id: base_metadata,
         config.metadata_id: integration_meta,
     }
 
 
 @multimethod
 def adapt_to_client(current: Any, desired: Any) -> Union[NodeV1, EdgeV1]:
+    """
+
+    Args:
+        current (Any):
+        desired (Any):
+
+    Returns:
+
+    Raises:
+
+    """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
 
 
 @adapt_to_client.register
 def adapt_column_to_client(current: Column, version: Literal["v1"] = "v1") -> NodeV1:
+    """
+
+    Args:
+        current (Column):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
     spec_dict = {
         "name": current.full_name,
         "namespace": current.namespace,
         "display_name": current.name,
         "data_source": config.integration_name,
         "metadata": build_metadata(current, version),
     }
     return Schema.to_model(spec_dict, version=version, typing_type="Node")
 
 
 @adapt_to_client.register
 def adapt_table_to_client(current: Table, version: Literal["v1"] = "v1") -> NodeV1:
+    """
+
+    Args:
+        current (Table):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
     metadata = {
         "node_type": NodeTypeLabels.table.value,
         "schema": current.table_schema,
     }
     spec_dict = {
         "name": current.full_name,
         "namespace": current.namespace,
@@ -172,21 +304,43 @@
         "metadata": build_metadata(current, version),
     }
     metadata.update(current.metadata)
     return Schema.to_model(spec_dict, version=version, typing_type="Node")
 
 
 def make_name(node1: ID, node2: ID) -> str:
+    """
+
+    Args:
+        node1 (ID):
+        node2 (ID):
+
+    Returns:
+
+    Raises:
+
+    """
     node1_name = f"{node1.namespace}:{node1.full_name}"
     node2_name = f"{node2.namespace}:{node2.full_name}"
     return f"{node1_name} -> {node2_name}"
 
 
 @adapt_to_client.register
 def adapt_edge_to_client(current: Edge, version: Literal["v1"] = "v1") -> EdgeV1:
+    """
+
+    Args:
+        current (Edge):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
     spec_dict = {
         "data_source": config.integration_name,
         "name": make_name(current.source, current.destination),
         "namespace": current.source.namespace,
         "source": {
             "name": current.source.full_name,
             "namespace": current.source.namespace,
@@ -198,8 +352,19 @@
         "metadata": build_metadata(current, version),
     }
     return Schema.to_model(spec_dict, version=version, typing_type="Edge")
 
 
 @adapt_to_client.register
 def adapt_list_to_client(objs: Sequence, version: Literal["v1"]) -> List:
+    """
+
+    Args:
+        objs (Sequence):
+        version (Literal["v1"]):
+
+    Returns:
+
+    Raises:
+
+    """
     return [adapt_to_client(item, version) for item in objs]
```

### Comparing `grai_source_bigquery-0.0.6/src/grai_source_bigquery/models.py` & `grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,132 +1,248 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, root_validator, validator
 
 
 class BigqueryNode(BaseModel):
+    """ """
+
     pass
 
 
 class ID(BigqueryNode):
+    """ """
+
     name: str
     namespace: str
     full_name: str
 
     class Config:
+        """ """
+
         extra = "forbid"
 
 
 class TableID(ID):
+    """ """
+
     table_schema: str
 
     @root_validator(pre=True)
     def make_full_name(cls, values: Dict) -> Dict:
+        """
+
+        Args:
+            values (Dict):
+
+        Returns:
+
+        Raises:
+
+        """
         if values.get("full_name", None) is None:
             values["full_name"] = f"{values['table_schema']}.{values['name']}"
         return values
 
 
 class ColumnID(ID):
+    """ """
+
     table_schema: str
     table_name: str
 
     @root_validator(pre=True)
     def make_full_name(cls, values: Dict) -> Dict:
+        """
+
+        Args:
+            values (Dict):
+
+        Returns:
+
+        Raises:
+
+        """
         full_name = values.get("full_name", None)
         if values.get("full_name", None) is None:
             values["full_name"] = f"{values['table_schema']}.{values['table_name']}.{values['name']}"
         return values
 
     @validator("table_name")
     def validate_name(cls, value):
+        """
+
+        Args:
+            value:
+
+        Returns:
+
+        Raises:
+
+        """
         if value.startswith('"') and value.endswith('"'):
             return value
         return value.lower()
 
 
 class Column(BigqueryNode):
+    """ """
+
     name: str = Field(alias="column_name")
     table: str
     column_schema: str = Field(alias="schema")
     data_type: str
     is_nullable: bool
     namespace: str
     default_value: Any = Field(alias="column_default")
     is_pk: Optional[bool]
     full_name: Optional[str] = None
 
     class Config:
+        """ """
+
         allow_population_by_field_name = True
 
     @validator("full_name", always=True)
     def make_full_name(cls, full_name: Optional[str], values: Dict) -> str:
+        """
+
+        Args:
+            full_name (Optional[str]):
+            values (Dict):
+
+        Returns:
+
+        Raises:
+
+        """
         if full_name is not None:
             return full_name
         result = f"{values['column_schema']}.{values['table']}.{values['name']}"
         return result
 
     @validator("name")
     def validate_name(cls, value):
+        """
+
+        Args:
+            value:
+
+        Returns:
+
+        Raises:
+
+        """
         if value.startswith('"') and value.endswith('"'):
             return value
         return value.lower()
 
 
 class Constraint(str, Enum):
+    """ """
+
     foreign_key = "f"
     primary_key = "p"
     belongs_to = "bt"
+    bigquery_model = "bqm"
 
 
 class Edge(BaseModel):
+    """ """
+
     source: Union[ColumnID, TableID]
     destination: Union[ColumnID, TableID]
     definition: Optional[str]
     constraint_type: Constraint
     metadata: Optional[Dict] = None
 
+    def __hash__(self):
+        """
+
+        Returns:
+
+        Raises:
+
+        """
+        return hash((self.source.full_name, self.destination.full_name, self.constraint_type))
+
 
 class TableType(str, Enum):
+    """ """
+
     Table = "BASE TABLE"
     Clone = "CLONE"
     Snapshot = "SNAPSHOT"
     View = "VIEW"
     Materialized_View = "MATERIALIZED VIEW"
     External = "EXTERNAL"
 
 
 class Table(BigqueryNode):
+    """ """
+
     name: str = Field(alias="table_name")
     table_schema: str = Field(alias="schema")
     table_type: TableType
     table_dataset: str
     namespace: str
     columns: List[Column] = []
     metadata: Dict = {}
     full_name: Optional[str] = None
 
     class Config:
+        """ """
+
         allow_population_by_field_name = True
 
     @validator("full_name", always=True)
     def make_full_name(cls, full_name: Optional[str], values: Dict) -> str:
+        """
+
+        Args:
+            full_name (Optional[str]):
+            values (Dict):
+
+        Returns:
+
+        Raises:
+
+        """
         if full_name is not None:
             return full_name
 
         return f"{values['table_schema']}.{values['name']}"
 
     @validator("name")
     def validate_name(cls, value):
+        """
+
+        Args:
+            value:
+
+        Returns:
+
+        Raises:
+
+        """
         if value.startswith('"') and value.endswith('"'):
             return value
         return value.lower()
 
     def get_edges(self) -> List[Edge]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         return [
             Edge(
                 constraint_type=Constraint("bt"),
                 source=TableID(
                     table_schema=self.table_schema,
                     name=self.name,
                     namespace=self.namespace,
@@ -139,26 +255,37 @@
                 ),
             )
             for column in self.columns
         ]
 
 
 class EdgeQuery(BaseModel):
+    """ """
+
     namespace: str
     constraint_name: str
     constraint_type: str
     self_schema: str
     self_table: str
     self_columns: List[str]
     foreign_schema: str
     foreign_table: str
     foreign_columns: List[str]
     definition: str
 
     def to_edge(self) -> Optional[Edge]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         if not len(self.self_columns) == 1 and len(self.foreign_columns) == 1:
             return None
 
         destination = ColumnID(
             table_schema=self.self_schema,
             table_name=self.self_table,
             name=self.self_columns[0],
```

### Comparing `grai_source_bigquery-0.0.6/PKG-INFO` & `grai_source_bigquery-0.1.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: grai-source-bigquery
-Version: 0.0.6
+Version: 0.1.0a1
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-cloud-bigquery (>=3.5.0,<4.0.0)
+Requires-Dist: google-cloud-logging (>=3.5.0,<4.0.0)
 Requires-Dist: grai-client (>=0.2.0,<0.3.0)
 Requires-Dist: grai-schemas (>=0.1.9,<0.2.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: setuptools (>=67.1.0,<68.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-bigquery
```

