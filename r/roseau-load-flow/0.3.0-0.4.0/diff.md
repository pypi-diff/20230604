# Comparing `tmp/roseau_load_flow-0.3.0.tar.gz` & `tmp/roseau_load_flow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roseau_load_flow-0.3.0.tar", max compression
+gzip compressed data, was "roseau_load_flow-0.4.0.tar", max compression
```

## Comparing `roseau_load_flow-0.3.0.tar` & `roseau_load_flow-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1506 2023-02-21 17:58:50.446091 roseau_load_flow-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     1298 2023-02-21 17:58:50.446091 roseau_load_flow-0.3.0/README.md
--rw-r--r--   0        0        0     3060 2023-02-21 17:58:50.478091 roseau_load_flow-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      379 2023-02-21 17:58:50.478091 roseau_load_flow-0.3.0/roseau/load_flow/__about__.py
--rw-r--r--   0        0        0     1850 2023-02-21 17:58:50.478091 roseau_load_flow-0.3.0/roseau/load_flow/__init__.py
--rw-r--r--   0        0        0     6222 2023-02-21 17:58:50.478091 roseau_load_flow-0.3.0/roseau/load_flow/converters.py
--rw-r--r--   0        0        0     4274 2023-02-21 17:58:50.478091 roseau_load_flow-0.3.0/roseau/load_flow/exceptions.py
--rw-r--r--   0        0        0      464 2023-02-21 17:58:50.478091 roseau_load_flow-0.3.0/roseau/load_flow/io/__init__.py
--rw-r--r--   0        0        0    14364 2023-02-21 17:58:50.478091 roseau_load_flow-0.3.0/roseau/load_flow/io/dgs.py
--rw-r--r--   0        0        0    15564 2023-02-21 17:58:50.478091 roseau_load_flow-0.3.0/roseau/load_flow/io/dict.py
--rw-r--r--   0        0        0     1247 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/__init__.py
--rw-r--r--   0        0        0     5312 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/branches.py
--rw-r--r--   0        0        0     5510 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/buses.py
--rw-r--r--   0        0        0     6740 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/core.py
--rw-r--r--   0        0        0     4069 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/grounds.py
--rw-r--r--   0        0        0      177 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/lines/__init__.py
--rw-r--r--   0        0        0    14887 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/lines/lines.py
--rw-r--r--   0        0        0    27238 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/lines/parameters.py
--rw-r--r--   0        0        0      351 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/loads/__init__.py
--rw-r--r--   0        0        0    32454 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/loads/flexible_parameters.py
--rw-r--r--   0        0        0    19075 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/loads/loads.py
--rw-r--r--   0        0        0     4036 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/potential_refs.py
--rw-r--r--   0        0        0     7316 2023-02-21 17:58:50.482091 roseau_load_flow-0.3.0/roseau/load_flow/models/sources.py
--rw-r--r--   0        0        0      219 2023-02-21 17:58:50.486091 roseau_load_flow-0.3.0/roseau/load_flow/models/transformers/__init__.py
--rw-r--r--   0        0        0     9756 2023-02-21 17:58:50.486091 roseau_load_flow-0.3.0/roseau/load_flow/models/transformers/parameters.py
--rw-r--r--   0        0        0     6974 2023-02-21 17:58:50.486091 roseau_load_flow-0.3.0/roseau/load_flow/models/transformers/transformers.py
--rw-r--r--   0        0        0    47471 2023-02-21 17:58:50.486091 roseau_load_flow-0.3.0/roseau/load_flow/network.py
--rw-r--r--   0        0        0     1271 2023-02-21 17:58:50.494090 roseau_load_flow-0.3.0/roseau/load_flow/typing.py
--rw-r--r--   0        0        0      517 2023-02-21 17:58:50.494090 roseau_load_flow-0.3.0/roseau/load_flow/units.py
--rw-r--r--   0        0        0      732 2023-02-21 17:58:50.494090 roseau_load_flow-0.3.0/roseau/load_flow/utils/__init__.py
--rw-r--r--   0        0        0     1002 2023-02-21 17:58:50.494090 roseau_load_flow-0.3.0/roseau/load_flow/utils/_versions.py
--rw-r--r--   0        0        0     2022 2023-02-21 17:58:50.494090 roseau_load_flow-0.3.0/roseau/load_flow/utils/constants.py
--rw-r--r--   0        0        0     4567 2023-02-21 17:58:50.494090 roseau_load_flow-0.3.0/roseau/load_flow/utils/mixins.py
--rw-r--r--   0        0        0    15765 2023-02-21 17:58:50.494090 roseau_load_flow-0.3.0/roseau/load_flow/utils/types.py
--rw-r--r--   0        0        0     2302 1970-01-01 00:00:00.000000 roseau_load_flow-0.3.0/setup.py
--rw-r--r--   0        0        0     2511 1970-01-01 00:00:00.000000 roseau_load_flow-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-02-21 17:58:50.446091 roseau_load_flow-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     2186 2023-06-04 16:06:36.162912 roseau_load_flow-0.4.0/README.md
+-rw-r--r--   0        0        0     3105 2023-06-04 16:06:36.198912 roseau_load_flow-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      379 2023-02-21 17:58:50.478091 roseau_load_flow-0.4.0/roseau/load_flow/__about__.py
+-rw-r--r--   0        0        0     1850 2023-02-21 17:58:50.478091 roseau_load_flow-0.4.0/roseau/load_flow/__init__.py
+-rw-r--r--   0        0        0     6222 2023-02-21 17:58:50.478091 roseau_load_flow-0.4.0/roseau/load_flow/converters.py
+-rw-r--r--   0        0        0     4380 2023-06-04 16:06:36.198912 roseau_load_flow-0.4.0/roseau/load_flow/exceptions.py
+-rw-r--r--   0        0        0      464 2023-02-21 17:58:50.478091 roseau_load_flow-0.4.0/roseau/load_flow/io/__init__.py
+-rw-r--r--   0        0        0    14411 2023-06-04 16:06:36.198912 roseau_load_flow-0.4.0/roseau/load_flow/io/dgs.py
+-rw-r--r--   0        0        0    15564 2023-02-21 17:58:50.478091 roseau_load_flow-0.4.0/roseau/load_flow/io/dict.py
+-rw-r--r--   0        0        0     1247 2023-02-21 17:58:50.482091 roseau_load_flow-0.4.0/roseau/load_flow/models/__init__.py
+-rw-r--r--   0        0        0     5341 2023-06-04 16:06:36.198912 roseau_load_flow-0.4.0/roseau/load_flow/models/branches.py
+-rw-r--r--   0        0        0     5539 2023-06-04 16:06:36.198912 roseau_load_flow-0.4.0/roseau/load_flow/models/buses.py
+-rw-r--r--   0        0        0     6740 2023-02-21 17:58:50.482091 roseau_load_flow-0.4.0/roseau/load_flow/models/core.py
+-rw-r--r--   0        0        0     4099 2023-06-04 16:06:36.198912 roseau_load_flow-0.4.0/roseau/load_flow/models/grounds.py
+-rw-r--r--   0        0        0      177 2023-02-21 17:58:50.482091 roseau_load_flow-0.4.0/roseau/load_flow/models/lines/__init__.py
+-rw-r--r--   0        0        0    14887 2023-02-21 17:58:50.482091 roseau_load_flow-0.4.0/roseau/load_flow/models/lines/lines.py
+-rw-r--r--   0        0        0    27278 2023-06-04 16:06:36.198912 roseau_load_flow-0.4.0/roseau/load_flow/models/lines/parameters.py
+-rw-r--r--   0        0        0      351 2023-02-21 17:58:50.482091 roseau_load_flow-0.4.0/roseau/load_flow/models/loads/__init__.py
+-rw-r--r--   0        0        0    36005 2023-06-04 16:06:36.198912 roseau_load_flow-0.4.0/roseau/load_flow/models/loads/flexible_parameters.py
+-rw-r--r--   0        0        0    19926 2023-06-04 16:06:36.198912 roseau_load_flow-0.4.0/roseau/load_flow/models/loads/loads.py
+-rw-r--r--   0        0        0     4066 2023-06-04 16:06:36.198912 roseau_load_flow-0.4.0/roseau/load_flow/models/potential_refs.py
+-rw-r--r--   0        0        0     7345 2023-06-04 16:06:36.198912 roseau_load_flow-0.4.0/roseau/load_flow/models/sources.py
+-rw-r--r--   0        0        0      219 2023-02-21 17:58:50.486091 roseau_load_flow-0.4.0/roseau/load_flow/models/transformers/__init__.py
+-rw-r--r--   0        0        0    10381 2023-06-04 16:06:36.202912 roseau_load_flow-0.4.0/roseau/load_flow/models/transformers/parameters.py
+-rw-r--r--   0        0        0     6974 2023-02-21 17:58:50.486091 roseau_load_flow-0.4.0/roseau/load_flow/models/transformers/transformers.py
+-rw-r--r--   0        0        0    60262 2023-06-04 16:06:36.202912 roseau_load_flow-0.4.0/roseau/load_flow/network.py
+-rw-r--r--   0        0        0     1905 2023-06-04 16:06:36.202912 roseau_load_flow-0.4.0/roseau/load_flow/solvers.py
+-rw-r--r--   0        0        0     1183 2023-06-04 16:06:36.202912 roseau_load_flow-0.4.0/roseau/load_flow/typing.py
+-rw-r--r--   0        0        0      517 2023-02-21 17:58:50.494090 roseau_load_flow-0.4.0/roseau/load_flow/units.py
+-rw-r--r--   0        0        0      734 2023-06-04 16:06:36.202912 roseau_load_flow-0.4.0/roseau/load_flow/utils/__init__.py
+-rw-r--r--   0        0        0     1002 2023-02-21 17:58:50.494090 roseau_load_flow-0.4.0/roseau/load_flow/utils/_versions.py
+-rw-r--r--   0        0        0     2035 2023-06-04 16:06:36.202912 roseau_load_flow-0.4.0/roseau/load_flow/utils/constants.py
+-rw-r--r--   0        0        0     4597 2023-06-04 16:06:36.202912 roseau_load_flow-0.4.0/roseau/load_flow/utils/mixins.py
+-rw-r--r--   0        0        0    15773 2023-06-04 16:06:36.206912 roseau_load_flow-0.4.0/roseau/load_flow/utils/types.py
+-rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 roseau_load_flow-0.4.0/PKG-INFO
```

### Comparing `roseau_load_flow-0.3.0/LICENSE.md` & `roseau_load_flow-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.3.0/pyproject.toml` & `roseau_load_flow-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "roseau_load_flow"
-version = "0.3.0"
-description = "Three-phase load flow solver"
+version = "0.4.0"
+description = "Highly capable three-phase load flow solver"
 authors = [
     "Ali Hamdan <ali.hamdan@roseautechnologies.com>",
     "Sébastien Vallet <sebastien.vallet@roseautechnologies.com>",
     "Benoît Vinot <benoit.vinot@roseautechnologies.com>",
     "Victor Gouin <victor.gouin@roseautechnologies.com>",
 ]
 maintainers = ["Ali Hamdan <ali.hamdan@roseautechnologies.com>"]
@@ -37,28 +37,29 @@
 numpy = ">=1.21.5"
 pandas = ">=1.4.0"
 geopandas = ">=0.10.2"
 shapely = ">=2.0.0"
 regex = ">=2022.1.18"
 requests = ">=2.28.1"
 pint = ">=0.19.2"
+typing-extensions = ">=4.6.2"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.1.0"
 requests-mock = "^1.9.3"
 coverage = { version = "^7.0.5", extras = ["toml"] }
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.0"
 black = { version = "^23.1.0", extras = ["jupyter"] }
 
 [tool.poetry.group.doc.dependencies]
-Sphinx = "^5.1.0"
+Sphinx = "^6.2.0"
 myst-parser = ">=0.16.1"
 sphinx-math-dollar = "^1.2.1"
 sphinx-autoapi = "^2.0.0"
 sphinx-copybutton = ">=0.5.1"
 sphinx-inline-tabs = ">=2022.1.2b11"
 jupyter = "^1.0.0"
 nbsphinx = ">=0.8.9"
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/__init__.py` & `roseau_load_flow-0.4.0/roseau/load_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/converters.py` & `roseau_load_flow-0.4.0/roseau/load_flow/converters.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/exceptions.py` & `roseau_load_flow-0.4.0/roseau/load_flow/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module contains the exceptions used by Roseau Load Flow.
 """
 import unicodedata
 from enum import Enum, auto
 from typing import Union
 
-from roseau.load_flow.typing import Self
+from typing_extensions import Self
 
 
 class RoseauLoadFlowExceptionCode(Enum):
     """Error codes used by Roseau Load Flow."""
 
     # Generic
     BAD_GEOMETRY_TYPE = auto()
@@ -30,15 +30,15 @@
     BAD_BRANCH_ID = auto()
     BAD_BRANCH_TYPE = auto()
     BAD_Z_LINE_SHAPE = auto()
     BAD_Y_SHUNT_SHAPE = auto()
     BAD_LINE_MODEL = auto()
     BAD_LINE_TYPE = auto()
     BAD_CONDUCTOR_TYPE = auto()
-    BAD_ISOLATION_TYPE = auto()
+    BAD_INSULATION_TYPE = auto()
     BAD_Z_LINE_VALUE = auto()
     BAD_Y_SHUNT_VALUE = auto()
     BAD_TRANSFORMER_WINDINGS = auto()
     BAD_TRANSFORMER_TYPE = auto()
     BAD_TRANSFORMER_VOLTAGES = auto()
     BAD_TRANSFORMER_PARAMETERS = auto()
     BAD_TYPE_NAME_SYNTAX = auto()
@@ -81,14 +81,19 @@
     NO_LOAD_FLOW_CONVERGENCE = auto()
     BAD_REQUEST = auto()
     BAD_LOAD_FLOW_RESULT = auto()
     LOAD_FLOW_NOT_RUN = auto()
     SEVERAL_NETWORKS = auto()
     TOO_MANY_BUSES = auto()
 
+    # Solver
+    BAD_SOLVER_NAME = auto()
+    BAD_SOLVER_PARAMS = auto()
+    NETWORK_SOLVER_MISMATCH = auto()
+
     # DGS export
     DGS_BAD_PHASE_TECHNOLOGY = auto()
     DGS_BAD_PHASE_NUMBER = auto()
 
     # JSON export
     JSON_LINE_PARAMETERS_DUPLICATES = auto()
     JSON_TRANSFORMER_PARAMETERS_DUPLICATES = auto()
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/io/dgs.py` & `roseau_load_flow-0.4.0/roseau/load_flow/io/dgs.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,21 +136,22 @@
                 xpn=typ_lne.at[type_id, "xpnline"],
                 bn=Q_(typ_lne.at[type_id, "bnline"], "uS/km"),
                 bpn=Q_(typ_lne.at[type_id, "bpnline"], "uS/km"),
             )
 
         for line_id in elm_lne.index:
             type_id = elm_lne.at[line_id, "typ_id"]  # id of the line type
+            lp = lines_params_dict[type_id]
             branches[line_id] = Line(
                 id=line_id,
                 bus1=buses[sta_cubic.at[elm_lne.at[line_id, "bus1"], "cterm"]],
                 bus2=buses[sta_cubic.at[elm_lne.at[line_id, "bus2"], "cterm"]],
                 length=elm_lne.at[line_id, "dline"],
-                parameters=lines_params_dict[type_id],
-                ground=ground,
+                parameters=lp,
+                ground=ground if lp.with_shunt else None,
             )
 
     # Transformers
     if elm_tr is not None:
         # Transformers type
         transformers_params_dict: dict[str, TransformerParameters] = {}
         transformers_tap: dict[str, int] = {}
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/io/dict.py` & `roseau_load_flow-0.4.0/roseau/load_flow/io/dict.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/__init__.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/branches.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/branches.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 from typing import Any, Optional, Union
 
 import numpy as np
 from shapely import LineString, Point
+from typing_extensions import Self
 
 from roseau.load_flow.converters import calculate_voltages
 from roseau.load_flow.models.buses import Bus
 from roseau.load_flow.models.core import Element
-from roseau.load_flow.typing import Id, JsonDict, Self
+from roseau.load_flow.typing import Id, JsonDict
 from roseau.load_flow.units import Q_, ureg
 from roseau.load_flow.utils import BranchType
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractBranch(Element):
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/buses.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/buses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from collections.abc import Sequence
 from typing import Any, Optional
 
 import numpy as np
 from shapely import Point
+from typing_extensions import Self
 
 from roseau.load_flow.converters import calculate_voltage_phases, calculate_voltages
 from roseau.load_flow.exceptions import RoseauLoadFlowException, RoseauLoadFlowExceptionCode
 from roseau.load_flow.models.core import Element
-from roseau.load_flow.typing import Id, JsonDict, Self
+from roseau.load_flow.typing import Id, JsonDict
 from roseau.load_flow.units import Q_, ureg
 
 logger = logging.getLogger(__name__)
 
 
 class Bus(Element):
     """An electrical bus."""
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/core.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/core.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/grounds.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/grounds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 from typing import Any, Optional
 
+from typing_extensions import Self
+
 from roseau.load_flow.exceptions import RoseauLoadFlowException, RoseauLoadFlowExceptionCode
 from roseau.load_flow.models.buses import Bus
 from roseau.load_flow.models.core import Element
-from roseau.load_flow.typing import Id, JsonDict, Self
+from roseau.load_flow.typing import Id, JsonDict
 from roseau.load_flow.units import Q_, ureg
 
 logger = logging.getLogger(__name__)
 
 
 class Ground(Element):
     """This element defines the ground.
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/lines/lines.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/lines/lines.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/lines/parameters.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/lines/parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import logging
 import re
 from typing import NoReturn, Optional
 
 import numpy as np
 import numpy.linalg as nplin
+from typing_extensions import Self
 
 from roseau.load_flow.exceptions import RoseauLoadFlowException, RoseauLoadFlowExceptionCode
-from roseau.load_flow.typing import Id, JsonDict, Self
+from roseau.load_flow.typing import Id, JsonDict
 from roseau.load_flow.units import Q_, ureg
 from roseau.load_flow.utils import (
     CX,
     EPSILON_0,
     EPSILON_R,
     MU_0,
     OMEGA,
     PI,
     RHO,
     TAN_D,
     ConductorType,
     Identifiable,
-    IsolationType,
+    InsulationType,
     JsonMixin,
     LineModel,
     LineType,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -298,15 +299,15 @@
     @classmethod
     @ureg.wraps(None, (None, None, None, None, None, "mm**2", "mm**2", "m", "m"), strict=False)
     def from_lv_exact(
         cls,
         type_name: str,
         line_type: LineType,
         conductor_type: ConductorType,
-        isolation_type: IsolationType,
+        insulation_type: InsulationType,
         section: float,
         section_neutral: float,
         height: float,
         external_diameter: float,
     ) -> Self:
         """Create line parameters from LV exact model.
 
@@ -316,15 +317,15 @@
 
             line_type:
                 Overhead or underground.
 
             conductor_type:
                 Type of the conductor
 
-            isolation_type:
+            insulation_type:
                 Type of insulator.
 
             section:
                 Surface of the phases (mm²).
 
             section_neutral:
                 Surface of the neutral (mm²).
@@ -339,28 +340,28 @@
             The created line parameters.
         """
         # TODO: Add documentation on the LV exact model
         z_line, y_shunt, model = cls._lv_exact_to_zy(
             type_name,
             line_type=line_type,
             conductor_type=conductor_type,
-            insulator_type=isolation_type,
+            insulator_type=insulation_type,
             section=section,
             section_neutral=section_neutral,
             height=height,
             external_diameter=external_diameter,
         )
         return cls(type_name, z_line=z_line, y_shunt=y_shunt)
 
     @staticmethod
     def _lv_exact_to_zy(
         type_name: str,
         line_type: LineType,
         conductor_type: ConductorType,
-        insulator_type: IsolationType,
+        insulator_type: InsulationType,
         section: float,
         section_neutral: float,
         height: float,
         external_diameter: float,
     ) -> tuple[np.ndarray, np.ndarray, LineModel]:
         """Create impedance and admittance matrix from a LV exact model.
 
@@ -515,15 +516,15 @@
         name: str,
         section_neutral: Optional[float] = None,
         height: Optional[float] = None,
         external_diameter: Optional[float] = None,
     ) -> Self:
         """Method to get the electrical parameters of a LV line from its canonical name.
         Some hypothesis will be made: the section of the neutral is the same as the other sections, the height and
-        external diameter are pre-defined, and the isolation is PVC.
+        external diameter are pre-defined, and the insulation is PVC.
 
         Args:
             name:
                 The name of the line the parameters must be computed. Eg. "S_AL_150".
 
             section_neutral:
                 Surface of the neutral (mm²). If None it will be the same as the section of the other phases.
@@ -543,30 +544,30 @@
             logger.error(msg)
             raise RoseauLoadFlowException(msg=msg, code=RoseauLoadFlowExceptionCode.BAD_TYPE_NAME_SYNTAX)
 
         # Check the user input and retrieve enumerated types
         line_type, conductor_type, section = name.split("_")
         line_type = LineType.from_string(line_type)
         conductor_type = ConductorType.from_string(conductor_type)
-        isolation_type = IsolationType.PVC
+        insulation_type = InsulationType.PVC
 
         section = float(section)
 
         if section_neutral is None:
             section_neutral = section
         if height is None:
             height = Q_(-1.5, "m") if line_type == LineType.UNDERGROUND else Q_(10.0, "m")
         if external_diameter is None:
             external_diameter = Q_(40, "mm")
 
         return cls.from_lv_exact(
             name,
             line_type=line_type,
             conductor_type=conductor_type,
-            isolation_type=isolation_type,
+            insulation_type=insulation_type,
             section=section,
             section_neutral=section_neutral,
             height=height,
             external_diameter=external_diameter,
         )
 
     @classmethod
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/loads/flexible_parameters.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/loads/flexible_parameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,56 @@
 import logging
 import warnings
 from typing import NoReturn
 
 import numpy as np
+from typing_extensions import Self
 
 from roseau.load_flow.exceptions import RoseauLoadFlowException, RoseauLoadFlowExceptionCode
-from roseau.load_flow.typing import ControlType, JsonDict, ProjectionType, Self
+from roseau.load_flow.typing import ControlType, JsonDict, ProjectionType
 from roseau.load_flow.units import Q_, ureg
 from roseau.load_flow.utils import JsonMixin
 
 logger = logging.getLogger(__name__)
 
 
 class Control(JsonMixin):
-    """A class to store the important values of a control."""
+    """Control class for flexible loads.
 
-    DEFAULT_ALPHA: float = 200.0
+    This class contains the information needed to formulate the control equations. This includes the control type,
+    control limits, and other factors.
+
+    The control for a :class:`PowerLoad` instance can be of four possible types:
+        * ``"constant"``: no control is applied. In this case, a simple :class:`PowerLoad` without `flexible_params`
+          could have been used instead.
+        * ``"p_max_u_production"``: control the maximum production active power of the load (inverter) based on the
+          voltage :math:`P^{\\max}_{\\mathrm{prod}}(U)`. With this control, the following functions are used
+          (depending on the :math:`\\alpha` value).
+
+          .. image:: /_static/Control_PU_Prod.svg
+              :width: 600
+              :align: center
+
+        * ``"p_max_u_consumption"``: control the maximum consumption active power of the load based on the voltage
+          :math:`P^{\\max}_{\\mathrm{cons}}(U)`. With this control, the following functions are used
+          (depending on the :math:`\\alpha` value).
+
+          .. image:: /_static/Control_PU_Cons.svg
+              :width: 600
+              :align: center
+
+        * ``"q_u"``: control the reactive power based on the voltage :math:`Q(U)`. With this control, the following
+          functions are used  (depending on the :math:`\\alpha` value).
+
+          .. image:: /_static/Control_QU.svg
+              :width: 600
+              :align: center
+    """
+
+    DEFAULT_ALPHA: float = 1000.0
 
     @ureg.wraps(None, (None, None, "V", "V", "V", "V", None), strict=False)
     def __init__(
         self,
         type: ControlType,
         u_min: float,
         u_down: float,
@@ -309,19 +340,37 @@
     def results_from_dict(self, data: JsonDict) -> NoReturn:
         msg = f"The {type(self).__name__} has no results to import."
         logger.error(msg)
         raise RoseauLoadFlowException(msg=msg, code=RoseauLoadFlowExceptionCode.JSON_NO_RESULTS)
 
 
 class Projection(JsonMixin):
-    """This class defines the projection on the feasible circle for a flexible load."""
+    """This class defines the projection on the feasible circle for a flexible load.
+
+    The three possible projection types are:
+        * ``"euclidean"``: for an Euclidean projection on the feasible space;
+
+        .. image:: /_static/Euclidean_Projection.svg
+            :width: 300
+            :align: center
+
+        * ``"keep_p"``: for maintaining a constant P;
 
-    # TODO: add the projection diagram (the feasible circle) to the docstring
+        .. image:: /_static/Constant_P_Projection.svg
+            :width: 300
+            :align: center
+
+        * ``"keep_q"``: for maintaining a constant Q.
+
+        .. image:: /_static/Constant_Q_Projection.svg
+            :width: 300
+            :align: center
+    """
 
-    DEFAULT_ALPHA: float = 100.0
+    DEFAULT_ALPHA: float = 1000.0
     DEFAULT_EPSILON: float = 0.01
 
     def __init__(self, type: ProjectionType, alpha: float = DEFAULT_ALPHA, epsilon: float = DEFAULT_EPSILON) -> None:
         """Projection constructor.
 
         Args:
             type:
@@ -402,15 +451,51 @@
     def results_from_dict(self, data: JsonDict) -> NoReturn:
         msg = f"The {type(self).__name__} has no results to import."
         logger.error(msg)
         raise RoseauLoadFlowException(msg=msg, code=RoseauLoadFlowExceptionCode.JSON_NO_RESULTS)
 
 
 class FlexibleParameter(JsonMixin):
-    """This class stores the required data to make a flexible parameter."""
+    """Flexible parameters of a flexible load.
+
+    This class encapsulate single-phase flexibility information of a flexible load:
+
+        * The active power :class:`Control` to apply;
+        * The reactive power :class:`Control` to apply;
+        * The :class:`Projection` to use when dealing with voltage violations;
+        * The apparent power of the flexible load (VA). This is the maximum power the load can consume/produce. It is
+            the radius of the feasible circle used by the projection
+
+    For multi-phase loads, you need to use a `FlexibleParameter` instance per phase.
+
+    Depending on the mix of controls and projection used through this class, the feasible domains in the :math:`(P, Q)`
+    space changes. Here is an illustration with a theoretical power depicting a production (negative
+    :math:`P^{\\mathrm{theo.}}`).
+
+    .. list-table::
+        :class: borderless
+        :header-rows: 1
+        :widths: 20 20 20 20 20
+
+        * -
+          - :math:`Q^{\\mathrm{const.}}`
+          - :math:`Q(U)` with an Euclidean projection
+          - :math:`Q(U)` with a constant P projection
+          - :math:`Q(U)` with a constant Q projection
+        * - :math:`P^{\\mathrm{const.}}`
+          - .. image:: /_static/Domain_Pconst_Qconst.svg
+          - .. image:: /_static/Domain_Pconst_QU_Eucl.svg
+          - .. image:: /_static/Domain_Pconst_QU_P.svg
+          - .. image:: /_static/Domain_Pconst_QU_Q.svg
+        * - :math:`P^{\\max}(U)`
+          - .. image:: /_static/Domain_PmaxU_Qconst.svg
+          - .. image:: /_static/Domain_PmaxU_QU.svg
+          - .. image:: /_static/Domain_PmaxU_QU.svg
+          - .. image:: /_static/Domain_PmaxU_QU.svg
+    """
 
     control_class: type[Control] = Control
     projection_class: type[Projection] = Projection
 
     @ureg.wraps(None, (None, None, None, None, "VA"), strict=False)
     def __init__(self, control_p: Control, control_q: Control, projection: Projection, s_max: float) -> None:
         """FlexibleParameter constructor.
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/loads/loads.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/loads/loads.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,45 @@
 from roseau.load_flow.typing import Id, JsonDict
 from roseau.load_flow.units import Q_, ureg
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractLoad(Element, ABC):
-    """An abstract class of an electric load."""
+    """An abstract class of an electric load.
+
+    The subclasses of this class can be used to depict:
+        * star-connected loads using a `phases` constructor argument containing a `"n"`
+
+        .. tab:: European Standards
+
+            .. image:: /_static/European_Star_Load.svg
+              :width: 300px
+              :align: center
+
+        .. tab:: American Standards
+
+            .. image:: /_static/American_Star_Load.svg
+              :width: 300px
+              :align: center
+
+        * delta-connected loads using a `phases` constructor argument which doesn't contain `"n"`
+
+        .. tab:: European Standards
+
+            .. image:: /_static/European_Delta_Load.svg
+              :width: 300px
+              :align: center
+
+        .. tab:: American Standards
+
+            .. image:: /_static/American_Delta_Load.svg
+              :width: 300px
+              :align: center
+    """
 
     _power_load_class: type["PowerLoad"]
     _current_load_class: type["CurrentLoad"]
     _impedance_load_class: type["ImpedanceLoad"]
     _flexible_parameter_class = FlexibleParameter
 
     _type: Literal["power", "current", "impedance"]
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/potential_refs.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/potential_refs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 from typing import Any, Optional, Union
 
+from typing_extensions import Self
+
 from roseau.load_flow.exceptions import RoseauLoadFlowException, RoseauLoadFlowExceptionCode
 from roseau.load_flow.models.buses import Bus
 from roseau.load_flow.models.core import Element
 from roseau.load_flow.models.grounds import Ground
-from roseau.load_flow.typing import Id, JsonDict, Self
+from roseau.load_flow.typing import Id, JsonDict
 from roseau.load_flow.units import Q_, ureg
 
 logger = logging.getLogger(__name__)
 
 
 class PotentialRef(Element):
     """A potential reference.
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/sources.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from collections.abc import Sequence
 from typing import Any, Optional
 
 import numpy as np
+from typing_extensions import Self
 
 from roseau.load_flow.converters import calculate_voltage_phases
 from roseau.load_flow.exceptions import RoseauLoadFlowException, RoseauLoadFlowExceptionCode
 from roseau.load_flow.models.buses import Bus
 from roseau.load_flow.models.core import Element
-from roseau.load_flow.typing import Id, JsonDict, Self
+from roseau.load_flow.typing import Id, JsonDict
 from roseau.load_flow.units import Q_, ureg
 
 logger = logging.getLogger(__name__)
 
 
 class VoltageSource(Element):
     r"""A voltage source.
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/transformers/parameters.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/transformers/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import NoReturn
 
 import numpy as np
+from typing_extensions import Self
 
 from roseau.load_flow.exceptions import RoseauLoadFlowException, RoseauLoadFlowExceptionCode
-from roseau.load_flow.typing import Id, JsonDict, Self
+from roseau.load_flow.typing import Id, JsonDict
 from roseau.load_flow.units import Q_, ureg
 from roseau.load_flow.utils import Identifiable, JsonMixin, TransformerType
 
 logger = logging.getLogger(__name__)
 
 
 class TransformerParameters(Identifiable, JsonMixin):
@@ -86,14 +87,26 @@
         if vsc > 1.0 or vsc < 0.0:
             msg = (
                 f"Transformer type {id!r} has the 'voltages on LV side during short circuit test' "
                 f"vsc={vsc}. It is a percentage that should be between 0 and 1."
             )
             logger.error(msg)
             raise RoseauLoadFlowException(msg=msg, code=RoseauLoadFlowExceptionCode.BAD_TRANSFORMER_PARAMETERS)
+        if psc / sn > vsc:
+            msg = (
+                f"Transformer type {id!r} has parameters that can't be modeled. The following inequality should be "
+                f"respected: psc/sn <= vsc"
+            )
+            logger.error(msg)
+            raise RoseauLoadFlowException(msg=msg, code=RoseauLoadFlowExceptionCode.BAD_TRANSFORMER_PARAMETERS)
+        if i0 * sn < p0:
+            logger.warning(
+                f"Transformer type {id!r} doesn't respect the inequality: i0 * sn > p0. The magnetizing admittance "
+                f"imaginary part will be null."
+            )
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, TransformerParameters):
             return NotImplemented
         else:
             return (
                 self.id == other.id
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/models/transformers/transformers.py` & `roseau_load_flow-0.4.0/roseau/load_flow/models/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/network.py` & `roseau_load_flow-0.4.0/roseau/load_flow/network.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import geopandas as gpd
 import pandas as pd
 import requests
 from pyproj import CRS
 from requests import Response
 from requests.auth import HTTPBasicAuth
+from typing_extensions import Self
 
 from roseau.load_flow.exceptions import RoseauLoadFlowException, RoseauLoadFlowExceptionCode
 from roseau.load_flow.io import network_from_dgs, network_from_dict, network_to_dict
 from roseau.load_flow.models import (
     AbstractBranch,
     AbstractLoad,
     Bus,
@@ -26,15 +27,16 @@
     Line,
     PotentialRef,
     PowerLoad,
     Switch,
     Transformer,
     VoltageSource,
 )
-from roseau.load_flow.typing import Id, JsonDict, Self, StrPath
+from roseau.load_flow.solvers import check_solver_params
+from roseau.load_flow.typing import Id, JsonDict, Solver, StrPath
 from roseau.load_flow.utils import JsonMixin
 
 logger = logging.getLogger(__name__)
 
 # Phases dtype for all data frames
 _PHASE_DTYPE = pd.CategoricalDtype(categories=["a", "b", "c", "n"], ordered=True)
 # Phases dtype for voltage data frames
@@ -43,15 +45,15 @@
 _T = TypeVar("_T", bound=Element)
 
 
 class ElectricalNetwork(JsonMixin):
     """Electrical network class.
 
     This class represents an electrical network, its elements, and their connections. After
-    creating the network, the load flow algorithm can be run on it using the
+    creating the network, the load flow solver can be run on it using the
     :meth:`solve_load_flow` method.
 
     Args:
         buses:
             The buses of the network. Either a list of buses or a dictionary of buses with
             their IDs as keys. Buses are the nodes of the network. They connect other elements
             such as loads and sources. Buses can be connected together with branches.
@@ -81,27 +83,30 @@
             The potential references of the network. Either a list of potential references or a
             dictionary of potential references with their IDs as keys. As the name suggests, this
             element defines the reference of potentials of the network. A potential reference per
             galvanically isolated section of the network is expected. A potential reference can
             be connected to a bus or to a ground.
 
     Attributes:
-        DEFAULT_PRECISION (float):
-            The default precision needed for the convergence of the load flow algorithm. At each
+        DEFAULT_TOLERANCE (float):
+            The default tolerance needed for the convergence of the load flow solver. At each
             iteration, the solver computes the residuals of the equations of the problem. When the
             maximum of the absolute values of the residuals vector is lower than the provided
-            precision, the solver stops. Default is 1e-6.
+            tolerance, the solver stops. Default is 1e-6.
 
         DEFAULT_MAX_ITERATIONS (int):
             Maximum number of iterations to perform the load flow analysis. The solver stops when
             this number of iterations is reached. Default is 20.
 
         DEFAULT_BASE_URL (str):
             Base URL of the Roseau Load Flow API endpoint.
 
+        DEFAULT_SOLVER (str):
+            The default solver to compute the load flow.
+
         buses (dict[Id, Bus]):
             Dictionary of buses of the network indexed by their IDs. Also available as a
             :attr:`GeoDataFrame<buses_frame>`.
 
         branches (dict[Id, AbstractBranch]):
             Dictionary of branches of the network indexed by their IDs. Also available as a
             :attr:`GeoDataFrame<branches_frame>`.
@@ -124,28 +129,29 @@
 
         res_info (JsonDict):
             Dictionary containing solver information on the last run of the load flow analysis.
             Empty if the load flow analysis has not been run yet.
             Example::
 
                 {
-                    "resolution_method": "newton",
-                    "precision": 1e-06,
+                    "solver": "newton",
+                    "tolerance": 1e-06,
                     "max_iterations": 20,
                     "warm_start": True,
                     "status": "success",
                     "iterations": 2,
-                    "final_precision": 1.8595619621919468e-07
+                    "residual": 1.8595619621919468e-07
                 }
     """
 
-    DEFAULT_PRECISION: float = 1e-6
+    DEFAULT_TOLERANCE: float = 1e-6
     DEFAULT_MAX_ITERATIONS: int = 20
     DEFAULT_BASE_URL: str = "https://load-flow-api-dev.roseautechnologies.com/"
     DEFAULT_WARM_START: bool = True
+    DEFAULT_SOLVER: Solver = "newton_goldstein"
 
     # Default classes to use
     branch_class = AbstractBranch
     line_class = Line
     transformer_class = Transformer
     switch_class = Switch
     load_class = AbstractLoad
@@ -233,18 +239,18 @@
         branches: list[AbstractBranch] = []
         loads: list[AbstractLoad] = []
         sources: list[VoltageSource] = []
         grounds: list[Ground] = []
         potential_refs: list[PotentialRef] = []
 
         elements: list[Element] = [initial_bus]
-        visited_elements: list[Element] = []
+        visited_elements: set[Element] = set()
         while elements:
             e = elements.pop(-1)
-            visited_elements.append(e)
+            visited_elements.add(e)
             if isinstance(e, Bus):
                 buses.append(e)
             elif isinstance(e, AbstractBranch):
                 branches.append(e)
             elif isinstance(e, AbstractLoad):
                 loads.append(e)
             elif isinstance(e, VoltageSource):
@@ -348,96 +354,116 @@
     #
     # Method to solve a load flow
     #
     def solve_load_flow(
         self,
         auth: Union[tuple[str, str], HTTPBasicAuth],
         base_url: str = DEFAULT_BASE_URL,
-        precision: float = DEFAULT_PRECISION,
         max_iterations: int = DEFAULT_MAX_ITERATIONS,
+        tolerance: float = DEFAULT_TOLERANCE,
         warm_start: bool = DEFAULT_WARM_START,
+        solver: Solver = DEFAULT_SOLVER,
+        solver_params: Optional[JsonDict] = None,
     ) -> int:
         """Solve the load flow for this network (Requires internet access).
 
-        Execute a Newton algorithm for load flow calculation. To get the results of the
-        load flow for the whole network, use the different `res_` properties (e.g.
-        ``print(net.res_buses``). To get the results for a specific element, use the
-        element directly (e.g. ``print(net.buses["bus1"].res_potentials)``
+        To get the results of the load flow for the whole network, use the `res_` properties on the
+        network (e.g. ``print(net.res_buses``). To get the results for a specific element, use the
+        `res_` properties on the element (e.g. ``print(net.buses["bus1"].res_potentials)``.
 
         Args:
             auth:
                 The login and password for the roseau load flow api.
 
             base_url:
                 The base url to request the load flow solver.
 
-            precision:
-                Precision needed for the convergence.
-
             max_iterations:
                 The maximum number of allowed iterations.
 
+            tolerance:
+                Tolerance needed for the convergence.
+
             warm_start:
-                Should we use the values of potentials of the last successful load flow result (if any)?
+                If true, initialize the solver with the potentials of the last successful load flow
+                result (if any).
+
+            solver:
+                The name of the solver to use for the load flow. The options are:
+                    - ``'newton'``: the classical Newton-Raphson solver.
+                    - ``'newton_goldstein'``: the Newton-Raphson solver with the Goldstein and
+                      Price linear search.
+
+            solver_params:
+                A dictionary of parameters used by the solver. Available parameters depend on the
+                solver chosen. For more information, see the :ref:`solvers` page.
 
         Returns:
             The number of iterations taken.
         """
         from roseau.load_flow import __version__
 
+        solver_params = check_solver_params(solver=solver, params=solver_params)
         if not self._valid:
             warm_start = False  # Otherwise, we may get an error when calling self.results_to_dict()
             self._check_validity(constructed=True)
             self._create_network()
 
         # Get the data
-        data = {"network": self.to_dict()}
+        data = {
+            "network": self.to_dict(),
+            "solver": {
+                "name": solver,
+                "params": solver_params,
+                "max_iterations": max_iterations,
+                "tolerance": tolerance,
+                "warm_start": warm_start,
+            },
+        }
         if warm_start and self.res_info.get("status", "failure") == "success":
-            # Ignore warnings because results may not be valid (a load power has been changed, etc.)
+            # Ignore warnings because results may be invalid (a load power has been changed, etc.)
             data["results"] = self._results_to_dict(False)
 
         # Request the server
-        params = {"max_iterations": max_iterations, "precision": precision, "warm_start": warm_start}
         response = requests.post(
             url=urljoin(base_url, "solve/"),
-            params=params,
             json=data,
             auth=auth,
             headers={"accept": "application/json", "rlf-version": __version__},
         )
 
         # Read the response
         # Check the response headers
         remote_rlf_version = response.headers.get("rlf-new-version")
         if remote_rlf_version is not None:
             warnings.warn(
                 message=f"A new version ({remote_rlf_version}) of the library roseau-load-flow is available. Please "
-                f"visit https://github.com/RoseauTechnologies/Roseau_Load_Flow for more information.",
+                f"visit https://roseautechnologies.github.io/Roseau_Load_Flow/Installation.html for more information.",
                 category=UserWarning,
                 stacklevel=2,
             )
 
         # HTTP 4xx,5xx
         if not response.ok:
             self._parse_error(response=response)
 
         # HTTP 200
         results: JsonDict = response.json()
         self.res_info = results["info"]
         if self.res_info["status"] != "success":
             msg = (
                 f"The load flow did not converge after {self.res_info['iterations']} iterations. The norm of "
-                f"the residuals is {self.res_info['final_precision']:.5n}"
+                f"the residuals is {self.res_info['residual']:.5n}"
             )
             logger.error(msg=msg)
             raise RoseauLoadFlowException(msg=msg, code=RoseauLoadFlowExceptionCode.NO_LOAD_FLOW_CONVERGENCE)
 
         logger.info(
-            f"The load flow converged after {self.res_info['iterations']} iterations (final error="
-            f"{self.res_info['final_precision']:.5n})."
+            f"The load flow converged after {self.res_info['iterations']} iterations (residual="
+            f"{self.res_info['residual']:.5n})."
         )
 
         # Dispatch the results
         self._results_from_dict(data=results)
 
         return self.res_info["iterations"]
 
@@ -914,21 +940,21 @@
         to the network field of elements.
 
         Args:
             constructed:
                 True if the network is already constructed, and we have added an element, False
                 otherwise.
         """
-        elements: list[Element] = []
-        elements.extend(self.buses.values())
-        elements.extend(self.branches.values())
-        elements.extend(self.loads.values())
-        elements.extend(self.sources.values())
-        elements.extend(self.grounds.values())
-        elements.extend(self.potential_refs.values())
+        elements: set[Element] = set()
+        elements.update(self.buses.values())
+        elements.update(self.branches.values())
+        elements.update(self.loads.values())
+        elements.update(self.sources.values())
+        elements.update(self.grounds.values())
+        elements.update(self.potential_refs.values())
 
         found_source = False
         for element in elements:
             # Check connected elements and check network assignment
             for adj_element in element._connected_elements:
                 if adj_element not in elements:
                     msg = (
@@ -961,28 +987,28 @@
                 element._network = self
             elif element.network != self:
                 element._raise_several_network()
 
     @staticmethod
     def _check_ref(elements: list[Element]) -> None:
         """Check the number of potential references to avoid having a singular jacobian matrix."""
-        visited_elements: list[Element] = []
+        visited_elements: set[Element] = set()
         for initial_element in elements:
             if initial_element in visited_elements or isinstance(initial_element, Transformer):
                 continue
-            visited_elements.append(initial_element)
+            visited_elements.add(initial_element)
             connected_component: list[Element] = []
             to_visit = [initial_element]
             while to_visit:
                 element = to_visit.pop(-1)
                 connected_component.append(element)
                 for connected_element in element._connected_elements:
                     if connected_element not in visited_elements and not isinstance(connected_element, Transformer):
                         to_visit.append(connected_element)
-                        visited_elements.append(connected_element)
+                        visited_elements.add(connected_element)
 
             potential_ref = 0
             for element in connected_component:
                 if isinstance(element, PotentialRef):
                     potential_ref += 1
 
             if potential_ref == 0:
@@ -1101,7 +1127,275 @@
             buses=buses,
             branches=branches,
             loads=loads,
             sources=sources,
             grounds=grounds,
             potential_refs=potential_refs,
         )
+
+    #
+    # Plot
+    #
+    #
+    # def plot(
+    #     self,
+    #     ax: Optional["Axes"] = None,
+    #     crs: Optional[CRS_LIKE_TYPE] = None,
+    #     zoom: Union[str, int] = DEFAULT_ZOOM,
+    #     source: Optional[Union[TileProvider, str]] = None,
+    #     min_size: Optional[float] = DEFAULT_MIN_SIZE,
+    #     margin: Optional[float] = DEFAULT_MARGIN,
+    #     loads_plot_kwargs: Optional[dict[str, Any]] = None,
+    #     slacks_plot_kwargs: Optional[dict[str, Any]] = None,
+    #     junctions_plot_kwargs: Optional[dict[str, Any]] = None,
+    #     branches_plot_kwargs: Optional[dict[str, Any]] = None,
+    # ) -> tuple["Axes", gpd.GeoDataFrame, gpd.GeoDataFrame]:
+    #     """A basic plot function. It plots the network described by the two `geopandas.GeoDataFrame` `buses` and
+    #     `branches`. It also adds a base map which can come from Maptiler or OSM.
+    #
+    #     Args:
+    #         ax:
+    #             The axes on which plot the network.
+    #
+    #         crs:
+    #             The CRS to use for the projection of data. By default pseudo mercator (EPSG:3857).
+    #
+    #         zoom:
+    #             The zoom to use for the background tiles. By default, 'auto' so let contextily decides.
+    #
+    #         source:
+    #             A tile source. One taken from `sirao_core.io.providers` or an URL. If None or not provided, use
+    #             `NetworkPlotExporter.DEFAULT_SOURCE`.
+    #
+    #         min_size:
+    #             The minimum size (in metres) allowed for the plot. This is to ensure a pertinent zoom level on the map.
+    #             Pass None to define no minimum size (this is equivalent to 0.0). Default to 100.0.
+    #
+    #         margin:
+    #             The margin to use for each side of the plot. It is a percentage of the network's size. Pass None to
+    #             define no margin (this is equivalent to 0.0). Default to 0.05.
+    #
+    #         loads_plot_kwargs:
+    #             The keyword arguments to give to the `geopandas.GeoDataFrame.plot` function (except the `ax`
+    #             argument) to plot the loads buses.
+    #
+    #         slacks_plot_kwargs:
+    #             The keyword arguments to give to the `geopandas.GeoDataFrame.plot` function (except the `ax`
+    #             argument) to plot the slack buses
+    #
+    #         junctions_plot_kwargs:
+    #             The keyword arguments to give to the `geopandas.GeoDataFrame.plot` function (except the `ax`
+    #             argument) to plot the junction buses. To ignore this plot, just pass `{'marker':''}`.
+    #
+    #         branches_plot_kwargs:
+    #             The keyword arguments to give to the `geopandas.GeoDataFrame.plot` function (except the `ax`
+    #             argument) to plot the branches.
+    #
+    #     Returns:
+    #         The axe on which the network has been plotted and the data frames of buses and branches converted to the
+    #         new CRS.
+    #     """
+    #     ax, buses, branches, crs = self.plot_without_basemap(
+    #         ax=ax,
+    #         crs=crs,
+    #         loads_plot_kwargs=loads_plot_kwargs,
+    #         slacks_plot_kwargs=slacks_plot_kwargs,
+    #         junctions_plot_kwargs=junctions_plot_kwargs,
+    #         branches_plot_kwargs=branches_plot_kwargs,
+    #     )
+    #
+    #     # Resize axes according to the provided minimum size and margin
+    #     self.resize_axis(ax=ax, min_size=min_size, margin=margin)
+    #
+    #     # Add the base map
+    #     self.add_basemap(ax=ax, crs=crs, zoom=zoom, source=source)
+    #
+    #     return ax, buses, branches
+    #
+    #
+    # def plot_without_basemap(
+    #     self,
+    #     ax: Optional["Axes"] = None,
+    #     crs: Optional[CRS_LIKE_TYPE] = None,
+    #     loads_plot_kwargs: Optional[dict[str, Any]] = None,
+    #     slacks_plot_kwargs: Optional[dict[str, Any]] = None,
+    #     junctions_plot_kwargs: Optional[dict[str, Any]] = None,
+    #     branches_plot_kwargs: Optional[dict[str, Any]] = None,
+    # ) -> tuple["Axes", gpd.GeoDataFrame, gpd.GeoDataFrame, CRS_LIKE_TYPE]:
+    #     """A basic plot function. It plots the network described by the two `geopandas.GeoDataFrame` `buses` and
+    #     `branches` without adding basemap.
+    #
+    #     Args:
+    #         ax:
+    #             The axes on which plot the network.
+    #
+    #         crs:
+    #             The CRS to use for the projection of data. By default pseudo mercator (EPSG:3857).
+    #
+    #         loads_plot_kwargs:
+    #             The keyword arguments to give to the `geopandas.GeoDataFrame.plot` function (except the `ax`
+    #             argument) to plot the loads buses.
+    #
+    #         slacks_plot_kwargs:
+    #             The keyword arguments to give to the `geopandas.GeoDataFrame.plot` function (except the `ax`
+    #             argument) to plot the slack buses
+    #
+    #         junctions_plot_kwargs:
+    #             The keyword arguments to give to the `geopandas.GeoDataFrame.plot` function (except the `ax`
+    #             argument) to plot the junction buses. To ignore this plot, just pass `{'marker':''}`.
+    #
+    #         branches_plot_kwargs:
+    #             The keyword arguments to give to the `geopandas.GeoDataFrame.plot` function (except the `ax`
+    #             argument) to plot the branches.
+    #
+    #     Returns:
+    #         The axe on which the network has been plotted, the data frames of buses and branches converted to the new
+    #         CRS and the new CRS used.
+    #     """
+    #     from matplotlib import pyplot as plt
+    #
+    #     # Default arguments
+    #     loads_plot_kwargs = loads_plot_kwargs if loads_plot_kwargs is not None else self.DEFAULT_LOADS_PLOT_KWARGS
+    #     branches_plot_kwargs = (
+    #         branches_plot_kwargs if branches_plot_kwargs is not None else self.DEFAULT_BRANCHES_PLOT_KWARGS
+    #     )
+    #     slacks_plot_kwargs = slacks_plot_kwargs if slacks_plot_kwargs is not None else self.DEFAULT_SLACKS_PLOT_KWARGS
+    #     junctions_plot_kwargs = (
+    #         junctions_plot_kwargs if junctions_plot_kwargs is not None else self.DEFAULT_JUNCTIONS_PLOT_KWARGS
+    #     )
+    #     if crs is None:
+    #         crs = CRS.from_epsg(3857)
+    #
+    #     # Get the data and convert them to the provided CRS
+    #     buses = self.buses_frame.to_crs(crs=crs)
+    #     branches = self.branches_frame.to_crs(crs=crs)
+    #
+    #     # Get the axes
+    #     if ax is None:
+    #         ax: "Axes" = plt.gca()
+    #     ax.axis("off")
+    #
+    #     # Plot buses
+    #     # When "marker" is "" and in some other cases, matplotlib raises a ValueError. In these cases,
+    #     # it often means that we do not want to plot the layer, so we just continue
+    #     for bus_type, buses_gdf in buses.groupby(by="bus_type", observed=True):
+    #         if bus_type == "slack":
+    #             if slacks_plot_kwargs["marker"] != "":
+    #                 self._plot_with_stroke(df=buses_gdf, ax=ax, stroke_color="white", **slacks_plot_kwargs)
+    #         elif bus_type == "junction":
+    #             if junctions_plot_kwargs["marker"] != "":
+    #                 self._plot_with_stroke(df=buses_gdf, ax=ax, stroke_color="white", **junctions_plot_kwargs)
+    #         elif bus_type == "load":
+    #             if loads_plot_kwargs["marker"] != "":
+    #                 self._plot_with_stroke(df=buses_gdf, ax=ax, stroke_color="white", **loads_plot_kwargs)
+    #         else:
+    #             logger.warning(
+    #                 f"The bus type {bus_type!r} is unknown so we ignore the {buses_gdf.shape[0]} buses of this type "
+    #                 f"for the plot."
+    #             )
+    #
+    #     if len(branches.index) > 0:
+    #         # Plot branches
+    #         self._plot_with_stroke(df=branches, ax=ax, stroke_color="white", **branches_plot_kwargs)
+    #
+    #     return ax, buses, branches, crs
+    #
+    #
+    # @staticmethod
+    # def _plot_with_stroke(
+    #     df: Union[pd.DataFrame, gpd.GeoDataFrame],
+    #     ax: "Axes",
+    #     stroke_color: Optional[str] = None,
+    #     stroke_zorder: float = 1,
+    #     stroke_width: float = 3,
+    #     **kwargs,
+    # ):
+    #     """Plot a data frame or geo data frame with a stroke.
+    #
+    #     Args:
+    #         df:
+    #             The data frame or geo data frame to plot.
+    #
+    #         ax:
+    #             The axes on which to plot the data.
+    #
+    #         stroke_color:
+    #             The color to use for the stroke. If None or not provided, no stroke will be plotted.
+    #
+    #         stroke_zorder:
+    #             The zorder to pass to matplotlib for the stroke. By default, use 1.
+    #
+    #         stroke_width:
+    #             The line width to use for the stroke. It should be greater than the line width uses for the normal plot.
+    #             By default, use 3.
+    #
+    #     Keyword Args:
+    #         The keyword arguments to pass to the data frame plot method.
+    #     """
+    #     df.plot(ax=ax, **kwargs)
+    #
+    #     kwargs.pop("zorder", None)
+    #     kwargs.pop("linewidth", None)
+    #     kwargs.pop("color", None)
+    #     kwargs.pop("column", None)
+    #     kwargs.pop("cmap", None)
+    #     kwargs.pop("label", None)
+    #     if stroke_color is not None:
+    #         df.plot(ax=ax, zorder=stroke_zorder, linewidth=stroke_width, color=stroke_color, **kwargs)
+    #
+    # @staticmethod
+    # def resize_axe(ax: "Axes", figsize:tuple[float, float]):
+    #     xmin, xmax, ymin, ymax = ax.axis()
+    #     xlen, ylen = (xmax - xmin, ymax - ymin)
+    #     xfig, yfig = figsize
+    #     xratio = xlen / xfig
+    #     yratio = ylen / yfig
+    #
+    #     if xratio > yratio:
+    #         expand = (xratio * yfig - ylen) / 2.0
+    #         ax.set_ylim(ymin=ymin - expand, ymax=ymax + expand)
+    #     elif xratio < yratio:
+    #         expand = (yratio * xfig - xlen) / 2.0
+    #         ax.set_xlim(xmin=xmin - expand, xmax=xmax + expand)
+    #
+    # def add_basemap(
+    #     self,
+    #     ax: "Axes",
+    #     crs: CRS_LIKE_TYPE,
+    #     zoom: Union[str, int] = DEFAULT_ZOOM,
+    #     source: Optional[Union[TileProvider, str]] = None,
+    # ):
+    #     """Add a basemap to the provided axes.
+    #
+    #     Args:
+    #         ax:
+    #             The axes on which to add the basemap.
+    #
+    #         crs:
+    #             The CRS to use for the projection of data.
+    #
+    #         zoom:
+    #             The zoom to use for the background tiles. By default, use "auto".
+    #
+    #         source:
+    #             A tile source. One taken from `sirao_core.io.providers` or an URL. If None or not provided, use
+    #             `NetworkPlotExporter.DEFAULT_SOURCE`.
+    #     """
+    #     import contextily as ctx
+    #
+    #     ax.axis("off")
+    #     if source is None:
+    #         source = self.DEFAULT_SOURCE
+    #     try:
+    #         logger.info(
+    #             f"Start adding basemap from {source['url'] if 'url' in source else source} to the plot."
+    #         )
+    #         ctx.add_basemap(ax=ax, zoom=zoom, source=source, crs=str(crs), reset_extent=True)
+    #         logger.info("Basemap was successfully added to the plot.")
+    #     except (HTTPError, UnidentifiedImageError) as e:
+    #         logger.error(
+    #             f"The following error has been raised by contextily when trying to add basemap to the plot:\n"
+    #             f"{e.__module__}.{e.__class__.__name__}: {e}"
+    #         )
+    #         if source != self.DEFAULT_SOURCE:
+    #             logger.info(f"Adding default basemap from {self.DEFAULT_SOURCE['url']} to the plot.")
+    #             ctx.add_basemap(ax=ax, zoom=zoom, source=self.DEFAULT_SOURCE, crs=str(crs), reset_extent=True)
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/typing.py` & `roseau_load_flow-0.4.0/roseau/load_flow/typing.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,36 +17,31 @@
 
     Available types of control for flexible loads.
 
 .. class:: ProjectionType
 
     Available types of projections for flexible loads control.
 
-.. class:: Self
+.. class:: Solver
 
-    The type of the class itself.
+    Available solvers for the load flow computation.
 """
 import os
 import sys
-from typing import TYPE_CHECKING, Any, Literal, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Literal, Union
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias as TypeAlias
 elif TYPE_CHECKING:
     from typing_extensions import TypeAlias as TypeAlias
 else:
     TypeAlias = Any
 
 Id: TypeAlias = Union[int, str]
 JsonDict: TypeAlias = dict[str, Any]
 StrPath: TypeAlias = Union[str, os.PathLike[str]]
 ControlType: TypeAlias = Literal["constant", "p_max_u_production", "p_max_u_consumption", "q_u"]
 ProjectionType: TypeAlias = Literal["euclidean", "keep_p", "keep_q"]
+Solver: TypeAlias = Literal["newton", "newton_goldstein"]
 
-if sys.version_info >= (3, 11):
-    from typing import Self as Self
-elif TYPE_CHECKING:
-    from typing_extensions import Self as Self
-else:
-    Self = TypeVar("Self")
 
-__all__ = ["Id", "JsonDict", "StrPath", "ControlType", "ProjectionType"]
+__all__ = ["Id", "JsonDict", "StrPath", "ControlType", "ProjectionType", "Solver"]
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/units.py` & `roseau_load_flow-0.4.0/roseau/load_flow/units.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/utils/_versions.py` & `roseau_load_flow-0.4.0/roseau/load_flow/utils/_versions.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/utils/constants.py` & `roseau_load_flow-0.4.0/roseau/load_flow/utils/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 from roseau.load_flow.units import Q_
-from roseau.load_flow.utils.types import ConductorType, IsolationType, LineType
+from roseau.load_flow.utils.types import ConductorType, InsulationType, LineType
 
 PI = np.pi
 """The famous constant :math:`\\pi`."""
 
 MU_0 = Q_(4 * PI * 1e-7, "H/m")
 """magnetic permeability of the vacuum (H/m)."""
 
@@ -49,23 +49,23 @@
     ConductorType.AM: Q_(12.9, "mm"),
     ConductorType.AA: np.nan,  # TODO
     ConductorType.LA: np.nan,  # TODO
 }
 """Skin effect of certain conductor materials (mm)."""
 
 TAN_D = {
-    IsolationType.PVC: Q_(600e-4),
-    IsolationType.HDPE: Q_(6e-4),
-    IsolationType.LDPE: Q_(6e-4),
-    IsolationType.PEX: Q_(30e-4),
-    IsolationType.EPR: Q_(125e-4),
+    InsulationType.PVC: Q_(600e-4),
+    InsulationType.HDPE: Q_(6e-4),
+    InsulationType.LDPE: Q_(6e-4),
+    InsulationType.PEX: Q_(30e-4),
+    InsulationType.EPR: Q_(125e-4),
 }
-"""Loss angles of certain isolation materials."""
+"""Loss angles of certain insulation materials."""
 
 EPSILON_R = {
-    IsolationType.PVC: Q_(6.5),
-    IsolationType.HDPE: Q_(2.3),
-    IsolationType.LDPE: Q_(2.2),
-    IsolationType.PEX: Q_(2.5),
-    IsolationType.EPR: Q_(3.1),
+    InsulationType.PVC: Q_(6.5),
+    InsulationType.HDPE: Q_(2.3),
+    InsulationType.LDPE: Q_(2.2),
+    InsulationType.PEX: Q_(2.5),
+    InsulationType.EPR: Q_(3.1),
 }
-"""Relative permittivity of certain isolation materials."""
+"""Relative permittivity of certain insulation materials."""
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/utils/mixins.py` & `roseau_load_flow-0.4.0/roseau/load_flow/utils/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import json
 import logging
 import re
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
 from typing import Any
 
+from typing_extensions import Self
+
 from roseau.load_flow.exceptions import RoseauLoadFlowException, RoseauLoadFlowExceptionCode
-from roseau.load_flow.typing import Id, JsonDict, Self, StrPath
+from roseau.load_flow.typing import Id, JsonDict, StrPath
 
 logger = logging.getLogger(__name__)
 
 
 class Identifiable(metaclass=ABCMeta):
     """An identifiable object."""
```

### Comparing `roseau_load_flow-0.3.0/roseau/load_flow/utils/types.py` & `roseau_load_flow-0.4.0/roseau/load_flow/utils/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from enum import Enum, auto, unique
 from typing import Optional
 
 import regex
+from typing_extensions import Self
 
 from roseau.load_flow.exceptions import RoseauLoadFlowException, RoseauLoadFlowExceptionCode
-from roseau.load_flow.typing import Self
 
 # The local logger
 logger = logging.getLogger(__name__)
 
 
 @unique
 class LineType(Enum):
@@ -147,65 +147,65 @@
         Returns:
             The code of the enumerated value.
         """
         return self.name.upper()
 
 
 @unique
-class IsolationType(Enum):
-    """The type of the isolation for a wire."""
+class InsulationType(Enum):
+    """The type of the insulation for a wire."""
 
     UNKNOWN = auto()
-    """The isolation of the conductor is made with unknown material."""
+    """The insulation of the conductor is made with unknown material."""
     HDPE = auto()
-    """The isolation of the conductor is made with High-Density PolyEthylene."""
+    """The insulation of the conductor is made with High-Density PolyEthylene."""
     LDPE = auto()
-    """The isolation of the conductor is made with Low-Density PolyEthylene."""
+    """The insulation of the conductor is made with Low-Density PolyEthylene."""
     PEX = auto()
-    """The isolation of the conductor is made with Cross-linked polyethylene."""
+    """The insulation of the conductor is made with Cross-linked polyethylene."""
     EPR = auto()
-    """The isolation of the conductor is made with Ethylene-Propylene Rubber."""
+    """The insulation of the conductor is made with Ethylene-Propylene Rubber."""
     PVC = auto()
-    """The isolation of the conductor is made with PolyVinyl Chloride."""
+    """The insulation of the conductor is made with PolyVinyl Chloride."""
 
     def __str__(self) -> str:
-        """Print a `IsolationType`
+        """Print a `InsulationType`
 
         Returns:
-            A printable string of the isolation type.
+            A printable string of the insulation type.
         """
         return self.name.upper()
 
     @classmethod
     def from_string(cls, string: str) -> Self:
-        """Convert a string into a IsolationType
+        """Convert a string into a InsulationType
 
         Args:
             string:
                 The string to convert
 
         Returns:
-            The corresponding IsolationType.
+            The corresponding InsulationType.
         """
         if string.lower() in ("", "unknown", "nan"):
             return cls.UNKNOWN
         elif string == "HDPE":
             return cls.HDPE
         elif string == "LDPE":
             return cls.LDPE
         elif string == "PEX":
             return cls.PEX
         elif string == "EPR":
             return cls.EPR
         elif string == "PVC":
             return cls.PVC
         else:
-            msg = f"The string {string!r} cannot be converted into a IsolationType."
+            msg = f"The string {string!r} cannot be converted into a InsulationType."
             logger.error(msg)
-            raise RoseauLoadFlowException(msg=msg, code=RoseauLoadFlowExceptionCode.BAD_ISOLATION_TYPE)
+            raise RoseauLoadFlowException(msg=msg, code=RoseauLoadFlowExceptionCode.BAD_INSULATION_TYPE)
 
 
 @unique
 class LineModel(Enum):
     """An enumerated class for the different line models."""
 
     UNKNOWN = auto()
```

### Comparing `roseau_load_flow-0.3.0/PKG-INFO` & `roseau_load_flow-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,71 @@
 Metadata-Version: 2.1
 Name: roseau-load-flow
-Version: 0.3.0
-Summary: Three-phase load flow solver
+Version: 0.4.0
+Summary: Highly capable three-phase load flow solver
 Home-page: https://github.com/RoseauTechnologies/Roseau_Load_Flow/
 License: Proprietary
 Author: Ali Hamdan
 Author-email: ali.hamdan@roseautechnologies.com
 Maintainer: Ali Hamdan
 Maintainer-email: ali.hamdan@roseautechnologies.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: geopandas (>=0.10.2)
 Requires-Dist: numpy (>=1.21.5)
 Requires-Dist: pandas (>=1.4.0)
 Requires-Dist: pint (>=0.19.2)
 Requires-Dist: regex (>=2022.1.18)
 Requires-Dist: requests (>=2.28.1)
 Requires-Dist: shapely (>=2.0.0)
+Requires-Dist: typing-extensions (>=4.6.2)
 Project-URL: Repository, https://github.com/RoseauTechnologies/Roseau_Load_Flow/
 Description-Content-Type: text/markdown
 
 # Roseau Load Flow #
 
 ![CI](https://github.com/RoseauTechnologies/Roseau_Load_Flow/workflows/CI/badge.svg)
 [![Documentation](https://github.com/RoseauTechnologies/Roseau_Load_Flow/actions/workflows/doc.yml/badge.svg)](https://github.com/RoseauTechnologies/Roseau_Load_Flow/actions/workflows/doc.yml)
 [![pre-commit](https://github.com/RoseauTechnologies/Roseau_Load_Flow/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/RoseauTechnologies/Roseau_Load_Flow/actions/workflows/pre-commit.yml)
 
-*Roseau Load Flow* is a highly capable three-phase load flow solver. This project is compatible
-with Python 3.9 and above.
+*Roseau Load Flow* is a highly capable three-phase load flow solver. This project is compatible with Python 3.9 and
+above.
 
 Please take a look at our documentation to see how to install and use `roseau_load_flow`.
 
 * [Installation](https://roseautechnologies.github.io/Roseau_Load_Flow/installation.html)
 * [Usage](https://roseautechnologies.github.io/Roseau_Load_Flow/notebooks/Getting_Started.html)
 
 # Accessing the solver #
 
-This is the client library for the *Roseau Load Flow* solver. To use the solver, you need to sign
-up for an account. For inquiry, please contact us at contact@roseautechnologies.com.
+This is the client library for the
+[*Roseau Load Flow*](https://www.roseautechnologies.com/en/roseau-load-flow-en/) solver. To use the solver, you
+need to sign up for an account. For inquiry, please contact us at contact@roseautechnologies.com.
+
+If you are a **student or a teacher, free API credentials are provided**. Please contact us at
+contact@roseautechnologies.com.
+
+# Network data #
+
+With this library, there is a sample of 20 low-voltage and 20 medium-voltage feeders included for an easy
+start! Each network is given with its summer and winter load point. At *Roseau Technologies*, we are able to provide
+the major part of the French medium and low voltage networks. For more information, please contact us at
+contact@roseautechnologies.com.
 
 # Bug reports / Feature requests #
 
-If you find a bug or have a feature request, please open an issue on the
+If you find a bug or have a feature request, please open an issue on
 [GitHub](https://github.com/RoseauTechnologies/Roseau_Load_Flow/issues)
 
+# Credits #
+
+This software is developed by [Roseau Technologies](https://www.roseautechnologies.com/en).
+[![Linkedin](https://i.stack.imgur.com/gVE0j.png) LinkedIn](https://www.linkedin.com/company/roseau-technologies/)
+&nbsp;
+[![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/RoseauTechnologies)
+
```

