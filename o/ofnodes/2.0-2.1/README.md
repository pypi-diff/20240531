# Comparing `tmp/ofnodes-2.0.tar.gz` & `tmp/ofnodes-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-2.0.tar", max compression
+gzip compressed data, was "ofnodes-2.1.tar", max compression
```

## Comparing `ofnodes-2.0.tar` & `ofnodes-2.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-2.0/LICENSE
--rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-2.0/README.md
--rw-r--r--   0        0        0      588 2024-05-11 15:26:44.285220 ofnodes-2.0/pyproject.toml
--rw-r--r--   0        0        0     1488 2024-04-25 04:48:44.846592 ofnodes-2.0/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 02:55:30.992047 ofnodes-2.0/src/ofnodes/components/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-2.0/src/ofnodes/components/nodes/__init__ copy.py
--rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-2.0/src/ofnodes/components/nodes/__init__.py
--rw-r--r--   0        0        0     2712 2024-05-11 14:42:17.923628 ofnodes-2.0/src/ofnodes/components/nodes/descriptors.py
--rw-r--r--   0        0        0      838 2024-05-11 14:41:55.031803 ofnodes-2.0/src/ofnodes/components/nodes/mixins.py
--rw-r--r--   0        0        0        0 2024-04-23 17:49:14.794379 ofnodes-2.0/src/ofnodes/components/structures/__init__.py
--rw-r--r--   0        0        0     9137 2024-05-11 15:14:12.690257 ofnodes-2.0/src/ofnodes/components/structures/descriptors.py
--rw-r--r--   0        0        0    19197 2024-05-11 15:11:36.999269 ofnodes-2.0/src/ofnodes/components/structures/mixins.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-2.0/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     1557 2024-05-11 16:24:33.683641 ofnodes-2.0/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-2.0/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-30 21:45:59.484524 ofnodes-2.0/src/ofnodes/sorting/__init__.py
--rw-r--r--   0        0        0    11004 2024-05-11 15:14:52.185997 ofnodes-2.0/src/ofnodes/sorting/mixins.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-2.0/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0     3961 2024-05-09 21:36:54.532398 ofnodes-2.0/src/ofnodes/structures/randomaccessarray.py
--rw-r--r--   0        0        0     4872 2024-05-10 20:24:17.377084 ofnodes-2.0/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     2139 2024-04-26 14:35:49.613667 ofnodes-2.0/src/ofnodes/structures/stack.py
--rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 ofnodes-2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-2.1/LICENSE
+-rw-r--r--   0        0        0     3051 2024-05-29 03:59:32.240332 ofnodes-2.1/README.md
+-rw-r--r--   0        0        0      588 2024-05-30 02:45:09.898673 ofnodes-2.1/pyproject.toml
+-rw-r--r--   0        0        0     1643 2024-05-29 03:59:32.240332 ofnodes-2.1/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:55:30.992047 ofnodes-2.1/src/ofnodes/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-2.1/src/ofnodes/components/nodes/__init__ copy.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-2.1/src/ofnodes/components/nodes/__init__.py
+-rw-r--r--   0        0        0     2712 2024-05-11 16:31:08.229905 ofnodes-2.1/src/ofnodes/components/nodes/descriptors.py
+-rw-r--r--   0        0        0      838 2024-05-11 16:31:08.229905 ofnodes-2.1/src/ofnodes/components/nodes/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:49:14.794379 ofnodes-2.1/src/ofnodes/components/structures/__init__.py
+-rw-r--r--   0        0        0     9137 2024-05-11 16:31:08.229905 ofnodes-2.1/src/ofnodes/components/structures/descriptors.py
+-rw-r--r--   0        0        0    20500 2024-05-30 01:29:01.503753 ofnodes-2.1/src/ofnodes/components/structures/mixins.py
+-rw-r--r--   0        0        0      247 2024-05-29 03:59:32.240332 ofnodes-2.1/src/ofnodes/logging_config.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-2.1/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     1557 2024-05-16 08:50:30.077281 ofnodes-2.1/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-2.1/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-30 21:45:59.484524 ofnodes-2.1/src/ofnodes/sorting/__init__.py
+-rw-r--r--   0        0        0    15375 2024-05-30 02:40:31.509537 ofnodes-2.1/src/ofnodes/sorting/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-2.1/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0     4401 2024-05-29 17:14:20.199038 ofnodes-2.1/src/ofnodes/structures/randomaccessarray.py
+-rw-r--r--   0        0        0     7661 2024-05-30 02:27:10.559411 ofnodes-2.1/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     2139 2024-04-26 14:35:49.613667 ofnodes-2.1/src/ofnodes/structures/stack.py
+-rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 ofnodes-2.1/PKG-INFO
```

### Comparing `ofnodes-2.0/LICENSE` & `ofnodes-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofnodes-2.0/README.md` & `ofnodes-2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -50,9 +50,23 @@
 ```
 For more usage examples, please refer to the [Documentation][1]
 
 ## Documentation
 For detailed usage information , API reference, and code examples,
 please refer to the [Documentation][1].
 
+## Configuring Logging
+
+To configure logging for the my_package library, you can use the `configure_logging` function:
+
+```python
+from ofnodes.structures.randomaccessarray import RandomAccessArray
+
+# Configure logging to display debug messages
+ofnodes.configure_logging(level=logging.DEBUG)
+
+# Now you can use the library, and it will produce log output
+raarray = ofnodes.RandomAccessArray([8, 2, 6, 4, 5])
+raarray.index_based_insertion_sort()
+
 
 [1]: https://robert-portelli.github.io/ofnodes/
```

### Comparing `ofnodes-2.0/pyproject.toml` & `ofnodes-2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "2.0"
+version = "2.1"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-2.0/src/ofnodes/__init__.py` & `ofnodes-2.1/src/ofnodes/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 __docformat__ = "restructuredtext"
 
-
+import logging
 from ofnodes.nodes.singlynode import SinglyNode
 from ofnodes.structures.singlylinkedlist import SinglyLinkedList
+from ofnodes.structures.randomaccessarray import RandomAccessArray
+from ofnodes.structures.stack import Stack
+
 
 
 __doc__ = """
 ofnodes - an illustration of node-based objects and algorithms in Python
 ========================================================================
 **ofnodes** is a Python Package providing examples of the Author's ability
 to implement data structures and algorithms in Python. It is not a substitute
@@ -25,8 +28,8 @@
 linked data structures. While the primary purpose of the Tail descriptor is to
 facilitate efficient management of the data structure's tail node, its implementation
 also aligns with best practices for preventing cyclic dependencies within linked data
 structures. By adhering to these design principles, the library promotes safe and
 reliable usage of linked data structures, reducing the risk of unintended cyclic
 references and associated issues.
 """
-__all__ = ['SinglyNode','SinglyLinkedList']
+__all__ = ['SinglyNode','SinglyLinkedList', 'RandomAccessArray', 'Stack']
```

### Comparing `ofnodes-2.0/src/ofnodes/components/nodes/descriptors.py` & `ofnodes-2.1/src/ofnodes/components/nodes/descriptors.py`

 * *Files identical despite different names*

### Comparing `ofnodes-2.0/src/ofnodes/components/nodes/mixins.py` & `ofnodes-2.1/src/ofnodes/components/nodes/mixins.py`

 * *Files identical despite different names*

### Comparing `ofnodes-2.0/src/ofnodes/components/structures/descriptors.py` & `ofnodes-2.1/src/ofnodes/components/structures/descriptors.py`

 * *Files identical despite different names*

### Comparing `ofnodes-2.0/src/ofnodes/components/structures/mixins.py` & `ofnodes-2.1/src/ofnodes/components/structures/mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,54 @@
 from typing import Any
 from ofnodes.nodes.singlynode import SinglyNode
 
+class CycleDetectionMixin:
+    """Mixin class providing cycle detection support for reference-based data structures.
+
+    This mixin implements Floyd's Tortoise and Hare algorithm for cycle detection in linked lists.
+
+    Attributes:
+        None
+
+    Methods:
+        reference_based_cycle_detection: Detects cycles in a reference-based data structure.
+
+    Usage:
+        This mixin can be used with classes representing reference-based data structures to detect cycles.
+
+    Example:
+        >>> sllist = SinglyLinkedList([8, 2, 6, 4, 5])
+        >>> sllist.reference_based_cycle_detection()
+        False
+        >>> setattr(sllist.head.next, '_next', sllist.head.next)
+        >>> sllist.reference_based_cycle_detection()
+        True
+    """
+
+    __slots__ = ()
+
+    def reference_based_cycle_detection(self):
+        """Detects cycles using Floyd's tortoise and hare algorithm.
+
+        Returns:
+            bool: True if a cycle is detected, False otherwise.
+
+        """
+        if self.tail.next is not None:  # tail causing cycle
+            return True
+
+        slow = self.head
+        fast = self.head.next
+        while fast and fast.next:
+            if slow == fast:
+                return True
+            slow = slow.next
+            fast = fast.next.next
+        return False
+
 class SearchMixin:
     """Mixin class providing search functionality for linked lists."""
     __slots__ = ()
     def search(self, target_data):
         """Searches each node's data in a linked list until the first occurrence of
         the target is found.
 
@@ -113,15 +157,15 @@
                 setattr(current_node, '_next', current_node.next.next)
                 return node
             current_node = current_node.next
 
         if getattr(self._tail, 'data') == self._target:
             return self.remove_tail()
 
-    def remove_head(self) -> None:
+    def remove_head(self) -> SinglyNode:
         """Removes the head node from the linked structure.
 
             Raises:
                 ValueError: If the linked structure is empty.
 
             Returns:
                 None
```

### Comparing `ofnodes-2.0/src/ofnodes/nodes/singlynode.py` & `ofnodes-2.1/src/ofnodes/nodes/singlynode.py`

 * *Files identical despite different names*

### Comparing `ofnodes-2.0/src/ofnodes/structures/randomaccessarray.py` & `ofnodes-2.1/src/ofnodes/structures/randomaccessarray.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,15 +77,23 @@
             >>> [raarray.__setitem__(i, val) for i, val in enumerate([8, 2, 6, 4, 5])]
             >>> str(raarray)
             '[8, 2, 6, 4, 5]'
         """
         return f"[{', '.join(str(item) for item in self._data)}]"
 
     def bubble_sort(self, ascending=True):
-        """
+        """Sorts the elements of the data structure using bubble sort.
+
+        This method sorts the elements of the data structure in place using the
+        bubble sort algorithm. It supports both ascending and descending order
+        based on the `ascending` parameter.
+
+        Args:
+            ascending (bool): If True, sorts the elements in ascending order.
+                If False, sorts the elements in descending order. Defaults to True.
         Examples:
             >>> raarray = RandomAccessArray(5)
             >>> [raarray.__setitem__(i, val) for i, val in enumerate([8, 2, 6, 4, 5])]
             [None, None, None, None, None]
             >>> raarray.bubble_sort()
             >>> raarray
             RandomAccessArray([2, 4, 5, 6, 8])
```

### Comparing `ofnodes-2.0/src/ofnodes/structures/stack.py` & `ofnodes-2.1/src/ofnodes/structures/stack.py`

 * *Files identical despite different names*

### Comparing `ofnodes-2.0/PKG-INFO` & `ofnodes-2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 2.0
+Version: 2.1
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -62,9 +62,23 @@
 ```
 For more usage examples, please refer to the [Documentation][1]
 
 ## Documentation
 For detailed usage information , API reference, and code examples,
 please refer to the [Documentation][1].
 
+## Configuring Logging
+
+To configure logging for the my_package library, you can use the `configure_logging` function:
+
+```python
+from ofnodes.structures.randomaccessarray import RandomAccessArray
+
+# Configure logging to display debug messages
+ofnodes.configure_logging(level=logging.DEBUG)
+
+# Now you can use the library, and it will produce log output
+raarray = ofnodes.RandomAccessArray([8, 2, 6, 4, 5])
+raarray.index_based_insertion_sort()
+
 
 [1]: https://robert-portelli.github.io/ofnodes/
```

