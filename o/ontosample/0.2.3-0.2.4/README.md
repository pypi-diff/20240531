# Comparing `tmp/ontosample-0.2.3.tar.gz` & `tmp/ontosample-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontosample-0.2.3.tar", last modified: Wed May 22 13:32:17 2024, max compression
+gzip compressed data, was "ontosample-0.2.4.tar", last modified: Fri May 31 14:19:07 2024, max compression
```

## Comparing `ontosample-0.2.3.tar` & `ontosample-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.365126 ontosample-0.2.3/
--rw-rw-rw-   0        0        0    35184 2023-06-04 12:41:29.000000 ontosample-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     7753 2024-05-22 13:32:17.363878 ontosample-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     6945 2024-02-15 21:59:40.000000 ontosample-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.340467 ontosample-0.2.3/ontolearn_light/
--rw-rw-rw-   0        0        0       23 2024-05-21 12:09:14.000000 ontosample-0.2.3/ontolearn_light/__init__.py
--rw-rw-rw-   0        0        0    20532 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/abstracts.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.344906 ontosample-0.2.3/ontolearn_light/base/
--rw-rw-rw-   0        0        0      740 2024-05-21 14:36:30.000000 ontosample-0.2.3/ontolearn_light/base/__init__.py
--rw-rw-rw-   0        0        0    45660 2024-05-21 14:39:38.000000 ontosample-0.2.3/ontolearn_light/base/_base.py
--rw-rw-rw-   0        0        0    32628 2024-05-21 14:39:38.000000 ontosample-0.2.3/ontolearn_light/base/axioms.py
--rw-rw-rw-   0        0        0     5345 2024-05-21 14:39:38.000000 ontosample-0.2.3/ontolearn_light/base/complex_ce_instances.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.346419 ontosample-0.2.3/ontolearn_light/base/ext/
--rw-rw-rw-   0        0        0     4219 2024-04-22 13:06:57.000000 ontosample-0.2.3/ontolearn_light/base/ext/__init__.py
--rw-rw-rw-   0        0        0    27223 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/base/fast_instance_checker.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.349567 ontosample-0.2.3/ontolearn_light/base/owl/
--rw-rw-rw-   0        0        0       20 2023-11-21 13:25:19.000000 ontosample-0.2.3/ontolearn_light/base/owl/__init__.py
--rw-rw-rw-   0        0        0    17545 2024-04-22 13:25:14.000000 ontosample-0.2.3/ontolearn_light/base/owl/hierarchy.py
--rw-rw-rw-   0        0        0    24949 2024-04-22 13:25:14.000000 ontosample-0.2.3/ontolearn_light/base/owl/utils.py
--rw-rw-rw-   0        0        0    16573 2024-04-23 12:09:16.000000 ontosample-0.2.3/ontolearn_light/base/utils.py
--rw-rw-rw-   0        0        0    10334 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/concept_generator.py
--rw-rw-rw-   0        0        0    11689 2024-03-25 16:12:36.000000 ontosample-0.2.3/ontolearn_light/data_struct.py
--rw-rw-rw-   0        0        0      681 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/fitness_functions.py
--rw-rw-rw-   0        0        0    55971 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/knowledge_base.py
--rw-rw-rw-   0        0        0     2850 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/learning_problem.py
--rw-rw-rw-   0        0        0     3192 2023-10-10 12:27:39.000000 ontosample-0.2.3/ontolearn_light/metrics.py
--rw-rw-rw-   0        0        0    28669 2024-05-21 12:09:14.000000 ontosample-0.2.3/ontolearn_light/search.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.353064 ontosample-0.2.3/ontolearn_light/utils/
--rw-rw-rw-   0        0        0     6780 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/utils/__init__.py
--rw-rw-rw-   0        0        0     1208 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/utils/log_config.py
--rw-rw-rw-   0        0        0      216 2023-10-12 13:01:03.000000 ontosample-0.2.3/ontolearn_light/utils/oplogging.py
--rw-rw-rw-   0        0        0     6298 2024-05-22 13:25:05.000000 ontosample-0.2.3/ontolearn_light/utils/static_funcs.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.356841 ontosample-0.2.3/ontosample/
--rw-rw-rw-   0        0        0        0 2023-11-22 19:49:53.000000 ontosample-0.2.3/ontosample/__init__.py
--rw-rw-rw-   0        0        0    12200 2024-05-21 14:30:42.000000 ontosample-0.2.3/ontosample/_base.py
--rw-rw-rw-   0        0        0    17350 2024-05-21 14:34:34.000000 ontosample-0.2.3/ontosample/classic_samplers.py
--rw-rw-rw-   0        0        0    14067 2024-05-21 14:34:34.000000 ontosample-0.2.3/ontosample/lpc_samplers.py
--rw-rw-rw-   0        0        0     6710 2024-05-21 14:34:34.000000 ontosample-0.2.3/ontosample/lpf_samplers.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.362607 ontosample-0.2.3/ontosample.egg-info/
--rw-rw-rw-   0        0        0     7753 2024-05-22 13:32:17.000000 ontosample-0.2.3/ontosample.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2024-05-22 13:32:17.000000 ontosample-0.2.3/ontosample.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:32:17.000000 ontosample-0.2.3/ontosample.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2024-05-22 13:32:17.000000 ontosample-0.2.3/ontosample.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-22 13:32:17.000000 ontosample-0.2.3/ontosample.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       93 2023-06-04 12:41:29.000000 ontosample-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 13:32:17.365126 ontosample-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1017 2024-05-22 13:29:08.000000 ontosample-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:19:07.308831 ontosample-0.2.4/
+-rw-rw-rw-   0        0        0    35184 2023-06-04 12:41:29.000000 ontosample-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     7781 2024-05-31 14:19:07.308831 ontosample-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6945 2024-02-15 21:59:40.000000 ontosample-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 14:19:07.293069 ontosample-0.2.4/ontolearn_light/
+-rw-rw-rw-   0        0        0       23 2024-05-21 12:09:14.000000 ontosample-0.2.4/ontolearn_light/__init__.py
+-rw-rw-rw-   0        0        0    20533 2024-05-31 14:14:35.000000 ontosample-0.2.4/ontolearn_light/abstracts.py
+-rw-rw-rw-   0        0        0    10334 2024-05-21 14:46:58.000000 ontosample-0.2.4/ontolearn_light/concept_generator.py
+-rw-rw-rw-   0        0        0    11689 2024-03-25 16:12:36.000000 ontosample-0.2.4/ontolearn_light/data_struct.py
+-rw-rw-rw-   0        0        0     6510 2024-05-31 14:09:07.000000 ontosample-0.2.4/ontolearn_light/ea_utils.py
+-rw-rw-rw-   0        0        0      681 2024-05-21 14:46:58.000000 ontosample-0.2.4/ontolearn_light/fitness_functions.py
+-rw-rw-rw-   0        0        0    55731 2024-05-31 14:07:49.000000 ontosample-0.2.4/ontolearn_light/knowledge_base.py
+-rw-rw-rw-   0        0        0     2850 2024-05-21 14:46:58.000000 ontosample-0.2.4/ontolearn_light/learning_problem.py
+-rw-rw-rw-   0        0        0     3192 2023-10-10 12:27:39.000000 ontosample-0.2.4/ontolearn_light/metrics.py
+-rw-rw-rw-   0        0        0    28668 2024-05-31 14:07:49.000000 ontosample-0.2.4/ontolearn_light/search.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:19:07.297369 ontosample-0.2.4/ontolearn_light/utils/
+-rw-rw-rw-   0        0        0     6780 2024-05-21 14:46:58.000000 ontosample-0.2.4/ontolearn_light/utils/__init__.py
+-rw-rw-rw-   0        0        0     1208 2024-05-21 14:46:58.000000 ontosample-0.2.4/ontolearn_light/utils/log_config.py
+-rw-rw-rw-   0        0        0      216 2023-10-12 13:01:03.000000 ontosample-0.2.4/ontolearn_light/utils/oplogging.py
+-rw-rw-rw-   0        0        0     5772 2024-05-31 14:14:35.000000 ontosample-0.2.4/ontolearn_light/utils/static_funcs.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:19:07.301832 ontosample-0.2.4/ontosample/
+-rw-rw-rw-   0        0        0        0 2023-11-22 19:49:53.000000 ontosample-0.2.4/ontosample/__init__.py
+-rw-rw-rw-   0        0        0    12064 2024-05-31 14:07:49.000000 ontosample-0.2.4/ontosample/_base.py
+-rw-rw-rw-   0        0        0    17350 2024-05-21 14:34:34.000000 ontosample-0.2.4/ontosample/classic_samplers.py
+-rw-rw-rw-   0        0        0    14067 2024-05-21 14:34:34.000000 ontosample-0.2.4/ontosample/lpc_samplers.py
+-rw-rw-rw-   0        0        0     6710 2024-05-21 14:34:34.000000 ontosample-0.2.4/ontosample/lpf_samplers.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:19:07.307830 ontosample-0.2.4/ontosample.egg-info/
+-rw-rw-rw-   0        0        0     7781 2024-05-31 14:19:07.000000 ontosample-0.2.4/ontosample.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      794 2024-05-31 14:19:07.000000 ontosample-0.2.4/ontosample.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 14:19:07.000000 ontosample-0.2.4/ontosample.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2024-05-31 14:19:07.000000 ontosample-0.2.4/ontosample.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-31 14:19:07.000000 ontosample-0.2.4/ontosample.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       93 2023-06-04 12:41:29.000000 ontosample-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 14:19:07.309827 ontosample-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2024-05-31 14:14:35.000000 ontosample-0.2.4/setup.py
```

### Comparing `ontosample-0.2.3/LICENSE` & `ontosample-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/PKG-INFO` & `ontosample-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontosample
-Version: 0.2.3
+Version: 0.2.4
 Summary: Ontosample is a package that offers different sampling techniques for OWL ontologies.
 Home-page: https://github.com/alkidbaci/OntoSample
 Author: Alkid Baci
 Author-email: alkid1baci@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -14,14 +14,15 @@
 Requires-Dist: matplotlib>=3.3.4
 Requires-Dist: owlready2>=0.40
 Requires-Dist: torch>=1.7.1
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: sortedcontainers>=2.4.0
 Requires-Dist: owlapy==1.0.2
 Requires-Dist: requests>=2.31.0
+Requires-Dist: deap>=1.3.1
 
 # OntoSample
 
 OntoSample is a python package that offers classic sampling techniques for OWL ontologies/knowledge 
 bases. Furthermore, we have tailored the classic sampling techniques to the setting of concept 
 learning making use of learning problem.
```

### Comparing `ontosample-0.2.3/README.md` & `ontosample-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/ontolearn_light/abstracts.py` & `ontosample-0.2.4/ontolearn_light/abstracts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The main abstract classes."""
 
 import logging
 from abc import ABCMeta, abstractmethod
 from typing import Set, List, Tuple, Iterable, TypeVar, Generic, ClassVar, Optional
 from owlapy.class_expression import OWLClassExpression
 from owlapy.owl_ontology import OWLOntology
-from owlapy.util import iter_count
+from owlapy.utils import iter_count
 from .data_struct import Experience
 from .utils import read_csv
 from collections import OrderedDict
 
 _N = TypeVar('_N')  #:
 _KB = TypeVar('_KB', bound='AbstractKnowledgeBase')  #:
```

### Comparing `ontosample-0.2.3/ontolearn_light/base/_base.py` & `ontosample-0.2.4/ontolearn_light/knowledge_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,867 +1,1190 @@
-import logging
-from datetime import date, datetime
-from enum import Enum, auto
-from itertools import chain
-from types import MappingProxyType
-from typing import Iterable, Set, Final, List
+""" Knowledge Base."""
 
-import owlready2
-from owlapy.class_expression import OWLClassExpression, OWLThing, OWLClass, OWLObjectSomeValuesFrom
+import logging
+import random
+from collections import Counter
+from typing import Iterable, Optional, Callable, overload, Union, FrozenSet, Set, Dict, cast, Generator
+
+import owlapy
+from owlapy.class_expression import OWLClassExpression, OWLClass, OWLObjectSomeValuesFrom, OWLObjectAllValuesFrom, \
+    OWLThing, OWLObjectMinCardinality, OWLObjectOneOf
 from owlapy.iri import IRI
-from owlapy.owl_axiom import OWLObjectPropertyRangeAxiom, OWLAxiom, OWLObjectPropertyDomainAxiom, \
-    OWLDataPropertyRangeAxiom, OWLDataPropertyDomainAxiom, OWLClassAxiom, OWLSubClassOfAxiom, OWLEquivalentClassesAxiom
+from owlapy.owl_axiom import OWLClassAssertionAxiom, OWLObjectPropertyAssertionAxiom, OWLDataPropertyAssertionAxiom, \
+    OWLSubClassOfAxiom, OWLEquivalentClassesAxiom
+from owlapy.owl_datatype import OWLDatatype
 from owlapy.owl_individual import OWLNamedIndividual
-from owlapy.owl_literal import DoubleOWLDatatype, OWLLiteral, BooleanOWLDatatype, IntegerOWLDatatype, DateOWLDatatype, \
-    DateTimeOWLDatatype, DurationOWLDatatype, StringOWLDatatype
-from owlapy.owl_ontology import OWLOntologyID, OWLOntology
-from owlapy.owl_ontology_manager import OWLOntologyManager, OWLOntologyChange, AddImport
-from owlapy.owl_property import OWLDataProperty, OWLObjectPropertyExpression, OWLObjectInverseOf, OWLObjectProperty
-from owlready2 import declare_datatype
-from pandas import Timedelta
-
-from owlapy.converter import Owl2SparqlConverter
-from ontolearn_light.base import axioms
-from owlapy import namespaces
-from ontolearn_light.base.ext import OWLReasonerEx
-from ontolearn_light.base.utils import FromOwlready2
+from owlapy.owl_literal import BooleanOWLDatatype, NUMERIC_DATATYPES, DoubleOWLDatatype, TIME_DATATYPES, OWLLiteral
+from owlapy.owl_ontology import OWLOntology
+from owlapy.owl_ontology_manager import OWLOntologyManager
+from owlapy.owl_property import OWLObjectProperty, OWLDataProperty, OWLObjectPropertyExpression, \
+    OWLDataPropertyExpression
+from owlapy.owl_reasoner import OWLReasoner
+
+from owlapy.owl_ontology import Ontology
+from owlapy.owl_ontology_manager import OntologyManager
+from owlapy.owl_reasoner import FastInstanceCheckerReasoner, OntologyReasoner
+
+from owlapy.render import DLSyntaxObjectRenderer
+from ontolearn_light.search import EvaluatedConcept
+from .abstracts import AbstractKnowledgeBase, AbstractScorer, EncodedLearningProblem
+from .concept_generator import ConceptGenerator
+from owlapy.utils import OWLClassExpressionLengthMetric, iter_count, LRUCache
+from .learning_problem import PosNegLPStandard, EncodedPosNegLPStandard
+from owlapy.owl_hierarchy import ClassHierarchy, ObjectPropertyHierarchy, DatatypePropertyHierarchy
+
+from .utils.static_funcs import (init_length_metric, init_hierarchy_instances,
+                                 init_named_individuals, init_individuals_from_concepts)
+
+from owlapy.class_expression import OWLDataMaxCardinality, OWLDataSomeValuesFrom
+from owlapy import owl_expression_to_sparql, owl_expression_to_dl
+from owlapy.owl_data_ranges import OWLDataRange
+from owlapy.class_expression import OWLDataOneOf
 
 logger = logging.getLogger(__name__)
 
-_Datatype_map: Final = MappingProxyType({
-    int: IntegerOWLDatatype,
-    float: DoubleOWLDatatype,
-    bool: BooleanOWLDatatype,
-    str: StringOWLDatatype,
-    date: DateOWLDatatype,
-    datetime: DateTimeOWLDatatype,
-    Timedelta: DurationOWLDatatype,
-})
 
-_parse_concept_to_owlapy = FromOwlready2().map_concept
-_parse_datarange_to_owlapy = FromOwlready2().map_datarange
+def depth_Default_ReasonerFactory(onto: OWLOntology) -> OWLReasoner:
+    assert isinstance(onto, Ontology)
+    base_reasoner = OntologyReasoner(ontology=onto)
+    return FastInstanceCheckerReasoner(ontology=onto, base_reasoner=base_reasoner)
+
+
+class KnowledgeBase(AbstractKnowledgeBase):
+    """Representation of an OWL knowledge base in Ontolearn.
+
+    Args:
+        path: Path to an ontology file that is to be loaded.
+        ontologymanager_factory: Factory that creates an ontology manager to be used to load the file.
+        ontology: OWL ontology object.
+        reasoner_factory: Factory that creates a reasoner to reason about the ontology.
+        reasoner: reasoner Over the ontology.
+        length_metric_factory: See :attr:`length_metric`.
+        length_metric: Length metric that is used in calculation of class expression lengths.
+        individuals_cache_size: How many individuals of class expressions to cache.
+        backend_store: Whether to sync the world to backend store.
+            reasoner of this object, if you enter a reasoner using :arg:`reasoner_factory` or :arg:`reasoner`
+            argument it will override this setting.
+        include_implicit_individuals: Whether to identify and consider instances which are not set as OWL Named
+            Individuals (does not contain this type) as individuals.
 
-_VERSION_IRI: Final = IRI.create(namespaces.OWL, "versionIRI")
+    Attributes:
+        generator (ConceptGenerator): Instance of concept generator.
+        path (str): Path of the ontology file.
+        use_individuals_cache (bool): Whether to use individuals cache to store individuals for method efficiency.
+    """
+    # __slots__ = '_manager', '_ontology', '_reasoner', '_length_metric', \
+    #    '_ind_set', '_ind_cache', 'path', 'use_individuals_cache', 'generator', '_class_hierarchy', \
+    #    '_object_property_hierarchy', '_data_property_hierarchy', '_op_domains', '_op_ranges', '_dp_domains', \
+    #    '_dp_ranges'
+
+    length_metric: OWLClassExpressionLengthMetric
+
+    ind_set: FrozenSet[OWLNamedIndividual]
+    ind_cache: LRUCache[OWLClassExpression, FrozenSet[OWLNamedIndividual]]  # class expression => individuals
+
+    path: str
+    use_individuals_cache: bool
+    generator: ConceptGenerator
+
+    @overload
+    def __init__(self, *,
+                 path: str,
+                 ontologymanager_factory: Callable[[], OWLOntologyManager] = OntologyManager(
+                     world_store=None),
+                 reasoner_factory: Callable[[OWLOntology], OWLReasoner] = None,
+                 length_metric: Optional[OWLClassExpressionLengthMetric] = None,
+                 length_metric_factory: Optional[Callable[[], OWLClassExpressionLengthMetric]] = None,
+                 individuals_cache_size=128,
+                 backend_store: bool = False,
+                 include_implicit_individuals=False):
+        ...
+
+    @overload
+    def __init__(self, *,
+                 ontology: OWLOntology,
+                 reasoner: OWLReasoner,
+                 load_class_hierarchy: bool = True,
+                 length_metric: Optional[OWLClassExpressionLengthMetric] = None,
+                 length_metric_factory: Optional[Callable[[], OWLClassExpressionLengthMetric]] = None,
+                 individuals_cache_size=128):
+        ...
+
+    def __init__(self, *,
+                 path: Optional[str] = None,
+
+                 ontologymanager_factory: Optional[Callable[[], OWLOntologyManager]] = None,
+                 reasoner_factory: Optional[Callable[[OWLOntology], OWLReasoner]] = None,
+                 length_metric_factory: Optional[Callable[[], OWLClassExpressionLengthMetric]] = None,
+
+                 ontology: Optional[OWLOntology] = None,
+                 reasoner: Optional[OWLReasoner] = None,
+                 length_metric: Optional[OWLClassExpressionLengthMetric] = None,
+
+                 individuals_cache_size=128,
+                 backend_store: bool = False,
+                 class_hierarchy: Optional[ClassHierarchy] = None,
+                 load_class_hierarchy: bool = True,
+                 object_property_hierarchy: Optional[ObjectPropertyHierarchy] = None,
+                 data_property_hierarchy: Optional[DatatypePropertyHierarchy] = None,
+                 include_implicit_individuals=False
+                 ):
+        AbstractKnowledgeBase.__init__(self)
+        self.path = path
+
+        if ontology is not None:
+            self.manager = ontology.get_owl_ontology_manager()
+            self.ontology = ontology
+        elif ontologymanager_factory is not None:
+            self.manager = ontologymanager_factory()
+        else:  # default to Owlready2 implementation
+            if path is not None and backend_store:
+                self.manager = OntologyManager(world_store=path + ".or2")
+            else:
+                self.manager = OntologyManager(world_store=None)
+            # raise TypeError("neither ontology nor manager factory given")
 
+        if ontology is None:
+            if path is None:
+                raise TypeError("path missing")
+            else:
+                self.ontology = self.manager.load_ontology(IRI.create('file://' + self.path))
+                if isinstance(self.manager, OntologyManager) and backend_store:
+                    self.manager.save_world()
+                    logger.debug("Synced world to backend store")
+
+        reasoner: OWLReasoner
+        if reasoner is not None:
+            self.reasoner = reasoner
+        elif reasoner_factory is not None:
+            self.reasoner = reasoner_factory(self.ontology)
+        else:
+            self.reasoner = FastInstanceCheckerReasoner(ontology=self.ontology, base_reasoner=OntologyReasoner(
+                                                                                                ontology=self.ontology))
+
+        self.length_metric = init_length_metric(length_metric, length_metric_factory)
+
+        if load_class_hierarchy:
+            self.class_hierarchy: ClassHierarchy
+            self.object_property_hierarchy: ObjectPropertyHierarchy
+            self.data_property_hierarchy: DatatypePropertyHierarchy
+            (self.class_hierarchy,
+             self.object_property_hierarchy,
+             self.data_property_hierarchy) = init_hierarchy_instances(self.reasoner,
+                                                                      class_hierarchy=class_hierarchy,
+                                                                      object_property_hierarchy=object_property_hierarchy,
+                                                                      data_property_hierarchy=data_property_hierarchy)
+        # Object property domain and range:
+        self.op_domains: Dict[OWLObjectProperty, OWLClassExpression]
+        self.op_domains = dict()
+        self.op_ranges: Dict[OWLObjectProperty, OWLClassExpression]
+        self.op_ranges = dict()
+        # Data property domain and range:g
+        self.dp_domains: Dict[OWLDataProperty, OWLClassExpression]
+        self.dp_domains = dict()
+        self.dp_ranges: Dict[OWLDataProperty, FrozenSet[OWLDataRange]]
+        self.dp_ranges = dict()
+        # OWL class expression generator
+        self.generator = ConceptGenerator()
+
+        self.use_individuals_cache, self.ind_cache = init_named_individuals(individuals_cache_size)
+        self.ind_set = init_individuals_from_concepts(include_implicit_individuals,
+                                                      reasoner=self.reasoner,
+                                                      ontology=self.ontology,
+                                                      individuals_per_concept=(self.individuals(i) for i in
+                                                                               self.get_concepts()))
 
-def _parse_duration_datatype(literal: str):
-    return Timedelta(literal)
+        self.describe()
 
+    def individuals(self, concept: Optional[OWLClassExpression] = None) -> Iterable[OWLNamedIndividual]:
+        """Given an OWL class expression, retrieve all individuals belonging to it.
 
-def _unparse_duration_datatype(literal: Timedelta):
-    return literal.isoformat()
 
+        Args:
+            concept: Class expression of which to list individuals.
+        Returns:
+            Individuals belonging to the given class.
+        """
 
-declare_datatype(Timedelta, IRI.create(namespaces.XSD, "duration").as_str(),
-                 _parse_duration_datatype, _unparse_duration_datatype)
+        if concept is None or concept.is_owl_thing():
+            for i in self.ind_set:
+                yield i
+        else:
+            yield from self.maybe_cache_individuals(concept)
 
+    def abox(self, individual: Union[OWLNamedIndividual, Iterable[OWLNamedIndividual]] = None, mode='native'):
+        """
+        Get all the abox axioms for a given individual. If no individual is given, get all abox axioms
 
-class BaseReasoner_Owlready2(Enum):
-    """Enumeration class for base reasoner when calling sync_reasoner.
+        Args:
+            individual (OWLNamedIndividual): Individual/s to get the abox axioms from.
+            mode (str): The return format.
+             1) 'native' -> returns triples as tuples of owlapy objects,
+             2) 'iri' -> returns triples as tuples of IRIs as string,
+             3) 'axiom' -> triples are represented by owlapy axioms.
 
-    Attributes:
-        PELLET: Pellet base reasoner.
-        HERMIT: HermiT base reasoner.
-    """
-    PELLET = auto()
-    HERMIT = auto()
+        Returns: Iterable of tuples or owlapy axiom, depending on the mode.
+        """
 
+        assert mode in ['native', 'iri', 'axiom',
+                        "expression"], "Valid modes are: 'native', 'iri' ,'expression' or 'axiom'"
 
-class OWLOntologyManager_Owlready2(OWLOntologyManager):
-    __slots__ = '_world'
+        if isinstance(individual, OWLNamedIndividual):
+            inds = [individual]
+        elif isinstance(individual, Iterable):
+            inds = individual
+        else:
+            inds = self.individuals()
+
+        for i in inds:
+            if mode == "native":
+                # Obtain all class assertion triples/axioms
+                # For now, 'rdfs:type' predicate will be represented as an IRI
+                yield from ((i, IRI.create("http://www.w3.org/1999/02/22-rdf-syntax-ns#type"), t) for t in
+                            self.get_types(ind=i, direct=True))
+
+                # Obtain all property assertion triples/axioms
+                for dp in self.get_data_properties_for_ind(ind=i):
+                    yield from ((i, dp, literal) for literal in self.get_data_property_values(i, dp))
+
+                for op in self.get_object_properties_for_ind(ind=i):
+                    yield from ((i, op, ind) for ind in self.get_object_property_values(i, op))
+            elif mode == "iri":
+                yield from ((i.str, "http://www.w3.org/1999/02/22-rdf-syntax-ns#type",
+                             t.str) for t in self.get_types(ind=i, direct=True))
+                for dp in self.get_data_properties_for_ind(ind=i):
+                    yield from ((i.str, dp.str, literal.get_literal()) for literal in
+                                self.get_data_property_values(i, dp))
+                for op in self.get_object_properties_for_ind(ind=i):
+                    yield from ((i.str, op.str, ind.str) for ind in
+                                self.get_object_property_values(i, op))
+            elif mode == "axiom":
+                yield from (OWLClassAssertionAxiom(i, t) for t in self.get_types(ind=i, direct=True))
+                for dp in self.get_data_properties_for_ind(ind=i):
+                    yield from (OWLDataPropertyAssertionAxiom(i, dp, literal) for literal in
+                                self.get_data_property_values(i, dp))
+                for op in self.get_object_properties_for_ind(ind=i):
+                    yield from (OWLObjectPropertyAssertionAxiom(i, op, ind) for ind in
+                                self.get_object_property_values(i, op))
+            elif mode == "expression":
+                object_restrictions_quantifiers = dict()
+                # To no return duplicate objects.
+                quantifier_gate = set()
+                # (1) Iterate over triples where individual is in the subject position. Recursion
+                for s, p, o in self.abox(individual=individual, mode="native"):
+                    if isinstance(p, IRI) and isinstance(o, OWLClass):
+                        """ Return OWLClass """
+                        yield o
+                    elif isinstance(p, OWLObjectProperty) and isinstance(o, OWLNamedIndividual):
+                        """ STORE: ObjectSomeValuesFrom with ObjectOneOf over OWLNamedIndividual"""
+                        object_restrictions_quantifiers.setdefault(p, []).append(o)
+                    elif isinstance(p, OWLDataProperty) and isinstance(o, OWLLiteral):
+                        """ RETURN: OWLDataSomeValuesFrom with OWLDataOneOf over OWLLiteral"""
+                        yield OWLDataSomeValuesFrom(property=p, filler=OWLDataOneOf(o))
+                    else:
+                        raise RuntimeError("Unrecognized triples to expression mappings")
+
+                for k, iter_inds in object_restrictions_quantifiers.items():
+                    # RETURN Existential Quantifiers over Nominals: \exists r. {x....y}
+                    for x in iter_inds:
+                        yield OWLObjectSomeValuesFrom(property=k, filler=OWLObjectOneOf(values=x))
+                    type_: OWLClass
+                    count: int
+                    for type_, count in Counter(
+                            [type_i for i in iter_inds for type_i in self.get_types(ind=i, direct=True)]).items():
+                        existential_quantifier = OWLObjectSomeValuesFrom(property=k, filler=type_)
+                        if existential_quantifier in quantifier_gate:
+                            continue
+                        else:
+                            # RETURN Existential Quantifiers over Concepts: \exists r. C
+                            quantifier_gate.add(existential_quantifier)
+                            yield existential_quantifier
+                        if count > 1:
+                            min_cardinality_item = OWLObjectMinCardinality(cardinality=count, property=k, filler=type_)
+                            if min_cardinality_item in quantifier_gate:
+                                continue
+                            else:
+                                quantifier_gate.add(min_cardinality_item)
+                                # RETURN \ge number r. C
+                                yield min_cardinality_item
 
-    _world: owlready2.namespace.World
 
-    def __init__(self, world_store=None):
-        """Ontology manager in Ontolearn.
-        Creates a world where ontology is loaded.
-        Used to make changes in the ontology.
+            else:
+                raise RuntimeError(f"Unrecognized mode:{mode}")
+
+    def tbox(self, entities: Union[Iterable[OWLClass], Iterable[OWLDataProperty], Iterable[OWLObjectProperty], OWLClass,
+    OWLDataProperty, OWLObjectProperty, None] = None, mode='native'):
+        """Get all the tbox axioms for the given concept-s|propert-y/ies.
+         If no concept-s|propert-y/ies are given, get all tbox axioms.
+
+         Args:
+             @TODO: entities or namedindividuals ?!
+             entities: Entities to obtain tbox axioms from. This can be a single
+              OWLClass/OWLDataProperty/OWLObjectProperty object, a list of those objects or None. If you enter a list
+              that combines classes and properties (which we don't recommend doing), only axioms for one type will be
+              returned, whichever comes first (classes or props).
+             mode (str): The return format.
+              1) 'native' -> returns triples as tuples of owlapy objects,
+              2) 'iri' -> returns triples as tuples of IRIs as string,
+              3) 'axiom' -> triples are represented by owlapy axioms.
+
+         Returns: Iterable of tuples or owlapy axiom, depending on the mode.
+
+        """
+        assert mode in ['native', 'iri', 'axiom'], "Valid modes are: 'native', 'iri' or 'axiom'"
+        if mode == "iri":
+            print("WARN  KnowledgeBase.tbox()    :: Ranges of data properties are not implemented for the 'iri' mode!")
+        include_all = False
+        results = set()  # Using a set to avoid yielding duplicated results.
+        classes = False
+        if isinstance(entities, Iterable):
+            ens = list(entities)
+            if isinstance(ens[0], OWLClass):
+                classes = True
+        elif not isinstance(entities, Iterable) and entities:
+            ens = [entities]
+            if isinstance(entities, OWLClass):
+                classes = True
+        else:
+            ens = list(self.get_concepts())
+            ens.extend(list(self.get_object_properties()))
+            ens.extend(list(self.get_data_properties()))
+            include_all = True
+
+        if include_all or classes:
+            for concept in ens:
+                if not isinstance(concept, OWLClass):
+                    continue
+                if mode == 'native':
+                    [results.add((j, IRI.create("http://www.w3.org/2000/01/rdf-schema#subClassOf"), concept)) for j in
+                     self.get_direct_sub_concepts(concept)]
+                    [results.add((concept, IRI.create("http://www.w3.org/2002/07/owl#equivalentClass"), j)) for j in
+                     self.reasoner.equivalent_classes(concept, only_named=True)]
+                    if not include_all:  # This kind of check is just for performance purposes
+                        [results.add((concept, IRI.create("http://www.w3.org/2000/01/rdf-schema#subClassOf"), j)) for j
+                         in
+                         self.get_direct_parents(concept)]
+                elif mode == 'iri':
+                    [results.add((j.str, "http://www.w3.org/2000/01/rdf-schema#subClassOf",
+                                  concept.str)) for j in self.get_direct_sub_concepts(concept)]
+                    [results.add((concept.str, "http://www.w3.org/2002/07/owl#equivalentClass",
+                                  cast(OWLClass, j).str)) for j in
+                     self.reasoner.equivalent_classes(concept, only_named=True)]
+                    if not include_all:
+                        [results.add((concept.str, "http://www.w3.org/2000/01/rdf-schema#subClassOf",
+                                      j.str)) for j in self.get_direct_parents(concept)]
+                elif mode == "axiom":
+                    [results.add(OWLSubClassOfAxiom(super_class=concept, sub_class=j)) for j in
+                     self.get_direct_sub_concepts(concept)]
+                    [results.add(OWLEquivalentClassesAxiom([concept, j])) for j in
+                     self.reasoner.equivalent_classes(concept, only_named=True)]
+                    if not include_all:
+                        [results.add(OWLSubClassOfAxiom(super_class=j, sub_class=concept)) for j in
+                         self.get_direct_parents(concept)]
+        if include_all or not classes:
+            for prop in ens:
+                if isinstance(prop, OWLObjectProperty):
+                    prop_type = "Object"
+                elif isinstance(prop, OWLDataProperty):
+                    prop_type = "Data"
+                else:
+                    continue
+                if mode == 'native':
+                    [results.add((j, IRI.create("http://www.w3.org/2000/01/rdf-schema#subPropertyOf"), prop)) for j in
+                     getattr(self.reasoner, "sub_" + prop_type.lower() + "_properties")(prop, direct=True)]
+                    [results.add((prop, IRI.create("http://www.w3.org/2002/07/owl#equivalentProperty"), j)) for j in
+                     getattr(self.reasoner, "equivalent_" + prop_type.lower() + "_properties")(prop)]
+                    [results.add((prop, IRI.create("http://www.w3.org/2000/01/rdf-schema#domain"), j)) for j in
+                     getattr(self.reasoner, prop_type.lower() + "_property_domains")(prop, direct=True)]
+                    [results.add((prop, IRI.create("http://www.w3.org/2000/01/rdf-schema#range"), j)) for j in
+                     getattr(self.reasoner, prop_type.lower() + "_property_ranges")(prop, direct=True)]
+                    if not include_all:
+                        [results.add((prop, IRI.create("http://www.w3.org/2000/01/rdf-schema#subPropertyOf"), j)) for j
+                         in getattr(self.reasoner, "super_" + prop_type.lower() + "_properties")(prop, direct=True)]
+                elif mode == 'iri':
+                    [results.add((j.str, "http://www.w3.org/2000/01/rdf-schema#subPropertyOf",
+                                  prop.str)) for j in
+                     getattr(self.reasoner, "sub_" + prop_type.lower() + "_properties")(prop, direct=True)]
+                    [results.add((prop.str, "http://www.w3.org/2002/07/owl#equivalentProperty",
+                                  j.str)) for j in
+                     getattr(self.reasoner, "equivalent_" + prop_type.lower() + "_properties")(prop)]
+                    [results.add((prop.str, "http://www.w3.org/2000/01/rdf-schema#domain",
+                                  j.str)) for j in
+                     getattr(self.reasoner, prop_type.lower() + "_property_domains")(prop, direct=True)]
+                    if prop_type == 'Object':
+                        [results.add((prop.str, "http://www.w3.org/2000/01/rdf-schema#range",
+                                      j.str)) for j in
+                         self.reasoner.object_property_ranges(prop, direct=True)]
+                    # # ranges of data properties not implemented for this mode
+                    # else:
+                    #     [results.add((prop.str, "http://www.w3.org/2000/01/rdf-schema#range",
+                    #                   str(j))) for j in self.reasoner.data_property_ranges(prop, direct=True)]
+
+                    if not include_all:
+                        [results.add((prop.str, "http://www.w3.org/2000/01/rdf-schema#subPropertyOf",
+                                      j.str)) for j
+                         in getattr(self.reasoner, "super_" + prop_type.lower() + "_properties")(prop, direct=True)]
+                elif mode == 'axiom':
+                    [results.add(getattr(owlapy.owl_axiom, "OWLSub" + prop_type + "PropertyOfAxiom")(j, prop)) for j in
+                     getattr(self.reasoner, "sub_" + prop_type.lower() + "_properties")(prop, direct=True)]
+                    [results.add(getattr(owlapy.owl_axiom, "OWLEquivalent" + prop_type + "PropertiesAxiom")([j, prop]))
+                     for
+                     j in
+                     getattr(self.reasoner, "equivalent_" + prop_type.lower() + "_properties")(prop)]
+                    [results.add(getattr(owlapy.owl_axiom, "OWL" + prop_type + "PropertyDomainAxiom")(prop, j)) for j in
+                     getattr(self.reasoner, prop_type.lower() + "_property_domains")(prop, direct=True)]
+                    [results.add(getattr(owlapy.owl_axiom, "OWL" + prop_type + "PropertyRangeAxiom")(prop, j)) for j in
+                     getattr(self.reasoner, prop_type.lower() + "_property_ranges")(prop, direct=True)]
+                    if not include_all:
+                        [results.add(getattr(owlapy.owl_axiom, "OWLSub" + prop_type + "PropertyOfAxiom")(prop, j)) for j
+                         in getattr(self.reasoner, "super_" + prop_type.lower() + "_properties")(prop, direct=True)]
+
+        return results
+
+    def triples(self, mode="native"):
+        """Get all tbox and abox axioms/triples.
 
         Args:
-            world_store: The file name of the world store. Leave to default value to create a new world.
+            mode (str): The return format.
+              1) 'native' -> returns triples as tuples of owlapy objects,
+              2) 'iri' -> returns triples as tuples of IRIs as string,
+              3) 'axiom' -> triples are represented by owlapy axioms.
+
+        Returns: Iterable of tuples or owlapy axiom, depending on the mode.
         """
-        if world_store is None:
-            self._world = owlready2.World()
+        yield from self.abox(mode=mode)
+        yield from self.tbox(mode=mode)
+
+    def ignore_and_copy(self, ignored_classes: Optional[Iterable[OWLClass]] = None,
+                        ignored_object_properties: Optional[Iterable[OWLObjectProperty]] = None,
+                        ignored_data_properties: Optional[Iterable[OWLDataProperty]] = None) -> 'KnowledgeBase':
+        """Makes a copy of the knowledge base while ignoring specified concepts and properties.
+
+        Args:
+            ignored_classes: Classes to ignore.
+            ignored_object_properties: Object properties to ignore.
+            ignored_data_properties: Data properties to ignore.
+        Returns:
+            A new KnowledgeBase with the hierarchies restricted as requested.
+        """
+
+        new = object.__new__(KnowledgeBase)
+
+        AbstractKnowledgeBase.__init__(new)
+        new.manager = self.manager
+        new.ontology = self.ontology
+        new.reasoner = self.reasoner
+        new.length_metric = self.length_metric
+        new.ind_set = self.ind_set
+        new.path = self.path
+        new.use_individuals_cache = self.use_individuals_cache
+        new.generator = self.generator
+        new.op_domains = self.op_domains
+        new.op_ranges = self.op_ranges
+        new.dp_domains = self.dp_domains
+        new.dp_ranges = self.dp_ranges
+
+        if self.use_individuals_cache:
+            new.ind_cache = LRUCache(maxsize=self.ind_cache.maxsize)
+
+        if ignored_classes is not None:
+            owl_concepts_to_ignore = set()
+            for i in ignored_classes:
+                if self.contains_class(i):
+                    owl_concepts_to_ignore.add(i)
+                else:
+                    raise ValueError(
+                        f'{i} could not found in \n{self} \n'
+                        f'{[_ for _ in self.ontology.classes_in_signature()]}.')
+            if logger.isEnabledFor(logging.INFO):
+                r = DLSyntaxObjectRenderer()
+                logger.info('Concepts to ignore: {0}'.format(' '.join(map(r.render, owl_concepts_to_ignore))))
+            new.class_hierarchy = self.class_hierarchy.restrict_and_copy(remove=owl_concepts_to_ignore)
+        else:
+            new.class_hierarchy = self.class_hierarchy
+
+        if ignored_object_properties is not None:
+            new.object_property_hierarchy = self.object_property_hierarchy.restrict_and_copy(
+                remove=ignored_object_properties)
         else:
-            self._world = owlready2.World(filename=world_store)
+            new.object_property_hierarchy = self.object_property_hierarchy
+
+        if ignored_data_properties is not None:
+            new.data_property_hierarchy = self.data_property_hierarchy.restrict_and_copy(
+                remove=ignored_data_properties)
+        else:
+            new.data_property_hierarchy = self.data_property_hierarchy
+
+        return new
+
+    def concept_len(self, ce: OWLClassExpression) -> int:
+        """Calculates the length of a concept and is used by some concept learning algorithms to
+        find the best results considering also the length of the concepts.
+
+        Args:
+            ce: The concept to be measured.
+        Returns:
+            Length of the concept.
+        """
+        # @TODO: CD: Computing the length of a concept should be disantangled from KB
+        # @TODO: CD: Ideally, this should be a static function
+
+        return self.length_metric.length(ce)
 
-    def create_ontology(self, iri: IRI) -> 'OWLOntology_Owlready2':
-        return OWLOntology_Owlready2(self, iri, load=False)
+    def clean(self):
+        """Clean all stored values (states and caches) if there is any.
 
-    def load_ontology(self, iri: IRI) -> 'OWLOntology_Owlready2':
-        return OWLOntology_Owlready2(self, iri, load=True)
+        Note:
+            1. If you have more than one learning problem that you want to fit to the same model (i.e. to learn the
+            concept using the same concept learner model) use this method to make sure that you have cleared every
+            previous stored value.
+            2. If you store another KnowledgeBase instance using the same variable name as before, it is recommended to
+            use this method before the initialization to avoid data mismatch.
+        """
 
-    def apply_change(self, change: OWLOntologyChange):
-        if isinstance(change, AddImport):
-            ont_x: owlready2.namespace.Ontology = self._world.get_ontology(
-                change.get_ontology().get_ontology_id().get_ontology_iri().as_str())
-            ont_x.imported_ontologies.append(
-                self._world.get_ontology(change.get_import_declaration().str))
+        self.op_domains.clear()
+        if self.use_individuals_cache:
+            self.ind_cache.cache_clear()
+
+    def cache_individuals(self, ce: OWLClassExpression) -> None:
+        if not self.use_individuals_cache:
+            raise TypeError
+        if ce in self.ind_cache:
+            return
+        if isinstance(self.reasoner, FastInstanceCheckerReasoner):
+            self.ind_cache[ce] = self.reasoner._find_instances(ce)  # performance hack
+        else:
+            temp = self.reasoner.instances(ce)
+            self.ind_cache[ce] = frozenset(temp)
+
+    def maybe_cache_individuals(self, ce: OWLClassExpression) -> Iterable[OWLNamedIndividual]:
+        if self.use_individuals_cache:
+            self.cache_individuals(ce)
+            yield from self.ind_cache[ce]
+        else:
+            yield from self.reasoner.instances(ce)
+
+    def maybe_cache_individuals_count(self, ce: OWLClassExpression) -> int:
+        if self.use_individuals_cache:
+            self.cache_individuals(ce)
+            r = self.ind_cache[ce]
+            return len(r)
         else:
-            # TODO XXX
-            raise NotImplementedError
+            return iter_count(self.reasoner.instances(ce))
 
-    def add_axiom(self, ontology: OWLOntology, axiom: OWLAxiom):
-        axioms._add_axiom(axiom, ontology, self._world)
+    def individuals_count(self, concept: Optional[OWLClassExpression] = None) -> int:
+        """Returns the number of all individuals belonging to the concept in the ontology.
 
-    def remove_axiom(self, ontology: OWLOntology, axiom: OWLAxiom):
-        axioms._remove_axiom(axiom, ontology, self._world)
+        Args:
+            concept: Class expression of the individuals to count.
+        Returns:
+            Number of the individuals belonging to the given class.
+        """
 
-    def save_ontology(self, ontology: OWLOntology, document_iri: IRI):
-        ont_x: owlready2.namespace.Ontology = self._world.get_ontology(
-            ontology.get_ontology_id().get_ontology_iri().as_str()
-        )
-        if document_iri.get_namespace().startswith('file:/'):
-            filename = document_iri.as_str()[len('file:/'):]
-            ont_x.save(file=filename)
+        if concept is None or concept.is_owl_thing():
+            return len(self.ind_set)
         else:
-            # TODO XXX
-            raise NotImplementedError
+            return self.maybe_cache_individuals_count(concept)
+
+    @overload
+    def individuals_set(self, concept: OWLClassExpression):
+        ...
+
+    @overload
+    def individuals_set(self, individual: OWLNamedIndividual):
+        ...
+
+    @overload
+    def individuals_set(self, individuals: Iterable[OWLNamedIndividual]):
+        ...
+
+    def individuals_set(self,
+                        arg: Union[Iterable[OWLNamedIndividual], OWLNamedIndividual, OWLClassExpression]) -> FrozenSet:
+        """Retrieve the individuals specified in the arg as a frozenset. If `arg` is an OWLClassExpression then this
+        method behaves as the method "individuals" but will return the final result as a frozenset.
 
-    def save_world(self):
-        """Saves the actual state of the quadstore in the SQLite3 file.
+        Args:
+            arg: more than one individual/ single individual/ class expression of which to list individuals.
+        Returns:
+            Frozenset of the individuals depending on the arg type.
         """
-        self._world.save()
 
+        if isinstance(arg, OWLClassExpression):
+            if self.use_individuals_cache:
+                self.cache_individuals(arg)
+                r = self.ind_cache[arg]
+                return r
+            else:
+                return frozenset(self.individuals(arg))
+        elif isinstance(arg, OWLNamedIndividual):
+            return frozenset({arg})
+        else:
+            return frozenset(arg)
+
+    def all_individuals_set(self):
+        """Retrieve all the individuals of the knowledge base.
 
-class OWLOntology_Owlready2(OWLOntology):
-    __slots__ = '_manager', '_iri', '_world', '_onto'
+        Returns:
+            Frozenset of the all individuals.
+        """
 
-    _manager: OWLOntologyManager_Owlready2
-    _onto: owlready2.Ontology
-    _world: owlready2.World
+        if self.ind_set is not None:
+            return self.ind_set
+        else:
+            return frozenset(self.ontology.individuals_in_signature())
 
-    def __init__(self, manager: OWLOntologyManager_Owlready2, ontology_iri: IRI, load: bool):
-        """Represents an Ontology in Ontolearn.
+    def most_general_object_properties(self, *, domain: OWLClassExpression, inverse: bool = False) \
+            -> Iterable[OWLObjectProperty]:
+        """Find the most general object property.
 
         Args:
-            manager: Ontology manager.
-            ontology_iri: IRI of the ontology.
-            load: Whether to load the ontology or not.
+            domain: Domain for which to search properties.
+            inverse: Inverse order?
         """
-        self._manager = manager
-        self._iri = ontology_iri
-        self._world = manager._world
-        onto = self._world.get_ontology(ontology_iri.as_str())
-        if load:
-            onto = onto.load()
-        self._onto = onto
+        assert isinstance(domain, OWLClassExpression)
+        func: Callable
+        func = self.get_object_property_ranges if inverse else self.get_object_property_domains
+
+        inds_domain = self.individuals_set(domain)
+        for prop in self.object_property_hierarchy.most_general_roles():
+            if domain.is_owl_thing() or inds_domain <= self.individuals_set(func(prop)):
+                yield prop
 
-    def classes_in_signature(self) -> Iterable[OWLClass]:
-        for c in self._onto.classes():
-            yield OWLClass(IRI.create(c.iri))
+    def data_properties_for_domain(self, domain: OWLClassExpression, data_properties: Iterable[OWLDataProperty]) \
+            -> Iterable[OWLDataProperty]:
+        assert isinstance(domain, OWLClassExpression)
 
-    def data_properties_in_signature(self) -> Iterable[OWLDataProperty]:
-        for dp in self._onto.data_properties():
-            yield OWLDataProperty(IRI.create(dp.iri))
+        inds_domain = self.individuals_set(domain)
+        for prop in data_properties:
+            if domain.is_owl_thing() or inds_domain <= self.individuals_set(self.get_data_property_domains(prop)):
+                yield prop
+
+    # in case more types of AbstractLearningProblem are introduced to the project uncomment the method below and use
+    # decorators
+    # @singledispatchmethod
+    # def encode_learning_problem(self, lp: AbstractLearningProblem):
+    #     raise NotImplementedError(lp)
 
-    def object_properties_in_signature(self) -> Iterable[OWLObjectProperty]:
-        for op in self._onto.object_properties():
-            yield OWLObjectProperty(IRI.create(op.iri))
+    def encode_learning_problem(self, lp: PosNegLPStandard):
+        """
+        @TODO: A learning problem (DL concept learning problem) should not be a part of a knowledge base
 
-    def individuals_in_signature(self) -> Iterable[OWLNamedIndividual]:
-        for i in self._onto.individuals():
-            yield OWLNamedIndividual(IRI.create(i.iri))
+        Provides the encoded learning problem (lp), i.e. the class containing the set of OWLNamedIndividuals
+        as follows:
+            kb_pos --> the positive examples set,
+            kb_neg --> the negative examples set,
+            kb_all --> all lp individuals / all individuals set,
+            kb_diff --> kb_all - (kb_pos + kb_neg).
+        Note:
+            Simple access of the learning problem individuals divided in respective sets.
+            You will need the encoded learning problem to use the method evaluate_concept of this class.
+        Args:
+            lp (PosNegLPStandard): The learning problem.
+        Return:
+            EncodedPosNegLPStandard: The encoded learning problem.
+        """
+        if lp.all is None:
+            kb_all = self.all_individuals_set()
+        else:
+            kb_all = self.individuals_set(lp.all)
 
-    def equivalent_classes_axioms(self, c: OWLClass) -> Iterable[OWLEquivalentClassesAxiom]:
-        c_x: owlready2.ThingClass = self._world[c.str]
-        # TODO: Should this also return EquivalentClasses general class axioms? Compare to java owlapi
-        for ec_x in c_x.equivalent_to:
-            yield OWLEquivalentClassesAxiom([c, _parse_concept_to_owlapy(ec_x)])
+        assert 0 < len(lp.pos) < len(kb_all) and len(kb_all) > len(lp.neg)
+        if logger.isEnabledFor(logging.INFO):
+            r = DLSyntaxObjectRenderer()
+            logger.info('E^+:[ {0} ]'.format(', '.join(map(r.render, lp.pos))))
+            logger.info('E^-:[ {0} ]'.format(', '.join(map(r.render, lp.neg))))
+
+        kb_pos = self.individuals_set(lp.pos)
+        if len(lp.neg) == 0:  # if negatives are not provided, randomly sample.
+            kb_neg = type(kb_all)(random.sample(list(kb_all), len(kb_pos)))
+        else:
+            kb_neg = self.individuals_set(lp.neg)
+
+        try:
+            assert len(kb_pos) == len(lp.pos)
+        except AssertionError:
+            print(lp.pos)
+            print(kb_pos)
+            print(kb_all)
+            print('Assertion error. Exiting.')
+            raise
+        if lp.neg:
+            assert len(kb_neg) == len(lp.neg)
+
+        return EncodedPosNegLPStandard(
+            kb_pos=kb_pos,
+            kb_neg=kb_neg,
+            kb_all=kb_all,
+            kb_diff=kb_all.difference(kb_pos.union(kb_neg)))
+
+    def evaluate_concept(self, concept: OWLClassExpression, quality_func: AbstractScorer,
+                         encoded_learning_problem: EncodedLearningProblem) -> EvaluatedConcept:
+        """Evaluates a concept by using the encoded learning problem examples, in terms of Accuracy or F1-score.
+
+        @ TODO: A knowledge base is a data structure and the context of "evaluating" a concept seems to be unrelated
+
+        Note:
+            This method is useful to tell the quality (e.q) of a generated concept by the concept learners, to get
+            the set of individuals (e.inds) that are classified by this concept and the amount of them (e.ic).
+        Args:
+            concept: The concept to be evaluated.
+            quality_func: Quality measurement in terms of Accuracy or F1-score.
+            encoded_learning_problem: The encoded learning problem.
+        Return:
+            The evaluated concept.
+        """
 
-    def general_class_axioms(self) -> Iterable[OWLClassAxiom]:
-        # TODO: At the moment owlready2 only supports SubClassOf general class axioms. (18.02.2023)
-        for ca in self._onto.general_class_axioms():
-            yield from (OWLSubClassOfAxiom(_parse_concept_to_owlapy(ca.left_side), _parse_concept_to_owlapy(c))
-                        for c in ca.is_a)
+        e = EvaluatedConcept()
+        e.inds = self.individuals_set(concept)
+        e.ic = len(e.inds)
+        _, e.q = quality_func.score_elp(e.inds, encoded_learning_problem)
+        return e
 
-    def get_owl_ontology_manager(self) -> OWLOntologyManager_Owlready2:
-        return self._manager
+    def get_leaf_concepts(self, concept: OWLClass):
+        """Get leaf classes.
 
-    def get_ontology_id(self) -> OWLOntologyID:
-        onto_iri = self._world._unabbreviate(self._onto.storid)
-        look_version = self._world._get_obj_triple_sp_o(
-            self._onto.storid,
-            self._world._abbreviate(_VERSION_IRI.as_str()))
-        if look_version is not None:
-            version_iri = self._world._unabbreviate(look_version)
-        else:
-            version_iri = None
+        Args:
+            concept: Atomic class for which to find leaf classes.
 
-        return OWLOntologyID(IRI.create(onto_iri) if onto_iri is not None else None,
-                             IRI.create(version_iri) if version_iri is not None else None)
+        Returns:
+            Leaf classes { x \\| (x subClassOf concept) AND not exist y: y subClassOf x )}. """
+        assert isinstance(concept, OWLClass)
+        yield from self.class_hierarchy.leaves(of=concept)
+
+    def get_least_general_named_concepts(self) -> Generator[OWLClass, None, None]:
+        """Get leaf classes.
+        @TODO: Docstring needed
+        Returns:
+        """
+        yield from self.class_hierarchy.leaves()
 
-    def data_property_domain_axioms(self, pe: OWLDataProperty) -> Iterable[OWLDataPropertyDomainAxiom]:
-        p_x: owlready2.DataPropertyClass = self._world[pe.str]
-        domains = set(p_x.domains_indirect())
-        if len(domains) == 0:
-            yield OWLDataPropertyDomainAxiom(pe, OWLThing)
-        else:
-            for dom in domains:
-                if isinstance(dom, (owlready2.ThingClass, owlready2.ClassConstruct)):
-                    yield OWLDataPropertyDomainAxiom(pe, _parse_concept_to_owlapy(dom))
-                else:
-                    logger.warning("Construct %s not implemented at %s", dom, pe)
-                    pass  # XXX TODO
+    def least_general_named_concepts(self) -> Generator[OWLClass, None, None]:
+        """Get leaf classes.
+        @TODO: Docstring needed
+        Returns:
+        """
+        yield from self.class_hierarchy.leaves()
 
-    def data_property_range_axioms(self, pe: OWLDataProperty) -> Iterable[OWLDataPropertyRangeAxiom]:
-        p_x: owlready2.DataPropertyClass = self._world[pe.str]
-        ranges = set(chain.from_iterable(super_prop.range for super_prop in p_x.ancestors()))
-        if len(ranges) == 0:
-            pass
-            # TODO
-        else:
-            for rng in ranges:
-                if rng in _Datatype_map:
-                    yield OWLDataPropertyRangeAxiom(pe, _Datatype_map[rng])
-                elif isinstance(rng, owlready2.ClassConstruct):
-                    yield OWLDataPropertyRangeAxiom(pe, _parse_datarange_to_owlapy(rng))
-                else:
-                    logger.warning("Datatype %s not implemented at %s", rng, pe)
-                    pass  # XXX TODO
+    def get_most_general_classes(self) -> Generator[OWLClass, None, None]:
+        """Get most general named concepts classes.
+        @TODO: Docstring needed
+        Returns:"""
+        yield from self.class_hierarchy.roots()
 
-    def object_property_domain_axioms(self, pe: OWLObjectProperty) -> Iterable[OWLObjectPropertyDomainAxiom]:
-        p_x: owlready2.ObjectPropertyClass = self._world[pe.str]
-        domains = set(p_x.domains_indirect())
-        if len(domains) == 0:
-            yield OWLObjectPropertyDomainAxiom(pe, OWLThing)
-        else:
-            for dom in domains:
-                if isinstance(dom, (owlready2.ThingClass, owlready2.ClassConstruct)):
-                    yield OWLObjectPropertyDomainAxiom(pe, _parse_concept_to_owlapy(dom))
-                else:
-                    logger.warning("Construct %s not implemented at %s", dom, pe)
-                    pass  # XXX TODO
+    def get_direct_sub_concepts(self, concept: OWLClass) -> Iterable[OWLClass]:
+        """Direct sub-classes of atomic class.
 
-    def object_property_range_axioms(self, pe: OWLObjectProperty) -> Iterable[OWLObjectPropertyRangeAxiom]:
-        p_x: owlready2.ObjectPropertyClass = self._world[pe.str]
-        ranges = set(chain.from_iterable(super_prop.range for super_prop in p_x.ancestors()))
-        if len(ranges) == 0:
-            yield OWLObjectPropertyRangeAxiom(pe, OWLThing)
-        else:
-            for rng in ranges:
-                if isinstance(rng, (owlready2.ThingClass, owlready2.ClassConstruct)):
-                    yield OWLObjectPropertyRangeAxiom(pe, _parse_concept_to_owlapy(rng))
-                else:
-                    logger.warning("Construct %s not implemented at %s", rng, pe)
-                    pass  # XXX TODO
+        Args:
+            concept: Atomic concept.
 
-    def get_original_iri(self):
-        """Get the IRI argument that was used to create this ontology."""
-        return self._iri
-
-    def __eq__(self, other):
-        if type(other) == type(self):
-            return self._onto.loaded == other._onto.loaded and self._onto.base_iri == other._onto.base_iri
-        return NotImplemented
+        Returns:
+            Direct sub classes of concept { x \\| ( x subClassOf concept )}."""
+        assert isinstance(concept, OWLClass)
+        yield from self.class_hierarchy.sub_classes(concept, direct=True)
 
-    def __hash__(self):
-        return hash(self._onto.base_iri)
+    def get_object_property_domains(self, prop: OWLObjectProperty) -> OWLClassExpression:
+        """Get the domains of an object property.
 
-    def __repr__(self):
-        return f'OWLOntology_Owlready2({IRI.create(self._onto.base_iri)}, {self._onto.loaded})'
+        Args:
+            prop: Object property.
 
+        Returns:
+            Domains of the property.
+        """
+        if prop not in self.op_domains:
+            domains = list(self.reasoner.object_property_domains(prop, direct=True))
+            self.op_domains[prop] = self.generator.intersection(domains) if len(domains) > 1 else domains[0]
+        return self.op_domains[prop]
 
-class OWLReasoner_Owlready2(OWLReasonerEx):
-    __slots__ = '_ontology', '_world'
+    def get_object_property_ranges(self, prop: OWLObjectProperty) -> OWLClassExpression:
+        """Get the ranges of an object property.
 
-    _ontology: OWLOntology_Owlready2
-    _world: owlready2.World
+        Args:
+            prop: Object property.
 
-    def __init__(self, ontology: OWLOntology_Owlready2, isolate: bool = False):
-        """
-        Base reasoner in Ontolearn, used to reason in the given ontology.
-
-        Args:
-            ontology: The ontology that should be used by the reasoner.
-            isolate: Whether to isolate the reasoner in a new world + copy of the original ontology.
-                     Useful if you create multiple reasoner instances in the same script.
-        """
-        super().__init__(ontology)
-        assert isinstance(ontology, OWLOntology_Owlready2)
-        self._owl2sparql_converter = Owl2SparqlConverter()
-
-        if isolate:
-            self._isolated = True
-            new_manager = OWLOntologyManager_Owlready2()
-            self._ontology = new_manager.load_ontology(ontology.get_original_iri())
-            self._world = new_manager._world
-            print("INFO  OWLReasoner    :: Using isolated ontology\n"
-                  "INFO  OWLReasoner    :: Changes you make in the original ontology won't be reflected to the isolated"
-                  " ontology\n"
-                  "INFO  OWLReasoner    :: To make changes on the isolated ontology use the method "
-                  "`update_isolated_ontology()`")
-
-        else:
-            self._isolated = False
-            self._ontology = ontology
-            self._world = ontology._world
-
-    def update_isolated_ontology(self, axioms_to_add: List[OWLAxiom] = None,
-                                 axioms_to_remove: List[OWLAxiom] = None):
-        """
-        Add or remove axioms to the isolated ontology that the reasoner is using.
-
-        Args:
-            axioms_to_add (List[OWLAxiom]): Axioms to add to the isolated ontology.
-            axioms_to_remove (List[OWLAxiom]): Axioms to remove from the isolated ontology.
-        """
-        if self._isolated:
-            if axioms_to_add is None and axioms_to_remove is None:
-                raise ValueError(f"At least one argument should be specified in method: "
-                                 f"{self.update_isolated_ontology.__name__}")
-            manager = self._ontology.get_owl_ontology_manager()
-            if axioms_to_add is not None:
-                for axiom in axioms_to_add:
-                    manager.add_axiom(self._ontology, axiom)
-            if axioms_to_remove is not None:
-                for axiom in axioms_to_remove:
-                    manager.remove_axiom(self._ontology, axiom)
-        else:
-            raise AssertionError(f"Misuse of method '{self.update_isolated_ontology.__name__}'. The reasoner is not "
-                                 f"using an isolated ontology.")
-
-    def data_property_domains(self, pe: OWLDataProperty, direct: bool = False) -> Iterable[OWLClassExpression]:
-        domains = {d.get_domain() for d in self.get_root_ontology().data_property_domain_axioms(pe)}
-        super_domains = set(chain.from_iterable([self.super_classes(d) for d in domains]))
-        yield from domains - super_domains
-        if not direct:
-            yield from super_domains
-
-    def object_property_domains(self, pe: OWLObjectProperty, direct: bool = False) -> Iterable[OWLClassExpression]:
-        domains = {d.get_domain() for d in self.get_root_ontology().object_property_domain_axioms(pe)}
-        super_domains = set(chain.from_iterable([self.super_classes(d) for d in domains]))
-        yield from domains - super_domains
-        if not direct:
-            yield from super_domains
-
-    def object_property_ranges(self, pe: OWLObjectProperty, direct: bool = False) -> Iterable[OWLClassExpression]:
-        ranges = {r.get_range() for r in self.get_root_ontology().object_property_range_axioms(pe)}
-        super_ranges = set(chain.from_iterable([self.super_classes(d) for d in ranges]))
-        yield from ranges - super_ranges
-        if not direct:
-            yield from super_ranges
-
-    def equivalent_classes(self, ce: OWLClassExpression, only_named: bool = True) -> Iterable[OWLClassExpression]:
-        seen_set = {ce}
-        if isinstance(ce, OWLClass):
-            c_x: owlready2.ThingClass = self._world[ce.str]
-            for eq_x in c_x.INDIRECT_equivalent_to:
-                eq = _parse_concept_to_owlapy(eq_x)
-                if (isinstance(eq, OWLClass) or
-                    (isinstance(eq, OWLClassExpression) and not only_named)) and eq not in seen_set:
-                    seen_set.add(eq)
-                    yield eq
-                # Workaround for problems in owlready2. It does not always recognize equivalent complex class
-                # expressions through INDIRECT_equivalent_to. Maybe it will work as soon as owlready2 adds support for
-                # EquivalentClasses general class axioms.
-                if not only_named and isinstance(eq_x, owlready2.ThingClass):
-                    for eq_2_x in eq_x.equivalent_to:
-                        eq_2 = _parse_concept_to_owlapy(eq_2_x)
-                        if eq_2 not in seen_set:
-                            seen_set.add(eq_2)
-                            yield eq_2
-        elif isinstance(ce, OWLClassExpression):
-            # Extend as soon as owlready2 supports EquivalentClasses general class axioms
-            # Slow but works. No better way to do this in owlready2 without using the reasoners at the moment.
-            # Might be able to change this when owlready2 supports general class axioms for EquivalentClasses.
-            for c in self._ontology.classes_in_signature():
-                if ce in self.equivalent_classes(c, only_named=False) and c not in seen_set:
-                    seen_set.add(c)
-                    yield c
-                    for e_c in self.equivalent_classes(c, only_named=False):
-                        if e_c not in seen_set and (not only_named or isinstance(e_c, OWLClass)):
-                            seen_set.add(e_c)
-                            yield e_c
-        else:
-            raise ValueError(f'Equivalent classes not implemented for: {ce}')
-
-    def _find_disjoint_classes(self, ce: OWLClassExpression, only_named: bool = True, seen_set=None):
-        if isinstance(ce, OWLClass):
-            c_x: owlready2.ThingClass = self._world[ce.str]
-            for d_x in chain.from_iterable(map(lambda d: d.entities, c_x.disjoints())):
-                if d_x != c_x and (isinstance(d_x, owlready2.ThingClass) or
-                                   (isinstance(d_x, owlready2.ClassConstruct) and not only_named)):
-                    d_owlapy = _parse_concept_to_owlapy(d_x)
-                    seen_set.add(d_owlapy)
-                    yield d_owlapy
-                    for c in self.equivalent_classes(d_owlapy, only_named=only_named):
-                        if c not in seen_set:
-                            seen_set.add(c)
-                            yield c
-                    for c in self.sub_classes(d_owlapy, only_named=only_named):
-                        if c not in seen_set:
-                            seen_set.add(c)
-                            yield c
-        elif isinstance(ce, OWLClassExpression):
-            # Extend as soon as owlready2 supports DisjointClasses general class axioms
-            # Slow but works. No better way to do this in owlready2 without using the reasoners at the moment.
-            # Might be able to change this when owlready2 supports general class axioms for DjsjointClasses
-            yield from (c for c in self._ontology.classes_in_signature() if ce in self.disjoint_classes(c, False))
-        else:
-            raise ValueError(f'Equivalent classes not implemented for: {ce}')
-
-    def disjoint_classes(self, ce: OWLClassExpression, only_named: bool = True) -> Iterable[OWLClassExpression]:
-        seen_set = set()
-        yield from self._find_disjoint_classes(ce, only_named, seen_set)
-        for c in self.super_classes(ce, only_named=only_named):
-            if c != OWLClass(IRI('http://www.w3.org/2002/07/owl#', 'Thing')):
-                yield from self._find_disjoint_classes(c, only_named=only_named, seen_set=seen_set)
-
-    def different_individuals(self, ind: OWLNamedIndividual) -> Iterable[OWLNamedIndividual]:
-        i: owlready2.Thing = self._world[ind.str]
-        yield from (OWLNamedIndividual(IRI.create(d_i.iri))
-                    for d_i in chain.from_iterable(map(lambda x: x.entities, i.differents()))
-                    if isinstance(d_i, owlready2.Thing) and i != d_i)
-
-    def same_individuals(self, ind: OWLNamedIndividual) -> Iterable[OWLNamedIndividual]:
-        i: owlready2.Thing = self._world[ind.str]
-        yield from (OWLNamedIndividual(IRI.create(d_i.iri)) for d_i in i.equivalent_to
-                    if isinstance(d_i, owlready2.Thing))
-
-    def data_property_values(self, ind: OWLNamedIndividual, pe: OWLDataProperty, direct: bool = True) \
-            -> Iterable[OWLLiteral]:
-        i: owlready2.Thing = self._world[ind.str]
-        p: owlready2.DataPropertyClass = self._world[pe.str]
-        retrieval_func = p._get_values_for_individual if direct else p._get_indirect_values_for_individual
-        for val in retrieval_func(i):
-            yield OWLLiteral(val)
-
-    def all_data_property_values(self, pe: OWLDataProperty, direct: bool = True) -> Iterable[OWLLiteral]:
-        p: owlready2.DataPropertyClass = self._world[pe.str]
-        relations = p.get_relations()
-        if not direct:
-            indirect_relations = chain.from_iterable(
-                map(lambda x: self._world[x.str].get_relations(),
-                    self.sub_data_properties(pe, direct=False)))
-            relations = chain(relations, indirect_relations)
-        for _, val in relations:
-            yield OWLLiteral(val)
-
-    def object_property_values(self, ind: OWLNamedIndividual, pe: OWLObjectPropertyExpression, direct: bool = False) \
-            -> Iterable[OWLNamedIndividual]:
-        if isinstance(pe, OWLObjectProperty):
-            i: owlready2.Thing = self._world[ind.str]
-            p: owlready2.ObjectPropertyClass = self._world[pe.str]
-            # Recommended to use direct=False because _get_values_for_individual does not give consistent result
-            # for the case when there are equivalent object properties. At least until this is fixed on owlready2.
-            retieval_func = p._get_values_for_individual if direct else p._get_indirect_values_for_individual
-            for val in retieval_func(i):
-                yield OWLNamedIndividual(IRI.create(val.iri))
-        elif isinstance(pe, OWLObjectInverseOf):
-            p: owlready2.ObjectPropertyClass = self._world[pe.get_named_property().str]
-            inverse_p = p.inverse_property
-            # If the inverse property is explicitly defined we can take shortcut
-            if inverse_p is not None:
-                yield from self.object_property_values(ind, OWLObjectProperty(IRI.create(inverse_p.iri)), direct)
-            else:
-                if not direct:
-                    raise NotImplementedError('Indirect values of inverse properties are only implemented if the '
-                                              'inverse property is explicitly defined in the ontology.'
-                                              f'Property: {pe}')
-                i: owlready2.Thing = self._world[ind.str]
-                for val in p._get_inverse_values_for_individual(i):
-                    yield OWLNamedIndividual(IRI.create(val.iri))
-        else:
-            raise NotImplementedError(pe)
-
-    def flush(self) -> None:
-        pass
-
-    def instances(self, ce: OWLClassExpression, direct: bool = False) -> Iterable[OWLNamedIndividual]:
-        if direct:
-            if isinstance(ce, OWLClass):
-                c_x: owlready2.ThingClass = self._world[ce.str]
-                for i in self._ontology._onto.get_instances_of(c_x):
-                    if isinstance(i, owlready2.Thing):
-                        yield OWLNamedIndividual(IRI.create(i.iri))
-            else:
-                raise NotImplementedError("instances for complex class expressions not implemented", ce)
+        Returns:
+            Ranges of the property.
+        """
+        if prop not in self.op_ranges:
+            ranges = list(self.reasoner.object_property_ranges(prop, direct=True))
+            self.op_ranges[prop] = self.generator.intersection(ranges) if len(ranges) > 1 else ranges[0]
+        return self.op_ranges[prop]
+
+    def get_data_property_domains(self, prop: OWLDataProperty) -> OWLClassExpression:
+        """Get the domains of a data property.
+
+        Args:
+            prop: Data property.
+
+        Returns:
+            Domains of the property.
+        """
+        if prop not in self.dp_domains:
+            domains = list(self.reasoner.data_property_domains(prop, direct=True))
+            self.dp_domains[prop] = self.generator.intersection(domains) if len(domains) > 1 else domains[0]
+        return self.dp_domains[prop]
+
+    def get_data_property_ranges(self, prop: OWLDataProperty) -> FrozenSet[OWLDataRange]:
+        """Get the ranges of a data property.
+
+        Args:
+            prop: Data property.
+
+        Returns:
+            Ranges of the property.
+        """
+        if prop not in self.dp_ranges:
+            self.dp_ranges[prop] = frozenset(self.reasoner.data_property_ranges(prop, direct=True))
+        return self.dp_ranges[prop]
+
+    def most_general_data_properties(self, *, domain: OWLClassExpression) -> Iterable[OWLDataProperty]:
+        """Find most general data properties that are applicable to a domain.
+
+        Args:
+            domain: Domain for which to search properties.
+
+        Returns:
+            Most general data properties for the given domain.
+        """
+        yield from self.data_properties_for_domain(domain, self.get_data_properties())
+
+    def most_general_boolean_data_properties(self, *, domain: OWLClassExpression) -> Iterable[OWLDataProperty]:
+        """Find most general boolean data properties that are applicable to a domain.
+
+        Args:
+            domain: Domain for which to search properties.
+
+        Returns:
+            Most general boolean data properties for the given domain.
+        """
+        yield from self.data_properties_for_domain(domain, self.get_boolean_data_properties())
+
+    def most_general_numeric_data_properties(self, *, domain: OWLClassExpression) -> Iterable[OWLDataProperty]:
+        """Find most general numeric data properties that are applicable to a domain.
+
+        Args:
+            domain: Domain for which to search properties.
+
+        Returns:
+            Most general numeric data properties for the given domain.
+        """
+        yield from self.data_properties_for_domain(domain, self.get_numeric_data_properties())
+
+    def most_general_time_data_properties(self, *, domain: OWLClassExpression) -> Iterable[OWLDataProperty]:
+        """Find most general time data properties that are applicable to a domain.
+
+        Args:
+            domain: Domain for which to search properties.
+
+        Returns:
+            Most general time data properties for the given domain.
+        """
+        yield from self.data_properties_for_domain(domain, self.get_time_data_properties())
+
+    def most_general_existential_restrictions(self, *,
+                                              domain: OWLClassExpression, filler: Optional[OWLClassExpression] = None) \
+            -> Iterable[OWLObjectSomeValuesFrom]:
+        """Find most general existential restrictions that are applicable to a domain.
+
+        Args:
+            domain: Domain for which to search properties.
+            filler: Optional filler to put in the restriction (not normally used).
+
+        Returns:
+           Most general existential restrictions for the given domain.
+        """
+        if filler is None:
+            filler = self.generator.thing
+        assert isinstance(filler, OWLClassExpression)
+
+        for prop in self.most_general_object_properties(domain=domain):
+            yield OWLObjectSomeValuesFrom(property=prop, filler=filler)
+
+    def most_general_universal_restrictions(self, *,
+                                            domain: OWLClassExpression, filler: Optional[OWLClassExpression] = None) \
+            -> Iterable[OWLObjectAllValuesFrom]:
+        """Find most general universal restrictions that are applicable to a domain.
+
+        Args:
+            domain: Domain for which to search properties.
+            filler: Optional filler to put in the restriction (not normally used).
+
+        Returns:
+            Most general universal restrictions for the given domain.
+        """
+        if filler is None:
+            filler = self.generator.thing
+        assert isinstance(filler, OWLClassExpression)
+
+        for prop in self.most_general_object_properties(domain=domain):
+            yield OWLObjectAllValuesFrom(property=prop, filler=filler)
+
+    def most_general_existential_restrictions_inverse(self, *,
+                                                      domain: OWLClassExpression,
+                                                      filler: Optional[OWLClassExpression] = None) \
+            -> Iterable[OWLObjectSomeValuesFrom]:
+        """Find most general inverse existential restrictions that are applicable to a domain.
+
+        Args:
+            domain: Domain for which to search properties.
+            filler: Optional filler to put in the restriction (not normally used).
+
+        Returns:
+            Most general existential restrictions over inverse property.
+        """
+        if filler is None:
+            filler = self.generator.thing
+        assert isinstance(filler, OWLClassExpression)
+
+        for prop in self.most_general_object_properties(domain=domain, inverse=True):
+            yield OWLObjectSomeValuesFrom(property=prop.get_inverse_property(), filler=filler)
+
+    def most_general_universal_restrictions_inverse(self, *,
+                                                    domain: OWLClassExpression,
+                                                    filler: Optional[OWLClassExpression] = None) \
+            -> Iterable[OWLObjectAllValuesFrom]:
+        """Find most general inverse universal restrictions that are applicable to a domain.
+
+        Args:
+            domain: Domain for which to search properties.
+            filler: Optional filler to put in the restriction (not normally used).
+
+        Returns:
+            Most general universal restrictions over inverse property.
+        """
+        if filler is None:
+            filler = self.generator.thing
+        assert isinstance(filler, OWLClassExpression)
+
+        for prop in self.most_general_object_properties(domain=domain, inverse=True):
+            yield OWLObjectAllValuesFrom(property=prop.get_inverse_property(), filler=filler)
+
+    def get_direct_parents(self, concept: OWLClassExpression) -> Iterable[OWLClass]:
+        """Direct parent concepts.
+
+        Args:
+            concept: Concept to find super concepts of.
+
+        Returns:
+            Direct parent concepts.
+        """
+        assert isinstance(concept, OWLClass)
+        yield from self.class_hierarchy.super_classes(concept, direct=True)
+
+    def get_all_direct_sub_concepts(self, concept: OWLClassExpression) -> Iterable[OWLClassExpression]:
+        """All direct sub concepts of a concept.
+
+        Args:
+            concept: Parent concept for which to get sub concepts.
+
+        Returns:
+            Direct sub concepts.
+        """
+        assert isinstance(concept, OWLClass)
+        yield from self.class_hierarchy.sub_classes(concept, direct=True)
+
+    def get_all_sub_concepts(self, concept: OWLClassExpression) -> Iterable[OWLClassExpression]:
+        """All sub concepts of a concept.
+
+        Args:
+            concept: Parent concept for which to get sub concepts.
+
+        Returns:
+            Sub concepts.
+        """
+        assert isinstance(concept, OWLClass)
+        yield from self.class_hierarchy.sub_classes(concept, direct=False)
+
+    def get_concepts(self) -> Iterable[OWLClass]:
+        """Get all concepts of this concept generator.
+
+        Returns:
+            Concepts.
+        """
+        yield from self.class_hierarchy.items()
+
+    def get_classes_in_signature(self):
+        return self.get_concepts()
+
+    @property
+    def concepts(self) -> Iterable[OWLClass]:
+        """Get all concepts of this concept generator.
+
+        Returns:
+            Concepts.
+        """
+        yield from self.class_hierarchy.items()
+
+    @property
+    def object_properties(self) -> Iterable[OWLObjectProperty]:
+        """Get all object properties of this concept generator.
+
+        Returns:
+            Object properties.
+        """
+
+        yield from self.object_property_hierarchy.items()
+
+    @property
+    def data_properties(self) -> Iterable[OWLDataProperty]:
+        """Get all data properties of this concept generator.
+
+        Returns:
+            Data properties for the given range.
+        """
+        yield from self.data_property_hierarchy.items()
+
+    def get_object_properties(self) -> Iterable[OWLObjectProperty]:
+        """Get all object properties of this concept generator.
+
+        Returns:
+            Object properties.
+        """
+
+        yield from self.object_property_hierarchy.items()
+
+    def get_data_properties(self, ranges: Set[OWLDatatype] = None) -> Iterable[OWLDataProperty]:
+        """Get all data properties of this concept generator for the given ranges.
+
+        Args:
+           ranges: Ranges for which to extract the data properties.
+
+        Returns:
+            Data properties for the given range.
+        """
+        if ranges is not None:
+            for dp in self.data_property_hierarchy.items():
+                if self.get_data_property_ranges(dp) & ranges:
+                    yield dp
         else:
-            if ce.is_owl_thing():
-                yield from self._ontology.individuals_in_signature()
-            elif isinstance(ce, OWLClass):
-                c_x: owlready2.ThingClass = self._world[ce.str]
-                for i in c_x.instances(world=self._world):
-                    if isinstance(i, owlready2.Thing):
-                        yield OWLNamedIndividual(IRI.create(i.iri))
-            # elif isinstance(ce, OWLObjectSomeValuesFrom) and ce.get_filler().is_owl_thing()\
-            #         and isinstance(ce.get_property(), OWLProperty):
-            #     seen_set = set()
-            #     p_x: owlready2.ObjectProperty = self._world[ce.get_property().get_named_property().str]
-            #     for i, _ in p_x.get_relations():
-            #         if isinstance(i, owlready2.Thing) and i not in seen_set:
-            #             seen_set.add(i)
-            #             yield OWLNamedIndividual(IRI.create(i.iri))
-            else:
-                raise NotImplementedError("instances for complex class expressions not implemented", ce)
+            yield from self.data_property_hierarchy.items()
 
-    def _sub_classes_recursive(self, ce: OWLClassExpression, seen_set: Set, only_named: bool = True) \
-            -> Iterable[OWLClassExpression]:
+    def get_boolean_data_properties(self) -> Iterable[OWLDataProperty]:
+        """Get all boolean data properties of this concept generator.
 
-        # work around issue in class equivalence detection in Owlready2
-        for c in [ce, *self.equivalent_classes(ce, only_named=False)]:
-            if c not in seen_set:
-                seen_set.add(c)
-                yield c
-            # First go through all general class axioms, they should only have complex classes as sub_classes.
-            # Done for OWLClass and OWLClassExpression.
-            for axiom in self._ontology.general_class_axioms():
-                if (isinstance(axiom, OWLSubClassOfAxiom) and axiom.get_super_class() == c
-                        and axiom.get_sub_class() not in seen_set):
-                    seen_set.add(axiom.get_sub_class())
-                    if not only_named:
-                        yield axiom.get_sub_class()
-                    yield from self._sub_classes_recursive(axiom.get_sub_class(), seen_set, only_named)
-
-            if isinstance(c, OWLClass):
-                c_x: owlready2.EntityClass = self._world[c.str]
-                # Subclasses will only return named classes
-                for sc_x in c_x.subclasses(world=self._world):
-                    sc = _parse_concept_to_owlapy(sc_x)
-                    if isinstance(sc, OWLClass) and sc not in seen_set:
-                        seen_set.add(sc)
-                        yield sc
-                        yield from self._sub_classes_recursive(sc, seen_set, only_named=only_named)
-            elif isinstance(c, OWLClassExpression):
-                # Slow but works. No better way to do this in owlready2 without using the reasoners at the moment.
-                for atomic_c in self._ontology.classes_in_signature():
-                    if c in self.super_classes(atomic_c, direct=True, only_named=False) and atomic_c not in seen_set:
-                        seen_set.add(atomic_c)
-                        yield atomic_c
-                        yield from self._sub_classes_recursive(atomic_c, seen_set, only_named=only_named)
-                if isinstance(ce, OWLObjectSomeValuesFrom):
-                    for r in self.sub_object_properties(ce.get_property()):
-                        osvf = OWLObjectSomeValuesFrom(property=r,
-                                                       filler=ce.get_filler())
-                        if osvf not in seen_set:
-                            seen_set.add(osvf)
-                            yield osvf
-                            # yield from self._sub_classes_recursive(osvf, seen_set, only_named=only_named)
-            else:
-                raise ValueError(f'Sub classes retrieval not implemented for: {ce}')
+        Returns:
+            Boolean data properties.
+        """
+        yield from self.get_data_properties({BooleanOWLDatatype})
 
-    def sub_classes(self, ce: OWLClassExpression, direct: bool = False, only_named: bool = True) \
-            -> Iterable[OWLClassExpression]:
-        if not direct:
-            seen_set = {ce}
-            yield from self._sub_classes_recursive(ce, seen_set, only_named=only_named)
-        else:
-            # First go through all general class axioms, they should only have complex classes as sub_classes.
-            # Done for OWLClass and OWLClassExpression.
-            if not only_named:
-                for axiom in self._ontology.general_class_axioms():
-                    if isinstance(axiom, OWLSubClassOfAxiom) and axiom.get_super_class() == ce:
-                        yield axiom.get_sub_class()
-            if isinstance(ce, OWLClass):
-                c_x: owlready2.ThingClass = self._world[ce.str]
-                # Subclasses will only return named classes
-                for sc in c_x.subclasses(world=self._world):
-                    if isinstance(sc, owlready2.ThingClass):
-                        yield OWLClass(IRI.create(sc.iri))
-            elif isinstance(ce, OWLClassExpression):
-                # Slow but works. No better way to do this in owlready2 without using the reasoners at the moment.
-                for c in self._ontology.classes_in_signature():
-                    if ce in self.super_classes(c, direct=True, only_named=False):
-                        yield c
-            else:
-                raise ValueError(f'Sub classes retrieval not implemented for: {ce}')
+    def get_numeric_data_properties(self) -> Iterable[OWLDataProperty]:
+        """Get all numeric data properties of this concept generator.
 
-    def _super_classes_recursive(self, ce: OWLClassExpression, seen_set: Set, only_named: bool = True) \
-            -> Iterable[OWLClassExpression]:
-        # work around issue in class equivalence detection in Owlready2
-        for c in [ce, *self.equivalent_classes(ce, only_named=False)]:
-            if c not in seen_set:
-                seen_set.add(c)
-                yield c
-            if isinstance(c, OWLClass):
-                c_x: owlready2.EntityClass = self._world[c.str]
-                for sc_x in c_x.is_a:
-                    sc = _parse_concept_to_owlapy(sc_x)
-                    if (isinstance(sc, OWLClass) or isinstance(sc, OWLClassExpression)) and sc not in seen_set:
-                        seen_set.add(sc)
-                        # Return class expression if it is a named class or complex class expressions should be
-                        # included
-                        if isinstance(sc, OWLClass) or not only_named:
-                            yield sc
-                        yield from self._super_classes_recursive(sc, seen_set, only_named=only_named)
-            elif isinstance(c, OWLClassExpression):
-                for axiom in self._ontology.general_class_axioms():
-                    if (isinstance(axiom, OWLSubClassOfAxiom) and axiom.get_sub_class() == c
-                            and (axiom.get_super_class() not in seen_set)):
-                        super_class = axiom.get_super_class()
-                        seen_set.add(super_class)
-                        # Return class expression if it is a named class or complex class expressions should be
-                        # included
-                        if isinstance(super_class, OWLClass) or not only_named:
-                            yield super_class
-                        yield from self._super_classes_recursive(super_class, seen_set, only_named=only_named)
-
-                # Slow but works. No better way to do this in owlready2 without using the reasoners at the moment.
-                for atomic_c in self._ontology.classes_in_signature():
-                    if c in self.sub_classes(atomic_c, direct=True, only_named=False) and atomic_c not in seen_set:
-                        seen_set.add(atomic_c)
-                        yield atomic_c
-                        yield from self._super_classes_recursive(atomic_c, seen_set, only_named=only_named)
-            else:
-                raise ValueError(f'Super classes retrieval not supported for: {ce}')
+        Returns:
+            Numeric data properties.
+        """
+        yield from self.get_data_properties(NUMERIC_DATATYPES)
 
-    def super_classes(self, ce: OWLClassExpression, direct: bool = False, only_named: bool = True) \
-            -> Iterable[OWLClassExpression]:
-        if not direct:
-            seen_set = {ce}
-            yield from self._super_classes_recursive(ce, seen_set, only_named=only_named)
-        else:
-            if isinstance(ce, OWLClass):
-                c_x: owlready2.ThingClass = self._world[ce.str]
-                for sc in c_x.is_a:
-                    if (isinstance(sc, owlready2.ThingClass) or
-                            (not only_named and isinstance(sc, owlready2.ClassConstruct))):
-                        yield _parse_concept_to_owlapy(sc)
-            elif isinstance(ce, OWLClassExpression):
-                seen_set = set()
-                for axiom in self._ontology.general_class_axioms():
-                    if (isinstance(axiom, OWLSubClassOfAxiom) and axiom.get_sub_class() == ce
-                            and (not only_named or isinstance(axiom.get_super_class(), OWLClass))):
-                        seen_set.add(axiom.get_super_class())
-                        yield axiom.get_super_class()
-                # Slow but works. No better way to do this in owlready2 without using the reasoners at the moment.
-                # TODO: Might not be needed, in theory the general class axioms above should cover all classes
-                # that can be found here
-                for c in self._ontology.classes_in_signature():
-                    if ce in self.sub_classes(c, direct=True, only_named=False) and c not in seen_set:
-                        seen_set.add(c)
-                        yield c
-            else:
-                raise ValueError(f'Super classes retrieval not supported for {ce}')
+    def get_double_data_properties(self) -> Iterable[OWLDataProperty]:
+        """Get all numeric data properties of this concept generator.
 
-    def equivalent_object_properties(self, op: OWLObjectPropertyExpression) -> Iterable[OWLObjectPropertyExpression]:
-        if isinstance(op, OWLObjectProperty):
-            p_x: owlready2.ObjectPropertyClass = self._world[op.str]
-            yield from (OWLObjectProperty(IRI.create(ep_x.iri)) for ep_x in p_x.INDIRECT_equivalent_to
-                        if isinstance(ep_x, owlready2.ObjectPropertyClass))
-        else:
-            raise NotImplementedError("equivalent properties of inverse properties not yet implemented", op)
-
-    def equivalent_data_properties(self, dp: OWLDataProperty) -> Iterable[OWLDataProperty]:
-        p_x: owlready2.DataPropertyClass = self._world[dp.str]
-        yield from (OWLDataProperty(IRI.create(ep_x.iri)) for ep_x in p_x.INDIRECT_equivalent_to
-                    if isinstance(ep_x, owlready2.DataPropertyClass))
-
-    def _find_disjoint_object_properties(self, op: OWLObjectPropertyExpression, seen_set=None) \
-            -> Iterable[OWLObjectPropertyExpression]:
-        if isinstance(op, OWLObjectProperty):
-            p_x: owlready2.ObjectPropertyClass = self._world[op.str]
-            ont_x: owlready2.Ontology = self.get_root_ontology()._onto
-            for disjoint in ont_x.disjoint_properties():
-                if p_x in disjoint.entities:
-                    for o_p in disjoint.entities:
-                        if isinstance(o_p, owlready2.ObjectPropertyClass) and o_p != p_x:
-                            op_owlapy = OWLObjectProperty(IRI.create(o_p.iri))
-                            seen_set.add(op_owlapy)
-                            yield op_owlapy
-                            for o in self.equivalent_object_properties(op_owlapy):
-                                if o not in seen_set:
-                                    seen_set.add(o)
-                                    yield o
-                            for o in self.sub_object_properties(op_owlapy):
-                                if o not in seen_set:
-                                    seen_set.add(o)
-                                    yield o
-        else:
-            raise NotImplementedError("disjoint object properties of inverse properties not yet implemented", op)
-
-    def disjoint_object_properties(self, op: OWLObjectPropertyExpression) -> Iterable[OWLObjectPropertyExpression]:
-        seen_set = set()
-        yield from self._find_disjoint_object_properties(op, seen_set)
-        for o in self.super_object_properties(op):
-            if o != OWLObjectProperty(IRI('http://www.w3.org/2002/07/owl#', 'ObjectProperty')):
-                yield from self._find_disjoint_object_properties(o, seen_set=seen_set)
-
-    def _find_disjoint_data_properties(self, dp: OWLDataProperty, seen_set=None) -> Iterable[OWLDataProperty]:
-        p_x: owlready2.DataPropertyClass = self._world[dp.str]
-        ont_x: owlready2.Ontology = self.get_root_ontology()._onto
-        for disjoint in ont_x.disjoint_properties():
-            if p_x in disjoint.entities:
-                for d_p in disjoint.entities:
-                    if isinstance(d_p, owlready2.DataPropertyClass) and d_p != p_x:
-                        dp_owlapy = OWLDataProperty(IRI.create(d_p.iri))
-                        seen_set.add(dp_owlapy)
-                        yield dp_owlapy
-                        for d in self.equivalent_data_properties(dp_owlapy):
-                            if d not in seen_set:
-                                seen_set.add(d)
-                                yield d
-                        for d in self.sub_data_properties(dp_owlapy):
-                            if d not in seen_set:
-                                seen_set.add(d)
-                                yield d
-
-    def disjoint_data_properties(self, dp: OWLDataProperty) -> Iterable[OWLDataProperty]:
-        seen_set = set()
-        yield from self._find_disjoint_data_properties(dp, seen_set)
-        for d in self.super_data_properties(dp):
-            if d != OWLDataProperty(IRI('http://www.w3.org/2002/07/owl#', 'DatatypeProperty')):
-                yield from self._find_disjoint_data_properties(d, seen_set=seen_set)
+        Returns:
+            Numeric data properties.
+        """
+        yield from self.get_data_properties(DoubleOWLDatatype)
 
-    def _sup_or_sub_data_properties_recursive(self, dp: OWLDataProperty, seen_set: Set, super_or_sub="") \
-            -> Iterable[OWLDataProperty]:
-        for d in self.equivalent_data_properties(dp):
-            if d not in seen_set:
-                seen_set.add(d)
-                yield d
-        p_x: owlready2.DataPropertyClass = self._world[dp.str]
-        assert isinstance(p_x, owlready2.DataPropertyClass)
-        if super_or_sub == "super":
-            dps = set(p_x.is_a)
-        else:
-            dps = set(p_x.subclasses(world=self._world))
-        for sp_x in dps:
-            if isinstance(sp_x, owlready2.DataPropertyClass):
-                sp = OWLDataProperty(IRI.create(sp_x.iri))
-                if sp not in seen_set:
-                    seen_set.add(sp)
-                    yield sp
-                    yield from self._sup_or_sub_data_properties_recursive(sp, seen_set, super_or_sub)
-
-    def _sup_or_sub_data_properties(self, dp: OWLDataProperty, direct: bool = False, super_or_sub=""):
-        assert isinstance(dp, OWLDataProperty)
-        if direct:
-            p_x: owlready2.DataPropertyClass = self._world[dp.str]
-            if super_or_sub == "super":
-                dps = set(p_x.is_a)
-            else:
-                dps = set(p_x.subclasses(world=self._world))
-            for sp in dps:
-                if isinstance(sp, owlready2.DataPropertyClass):
-                    yield OWLDataProperty(IRI.create(sp.iri))
-        else:
-            seen_set = set()
-            yield from self._sup_or_sub_data_properties_recursive(dp, seen_set, super_or_sub)
-
-    def super_data_properties(self, dp: OWLDataProperty, direct: bool = False) -> Iterable[OWLDataProperty]:
-        """Gets the stream of data properties that are the strict (potentially direct) super properties of the
-         specified data property with respect to the imports closure of the root ontology.
+    def get_time_data_properties(self) -> Iterable[OWLDataProperty]:
+        """Get all time data properties of this concept generator.
 
-         Args:
-             dp (OWLDataProperty): The data property whose super properties are to be retrieved.
-             direct (bool): Specifies if the direct super properties should be retrieved (True) or if the all
-                            super properties (ancestors) should be retrieved (False).
-
-         Returns:
-             Iterable of super properties.
-         """
-        yield from self._sup_or_sub_data_properties(dp, direct, "super")
-
-    def sub_data_properties(self, dp: OWLDataProperty, direct: bool = False) -> Iterable[OWLDataProperty]:
-        yield from self._sup_or_sub_data_properties(dp, direct, "sub")
-
-    def _sup_or_sub_object_properties_recursive(self, op: OWLObjectProperty, seen_set: Set, super_or_sub=""):
-        for o in self.equivalent_object_properties(op):
-            if o not in seen_set:
-                seen_set.add(o)
-                yield o
-        p_x: owlready2.ObjectPropertyClass = self._world[op.str]
-        assert isinstance(p_x, owlready2.ObjectPropertyClass)
-        if super_or_sub == "super":
-            dps = set(p_x.is_a)
-        else:
-            dps = set(p_x.subclasses(world=self._world))
-        for sp_x in dps:
-            if isinstance(sp_x, owlready2.ObjectPropertyClass):
-                sp = OWLObjectProperty(IRI.create(sp_x.iri))
-                if sp not in seen_set:
-                    seen_set.add(sp)
-                    yield sp
-                    yield from self._sup_or_sub_object_properties_recursive(sp, seen_set, super_or_sub)
-
-    def _sup_or_sub_object_properties(self, op: OWLObjectPropertyExpression, direct: bool = False, super_or_sub="") \
-            -> Iterable[OWLObjectPropertyExpression]:
-        if isinstance(op, OWLObjectProperty):
-            if direct:
-                p_x: owlready2.ObjectPropertyClass = self._world[op.str]
-                if super_or_sub == "super":
-                    dps = set(p_x.is_a)
-                else:
-                    dps = set(p_x.subclasses(world=self._world))
-                for sp in dps:
-                    if isinstance(sp, owlready2.ObjectPropertyClass):
-                        yield OWLObjectProperty(IRI.create(sp.iri))
-            else:
-                seen_set = set()
-                yield from self._sup_or_sub_object_properties_recursive(op, seen_set, super_or_sub)
-        elif isinstance(op, OWLObjectInverseOf):
-            p: owlready2.ObjectPropertyClass = self._world[op.get_named_property().str]
-            inverse_p = p.inverse_property
-            if inverse_p is not None:
-                yield from self._sup_or_sub_object_properties(OWLObjectProperty(IRI.create(inverse_p.iri)), direct,
-                                                              super_or_sub)
-            else:
-                raise NotImplementedError(f'{super_or_sub} properties of inverse properties are only implemented if the'
-                                          ' inverse property is explicitly defined in the ontology. '
-                                          f'Property: {op}')
-        else:
-            raise NotImplementedError(op)
-
-    def super_object_properties(self, op: OWLObjectPropertyExpression, direct: bool = False) \
-            -> Iterable[OWLObjectPropertyExpression]:
-        """Gets the stream of object properties that are the strict (potentially direct) super properties of the
-         specified object property with respect to the imports closure of the root ontology.
+        Returns:
+            Time data properties.
+        """
+        yield from self.get_data_properties(TIME_DATATYPES)
 
-         Args:
-             op (OWLObjectPropertyExpression): The object property expression whose super properties are to be
-                                                retrieved.
-             direct (bool): Specifies if the direct super properties should be retrieved (True) or if the all
-                            super properties (ancestors) should be retrieved (False).
-
-         Returns:
-             Iterable of super properties.
-         """
-        yield from self._sup_or_sub_object_properties(op, direct, "super")
-
-    def sub_object_properties(self, op: OWLObjectPropertyExpression, direct: bool = False) \
-            -> Iterable[OWLObjectPropertyExpression]:
-        yield from self._sup_or_sub_object_properties(op, direct, "sub")
-
-    def types(self, ind: OWLNamedIndividual, direct: bool = False) -> Iterable[OWLClass]:
-        i: owlready2.Thing = self._world[ind.str]
-        if direct:
-            for c in i.is_a:
-                if isinstance(c, owlready2.ThingClass):
-                    yield OWLClass(IRI.create(c.iri))
-                # Anonymous classes are ignored
-        else:
-            for c in i.INDIRECT_is_a:
-                if isinstance(c, owlready2.ThingClass):
-                    yield OWLClass(IRI.create(c.iri))
-                # Anonymous classes are ignored
-
-    def _sync_reasoner(self, other_reasoner: BaseReasoner_Owlready2 = None,
-                       infer_property_values: bool = True,
-                       infer_data_property_values: bool = True, debug: bool = False) -> None:
-        """Call Owlready2's sync_reasoner method, which spawns a Java process on a temp file to infer more.
-
-        Args:
-            other_reasoner: Set to BaseReasoner.PELLET (default) or BaseReasoner.HERMIT.
-            infer_property_values: Whether to infer property values.
-            infer_data_property_values: Whether to infer data property values (only for PELLET).
-        """
-        assert other_reasoner is None or isinstance(other_reasoner, BaseReasoner_Owlready2)
-        with self.get_root_ontology()._onto:
-            if other_reasoner == BaseReasoner_Owlready2.HERMIT:
-                owlready2.sync_reasoner_hermit(self._world, infer_property_values=infer_property_values, debug=debug)
-            else:
-                owlready2.sync_reasoner_pellet(self._world,
-                                               infer_property_values=infer_property_values,
-                                               infer_data_property_values=infer_data_property_values,
-                                               debug=debug)
-
-    def get_root_ontology(self) -> OWLOntology:
-        return self._ontology
-
-    def is_isolated(self):
-        """Return True if this reasoner is using an isolated ontology."""
-        return self._isolated
-
-    def is_using_triplestore(self):
-        # TODO: Deprecated! Remove after it is removed from OWLReasoner in owlapy
-        pass
+    def get_types(self, ind: OWLNamedIndividual, direct: bool = False) -> Iterable[OWLClass]:
+        """Get the named classes which are (direct) types of the specified individual.
+
+        Args:
+            ind: Individual.
+            direct: Whether to consider direct types.
+
+        Returns:
+            Types of the given individual.
+        """
+        all_types = set(self.get_concepts())
+        for type_ in self.reasoner.types(ind, direct):
+            if type_ in all_types or type_ == OWLThing:
+                yield type_
+
+    def get_object_properties_for_ind(self, ind: OWLNamedIndividual, direct: bool = True) \
+            -> Iterable[OWLObjectProperty]:
+        """Get the object properties for the given individual.
+
+        Args:
+            ind: Individual
+            direct: Whether only direct properties should be considered (True), or if also
+                    indirect properties should be considered (False). Indirect properties
+                    would be super properties super_p of properties p with ObjectPropertyAssertion(p ind obj).
+
+        Returns:
+            Object properties.
+        """
+        properties = set(self.get_object_properties())
+        yield from (pe for pe in self.reasoner.ind_object_properties(ind, direct) if pe in properties)
+
+    def get_data_properties_for_ind(self, ind: OWLNamedIndividual, direct: bool = True) -> Iterable[OWLDataProperty]:
+        """Get the data properties for the given individual
+
+        Args:
+            ind: Individual
+            direct: Whether only direct properties should be considered (True), or if also
+                    indirect properties should be considered (False). Indirect properties
+                    would be super properties super_p of properties p with ObjectPropertyAssertion(p ind obj).
+
+        Returns:
+            Data properties.
+        """
+        properties = set(self.get_data_properties())
+        yield from (pe for pe in self.reasoner.ind_data_properties(ind, direct) if pe in properties)
+
+    def get_object_property_values(self, ind: OWLNamedIndividual,
+                                   property_: OWLObjectPropertyExpression,
+                                   direct: bool = True) -> Iterable[OWLNamedIndividual]:
+        """Get the object property values for the given individual and property.
+
+        Args:
+            ind: Individual.
+            property_: Object property.
+            direct: Whether only the property property_ should be considered (True), or if also
+                    the values of sub properties of property_ should be considered (False).
+
+        Returns:
+            Individuals.
+        """
+        yield from self.reasoner.object_property_values(ind, property_, direct)
+
+    def get_data_property_values(self, ind: OWLNamedIndividual,
+                                 property_: OWLDataPropertyExpression,
+                                 direct: bool = True) -> Iterable[OWLLiteral]:
+        """Get the data property values for the given individual and property.
+
+        Args:
+            ind: Individual.
+            property_: Data property.
+            direct: Whether only the property property_ should be considered (True), or if also
+                    the values of sub properties of property_ should be considered (False).
+
+        Returns:
+            Literals.
+        """
+        yield from self.reasoner.data_property_values(ind, property_, direct)
+
+    def contains_class(self, concept: OWLClassExpression) -> bool:
+        """Check if an atomic class is contained within this concept generator.
+
+        Args:
+            concept: Atomic class.
+
+        Returns:
+            Whether the class is contained in the concept generator.
+        """
+        assert isinstance(concept, OWLClass)
+        return concept in self.class_hierarchy
+
+    def __repr__(self):
+        properties_count = iter_count(self.ontology.object_properties_in_signature()) + iter_count(
+            self.ontology.data_properties_in_signature())
+        class_count = iter_count(self.ontology.classes_in_signature())
+        individuals_count = self.individuals_count()
+
+        return f'KnowledgeBase(path={repr(self.path)} <{class_count} classes, {properties_count} properties, ' \
+               f'{individuals_count} individuals)'
```

### Comparing `ontosample-0.2.3/ontolearn_light/concept_generator.py` & `ontosample-0.2.4/ontolearn_light/concept_generator.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/ontolearn_light/data_struct.py` & `ontosample-0.2.4/ontolearn_light/data_struct.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/ontolearn_light/fitness_functions.py` & `ontosample-0.2.4/ontolearn_light/fitness_functions.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/ontolearn_light/learning_problem.py` & `ontosample-0.2.4/ontolearn_light/learning_problem.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/ontolearn_light/metrics.py` & `ontosample-0.2.4/ontolearn_light/metrics.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/ontolearn_light/search.py` & `ontosample-0.2.4/ontolearn_light/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 from abc import abstractmethod, ABCMeta
 from functools import total_ordering
 from queue import PriorityQueue
 from typing import List, Optional, ClassVar, Final, Iterable, TypeVar, Generic, Set, Tuple, Dict
 from owlapy.owl_object import OWLObjectRenderer
 from owlapy.class_expression import OWLClassExpression
 from owlapy.render import DLSyntaxObjectRenderer
-from owlapy.util import as_index, OrderedOWLObject
+from owlapy.utils import as_index, OrderedOWLObject
 from .abstracts import AbstractNode, AbstractHeuristic, AbstractScorer, AbstractOEHeuristicNode, LBLSearchTree, \
     AbstractConceptNode, EncodedLearningProblem, DRILLAbstractTree
+from owlapy import owl_expression_to_dl
 
 _N = TypeVar('_N')  #:
 
-from owlapy import owl_expression_to_dl
-
 
 # Due to a bug in Python, we cannot use the slots like we should be able to. Hence, the attribute access is also
 # invalid but there is nothing we can do. See https://mail.python.org/pipermail/python-list/2002-December/126637.html
 
 # noinspection PyUnresolvedReferences
 # noinspection PyDunderSlots
 class _NodeConcept(metaclass=ABCMeta):
```

### Comparing `ontosample-0.2.3/ontolearn_light/utils/__init__.py` & `ontosample-0.2.4/ontolearn_light/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/ontolearn_light/utils/log_config.py` & `ontosample-0.2.4/ontolearn_light/utils/log_config.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/ontolearn_light/utils/static_funcs.py` & `ontosample-0.2.4/ontolearn_light/utils/static_funcs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from itertools import chain
-from typing import Optional, Callable, Tuple, Generator, List, Union
-import pandas
-import matplotlib.pyplot as plt
-import numpy as np
+from typing import Optional, Callable, Tuple, Generator, List, Union, Final
 from owlapy.class_expression import OWLClass, OWLClassExpression
 from owlapy.iri import IRI
 from owlapy.owl_axiom import OWLEquivalentClassesAxiom
 from owlapy.owl_ontology import OWLOntology
 from owlapy.owl_ontology_manager import OWLOntologyManager
-from ..base.owl.hierarchy import ClassHierarchy, ObjectPropertyHierarchy, DatatypePropertyHierarchy
-from ..base.owl.utils import OWLClassExpressionLengthMetric
-from owlapy.util import LRUCache
+from owlapy.owl_hierarchy import ClassHierarchy, ObjectPropertyHierarchy, DatatypePropertyHierarchy
+from owlapy.utils import OWLClassExpressionLengthMetric, LRUCache
 import traceback
 
 
 def init_length_metric(length_metric: Optional[OWLClassExpressionLengthMetric] = None,
                        length_metric_factory: Optional[Callable[[], OWLClassExpressionLengthMetric]] = None):
     """ Initialize the technique on computing length of a concept"""
     if length_metric is not None:
@@ -103,41 +99,28 @@
 
     if precision == 0 or recall == 0:
         return 0.0
 
     f_1 = 2 * ((precision * recall) / (precision + recall))
     return f_1
 
-
-def plot_umap_reduced_embeddings(X: pandas.DataFrame, y: List[float], name: str = "umap_visualization.pdf") -> None:
-    import umap
-    reducer = umap.UMAP(random_state=1)
-    embedding = reducer.fit_transform(X)
-    plt.scatter(embedding[:, 0], embedding[:, 1],
-                c=["r" if x == 1 else "b" for x in y])
-    plt.grid()
-    plt.gca().set_aspect('equal', 'datalim')
-    plt.savefig(name)
-    plt.show()
-
-
 def save_owl_class_expressions(expressions: Union[OWLClassExpression, List[OWLClassExpression]],
                                path: str = 'Predictions',
                                rdf_format: str = 'rdfxml') -> None:
     assert isinstance(expressions, OWLClassExpression) or isinstance(expressions[0],
                                                                      OWLClassExpression), "expressions must be either OWLClassExpression or a list of OWLClassExpression"
     if isinstance(expressions, OWLClassExpression):
         expressions = [expressions]
     NS: Final = 'https://dice-research.org/predictions#'
 
     if rdf_format != 'rdfxml':
         raise NotImplementedError(f'Format {rdf_format} not implemented.')
-    from ..base import OWLOntologyManager_Owlready2
+    from owlapy.owl_ontology_manager import OntologyManager
     # ()
-    manager: OWLOntologyManager = OWLOntologyManager_Owlready2()
+    manager: OWLOntologyManager = OntologyManager()
     # ()
     ontology: OWLOntology = manager.create_ontology(IRI.create(NS))
     # () Iterate over concepts
     for th, i in enumerate(expressions):
         cls_a = OWLClass(IRI.create(NS, str(th)))
         equivalent_classes_axiom = OWLEquivalentClassesAxiom([cls_a, i])
         try:
```

### Comparing `ontosample-0.2.3/ontosample/_base.py` & `ontosample-0.2.4/ontosample/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import random
 import logging
 from typing import Iterable
 
 from owlapy.iri import IRI
 from owlapy.owl_axiom import OWLObjectPropertyAssertionAxiom, OWLDeclarationAxiom, OWLDataPropertyAssertionAxiom
 from owlapy.owl_individual import OWLNamedIndividual
+from owlapy.owl_reasoner import FastInstanceCheckerReasoner, OntologyReasoner
+from owlapy.owl_ontology_manager import OntologyManager
 
 try:
     from ontolearn.knowledge_base import KnowledgeBase
-    from ontolearn.base import OWLReasoner_FastInstanceChecker, OWLReasoner_Owlready2, \
-        OWLOntologyManager_Owlready2
 except ModuleNotFoundError:
     from ontolearn_light.knowledge_base import KnowledgeBase
-    from ontolearn_light.base import OWLReasoner_FastInstanceChecker, OWLReasoner_Owlready2, OWLOntologyManager_Owlready2
 
 logger = logging.getLogger(__name__)
 
 
 class Neighbor:
     """
         Class structure to save a neighbor node in such a way that it also stores the edge type which make the
@@ -168,18 +167,18 @@
                 data_properties_percentage: Percentage of data properties inclusion for each node( values from 0-1 )
                     edges as values.
 
             Returns:
                 Sample of the graph/ontology (of type KnowledgeBase).
         """
 
-        self._manager = OWLOntologyManager_Owlready2()
+        self._manager = OntologyManager()
         self._ontology = self._manager.load_ontology(self.graph.ontology.get_original_iri())
-        self._reasoner = OWLReasoner_FastInstanceChecker(ontology=self._ontology,
-                                                         base_reasoner=OWLReasoner_Owlready2(
+        self._reasoner = FastInstanceCheckerReasoner(ontology=self._ontology,
+                                                         base_reasoner=OntologyReasoner(
                                                              ontology=self._ontology))
 
         assert len(self._sampled_nodes_edges) > 0, "The current sample is empty"
         axioms_to_remove = set(map(OWLDeclarationAxiom, self._get_removed_nodes()))
         for a in axioms_to_remove:
             self._manager.remove_axiom(self._ontology, a)
```

### Comparing `ontosample-0.2.3/ontosample/classic_samplers.py` & `ontosample-0.2.4/ontosample/classic_samplers.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/ontosample/lpc_samplers.py` & `ontosample-0.2.4/ontosample/lpc_samplers.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/ontosample/lpf_samplers.py` & `ontosample-0.2.4/ontosample/lpf_samplers.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.3/ontosample.egg-info/PKG-INFO` & `ontosample-0.2.4/ontosample.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontosample
-Version: 0.2.3
+Version: 0.2.4
 Summary: Ontosample is a package that offers different sampling techniques for OWL ontologies.
 Home-page: https://github.com/alkidbaci/OntoSample
 Author: Alkid Baci
 Author-email: alkid1baci@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -14,14 +14,15 @@
 Requires-Dist: matplotlib>=3.3.4
 Requires-Dist: owlready2>=0.40
 Requires-Dist: torch>=1.7.1
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: sortedcontainers>=2.4.0
 Requires-Dist: owlapy==1.0.2
 Requires-Dist: requests>=2.31.0
+Requires-Dist: deap>=1.3.1
 
 # OntoSample
 
 OntoSample is a python package that offers classic sampling techniques for OWL ontologies/knowledge 
 bases. Furthermore, we have tailored the classic sampling techniques to the setting of concept 
 learning making use of learning problem.
```

### Comparing `ontosample-0.2.3/setup.py` & `ontosample-0.2.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 setup(
     name="ontosample",
     description="Ontosample is a package that offers different sampling techniques for OWL ontologies.",
-    version="0.2.3",
+    version="0.2.4",
     packages=find_packages(),
     install_requires=[
         "matplotlib>=3.3.4",
         "owlready2>=0.40",
         "torch>=1.7.1",
         "pandas>=1.5.0",
         "sortedcontainers>=2.4.0",
         "owlapy==1.0.2",
-        "requests>=2.31.0"],
+        "requests>=2.31.0",
+        "deap>=1.3.1"],
     author='Alkid Baci',
     author_email='alkid1baci@gmail.com',
     url='https://github.com/alkidbaci/OntoSample',
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Topic :: Scientific/Engineering :: Artificial Intelligence"],
```

