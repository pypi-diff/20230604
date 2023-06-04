# Comparing `tmp/arango_orm-0.7.1.tar.gz` & `tmp/arango_orm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arango_orm-0.7.1.tar", max compression
+gzip compressed data, was "arango_orm-0.7.2.tar", max compression
```

## Comparing `arango_orm-0.7.1.tar` & `arango_orm-0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35141 2023-06-04 18:17:00.395211 arango_orm-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0    21405 2023-06-04 18:17:00.395211 arango_orm-0.7.1/README.rst
--rw-r--r--   0        0        0      236 2023-06-04 18:17:00.395211 arango_orm-0.7.1/arango_orm/__init__.py
--rw-r--r--   0        0        0    16436 2023-06-04 18:17:00.395211 arango_orm-0.7.1/arango_orm/collections.py
--rw-r--r--   0        0        0     3463 2023-06-04 18:17:00.395211 arango_orm-0.7.1/arango_orm/connection_pool.py
--rw-r--r--   0        0        0    22738 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/database.py
--rw-r--r--   0        0        0      790 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/event/__init__.py
--rw-r--r--   0        0        0      427 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/exceptions.py
--rw-r--r--   0        0        0       33 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/fields.py
--rw-r--r--   0        0        0    12783 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/graph.py
--rw-r--r--   0        0        0     8908 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/query.py
--rw-r--r--   0        0        0     2375 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/references.py
--rw-r--r--   0        0        0      615 2023-06-04 18:17:00.399211 arango_orm-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    23097 1970-01-01 00:00:00.000000 arango_orm-0.7.1/setup.py
--rw-r--r--   0        0        0    22070 1970-01-01 00:00:00.000000 arango_orm-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35141 2023-06-04 18:26:35.527913 arango_orm-0.7.2/LICENSE.txt
+-rw-r--r--   0        0        0    21405 2023-06-04 18:26:35.527913 arango_orm-0.7.2/README.rst
+-rw-r--r--   0        0        0      236 2023-06-04 18:26:35.527913 arango_orm-0.7.2/arango_orm/__init__.py
+-rw-r--r--   0        0        0    16436 2023-06-04 18:26:35.527913 arango_orm-0.7.2/arango_orm/collections.py
+-rw-r--r--   0        0        0     3463 2023-06-04 18:26:35.527913 arango_orm-0.7.2/arango_orm/connection_pool.py
+-rw-r--r--   0        0        0    22738 2023-06-04 18:26:35.527913 arango_orm-0.7.2/arango_orm/database.py
+-rw-r--r--   0        0        0      790 2023-06-04 18:26:35.531913 arango_orm-0.7.2/arango_orm/event/__init__.py
+-rw-r--r--   0        0        0      427 2023-06-04 18:26:35.531913 arango_orm-0.7.2/arango_orm/exceptions.py
+-rw-r--r--   0        0        0       33 2023-06-04 18:26:35.531913 arango_orm-0.7.2/arango_orm/fields.py
+-rw-r--r--   0        0        0    12783 2023-06-04 18:26:35.531913 arango_orm-0.7.2/arango_orm/graph.py
+-rw-r--r--   0        0        0     8908 2023-06-04 18:26:35.531913 arango_orm-0.7.2/arango_orm/query.py
+-rw-r--r--   0        0        0     2375 2023-06-04 18:26:35.531913 arango_orm-0.7.2/arango_orm/references.py
+-rw-r--r--   0        0        0      729 2023-06-04 18:26:35.531913 arango_orm-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    23137 1970-01-01 00:00:00.000000 arango_orm-0.7.2/setup.py
+-rw-r--r--   0        0        0    22190 1970-01-01 00:00:00.000000 arango_orm-0.7.2/PKG-INFO
```

### Comparing `arango_orm-0.7.1/LICENSE.txt` & `arango_orm-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arango_orm-0.7.1/README.rst` & `arango_orm-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `arango_orm-0.7.1/arango_orm/collections.py` & `arango_orm-0.7.2/arango_orm/collections.py`

 * *Files identical despite different names*

### Comparing `arango_orm-0.7.1/arango_orm/connection_pool.py` & `arango_orm-0.7.2/arango_orm/connection_pool.py`

 * *Files identical despite different names*

### Comparing `arango_orm-0.7.1/arango_orm/database.py` & `arango_orm-0.7.2/arango_orm/database.py`

 * *Files identical despite different names*

### Comparing `arango_orm-0.7.1/arango_orm/event/__init__.py` & `arango_orm-0.7.2/arango_orm/event/__init__.py`

 * *Files identical despite different names*

### Comparing `arango_orm-0.7.1/arango_orm/graph.py` & `arango_orm-0.7.2/arango_orm/graph.py`

 * *Files identical despite different names*

### Comparing `arango_orm-0.7.1/arango_orm/query.py` & `arango_orm-0.7.2/arango_orm/query.py`

 * *Files identical despite different names*

### Comparing `arango_orm-0.7.1/arango_orm/references.py` & `arango_orm-0.7.2/arango_orm/references.py`

 * *Files identical despite different names*

### Comparing `arango_orm-0.7.1/setup.py` & `arango_orm-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['marshmallow==3.15.0', 'python-arango==7.1.0']
 
 setup_kwargs = {
     'name': 'arango-orm',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': 'A SQLAlchemy like ORM implementation for arangodb',
     'long_description': 'Python ORM Layer For ArangoDB\n=============================\n\n**arango_orm** is a python ORM layer inspired by SQLAlchemy but aimed to work\nwith the multi-model database ArangoDB. It supports accessing both collections\nand graphs using the ORM. The actual communication with the database is done\nusing **python-arango** (the database driver for accessing arangodb from\npython) and object serialization and de-serialization is handled using\n**marshmallow**.\n\n\nInstallation:\n-------------\n\n::\n\n    pip install arango-orm\n\n\nConnecting to a Database\n-------------------------\n\n.. code-block:: python\n\n    from arango import ArangoClient\n    from arango_orm import Database\n\n    client = ArangoClient(hosts=\'http://localhost:8529\')\n    test_db = client.db(\'test\', username=\'test\', password=\'test\')\n\n    db = Database(test_db)\n\n\nUsing a Connection Pool\n-----------------------\n\nNote: This is deprecated since python arango version 5.0. Since now the base\nlibrary supports the hosts parameter. This will be removed in future versions.\nUsers should instead use the pool in ArangoClient like:\n\n.. code-block:: python\n\n  client = ArangoClient(\n    hosts=[\'http://host1:8529\', \'http://host2:8529\'],\n    host_resolver=\'roundrobin\'\n  )\n\n\nConnection pools allow using multiple connections for accessing the database.\nThough these can be used on a single machine setup, they are more useful to use\nwith arango clusters.\n\nConnection pools support the same methods and properties that the Database class\ndoes. So they can be used interchangeably with Database.\n\n.. code-block:: python\n\n    from arango import ArangoClient\n    from arango_orm import ConnectionPool\n\n    client1 = ArangoClient(protocol=\'http\', host=\'localhost\', port=8529)\n    client2 = ArangoClient(protocol=\'http\', host=\'127.0.0.1\', port=8529)\n\n    db = ConnectionPool([client1, client2], \'test\', \'test\', \'test\')\n\n\nWorking With Collections\n-------------------------\n\nFirst we need to define data models (similar to SQLAlchemy\'s models) to specify what data our collection(s) will contain and how to marshal it\n\n.. code-block:: python\n\n    from arango_orm import Collection\n    from arango_orm.fields import String, Date\n\n    class Student(Collection):\n\n        __collection__ = \'students\'\n        _index = [{\'type\': \'hash\', \'fields\': [\'name\'], \'unique\': True}]\n\n        _key = String(required=True)  # registration number\n        name = String(required=True, allow_none=False)\n        dob = Date()\n\n\nCreate Collection in the Database\n_________________________________\n\n.. code-block:: python\n\n    db.create_collection(Student)\n\n\nDrop a Collection\n__________________\n\n.. code-block:: python\n\n    db.drop_collection(Student)\n\nCheck if a collection exists\n____________________________\n\n.. code-block:: python\n\n    db.has_collection(Student)\n    db.has_collection(\'students\')\n\nAdd Records\n___________\n\n.. code-block:: python\n\n    from datetime import date\n    s = Student(name=\'test\', _key=\'12312\', dob=date(year=2016, month=9, day=12))\n    db.add(s)\n    print(s._id)  # students/12312\n\n\nGet Total Records in the Collection\n___________________________________\n\n.. code-block:: python\n\n    db.query(Student).count()\n\n\nGet Record By Key\n_________________\n\n.. code-block:: python\n\n    s = db.query(Student).by_key(\'12312\')\n\n\nUpdate a Record\n________________\n\n.. code-block:: python\n\n    s = db.query(Student).by_key(\'12312\')\n    s.name = \'Anonymous\'\n    db.update(s)\n\nDelete a Record\n________________\n\n.. code-block:: python\n\n    s = db.query(Student).by_key(\'12312\')\n    db.delete(s)\n\nGet All Records in a Collection\n________________________________\n\n.. code-block:: python\n\n    students = db.query(Student).all()\n\nGet First Record Matching the Query\n____________________________________\n\n.. code-block:: python\n\n    first_student = db.query(Student).first()\n\nFilter Records\n______________\n\nUsing bind parameters (recommended)\n\n.. code-block:: python\n\n    records = db.query(Student).filter("name==@name", name=\'Anonymous\').all()\n\nUsing plain condition strings (not safe in case of unsanitized user supplied input)\n\n.. code-block:: python\n\n    records = db.query(Student).filter("name==\'Anonymous\'").all()\n\n\nFilter Using OR\n_______________\n\n.. code-block:: python\n\n    # Get all documents where student name starts with A or B\n    records = db.query(Student).filter(\n                "LIKE(rec.name, \'A%\')", prepend_rec_name=False).filter(\n                "LIKE(rec.name, \'B%\')", prepend_rec_name=False, _or=True).all()\n\n\nFilter, Sort and Limit\n______________________\n\n.. code-block:: python\n\n    # Last 5 students with names starting with A\n    records = db.query(Student).filter(\n                "LIKE(rec.name, \'A%\')", prepend_rec_name=False).sort("name DESC").limit(5).all()\n\n    # Query students with pagination (limit&offset)\n    page_num, per_page = 2, 10\n    page = db.query(Student).sort("name DESC").limit(per_page, start_from=(page_num - 1) * per_page)\n\nFetch Only Some Fields\n______________________\n\n    .. code-block:: python\n\n        c = db.query(Student).limit(2).returns(\'_key\', \'name\').first()\n\nUpdate Multiple Records\n_______________________\n\n.. code-block:: python\n\n    db.query(Student).filter("name==@name", name=\'Anonymous\').update(name=\'Mr. Anonymous\')\n\n\nDelete Multiple Records\n_______________________\n\n.. code-block:: python\n\n    db.query(Student).filter("LIKE(rec.name, \'test%\')", prepend_rec_name=False).delete()\n\n\nDelete All Records\n___________________\n\n.. code-block:: python\n\n    db.query(Student).delete()\n\n\n\nBulk Create Records\n_______________________\n\n.. code-block:: python\n\n    s1 = Student(name=\'test1\', _key=\'12345\', dob=date(year=2016, month=9, day=12))\n    s2 = Student(name=\'test2\', _key=\'22346\', dob=date(year=2015, month=9, day=12)\n    car1 = Car(make="Honda", model="Fiat", year=2010)\n    car2 = Car(make="Honda", model="Skoda", year=2015)\n\n    db.bulk_add(entity_list=[p_ref_10, p_ref_11, car1, car2])\n\n\nBulk Update Records\n_______________________\n\n.. code-block:: python\n\n    p_ref1 = db.query(Person).by_key("12312")\n    p_ref2 = db.query(Person).by_key("12345")\n    p_ref1.name = "Bruce"\n    p_ref2.name = "Eliza"\n    db.bulk_update(entity_list=[p_ref1, p_ref2])\n\n\nQuery Using AQL\n________________\n\n.. code-block:: python\n\n    db.add(Student(name=\'test1\', _key=\'12345\', dob=date(year=2016, month=9, day=12)))\n    db.add(Student(name=\'test2\', _key=\'22346\', dob=date(year=2015, month=9, day=12)))\n\n    students = [Student._load(s) for s in db.aql.execute("FOR st IN students RETURN st")]\n\nReference Fields\n----------------\n\nReference fields allow linking documents from another collection class within a collection instance.\nThese are similar in functionality to SQLAlchemy\'s relationship function.\n\n.. code-block:: python\n\n    from arango import ArangoClient\n    from arango_orm.database import Database\n\n    from arango_orm.fields import String\n    from arango_orm import Collection, Relation, Graph, GraphConnection\n    from arango_orm.references import relationship, graph_relationship\n\n\n    class Person(Collection):\n\n        __collection__ = \'persons\'\n\n        _index = [{\'type\': \'hash\', \'unique\': False, \'fields\': [\'name\']}]\n        _allow_extra_fields = False  # prevent extra properties from saving into DB\n\n        _key = String(required=True)\n        name = String(required=True, allow_none=False)\n\n        cars = relationship(__name__ + ".Car", \'_key\', target_field=\'owner_key\')\n\n        def __str__(self):\n            return "<Person(" + self.name + ")>"\n\n\n    class Car(Collection):\n\n        __collection__ = \'cars\'\n        _allow_extra_fields = True\n\n        make = String(required=True)\n        model = String(required=True)\n        year = Integer(required=True)\n        owner_key = String()\n\n        owner = relationship(Person, \'owner_key\', cache=False)\n\n        def __str__(self):\n            return "<Car({} - {} - {})>".format(self.make, self.model, self.year)\n\n    client = ArangoClient(hosts=\'http://localhost:8529\')\n    test_db = client.db(\'test\', username=\'test\', password=\'test\')\n    db = Database(test_db)\n\n    p = Person(_key=\'kashif\', name=\'Kashif Iftikhar\')\n    db.add(p)\n    p2 = Person(_key=\'azeen\', name=\'Azeen Kashif\')\n    db.add(p2)\n\n    c1 = Car(make=\'Honda\', model=\'Civic\', year=1984, owner_key=\'kashif\')\n    db.add(c1)\n\n    c2 = Car(make=\'Mitsubishi\', model=\'Lancer\', year=2005, owner_key=\'kashif\')\n    db.add(c2)\n\n    c3 = Car(make=\'Acme\', model=\'Toy Racer\', year=2016, owner_key=\'azeen\')\n    db.add(c3)\n\n    print(c1.owner)\n    print(c1.owner.name)\n    print(c2.owner.name)\n    print(c3.owner.name)\n\n    print(p.cars)\n    print(p.cars[0].make)\n    print(p2.cars)\n\n\nWorking With Graphs\n-------------------\n\nWorking with graphs involves creating collection classes and optionally Edge/Relation classes. Users can use the built-in Relation class for specifying relations but if relations need to contain extra attributes then it\'s required to create a sub-class of Relation class. Graph functionality is explain below with the help of a university graph example containing students, teachers, subjects and the areas where students and teachers reside in.\n\nFirst we create some collections and relationships\n\n.. code-block:: python\n\n    from arango_orm.fields import String, Date, Integer, Boolean\n    from arango_orm import Collection, Relation, Graph, GraphConnection\n\n\n    class Student(Collection):\n\n        __collection__ = \'students\'\n\n        _key = String(required=True)  # registration number\n        name = String(required=True, allow_none=False)\n        age = Integer()\n\n        def __str__(self):\n            return "<Student({})>".format(self.name)\n\n\n    class Teacher(Collection):\n\n        __collection__ = \'teachers\'\n\n        _key = String(required=True)  # employee id\n        name = String(required=True)\n\n        def __str__(self):\n            return "<Teacher({})>".format(self.name)\n\n\n    class Subject(Collection):\n\n        __collection__ = \'subjects\'\n\n        _key = String(required=True)  # subject code\n        name = String(required=True)\n        credit_hours = Integer()\n        has_labs = Boolean(missing=True)\n\n        def __str__(self):\n            return "<Subject({})>".format(self.name)\n\n\n    class Area(Collection):\n\n        __collection__ = \'areas\'\n\n        _key = String(required=True)  # area name\n\n\n    class SpecializesIn(Relation):\n\n        __collection__ = \'specializes_in\'\n\n        expertise_level = String(required=True, options=["expert", "medium", "basic"])\n\n        def __str__(self):\n            return "<SpecializesIn(_key={}, expertise_level={}, _from={}, _to={})>".format(\n                self._key, self.expertise_level, self._from, self._to)\n\n\nNext we sub-class the Graph class to specify the relationships between the various collections\n\n.. code-block:: python\n\n    class UniversityGraph(Graph):\n\n        __graph__ = \'university_graph\'\n\n        graph_connections = [\n            # Using general Relation class for relationship\n            GraphConnection(Student, Relation("studies"), Subject),\n            GraphConnection(Teacher, Relation("teaches"), Subject),\n\n            # Using specific classes for vertex and edges\n            GraphConnection(Teacher, SpecializesIn, Subject),\n            GraphConnection([Teacher, Student], Relation("resides_in"), Area)\n        ]\n\nNow it\'s time to create the graph. Note that we don\'t need to create the collections individually, creating the graph will create all collections that it contains\n\n.. code-block:: python\n\n    from arango import ArangoClient\n    from arango_orm.database import Database\n\n    client = ArangoClient(hosts=\'http://localhost:8529\')\n    test_db = client.db(\'test\', username=\'test\', password=\'test\')\n\n    db = Database(test_db)\n\n    uni_graph = UniversityGraph(connection=db)\n    db.create_graph(uni_graph)\n\n\nNow the graph and all it\'s collections have been created, we can verify their existence:\n\n.. code-block:: python\n\n    [c[\'name\'] for c in db.collections()]\n    db.graphs()\n\nNow let\'s insert some data into our graph:\n\n.. code-block:: python\n\n    students_data = [\n        Student(_key=\'S1001\', name=\'John Wayne\', age=30),\n        Student(_key=\'S1002\', name=\'Lilly Parker\', age=22),\n        Student(_key=\'S1003\', name=\'Cassandra Nix\', age=25),\n        Student(_key=\'S1004\', name=\'Peter Parker\', age=20)\n    ]\n\n    teachers_data = [\n        Teacher(_key=\'T001\', name=\'Bruce Wayne\'),\n        Teacher(_key=\'T002\', name=\'Barry Allen\'),\n        Teacher(_key=\'T003\', name=\'Amanda Waller\')\n    ]\n\n    subjects_data = [\n        Subject(_key=\'ITP101\', name=\'Introduction to Programming\', credit_hours=4, has_labs=True),\n        Subject(_key=\'CS102\', name=\'Computer History\', credit_hours=3, has_labs=False),\n        Subject(_key=\'CSOOP02\', name=\'Object Oriented Programming\', credit_hours=3, has_labs=True),\n    ]\n\n    areas_data = [\n        Area(_key="Gotham"),\n        Area(_key="Metropolis"),\n        Area(_key="StarCity")\n    ]\n\n    for s in students_data:\n        db.add(s)\n\n    for t in teachers_data:\n        db.add(t)\n\n    for s in subjects_data:\n        db.add(s)\n\n    for a in areas_data:\n        db.add(a)\n\nNext let\'s add some relations, we can add relations by manually adding the relation/edge record into the edge collection, like:\n\n.. code-block:: python\n\n    db.add(SpecializesIn(_from="teachers/T001", _to="subjects/ITP101", expertise_level="medium"))\n\nOr we can use the graph object\'s relation method to generate a relation document from given objects:\n\n.. code-block:: python\n\n    gotham = db.query(Area).by_key("Gotham")\n    metropolis = db.query(Area).by_key("Metropolis")\n    star_city = db.query(Area).by_key("StarCity")\n\n    john_wayne = db.query(Student).by_key("S1001")\n    lilly_parker = db.query(Student).by_key("S1002")\n    cassandra_nix = db.query(Student).by_key("S1003")\n    peter_parker = db.query(Student).by_key("S1004")\n\n    intro_to_prog = db.query(Subject).by_key("ITP101")\n    comp_history = db.query(Subject).by_key("CS102")\n    oop = db.query(Subject).by_key("CSOOP02")\n\n    barry_allen = db.query(Teacher).by_key("T002")\n    bruce_wayne = db.query(Teacher).by_key("T001")\n    amanda_waller = db.query(Teacher).by_key("T003")\n\n    db.add(uni_graph.relation(peter_parker, Relation("studies"), oop))\n    db.add(uni_graph.relation(peter_parker, Relation("studies"), intro_to_prog))\n    db.add(uni_graph.relation(john_wayne, Relation("studies"), oop))\n    db.add(uni_graph.relation(john_wayne, Relation("studies"), comp_history))\n    db.add(uni_graph.relation(lilly_parker, Relation("studies"), intro_to_prog))\n    db.add(uni_graph.relation(lilly_parker, Relation("studies"), comp_history))\n    db.add(uni_graph.relation(cassandra_nix, Relation("studies"), oop))\n    db.add(uni_graph.relation(cassandra_nix, Relation("studies"), intro_to_prog))\n\n    db.add(uni_graph.relation(barry_allen, SpecializesIn(expertise_level="expert"), oop))\n    db.add(uni_graph.relation(barry_allen, SpecializesIn(expertise_level="expert"), intro_to_prog))\n    db.add(uni_graph.relation(bruce_wayne, SpecializesIn(expertise_level="medium"), oop))\n    db.add(uni_graph.relation(bruce_wayne, SpecializesIn(expertise_level="expert"), comp_history))\n    db.add(uni_graph.relation(amanda_waller, SpecializesIn(expertise_level="basic"), intro_to_prog))\n    db.add(uni_graph.relation(amanda_waller, SpecializesIn(expertise_level="medium"), comp_history))\n\n    db.add(uni_graph.relation(bruce_wayne, Relation("teaches"), oop))\n    db.add(uni_graph.relation(barry_allen, Relation("teaches"), intro_to_prog))\n    db.add(uni_graph.relation(amanda_waller, Relation("teaches"), comp_history))\n\n    db.add(uni_graph.relation(bruce_wayne, Relation("resides_in"), gotham))\n    db.add(uni_graph.relation(barry_allen, Relation("resides_in"), star_city))\n    db.add(uni_graph.relation(amanda_waller, Relation("resides_in"), metropolis))\n    db.add(uni_graph.relation(john_wayne, Relation("resides_in"), gotham))\n    db.add(uni_graph.relation(lilly_parker, Relation("resides_in"), metropolis))\n    db.add(uni_graph.relation(cassandra_nix, Relation("resides_in"), star_city))\n    db.add(uni_graph.relation(peter_parker, Relation("resides_in"), metropolis))\n\nWith our graph populated with some sample data, let\'s explore the ways we can work with the graph.\n\n\nExpanding Documents\n___________________\n\nWe can expand any Collection (not Relation) object to access the data that is linked to it. We can sepcify which links (\'inbound\', \'outbound\', \'any\') to expand and the depth to which those should be expanded to. Let\'s see all immediate connections that Bruce Wayne has in our graph:\n\n.. code-block:: python\n\n    bruce = db.query(Teacher).by_key("T001")\n    uni_graph.expand(bruce, depth=1, direction=\'any\')\n\nGraph expansion on an object adds a **_relations** dictionary that contains all the relations for the object according to the expansion criteria:\n\n.. code-block:: python\n\n    bruce._relations\n\nReturns::\n\n    {\n    \'resides_in\': [<Relation(_key=4205290, _from=teachers/T001, _to=areas/Gotham)>],\n    \'specializes_in\': [<SpecializesIn(_key=4205114, expertise_level=medium, _from=teachers/T001, _to=subjects/ITP101)>,\n     <SpecializesIn(_key=4205271, expertise_level=expert, _from=teachers/T001, _to=subjects/CS102)>,\n     <SpecializesIn(_key=4205268, expertise_level=medium, _from=teachers/T001, _to=subjects/CSOOP02)>],\n    \'teaches\': [<Relation(_key=4205280, _from=teachers/T001, _to=subjects/CSOOP02)>]\n    }\n\nWe can use _from and _to of a relation object to access the id\'s for both sides of the link. We also have _object_from and _object_to to access the objects on both sides, for example:\n\n.. code-block:: python\n\n    bruce._relations[\'resides_in\'][0]._object_from.name\n    # \'Bruce Wayne\'\n\n    bruce._relations[\'resides_in\'][0]._object_to._key\n    # \'Gotham\'\n\nThere is also a special attribute called **_next** that allows accessing the other side of the relationship irrespective of the relationship direction. For example, for outbound relationships the _object_from contains the source object while for inbound_relationships _object_to contains the source object. But if we\'re only interested in traversal of the graph then it\'s more useful at times to access the other side of the relationship w.r.t the current object irrespective of it\'s direction:\n\n.. code-block:: python\n\n    bruce._relations[\'resides_in\'][0]._next._key\n    # \'Gotham\'\n\nLet\'s expand the bruce object to 2 levels and see **_next** in more action:\n\n.. code-block:: python\n\n    uni_graph.expand(bruce, depth=2)\n\n    # All relations of the area where bruce resides in\n    bruce._relations[\'resides_in\'][0]._object_to._relations\n    # -> {\'resides_in\': [<Relation(_key=4205300, _from=students/S1001, _to=areas/Gotham)>]}\n\n    # Name of the student that resides in the same area as bruce\n    bruce._relations[\'resides_in\'][0]._object_to._relations[\'resides_in\'][0]._object_from.name\n    # \'John Wayne\'\n\n    # The same action using _next without worrying about direction\n    bruce._relations[\'resides_in\'][0]._next._relations[\'resides_in\'][0]._next.name\n    # \'John Wayne\'\n\n    # Get names of all people that reside in the same area and Bruce Wayne\n    [p._next.name for p in bruce._relations[\'resides_in\'][0]._next._relations[\'resides_in\']]\n    # [\'John Wayne\']\n\n\nInheritance Mapping\n__________________________\n\nFor inheritance mapping, **arango_orm** offers you two ways to define it.\n\n1. Discriminator field/mapping:\n\nDiscriminator field/mapping are defined at entity level:\n\n.. code-block:: python\n\n    class Vehicle(Collection):\n        __collection__ = "vehicle"\n\n        _inheritance_field = "discr"\n        _inheritance_mapping = {\n            \'Bike\': \'moto\',\n            \'Truck\': \'truck\'\n        }\n\n        _key = String()\n        brand = String()\n        model = String()\n        # discr field match what you defined in _inheritance_field\n        # the field type depends on the values of your _inheritance_mapping\n        discr = String(required=True)\n\n\n    class Bike(Vehicle):\n        motor_size = Float()\n\n\n    class Truck(Vehicle):\n        traction_power = Float()\n\n\n2. Inheritance mapping resolver:\n\nThe `inheritance_mapping_resolver` is a function defined at graph level; it allows you to make either a simple test\non a discriminator field, or complex inference\n\n.. code-block:: python\n\n    class OwnershipGraph2(Graph):\n        __graph__ = "ownership_graph"\n\n        graph_connections = [\n            GraphConnection(Owner2, Own2, Vehicle2)\n        ]\n\n        def inheritance_mapping_resolver(self, col_name: str, doc_dict: dict = {}):\n            if col_name == \'vehicle\':\n                if \'traction_power\' in doc_dict:\n                    return Truck2\n                else:\n                    return Bike2\n\n            return self.vertices[col_name]\n\n\nGraph Traversal Using AQL\n__________________________\n\nThe graph module also supports traversals using AQL, the results are converted to objects and have the\nsame structure as graph.expand method:\n\n.. code-block:: python\n\n    obj = uni_graph.aql("FOR v, e, p IN 1..2 INBOUND \'areas/Gotham\' GRAPH \'university_graph\' RETURN p")\n    print(obj._key)\n    # Gotham\n\n    gotham_residents = [rel._next.name for rel in obj._relations[\'resides_in\']]\n    print(gotham_residents)\n    # [\'Bruce Wayne\', \'John Wayne\']\n\n\nFor Developers\n==============\n\nRunning the Test Cases\n----------------------\n\n```bash\nARANGO_HOSTS="http://127.0.0.1:8529" ARANGO_USERNAME=root ARANGO_PASSWORD=toor ARANGO_DATABASE=test_db pytest tests\n```\n',
     'author': 'Kashif Iftikhar',
     'author_email': 'kashif@compulife.com.pk',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://arango-orm.readthedocs.io/en/latest/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `arango_orm-0.7.1/PKG-INFO` & `arango_orm-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: arango-orm
-Version: 0.7.1
+Version: 0.7.2
 Summary: A SQLAlchemy like ORM implementation for arangodb
+Home-page: https://arango-orm.readthedocs.io/en/latest/
 License: GNU General Public License v2 (GPLv2)
 Author: Kashif Iftikhar
 Author-email: kashif@compulife.com.pk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: marshmallow (==3.15.0)
 Requires-Dist: python-arango (==7.1.0)
+Project-URL: Repository, https://github.com/kashifpk/arango-orm
 Description-Content-Type: text/x-rst
 
 Python ORM Layer For ArangoDB
 =============================
 
 **arango_orm** is a python ORM layer inspired by SQLAlchemy but aimed to work
 with the multi-model database ArangoDB. It supports accessing both collections
```

