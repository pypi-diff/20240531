# Comparing `tmp/Sanatio-0.0.1.tar.gz` & `tmp/Sanatio-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sanatio-0.0.1.tar", last modified: Fri Nov 18 03:36:36 2022, max compression
+gzip compressed data, was "Sanatio-1.0.0.tar", last modified: Fri May 31 15:34:15 2024, max compression
```

## Comparing `Sanatio-0.0.1.tar` & `Sanatio-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxrwxrwx   0 dr        (1000) dr        (1000)        0 2022-11-18 03:36:36.323410 Sanatio-0.0.1/
--rwxrwxrwx   0 dr        (1000) dr        (1000)    11545 2022-11-16 17:34:52.000000 Sanatio-0.0.1/LICENSE
--rwxrwxrwx   0 dr        (1000) dr        (1000)     1628 2022-11-18 03:36:36.323410 Sanatio-0.0.1/PKG-INFO
--rwxrwxrwx   0 dr        (1000) dr        (1000)      694 2022-11-18 03:35:33.000000 Sanatio-0.0.1/README.md
-drwxrwxrwx   0 dr        (1000) dr        (1000)        0 2022-11-18 03:36:36.153824 Sanatio-0.0.1/Sanatio.egg-info/
--rwxrwxrwx   0 dr        (1000) dr        (1000)     1628 2022-11-18 03:36:35.000000 Sanatio-0.0.1/Sanatio.egg-info/PKG-INFO
--rwxrwxrwx   0 dr        (1000) dr        (1000)      297 2022-11-18 03:36:35.000000 Sanatio-0.0.1/Sanatio.egg-info/SOURCES.txt
--rwxrwxrwx   0 dr        (1000) dr        (1000)        1 2022-11-18 03:36:35.000000 Sanatio-0.0.1/Sanatio.egg-info/dependency_links.txt
--rwxrwxrwx   0 dr        (1000) dr        (1000)       27 2022-11-18 03:36:35.000000 Sanatio-0.0.1/Sanatio.egg-info/requires.txt
--rwxrwxrwx   0 dr        (1000) dr        (1000)        8 2022-11-18 03:36:35.000000 Sanatio-0.0.1/Sanatio.egg-info/top_level.txt
-drwxrwxrwx   0 dr        (1000) dr        (1000)        0 2022-11-18 03:36:36.235880 Sanatio-0.0.1/sanatio/
--rwxrwxrwx   0 dr        (1000) dr        (1000)        0 2022-11-16 04:16:47.000000 Sanatio-0.0.1/sanatio/__init__.py
-drwxrwxrwx   0 dr        (1000) dr        (1000)        0 2022-11-18 03:36:36.297769 Sanatio-0.0.1/sanatio/assets/
--rwxrwxrwx   0 dr        (1000) dr        (1000)    30994 2022-11-17 13:40:45.000000 Sanatio-0.0.1/sanatio/assets/country.json
--rwxrwxrwx   0 dr        (1000) dr        (1000)     1181 2022-11-16 04:22:52.000000 Sanatio-0.0.1/sanatio/assets/regex.json
--rwxrwxrwx   0 dr        (1000) dr        (1000)    14407 2022-11-18 03:20:27.000000 Sanatio-0.0.1/sanatio/main.py
--rwxrwxrwx   0 dr        (1000) dr        (1000)      670 2022-11-18 03:21:21.000000 Sanatio-0.0.1/sanatio/utils.py
--rwxrwxrwx   0 dr        (1000) dr        (1000)       74 2022-11-18 03:36:36.335934 Sanatio-0.0.1/setup.cfg
--rwxrwxrwx   0 dr        (1000) dr        (1000)     1287 2022-11-18 03:35:49.000000 Sanatio-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.068648 Sanatio-1.0.0/
+-rw-rw-rw-   0        0        0    11545 2024-05-30 04:29:04.000000 Sanatio-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2224 2024-05-31 15:34:15.068648 Sanatio-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2024-05-30 04:29:04.000000 Sanatio-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.006453 Sanatio-1.0.0/Sanatio.egg-info/
+-rw-rw-rw-   0        0        0     2224 2024-05-31 15:34:14.000000 Sanatio-1.0.0/Sanatio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2024-05-31 15:34:14.000000 Sanatio-1.0.0/Sanatio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 15:34:14.000000 Sanatio-1.0.0/Sanatio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-31 15:34:14.000000 Sanatio-1.0.0/Sanatio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-31 15:34:14.000000 Sanatio-1.0.0/Sanatio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.012054 Sanatio-1.0.0/sanatio/
+-rw-rw-rw-   0        0        0       61 2024-05-31 14:54:09.000000 Sanatio-1.0.0/sanatio/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.016050 Sanatio-1.0.0/sanatio/assets/
+-rw-rw-rw-   0        0        0    25900 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/assets/country.json
+-rw-rw-rw-   0        0        0     1181 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/assets/regex.json
+-rw-rw-rw-   0        0        0    15058 2024-05-30 04:45:20.000000 Sanatio-1.0.0/sanatio/main.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.023600 Sanatio-1.0.0/sanatio/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-31 15:11:29.000000 Sanatio-1.0.0/sanatio/utils/__init__.py
+-rw-rw-rw-   0        0        0      655 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/utils/checksum.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:34:15.028883 Sanatio-1.0.0/sanatio/utils/checksum_algorithms/
+-rw-rw-rw-   0        0        0        0 2024-05-31 15:11:29.000000 Sanatio-1.0.0/sanatio/utils/checksum_algorithms/__init__.py
+-rw-rw-rw-   0        0        0     1318 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/utils/checksum_algorithms/luhn_algorithm.py
+-rw-rw-rw-   0        0        0     1741 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/utils/checksum_algorithms/verhoeff_algorithm.py
+-rw-rw-rw-   0        0        0      691 2024-05-30 04:29:04.000000 Sanatio-1.0.0/sanatio/utils/utils.py
+-rw-rw-rw-   0        0        0       81 2024-05-31 15:34:15.073617 Sanatio-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1304 2024-05-31 14:46:18.000000 Sanatio-1.0.0/setup.py
```

### Comparing `Sanatio-0.0.1/LICENSE` & `Sanatio-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Sanatio-0.0.1/sanatio/assets/country.json` & `Sanatio-1.0.0/sanatio/assets/country.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9501108647450113%*

 * *Differences: {"'AF'": "{delete: ['DrivingLicense']}",*

 * * "'AM'": "{delete: ['DrivingLicense']}",*

 * * "'AR'": "{delete: ['DrivingLicense']}",*

 * * "'AT'": "{delete: ['DrivingLicense']}",*

 * * "'AU'": "{delete: ['DrivingLicense']}",*

 * * "'AZ'": "{delete: ['DrivingLicense']}",*

 * * "'BD'": "{delete: ['DrivingLicense']}",*

 * * "'BR'": "{delete: ['DrivingLicense']}",*

 * * "'BY'": "{delete: ['DrivingLicense']}",*

 * * "'CA'": "{delete: ['DrivingLicense']}",*

 * * "'CH'": "{delete: ['DrivingLicense']}",*

 * * "'CN'": "{delete: ['DrivingLicense']}",*

 * * "'CY'": "{delete: [ […]*

```diff
@@ -1,18 +1,13 @@
 {
     "AF": {
         "Code": "AF",
         "Currency": "AFN",
         "CurrencyName": "Afghani",
         "CurrencySymbol": "\u060b",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Afghanistan",
@@ -30,19 +25,14 @@
         }
     },
     "AM": {
         "Code": "AM",
         "Currency": "AMD",
         "CurrencyName": "Dram",
         "CurrencySymbol": "\u058f",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Armenia",
@@ -59,19 +49,14 @@
         }
     },
     "AR": {
         "Code": "AR",
         "Currency": "ARS",
         "CurrencyName": "Peso",
         "CurrencySymbol": "$",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Argentina",
@@ -88,19 +73,14 @@
         }
     },
     "AT": {
         "Code": "AT",
         "Currency": "EUR",
         "CurrencyName": "Euro",
         "CurrencySymbol": "\u20ac",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Austria",
@@ -117,19 +97,14 @@
         }
     },
     "AU": {
         "Code": "AU",
         "Currency": "AUD",
         "CurrencyName": "Dollar",
         "CurrencySymbol": "$",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Australia",
@@ -146,19 +121,14 @@
         }
     },
     "AZ": {
         "Code": "AZ",
         "Currency": "AZN",
         "CurrencyName": "Manat",
         "CurrencySymbol": "\u20bc",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Azerbaijan",
@@ -175,19 +145,14 @@
         }
     },
     "BD": {
         "Code": "BD",
         "Currency": "BDT",
         "CurrencyName": "Taka",
         "CurrencySymbol": "\u09f3",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Bangladesh",
@@ -204,19 +169,14 @@
         }
     },
     "BR": {
         "Code": "BR",
         "Currency": "BRL",
         "CurrencyName": "Real",
         "CurrencySymbol": "R$",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Brazil",
@@ -233,19 +193,14 @@
         }
     },
     "BY": {
         "Code": "BY",
         "Currency": "BYR",
         "CurrencyName": "Ruble",
         "CurrencySymbol": "p.",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Belarus",
@@ -262,19 +217,14 @@
         }
     },
     "CA": {
         "Code": "CA",
         "Currency": "CAD",
         "CurrencyName": "Dollar",
         "CurrencySymbol": "$",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Canada",
@@ -291,19 +241,14 @@
         }
     },
     "CH": {
         "Code": "CH",
         "Currency": "CHF",
         "CurrencyName": "Franc",
         "CurrencySymbol": "Fr.",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Switzerland",
@@ -320,19 +265,14 @@
         }
     },
     "CN": {
         "Code": "CN",
         "Currency": "CNY",
         "CurrencyName": "Yuan RenMinLengthbi",
         "CurrencySymbol": "\u00a5",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "China",
@@ -349,19 +289,14 @@
         }
     },
     "CY": {
         "Code": "CY",
         "Currency": "EUR",
         "CurrencyName": "Euro",
         "CurrencySymbol": "\u20ac",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Cyprus",
@@ -378,19 +313,14 @@
         }
     },
     "CZ": {
         "Code": "CZ",
         "Currency": "CZK",
         "CurrencyName": "Koruna",
         "CurrencySymbol": "K\u010d",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Czech Republic",
@@ -407,19 +337,14 @@
         }
     },
     "DE": {
         "Code": "DE",
         "Currency": "EUR",
         "CurrencyName": "Euro",
         "CurrencySymbol": "\u20ac",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Germany",
@@ -436,19 +361,14 @@
         }
     },
     "DK": {
         "Code": "DK",
         "Currency": "DKK",
         "CurrencyName": "Krone",
         "CurrencySymbol": "kr.",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Denmark",
@@ -465,19 +385,14 @@
         }
     },
     "DZ": {
         "Code": "DZ",
         "Currency": "DZD",
         "CurrencyName": "Dinar",
         "CurrencySymbol": "\u062f.\u062c",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Algeria",
@@ -494,19 +409,14 @@
         }
     },
     "ES": {
         "Code": "ES",
         "Currency": "EUR",
         "CurrencyName": "Euro",
         "CurrencySymbol": "\u20ac",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Spain",
@@ -523,19 +433,14 @@
         }
     },
     "FI": {
         "Code": "FI",
         "Currency": "EUR",
         "CurrencyName": "Euro",
         "CurrencySymbol": "\u20ac",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Finland",
@@ -552,19 +457,14 @@
         }
     },
     "FR": {
         "Code": "FR",
         "Currency": "EUR",
         "CurrencyName": "Euro",
         "CurrencySymbol": "\u20ac",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "France",
@@ -581,19 +481,14 @@
         }
     },
     "GB": {
         "Code": "GB",
         "Currency": "GBP",
         "CurrencyName": "Pound",
         "CurrencySymbol": "\u00a3",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "United Kingdom",
@@ -610,19 +505,14 @@
         }
     },
     "ID": {
         "Code": "ID",
         "Currency": "IDR",
         "CurrencyName": "Rupiah",
         "CurrencySymbol": "Rp",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Indonesia",
@@ -639,19 +529,14 @@
         }
     },
     "IE": {
         "Code": "IE",
         "Currency": "EUR",
         "CurrencyName": "Euro",
         "CurrencySymbol": "\u20ac",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Ireland",
@@ -668,19 +553,14 @@
         }
     },
     "IN": {
         "Code": "IN",
         "Currency": "INR",
         "CurrencyName": "Rupee",
         "CurrencySymbol": "\u20b9",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {
             "Format": "^[A-Z]{2,2}[0-9]{1,2}[A-Z]{1,2}[0-9]{4,4}$",
             "MaxLength": 10,
             "MinLength": 9,
             "Regex": "^[A-Z]{2,2}[0-9]{1,2}[A-Z]{1,2}[0-9]{4,4}$"
         },
         "MobileNumber": {
@@ -702,19 +582,14 @@
         }
     },
     "IR": {
         "Code": "IR",
         "Currency": "IRR",
         "CurrencyName": "Rial",
         "CurrencySymbol": "\ufdfc",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Iran",
@@ -731,19 +606,14 @@
         }
     },
     "IT": {
         "Code": "IT",
         "Currency": "EUR",
         "CurrencyName": "Euro",
         "CurrencySymbol": "\u20ac",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Italy",
@@ -760,19 +630,14 @@
         }
     },
     "JP": {
         "Code": "JP",
         "Currency": "JPY",
         "CurrencyName": "Yen",
         "CurrencySymbol": "\u00a5",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Japan",
@@ -789,19 +654,14 @@
         }
     },
     "LY": {
         "Code": "LY",
         "Currency": "LYD",
         "CurrencyName": "Dinar",
         "CurrencySymbol": "\u0644.\u062f",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Libya",
@@ -818,19 +678,14 @@
         }
     },
     "MX": {
         "Code": "MX",
         "Currency": "MXN",
         "CurrencyName": "Peso",
         "CurrencySymbol": "$",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Mexico",
@@ -847,19 +702,14 @@
         }
     },
     "MY": {
         "Code": "MY",
         "Currency": "MYR",
         "CurrencyName": "Ringgit",
         "CurrencySymbol": "RM",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Malaysia",
@@ -876,19 +726,14 @@
         }
     },
     "PK": {
         "Code": "PK",
         "Currency": "PKR",
         "CurrencyName": "Rupee",
         "CurrencySymbol": "\u20a8",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Pakistan",
@@ -905,19 +750,14 @@
         }
     },
     "PL": {
         "Code": "PL",
         "Currency": "PLN",
         "CurrencyName": "Zloty",
         "CurrencySymbol": "z\u0142",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Poland",
@@ -934,19 +774,14 @@
         }
     },
     "PT": {
         "Code": "PT",
         "Currency": "EUR",
         "CurrencyName": "Euro",
         "CurrencySymbol": "\u20ac",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Portugal",
@@ -963,19 +798,14 @@
         }
     },
     "SA": {
         "Code": "SA",
         "Currency": "SAR",
         "CurrencyName": "Riyal",
         "CurrencySymbol": "\ufdfc",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Saudi Arabia",
@@ -992,19 +822,14 @@
         }
     },
     "SE": {
         "Code": "SE",
         "Currency": "SEK",
         "CurrencyName": "Krona",
         "CurrencySymbol": "kr",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Sweden",
@@ -1021,19 +846,14 @@
         }
     },
     "SG": {
         "Code": "SG",
         "Currency": "SGD",
         "CurrencyName": "Dollar",
         "CurrencySymbol": "$",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Singapore",
@@ -1050,19 +870,14 @@
         }
     },
     "TH": {
         "Code": "TH",
         "Currency": "THB",
         "CurrencyName": "Baht",
         "CurrencySymbol": "\u0e3f",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Thailand",
@@ -1079,19 +894,14 @@
         }
     },
     "TR": {
         "Code": "TR",
         "Currency": "TRY",
         "CurrencyName": "Lira",
         "CurrencySymbol": "\u20ba",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Turkey",
@@ -1108,19 +918,14 @@
         }
     },
     "UA": {
         "Code": "UA",
         "Currency": "UAH",
         "CurrencyName": "Hryvnia",
         "CurrencySymbol": "\u20b4",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "Ukraine",
@@ -1137,19 +942,14 @@
         }
     },
     "US": {
         "Code": "US",
         "Currency": "USD",
         "CurrencyName": "Dollar",
         "CurrencySymbol": "$",
-        "DrivingLicense": {
-            "MaxLength": 9,
-            "MinLength": 9,
-            "Regex": "^[0-9]{9}$"
-        },
         "LicensePlate": {
             "Format": "",
             "MaxLength": 6,
             "MinLength": 6,
             "Regex": ""
         },
         "MobileNumber": {
@@ -1171,19 +971,14 @@
         }
     },
     "ZA": {
         "Code": "ZA",
         "Currency": "ZAR",
         "CurrencyName": "Rand",
         "CurrencySymbol": "R",
-        "DrivingLicense": {
-            "MaxLength": 0,
-            "MinLength": 0,
-            "Regex": ""
-        },
         "LicensePlate": {},
         "MobileNumber": {
             "MaxLength": 0,
             "MinLength": 0,
             "Regex": ""
         },
         "Name": "South Africa",
```

### Comparing `Sanatio-0.0.1/sanatio/assets/regex.json` & `Sanatio-1.0.0/sanatio/assets/regex.json`

 * *Files identical despite different names*

### Comparing `Sanatio-0.0.1/sanatio/main.py` & `Sanatio-1.0.0/sanatio/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,185 +1,184 @@
 import re
 import json
 from datetime import datetime
 from dateutil.parser import parse
 from Levenshtein import distance as levenshtein_distance
 
-from sanatio.utils import all_country, regexs
+from sanatio.utils.utils import all_country, regexs
+from sanatio.utils.checksum import checksum_aadhar, checksum_credit_card
 
 class Validator(object):
     """ Validator class for validating the data """
     def __init__(self):
         pass
 
-    def __isvalidString(self, value):
+    def __isvalidString(self, value: str) -> bool:
         """ check if the string is valid or not """
         if value is None or value == '':
             return False
 
         if isinstance(value, str):
             return True
 
-        return False
-
-    def __isvalidNumber(self, value):
+    def __isvalidNumber(self, value: int)-> bool:
         """ check if the number is valid or not """
         if value is None:
             return False
 
         if isinstance(value, (int, float)):
             return True
 
-        return False
-
-    def __isvalidBoolean(self, value):
+    def __isvalidBoolean(self, value: bool)-> bool:
         """ check if the string is boolean or not """
         if value is None:
             return False
+
         if isinstance(value, bool):
             return True
 
-        return False
-    
-    def isPostalCode(self, value, locale):
+    def isAadharCard(self, value)-> bool:
+        """ check if the string is Aadhar card or not """
+        regex = "^[2-9]{1}[0-9]{3}[0-9]{4}[0-9]{4}$"  # need to improve regex for space and hyphen
+        value = value.strip().replace(" ", "")
+        if self.isLength(value, 12, 12):
+            if isinstance(value, int):
+                value = str(value)
+
+            if value[0] != '0' or value[0] != '1':
+                if re.match(regex, value):
+                    if checksum_aadhar(value):
+                        return True
+
+    def isPostalCode(self, value, locale: str)-> bool:
         """ check if the string is postal code or not """
         country_data = all_country[locale]
-        
+
         PostalCode = country_data['PostalCode']
-        
+
         PostalCodeFormat = PostalCode['Format']
         PostalCodeRegex = PostalCode['Regex']
         MinPostalCodeLength = PostalCode['MinLength']
         MaxPostalCodeLength = PostalCode['MaxLength']
-        
+
         if re.match(PostalCodeRegex, value) and re.match(PostalCodeFormat, value) \
             and self.isLength(str(value), MinPostalCodeLength, MaxPostalCodeLength):
                 return True
 
         return False
 
-    def isLicensePlate(self, value, locale):
+    def isLicensePlate(self, value, locale: str) -> bool:
         """ check if the string is license plate or not """
         value = value.upper()
         country_data = all_country[locale]
 
         LicensePlate = country_data['LicensePlate']
         Format = LicensePlate['Format']
         Regex = LicensePlate['Regex']
         MinLength = LicensePlate['MinLength']
         MaxLength = LicensePlate['MaxLength']
-        
+
 
         if re.match(Format, value) and re.match(Regex, value) \
             and self.isLength(value, MinLength, MaxLength):
                 return True
 
         return False
-    
-    def isPassportNumber(self, value, locale):  # TODO: research more about passport number
+
+    def isPassportNumber(self, value, locale: str)-> bool:  # TODO: research more about passport number
         """ check if the string is passport number or not """
         country_data = all_country[locale]
-        
+
         PassportNumberRegex = country_data['PassportNumberRegex']
         if re.match(PassportNumberRegex, value):
             return True
         return False
 
-    def isMobilePhone(self, value, locale):
+    def isMobilePhone(self, value, locale: str) -> bool:
         """ check if the string is mobile phone or not """
         country_data = all_country[locale]
 
         MobileNumberRegex = country_data['MobileNumberRegex']
 
         if re.match(MobileNumberRegex, value):
             return True
 
         return False
-    
-    def isDriverLicense(self, value, locale):
-        """ check if the string is driver license or not """
-        country_data = all_country[locale]
-
-        DrivingLicenseNumberRegex = country_data['DrivingLicenseNumberRegex']
-
-        if re.match(DrivingLicenseNumberRegex, value):
-            return True
 
-        return False
-    
-    def isDiscordUsername(self, value):
+    def isDiscordUsername(self, value: str) -> bool:
         regex = "^.{3,32}#[0-9]{4}$"
         if re.match(regex, value):
             return True
         return False
-    
-    def isCreditCard(self, value):
+
+    def isCreditCard(self, value: str) -> bool:  # checksum not implemented
         regex = regexs['credit_card_regex']
         if re.match(regex, value):
-            return True
+            if checksum_credit_card(value):
+                return True
         return False
 
-    def equals(self, value1, value2, ignoreCase=False)-> bool:
+    def equals(self, value1: str, value2: str, ignoreCase: bool=False)-> bool:
         """ Check if the two string are equal or not """
         if not self.__isvalidString(value1) or not self.__isvalidString(value2):
             return False
-        
+
         if ignoreCase:
             value1 = value1.lower()
             value2 = value2.lower()
 
         if value1 == value2:
             return True
 
         return False
 
-    def isLength(self, value, min=0, max=None):
+    def isLength(self, value: str, min: int=0, max: int=None) -> bool:
         """ check if the string length is between min and max """
         if min <= len(value) <= max:
             return True
 
         return False
 
-    def isEmpty(self, value):
+    def isEmpty(self, value: str) -> bool:
         """ check if the string is empty or not """
         value = value.strip()
         if value == "":
             return True
 
         return False
 
-    def isAlphanumeric(self, value):
+    def isAlphanumeric(self, value: str) -> bool:
         if value.isalnum():
             return True
 
         return False
 
-    def isAlpha(self, value):
+    def isAlpha(self, value: str) -> bool:
         if value.isalpha():
             return True
 
         return False
 
-    def isAscii(self, value):
+    def isAscii(self, value) -> bool:
         if value.isascii():
             return True
 
         return False
 
-    def contains(self, value, substring, ignoreCase=False):
+    def contains(self, value: str, substring: str, ignoreCase: bool=False) -> bool:
         if ignoreCase:
             value = value.lower()
             substring = substring.lower()
 
         if substring in value:
             return True
 
         return False
 
-    def isAfter(self, date1, date2=datetime.now()):
+    def isAfter(self, date1, date2=datetime.now()) -> bool:
         """ check if date1 is after date2 default date2 is current date
 
         Args:
             date1 (str): date in string format
             date2 (str): date in string format default is current date
 
         """
@@ -190,15 +189,15 @@
             date2 = datetime.strptime(date2, '%Y-%m-%d')
 
         if date1 > date2:
             return True
 
         return False
 
-    def isBefore(self, date1, date2=datetime.now()):
+    def isBefore(self, date1, date2=datetime.now()) -> bool:
         """
         check if date1 is before date2 default date2 is current date
 
         Args:
             date1 (str): date in string format
             date2 (str): date in string format default is current date
         """
@@ -208,151 +207,153 @@
             date2 = datetime.strptime(date2, '%Y-%m-%d')
 
         if date1 < date2:
             return True
 
         return False
 
-    def isDate(self, value):
+    def isDate(self, value) -> bool:
         """ check if the string is date or not """
         if not self.__isvalidString(value):
             return False
         try:
             date_obj = parse(value)
             if date_obj:
                 return True
         except Exception:
             return False
         return False
-    
-    def isLeapYear(self, year):
+
+    def isLeapYear(self, year) -> bool:
         """ check if the year is leap year or not """
         if year % 4 == 0:
             if year % 100 == 0:
                 if year % 400 == 0:
                     return True
                 else:
                     return False
             else:
                 return True
         else:
             return False
 
 
-    def isEmail(self, value, checkDNS=False):
+    def isEmail(self, value: str, checkDNS: bool=False) -> bool:
         """ check if the string is email or not """
         if not self.__isvalidString(value):
             return False
         regex = "^[a-zA-Z0-9+_.-]+@[a-zA-Z0-9.-]+$"
         if re.search(regex, value):
             return True
 
         return False
 
-    def isDecimal(self, value):
+    def isDecimal(self, value: float) -> bool:
         """ check if the string is decimal or not """
         if not self.__isvalidNumber(value):
             return False
-    
+
         if value.isdecimal():
             return True
 
         return False
 
-    def isDivisibleBy(self, number, divisor):
+    def isDivisibleBy(self, number: int, divisor: int) -> bool:
         """ check if the number is divisible by divisor or not """
         if self.__isvalidNumber(number) and self.__isvalidNumber(divisor) and divisor != 0:
             if number % divisor == 0:
                 return True
 
         return False
 
-    def isEAN(self, value):
+    def isEAN(self, value) -> bool:
         """ check if the string is EAN or not """
         pass
 
-    def isHash(self, value):
+    def isHash(self, value) -> bool:
         """ check if the string is hash or not """
         pass
 
-    def isIMEI(self, value):
+    def isIMEI(self, value) -> bool:
         """ check if the string is IMEI or not """
         if len(value) == 15 or len(value) == 17:
             return True
         return False
 
-    def isIPV4(self, value):
+    def isIPV4(self, value: str) -> bool:
         """ check if the string is IP or not """
         regex = regexs['ipv4_regex']
         if re.search(regex, value):
             return True
         return False
 
-    def isIPV6(self, value):
+    def isIPV6(self, value: str) -> bool:
         regex = regexs['ipv6_regex']
         if re.match(regex, value):
             return True
         return False
 
-    def isSSN(self, value):
+    def isSSN(self, value) -> bool:
         """ check if the string is SSN or not """
         regex = '^(?!0{3})(?!6{3})[0-8]\d{2}-(?!0{2})\d{2}-(?!0{4})\d{4}$'
         if re.match(regex, value):
             return True
         return False
-    
-    def isJSON(self, value):
+
+    def isJSON(self, value) -> bool:
         """ check if the string is JSON or not """
         try:
             json.loads(value)
             return True
         except ValueError:
             return False
 
-    def isJWT(self, value):
+    def isJWT(self, value) -> bool:
         """ check if the string is JWT or not """
         regex = "^[A-Za-z0-9_-]{2,}(?:\.[A-Za-z0-9_-]{2,}){2}$"
         if re.match(regex, value):
             return True
 
         return False
 
-    def isLatLong(self, value):
+    def isLatLong(self, value: str) -> bool:
         """ check if the string is lat long or not """
         regex = "^((\-?|\+?)?\d+(\.\d+)?),\s*((\-?|\+?)?\d+(\.\d+)?)$"
         if re.match(regex, value):
             return True
         return False
 
-    def isMACAddress(self, value):
+    def isMACAddress(self, value: str) -> bool:
         """ check if the string is MAC address or not """
         regex = regexs['mac_address_regex']
         if self.__isvalidString(value) and re.search(regex, value, re.IGNORECASE):
             return True
         return False
 
-    def isMD5(self, value):
+    def isMD5(self, value) -> bool:
         """ check if the string is MD5 or not """
         pass
 
-   
-    def isPort(self, value):
+    def isPort(self, value: int) -> bool:
         """ check if the string is port or not
         A port number is a 16-bit unsigned integer,
         so it has a minimum value of 0 and a maximum value of 65535.
         """
         if value.isdigit() and 0 <= int(value) <= 65535:
             return True
         return False
 
-    def isSlug(self, value):
+    def isSlug(self, value: str) -> bool:
         """ check if the string is slug or not """
-        pass
+        regex = "^[a-z0-9-]+$"
+        if re.match(regex, value):
+            return True
+        return False
 
-    def isStrongPassword(self, value):
+    def isStrongPassword(self, value: str) -> bool:
         """ check if the string is strong password or not
 
         requirements:
             1. At least 8 characters long
             2. At least one uppercase letter
             3. At least one lowercase letter
             4. At least one number
@@ -371,85 +372,83 @@
             return False
 
         if not re.search("[_@$]", value):
             return False
 
         return True
 
-    def isUUID(self, value):
+    def isUUID(self, value: str) -> bool:
         """ check if the string is UUID or not """
         pass
 
-    # Sanitizers functions
     def toDate(self, value):  # need to improve this function
         """ convert string to date """
         format = '%Y-%m-%d'
         if self.isDate(value):
             date = datetime.strptime(value, format)
             return date
-        
+
         else:
             return None
-        
-    
+
     def toInt(self, value):
         """ convert string to int """
         if isinstance(value, int):
             return value
-        
+
         elif isinstance(value, float):
             return int(value)
-        
+
         try:
             value = int(float(value))
             return value
-        
+
         except ValueError:
             value = 0
-        
+
         return value
 
     def trim(self, value):
         """ trim string """
         if self.__isvalidString(value):
             return value.strip()
-        
+
     def ltrim(self, value):
         if self.__isvalidString(value):
             return value.lstrip()
-        
+
     def rtrim(self, value):
         if self.__isvalidString(value):
             return value.rstrip()
-        
+
     def toUpperCase(self, value):
         """ convert string to upper case """
         if self.__isvalidString(value):
             return value.upper()
 
     def toLowerCase(self, value):
         """ convert string to lower case """
         if self.__isvalidString(value):
             return value.lower()
 
     def removeSpaces(self, value):
         """ remove spaces from string """
         if self.__isvalidString(value):
             return value.replace(" ", "")
-        
+
     def removeSymbols(self, value):
         """ remove symbols from string """
         if self.__isvalidString(value):
             return re.sub(r'[^\w\s]', '', value)
-    
+
     def levenshtein_distance(self, value1, value2):
         """ calculate distance between two strings """
         distance = levenshtein_distance(value1, value2)
         return distance
-    
+
     def edit_distance(self, value1, value2):
         """ calculate distance between two strings """
         if len(value1) > len(value2):
             difference = len(value1) - len(value2)
 
         elif len(value2) > len(value1):
             difference = len(value2) - len(value1)
@@ -468,15 +467,15 @@
         if self.__isvalidString(value):
             return value.encode("ascii", "ignore").decode()
 
     def removeNonWord(self, value):
         """ remove non word characters from string """
         if self.__isvalidString(value):
             return re.sub(r'[^\w]', '', value)
-        
+
     def removeNonNumeric(self, value):
         """ remove non numeric characters from string """
         if self.__isvalidString(value):
             return re.sub(r'[^\d]', '', value)
 
     def removeTags(self, value):
         """ remove tags from string """
```

### Comparing `Sanatio-0.0.1/sanatio/utils.py` & `Sanatio-1.0.0/sanatio/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import json
 import re
 
-ROOT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+ROOT_DIR = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 ASSETS_DIR = os.path.join(ROOT_DIR, 'sanatio/assets')
 
 
 def load_json(filename):
     if not os.path.exists(filename):
         raise FileNotFoundError(f'File {filename} not found')
     
@@ -18,7 +18,9 @@
     
 
 def load_asset(filename):
     return load_json(os.path.join(ASSETS_DIR, filename))
 
 all_country = load_asset('country.json')
 regexs = load_asset('regex.json')
+
+
```

### Comparing `Sanatio-0.0.1/setup.py` & `Sanatio-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 from glob import glob
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
+with open("README.md", "rb") as fh:
+    long_description = fh.read().decode("utf-8")
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.read().splitlines()
 
 setuptools.setup(
     name="Sanatio",
-    version="0.0.1",
+    version="1.0.0",
     author="Deepak Raj",
     author_email="deepak008@live.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Py-Contributors/validator.py",
     data_files=[('assets', glob('sanatio/assets/*'))],
```

