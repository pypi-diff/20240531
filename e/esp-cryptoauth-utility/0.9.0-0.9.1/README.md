# Comparing `tmp/esp-cryptoauth-utility-0.9.0.tar.gz` & `tmp/esp-cryptoauth-utility-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esp-cryptoauth-utility-0.9.0.tar", last modified: Thu Aug 11 08:49:11 2022, max compression
+gzip compressed data, was "dist/esp-cryptoauth-utility-0.9.1.tar", last modified: Fri Aug 12 14:58:26 2022, max compression
```

## Comparing `esp-cryptoauth-utility-0.9.0.tar` & `esp-cryptoauth-utility-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6411 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/esp_cryptoauth_utility.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/esp_cryptoauth_utility.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/esp_cryptoauth_utility.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/esp_cryptoauth_utility.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/esp_cryptoauth_utility.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/esp_cryptoauth_utility.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/helper_scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/helper_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29498 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/helper_scripts/cert2certdef.py
--rw-r--r--   0 runner    (1001) docker     (121)     4815 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/helper_scripts/cert_sign.py
--rw-r--r--   0 runner    (1001) docker     (121)    12352 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/helper_scripts/manifest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3541 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/helper_scripts/serial.py
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/sample_bins/
--rw-r--r--   0 runner    (1001) docker     (121)   156096 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/sample_bins/secure_cert_mfg.bin
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/sample_certs/
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/sample_certs/sample_root_ca.pem
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/sample_certs/sample_root_ca_key.pem
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/sample_certs/sample_signer_cert.pem
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/sample_certs/sample_signer_key.pem
--rw-r--r--   0 runner    (1001) docker     (121)     7866 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/secure_cert_mfg.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-11 08:49:11.000000 esp-cryptoauth-utility-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3182 2022-08-11 08:49:02.000000 esp-cryptoauth-utility-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6272 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/esp_cryptoauth_utility.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/esp_cryptoauth_utility.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/esp_cryptoauth_utility.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/esp_cryptoauth_utility.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/esp_cryptoauth_utility.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/esp_cryptoauth_utility.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/helper_scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/helper_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29498 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/helper_scripts/cert2certdef.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4815 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/helper_scripts/cert_sign.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12352 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/helper_scripts/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3541 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/helper_scripts/serial.py
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/sample_bins/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/sample_bins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   156096 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/sample_bins/secure_cert_mfg.bin
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/sample_certs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/sample_certs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/sample_certs/sample_signer_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/sample_certs/sample_signer_key.pem
+-rw-r--r--   0 runner    (1001) docker     (121)     8027 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/secure_cert_mfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-12 14:58:26.000000 esp-cryptoauth-utility-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3212 2022-08-12 14:58:13.000000 esp-cryptoauth-utility-0.9.1/setup.py
```

### Comparing `esp-cryptoauth-utility-0.9.0/LICENSE` & `esp-cryptoauth-utility-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-cryptoauth-utility-0.9.0/PKG-INFO` & `esp-cryptoauth-utility-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-cryptoauth-utility
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python utility which helps to configure and provision ATECC608 chip connected to ESP32 module
 Home-page: https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility
 Author: Espressif Systems
 Author-email: 
 Project-URL: Documentation, https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility#readme
 Project-URL: Source, https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility
 Classifier: Intended Audience :: Developers
@@ -27,12 +27,12 @@
 ======================
 The python utility helps to configure and provision ATECC608 chip connected to ESP32 module. 
 
 The esp-cryptoauth-utility is `hosted on github <https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility>`_.
 
 Documentation
 -------------
-Visit online `esp-cryptoauth-utility documentation <https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility#readme/>`_ or run ``secure_cert_mfg.py.py -h``.
+Visit online `esp-cryptoauth-utility documentation <https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility#readme/>`_ or run ``secure_cert_mfg.py -h``.
 
 License
 -------
 The License for the project can be found `here <https://github.com/espressif/esp-cryptoauthlib/blob/master/esp_cryptoauth_utility/LICENSE>`_
```

### Comparing `esp-cryptoauth-utility-0.9.0/README.md` & `esp-cryptoauth-utility-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 # ESP_CRYPTOAUTH_UTILITY
+
 # Description
  The python utility helps to configure and provision `ATECC608` chip on `ESP32-WROOM-32SE` module.The [ESP32-WROOM-32SE](https://www.espressif.com/sites/default/files/documentation/esp32-wroom-32se_datasheet_en.pdf) module has Microchip's [ATECC608A](https://www.microchip.com/wwwproducts/en/ATECC608A) integrated on the module. The latest ESP32-WROOM-32SE modules have the Microchip's [ATECC608B](https://www.microchip.com/en-us/products/security-ics/trust-platform/trust-and-go) integrated on the module.
     There are currently three types of ATECC608 which are [Trust & Go](https://www.microchip.com/wwwproducts/en/ATECC608A-TNGTLS), [TrustFlex](https://www.microchip.com/wwwproducts/en/ATECC608A-TFLXTLS) and [TrustCustom](https://www.microchip.com/wwwproducts/en/ATECC608A). `Trust & Go` and `TrustFlex` chips are preconfigured by the manufacturer (Microchip) so we only need to generate manifest file for those chips. `TrustCustom` type of chips are not configured, so for `TrustCustom` type of chips need to be first configured and then provisioned with a newly  generated device certificate and key pair. The script automatically detects which type of ATECC608 chip is integrated with `ESP32-WROOM-32SE` so it will proceed to next required steps on its own.
 
 # Hardware Required
 It requires [ESP32-WROOM-32SE](https://www.espressif.com/sites/default/files/documentation/esp32-wroom-32se_datasheet_en.pdf) which has Microchip's [ATECC608A](https://www.microchip.com/wwwproducts/en/ATECC608A) (Secure Element) integrated on the module.
 
 An ESP32 to which ATECC608 is connected with I2C interface can also be used by setting the I2C pin configurations (see below option about providing I2C pin cfg).
 
 > Note: It is recommended to change directory to `esp_cryptoauth_utility` to execute all following commands if not already done.
 
-## Install python dependancies
-To use the utility some python depencancies must be installed with following command(current directory should be `esp_cryptoauth_utility` for executing the command).
+## Installation
 
-    pip install -r requirements.txt
+```
+pip install esp-cryptoauth-utility
+```
 
 ## Step 1:- Generate Signer Certificate
+
 Signer cert and key pair:
-* In case of `TrustCustom` chips ,these certificate and key pair are used to sign the device cert which is going to be generted.
+* In case of `TrustCustom` chips ,these certificate and key pair are used to sign the device cert which is going to be generated.
 
 * In case of `Trust & Go` and `TrustFlex` devices the device certs are already signed by microchip signer cert, and the signer cert and key pair generated in this step are used to sign the manifest file.
 
-By default the utility uses the `sample_signer_cert.pem` located in the `sample_certs` folder.if you want to keep using default certificats, then directly proceed to next step(Step 2).
+By default the utility uses the `sample_signer_cert.pem` located in the `sample_certs` directory. If you want to keep using default certificates, then directly proceed to next step (Step 2).
 
 Create a signer key and signer cert by executing following commands sequentially. The second command will ask some details about certificate such as `ORG, CN` which are needed to be filled by the user.
 
- `Important`: The signer cert `CN`_(Common Name)_ must end with `FFFF` as it is required by the `cert2certdef.py` (file by microchip) to create its definition properly. for e.g valid CN = `Sample Signer FFFF`( This is compulsory only in case of `TrustCustom` type of chips and not for the other two).
+ `Important`: The signer cert `CN`_(Common Name)_ must end with `FFFF` as it is required by the `cert2certdef.py` (file by microchip) to create its definition properly. For example, valid CN = `Sample Signer FFFF` (This is compulsory only in case of `TrustCustom` type of chips and not for the other two).
 
-    openssl ecparam -out signerkey.pem -name prime256v1 -genkey
-
-    openssl req -new -x509 -key signerkey.pem -out signercert.pem -days 365
+```bash
+openssl ecparam -out signerkey.pem -name prime256v1 -genkey
+openssl req -new -x509 -key signerkey.pem -out signercert.pem -days 365
+```
 
 ## Step 2:- Provision the module/Generate manifest file
 
 *   The tool will automatically detect the type of ATECC608 chip connected to ESP module and perform its intended task which are as follows.
 
-    * For `TrustCustom` type of ATECC608 chip first configure ATECC608 chip with its default configuration options.The tool will create a device cert by generating a private key on slot 0 of the module, passing the CSR to host, sign the CSR with signer cert generated in step above. To set validity of device cert please refer [device_cert_validity](README.md#set-validity-of-device-cert-for-trustcustom). save the device cert on the ATECC chip as well as on the host machine as `device_cert.pem`,it also saves the cert definitions in `output_files` folder for future use.
+    * For `TrustCustom` type of ATECC608 chip first configure ATECC608 chip with its default configuration options.The tool will create a device cert by generating a private key on slot 0 of the module, passing the CSR to host, sign the CSR with signer cert generated in step above. To set validity of device cert please refer [device_cert_validity](README.md#set-validity-of-device-cert-for-trustcustom). Save the device cert on the ATECC chip as well as on the host machine as `device_cert.pem`, it also saves the cert definitions in `output_files` directory for future use.
 
     * For `Trust & Go` and `TrustFlex` type of ATECC608 devices this script will generate the manifest file with the name of chip serial number.The manifest file will be signed with the signer cert generated above. The generated manifest file should be registered with the cloud to register the device certificate.
 
 The command is as follows:
 
 ```
 python secure_cert_mfg.py --signer-cert signercert.pem --signer-cert-private-key signerkey.pem --port /UART/COM/PORT
 ```
+
 > Note: The names `signercert.pem` and `signerkey.pem` denote the name of the signer cert and key files respectively, you can replace them with `relative/path/to/you/signer/cert` and `key` respectively. The `UART/COM/PORT` represents the host machine COM port to which your ESP32-WROOM-32SE is connected.Please refer [check serial port](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/establish-serial-connection.html#check-port-on-windows) for obtaining the serial port connected to ESP.
 
-If you do not provide `signer-cert` and `signer_key` in above command, `sample_signer_cert.pem` stored at `sample_certs` will be used.
+If you do not provide `signer-cert` and `signer-cert-private-key` in above command, `sample_signer_cert.pem` stored at `sample_certs` will be used.
 
 ---
 ### Provide I2C pin configuration (for modules other than ESP32-WROOM32-SE)
 The I2C pins of the ESP32 to which ATECC608 chip is connected can be provided as a parameter to the python script.
 The command is as follows:
 ```
 python secure_cert_mfg.py --i2c-sda-pin /* SDA pin no */ --i2c-scl-pin /* SCL pin no */ /* + other options */
```

### Comparing `esp-cryptoauth-utility-0.9.0/esp_cryptoauth_utility.egg-info/PKG-INFO` & `esp-cryptoauth-utility-0.9.1/esp_cryptoauth_utility.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-cryptoauth-utility
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python utility which helps to configure and provision ATECC608 chip connected to ESP32 module
 Home-page: https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility
 Author: Espressif Systems
 Author-email: 
 Project-URL: Documentation, https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility#readme
 Project-URL: Source, https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility
 Classifier: Intended Audience :: Developers
@@ -27,12 +27,12 @@
 ======================
 The python utility helps to configure and provision ATECC608 chip connected to ESP32 module. 
 
 The esp-cryptoauth-utility is `hosted on github <https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility>`_.
 
 Documentation
 -------------
-Visit online `esp-cryptoauth-utility documentation <https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility#readme/>`_ or run ``secure_cert_mfg.py.py -h``.
+Visit online `esp-cryptoauth-utility documentation <https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility#readme/>`_ or run ``secure_cert_mfg.py -h``.
 
 License
 -------
 The License for the project can be found `here <https://github.com/espressif/esp-cryptoauthlib/blob/master/esp_cryptoauth_utility/LICENSE>`_
```

### Comparing `esp-cryptoauth-utility-0.9.0/esp_cryptoauth_utility.egg-info/SOURCES.txt` & `esp-cryptoauth-utility-0.9.1/esp_cryptoauth_utility.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 esp_cryptoauth_utility.egg-info/requires.txt
 esp_cryptoauth_utility.egg-info/top_level.txt
 helper_scripts/__init__.py
 helper_scripts/cert2certdef.py
 helper_scripts/cert_sign.py
 helper_scripts/manifest.py
 helper_scripts/serial.py
+sample_bins/__init__.py
 sample_bins/secure_cert_mfg.bin
-sample_certs/sample_root_ca.pem
-sample_certs/sample_root_ca_key.pem
+sample_certs/__init__.py
 sample_certs/sample_signer_cert.pem
 sample_certs/sample_signer_key.pem
```

### Comparing `esp-cryptoauth-utility-0.9.0/helper_scripts/cert2certdef.py` & `esp-cryptoauth-utility-0.9.1/helper_scripts/cert2certdef.py`

 * *Files identical despite different names*

### Comparing `esp-cryptoauth-utility-0.9.0/helper_scripts/cert_sign.py` & `esp-cryptoauth-utility-0.9.1/helper_scripts/cert_sign.py`

 * *Files identical despite different names*

### Comparing `esp-cryptoauth-utility-0.9.0/helper_scripts/manifest.py` & `esp-cryptoauth-utility-0.9.1/helper_scripts/manifest.py`

 * *Files identical despite different names*

### Comparing `esp-cryptoauth-utility-0.9.0/helper_scripts/serial.py` & `esp-cryptoauth-utility-0.9.1/helper_scripts/serial.py`

 * *Files identical despite different names*

### Comparing `esp-cryptoauth-utility-0.9.0/sample_bins/secure_cert_mfg.bin` & `esp-cryptoauth-utility-0.9.1/sample_bins/secure_cert_mfg.bin`

 * *Files identical despite different names*

### Comparing `esp-cryptoauth-utility-0.9.0/sample_certs/sample_signer_cert.pem` & `esp-cryptoauth-utility-0.9.1/sample_certs/sample_signer_cert.pem`

 * *Files identical despite different names*

### Comparing `esp-cryptoauth-utility-0.9.0/secure_cert_mfg.py` & `esp-cryptoauth-utility-0.9.1/secure_cert_mfg.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,41 +14,51 @@
 import argparse
 from pyasn1_modules import pem
 from sys import exit
 import helper_scripts as hs
 import binascii
 import os
 import sys
+import sample_bins
+import sample_certs
+
 try:
     import esptool
 except ImportError:  # cheat and use IDF's copy of esptool if available
     idf_path = os.getenv("IDF_PATH")
     if not idf_path or not os.path.exists(idf_path):
         raise
     sys.path.insert(0, os.path.join(idf_path, "components", "esptool_py", "esptool"))
     import esptool
 
-BINARY_STUB_PATH = os.path.join(os.path.dirname(__file__),
-                                'sample_bins', 'secure_cert_mfg.bin')
+BINARY_STUB_PATH = os.path.join(sample_bins.__path__[0],
+                                'secure_cert_mfg.bin')
+
+SAMPLE_SIGNERCERT_PATH = os.path.join(sample_certs.__path__[0],
+                                      'sample_signer_cert.pem')
+
+SAMPLE_SIGNERKEY_PATH = os.path.join(sample_certs.__path__[0],
+                                     'sample_signer_key.pem')
+
 
 def main():
     parser = argparse.ArgumentParser(description='''Provision the ESPWROOM32SE device with
         device_certificate and signer_certificate required for TLS authentication''')
 
     parser.add_argument(
         '--signer-cert',
         dest='signer_cert',
-        default=os.path.join(os.path.dirname(__file__), 'sample_certs', 'sample_signer_cert.pem'),
+        default=SAMPLE_SIGNERCERT_PATH,
         metavar='relative/path/to/signer_cert.pem',
         help='relative path(from secure_cert_mfg.py) to signer certificate.')
 
     parser.add_argument(
         '--signer-cert-private-key',
         dest='signer_privkey',
-        default=os.path.join(os.path.dirname(__file__), 'sample_certs', 'sample_signer_key.pem'),
+        default=SAMPLE_SIGNERKEY_PATH,
         metavar='relative/path/to/signer-priv-key',
         help='relative path(from secure_cert_mfg.py) to signer certificate private key')
 
     parser.add_argument(
         "--pwd", '--password',
         dest='password',
         metavar='[password]',
```

### Comparing `esp-cryptoauth-utility-0.9.0/setup.py` & `esp-cryptoauth-utility-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,28 @@
     print(
         "Package setuptools is missing from your Python installation. "
         "Please see the installation section in the esp-cryptoauth-utillity documentation"
         " for instructions on how to install it."
     )
     exit(1)
 
-VERSION = "0.9.0"
+VERSION = "0.9.1"
 
 long_description = """
 ======================
 esp-cryptoauth-utility
 ======================
 The python utility helps to configure and provision ATECC608 chip connected to ESP32 module. 
 
 The esp-cryptoauth-utility is `hosted on github <https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility>`_.
 
 Documentation
 -------------
 Visit online `esp-cryptoauth-utility documentation <https://github.com/espressif/esp-cryptoauthlib/tree/master/esp_cryptoauth_utility#readme/>`_ \
-or run ``secure_cert_mfg.py.py -h``.
+or run ``secure_cert_mfg.py -h``.
 
 License
 -------
 The License for the project can be found `here <https://github.com/espressif/esp-cryptoauthlib/blob/master/esp_cryptoauth_utility/LICENSE>`_
 """
 
 setup(
@@ -74,10 +74,11 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     python_requires=">=3.7",
     setup_requires=(["wheel"] if "bdist_wheel" in sys.argv else []),
     install_requires=get_install_requires(),
+    include_package_data = True,
     packages=find_packages(),
     scripts=["secure_cert_mfg.py"],
 )
```

