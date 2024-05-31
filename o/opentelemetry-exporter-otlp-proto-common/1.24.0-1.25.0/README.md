# Comparing `tmp/opentelemetry_exporter_otlp_proto_common-1.24.0.tar.gz` & `tmp/opentelemetry_exporter_otlp_proto_common-1.25.0.tar.gz`

## Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0.tar` & `opentelemetry_exporter_otlp_proto_common-1.25.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/__init__.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/_log_encoder.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/metrics_encoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/py.typed
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/trace_encoder.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/version.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/_internal/__init__.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/_internal/_log_encoder/__init__.py
--rw-r--r--   0        0        0    13522 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/_internal/metrics_encoder/__init__.py
--rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/_internal/trace_encoder/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/tests/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/tests/test_backoff.py
--rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/tests/test_log_encoder.py
--rw-r--r--   0        0        0    39009 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/tests/test_metrics_encoder.py
--rw-r--r--   0        0        0    16663 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/tests/test_trace_encoder.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/LICENSE
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/README.rst
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/pyproject.toml
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.24.0/PKG-INFO
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/__init__.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/_log_encoder.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/metrics_encoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/py.typed
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/trace_encoder.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/version.py
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/_internal/__init__.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/_internal/_log_encoder/__init__.py
+-rw-r--r--   0        0        0    13522 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/_internal/metrics_encoder/__init__.py
+-rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/_internal/trace_encoder/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/tests/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/tests/test_backoff.py
+-rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/tests/test_log_encoder.py
+-rw-r--r--   0        0        0    39009 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/tests/test_metrics_encoder.py
+-rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/tests/test_trace_encoder.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/LICENSE
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/README.rst
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/pyproject.toml
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.25.0/PKG-INFO
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/__init__.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/_log_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/_log_encoder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/metrics_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/metrics_encoder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/trace_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/trace_encoder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/version.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.24.0"
+__version__ = "1.25.0"
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/_internal/__init__.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/_internal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,17 +102,18 @@
 
 def _encode_attributes(
     attributes: Attributes,
 ) -> Optional[List[PB2KeyValue]]:
     if attributes:
         pb2_attributes = []
         for key, value in attributes.items():
+            # pylint: disable=broad-exception-caught
             try:
                 pb2_attributes.append(_encode_key_value(key, value))
-            except Exception as error:  # pylint: disable=broad-except
+            except Exception as error:
                 _logger.exception(error)
     else:
         pb2_attributes = None
     return pb2_attributes
 
 
 def _get_resource_data(
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/_internal/_log_encoder/__init__.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/_internal/_log_encoder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 def encode_logs(batch: Sequence[LogData]) -> ExportLogsServiceRequest:
     return ExportLogsServiceRequest(resource_logs=_encode_resource_logs(batch))
 
 
 def _encode_log(log_data: LogData) -> PB2LogRecord:
     return PB2LogRecord(
         time_unix_nano=log_data.log_record.timestamp,
+        observed_time_unix_nano=log_data.log_record.observed_timestamp,
         span_id=_encode_span_id(log_data.log_record.span_id),
         trace_id=_encode_trace_id(log_data.log_record.trace_id),
         flags=int(log_data.log_record.trace_flags),
         body=_encode_value(log_data.log_record.body),
         severity_text=log_data.log_record.severity_text,
         attributes=_encode_attributes(log_data.log_record.attributes),
         dropped_attributes_count=log_data.log_record.dropped_attributes,
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/_internal/metrics_encoder/__init__.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/_internal/metrics_encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/src/opentelemetry/exporter/otlp/proto/common/_internal/trace_encoder/__init__.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/src/opentelemetry/exporter/otlp/proto/common/_internal/trace_encoder/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,35 +13,33 @@
 # limitations under the License.
 
 import logging
 from collections import defaultdict
 from typing import List, Optional, Sequence
 
 from opentelemetry.exporter.otlp.proto.common._internal import (
-    _encode_trace_id,
-    _encode_span_id,
-    _encode_instrumentation_scope,
     _encode_attributes,
+    _encode_instrumentation_scope,
     _encode_resource,
+    _encode_span_id,
+    _encode_trace_id,
 )
 from opentelemetry.proto.collector.trace.v1.trace_service_pb2 import (
     ExportTraceServiceRequest as PB2ExportTraceServiceRequest,
 )
 from opentelemetry.proto.trace.v1.trace_pb2 import (
-    ScopeSpans as PB2ScopeSpans,
-)
-from opentelemetry.proto.trace.v1.trace_pb2 import (
     ResourceSpans as PB2ResourceSpans,
 )
+from opentelemetry.proto.trace.v1.trace_pb2 import ScopeSpans as PB2ScopeSpans
 from opentelemetry.proto.trace.v1.trace_pb2 import Span as PB2SPan
+from opentelemetry.proto.trace.v1.trace_pb2 import SpanFlags as PB2SpanFlags
 from opentelemetry.proto.trace.v1.trace_pb2 import Status as PB2Status
 from opentelemetry.sdk.trace import Event, ReadableSpan
-from opentelemetry.trace import Link
-from opentelemetry.trace import SpanKind
-from opentelemetry.trace.span import SpanContext, TraceState, Status
+from opentelemetry.trace import Link, SpanKind
+from opentelemetry.trace.span import SpanContext, Status, TraceState
 
 # pylint: disable=E1101
 _SPAN_KIND_MAP = {
     SpanKind.INTERNAL: PB2SPan.SpanKind.SPAN_KIND_INTERNAL,
     SpanKind.SERVER: PB2SPan.SpanKind.SPAN_KIND_SERVER,
     SpanKind.CLIENT: PB2SPan.SpanKind.SPAN_KIND_CLIENT,
     SpanKind.PRODUCER: PB2SPan.SpanKind.SPAN_KIND_PRODUCER,
@@ -100,14 +98,21 @@
                 schema_url=sdk_resource.schema_url,
             )
         )
 
     return pb2_resource_spans
 
 
+def _span_flags(parent_span_context: Optional[SpanContext]) -> int:
+    flags = PB2SpanFlags.SPAN_FLAGS_CONTEXT_HAS_IS_REMOTE_MASK
+    if parent_span_context and parent_span_context.is_remote:
+        flags |= PB2SpanFlags.SPAN_FLAGS_CONTEXT_IS_REMOTE_MASK
+    return flags
+
+
 def _encode_span(sdk_span: ReadableSpan) -> PB2SPan:
     span_context = sdk_span.get_span_context()
     return PB2SPan(
         trace_id=_encode_trace_id(span_context.trace_id),
         span_id=_encode_span_id(span_context.span_id),
         trace_state=_encode_trace_state(span_context.trace_state),
         parent_span_id=_encode_parent_id(sdk_span.parent),
@@ -118,14 +123,15 @@
         attributes=_encode_attributes(sdk_span.attributes),
         events=_encode_events(sdk_span.events),
         links=_encode_links(sdk_span.links),
         status=_encode_status(sdk_span.status),
         dropped_attributes_count=sdk_span.dropped_attributes,
         dropped_events_count=sdk_span.dropped_events,
         dropped_links_count=sdk_span.dropped_links,
+        flags=_span_flags(sdk_span.parent),
     )
 
 
 def _encode_events(
     events: Sequence[Event],
 ) -> Optional[List[PB2SPan.Event]]:
     pb2_events = None
@@ -148,14 +154,15 @@
         pb2_links = []
         for link in links:
             encoded_link = PB2SPan.Link(
                 trace_id=_encode_trace_id(link.context.trace_id),
                 span_id=_encode_span_id(link.context.span_id),
                 attributes=_encode_attributes(link.attributes),
                 dropped_attributes_count=link.attributes.dropped,
+                flags=_span_flags(link.context),
             )
             pb2_links.append(encoded_link)
     return pb2_links
 
 
 def _encode_status(status: Status) -> Optional[PB2Status]:
     pb2_status = None
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/tests/test_backoff.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/tests/test_backoff.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/tests/test_log_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/tests/test_log_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         )
 
     @staticmethod
     def _get_sdk_log_data() -> List[LogData]:
         log1 = LogData(
             log_record=SDKLogRecord(
                 timestamp=1644650195189786880,
+                observed_timestamp=1644650195189786881,
                 trace_id=89564621134313219400156819398935297684,
                 span_id=1312458408527513268,
                 trace_flags=TraceFlags(0x01),
                 severity_text="WARN",
                 severity_number=SeverityNumber.WARN,
                 body="Do not go gentle into that good night. Rage, rage against the dying of the light",
                 resource=SDKResource(
@@ -85,14 +86,15 @@
                 "first_name", "first_version"
             ),
         )
 
         log2 = LogData(
             log_record=SDKLogRecord(
                 timestamp=1644650249738562048,
+                observed_timestamp=1644650249738562049,
                 trace_id=0,
                 span_id=0,
                 trace_flags=TraceFlags.DEFAULT,
                 severity_text="WARN",
                 severity_number=SeverityNumber.WARN,
                 body="Cooper, this is no time for caution!",
                 resource=SDKResource({"second_resource": "CASE"}),
@@ -102,14 +104,15 @@
                 "second_name", "second_version"
             ),
         )
 
         log3 = LogData(
             log_record=SDKLogRecord(
                 timestamp=1644650427658989056,
+                observed_timestamp=1644650427658989057,
                 trace_id=271615924622795969659406376515024083555,
                 span_id=4242561578944770265,
                 trace_flags=TraceFlags(0x01),
                 severity_text="DEBUG",
                 severity_number=SeverityNumber.DEBUG,
                 body="To our galaxy",
                 resource=SDKResource({"second_resource": "CASE"}),
@@ -117,14 +120,15 @@
             ),
             instrumentation_scope=None,
         )
 
         log4 = LogData(
             log_record=SDKLogRecord(
                 timestamp=1644650584292683008,
+                observed_timestamp=1644650584292683009,
                 trace_id=212592107417388365804938480559624925555,
                 span_id=6077757853989569223,
                 trace_flags=TraceFlags(0x01),
                 severity_text="INFO",
                 severity_number=SeverityNumber.INFO,
                 body="Love is the one thing that transcends time and space",
                 resource=SDKResource(
@@ -160,14 +164,15 @@
                         PB2ScopeLogs(
                             scope=PB2InstrumentationScope(
                                 name="first_name", version="first_version"
                             ),
                             log_records=[
                                 PB2LogRecord(
                                     time_unix_nano=1644650195189786880,
+                                    observed_time_unix_nano=1644650195189786881,
                                     trace_id=_encode_trace_id(
                                         89564621134313219400156819398935297684
                                     ),
                                     span_id=_encode_span_id(
                                         1312458408527513268
                                     ),
                                     flags=int(TraceFlags(0x01)),
@@ -186,14 +191,15 @@
                             scope=PB2InstrumentationScope(
                                 name="another_name",
                                 version="another_version",
                             ),
                             log_records=[
                                 PB2LogRecord(
                                     time_unix_nano=1644650584292683008,
+                                    observed_time_unix_nano=1644650584292683009,
                                     trace_id=_encode_trace_id(
                                         212592107417388365804938480559624925555
                                     ),
                                     span_id=_encode_span_id(
                                         6077757853989569223
                                     ),
                                     flags=int(TraceFlags(0x01)),
@@ -228,14 +234,15 @@
                             scope=PB2InstrumentationScope(
                                 name="second_name",
                                 version="second_version",
                             ),
                             log_records=[
                                 PB2LogRecord(
                                     time_unix_nano=1644650249738562048,
+                                    observed_time_unix_nano=1644650249738562049,
                                     trace_id=_encode_trace_id(0),
                                     span_id=_encode_span_id(0),
                                     flags=int(TraceFlags.DEFAULT),
                                     severity_text="WARN",
                                     severity_number=SeverityNumber.WARN.value,
                                     body=_encode_value(
                                         "Cooper, this is no time for caution!"
@@ -245,14 +252,15 @@
                             ],
                         ),
                         PB2ScopeLogs(
                             scope=PB2InstrumentationScope(),
                             log_records=[
                                 PB2LogRecord(
                                     time_unix_nano=1644650427658989056,
+                                    observed_time_unix_nano=1644650427658989057,
                                     trace_id=_encode_trace_id(
                                         271615924622795969659406376515024083555
                                     ),
                                     span_id=_encode_span_id(
                                         4242561578944770265
                                     ),
                                     flags=int(TraceFlags(0x01)),
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/tests/test_metrics_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/tests/test_metrics_encoder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/tests/test_trace_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.25.0/tests/test_trace_encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             start_times[0] + (50 * 10**6),
             start_times[1] + (100 * 10**6),
             start_times[2] + (200 * 10**6),
             start_times[3] + (300 * 10**6),
         )
 
         parent_span_context = SDKSpanContext(
-            trace_id, 0x1111111111111111, is_remote=False
+            trace_id, 0x1111111111111111, is_remote=True
         )
 
         other_context = SDKSpanContext(
             trace_id, 0x2222222222222222, is_remote=False
         )
 
         span1 = SDKSpan(
@@ -248,20 +248,22 @@
                                                 PB2KeyValue(
                                                     key="key_bool",
                                                     value=PB2AnyValue(
                                                         bool_value=True
                                                     ),
                                                 ),
                                             ],
+                                            flags=0x100,
                                         )
                                     ],
                                     status=PB2Status(
                                         code=SDKStatusCode.ERROR.value,
                                         message="Example description",
                                     ),
+                                    flags=0x300,
                                 )
                             ],
                         ),
                         PB2ScopeSpans(
                             scope=PB2InstrumentationScope(
                                 name="name",
                                 version="version",
@@ -280,14 +282,15 @@
                                         3
                                     ].start_time,
                                     end_time_unix_nano=otel_spans[3].end_time,
                                     attributes=None,
                                     events=None,
                                     links=None,
                                     status={},
+                                    flags=0x100,
                                 )
                             ],
                         ),
                     ],
                 ),
                 PB2ResourceSpans(
                     resource=PB2Resource(
@@ -317,14 +320,15 @@
                                         1
                                     ].start_time,
                                     end_time_unix_nano=otel_spans[1].end_time,
                                     attributes=None,
                                     events=None,
                                     links=None,
                                     status={},
+                                    flags=0x100,
                                 ),
                                 PB2SPan(
                                     trace_id=trace_id,
                                     span_id=_encode_span_id(
                                         otel_spans[2].context.span_id
                                     ),
                                     trace_state=None,
@@ -342,14 +346,15 @@
                                                 string_value="hello_world"
                                             ),
                                         ),
                                     ],
                                     events=None,
                                     links=None,
                                     status={},
+                                    flags=0x100,
                                 ),
                             ],
                         )
                     ],
                 ),
             ]
         )
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/.gitignore` & `opentelemetry_exporter_otlp_proto_common-1.25.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/LICENSE` & `opentelemetry_exporter_otlp_proto_common-1.25.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright The OpenTelemetry Authors
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/README.rst` & `opentelemetry_exporter_otlp_proto_common-1.25.0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/pyproject.toml` & `opentelemetry_exporter_otlp_proto_common-1.25.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 license = {text = "Apache-2.0"}
 requires-python = ">=3.8"
 authors = [
   { name = "OpenTelemetry Authors", email = "cncf-opentelemetry-contributors@lists.cncf.io" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
+  "Framework :: OpenTelemetry",
+  "Framework :: OpenTelemetry :: Exporters",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-  "opentelemetry-proto == 1.24.0",
+  "opentelemetry-proto == 1.25.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-otlp-proto-common"
 
 [tool.hatch.version]
 path = "src/opentelemetry/exporter/otlp/proto/common/version.py"
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.24.0/PKG-INFO` & `opentelemetry_exporter_otlp_proto_common-1.25.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.3
 Name: opentelemetry-exporter-otlp-proto-common
-Version: 1.24.0
+Version: 1.25.0
 Summary: OpenTelemetry Protobuf encoding
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-otlp-proto-common
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: OpenTelemetry
+Classifier: Framework :: OpenTelemetry :: Exporters
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: opentelemetry-proto==1.24.0
+Requires-Dist: opentelemetry-proto==1.25.0
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Protobuf Encoding
 ===============================
 
 |pypi|
```

