# Comparing `tmp/nfdi4culture-0.2-py3-none-any.whl.zip` & `tmp/nfdi4culture-0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 260950 bytes, number of entries: 9
--rw-r--r--  2.0 unx       20 b- defN 80-Jan-01 00:00 nfdi4culture/__init__.py
+Zip file size: 263177 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       55 b- defN 80-Jan-01 00:00 nfdi4culture/__init__.py
 -rw-r--r--  2.0 unx    38806 b- defN 80-Jan-01 00:00 nfdi4culture/cto.ttl
--rw-r--r--  2.0 unx    61101 b- defN 80-Jan-01 00:00 nfdi4culture/cto1.py
+-rw-r--r--  2.0 unx    62306 b- defN 80-Jan-01 00:00 nfdi4culture/cto1.py
 -rw-r--r--  2.0 unx      118 b- defN 80-Jan-01 00:00 nfdi4culture/helpers.py
+-rw-r--r--  2.0 unx     4300 b- defN 80-Jan-01 00:00 nfdi4culture/marc.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 nfdi4culture/ontology.py
 -rw-r--r--  2.0 unx   239711 b- defN 80-Jan-01 00:00 nfdi4culture/schema.ttl
--rw-r--r--  2.0 unx     2013 b- defN 80-Jan-01 00:00 nfdi4culture-0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 nfdi4culture-0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx      689 b- defN 16-Jan-01 00:00 nfdi4culture-0.2.dist-info/RECORD
-9 files, 342546 bytes uncompressed, 259776 bytes compressed:  24.2%
+-rw-r--r--  2.0 unx     1100 b- defN 80-Jan-01 00:00 nfdi4culture-0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2013 b- defN 80-Jan-01 00:00 nfdi4culture-0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 nfdi4culture-0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx      861 b- defN 16-Jan-01 00:00 nfdi4culture-0.3.dist-info/RECORD
+11 files, 349358 bytes uncompressed, 261735 bytes compressed:  25.1%
```

## zipnote {}

```diff
@@ -6,23 +6,29 @@
 
 Filename: nfdi4culture/cto1.py
 Comment: 
 
 Filename: nfdi4culture/helpers.py
 Comment: 
 
+Filename: nfdi4culture/marc.py
+Comment: 
+
 Filename: nfdi4culture/ontology.py
 Comment: 
 
 Filename: nfdi4culture/schema.ttl
 Comment: 
 
-Filename: nfdi4culture-0.2.dist-info/METADATA
+Filename: nfdi4culture-0.3.dist-info/LICENSE.txt
+Comment: 
+
+Filename: nfdi4culture-0.3.dist-info/METADATA
 Comment: 
 
-Filename: nfdi4culture-0.2.dist-info/WHEEL
+Filename: nfdi4culture-0.3.dist-info/WHEEL
 Comment: 
 
-Filename: nfdi4culture-0.2.dist-info/RECORD
+Filename: nfdi4culture-0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nfdi4culture/__init__.py

```diff
@@ -1 +1,2 @@
-from .cto1 import *
+from . import cto1 as cto
+from .marc import parse_marc
```

## nfdi4culture/cto1.py

```diff
@@ -8,505 +8,481 @@
 
 
 # Import libraries
 from datetime import date, datetime
 from rdflib import Graph, Namespace
 from rdflib.term import BNode, Literal, URIRef
 from validators import url
-from ingest import FeedData, FeedElementData
 
 # Define namespaces
 from rdflib.namespace import OWL, RDF, RDFS, SDO, SKOS, XSD
-NFDICORE = Namespace('https://nfdi.fiz-karlsruhe.de/ontology/')
-CTO = Namespace('https://nfdi4culture.de/ontology#')
-MO = Namespace('http://purl.org/ontology/mo/')
-N4C = Namespace('https://nfdi4culture.de/id/')
-GN = Namespace('http://sws.geonames.org/')
-IC = Namespace('https://iconclass.org/')
-AAT = Namespace('http://vocab.getty.edu/page/aat/')
-GND = Namespace('https://d-nb.info/gnd/')
-WD = Namespace('http://www.wikidata.org/entity/')
-VIAF = Namespace('https://viaf.org/viaf/')
-RISM = Namespace('https://rism.online/')
-FG = Namespace('https://database.factgrid.de/wiki/Item:')
-ISIL = Namespace('https://ld.zdb-services.de/resource/organisations/')
+
+NFDICORE = Namespace("https://nfdi.fiz-karlsruhe.de/ontology/")
+CTO = Namespace("https://nfdi4culture.de/ontology#")
+MO = Namespace("http://purl.org/ontology/mo/")
+N4C = Namespace("https://nfdi4culture.de/id/")
+GN = Namespace("http://sws.geonames.org/")
+IC = Namespace("https://iconclass.org/")
+AAT = Namespace("http://vocab.getty.edu/page/aat/")
+GND = Namespace("https://d-nb.info/gnd/")
+WD = Namespace("http://www.wikidata.org/entity/")
+VIAF = Namespace("https://viaf.org/viaf/")
+RISM = Namespace("https://rism.online/")
+FG = Namespace("https://database.factgrid.de/wiki/Item:")
+ISIL = Namespace("https://ld.zdb-services.de/resource/organisations/")
 
 
 # FEED ELEMENT ################################################################
 
 
 class FeedElement:
-    '''
+    """
     Object designed to serialise all triples for an nfdicore/cto feed element
-    '''
+    """
 
     store = None
 
-
     @property
     def feed_uri(self):
-        '''
+        """
         URI of the feed that the element is part of (provides single URIRef)
-        '''
+        """
         return self._feed_uri
 
     @feed_uri.setter
-    def feed_uri(self, value:str|Literal|URIRef|None):
+    def feed_uri(self, value: str | Literal | URIRef | None):
         self._feed_uri = urify(value)
 
-
     @property
     def element_type(self):
-        '''
+        """
         Schema.org class URI or generic string 'person', 'organization', 'place', 'event', or 'item' (provides single URIRef or string)
-        '''
+        """
         return self._element_type
 
     @element_type.setter
-    def element_type(self, value:str|URIRef|None):
+    def element_type(self, value: str | URIRef | None):
         self._element_type = spacify_uri(value)
 
-
     @property
     def element_uri(self):
-        '''
+        """
         URI of the feed element (provides single URIRef)
-        '''
+        """
         return self._element_uri
 
     @element_uri.setter
-    def element_uri(self, value:str|Literal|URIRef|None):
+    def element_uri(self, value: str | Literal | URIRef | None):
         self._element_uri = urify(value)
 
-
     @property
     def element_uri_same(self):
-        '''
+        """
         Additional URIs identifying the same feed element (provides list of URIRef)
-        '''
+        """
         return self._element_uri_same
 
     @element_uri_same.setter
-    def element_uri_same(self, value:str|list|Literal|URIRef|None):
+    def element_uri_same(self, value: str | list | Literal | URIRef | None):
         self._element_uri_same = urify_list(value)
 
-
     @property
     def label(self):
-        '''
+        """
         Main text label of the feed element (provides list of Literal)
-        '''
+        """
         return self._label
 
     @label.setter
-    def label(self, value:str|list|Literal|URIRef|None):
+    def label(self, value: str | list | Literal | URIRef | None):
         self._label = literalify_list(value)
 
-
     @property
     def label_alt(self):
-        '''
+        """
         Alternative text label of the feel element (provides list of Literal)
-        '''
+        """
         return self._label_alt
 
     @label_alt.setter
-    def label_alt(self, value:str|list|Literal|URIRef|None):
+    def label_alt(self, value: str | list | Literal | URIRef | None):
         self._label_alt = literalify_list(value)
 
-
     @property
     def shelf_mark(self):
-        '''
+        """
         Shelf mark in a holding repository, such as a library (provides list of Literal)
-        '''
+        """
         return self._shelf_mark
 
     @shelf_mark.setter
-    def shelf_mark(self, value:str|list|Literal|URIRef|None):
+    def shelf_mark(self, value: str | list | Literal | URIRef | None):
         self._shelf_mark = literalify_list(value)
 
-
     @property
     def image(self):
-        '''
+        """
         URL of an image representation of the element (provides list of Literal)
-        '''
+        """
         return self._image
 
     @image.setter
-    def image(self, value:str|list|Literal|URIRef|None):
+    def image(self, value: str | list | Literal | URIRef | None):
         self._image = literalify_list(value, SDO.URL)
 
-
     @property
     def lyrics(self):
-        '''
+        """
         Lyrics of a musical composition (provides list of Literal)
-        '''
+        """
         return self._lyrics
 
     @lyrics.setter
-    def lyrics(self, value:str|list|Literal|URIRef|None):
+    def lyrics(self, value: str | list | Literal | URIRef | None):
         self._lyrics = literalify_list(value)
 
-
     @property
     def text_incipit(self):
-        '''
+        """
         First few words of text content (provides list of Literal)
-        '''
+        """
         return self._text_incipit
 
     @text_incipit.setter
-    def text_incipit(self, value:str|list|Literal|URIRef|None):
+    def text_incipit(self, value: str | list | Literal | URIRef | None):
         self._text_incipit = literalify_list(value)
 
-
     @property
     def music_incipit(self):
-        '''
+        """
         Dictionary with the keys 'uri' (optional), 'clef', 'key_sig', 'time_sig', and 'pattern' (provides list of dict)
-        '''
+        """
         return self._music_incipit
 
     @music_incipit.setter
-    def music_incipit(self, value:dict|list|None):
-        self._music_incipit = dictify_list(value, ['uri', 'clef', 'key_sig', 'time_sig', 'pattern'])
+    def music_incipit(self, value: dict | list | None):
+        self._music_incipit = dictify_list(
+            value, ["uri", "clef", "key_sig", "time_sig", "pattern"]
+        )
         checked = []
         for i in self._music_incipit:
-            i['uri'] = urify(i['uri'])
-            i['clef'] = literalify(i['clef'])
-            i['key_sig'] = literalify(i['key_sig'])
-            i['time_sig'] = literalify(i['time_sig'])
-            i['pattern'] = literalify(i['pattern'])
+            i["uri"] = urify(i["uri"])
+            i["clef"] = literalify(i["clef"])
+            i["key_sig"] = literalify(i["key_sig"])
+            i["time_sig"] = literalify(i["time_sig"])
+            i["pattern"] = literalify(i["pattern"])
             checked.append(i)
         self._music_incipit = checked
 
-
     @property
     def source_file(self):
-        '''
+        """
         URL of the data source used for this element (provides list of Literal)
-        '''
+        """
         return self._source_file
 
     @source_file.setter
-    def source_file(self, value:str|list|Literal|URIRef|None):
+    def source_file(self, value: str | list | Literal | URIRef | None):
         self._source_file = literalify_list(value, SDO.URL)
 
-
     @property
     def iiif_image_api(self):
-        '''
+        """
         URL of the IIIF Image API of this element (provides list of Literal)
-        '''
+        """
         return self._iiif_image_api
 
     @iiif_image_api.setter
-    def iiif_image_api(self, value:str|list|Literal|URIRef|None):
+    def iiif_image_api(self, value: str | list | Literal | URIRef | None):
         self._iiif_image_api = literalify_list(value, SDO.URL)
 
-
     @property
     def iiif_presentation_api(self):
-        '''
+        """
         URL of the IIIF Presentation API of this element (provides list of Literal)
-        '''
+        """
         return self._iiif_presentation_api
 
     @iiif_presentation_api.setter
-    def iiif_presentation_api(self, value:str|list|Literal|URIRef|None):
+    def iiif_presentation_api(self, value: str | list | Literal | URIRef | None):
         self._iiif_presentation_api = literalify_list(value, SDO.URL)
 
-
     @property
     def ddb_api(self):
-        '''
+        """
         URL of the DDB API of this element (provides list of Literal)
-        '''
+        """
         return self._ddb_api
 
     @ddb_api.setter
-    def ddb_api(self, value:str|list|Literal|URIRef|None):
+    def ddb_api(self, value: str | list | Literal | URIRef | None):
         self._ddb_api = literalify_list(value, SDO.URL)
 
-
     @property
     def oaipmh_api(self):
-        '''
+        """
         URL of the OAI-PMH API of this element (provides list of Literal)
-        '''
+        """
         return self._oaipmh_api
 
     @oaipmh_api.setter
-    def oaipmh_api(self, value:str|list|Literal|URIRef|None):
+    def oaipmh_api(self, value: str | list | Literal | URIRef | None):
         self._oaipmh_api = literalify_list(value, SDO.URL)
 
-
     @property
     def publisher(self):
-        '''
+        """
         URI of the publisher of the element (provides list of URIRef)
-        '''
+        """
         return self._publisher
 
     @publisher.setter
-    def publisher(self, value:str|list|Literal|URIRef|None):
+    def publisher(self, value: str | list | Literal | URIRef | None):
         self._publisher = urify_list(value)
 
-
     @property
     def license(self):
-        '''
+        """
         URI of the element's license (provides list of URIRef)
-        '''
+        """
         return self._license
 
     @license.setter
-    def license(self, value:str|list|Literal|URIRef|None):
+    def license(self, value: str | list | Literal | URIRef | None):
         self._license = urify_list(value)
 
-
     @property
     def vocab_element_type(self):
-        '''
+        """
         Getty AAT URI and/or another string indicating the element type (provides list of URIRef or Literal)
-        '''
+        """
         return self._vocab_element_type
 
     @vocab_element_type.setter
-    def vocab_element_type(self, value:str|tuple|list|Literal|URIRef|None):
+    def vocab_element_type(self, value: str | tuple | list | Literal | URIRef | None):
         self._vocab_element_type = tuplify_uri_literal_list(value)
 
-
     @property
     def vocab_subject_concept(self):
-        '''
+        """
         URI and/or string of a subject, including Iconclass (provides list of URIRef or Literal)
-        '''
+        """
         return self._vocab_subject_concept
 
     @vocab_subject_concept.setter
-    def vocab_subject_concept(self, value:str|tuple|list|Literal|URIRef|None):
+    def vocab_subject_concept(
+        self, value: str | tuple | list | Literal | URIRef | None
+    ):
         self._vocab_subject_concept = tuplify_uri_literal_list(value)
 
-
     @property
     def vocab_related_location(self):
-        '''
+        """
         URI and/or string of a related place, including GeoNames (provides list of URIRef or Literal)
-        '''
+        """
         return self._vocab_related_location
 
     @vocab_related_location.setter
-    def vocab_related_location(self, value:str|tuple|list|Literal|URIRef|None):
+    def vocab_related_location(
+        self, value: str | tuple | list | Literal | URIRef | None
+    ):
         self._vocab_related_location = tuplify_uri_literal_list(value)
 
-
     @property
     def vocab_related_event(self):
-        '''
+        """
         URI and/or string of a related event (provides list of URIRef or Literal)
-        '''
+        """
         return self._vocab_related_event
 
     @vocab_related_event.setter
-    def vocab_related_event(self, value:str|tuple|list|Literal|URIRef|None):
+    def vocab_related_event(self, value: str | tuple | list | Literal | URIRef | None):
         self._vocab_related_event = tuplify_uri_literal_list(value)
 
-
     @property
     def vocab_related_organization(self):
-        '''
+        """
         URI and/or string of a related organization, including ISILs (provides list of URIRef or Literal)
-        '''
+        """
         return self._vocab_related_organization
 
     @vocab_related_organization.setter
-    def vocab_related_organization(self, value:str|tuple|list|Literal|URIRef|None):
+    def vocab_related_organization(
+        self, value: str | tuple | list | Literal | URIRef | None
+    ):
         self._vocab_related_organization = tuplify_uri_literal_list(value)
 
-
     @property
     def vocab_related_person(self):
-        '''
+        """
         URI and/or string of a related person (provides list of URIRef or Literal)
-        '''
+        """
         return self._vocab_related_person
 
     @vocab_related_person.setter
-    def vocab_related_person(self, value:str|tuple|list|Literal|URIRef|None):
+    def vocab_related_person(self, value: str | tuple | list | Literal | URIRef | None):
         self._vocab_related_person = tuplify_uri_literal_list(value)
 
-
     @property
     def vocab_further(self):
-        '''
+        """
         URI of further vocabulary terms which do not fit other categories (provides list of URIRef)
-        '''
+        """
         return self._vocab_further
 
     @vocab_further.setter
-    def vocab_further(self, value:str|list|Literal|URIRef|None):
+    def vocab_further(self, value: str | list | Literal | URIRef | None):
         self._vocab_further = urify_list(value)
 
-
     @property
     def related_item(self):
-        '''
+        """
         URI of a related creative work (provides list of URIRef)
-        '''
+        """
         return self._related_item
 
     @related_item.setter
-    def related_item(self, value:str|list|Literal|URIRef|None):
+    def related_item(self, value: str | list | Literal | URIRef | None):
         self._related_item = urify_list(value)
 
-
     @property
     def birth_date(self):
-        '''
+        """
         Exact date, datetime, or timestamp of a person's birth (provides list of Literal)
-        '''
+        """
         return self._birth_date
 
     @birth_date.setter
-    def birth_date(self, value:str|int|date|datetime|list|Literal|None):
+    def birth_date(self, value: str | int | date | datetime | list | Literal | None):
         self._birth_date = datify_list(value)
 
-
     @property
     def death_date(self):
-        '''
+        """
         Exact date, datetime, or timestamp of a person's death (provides list of Literal)
-        '''
+        """
         return self._death_date
 
     @death_date.setter
-    def death_date(self, value:str|int|date|datetime|list|Literal|None):
+    def death_date(self, value: str | int | date | datetime | list | Literal | None):
         self._death_date = datify_list(value)
 
-
     @property
     def foundation_date(self):
-        '''
+        """
         Exact date, datetime, or timestamp of an organisation's foundation (provides list of Literal)
-        '''
+        """
         return self._foundation_date
 
     @foundation_date.setter
-    def foundation_date(self, value:str|int|date|datetime|list|Literal|None):
+    def foundation_date(
+        self, value: str | int | date | datetime | list | Literal | None
+    ):
         self._foundation_date = datify_list(value)
 
-
     @property
     def dissolution_date(self):
-        '''
+        """
         Exact date, datetime, or timestamp of an organisation's dissolution (provides list of Literal)
-        '''
+        """
         return self._dissolution_date
 
     @dissolution_date.setter
-    def dissolution_date(self, value:str|int|date|datetime|list|Literal|None):
+    def dissolution_date(
+        self, value: str | int | date | datetime | list | Literal | None
+    ):
         self._dissolution_date = datify_list(value)
 
-
     @property
     def start_date(self):
-        '''
+        """
         Exact date, datetime, or timestamp when an event started (provides list of Literal)
-        '''
+        """
         return self._start_date
 
     @start_date.setter
-    def start_date(self, value:str|int|date|datetime|list|Literal|None):
+    def start_date(self, value: str | int | date | datetime | list | Literal | None):
         self._start_date = datify_list(value)
 
-
     @property
     def end_date(self):
-        '''
+        """
         Exact date, datetime, or timestamp when an event ended (provides list of Literal)
-        '''
+        """
         return self._end_date
 
     @end_date.setter
-    def end_date(self, value:str|int|date|datetime|list|Literal|None):
+    def end_date(self, value: str | int | date | datetime | list | Literal | None):
         self._end_date = datify_list(value)
 
-
     @property
     def creation_date(self):
-        '''
+        """
         Exact date, datetime, or timestamp of an item's creation (provides list of Literal)
-        '''
+        """
         return self._creation_date
 
     @creation_date.setter
-    def creation_date(self, value:str|int|date|datetime|list|Literal|None):
+    def creation_date(self, value: str | int | date | datetime | list | Literal | None):
         self._creation_date = datify_list(value)
 
-
     @property
     def creation_period(self):
-        '''
+        """
         String providing an item's creation period (provides list of Literal)
-        '''
+        """
         return self._creation_period
 
     @creation_period.setter
-    def creation_period(self, value:str|list|Literal|None):
+    def creation_period(self, value: str | list | Literal | None):
         self._creation_period = periodify_or_literalify_list(value)
 
-
     @property
     def destruction_date(self):
-        '''
+        """
         Exact date, datetime, or timestamp of an item's destruction (provides list of Literal)
-        '''
+        """
         return self._destruction_date
 
     @destruction_date.setter
-    def destruction_date(self, value:str|int|date|datetime|list|Literal|None):
+    def destruction_date(
+        self, value: str | int | date | datetime | list | Literal | None
+    ):
         self._destruction_date = datify_list(value)
 
-
     @property
     def approximate_period(self):
-        '''
+        """
         String providing a period that an item is associated with (provides list of Literal)
-        '''
+        """
         return self._approximate_period
 
     @approximate_period.setter
-    def approximate_period(self, value:str|list|Literal|None):
+    def approximate_period(self, value: str | list | Literal | None):
         self._approximate_period = periodify_or_literalify_list(value)
 
-
     @property
     def existence_period(self):
-        '''
+        """
         String providing the period of an item's existence (provides list of Literal)
-        '''
+        """
         return self._existence_period
 
     @existence_period.setter
-    def existence_period(self, value:str|list|Literal|None):
+    def existence_period(self, value: str | list | Literal | None):
         self._existence_period = periodify_or_literalify_list(value)
 
-
-    def __init__(self, data:FeedElementData|None = None, prepare:bool = True):
-        '''
+    def __init__(self, data=None, prepare: bool = True):
+        """
         Object designed to serialise all triples for an nfdicore/cto feed
 
             Parameters:
                 data (FeedElementData|None): Data object to set up the feed
                 prepare (bool): Add wrappers to prepare the connection of research data to research information
-        '''
+        """
 
         # Assign arguments
         self.prepare = prepare
 
         # Use data object if available
         if data:
             self.feed_uri = data.feed_uri
@@ -543,45 +519,56 @@
             self.end_date = data.end_date
             self.creation_date = data.creation_date
             self.creation_period = data.creation_period
             self.destruction_date = data.destruction_date
             self.approximate_period = data.approximate_period
             self.existence_period = data.existence_period
 
-
     def generate(self):
-        '''
+        """
         Generate triples and fill the store attribute
-        '''
+        """
 
         # Check requirements
         if self.element_uri == None:
-            raise ValueError('The feed element URI is missing.')
+            raise ValueError("The feed element URI is missing.")
         elif self.feed_uri == None:
-            raise ValueError('The feed URI is missing.')
+            raise ValueError("The feed URI is missing.")
         else:
             self.store = spacify_graph()
 
             # ELEMENT
 
             # Element and feed URI
             self.store.add((self.element_uri, RDF.type, CTO.DatafeedElement))
             self.store.add((self.element_uri, CTO.elementOf, self.feed_uri))
 
             # Element type: person
-            if self.element_type == 'person' or self.element_type in sdo_person:
+            if self.element_type == "person" or self.element_type in sdo_person:
                 self.store.add((self.element_uri, RDF.type, NFDICORE.Person))
-             # Element type: organization
-            elif self.element_type == 'organization' or self.element_type == 'organisation' or self.element_type in sdo_organization:
+            # Element type: organization
+            elif (
+                self.element_type == "organization"
+                or self.element_type == "organisation"
+                or self.element_type in sdo_organization
+            ):
                 self.store.add((self.element_uri, RDF.type, NFDICORE.Organization))
             # Element type: place
-            elif self.element_type == 'place' or self.element_type == 'location' or self.element_type in sdo_place:
+            elif (
+                self.element_type == "place"
+                or self.element_type == "location"
+                or self.element_type in sdo_place
+            ):
                 self.store.add((self.element_uri, RDF.type, NFDICORE.Place))
             # Element type: event
-            elif self.element_type == 'event' or self.element_type == 'date' or self.element_type in sdo_event:
+            elif (
+                self.element_type == "event"
+                or self.element_type == "date"
+                or self.element_type in sdo_event
+            ):
                 self.store.add((self.element_uri, RDF.type, NFDICORE.Event))
             # Element type: item that is a schema.org creative work
             elif self.element_type in sdo_item:
                 self.store.add((self.element_uri, RDF.type, self.element_type))
             # Element type: generic item
             else:
                 self.store.add((self.element_uri, RDF.type, CTO.Item))
@@ -605,21 +592,23 @@
 
             # Alternative label
             for i in self.label_alt:
                 self.store.add((self.element_uri, SKOS.altLabel, i))
 
             # Shelf mark
             for i in self.shelf_mark:
-                i = Literal(str(i)) # Removes lang
+                i = Literal(str(i))  # Removes lang
                 self.store.add((self.element_uri, CTO.shelfMark, i))
 
             # MEDIA LITERALS
 
             # URL
-            self.store.add((self.element_uri, SDO.url, literalify(self.element_uri, SDO.URL)))
+            self.store.add(
+                (self.element_uri, SDO.url, literalify(self.element_uri, SDO.URL))
+            )
 
             # Image
             for i in self.image:
                 self.store.add((self.element_uri, SDO.image, i))
 
             # Lyrics
             for i in self.lyrics:
@@ -630,24 +619,24 @@
 
             # Text incipit
             for i in self.text_incipit:
                 self.store.add((self.element_uri, CTO.textIncipit, i))
 
             # Music incipit
             for i in self.music_incipit:
-                if i['uri'] != None:
-                    uri_or_blank = i['uri']
+                if i["uri"] != None:
+                    uri_or_blank = i["uri"]
                 else:
                     uri_or_blank = BNode()
                 self.store.add((uri_or_blank, RDF.type, CTO.Incipit))
                 self.store.add((uri_or_blank, CTO.incipitOf, self.element_uri))
-                self.store.add((uri_or_blank, CTO.clef, i['clef']))
-                self.store.add((uri_or_blank, CTO.keySignature, i['key_sig']))
-                self.store.add((uri_or_blank, CTO.timeSignature, i['time_sig']))
-                self.store.add((uri_or_blank, CTO.pattern, i['pattern']))
+                self.store.add((uri_or_blank, CTO.clef, i["clef"]))
+                self.store.add((uri_or_blank, CTO.keySignature, i["key_sig"]))
+                self.store.add((uri_or_blank, CTO.timeSignature, i["time_sig"]))
+                self.store.add((uri_or_blank, CTO.pattern, i["pattern"]))
 
             # Source file
             for i in self.source_file:
                 self.store.add((self.element_uri, CTO.sourceFile, i))
 
             # API LITERALS
 
@@ -661,15 +650,17 @@
 
             # DDB API
             for i in self.ddb_api:
                 self.store.add((self.element_uri, CTO.ddbAPI, i))
 
             # OAI-PMH API
             for i in self.oaipmh_api:
-                self.store.add((self.element_uri, CTO['oai-pmhAPI'], i)) # Alternative notation due to hyphen
+                self.store.add(
+                    (self.element_uri, CTO["oai-pmhAPI"], i)
+                )  # Alternative notation due to hyphen
 
             # RIGHTS URIS
 
             # Publisher
             for i in self.publisher:
                 self.store.add((self.element_uri, NFDICORE.publisher, i))
 
@@ -716,15 +707,17 @@
                     self.store.add((t[has_uri], RDF.type, NFDICORE.Place))
                     self.store += vocabify(t[has_uri], self.element_uri)
                     for index, i in t:
                         if index != has_uri:
                             self.store.add((t[has_uri], RDFS.label, i))
                 else:
                     for i in t:
-                        self.store.add((self.element_uri, CTO.relatedLocationLiteral, i))
+                        self.store.add(
+                            (self.element_uri, CTO.relatedLocationLiteral, i)
+                        )
 
             # Related event
             has_uri = None
             for t in self.vocab_element_type:
                 for index, i in t:
                     if isinstance(i, URIRef):
                         has_uri = index
@@ -742,23 +735,27 @@
             # Related organization
             has_uri = None
             for t in self.vocab_element_type:
                 for index, i in t:
                     if isinstance(i, URIRef):
                         has_uri = index
                 if has_uri != None:
-                    self.store.add((self.element_uri, CTO.relatedOrganization, t[has_uri]))
+                    self.store.add(
+                        (self.element_uri, CTO.relatedOrganization, t[has_uri])
+                    )
                     self.store.add((t[has_uri], RDF.type, NFDICORE.Organization))
                     self.store += vocabify(t[has_uri], self.element_uri)
                     for index, i in t:
                         if index != has_uri:
                             self.store.add((t[has_uri], RDFS.label, i))
                 else:
                     for i in t:
-                        self.store.add((self.element_uri, CTO.relatedOrganizationLiteral, i))
+                        self.store.add(
+                            (self.element_uri, CTO.relatedOrganizationLiteral, i)
+                        )
 
             # Related person
             has_uri = None
             for t in self.vocab_element_type:
                 for index, i in t:
                     if isinstance(i, URIRef):
                         has_uri = index
@@ -780,41 +777,53 @@
             # Related item
             for i in self.related_item:
                 self.store.add((self.element_uri, CTO.relatedItem, i))
 
             # DATES BY TYPE
 
             # For persons
-            if self.element_type == 'person' or self.element_type in sdo_person:
+            if self.element_type == "person" or self.element_type in sdo_person:
 
                 # Birth date
                 for i in self.birth_date:
                     self.store.add((self.element_uri, NFDICORE.birthDate, i))
 
                 # Death date
                 for i in self.death_date:
                     self.store.add((self.element_uri, NFDICORE.deathDate, i))
 
             # For organizations
-            elif self.element_type == 'organization' or self.element_type == 'organisation' or self.element_type in sdo_organization:
+            elif (
+                self.element_type == "organization"
+                or self.element_type == "organisation"
+                or self.element_type in sdo_organization
+            ):
 
                 # Foundation date
                 for i in self.foundation_date:
                     self.store.add((self.element_uri, NFDICORE.foundationDate, i))
 
                 # Dissolution date
                 for i in self.dissolution_date:
                     self.store.add((self.element_uri, NFDICORE.dissolutionDate, i))
 
             # For places
-            elif self.element_type == 'place' or self.element_type == 'location' or self.element_type in sdo_place:
+            elif (
+                self.element_type == "place"
+                or self.element_type == "location"
+                or self.element_type in sdo_place
+            ):
                 pass
 
             # For events
-            elif self.element_type == 'event' or self.element_type == 'date' or self.element_type in sdo_event:
+            elif (
+                self.element_type == "event"
+                or self.element_type == "date"
+                or self.element_type in sdo_event
+            ):
 
                 # Start date
                 for i in self.start_date:
                     self.store.add((self.element_uri, NFDICORE.startDate, i))
 
                 # End date
                 for i in self.end_date:
@@ -839,163 +848,156 @@
                 for i in self.approximate_period:
                     self.store.add((self.element_uri, CTO.approximatePeriod, i))
 
                 # Existence period
                 for i in self.existence_period:
                     self.store.add((self.element_uri, CTO.existencePeriod, i))
 
-
-    def turtle(self, file_path:str):
-        '''
+    def turtle(self, file_path: str):
+        """
         Serialise triples as a Turtle file
 
             Parameters:
                 file_path (str): Path of the file to create
-        '''
+        """
 
         # Store triples and save file
         self.generate()
-        self.store.serialize(destination = file_path, format = 'turtle')
-
+        self.store.serialize(destination=file_path, format="turtle")
 
-    def ntriples(self, file_path:str):
-        '''
+    def ntriples(self, file_path: str):
+        """
         Serialise triples as an NTriples file
 
             Parameters:
                 file_path (str): Path of the file to create
-        '''
+        """
 
         # Store triples and save file
         self.generate()
-        self.store.serialize(destination = file_path, format = 'ntriples')
+        self.store.serialize(destination=file_path, format="ntriples")
 
-
-    def rdfxml(self, file_path:str):
-        '''
+    def rdfxml(self, file_path: str):
+        """
         Serialise triples as an NTriples file
 
             Parameters:
                 file_path (str): Path of the file to create
-        '''
+        """
 
         # Store triples and save file
         self.generate()
-        self.store.serialize(destination = file_path, format = 'xml')
+        self.store.serialize(destination=file_path, format="xml")
 
 
 # FEED ########################################################################
 
 
 class Feed:
-    '''
+    """
     Object designed to serialise all triples for an nfdicore/cto feed
-    '''
+    """
 
     store = None
 
-
     @property
     def feed_uri(self):
-        '''
+        """
         URI of the feed, preferably an NFDI4Culture IRI (provides single URIRef)
-        '''
+        """
         return self._feed_uri
 
     @feed_uri.setter
-    def feed_uri(self, value:str|Literal|URIRef|None):
+    def feed_uri(self, value: str | Literal | URIRef | None):
         self._feed_uri = urify(value)
 
-
     @property
     def feed_uri_same(self):
-        '''
+        """
         Additional URIs identifying the same feed (provides list of URIRef)
-        '''
+        """
         return self._feed_uri_same
 
     @feed_uri_same.setter
-    def feed_uri_same(self, value:str|list|Literal|URIRef|None):
+    def feed_uri_same(self, value: str | list | Literal | URIRef | None):
         self._feed_uri_same = urify_list(value)
 
-
     @property
     def catalog_uri(self):
-        '''
+        """
         URI of the catalog the feed belongs to, preferably an NFDI4Culture IRI (provides single URIRef)
-        '''
+        """
         return self._catalog_uri
 
     @catalog_uri.setter
-    def catalog_uri(self, value:str|Literal|URIRef|None):
+    def catalog_uri(self, value: str | Literal | URIRef | None):
         self._catalog_uri = urify(value)
 
-
     @property
     def catalog_uri_same(self):
-        '''
+        """
         Additional URIs identifying the same catalog (provides list of URIRef)
-        '''
+        """
         return self._catalog_uri_same
 
     @catalog_uri_same.setter
-    def catalog_uri_same(self, value:str|Literal|URIRef|None):
+    def catalog_uri_same(self, value: str | Literal | URIRef | None):
         self._catalog_uri_same = urify_list(value)
 
     @property
     def elements(self):
-        '''
+        """
         List of elements that are part of this feed (provides list of FeedElement)
-        '''
+        """
         return self._elements
 
     @elements.setter
-    def elements(self, value:list|FeedElement|None):
+    def elements(self, value: list | FeedElement | None):
         self._elements = elementify_list(value)
 
-
-    def __init__(self, data:FeedData|None = None, prepare:bool = True):
-        '''
+    def __init__(self, data=None, prepare: bool = True):
+        """
         Object designed to serialise all triples for an nfdicore/cto feed
 
             Parameters:
                 data (FeedData|None): Data object to set up the feed
                 prepare (bool): Add wrappers to prepare the connection of research data to research information
-        '''
+        """
 
         # Assign arguments
         self.prepare = prepare
 
         # Use data object if available
         if data:
             self.feed_uri = data.feed_uri
             self.feed_uri_same = data.feed_uri_same
             self.catalog_uri = data.catalog_uri
             self.catalog_uri_same = data.catalog_uri_same
             self.elements = data.elements
 
-
     def generate(self):
-        '''
+        """
         Generate triples and fill the store attribute
-        '''
+        """
 
         # Check requirements
         if self.feed_uri == None:
-            raise ValueError('The feed URI is missing.')
+            raise ValueError("The feed URI is missing.")
         else:
             self.store = spacify_graph()
 
             # Feed URI
             self.store.add((self.feed_uri, RDF.type, NFDICORE.Dataset))
 
             # Optional date modified
             if self.prepare:
                 today = date.today()
-                self.store.add((self.feed_uri, SDO.dateModified, Literal(today, datatype=XSD.date)))
+                self.store.add(
+                    (self.feed_uri, SDO.dateModified, Literal(today, datatype=XSD.date))
+                )
 
             # Same as feed URI
             for i in self.feed_uri_same:
                 self.store.add((self.feed_uri, OWL.sameAs, i))
 
             # Catalog URI
             if self.catalog_uri:
@@ -1008,68 +1010,65 @@
 
             # Add element triples and overwrite the feed URI
             for i in self.elements:
                 i.feed_uri = self.feed_uri
                 i.generate()
                 self.store += i.store
 
-
-    def turtle(self, file_path:str):
-        '''
+    def turtle(self, file_path: str):
+        """
         Serialise triples as a Turtle file
 
             Parameters:
                 file_path (str): Path of the file to create
-        '''
+        """
 
         # Store triples and save file
         self.generate()
-        self.store.serialize(destination = file_path, format = 'turtle')
-
+        self.store.serialize(destination=file_path, format="turtle")
 
-    def ntriples(self, file_path:str):
-        '''
+    def ntriples(self, file_path: str):
+        """
         Serialise triples as an NTriples file
 
             Parameters:
                 file_path (str): Path of the file to create
-        '''
+        """
 
         # Store triples and save file
         self.generate()
-        self.store.serialize(destination = file_path, format = 'ntriples')
+        self.store.serialize(destination=file_path, format="ntriples")
 
-
-    def rdfxml(self, file_path:str):
-        '''
+    def rdfxml(self, file_path: str):
+        """
         Serialise triples as an NTriples file
 
             Parameters:
                 file_path (str): Path of the file to create
-        '''
+        """
 
         # Store triples and save file
         self.generate()
-        self.store.serialize(destination = file_path, format = 'xml')
+        self.store.serialize(destination=file_path, format="xml")
 
 
 # TRIPLE HELPERS ##############################################################
 
 
-def vocabify(input:URIRef, element_uri:URIRef) -> URIRef:
-    '''
+def vocabify(input: URIRef, element_uri: URIRef) -> URIRef:
+    """
     Clean vocabulary URIs, add their respective vocab triple, and return the clean URIRef
 
         Parameters:
             input (URIRef): Variable to check and add a triple for
             element_uri (URIRef): URI of the element to add the triple to
 
         Returns:
             URIRef: Normalised input
-    '''
+    """
 
     # Set up graph
     output = spacify_graph()
 
     # Check which vocab triple is necessary
     if input in GN:
         output.add((element_uri, CTO.geonames, input))
@@ -1087,32 +1086,32 @@
         output.add((element_uri, CTO.rism, input))
     elif input in FG:
         output.add((element_uri, CTO.factgrid, input))
     elif input in ISIL:
         output.add((element_uri, CTO.isil, input))
     else:
         output.add((element_uri, CTO.externalVocabulary, input))
-            
+
     # Return altered input
     return output
 
 
 # INPUT HELPERS ###############################################################
 
 
-def urify(input:str|URIRef|Literal) -> URIRef|None:
-    '''
+def urify(input: str | URIRef | Literal) -> URIRef | None:
+    """
     Make sure a variable is a URI
 
         Parameters:
             input (str|URIRef|Literal): Variable to check and transform
 
         Returns:
             URIRef: URI value
-    '''
+    """
 
     # Turn str to URIRef
     if isinstance(input, str):
         if url(input):
             input = URIRef(input)
         else:
             input = None
@@ -1135,24 +1134,24 @@
     if input != None:
         input = spacify_uri(input)
 
     # Return URI
     return input
 
 
-def urify_list(input:str|list|Literal|URIRef|None) -> list:
-    '''
+def urify_list(input: str | list | Literal | URIRef | None) -> list:
+    """
     Make sure a variable contains a list of URIs
 
         Parameters:
             input (str|list|Literal|URIRef|None): Variable to check and transform
 
         Returns:
             list: List of URI values
-    '''
+    """
 
     # Catch type None
     if input == None:
         input = []
 
     # Turn str, URIRef, and Literal to list
     elif isinstance(input, (str, URIRef, Literal)):
@@ -1165,64 +1164,68 @@
         if i != None:
             output.append(i)
 
     # Return list
     return output
 
 
-def literalify(input:str|URIRef|Literal, data_type:URIRef = None) -> Literal|None:
-    '''
+def literalify(
+    input: str | URIRef | Literal, data_type: URIRef = None
+) -> Literal | None:
+    """
     Make sure a variable is a Literal
 
         Parameters:
             input (str|URIRef|Literal): Variable to check and transform
             data_type (URIRef): Data type of the literal
 
         Returns:
             Literal: Literal value
-    '''
+    """
 
     # Turn str to Literal
     if isinstance(input, str):
-        if input != '':
+        if input != "":
             input = Literal(input, datatype=data_type)
         else:
             input = None
 
     # Turn URIRef to Literal
     elif isinstance(input, URIRef):
-        if str(input) != '':
+        if str(input) != "":
             input = Literal(str(input), datatype=data_type)
         else:
             input = None
 
     # Check Literal
     elif isinstance(input, Literal):
-        if str(input) == '':
+        if str(input) == "":
             input = None
         else:
             input.datatype = data_type
     else:
         input = None
 
     # Return URI
     return input
 
 
-def literalify_list(input:str|list|Literal|URIRef|None, data_type:URIRef = None) -> list:
-    '''
+def literalify_list(
+    input: str | list | Literal | URIRef | None, data_type: URIRef = None
+) -> list:
+    """
     Make sure a variable contains a list of Literals
 
         Parameters:
             input (str|list|Literal|URIRef|None): Variable to check and transform
             data_type (URIRef): Data type of the literal
 
         Returns:
             list: List of URI values
-    '''
+    """
 
     # Catch type None
     if input == None:
         input = []
 
     # Turn str, URIRef, and Literal to list
     elif isinstance(input, (str, URIRef, Literal)):
@@ -1235,42 +1238,42 @@
         if i != None:
             output.append(i)
 
     # Return list
     return output
 
 
-def tuplify_uri_literal(input:str|tuple|Literal|URIRef) -> tuple:
-    '''
+def tuplify_uri_literal(input: str | tuple | Literal | URIRef) -> tuple:
+    """
     Make sure a variable contains a tuple with a URIRef and/or Literals
 
         Parameters:
             input (str|tuple|Literal|URIRef): Variable to check and transform
 
         Returns:
             tuple: Tuple with a URI value and/or Literals
-    '''
+    """
 
     # Turn str to tuple
     if isinstance(input, str):
-        if input != '':
+        if input != "":
             input = (Literal(input),)
         else:
             input = None
 
     # Turn Literal to tuple
     elif isinstance(input, Literal):
-        if str(input) != '':
+        if str(input) != "":
             input = (input,)
         else:
             input = None
 
     # Turn URIRef to tuple
     elif isinstance(input, URIRef):
-        if str(input) != '':
+        if str(input) != "":
             input = (input,)
         else:
             input = None
 
     # Check tuples to contain only Literals and URIRefs
     if isinstance(input, tuple):
         output = []
@@ -1289,24 +1292,26 @@
     else:
         input = None
 
     # Return tuple
     return input
 
 
-def tuplify_uri_literal_list(input:str|tuple|list|Literal|URIRef|None) -> list:
-    '''
+def tuplify_uri_literal_list(
+    input: str | tuple | list | Literal | URIRef | None,
+) -> list:
+    """
     Make sure a variable contains a list of tuples with a URIRef and/or Literals
 
         Parameters:
             input (str|tuple|list|Literal|URIRef|None): Variable to check and transform
 
         Returns:
             list: List of tuples with a URI value and/or Literals
-    '''
+    """
 
     # Catch type None
     if input == None:
         input = []
 
     # Turn str, tuple, URIRef, and Literal to list
     elif isinstance(input, (str, tuple, URIRef, Literal)):
@@ -1319,24 +1324,24 @@
         if i != None:
             output.append(i)
 
     # Return list
     return output
 
 
-def periodify_or_literalify_list(input:str|list|URIRef|Literal|None) -> list:
-    '''
+def periodify_or_literalify_list(input: str | list | URIRef | Literal | None) -> list:
+    """
     Make sure a variable contains a list of schema:DateTime periods and Literals
 
         Parameters:
             input (str|list|URIRef|Literal|None): Variable to check and transform
 
         Returns:
             list: List of schema:DateTimes and Literals
-    '''
+    """
 
     # Catch type None
     if input == None:
         input = []
 
     # Turn str, URIRef, and Literal to list
     elif isinstance(input, (str, URIRef, Literal)):
@@ -1353,89 +1358,89 @@
         if i != None:
             output.append(i)
 
     # Return list
     return output
 
 
-def periodify(input:str|URIRef|Literal|None) -> Literal:
-    '''
+def periodify(input: str | URIRef | Literal | None) -> Literal:
+    """
     Make sure a variable is a schema:DateTime period
 
         Parameters:
             input (str|URIRef|Literal|None): Variable to check and transform
 
         Returns:
             Literal: Literal with the data type schema:DateTime
-    '''
+    """
 
     # Turn URIRef and Literal to str
     if isinstance(input, (URIRef, Literal)):
-        if str(input) != '':
+        if str(input) != "":
             input = str(input)
         else:
             input = None
 
     # Check string
     elif isinstance(input, str):
-        if input == '':
+        if input == "":
             input = None
     else:
         input = None
 
     # Split in two if str contains a slash
-    if '/' in input:
-        parts_in = input.split('/', 1)
+    if "/" in input:
+        parts_in = input.split("/", 1)
         parts_out = []
         for part in parts_in:
             part = datify(part)
             parts_out.append(part)
 
         # Construct schema:DateTime Literal if both parts are dates
         if parts_out[0] != None and parts_out[1] != None:
-            input = str(parts_out[0]) + '/' + str(parts_out[1])
-            input = Literal(input, datatype = SDO.DateTime)
+            input = str(parts_out[0]) + "/" + str(parts_out[1])
+            input = Literal(input, datatype=SDO.DateTime)
         else:
             input = None
     else:
         input = None
 
     # Return period
     return input
 
 
-def datify(input:str|int|date|datetime|Literal) -> Literal:
-    '''
+def datify(input: str | int | date | datetime | Literal) -> Literal:
+    """
     Make sure a variable is a date
 
         Parameters:
             input (str|int|date|datetime|Literal): Variable to check and transform
 
         Returns:
             Literal: Literal with the right data type
-    '''
+    """
 
     # Leave date and datetime as is
     if isinstance(input, (date, datetime)):
         pass
 
     # Turn int (timestamp) to datetime
     if isinstance(input, int):
         input = datetime.fromtimestamp(input)
 
     # Turn Literal to str
     elif isinstance(input, Literal):
-        if str(input) != '':
+        if str(input) != "":
             input = str(input)
         else:
             input = None
 
     # Check string
     elif isinstance(input, str):
-        if input == '':
+        if input == "":
             input = None
     else:
         input = None
 
     # Convert str to date or datetime
     if isinstance(input, str):
         try:
@@ -1444,35 +1449,35 @@
             try:
                 input = datetime.fromisoformat(input)
             except:
                 input = None
 
     # Serialise datetime and date
     if input != None:
-        if isinstance(input, datetime): # Each datetime is also a date
-            input = Literal(input.isoformat(), datatype = XSD.dateTime)
+        if isinstance(input, datetime):  # Each datetime is also a date
+            input = Literal(input.isoformat(), datatype=XSD.dateTime)
         elif isinstance(input, date):
-            input = Literal(input.isoformat(), datatype = XSD.date)
+            input = Literal(input.isoformat(), datatype=XSD.date)
         else:
             input = None
 
     # Return date
     return input
 
 
-def datify_list(input:str|int|date|datetime|list|Literal|None) -> list:
-    '''
+def datify_list(input: str | int | date | datetime | list | Literal | None) -> list:
+    """
     Make sure a variable contains a list of dates
 
         Parameters:
             input (str|int|date|datetime|list|Literal|None): Variable to check and transform
 
         Returns:
             list: List of date literals
-    '''
+    """
 
     # Catch type None
     if input == None:
         input = []
 
     # Turn str, int, date, datetime and Literal to list
     elif isinstance(input, (str, int, date, datetime, Literal)):
@@ -1485,25 +1490,25 @@
         if i != None:
             output.append(i)
 
     # Return list
     return output
 
 
-def dictify(input:dict, keys:list = None) -> dict|None:
-    '''
+def dictify(input: dict, keys: list = None) -> dict | None:
+    """
     Make sure a variable is a dictionary
 
         Parameters:
             input (dict): Variable to check and transform
             keys (list): List of keys to limit dictionaries to
 
         Returns:
             dict: Orderly dictionary
-    '''
+    """
 
     # Check dictionary
     output = {}
     if isinstance(input, dict):
         if keys != None:
             for key, value in input.items():
                 if key in keys:
@@ -1511,25 +1516,25 @@
     else:
         input = None
 
     # Return dictionary
     return output
 
 
-def dictify_list(input:dict|list|None, keys:list = None) -> list:
-    '''
+def dictify_list(input: dict | list | None, keys: list = None) -> list:
+    """
     Make sure a variable contains a list of dictionaries
 
         Parameters:
             input (dict|list|None): Variable to check and transform
             keys (list): List of keys to limit dictionaries to
 
         Returns:
             list: List of dictionaries
-    '''
+    """
 
     # Catch type None
     if input == None:
         input = []
 
     # Turn dict to list
     elif isinstance(input, dict):
@@ -1542,24 +1547,24 @@
         if i != None:
             output.append(i)
 
     # Return list
     return output
 
 
-def elementify_list(input:list|FeedElement|None) -> list:
-    '''
+def elementify_list(input: list | FeedElement | None) -> list:
+    """
     Make sure a variable contains a list of FeedElements
 
         Parameters:
             input (list|FeedElement|None): Variable to check and transform
 
         Returns:
             list: List of FeedElements
-    '''
+    """
 
     # Catch type None
     if input == None:
         input = []
 
     # Turn FeedElement to list
     elif isinstance(input, FeedElement):
@@ -1579,70 +1584,78 @@
     return output
 
 
 # NAMESPACE HELPERS ###########################################################
 
 
 def spacify_graph() -> Graph:
-    '''
+    """
     Produce an empty graph object with all required namespaces
 
         Returns:
             Graph: Basic graph object
-    '''
+    """
 
     # Initialise graph
     output = Graph()
 
     # Ontologies
-    output.bind('cto', CTO)
-    output.bind('mo', MO)
-    output.bind('nfdicore', NFDICORE)
-    output.bind('owl', OWL)
-    output.bind('rdf', RDF)
-    output.bind('rdfs', RDFS)
-    output.bind('sdo', SDO)
-    output.bind('xsd', XSD)
+    output.bind("cto", CTO)
+    output.bind("mo", MO)
+    output.bind("nfdicore", NFDICORE)
+    output.bind("owl", OWL)
+    output.bind("rdf", RDF)
+    output.bind("rdfs", RDFS)
+    output.bind("sdo", SDO)
+    output.bind("xsd", XSD)
 
     # Vocabularies
-    output.bind('n4c', N4C)
-    output.bind('gn', GN)
-    output.bind('ic', IC)
-    output.bind('aat', AAT)
-    output.bind('gnd', GND)
-    output.bind('wd', WD)
-    output.bind('viaf', VIAF)
-    output.bind('rism', RISM)
-    output.bind('fg', FG)
-    output.bind('isil', ISIL)
+    output.bind("n4c", N4C)
+    output.bind("gn", GN)
+    output.bind("ic", IC)
+    output.bind("aat", AAT)
+    output.bind("gnd", GND)
+    output.bind("wd", WD)
+    output.bind("viaf", VIAF)
+    output.bind("rism", RISM)
+    output.bind("fg", FG)
+    output.bind("isil", ISIL)
 
     # Return graph
     return output
 
 
-def spacify_uri(input:URIRef) -> URIRef:
-    '''
+def spacify_uri(input: URIRef) -> URIRef:
+    """
     Normalise common 'http' and 'https' mistakes in namespaces of incoming URIRefs
 
         Parameters:
             input (URIRef): Variable to check and transform
 
         Returns:
             URIRef: Clean URIRef
-    '''
+    """
 
     # Remove trailing slashes
-    if str(input).endswith('/'):
+    if str(input).endswith("/"):
         input = URIRef(str(input)[:-1])
 
     # Avoid known GeoNames issues
-    if str(input).startswith('http://www.geonames.org/'):
-        input = URIRef(str(input).replace('http://www.geonames.org/', 'http://sws.geonames.org/', 1))
-    elif str(input).startswith('https://www.geonames.org/'):
-        input = URIRef(str(input).replace('https://www.geonames.org/', 'http://sws.geonames.org/', 1))
+    if str(input).startswith("http://www.geonames.org/"):
+        input = URIRef(
+            str(input).replace(
+                "http://www.geonames.org/", "http://sws.geonames.org/", 1
+            )
+        )
+    elif str(input).startswith("https://www.geonames.org/"):
+        input = URIRef(
+            str(input).replace(
+                "https://www.geonames.org/", "http://sws.geonames.org/", 1
+            )
+        )
 
     # List namespaces to check
     checks = [
         CTO,
         MO,
         NFDICORE,
         OWL,
@@ -1655,48 +1668,42 @@
         IC,
         AAT,
         GND,
         WD,
         VIAF,
         RISM,
         FG,
-        ISIL
+        ISIL,
     ]
 
     # Prepare http/https check if not a regular namespace
     for check in checks:
         if input not in check:
 
             # Switch http and https and test again
-            if str(input).startswith('http://'):
-                input_copy = URIRef(str(input).replace('http://', 'https://', 1))
+            if str(input).startswith("http://"):
+                input_copy = URIRef(str(input).replace("http://", "https://", 1))
                 if input_copy in check:
                     input = input_copy
-            elif str(input).startswith('https://'):
-                input_copy = URIRef(str(input).replace('https://', 'http://', 1))
+            elif str(input).startswith("https://"):
+                input_copy = URIRef(str(input).replace("https://", "http://", 1))
                 if input_copy in check:
                     input = input_copy
 
     # Return URIRef
     return input
 
 
 # HELPER VARS #################################################################
 
 
 # Lists of schema.org classes, collated on 17/4/2024, periodical update TODO
 # Some SDO items commented out as they are not in RDFLib's internal library
-sdo_feed = [
-    SDO.DataFeed,
-    SDO.Dataset
-]
-sdo_person = [
-    SDO.Person,
-    SDO.Patient
-]
+sdo_feed = [SDO.DataFeed, SDO.Dataset]
+sdo_person = [SDO.Person, SDO.Patient]
 sdo_organization = [
     SDO.Organization,
     SDO.Airline,
     SDO.Consortium,
     SDO.Corporation,
     SDO.EducationalOrganization,
     SDO.CollegeOrUniversity,
@@ -1779,24 +1786,24 @@
     SDO.BedAndBreakfast,
     SDO.Campground,
     SDO.Hostel,
     SDO.Hotel,
     SDO.Motel,
     SDO.Resort,
     SDO.SkiResort,
-    #SDO.VacationRental,
+    # SDO.VacationRental,
     SDO.MedicalBusiness,
     SDO.Dentist,
     SDO.MedicalClinic,
     SDO.CovidTestingFacility,
     SDO.Optician,
     SDO.Pharmacy,
     SDO.Physician,
-    #SDO.IndividualPhysician,
-    #SDO.PhysiciansOffice,
+    # SDO.IndividualPhysician,
+    # SDO.PhysiciansOffice,
     SDO.ProfessionalService,
     SDO.RadioStation,
     SDO.RealEstateAgent,
     SDO.RecyclingCenter,
     SDO.SelfStorage,
     SDO.ShoppingCenter,
     SDO.SportsActivityLocation,
@@ -1849,29 +1856,29 @@
     SDO.Hospital,
     SDO.MedicalClinic,
     SDO.Pharmacy,
     SDO.Physician,
     SDO.VeterinaryCare,
     SDO.NGO,
     SDO.NewsMediaOrganization,
-    #SDO.OnlineBusiness,
-    #SDO.OnlineStore,
+    # SDO.OnlineBusiness,
+    # SDO.OnlineStore,
     SDO.PerformingGroup,
     SDO.DanceGroup,
     SDO.MusicGroup,
     SDO.TheaterGroup,
-    #SDO.PoliticalParty,
+    # SDO.PoliticalParty,
     SDO.Project,
     SDO.FundingAgency,
     SDO.ResearchProject,
     SDO.ResearchOrganization,
-    #SDO.SearchRescueOrganization,
+    # SDO.SearchRescueOrganization,
     SDO.SportsOrganization,
     SDO.SportsTeam,
-    SDO.WorkersUnion
+    SDO.WorkersUnion,
 ]
 sdo_place = [
     SDO.Place,
     SDO.Accommodation,
     SDO.Apartment,
     SDO.CampingPitch,
     SDO.House,
@@ -1943,15 +1950,15 @@
     SDO.Volcano,
     SDO.LandmarksOrHistoricalBuildings,
     SDO.LocalBusiness,
     SDO.Residence,
     SDO.ApartmentComplex,
     SDO.GatedResidenceCommunity,
     SDO.TouristAttraction,
-    SDO.TouristDestination
+    SDO.TouristDestination,
 ]
 sdo_event = [
     SDO.Event,
     SDO.BusinessEvent,
     SDO.ChildrensEvent,
     SDO.ComedyEvent,
     SDO.CourseInstance,
@@ -1979,15 +1986,15 @@
     SDO.UserComments,
     SDO.UserDownloads,
     SDO.UserLikes,
     SDO.UserPageVisits,
     SDO.UserPlays,
     SDO.UserPlusOnes,
     SDO.UserTweets,
-    SDO.VisualArtsEvent
+    SDO.VisualArtsEvent,
 ]
 sdo_item = [
     SDO.CreativeWork,
     SDO.AmpStory,
     SDO.ArchiveComponent,
     SDO.Article,
     SDO.AdvertiserContentArticle,
@@ -2008,15 +2015,15 @@
     SDO.DiscussionForumPosting,
     SDO.TechArticle,
     SDO.APIReference,
     SDO.Atlas,
     SDO.Blog,
     SDO.Book,
     SDO.Audiobook,
-    #SDO.Certification,
+    # SDO.Certification,
     SDO.Chapter,
     SDO.Claim,
     SDO.Clip,
     SDO.MovieClip,
     SDO.RadioClip,
     SDO.TVClip,
     SDO.VideoGameClip,
@@ -2074,33 +2081,33 @@
     SDO.HowToStep,
     SDO.HowToTip,
     SDO.HyperToc,
     SDO.HyperTocEntry,
     SDO.LearningResource,
     SDO.Course,
     SDO.Quiz,
-    #SDO.Syllabus,
+    # SDO.Syllabus,
     SDO.Legislation,
     SDO.LegislationObject,
     SDO.Manuscript,
     SDO.Map,
     SDO.MathSolver,
     SDO.MediaObject,
-    #SDO['3DModel'], # Alternative notation due to number
+    # SDO['3DModel'], # Alternative notation due to number
     SDO.AmpStory,
     SDO.AudioObject,
     SDO.AudioObjectSnapshot,
     SDO.Audiobook,
     SDO.DataDownload,
     SDO.ImageObject,
     SDO.Barcode,
     SDO.ImageObjectSnapshot,
     SDO.LegislationObject,
     SDO.MusicVideoObject,
-    #SDO.TextObject,
+    # SDO.TextObject,
     SDO.VideoObject,
     SDO.VideoObjectSnapshot,
     SDO.MediaReviewItem,
     SDO.Menu,
     SDO.MenuSection,
     SDO.Message,
     SDO.EmailMessage,
@@ -2163,9 +2170,9 @@
     SDO.WebPageElement,
     SDO.SiteNavigationElement,
     SDO.Table,
     SDO.WPAdBlock,
     SDO.WPFooter,
     SDO.WPHeader,
     SDO.WPSideBar,
-    SDO.WebSite
+    SDO.WebSite,
 ]
```

## Comparing `nfdi4culture-0.2.dist-info/METADATA` & `nfdi4culture-0.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfdi4culture
-Version: 0.2
+Version: 0.3
 Summary: This package provides a Python interface to the NFDI4Culture infrastructure.
 Home-page: https://nfdi4culture.de/
 License: MIT
 Author: Etienne Posthumus
 Author-email: ep@epoz.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `nfdi4culture-0.2.dist-info/RECORD` & `nfdi4culture-0.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-nfdi4culture/__init__.py,sha256=VGQ-yLEuTXeuOFoxGWnClhHPdPCuyauUIzplgy7Aw-A,20
+nfdi4culture/__init__.py,sha256=G8LN064KT_A-KF1dzoCw4nJ1MLQH25m4dS1UXJsa8UY,55
 nfdi4culture/cto.ttl,sha256=WJdSo5oFonJzQQ_ZdqQFdKd0qsHNfCVjwgY1mn758f8,38806
-nfdi4culture/cto1.py,sha256=3SLdacJWXVHgGwZFygB-dK6vk9QnFE7xYQMe5Tq8d8c,61101
+nfdi4culture/cto1.py,sha256=bEtlwFF8lfrp1Syl9YbQnpX6_lRvxDPt8nFt2jykLx8,62306
 nfdi4culture/helpers.py,sha256=8AViLLogvQ3EJekTty0_adZfcfVumDxuvAFEOp2Z9Pw,118
+nfdi4culture/marc.py,sha256=qslOtQyx2lvv-b4mhUNKm20C_iObGMAIGEFn9luMhyE,4300
 nfdi4culture/ontology.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nfdi4culture/schema.ttl,sha256=dm3hoKrEkRcm05rNkN7pKJ2T76nz0OGMU1ualzMj6kY,239711
-nfdi4culture-0.2.dist-info/METADATA,sha256=GPtZef-lVe2P5GatVe-g607JeNgZvwi9Dy7Nd9Cwk_w,2013
-nfdi4culture-0.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-nfdi4culture-0.2.dist-info/RECORD,,
+nfdi4culture-0.3.dist-info/LICENSE.txt,sha256=9RDDwR-AzNwoNKlyGAjkJlgWhTiGY3TKZ_w38NoXs8c,1100
+nfdi4culture-0.3.dist-info/METADATA,sha256=KvGqcH-svdGjp_2HJ4-iG1IpwilBcDzv07i1Bl0yhqI,2013
+nfdi4culture-0.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+nfdi4culture-0.3.dist-info/RECORD,,
```

