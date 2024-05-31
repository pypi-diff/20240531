# Comparing `tmp/pycanum-4.2.7-cp39-cp39-win32.whl.zip` & `tmp/pycanum-5.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 395586 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat   463872 b- defN 16-Oct-18 05:03 pycanum/SysamPCI.dll
+Zip file size: 67044 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        1 b- defN 16-Oct-18 05:03 pycanum/__init__.py
--rw-rw-rw-  2.0 fat     7379 b- defN 16-Oct-18 05:03 pycanum/main.py
--rw-rw-rw-  2.0 fat   209920 b- defN 16-Oct-17 20:29 pycanum/portaudio_x86.dll
+-rw-rw-rw-  2.0 fat     4302 b- defN 24-May-21 09:44 pycanum/httpdata.py
+-rw-rw-rw-  2.0 fat    12547 b- defN 24-May-22 07:10 pycanum/main.py
 -rw-rw-rw-  2.0 fat    55808 b- defN 16-Sep-14 20:22 pycanum/pthreadVC2.dll
--rw-rw-rw-  2.0 fat    53760 b- defN 22-Aug-19 10:29 pycanum/pysysam.cp39-win32.pyd
--rw-rw-rw-  2.0 fat    22566 b- defN 22-Aug-19 11:45 pycanum-4.2.7.dist-info/LICENCE.txt
--rw-rw-rw-  2.0 fat      290 b- defN 22-Aug-19 11:45 pycanum-4.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       96 b- defN 22-Aug-19 11:45 pycanum-4.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 22-Aug-19 11:45 pycanum-4.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      865 b- defN 22-Aug-19 11:46 pycanum-4.2.7.dist-info/RECORD
-11 files, 814565 bytes uncompressed, 394140 bytes compressed:  51.6%
+-rw-rw-rw-  2.0 fat    16298 b- defN 24-Apr-25 15:55 pycanum/pycanum.py
+-rw-rw-rw-  2.0 fat    84480 b- defN 24-May-31 07:04 pycanum/sysamhttp.exe
+-rw-rw-rw-  2.0 fat    22566 b- defN 24-May-31 07:05 pycanum-5.0.0.dist-info/LICENCE.txt
+-rw-rw-rw-  2.0 fat      285 b- defN 24-May-31 07:05 pycanum-5.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-31 07:05 pycanum-5.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-31 07:05 pycanum-5.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      846 b- defN 24-May-31 07:05 pycanum-5.0.0.dist-info/RECORD
+11 files, 197233 bytes uncompressed, 65632 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
-Filename: pycanum/SysamPCI.dll
+Filename: pycanum/__init__.py
 Comment: 
 
-Filename: pycanum/__init__.py
+Filename: pycanum/httpdata.py
 Comment: 
 
 Filename: pycanum/main.py
 Comment: 
 
-Filename: pycanum/portaudio_x86.dll
+Filename: pycanum/pthreadVC2.dll
 Comment: 
 
-Filename: pycanum/pthreadVC2.dll
+Filename: pycanum/pycanum.py
 Comment: 
 
-Filename: pycanum/pysysam.cp39-win32.pyd
+Filename: pycanum/sysamhttp.exe
 Comment: 
 
-Filename: pycanum-4.2.7.dist-info/LICENCE.txt
+Filename: pycanum-5.0.0.dist-info/LICENCE.txt
 Comment: 
 
-Filename: pycanum-4.2.7.dist-info/METADATA
+Filename: pycanum-5.0.0.dist-info/METADATA
 Comment: 
 
-Filename: pycanum-4.2.7.dist-info/WHEEL
+Filename: pycanum-5.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: pycanum-4.2.7.dist-info/top_level.txt
+Filename: pycanum-5.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pycanum-4.2.7.dist-info/RECORD
+Filename: pycanum-5.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycanum/main.py

```diff
@@ -1,187 +1,366 @@
-#coding = utf-8
-# -*- coding: utf-8 -*-
-import pycanum.pysysam as sysam
-import numpy
-import math
+INSTALLED = True
 
+import requests
+import struct
+import numpy as np
+
+if INSTALLED:
+    from pycanum.httpdata import HttpData
+else:
+    from httpdata import HttpData
+
+import time
+import os
+import subprocess
+
+
+if INSTALLED:
+    PATH = os.path.dirname(__file__)+"\\"
+else:
+    PATH = "../build/Debug/"
 
-SYSAM_SP5 = 1
-SYSAM_PCI = 2
 ENTREE_CHRONO = 16
+SIGNAL_MAX_SIZE = 200000
+
 
 class Sysam:
-    def __init__(self,nom):
-        self.ouvert = False
-        self.sysamid = 0
-        if (nom=="SP5"):
-            self.sysamid = SYSAM_SP5;
-        if (nom=="PCI"):
-            self.sysamid = SYSAM_PCI;
-        self.ouvrir()
-    def ouvrir(self):
-        if self.ouvert:
-            print("CAN Sysam ouvert")
-            return
-        if (self.sysamid==0):
-            print("CAN Sysam non connu")
-            return
-        sysam.can_ouvrir(self.sysamid)
-        self.ouvert = True
+    def __init__(self,nom='SP5'):
+        os.system('start /B '+PATH+'sysamhttp.exe "http://127.0.0.1:5000/"')
+        time.sleep(0.1)
+        self.http = HttpData("http://127.0.0.1:5000/")
+        self.http.sendRequest("ouvrir")
+        self.ecrire(1,0.0,2,0.0)
+
     def fermer(self):
-        sysam.can_fermer()
-        self.ouvert = False
-    def reset(self):
-        sysam.can_reset()
+        self.http.initData()
+        self.http.sendRequest("fermer")
+        self.http.initData()
+        self.http.sendRequest("terminate")
+
+    def afficher_calibrage(self):
+        self.http.initData()
+        self.http.sendRequest("afficher_calibrage")
+
     def config_entrees(self,voies,calibres,diff=[]):
-       sysam.can_config_entrees(voies,calibres,diff)
+        self.http.initData()
+        self.http.writeInt8(len(voies))
+        for v in voies:
+            self.http.writeInt8(v)
+        self.http.writeInt8(len(calibres))
+        for c in calibres:
+            self.http.writeFloat(c)
+        self.http.writeInt8(len(diff))
+        for d in diff:
+            self.http.writeInt8(d)
+        self.http.sendRequest("config_entrees")
+
+    def activer_lecture(self,voies):
+        self.http.initData()
+        self.http.writeInt8(len(voies))
+        for v in voies:
+            self.http.writeInt8(v)
+        self.http.writeInt8(0)
+        self.http.sendRequest("activer_lecture")
+
+    def desactiver_lecture(self):
+        self.http.sendRequest("desactiver_lecture")
+
     def config_echantillon(self,techant,nbpoints):
-        sysam.can_config_echantillon(techant,nbpoints)
+        self.http.initData()
+        self.http.writeDouble(techant)
+        self.http.writeInt32(nbpoints,signed=False)
+        self.http.sendRequest("config_echantillon")
+
     def config_echantillon_permanent(self,techant,nbpoints):
-        sysam.can_config_echantillon_permanent(techant,nbpoints)
-    def config_quantification(self,quantification):
-        sysam.can_config_quantification(quantification)
+        self.http.initData()
+        self.http.writeDouble(techant)
+        self.http.writeInt32(nbpoints,signed=False)
+        self.http.sendRequest("config_echantillon_permanent")
+
     def config_trigger(self,voie,seuil,montant=1,pretrigger=1,pretriggerSouple=0,hysteresis=0):
-        sysam.can_config_trigger(0,voie,seuil,montant,pretrigger,pretriggerSouple,hysteresis)
+        self.http.initData()
+        self.http.writeInt8(0)
+        self.http.writeInt8(voie)
+        self.http.writeDouble(seuil)
+        self.http.writeInt8(montant)
+        self.http.writeInt32(pretrigger)
+        self.http.writeInt8(pretriggerSouple)
+        self.http.writeInt32(hysteresis,signed=False)
+        self.http.sendRequest("config_trigger")
+
+    
     def config_trigger_externe(self,pretrigger=1,pretriggerSouple=0):
-        sysam.can_config_trigger(1,0,0,1,pretrigger,pretriggerSouple,0)
+        self.http.initData()
+        self.http.writeInt8(1)
+        self.http.writeInt8(0)
+        self.http.writeDouble(0)
+        self.http.writeInt8(1)
+        self.http.writeInt32(pretrigger,signed=False)
+        self.http.writeInt8(pretriggerSouple)
+        self.http.writeInt32(0)
+        self.http.sendRequest("config_trigger")
+
+    def config_quantification(self,quantification):
+        self.http.initData()
+        self.http.writeInt8(quantification)
+        self.http.sendRequest("config_quantification")
+
+
+    def envoyer_signal(self,nsortie,valeurs):
+        if len(valeurs) > SIGNAL_MAX_SIZE:
+            valeurs = valeurs[0:SIGNAL_MAX_SIZE]
+        self.http.initData()
+        N = len(valeurs)
+        self.http.writeInt8(nsortie)
+        self.http.writeInt32(N,signed=False)
+        self.http.sendRequest("config_longueur_signal")
+        i = 0
+        size = 1000
+        while i < N:
+            self.http.initData()
+            self.http.writeInt8(nsortie)
+            i2 = min(i+size,N)
+            self.http.writeInt32(i2-i)
+            self.http.writeDoubleArray(valeurs[i:i2])
+            i += size
+            self.http.sendRequest("ajout_signal")
+        
+        
+
+    def config_sortie(self,nsortie,techant,valeurs,repetition=0):
+        self.envoyer_signal(nsortie,valeurs)
+        self.http.initData()
+        self.http.writeInt32(len(valeurs),signed=False)
+        self.http.writeInt32(0,signed=False)
+        self.http.sendRequest("config_longueur_signal")
+        self.http.initData()
+        self.http.writeInt8(nsortie)
+        self.http.writeDouble(techant)
+        self.http.writeInt8(repetition,signed=True)
+        self.http.sendRequest("config_sortie")
+        
+
     def acquerir(self):
-        sysam.can_acquerir()
+        self.http.initData()
+        self.http.sendRequest("acquerir")
+
     def acquerir_permanent(self):
-        sysam.can_acquerir_permanent()
+        self.http.initData()
+        self.http.sendRequest("acquerir_permanent")
+
     def lancer(self):
-        sysam.can_lancer()  
+        self.http.initData()
+        self.http.sendRequest("lancer")
+
     def lancer_permanent(self,repetition=0):
-        sysam.can_lancer_permanent(repetition)
+        self.http.initData()
+        self.http.writeInt8(repetition)
+        self.http.sendRequest("lancer_permanent")
+
+    def acquerir_avec_sorties(self,valeurs1,valeurs2):
+        if type(valeurs1)!=np.ndarray:
+            valeurs1 = np.zeros(0)
+        if type(valeurs2)!=np.ndarray:
+            valeurs2 = np.zeros(0)
+        self.envoyer_signal(1,valeurs1)
+        self.envoyer_signal(2,valeurs2)
+        self.http.initData()
+        self.http.sendRequest("acquerir_avec_sorties")
+
+    def lancer_avec_sorties(self,valeurs1,valeurs2):
+        if type(valeurs1)!=np.ndarray:
+            valeurs1 = np.zeros(0)
+        if type(valeurs2)!=np.ndarray:
+            valeurs2 = np.zeros(0)
+        self.envoyer_signal(1,valeurs1)
+        self.envoyer_signal(2,valeurs2)
+        self.http.initData()
+        self.http.sendRequest("lancer_avec_sorties")
+
     def stopper_acquisition(self):
-        sysam.can_stopper_acquisition()
-    def temps(self,reduction=1):
-        return sysam.can_temps(reduction)
+        self.http.initData()
+        self.http.sendRequest("stopper_acquisition")
+    
+
     def entrees(self,reduction=1):
-        return sysam.can_entrees(reduction)
+        self.http.initData()
+        self.http.writeInt32(reduction,signed=False)
+        self.http.sendRequest("entrees")
+        nombreEA = self.http.readInt8(signed=False)
+        nbpoints = self.http.readInt32(signed=False)
+        tensions = np.zeros((nombreEA,nbpoints),dtype=np.float64)
+        for v in range(nombreEA):
+            tensions[v] = self.http.readDoubleNdArray(nbpoints)
+        return tensions
+
     def entrees_filtrees(self,reduction=1):
-        return sysam.can_entrees_filtrees(reduction)
+        self.http.initData()
+        self.http.writeInt32(reduction,signed=False)
+        self.http.sendRequest("entrees_filtrees")
+        nombreEA = self.http.readInt8(signed=False)
+        nbpoints = self.http.readInt32(signed=False)
+        tensions = np.zeros((nombreEA,nbpoints),dtype=np.float64)
+        for v in range(nombreEA):
+            tensions[v] = self.http.readDoubleNdArray(nbpoints)
+        return tensions
+
+    def temps(self,reduction=1):
+        self.http.initData()
+        self.http.writeInt32(reduction,signed=False)
+        self.http.sendRequest("temps")
+        nombreEA = self.http.readInt8(signed=False)
+        nbpoints = self.http.readInt32(signed=False)
+        temps = np.zeros((nombreEA,nbpoints),dtype=np.float64)
+        for v in range(nombreEA):
+            temps[v] = self.http.readDoubleNdArray(nbpoints)
+        return temps
+
     def nombre_echant(self):
-        return sysam.can_nombre_echant()
+        self.http.initData()
+        self.http.sendRequest("nombre_echant")
+        nbpoints = self.http.readInt32(signed=False)
+        return nbpoints
+
     def paquet(self,premier,reduction=1):
-        if premier >=0:
-            return sysam.can_paquet(premier,reduction)
+        self.http.initData()
+        if premier>=0:
+            self.http.writeInt32(premier,signed=False)
+            self.http.writeInt32(reduction,signed=False)
+            self.http.sendRequest("paquet")
         else:
-            return sysam.can_paquet_circulaire(reduction)
+            self.http.writeInt32(reduction,signed=False)
+            self.http.sendRequest("paquet_circulaire")
+        
+        nombreEA = self.http.readInt8(signed=False)
+        nbpoints = self.http.readInt32(signed=False)
+        paquet = np.zeros((nombreEA*3,nbpoints),dtype=np.float64)
+        for v in range(nombreEA*3):
+            paquet[v] = self.http.readDoubleNdArray(nbpoints)
+        return paquet
+
     def paquet_filtrees(self,premier,reduction=1):
-        if premier >= 0:
-            return sysam.can_paquet_filtrees(premier,reduction)
+        self.http.initData()
+        if premier>=0:
+            self.http.writeInt32(premier,signed=False)
+            self.http.writeInt32(reduction,signed=False)
+            self.http.sendRequest("paquet_filtrees")
         else:
-            return sysam.can_paquet_circulaire_filtrees(reduction)
-    def config_sortie(self,nsortie,techant,valeurs,repetition=0):
-        sysam.can_config_sortie(nsortie,techant,valeurs,repetition)
+            self.http.writeInt32(reduction,signed=False)
+            self.http.sendRequest("paquet_circulaire_filtrees")
+        
+        nombreEA = self.http.readInt8(signed=False)
+        nbpoints = self.http.readInt32(signed=False)
+        paquet = np.zeros((nombreEA*2,nbpoints),dtype=np.float64)
+        for v in range(nombreEA*2):
+            paquet[v] = self.http.readDoubleNdArray(nbpoints)
+        return paquet
+
+    def lire(self):
+        self.http.initData()
+        self.http.sendRequest("lire")
+        nombreEA = self.http.readInt8(signed=False)
+        return self.http.readDoubleNdArray(nombreEA)
+        
+        
+
     def declencher_sorties(self,ns1,ns2):
-        sysam.can_declencher_sorties(ns1,ns2)
+        self.http.initData()
+        self.http.writeInt8(ns1)
+        self.http.writeInt8(ns2)
+        self.http.sendRequest("declencher_sorties")
+
     def stopper_sorties(self,ns1,ns2):
-        sysam.can_stopper_sorties(ns1,ns2)
-    def acquerir_avec_sorties(self,valeurs1,valeurs2):
-        if type(valeurs1)!=numpy.ndarray:
-            valeurs1 = numpy.zeros(0)
-        if type(valeurs2)!=numpy.ndarray:
-            valeurs2 = numpy.zeros(0)
-        sysam.can_acquerir_avec_sorties(valeurs1,valeurs2)
-    def lancer_avec_sorties(self,valeurs1,valeurs2):
-        if type(valeurs1)!=numpy.ndarray:
-            valeurs1 = numpy.zeros(0)
-        if type(valeurs2)!=numpy.ndarray:
-            valeurs2 = numpy.zeros(0)
-        sysam.can_lancer_avec_sorties(valeurs1,valeurs2)
+        self.http.initData()
+        self.http.writeInt8(ns1)
+        self.http.writeInt8(ns2)
+        self.http.sendRequest("stopper_sorties")
+
     def ecrire(self,ns1,valeur1,ns2,valeur2):
-        sysam.can_ecrire(ns1,valeur1,ns2,valeur2)
-    def activer_lecture(self,voies):
-        sysam.can_activer_lecture(voies,0)
-    def desactiver_lecture(self):
-        sysam.can_desactiver_lecture()
-    def lire(self):
-        return sysam.can_lire()
-    def portC_config(self,bit,etat):
-        sysam.can_portC_config(bit,etat)
-    def portC_ecrire(self,bit,etat):
-        sysam.can_portC_ecrire(bit,etat)
-    def portC_lire(self,bit):
-        return sysam.can_portC_lire(bit)
-    def portB_config(self,bit,etat):
-        sysam.can_portB_config(bit,etat)
+        self.http.initData()
+        self.http.writeInt8(ns1)
+        self.http.writeDouble(valeur1)
+        self.http.writeInt8(ns2)
+        self.http.writeDouble(valeur2)
+        self.http.sendRequest("ecrire")
+
+    def config_filtre(self,listeA,listeB):
+        self.envoyer_signal(1,np.array(listeA,dtype=np.float64))
+        self.envoyer_signal(2,np.array(listeB,dtype=np.float64))
+        self.http.initData()
+        self.http.sendRequest("config_filtre")
+
+    def portB_config(self,bits,etat):
+        self.http.initData()
+        self.http.writeInt8(bits)
+        self.http.writeInt8(etat)
+        self.http.sendRequest("portB_config")
+
+    def portC_config(self,bits,etat):
+        self.http.initData()
+        self.http.writeInt8(bits)
+        self.http.writeInt8(etat)
+        self.http.sendRequest("portC_config")
+
     def portB_ecrire(self,bit,etat):
-        sysam.can_portB_ecrire(bit,etat)
+        self.http.initData()
+        self.http.writeInt8(bit)
+        self.http.writeInt8(etat)
+        self.http.sendRequest("portB_ecrire")
+
+    def portC_ecrire(self,bit,etat):
+        self.http.initData()
+        self.http.writeInt8(bit)
+        self.http.writeInt8(etat)
+        self.http.sendRequest("portC_ecrire")
+
     def portB_lire(self,bit):
-        return sysam.can_portB_lire(bit)        
-    def config_filtre(self,listeA,listeB):
-        sysam.can_config_filtre(numpy.array(listeA,dtype=numpy.double),numpy.array(listeB,dtype=numpy.double))
+        self.http.initData()
+        self.http.writeInt8(bit)
+        self.http.sendRequest("portB_lire")
+        return self.http.readInt8(signed=False)
+
+    def portC_lire(self,bit):
+        self.http.initData()
+        self.http.writeInt8(bit)
+        self.http.sendRequest("portC_lire")
+        return self.http.readInt8(signed=False)
+
     def config_compteur(self,entree,front_montant,front_descend,hysteresis,duree):
-        sysam.can_config_compteur(entree,front_montant,front_descend,hysteresis,duree)
+        self.http.initData()
+        self.http.writeInt8(entree)
+        self.http.writeInt8(front_montant)
+        self.http.writeInt8(front_descend)
+        self.http.writeDouble(hysteresis)
+        self.http.writeDouble(duree)
+        self.http.sendRequest("config_compteur")
+
     def compteur(self):
-        sysam.can_compteur()
+        self.http.initData()
+        self.http.sendRequest("compteur")
+
     def lire_compteur(self):
-        n = sysam.can_lire_compteur()
-        return numpy.uint64(numpy.left_shift(n[0],32)+n[1])
-    def config_chrono(self,entree,front_debut,front_fin,hysteresis):
-        sysam.can_config_chrono(entree,front_debut,front_fin,hysteresis)
+        self.http.initData()
+        self.http.sendRequest("lire_compteur")
+        high = self.http.readInt32(signed=False)
+        low = self.http.readInt32(signed=False)
+        return np.uint64(np.left_shift(high,32)+low)
+
+    def config_chrono(self,entree,front_montant,front_descend,hysteresis):
+        self.http.initData()
+        self.http.writeInt8(entree)
+        self.http.writeInt8(front_montant)
+        self.http.writeInt8(front_descend)
+        self.http.writeDouble(hysteresis)
+        self.http.sendRequest("config_chrono")
+
     def chrono(self):
-        sysam.can_chrono()
-    def lire_chrono(self):
-        n = sysam.can_lire_chrono()
-        return numpy.uint64(2**32)*numpy.uint64(n[0])+numpy.uint64(n[1])
-    def afficher_calibrage(self):
-        sysam.can_afficher_calibrage()
-        
-def audio_table_start(ch1,ch2,f1,f2,fs=44000,fpb=256):
-    ch1 = numpy.array(ch1,dtype=numpy.float32)
-    ch2 = numpy.array(ch2,dtype=numpy.float32)
-    sysam.table_dds_start(fs,fpb,ch1,ch2,f1,f2)
-    
-def audio_table_stop(seconds):
-    sysam.table_dds_stop(seconds)
+        self.http.initData()
+        self.http.sendRequest("chrono")
 
-def harmonics_table(amp_list,phase_list,normalize,gain):
-    TABLE_SIZE = 256
-    amp = numpy.array(amp_list,dtype=numpy.float32)
-    phase = numpy.array(phase_list,dtype=numpy.float32)
-    if amp.size != phase.size:
-        raise SystemExit("amplitude et phase : tailles incompatibles")
-    t = numpy.arange(TABLE_SIZE)*1.0/TABLE_SIZE
-    table = numpy.zeros(TABLE_SIZE,dtype=numpy.float32)
-    for n in range(amp.size):
-        table = table+amp[n]*numpy.sin(2*numpy.pi*(n+1)*t+phase[n])
-    table = numpy.array(table,dtype=numpy.float32)
-    m = abs(table.min())
-    M = abs(table.max())
-    if normalize:
-        table = table/max(m,M)
-    return table*gain
-    
+    def lire_chrono(self):
+        self.http.initData()
+        self.http.sendRequest("lire_chrono")
+        high = self.http.readInt32(signed=False)
+        low = self.http.readInt32(signed=False)
+        return np.uint64(np.left_shift(high,32)+low)
 
-def audio_harmonics_start(a1,p1,a2,p2,f1,f2,norm=True,gain=1.0,fs=44000,fpb=256):
-    table_1 = harmonics_table(a1,p1,norm,gain)
-    table_2 = harmonics_table(a2,p2,norm,gain)
-    sysam.table_dds_start(fs,fpb,table_1,table_2,f1,f2)
-    return(table_1,table_2)
-       
-def audio_harmonics_stop(seconds):
-    sysam.table_dds_stop(seconds)
-
-class RingBuffer:
-    def __init__(self,number_blocks_exponent=4,samples_per_block=64,Id=0):
-        self.pointer = sysam.ring_buffer_init(number_blocks_exponent,samples_per_block,Id)
-        self.samples_per_block = samples_per_block
-    def delete(self):
-        sysam.ring_buffer_delete(self.pointer)
-    def write(self,data):
-        data = numpy.array(data,dtype=numpy.float32)
-        sysam.ring_buffer_write(self.pointer,data)
-
-def output_stream_start(sample_rate,ring_buffer_1,ring_buffer_2):
-    p1 = 0
-    if ring_buffer_1:
-        p1 = ring_buffer_1.pointer
-    p2 = 0
-    if ring_buffer_2:
-        p2 = ring_buffer_2.pointer
-    sysam.output_stream_start(int(sample_rate),p1,p2)
-    
-def output_stream_stop(seconds):
-    sysam.output_stream_stop(seconds)
```

## Comparing `pycanum-4.2.7.dist-info/LICENCE.txt` & `pycanum-5.0.0.dist-info/LICENCE.txt`

 * *Files identical despite different names*

