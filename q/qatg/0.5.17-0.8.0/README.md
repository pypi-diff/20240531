# Comparing `tmp/qatg-0.5.17.tar.gz` & `tmp/qatg-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qatg-0.5.17.tar", last modified: Tue Sep 27 09:54:19 2022, max compression
+gzip compressed data, was "dist/qatg-0.8.0.tar", last modified: Fri May 31 09:55:24 2024, max compression
```

## Comparing `qatg-0.5.17.tar` & `qatg-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)        0 2022-09-27 09:54:19.830623 qatg-0.5.17/
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)      240 2022-09-27 09:54:19.830623 qatg-0.5.17/PKG-INFO
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)     2885 2022-09-22 20:03:55.000000 qatg-0.5.17/README.md
-drwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)        0 2022-09-27 09:54:19.791623 qatg-0.5.17/qatg/
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)      423 2022-09-27 09:04:28.000000 qatg-0.5.17/qatg/__init__.py
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)     8474 2022-09-27 09:01:46.000000 qatg-0.5.17/qatg/qatgConfiguration.py
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)     1297 2022-09-27 08:51:50.000000 qatg-0.5.17/qatg/qatgFault.py
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)    10570 2022-09-27 09:02:55.000000 qatg-0.5.17/qatg/qatgMain.py
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)     1291 2022-09-27 09:04:14.000000 qatg-0.5.17/qatg/qatgUtil.py
-drwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)        0 2022-09-27 09:54:19.823623 qatg-0.5.17/qatg.egg-info/
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)      240 2022-09-27 09:54:19.000000 qatg-0.5.17/qatg.egg-info/PKG-INFO
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)      262 2022-09-27 09:54:19.000000 qatg-0.5.17/qatg.egg-info/SOURCES.txt
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)        1 2022-09-27 09:54:19.000000 qatg-0.5.17/qatg.egg-info/dependency_links.txt
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)       73 2022-09-27 09:54:19.000000 qatg-0.5.17/qatg.egg-info/requires.txt
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)        5 2022-09-27 09:54:19.000000 qatg-0.5.17/qatg.egg-info/top_level.txt
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)      140 2022-09-27 09:54:19.833619 qatg-0.5.17/setup.cfg
--rwxrwxrwx   0 martiansheep  (1000) martiansheep  (1000)      476 2022-09-27 07:26:22.000000 qatg-0.5.17/setup.py
+drwxr-xr-x   0 R11943177  (1106) lads_cmli_group   (502)        0 2024-05-31 09:55:24.000000 qatg-0.8.0/
+drwxr-xr-x   0 R11943177  (1106) lads_cmli_group   (502)        0 2024-05-31 09:55:24.000000 qatg-0.8.0/qatg/
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)      411 2024-05-31 09:44:11.000000 qatg-0.8.0/qatg/__init__.py
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)     8631 2024-05-31 09:44:11.000000 qatg-0.8.0/qatg/qatgConfiguration.py
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)     1297 2024-05-31 04:09:11.000000 qatg-0.8.0/qatg/qatgFault.py
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)    11460 2024-05-31 09:44:11.000000 qatg-0.8.0/qatg/qatgMain.py
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)     1736 2024-05-31 04:09:11.000000 qatg-0.8.0/qatg/qatgUtil.py
+drwxr-xr-x   0 R11943177  (1106) lads_cmli_group   (502)        0 2024-05-31 09:55:24.000000 qatg-0.8.0/qatg.egg-info/
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)    15141 2024-05-31 09:55:24.000000 qatg-0.8.0/qatg.egg-info/PKG-INFO
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)      274 2024-05-31 09:55:24.000000 qatg-0.8.0/qatg.egg-info/SOURCES.txt
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)        1 2024-05-31 09:55:24.000000 qatg-0.8.0/qatg.egg-info/dependency_links.txt
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)       91 2024-05-31 09:55:24.000000 qatg-0.8.0/qatg.egg-info/requires.txt
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)        5 2024-05-31 09:55:24.000000 qatg-0.8.0/qatg.egg-info/top_level.txt
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)     1563 2024-05-31 09:44:19.000000 qatg-0.8.0/LICENSE.txt
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)    13627 2024-05-31 09:44:11.000000 qatg-0.8.0/README.md
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)      282 2024-05-31 09:55:24.000000 qatg-0.8.0/setup.cfg
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)      623 2024-05-31 09:55:14.000000 qatg-0.8.0/setup.py
+-rw-r--r--   0 R11943177  (1106) lads_cmli_group   (502)    15141 2024-05-31 09:55:24.000000 qatg-0.8.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `qatg-0.5.17/qatg/qatgConfiguration.py` & `qatg-0.8.0/qatg/qatgConfiguration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import random
 import numpy as np
 from math import ceil
 from scipy.stats import chi2, ncx2
-from qiskit import Aer
-from qiskit import execute
 from qiskit import QuantumRegister, ClassicalRegister, QuantumCircuit
+
 import qiskit.circuit.library as qGate
 from qiskit.circuit.gate import Gate
-from qiskit.providers.aer.noise import NoiseModel
-from qiskit.providers.aer.noise.errors import standard_errors, ReadoutError
 
-# import sutff
+from qiskit import transpile
+from qiskit_aer import AerSimulator
+from qiskit_aer.noise import NoiseModel
+from qiskit_aer.noise.errors import standard_errors, ReadoutError
+
 import sys
 import os.path as osp
 sys.path.append(osp.dirname(osp.abspath(__file__)))
 
 from qatgUtil import *
 
 random.seed(114514)
@@ -24,15 +25,15 @@
 	def __init__(self, circuitSetup: dict, simulationSetup: dict, faultObject):
 		# circuitSetup: circuitSize, basisGateSet, quantumRegisterName, classicalRegisterName, circuitInitializedStates
 		
 		self.circuitSize = circuitSetup['circuitSize']
 		self.basisGateSet = circuitSetup['basisGateSet']
 		self.basisGateSetString = circuitSetup['basisGateSetString']
 		self.circuitInitializedStates = circuitSetup['circuitInitializedStates']
-		self.backend = Aer.get_backend('qasm_simulator')
+		self.backend = AerSimulator()
 
 		self.oneQubitErrorProb = simulationSetup['oneQubitErrorProb']
 		self.twoQubitErrorProb = simulationSetup['twoQubitErrorProb']
 		self.zeroReadoutErrorProb = simulationSetup['zeroReadoutErrorProb']
 		self.oneReadoutErrorProb = simulationSetup['oneReadoutErrorProb']
 
 		self.targetAlpha = simulationSetup['targetAlpha']
@@ -54,26 +55,26 @@
 		self.faultfreeDistribution = []
 		self.faultyDistribution = []
 		self.repetition = np.nan
 		self.boundary = np.nan
 		self.simulatedOverkill = np.nan
 		self.simulatedTestescape = np.nan
 		self.cktDepth = np.nan
-		self.effectSize = np.nan
+		self.OnestateFidelity = np.nan
 
 		self.noiseModel = self.getNoiseModel()
 
 	def __str__(self):
 		rt = ""
 		rt += "Target fault: { " + str(self.faultObject) + " }\n"
 		rt += "Length: " + str(self.cktDepth)
 		rt += "\tRepetition: " + str(self.repetition)
 		rt += "\tCost: " + str(self.cktDepth * self.repetition) + "\n"
 		rt += "Chi-Value boundary: " + str(self.boundary) + "\n"
-		rt += "Effect Size: " + str(self.effectSize) + "\n"
+		rt += "State Fidelity: " + str(self.OnestateFidelity) + "\n"
 		rt += "Overkill: "+ str(self.simulatedOverkill)
 		rt += "\tTest Escape: " + str(self.simulatedTestescape) + "\n"
 		# rt += "Circuit: \n" + str(self.faultfreeQCKT)
 
 		return rt
 
 	def getNoiseModel(self):
@@ -86,17 +87,17 @@
 		noiseModel = NoiseModel()
 		noiseModel.add_all_qubit_quantum_error(oneQubitError, self.basisGateSetString)
 		noiseModel.add_all_qubit_quantum_error(twoQubitError, ['cx'])
 		noiseModel.add_all_qubit_readout_error(qubitReadoutError)
 
 		return noiseModel
 
-	def setTemplate(self, template, effectSize):
+	def setTemplate(self, template, OnestateFidelity):
 		# template itself is faultfree
-		self.effectSize = effectSize
+		self.OnestateFidelity = OnestateFidelity
 
 		qbIndexes = self.faultObject.getQubits()
 
 		for gates in template:
 			# in template, a list for seperate qubits and a gate for all qubits
 			if isinstance(gates, list):
 				for k in range(len(gates)):
@@ -110,34 +111,35 @@
 				if self.faultObject.isSameGateType(gates):
 					self.faultyQCKT.append(self.faultObject.createFaultyGate(gates), qbIndexes)
 				else:
 					self.faultyQCKT.append(gates, qbIndexes)
 			else:
 				raise TypeError(f"Unknown object \"{gates}\" in template")
 
-			for qb in qbIndexes:
-				self.faultfreeQCKT.append(qGate.Barrier(qb))
-				self.faultyQCKT.append(qGate.Barrier(qb))
+			self.faultfreeQCKT.append(qGate.Barrier(len(qbIndexes)), qbIndexes)
+			self.faultyQCKT.append(qGate.Barrier(len(qbIndexes)), qbIndexes)
 
 		self.faultfreeQCKT.measure(self.quantumRegister, self.classicalRegister)
 		self.faultyQCKT.measure(self.quantumRegister, self.classicalRegister)
 
 		self.cktDepth = len(template)
 
 		return
 
 	def simulate(self):
-		simulateJob = execute(self.faultfreeQCKT, self.backend, noise_model = self.noiseModel, shots = self.simulationShots)
+		new_circuit = transpile(self.faultfreeQCKT, self.backend)
+		simulateJob = self.backend.run(new_circuit, noise_model = self.noiseModel, seed_simulator = 1, shots = self.simulationShots)
 		counts = simulateJob.result().get_counts()
 		self.faultfreeDistribution = [0] * (2 ** self.circuitSize)
 		for k in counts:
 			self.faultfreeDistribution[int(k, 2)] = counts[k]
 		self.faultfreeDistribution = np.array(self.faultfreeDistribution / np.sum(self.faultfreeDistribution))
 
-		simulateJob = execute(self.faultyQCKT, self.backend, noise_model = self.noiseModel, shots = self.simulationShots)
+		new_circuit = transpile(self.faultyQCKT, self.backend)
+		simulateJob = self.backend.run(new_circuit, noise_model = self.noiseModel, seed_simulator = 1, shots = self.simulationShots)
 		counts = simulateJob.result().get_counts()
 		self.faultyDistribution = [0] * (2 ** self.circuitSize)
 		for k in counts:
 			self.faultyDistribution[int(k, 2)] = counts[k]
 		self.faultyDistribution = np.array(self.faultyDistribution / np.sum(self.faultyDistribution))
 
 		self.repetition, self.boundary = self.calRepetition()
@@ -148,15 +150,17 @@
 		return
 
 	def calRepetition(self):
 		if self.faultfreeDistribution.shape != self.faultyDistribution.shape:
 			raise ValueError('input shape not consistency')
 
 		degreeOfFreedom = self.faultfreeDistribution.shape[0] - 1
+
 		effectSize = qatgCalEffectSize(self.faultyDistribution, self.faultfreeDistribution)
+		
 		lowerBoundEffectSize = 0.8 if effectSize > 0.8 else effectSize
 
 		chi2Value = chi2.ppf(self.targetAlpha, degreeOfFreedom)
 		repetition = ceil(chi2Value / (lowerBoundEffectSize ** 2))
 		nonCentrality = repetition * (effectSize ** 2)
 		nonChi2Value = ncx2.ppf(1 - self.targetBeta, degreeOfFreedom, nonCentrality)
 		while nonChi2Value < chi2Value:
@@ -211,8 +215,8 @@
 				testEscape += 1
 
 		return testEscape / self.testSampleTime
 
 	@property
 	def circuit(self):
 		return self.faultfreeQCKT
-	
+
```

### Comparing `qatg-0.5.17/qatg/qatgFault.py` & `qatg-0.8.0/qatg/qatgFault.py`

 * *Files identical despite different names*

### Comparing `qatg-0.5.17/qatg/qatgMain.py` & `qatg-0.8.0/qatg/qatgMain.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import numpy as np
 from numbers import Number
 from copy import deepcopy
 from qiskit import transpile
-from qiskit import QuantumRegister, ClassicalRegister, QuantumCircuit
+from qiskit import QuantumCircuit
 from qiskit.circuit import Parameter
 import qiskit.circuit.library as qGate
 
-# import stuff
 import sys
 import os.path as osp
 sys.path.append(osp.dirname(osp.abspath(__file__)))
 
 from qatgFault import QATGFault
 from qatgUtil import *
 from qatgConfiguration import QATGConfiguration
 
 class QATG():
 	"""qatg main class"""
 	def __init__(self, \
-			circuitSize: int, basisGateSet: list[qGate], circuitInitializedStates: dict, \
+			circuitSize: int, basisSingleQubitGateSet: list[qGate], circuitInitializedStates: dict, \
 			quantumRegisterName: str = 'q', classicalRegisterName: str = 'c', \
 			gridSlice: int = 11, gradientDescentMaxIteration: int = 1000, \
 			gradientDescentStep: float = 0.2, gradientMeasureStep: float = 0.0001, gradientDeltaThreshold: float = 1e-8, \
-			maxTestTemplateSize: int = 50, minRequiredEffectSize: float = 3, \
+			maxTestTemplateSize: int = 50, minRequiredStateFidelity: float = 0.4,\
 			oneQubitErrorProb = 0.001, twoQubitErrorProb = 0.1, \
 			zeroReadoutErrorProb = [0.985, 0.015], oneReadoutErrorProb = [0.015, 0.985], \
 			targetAlpha: float = 0.99, targetBeta: float = 0.999, \
 			simulationShots: int = 200000, testSampleTime: int = 10000, \
 			verbose: bool = False):
 		# init + config setup
+  		#change 3 to 0.4 LEE
 		if not isinstance(circuitSize, int):
 			raise TypeError('circuitSize must be int')
 		if circuitSize <= 0:
 			raise ValueError('circuitSize must be positive')
 		self.circuitSize = circuitSize
 		
 		# list[qGate]
-		self.basisGateSet = basisGateSet
+		self.basisGateSet = basisSingleQubitGateSet
 		self.basisGateSetString = [gate.__name__[:-4].lower() for gate in self.basisGateSet]
 
 		# dict{0: [], 1: [1, 0], 2: [1, 0, 0, 0]} etc.
 		self.circuitInitializedStates = circuitInitializedStates
 
 		self.quantumRegisterName = quantumRegisterName
 		self.classicalRegisterName = classicalRegisterName
@@ -54,15 +54,15 @@
 
 		self.gridSlice = gridSlice
 		self.gradientDescentMaxIteration = gradientDescentMaxIteration
 		self.gradientDescentStep = gradientDescentStep # suggest not too big
 		self.gradientMeasureStep = gradientMeasureStep # suggest not too big
 		self.gradientDeltaThreshold = gradientDeltaThreshold
 		self.maxTestTemplateSize = maxTestTemplateSize
-		self.minRequiredEffectSize = minRequiredEffectSize
+		self.minRequiredStateFidelity = minRequiredStateFidelity
 		
 		q = QuantumCircuit(1)
 		self.qiskitParameterTheta = Parameter('theta')
 		self.qiskitParameterPhi = Parameter('phi')
 		self.qiskitParameterLambda = Parameter('lam')
 		q.u(self.qiskitParameterTheta, self.qiskitParameterPhi, self.qiskitParameterLambda, 0)
 		try:
@@ -91,16 +91,16 @@
 		configurationList = [QATGConfiguration(self.circuitSetup, self.simulationSetup, fault) for fault in faultList]
 
 		for k in range(len(faultList)):
 			fault = faultList[k]
 			if not issubclass(type(fault), QATGFault):
 				raise TypeError(f"{fault} should be subclass of QATGFault")
 			initialState = self.circuitInitializedStates[len(fault.getQubits())]
-			template, effectSize = self.generateTestTemplate(faultObject = fault, initialState = initialState)
-			configurationList[k].setTemplate(template, effectSize)
+			template, OnestateFidelity = self.generateTestTemplate(faultObject = fault, initialState = initialState)
+			configurationList[k].setTemplate(template, OnestateFidelity)
 			if simulateConfiguration:
 				configurationList[k].simulate()
 
 		return configurationList
 
 	def generateTestTemplate(self, faultObject, initialState):
 		# list of "qGates"
@@ -110,23 +110,28 @@
 
 		faultyQuantumState = deepcopy(initialState)
 		faultfreeQuantumState = deepcopy(initialState)
 
 		for _ in range(self.maxTestTemplateSize):
 			newElement, faultyQuantumState, faultfreeQuantumState = self.findNewElement(faultObject, faultyQuantumState, faultfreeQuantumState)
 			templateGateList += newElement
-			effectSize = qatgCalEffectSize(faultyQuantumState, faultfreeQuantumState)
-			self.verbosePrint(f"Current effect size: {effectSize}")
+			OnestateFidelity = qatgOnestateFidelity(faultyQuantumState, faultfreeQuantumState)
+			self.verbosePrint(f"Current state Fidelity: {OnestateFidelity}")
 			self.verbosePrint("")
-			if effectSize > self.minRequiredEffectSize:
+			if OnestateFidelity < self.minRequiredStateFidelity: # > to < LEE
+				newElement, faultyQuantumState, faultfreeQuantumState = self.findNewElement(faultObject, faultyQuantumState, faultfreeQuantumState, True)
+				templateGateList += newElement
+				OnestateFidelity = qatgOnestateFidelity(faultyQuantumState, faultfreeQuantumState)
+				self.verbosePrint(f"Current state Fidelity: {OnestateFidelity}")
+				self.verbosePrint("")
 				break
 
-		return templateGateList, effectSize
+		return templateGateList, OnestateFidelity
 
-	def findNewElement(self, faultObject, faultyQuantumState, faultfreeQuantumState):
+	def findNewElement(self, faultObject, faultyQuantumState, faultfreeQuantumState, finalIteration = False):
 		# find new element
 		originalGate = faultObject.createOriginalGate()
 		faultyGateMatrix = faultObject.createFaultyGate(originalGate).to_matrix()
 		originalGateMatrix = originalGate.to_matrix()
 
 		def parameterSet2ActivationMatrix(parameterSet):
 			faultfreeGateMatrixList = [qatgU3(parameter) for parameter in parameterSet] # vertical
@@ -146,21 +151,27 @@
 			faultyActivation = np.array([1])
 			for k in range(len(faultfreeGateMatrixList)):
 				faultfreeActivation = np.kron(faultfreeGateMatrixList[k], faultfreeActivation)
 				faultyActivation = np.kron(faultyGateMatrixList[k], faultyActivation)
 			
 			return faultfreeActivation, faultyActivation
 
-		def score(parameterSet):
+		def score_state(parameterSet):
+			# parameterSet: [list of first U, list of second U, ...]
+			faultfreeActivation, faultyActivation = parameterSet2ActivationMatrix(parameterSet)
+			return 1 - qatgOnestateFidelity(
+				np.dot(np.matmul(originalGateMatrix, faultfreeActivation), faultfreeQuantumState), 
+				np.dot(np.matmul(faultyGateMatrix, faultyActivation), faultyQuantumState))
+		def score_opd(parameterSet):
 			# parameterSet: [list of first U, list of second U, ...]
 			faultfreeActivation, faultyActivation = parameterSet2ActivationMatrix(parameterSet)
 			return qatgVectorDistance(
 				np.dot(np.matmul(originalGateMatrix, faultfreeActivation), faultfreeQuantumState), 
 				np.dot(np.matmul(faultyGateMatrix, faultyActivation), faultyQuantumState))
-
+		score = score_opd if finalIteration else score_state
 		# 1. find best parameters
 		# grid search
 		qubitSize = len(faultObject.getQubits())
 		optimalParameterSet = [[0, 0, 0] for _ in range(qubitSize)]
 		for k in range(qubitSize):
 			results = []
 			for theta in np.linspace(-np.pi, np.pi, num=self.gridSlice, endpoint = True):
@@ -219,15 +230,15 @@
 		faultfreeQuantumState = np.dot(np.matmul(originalGateMatrix, faultfreeActivation), faultfreeQuantumState)
 		faultyQuantumState = np.dot(np.matmul(faultyGateMatrix, faultyActivation), faultyQuantumState)
 
 		return newElement, faultyQuantumState, faultfreeQuantumState
 
 	def U2GateSetsTranspile(self, UParameters):
 		# to gate list directly
-		resultCircuit = self.effectiveUGateCircuit.bind_parameters({ \
+		resultCircuit = self.effectiveUGateCircuit.assign_parameters({ \
 			self.qiskitParameterTheta: UParameters[0], \
 			self.qiskitParameterPhi: UParameters[1], \
 			self.qiskitParameterLambda: UParameters[2]})
 		for cktInstruction in resultCircuit.data:
 			cktInstruction.operation.params = [qatgWrapToPi(float(param)) for param in cktInstruction.operation.params]
 		return [cktInstruction.operation for cktInstruction in resultCircuit.data]
 		# return [gate for gate, _, _ in resultCircuit.data] # old version of qiskit
```

### Comparing `qatg-0.5.17/qatg/qatgUtil.py` & `qatg-0.8.0/qatg/qatgUtil.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from qiskit.quantum_info import state_fidelity,Statevector
 
 qatgINT_MIN = 1E-100
 qatgINT_MAX = 1E15
 
 def qatgU3(parameterList):
 	# theta=0, phi=0, lam=0
 	return np.array(
@@ -33,7 +34,16 @@
 	# effect size might be complex TODO
 	deltaSquare = np.square(np.abs(faultyQuantumState - faultfreeQuantumState))
 	effectSize = np.sum(deltaSquare / (np.abs(faultyQuantumState) + qatgINT_MIN))
 	effectSize = np.sqrt(effectSize)
 	if effectSize < 0.1: # why? TODO
 		effectSize = 0.1
 	return effectSize
+
+def qatgOnestateFidelity(faultyQuantumState, faultfreeQuantumState): #LEE
+	# deltaSquare = np.square(faultyQuantumState - faultfreeQuantumState)
+	# effect size might be complex TODO
+	#print((Statevector(faultfreeQuantumState)))
+	stateFidelity = state_fidelity(Statevector(faultfreeQuantumState),Statevector(faultyQuantumState),validate=True)
+	#print(effectSize)
+	return stateFidelity
+
```

