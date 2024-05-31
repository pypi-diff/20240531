# Comparing `tmp/ipmerge-0.1.0.tar.gz` & `tmp/ipmerge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipmerge-0.1.0.tar", last modified: Thu May 16 18:58:39 2024, max compression
+gzip compressed data, was "ipmerge-0.1.1.tar", last modified: Fri May 31 07:56:49 2024, max compression
```

## Comparing `ipmerge-0.1.0.tar` & `ipmerge-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,21 @@
--rw-r--r--   0        0        0     1070 2024-05-16 18:58:33.462396 ipmerge-0.1.0/LICENSE
--rw-r--r--   0        0        0      458 2024-05-16 18:58:33.462396 ipmerge-0.1.0/README.md
--rw-r--r--   0        0        0      610 2024-05-16 18:58:39.810371 ipmerge-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 18:58:33.462396 ipmerge-0.1.0/src/ipmerge/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 18:58:33.462396 ipmerge-0.1.0/src/ipmerge/address/__init__.py
--rw-r--r--   0        0        0     1606 2024-05-16 18:58:33.462396 ipmerge-0.1.0/src/ipmerge/address/address.py
--rw-r--r--   0        0        0     3462 2024-05-16 18:58:33.462396 ipmerge-0.1.0/src/ipmerge/address/address_block.py
--rw-r--r--   0        0        0     1362 2024-05-16 18:58:33.462396 ipmerge-0.1.0/src/ipmerge/address/exceptions.py
--rw-r--r--   0        0        0      720 2024-05-16 18:58:33.462396 ipmerge-0.1.0/src/ipmerge/address/ipv4.py
--rw-r--r--   0        0        0     7087 2024-05-16 18:58:33.462396 ipmerge-0.1.0/src/ipmerge/address/ipv6.py
--rw-r--r--   0        0        0     7423 2024-05-16 18:58:33.462396 ipmerge-0.1.0/src/ipmerge/ipmerge.py
--rw-r--r--   0        0        0     1857 2024-05-16 18:58:33.462396 ipmerge-0.1.0/src/ipmerge/parameters.py
--rw-r--r--   0        0        0        0 2024-05-16 18:58:33.466397 ipmerge-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      135 2024-05-16 18:58:33.466397 ipmerge-0.1.0/tests/test_ipv4.py
--rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 ipmerge-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-31 07:56:46.416036 ipmerge-0.1.1/LICENSE
+-rw-r--r--   0        0        0      458 2024-05-31 07:56:46.416036 ipmerge-0.1.1/README.md
+-rw-r--r--   0        0        0     1180 2024-05-31 07:56:49.796028 ipmerge-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 07:56:46.416036 ipmerge-0.1.1/src/ipmerge/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-31 07:56:46.416036 ipmerge-0.1.1/src/ipmerge/__main__.py
+-rw-r--r--   0        0        0       21 2024-05-31 07:56:46.416036 ipmerge-0.1.1/src/ipmerge/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-31 07:56:46.416036 ipmerge-0.1.1/src/ipmerge/address/__init__.py
+-rw-r--r--   0        0        0     1803 2024-05-31 07:56:46.416036 ipmerge-0.1.1/src/ipmerge/address/address.py
+-rw-r--r--   0        0        0     3774 2024-05-31 07:56:46.416036 ipmerge-0.1.1/src/ipmerge/address/address_block.py
+-rw-r--r--   0        0        0     1362 2024-05-31 07:56:46.416036 ipmerge-0.1.1/src/ipmerge/address/exceptions.py
+-rw-r--r--   0        0        0      720 2024-05-31 07:56:46.416036 ipmerge-0.1.1/src/ipmerge/address/ipv4.py
+-rw-r--r--   0        0        0     7517 2024-05-31 07:56:46.416036 ipmerge-0.1.1/src/ipmerge/address/ipv6.py
+-rw-r--r--   0        0        0     7804 2024-05-31 07:56:46.416036 ipmerge-0.1.1/src/ipmerge/ipmerge.py
+-rw-r--r--   0        0        0     2153 2024-05-31 07:56:46.416036 ipmerge-0.1.1/src/ipmerge/parameters.py
+-rw-r--r--   0        0        0        0 2024-05-31 07:56:46.416036 ipmerge-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2886 2024-05-31 07:56:46.416036 ipmerge-0.1.1/tests/address/test_address_block.py
+-rw-r--r--   0        0        0     1248 2024-05-31 07:56:46.416036 ipmerge-0.1.1/tests/address/test_ipv4.py
+-rw-r--r--   0        0        0     4670 2024-05-31 07:56:46.416036 ipmerge-0.1.1/tests/address/test_ipv6.py
+-rw-r--r--   0        0        0      567 2024-05-31 07:56:46.416036 ipmerge-0.1.1/tests/address/test_masks.py
+-rw-r--r--   0        0        0      873 2024-05-31 07:56:46.416036 ipmerge-0.1.1/tests/test_ipmerge.py
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 ipmerge-0.1.1/PKG-INFO
```

### Comparing `ipmerge-0.1.0/LICENSE` & `ipmerge-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipmerge-0.1.0/src/ipmerge/address/address.py` & `ipmerge-0.1.1/src/ipmerge/address/address.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,33 +9,43 @@
 _masksForPrefixes = dict[int, list[int]]()
 
 
 
 def _generateMasks(maxPrefix: int) -> list[int]:
 	masks = list[int]()
 
-	if maxPrefix >= 0:
-		masks.append(0)
+	if maxPrefix < 0:
+		raise InvalidPrefixException(maxPrefix, maxPrefix)
 	
-	for i in range(1, maxPrefix + 1):
-		masks.append(masks[i - 1] | (1 << (maxPrefix - i)))
+	masks.append(0)
 
+	if maxPrefix == 0:
+		return masks
+	
+	prefixBit = 1 << (maxPrefix - 1)
+
+	while prefixBit != 0:
+		masks.append(masks[len(masks) - 1] | prefixBit)
+		prefixBit >>= 1
+	
 	return masks
 
 def prefixToMask(maxPrefix: int, prefix: int) -> int:
+	if maxPrefix < 0:
+		raise InvalidPrefixException(prefix, maxPrefix)
 	if prefix < 0:
 		raise InvalidPrefixException(prefix)
 	
 	masks = _masksForPrefixes.get(maxPrefix)
 
 	if masks == None:
 		masks = _generateMasks(maxPrefix)
 		_masksForPrefixes[maxPrefix] = masks
 	
-	if prefix > len(masks):
+	if prefix >= len(masks):
 		raise InvalidPrefixException(prefix, maxPrefix)
 
 	return masks[prefix]
 
 
 
 class Address(SupportsInt, SupportsBytes):
```

### Comparing `ipmerge-0.1.0/src/ipmerge/address/address_block.py` & `ipmerge-0.1.1/src/ipmerge/address/address_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 		self._address = address
 		self._prefix = prefix
 		self._mask = prefixToMask(address.addressLength, prefix)
 
 		if (self._address.addressInt & (~self._mask)) != 0:		# network address isn't valid network address for the given prefix
 			raise InvalidNetworkAddressException(self._address.__str__(), self._prefix)
 	
+	def __eq__(self, value: object) -> bool:
+		if type(value) == Address_Block:
+			return self.address == value.address and self.prefix == value.prefix
+		else:
+			return False
+	
 	@property
 	def address(self):
 		return self._address
 	
 	@property
 	def prefix(self):
 		return self._prefix
@@ -54,26 +60,29 @@
 		else:
 			prefix = int(blockParts[1])
 			if prefix < 0 or prefix > address.addressLength:
 				raise InvalidPrefixException(prefix, address.addressLength, address.addressTypeText)
 
 		return Address_Block(address, prefix)
 	
-	def toString(self, compressed: bool = True, uppercase: bool = True, dualOutputMode: DualOutputMode = DualOutputMode.VALUE_DEPENDENT) -> str:
+	def toString(self, compressed: bool = True, uppercase: bool = True, dualOutputMode: DualOutputMode = DualOutputMode.VALUE_DEPENDENT, alwaysOutputPrefix: bool = False) -> str:
 		addressString: str
 		if type(self.address) == IPv6_Address:
 			addressString = self.address.toString(compressed, uppercase, dualOutputMode)
 		else:
 			addressString = self.address.toString()
 		
-		return addressString + "/" + str(self.prefix)
+		if alwaysOutputPrefix or self.prefix != self.address.addressLength:
+			return addressString + "/" + str(self.prefix)
+		else:
+			return addressString
 	
 	@staticmethod
 	def merge(block1: "Address_Block", block2: "Address_Block") -> "Address_Block | None":
-		if type(block1.address) != type(block1.address):
+		if type(block1.address) != type(block2.address):
 			return None
 		elif block1._mask == block2._mask:
 			if block1.address == block2.address:
 				if type(block1.address) == IPv6_Address:
 					block1.address.setDualAfterMerge(block1.address, block2.address)
 				return Address_Block(block1.address, block1.prefix)
```

### Comparing `ipmerge-0.1.0/src/ipmerge/address/exceptions.py` & `ipmerge-0.1.1/src/ipmerge/address/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipmerge-0.1.0/src/ipmerge/address/ipv4.py` & `ipmerge-0.1.1/src/ipmerge/address/ipv4.py`

 * *Files identical despite different names*

### Comparing `ipmerge-0.1.0/src/ipmerge/address/ipv6.py` & `ipmerge-0.1.1/src/ipmerge/address/ipv6.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 
 
 class DualOutputMode(Enum):
 	FORCE_NORMAL = 0
 	VALUE_DEPENDENT = 1
 	FORCE_DUAL = 2
 
+	@staticmethod
+	def toString(dualOutputMode: "DualOutputMode") -> str:
+		match dualOutputMode:
+			case DualOutputMode.FORCE_NORMAL: return "Force Normal"
+			case DualOutputMode.VALUE_DEPENDENT: return "Value Dependent"
+			case DualOutputMode.FORCE_DUAL: return "Force Dual"
+
+
 
 
 class IPv6Segments(list[int], SupportsInt, SupportsBytes):
 	@overload
 	def __init__(self) -> None: ...
 	@overload
 	def __init__(self, initial: bytes) -> None: ...
@@ -117,22 +125,25 @@
 	
 	@property
 	def string(self):	# for debugging
 		return self.toString()
 	
 	@staticmethod
 	def parse(string: str) -> "IPv6_Address | None":
+		if ":" not in string:
+			return None
+
 		string = string.strip().replace(" ", "")
 		
 		if string == "::":
 			return IPv6_Address(0, False)
 		
 		segments = string.split(":")
 
-		if len(segments) > 8:
+		if len(segments) > 8:	# too many segments
 			return None
 		
 		segmentList = IPv6Segments()
 		fillAt: None | int = None	# byte at which the 0-filling should start
 		dual = False
 
 		if string.startswith("::"):
@@ -151,15 +162,15 @@
 				if fillAt == None:
 					fillAt = i
 					continue
 				else:
 					return None
 			
 			if "." in segment:
-				if i != len(segments) - 1:	# not on last segment
+				if i != len(segments) - 1 or fillAt == len(segments):	# if not on last segment
 					return None
 				if len(segments) > 7:	# segment count check for a dual address
 					return None
 				dual = True
 				ipv4 = IPv4_Address.parse(segment)
 				if ipv4 != None:
 					segmentList.append((ipv4.addressInt >> 16) & 0xffff)
@@ -177,14 +188,16 @@
 				return None
 			
 			segmentList.append(segmentInt)
 
 		if type(fillAt) == int:
 			for _ in range(8 - len(segmentList)):
 				segmentList.insert(fillAt, 0)
+		elif fillAt == None and len(segmentList) != 8:
+			return None
 		
 		return IPv6_Address(segmentList, dual)
 
 	@staticmethod
 	def findLongestZeroSegmentString(segments: list[int]) -> tuple[int | None, int]:
 		maxZeros: int = 0
 		maxZerosIndex: int | None = None
```

### Comparing `ipmerge-0.1.0/src/ipmerge/ipmerge.py` & `ipmerge-0.1.1/src/ipmerge/ipmerge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from pathlib import Path
 from sys import argv, stderr, stdin, stdout
 from os import mkdir
 from typing import TextIO
 
-from address.address_block import Address_Block
-from parameters import IPMergeProgramParameters, IPMergeProgramParametersBuilder, DualOutputMode
+from .address.address_block import Address_Block
+from .parameters import IPMergeProgramParameters, IPMergeProgramParametersBuilder, DualOutputMode
 
 
 
 def _printUsage():
-	print(f"Usage: python {Path(__file__).name} [OPTIONS] INPUT_FILES...")
+	print(f"Usage: ipmerge [OPTIONS] INPUT_FILES...")
 	print("  INPUT_FILES - Files containing the CIDR blocks to be read and processed.")
 	print("                Use '-' to read from stdin.")
 
 def _printHelp():
 	_printUsage()
 	print()
 	print("Options:")
@@ -27,14 +27,16 @@
 	print("  -c, --compressed     Print addresses that allow shortening (i.e. IPv6) in shortened (compressed) format (default).")
 	print("  -f, --full           Print all addresses in full (uncompressed) format.")
 	print("  -p, --preserve       Print only dual IPv6 addresses in dual format and normal IPv6 addresses")
 	print("                         in normal format (default). Note: When a dual IPv6 address is merged with")
 	print("                         a normal IPv6 address, it becomes a normal IPv6 address.")
 	print("  -d, --dual           Force printing of IPv6 addresses in dual format.")
 	print("  -n, --normal         Force printing of IPv6 addresses in normal format.")
+	print("  -b, --block          Always output result in the CIDR block format (with explicit prefix).")
+	print("                         By default, prefix is not outputted if the block is a single (host) address.")
 	print()
 	print("Input files:")
 	print("- The input files contain CIDR blocks (in format [NETWORK_ADDRESS]/[PREFIX_LENGTH]).")
 	print("- The '/[PREFIX_LENGTH]' is optional and if missing, it is assumed that the IP is a host IP,")
 	print("    therefore a block with the maximum allowable prefix length (32 for IPv4, 128 for IPv6, ...).")
 	print("- Program exits with a failure if a network address invalid for the given prefix is encountered.")
 	print("- The '#' character serves as a line comment, anything on the line after it is ignored.")
@@ -73,14 +75,15 @@
 					case "--upper": parameters.uppercase = True
 					case "--lower": parameters.uppercase = False
 					case "--compressed": parameters.compressed = True
 					case "--full": parameters.compressed = False
 					case "--preserve": parameters.dualOutputMode = DualOutputMode.VALUE_DEPENDENT
 					case "--dual": parameters.dualOutputMode = DualOutputMode.FORCE_DUAL
 					case "--normal": parameters.dualOutputMode = DualOutputMode.FORCE_NORMAL
+					case "--block": parameters.alwaysOutputPrefix = True
 					case _:
 						stderr.write(f"Unknown option '{argument}'\n")
 						exit(1)
 			else:
 				for charIndex in range(1, len(argument)):
 					match argument[charIndex]:
 						case "h":
@@ -91,14 +94,15 @@
 						case "u": parameters.uppercase = True
 						case "l": parameters.uppercase = False
 						case "c": parameters.compressed = True
 						case "f": parameters.compressed = False
 						case "p": parameters.dualOutputMode = DualOutputMode.VALUE_DEPENDENT
 						case "d": parameters.dualOutputMode = DualOutputMode.FORCE_DUAL
 						case "n": parameters.dualOutputMode = DualOutputMode.FORCE_NORMAL
+						case "b": parameters.alwaysOutputPrefix = True
 						case _:
 							stderr.write(f"Unknown option '{argument[charIndex]}' in '{argument}'\n")
 							exit(1)
 		else:
 			parameters.inputFiles.append(argument)
 		
 		i += 1
@@ -116,16 +120,16 @@
 def readInput(fileNames : list[str]) -> dict[type, list[Address_Block]]:
 	blocks = dict[type, list[Address_Block]]()
 
 	for fileName in fileNames:
 		inputFile: TextIO = stdin if fileName == "-" else open(fileName, "rt")
 		
 		for line in inputFile:
-			line = line.split("#")[0]
-			if len(line.strip()) == 0:
+			line = line.split("#")[0].strip()
+			if len(line) == 0:
 				continue
 
 			block = Address_Block.parse(line)
 
 			blocksOfType = blocks.get(type(block.address))
 			if blocksOfType == None:
 				blocksOfType = list[Address_Block]()
@@ -164,25 +168,25 @@
 					index = 1
 
 def printOutput(output: TextIO, blockLists: dict[type, list[Address_Block]]) -> None:
 	parameters = IPMergeProgramParameters.getInstance()
 
 	for i, blocks in enumerate(blockLists.values()):
 		for block in blocks:
-			output.write(block.toString(parameters.compressed, parameters.uppercase, parameters.dualOutputMode))
+			output.write(block.toString(parameters.compressed, parameters.uppercase, parameters.dualOutputMode, parameters.alwaysOutputPrefix))
 			output.write("\n")
 		
 		if i < len(blockLists) - 1:
 			output.write("\n\n\n")
 
 
 
 
 
-def main():
+def main_inner():
 	IPMergeProgramParameters.setInstance(_parseParameters(argv))
 	parameters = IPMergeProgramParameters.getInstance()
 
 	blocks = readInput(parameters.inputFiles)
 	
 	originalBlockCount = 0
 	for block in blocks.values():
@@ -208,17 +212,21 @@
 		if parameters.verbosityLevel >= 2:
 			stderr.write("\n")
 		
 		stderr.write(f"Original block count: {originalBlockCount}.\n")
 		stderr.write(f"Merged block count: {currentSize} ({round(currentSize / float(originalBlockCount) * 100, 2)} %).\n")
 		stderr.write(f"Decrease by: {originalBlockCount - currentSize} ({round((originalBlockCount - currentSize) / float(originalBlockCount) * 100, 2)} %).\n")
 
+def main():
+	try:
+		main_inner()
+	except Exception as e:
+		stderr.write(e.__str__())
+		stderr.write("\n")
+		exit(1)
+
 
 
 
 
 if __name__ == '__main__':
-	try:
-		main()
-	except Exception as e:
-		stderr.write(e.__str__())
-		stderr.write("\n")
+	main()
```

### Comparing `ipmerge-0.1.0/PKG-INFO` & `ipmerge-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 Metadata-Version: 2.1
 Name: IPMerge
-Version: 0.1.0
+Version: 0.1.1
 Summary: Merge CIDR blocks of IPv4 and IPv6 addresses
-Author-Email: =?utf-8?q?Vojt=C4=9Bch_Kursa?= <it.vojtechkursa@gmail.com>
+Author-Email: Vojtech Kursa <it.vojtechkursa@gmail.com>
 License: MIT
+Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: System Administrators
+Classifier: Topic :: Utilities
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: Text Processing :: General
+Classifier: Natural Language :: English
+Classifier: Typing :: Typed
 Requires-Python: >=3.10
+Provides-Extra: tests
+Requires-Dist: pytest>=8.2.0; extra == "tests"
 Description-Content-Type: text/markdown
 
 # IPMerge
 
 A Python tool for merging CIDR blocks of IPv4 and IPv6 addresses.
 
 ## Features
```

