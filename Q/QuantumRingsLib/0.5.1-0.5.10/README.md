# Comparing `tmp/QuantumRingsLib-0.5.1-cp311-cp311-win_amd64.whl.zip` & `tmp/QuantumRingsLib-0.5.10-cp310-cp310-manylinux_2_34_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1322583 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat  3282432 b- defN 24-May-31 17:50 QuantumRingsLib.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat    11097 b- defN 24-May-31 17:55 QuantumRingsLib-0.5.1.dist-info/LICENSE.rst
--rw-rw-rw-  2.0 fat    20473 b- defN 24-May-31 17:55 QuantumRingsLib-0.5.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 24-May-31 17:55 QuantumRingsLib-0.5.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 24-May-31 17:55 QuantumRingsLib-0.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      528 b- defN 24-May-31 17:55 QuantumRingsLib-0.5.1.dist-info/RECORD
-6 files, 3314648 bytes uncompressed, 1321629 bytes compressed:  60.1%
+Zip file size: 1477282 bytes, number of entries: 6
+-rw-r--r--  2.0 unx  4702392 b- defN 24-May-31 18:45 QuantumRingsLib.cpython-310-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx    11097 b- defN 24-May-31 18:48 QuantumRingsLib-0.5.10.dist-info/LICENSE.rst
+-rw-r--r--  2.0 unx    20109 b- defN 24-May-31 18:48 QuantumRingsLib-0.5.10.dist-info/METADATA
+-rw-r--r--  2.0 unx      114 b- defN 24-May-31 18:48 QuantumRingsLib-0.5.10.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-May-31 18:48 QuantumRingsLib-0.5.10.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      545 b- defN 24-May-31 18:48 QuantumRingsLib-0.5.10.dist-info/RECORD
+6 files, 4734273 bytes uncompressed, 1476294 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: QuantumRingsLib.cp311-win_amd64.pyd
+Filename: QuantumRingsLib.cpython-310-x86_64-linux-gnu.so
 Comment: 
 
-Filename: QuantumRingsLib-0.5.1.dist-info/LICENSE.rst
+Filename: QuantumRingsLib-0.5.10.dist-info/LICENSE.rst
 Comment: 
 
-Filename: QuantumRingsLib-0.5.1.dist-info/METADATA
+Filename: QuantumRingsLib-0.5.10.dist-info/METADATA
 Comment: 
 
-Filename: QuantumRingsLib-0.5.1.dist-info/WHEEL
+Filename: QuantumRingsLib-0.5.10.dist-info/WHEEL
 Comment: 
 
-Filename: QuantumRingsLib-0.5.1.dist-info/top_level.txt
+Filename: QuantumRingsLib-0.5.10.dist-info/top_level.txt
 Comment: 
 
-Filename: QuantumRingsLib-0.5.1.dist-info/RECORD
+Filename: QuantumRingsLib-0.5.10.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `QuantumRingsLib-0.5.1.dist-info/LICENSE.rst` & `QuantumRingsLib-0.5.10.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `QuantumRingsLib-0.5.1.dist-info/METADATA` & `QuantumRingsLib-0.5.10.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,359 +1,359 @@
-Metadata-Version: 2.1
-Name: QuantumRingsLib
-Version: 0.5.1
-Summary: A Quantum Development Library
-Author-email: "Quantum Rings Inc." <contact@quantumrings.com>
-License: 
-        ====================
-        EVALUATION AGREEMENT
-        ====================
-        
-        **IMPORTANT:** PLEASE READ THIS EVALUATION AGREEMENT ("**AGREEMENT**") BEFORE CLICKING THE "ACCEPT" BUTTON, AND/OR USING
-        THE QUANTUM RINGS, INC. (**"QUANTUM"**) PRODUCT THAT ACCOMPANIES OR IS PROVIDED IN CONNECTION WITH THIS AGREEMENT. BY
-        CLICKING THE "ACCEPT" BUTTON, AND/OR USING THE SERVICES IN ANY WAY, YOU AND THE ENTITY THAT YOU REPRESENT ("**EVALUATOR**")
-        IS UNCONDITIONALLY CONSENTING TO BE BOUND BY AND IS BECOMING A PARTY TO THIS AGREEMENT WITH QUANTUM AND YOU REPRESENT
-        AND WARRANT THAT YOU HAVE THE AUTHORITY TO BIND SUCH ENTITY TO THESE TERMS. IF EVALUATOR DOES NOT UNCONDITIONALLY AGREE
-        TO ALL OF THE TERMS OF THIS AGREEMENT, USE OF THE SERVICES IS STRICTLY PROHIBITED. IF EVALUATOR HAS EXECUTED, OR
-        SUBSEQUENTLY EXECUTES, AN EVALUATION AGREEMENT OR AN END USER AGREEMENT WITH QUANTUM, THEN THE TERMS AND
-        CONDITIONS OF SUCH EXECUTED EVALUATION AGREEMENT OR END USER AGREEMENT, AS APPLICABLE, SHALL GOVERN AND CONTROL
-        YOUR USE OF THE PRODUCT.
-        
-        1. **BETA SERVICES**. Quantum is developing a proprietary, set of development tools for quantum computing (the
-        "**Services**"). Evaluator wishes to utilize an evaluation "beta" version of the Services, and Quantum desires to make a beta
-        version of the Services available to Evaluator, subject to the following terms and conditions. Subject to the terms and
-        conditions of this Agreement, Quantum hereby grants Evaluator, during the Term (as defined below), non-exclusive,
-        non-transferable, non-sublicensable right and license to access and use the Services solely for the purpose of evaluating the
-        performance and functionality of the Services (the "**Limited Purpose**"). Evaluator agrees to use and evaluate the Services for
-        a period of ninty days or such other period of time as mutually agreed by the parties in writing (the "**Term**"). Quantum's
-        services outside the scope of this Agreement, if any, shall be provided pursuant to Quantum's then-current applicable services
-        policies and procedures ("**Other Terms**"). Nothing in any of Quantum's Other Terms or any other existing agreements that
-        Evaluator may have with Quantum apply to or are applicable to this Agreement, or Evaluator's use of the Services offered
-        hereunder.
-        
-        2. **INTELLECTUAL PROPERTY.** The Services (excluding the Evaluator Content hosted thereon), Documentation, and all
-        other materials provided by Quantum hereunder, including but not limited to all manuals, reports, records, programs, data and
-        other materials, and all intellectual property rights in each of the foregoing, are the exclusive property of Quantum and its
-        suppliers. Evaluator agrees that it will not, and will not permit any other party to: (a) permit any party to access the Services
-        or any accompanying documentation ("**Documentation**"); (b) modify, adapt, alter or translate the Services or
-        Documentation; (c) sublicense, lease, rent, loan, distribute, or otherwise transfer the Services or Documentation to any third
-        party; (d) reverse engineer, decompile, disassemble, or otherwise derive or determine or attempt to derive or determine the
-        source code (or the underlying ideas, algorithms, structure or organization) of the Services; (e) use or copy the Services or
-        Documentation except for the Limited Purpose; or (f) publish or disclose to any third party any performance benchmark tests
-        or analyses or other non-public information relating to the Services or the use thereof.
-        
-        3. **FEEDBACK.** Evaluator understands and agrees that the Services represent a beta test version of unreleased software
-        and services that may contain bugs, defects, and errors. In exchange for the licenses granted to Evaluator to use such
-        software, Evaluator agrees to use good faith efforts to test, use, and evaluate the Services in live operations, and to promptly
-        report to Quantum, either orally or in writing, any errors, problems, defects, or suggestions for changes and improvements to
-        the Services (collectively, "**Feedback**"). Evaluator acknowledges and agrees that all Feedback and all intellectual property
-        rights therein are the exclusive property of Quantum, and hereby assigns to Quantum, all right, title and interest to any and all
-        Feedback. Further, Evaluator acknowledges and agrees that Feedback may be used by Quantum in Quantum's development
-        of and be incorporated into a version of the Services Quantum may make available for commercial distribution
-        ("**Commercial Release**") or any other software or intellectual property created by Quantum. Without limiting the foregoing,
-        Quantum may incorporate Feedback into its products and services and Evaluator will gain no rights in such products or
-        services by virtue of having disclosed Feedback. Evaluator agrees and acknowledges that the products and services
-        incorporating such Feedback will be the sole and exclusive property of Quantum, and Evaluator will gain no right, title or
-        interest in or to the Services, Documentation or any Commercial Release by virtue of Evaluator's provision of Feedback to
-        Quantum or for any other reason. Quantum has no obligation to create, distribute or otherwise offer a Commercial Release,
-        and in the event of such Commercial Release, Quantum has no obligation to offer the Commercial Release to Evaluator or to
-        offer Evaluator any discounted pricing schedules or special terms. Evaluator understands and agrees that the Commercial
-        Release may contain functions and functionality, and perform in a manner significantly different from the current beta version
-        of the Services. Accordingly, Evaluator acknowledges that any research or development performed, or business plans made,
-        by Evaluator regarding or in reliance upon the Services are done entirely at Evaluator's own risk.
-        
-        4. **DISCLAIMERS OF WARRANTIES.** Evaluator acknowledges that the Services contain prerelease code for testing
-        purposes only and are not at the level of performance and compatibility of a final, generally available product offering.
-        Furthermore, Evaluator acknowledges that the Services may contain bugs, errors, omissions and other problems that could
-        cause system or other failures and data loss. Evaluator acknowledges that Quantum may not introduce a product similar to or
-        compatible with the Services. Accordingly, Evaluator acknowledges that any research, development or other work that
-        
-        
-        Evaluator performs regarding the Services is done entirely at Evaluator's own risk. To the maximum extent permitted by law,
-        the Services, and all other documentation and materials are provided "AS IS" AND WITH ALL FAULTS. QUANTUM
-        MAKES NO WARRANTIES WITH RESPECT TO THE SERVICES OR DOCUMENTATION, WHETHER EXPRESS OR
-        IMPLIED, INCLUDING WARRANTIES OF TITLE, ACCURACY, INTERFERENCE WITH EVALUATOR'S QUIET
-        ENJOYMENT, SYSTEM INTEGRATION, NON-INFRINGEMENT, MERCHANTABILITY OR FITNESS FOR A
-        PARTICULAR PURPOSE. THE ENTIRE RISK ARISING OUT OF THE USE OR PERFORMANCE OF THE SERVICES
-        IS WITH EVALUATOR NO ORAL OR WRITTEN INFORMATION OR ADVICE GIVEN BY QUANTUM OR ITS
-        AGENTS OR EMPLOYEES SHALL IN ANY WAY INCREASE THE SCOPE OF THIS WARRANTY.
-        
-        5. **LIMITATION OF LIABILITY.** IN NO EVENT WILL QUANTUM OR ITS LICENSORS (IF ANY) BE LIABLE TO
-        EVALUATOR OR ANY THIRD PARTY FOR THE COST OF PROCUREMENT OF SUBSTITUTE SERVICES, LOST
-        PROFITS, LOST DATA, OR ANY SPECIAL, INDIRECT, CONSEQUENTIAL, INCIDENTAL OR PUNITIVE
-        DAMAGES, HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY ARISING IN ANY WAY OUT OF THIS
-        AGREEMENT OR EVALUATOR'S USE OF THE SERVICES, EVEN IF QUANTUM HAS BEEN ADVISED OF THE
-        POSSIBILITY OF SUCH DAMAGES. THE TOTAL CUMULATIVE LIABILITY, RELATED TO THIS AGREEMENT,
-        OF QUANTUM AND ITS LICENSORS (IF ANY) SHALL BE LIMITED TO FIFTY DOLLARS (U.S. $50). The parties
-        agree that the limitations of liability set forth in this section shall survive and continue in full force and effect despite any
-        failure of consideration or of an exclusive remedy. The parties acknowledge that the prices have been set and the Agreement
-        entered into in reliance upon these limitations of liability and that all such limitations form an essential basis of the bargain
-        between the parties.
-        
-        6. **CONFIDENTIALITY.** The structure, sequence, organization and code of the software used to provide the Services
-        constitute valuable trade secrets of Quantum and its suppliers. Evaluator will not disclose to any third party: any information
-        about the Services, including its existence, design, performance characteristics, feedback, and test results. Evaluator will use
-        reasonable efforts to prevent any access to the Services by anyone other than its employees who are obligated to comply with
-        the terms hereof.
-        
-        7. **PRODUCT DIAGNOSTIC REPORTING.** Evaluator acknowledges that the Services will store certain diagnostic information
-        about the routine operations of the Services (including, without limitation, its performance, data reduction ratios,
-        configuration data, and any software faults) and will periodically transmit this diagnostic information to Quantum. Evaluator
-        agrees that Quantum has a perpetual, irrevocable, worldwide, sublicenseable, and royalty-free right to use this diagnostic
-        information in any manner and that Evaluator will not interfere with the collection or transmission of such information to
-        Quantum. For clarification, there is no actual user data of Evaluator that is transmitted or provided to Quantum.
-        
-        8. **TERM AND TERMINATION.** This Agreement commences upon the Effective Date and will continue in effect until the
-        end of the Term. Either party may terminate this Agreement upon written notice to the other party. Upon termination,
-        Evaluator shall immediately cease all use of Services, and delete or destroy all copies of the Documentation in the possession
-        or control of Evaluator.
-        
-        9. **GENERAL PROVISIONS.** This Agreement will be governed by the laws of the State of Colorado. Evaluator submits to
-        the exclusive jurisdiction and venue of the federal and state courts located in Denver County, Colorado for any disputes
-        arising out of or related to this Agreement. Evaluator may not assign or transfer, by operation of law, change of control or
-        otherwise, any of its rights under this Agreement to any third party without Quantum's prior written consent. Any attempted
-        assignment or transfer in violation of the foregoing will be void. All waivers must be in writing. Any waiver or failure to
-        enforce any provision of this Agreement on one occasion will not be deemed a waiver of any other provision or of such
-        provision on any other occasion. If any part of this Agreement is found void and unenforceable, it will not affect the validity
-        of the balance of this Agreement, which shall remain valid and enforceable according to its terms. If any provision of this
-        Agreement is, for any reason, held to be invalid or unenforceable, the other provisions of this Agreement will remain
-        enforceable and the invalid or unenforceable provision will be deemed modified so that it is valid and enforceable to the
-        maximum extent permitted by law.
-Project-URL: Homepage, https://www.quantumrings.com/docs
-Project-URL: Documentation, https://www.quantumrings.com/docs
-Project-URL: API Reference, https://quantumrings.com/doc/modules.html
-Keywords: quantum,quantum circuit,quantum computing,quantum programming language,quantum register,quantum tools,tools,sdk
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Scientific/Engineering
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: ==3.11.*
-Description-Content-Type: text/x-rst
-License-File: LICENSE.rst
-
-
-.. _minimum-system-requirements:
-
-Minimum System Requirements
----------------------------
-
-A system with a configuration better than the minimum requirements is advised. 
-Lower configurations may affect the number of qubits that can be supported and
-may perform poorly.
-
--  Operating systems supported:
-
-   -  Windows 11 Pro
-   -  Debian GNU/Linux 12 (bookworm)
-   -  OpenSUSE Tumbleweed - Version 20240415
-   -  Oracle Linux 9.3
-   -  Ubuntu 22.04.4 LTS
-
--  64-bit Intel i9 x86 CPU (14 cores 20 logical processors recommended)
-
--  32 GB Installed physical memory
-
--  18 GB Available physical memory
-
--  64-bit Python version 3.11
-
-
-=========================
-Installation - Windows 11
-=========================
-
-The Quantum Rings SDK can be installed directly using pip. 
-Many users find Anaconda (https://www.anaconda.com/) a good way to install the Quantum Rings SDK and use the Python environment efficiently.
-From Anaconda, select a Python 3.11 channel and launch `CMD.exe Prompt` to go to the
-command prompt and execute the following command.
-
-.. code-block:: console
-
-    pip install QuantumRingsLib
-
-
-If you do not have a Python 3.11 channel, select `Environments` from the left panel, `+ Create` button from the menu bar
-at the bottom and select Python 3.11 from the `Create New Environment` dialog.
-
-Quantum Rings SDK requires a 64-bit version of Python 3.11.
-
-After installation of the SDK, launch Python 3.11 environment by selecting the installed channel, before running your code.
-
-====================
-Installation - Linux
-====================
-
-Checking whether your Linux platform is supported
--------------------------------------------------
-
-There are several variants of the Linux OS, with varying levels of inbuilt libraries. At present, we are supporting `manylinux_2_34_x86_64` platforms 
-based on 64 bit x86 processors. 
-Older platforms and other CPUs are not supported at the moment. If you have a specific requirement, please contact our technical support.
-
-To check whether your platform is supported, execute the following command from Python command line:
-
-.. code-block:: console
-
-    import platform
-    platform.platform()
-
-Watch for the `glibc` signature at the end. glibc2.34 and above are only supported.
-
-Installing Python 3.11 and creating the virtual environment
------------------------------------------------------------
-    
-Update all packages in your system using the following commands. Note that, this may cause incompatibilities in some installations due to variances 
-in packages and their mutual dependencies. Besides, this step might break existing software packages and make your system unusable. 
-You may refer to your operating system's manual or seek help from your system adminstrator. Alternatively, you can also use the Software Updater GUI tool,
-if that was packaged along with your system distribution.
-
-.. code-block:: console
-
-    sudo apt update        # Fetches the list of available updates
-    sudo apt upgrade       # Installs some updates; does not remove packages
-
-Note that `apt` command is not available in some Linux variants. You may have to use `dnf` on Oracle Linux distributions and `zypper` on Open SUSE distributions.
-
-
-Check whether your system has Python 3.11 installed by executing `python` from the terminal. If not, you can install Python 3.11 using the following command.
-
-.. code-block:: console
-
-    sudo apt install python3.11
-
-Create a virtual Python 3.11 environment and activate the environment using the following steps.
-
-.. code-block:: console
-
-    virtualenv --python=/usr/bin/python3.11 myenv
-    source myenv/bin/activate
-
-You may have to install `virtualenv` package if it is not already installed. When not required, you can deactivate the environment using `deactivate` command.
-
-Note that, `virtualenv` package is not available on Oracle Linux and Open SUSE Linux. You can use the following command equivalently on these distributions:
-
-.. code-block:: console
-
-    python3.11 -m venv myenv
-    source myenv/bin/activate
-
-
-Installing Jupyter notebook
----------------------------
-
-Now, launch the virtual environment, and execute the following command:
-
-.. code-block:: console
-
-    sudo su
-    source myenv/bin/activate
-    pip install notebook
-
-
-Ensuring that jupyter notebook launches the correct python version
-------------------------------------------------------------------
-
-Check whether your virtual environment launches the correct python version (3.11) my executing the command `python --version`. On some installations you may
-have to execute the following commands to ensure that the Jupyter notebook launches the correct python version. 
-
-.. code-block:: console
-
-    python -m pip install ipykernel
-    python -m ipykernel install --user
-
-Now, you can launch the Jupyter notebook using the command `jupyter-notebook` or `jupyter notebook`.  If you are logged in as `root`, then you may have to
-append `--allow-root`. Once the notebook server starts, you can click the local-host link to launch the notebook on the browser.
-
-
-Installing Curl
----------------
-
-On some installations, we found that curl was not installed. You can check whether curl is installed on your system by executing the command `curl` from the terminal. 
-If `curl` is not installed, you may use the following command:
-
-.. code-block:: console
-
-    sudo apt install curl
-
-Installing gcc
---------------
-
-On some installations, we got `libgomp.so` not found error and it required installation of gcc, as follows:
-
-.. code-block:: console
-
-    zypper install gcc
-
-
-Finally, installing the QuantumRingsLibrary
--------------------------------------------
-
-Now, you can install the QuantumRingsLibrary as follows:
-
-.. code-block:: console
-
-    pip install QuantumRingsLib
-
-
-=====
-Usage
-=====
-
-Obtain your account name and token from the Quantum Rings team. You can then use them to create the backend for execution.
-You can follow the reference code below for further information:
-
-
-.. code-block:: python
-        
-    import QuantumRingsLib
-    from QuantumRingsLib import QuantumRegister, AncillaRegister, ClassicalRegister, QuantumCircuit
-    from QuantumRingsLib import QuantumRingsProvider
-    from QuantumRingsLib import job_monitor
-    from QuantumRingsLib import JobStatus
-    from matplotlib import pyplot as plt
-    import numpy as np
-
-    provider = QuantumRingsProvider(token =<YOUR_TOKEN_HERE>, name=<YOUR_ACCOUNT_NAME_HERE>)
-    backend = provider.get_backend("scarlet_quantum_rings")
-    shots = 100
-
-    provider.active_account()
-
-
-
-==================
-Executing the Code
-==================
-
-You can execute the code in the backend as illustrated below and setup a job monitor to watch for completion. The code is executed in a background thread so
-you can use your system normally.
-
-*Using job_monitor function*
-
-.. code-block:: python
-
-    job = backend.run(qc, shots)
-    job_monitor(job)
-    result = job.result()
-    counts = result.get_counts()
-    print (counts)
-
-
-*Using wait_for_final_state function*
-
-.. code-block:: python
-
-    def jobCallback(job_id, state, job):
-        #print("Job Status: ", state)
-        pass
-
-    # Execute the circuit
-    job = backend.run(qc, shots)
-    job.wait_for_final_state(0, 5, jobCallback)
-    counts = job.result().get_counts() 
-
-
-
+Metadata-Version: 2.1
+Name: QuantumRingsLib
+Version: 0.5.10
+Summary: A Quantum Development Library
+Author-email: "Quantum Rings Inc." <contact@quantumrings.com>
+License: 
+        ====================
+        EVALUATION AGREEMENT
+        ====================
+        
+        **IMPORTANT:** PLEASE READ THIS EVALUATION AGREEMENT ("**AGREEMENT**") BEFORE CLICKING THE "ACCEPT" BUTTON, AND/OR USING
+        THE QUANTUM RINGS, INC. (**"QUANTUM"**) PRODUCT THAT ACCOMPANIES OR IS PROVIDED IN CONNECTION WITH THIS AGREEMENT. BY
+        CLICKING THE "ACCEPT" BUTTON, AND/OR USING THE SERVICES IN ANY WAY, YOU AND THE ENTITY THAT YOU REPRESENT ("**EVALUATOR**")
+        IS UNCONDITIONALLY CONSENTING TO BE BOUND BY AND IS BECOMING A PARTY TO THIS AGREEMENT WITH QUANTUM AND YOU REPRESENT
+        AND WARRANT THAT YOU HAVE THE AUTHORITY TO BIND SUCH ENTITY TO THESE TERMS. IF EVALUATOR DOES NOT UNCONDITIONALLY AGREE
+        TO ALL OF THE TERMS OF THIS AGREEMENT, USE OF THE SERVICES IS STRICTLY PROHIBITED. IF EVALUATOR HAS EXECUTED, OR
+        SUBSEQUENTLY EXECUTES, AN EVALUATION AGREEMENT OR AN END USER AGREEMENT WITH QUANTUM, THEN THE TERMS AND
+        CONDITIONS OF SUCH EXECUTED EVALUATION AGREEMENT OR END USER AGREEMENT, AS APPLICABLE, SHALL GOVERN AND CONTROL
+        YOUR USE OF THE PRODUCT.
+        
+        1. **BETA SERVICES**. Quantum is developing a proprietary, set of development tools for quantum computing (the
+        "**Services**"). Evaluator wishes to utilize an evaluation "beta" version of the Services, and Quantum desires to make a beta
+        version of the Services available to Evaluator, subject to the following terms and conditions. Subject to the terms and
+        conditions of this Agreement, Quantum hereby grants Evaluator, during the Term (as defined below), non-exclusive,
+        non-transferable, non-sublicensable right and license to access and use the Services solely for the purpose of evaluating the
+        performance and functionality of the Services (the "**Limited Purpose**"). Evaluator agrees to use and evaluate the Services for
+        a period of ninty days or such other period of time as mutually agreed by the parties in writing (the "**Term**"). Quantum's
+        services outside the scope of this Agreement, if any, shall be provided pursuant to Quantum's then-current applicable services
+        policies and procedures ("**Other Terms**"). Nothing in any of Quantum's Other Terms or any other existing agreements that
+        Evaluator may have with Quantum apply to or are applicable to this Agreement, or Evaluator's use of the Services offered
+        hereunder.
+        
+        2. **INTELLECTUAL PROPERTY.** The Services (excluding the Evaluator Content hosted thereon), Documentation, and all
+        other materials provided by Quantum hereunder, including but not limited to all manuals, reports, records, programs, data and
+        other materials, and all intellectual property rights in each of the foregoing, are the exclusive property of Quantum and its
+        suppliers. Evaluator agrees that it will not, and will not permit any other party to: (a) permit any party to access the Services
+        or any accompanying documentation ("**Documentation**"); (b) modify, adapt, alter or translate the Services or
+        Documentation; (c) sublicense, lease, rent, loan, distribute, or otherwise transfer the Services or Documentation to any third
+        party; (d) reverse engineer, decompile, disassemble, or otherwise derive or determine or attempt to derive or determine the
+        source code (or the underlying ideas, algorithms, structure or organization) of the Services; (e) use or copy the Services or
+        Documentation except for the Limited Purpose; or (f) publish or disclose to any third party any performance benchmark tests
+        or analyses or other non-public information relating to the Services or the use thereof.
+        
+        3. **FEEDBACK.** Evaluator understands and agrees that the Services represent a beta test version of unreleased software
+        and services that may contain bugs, defects, and errors. In exchange for the licenses granted to Evaluator to use such
+        software, Evaluator agrees to use good faith efforts to test, use, and evaluate the Services in live operations, and to promptly
+        report to Quantum, either orally or in writing, any errors, problems, defects, or suggestions for changes and improvements to
+        the Services (collectively, "**Feedback**"). Evaluator acknowledges and agrees that all Feedback and all intellectual property
+        rights therein are the exclusive property of Quantum, and hereby assigns to Quantum, all right, title and interest to any and all
+        Feedback. Further, Evaluator acknowledges and agrees that Feedback may be used by Quantum in Quantum's development
+        of and be incorporated into a version of the Services Quantum may make available for commercial distribution
+        ("**Commercial Release**") or any other software or intellectual property created by Quantum. Without limiting the foregoing,
+        Quantum may incorporate Feedback into its products and services and Evaluator will gain no rights in such products or
+        services by virtue of having disclosed Feedback. Evaluator agrees and acknowledges that the products and services
+        incorporating such Feedback will be the sole and exclusive property of Quantum, and Evaluator will gain no right, title or
+        interest in or to the Services, Documentation or any Commercial Release by virtue of Evaluator's provision of Feedback to
+        Quantum or for any other reason. Quantum has no obligation to create, distribute or otherwise offer a Commercial Release,
+        and in the event of such Commercial Release, Quantum has no obligation to offer the Commercial Release to Evaluator or to
+        offer Evaluator any discounted pricing schedules or special terms. Evaluator understands and agrees that the Commercial
+        Release may contain functions and functionality, and perform in a manner significantly different from the current beta version
+        of the Services. Accordingly, Evaluator acknowledges that any research or development performed, or business plans made,
+        by Evaluator regarding or in reliance upon the Services are done entirely at Evaluator's own risk.
+        
+        4. **DISCLAIMERS OF WARRANTIES.** Evaluator acknowledges that the Services contain prerelease code for testing
+        purposes only and are not at the level of performance and compatibility of a final, generally available product offering.
+        Furthermore, Evaluator acknowledges that the Services may contain bugs, errors, omissions and other problems that could
+        cause system or other failures and data loss. Evaluator acknowledges that Quantum may not introduce a product similar to or
+        compatible with the Services. Accordingly, Evaluator acknowledges that any research, development or other work that
+        
+        
+        Evaluator performs regarding the Services is done entirely at Evaluator's own risk. To the maximum extent permitted by law,
+        the Services, and all other documentation and materials are provided "AS IS" AND WITH ALL FAULTS. QUANTUM
+        MAKES NO WARRANTIES WITH RESPECT TO THE SERVICES OR DOCUMENTATION, WHETHER EXPRESS OR
+        IMPLIED, INCLUDING WARRANTIES OF TITLE, ACCURACY, INTERFERENCE WITH EVALUATOR'S QUIET
+        ENJOYMENT, SYSTEM INTEGRATION, NON-INFRINGEMENT, MERCHANTABILITY OR FITNESS FOR A
+        PARTICULAR PURPOSE. THE ENTIRE RISK ARISING OUT OF THE USE OR PERFORMANCE OF THE SERVICES
+        IS WITH EVALUATOR NO ORAL OR WRITTEN INFORMATION OR ADVICE GIVEN BY QUANTUM OR ITS
+        AGENTS OR EMPLOYEES SHALL IN ANY WAY INCREASE THE SCOPE OF THIS WARRANTY.
+        
+        5. **LIMITATION OF LIABILITY.** IN NO EVENT WILL QUANTUM OR ITS LICENSORS (IF ANY) BE LIABLE TO
+        EVALUATOR OR ANY THIRD PARTY FOR THE COST OF PROCUREMENT OF SUBSTITUTE SERVICES, LOST
+        PROFITS, LOST DATA, OR ANY SPECIAL, INDIRECT, CONSEQUENTIAL, INCIDENTAL OR PUNITIVE
+        DAMAGES, HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY ARISING IN ANY WAY OUT OF THIS
+        AGREEMENT OR EVALUATOR'S USE OF THE SERVICES, EVEN IF QUANTUM HAS BEEN ADVISED OF THE
+        POSSIBILITY OF SUCH DAMAGES. THE TOTAL CUMULATIVE LIABILITY, RELATED TO THIS AGREEMENT,
+        OF QUANTUM AND ITS LICENSORS (IF ANY) SHALL BE LIMITED TO FIFTY DOLLARS (U.S. $50). The parties
+        agree that the limitations of liability set forth in this section shall survive and continue in full force and effect despite any
+        failure of consideration or of an exclusive remedy. The parties acknowledge that the prices have been set and the Agreement
+        entered into in reliance upon these limitations of liability and that all such limitations form an essential basis of the bargain
+        between the parties.
+        
+        6. **CONFIDENTIALITY.** The structure, sequence, organization and code of the software used to provide the Services
+        constitute valuable trade secrets of Quantum and its suppliers. Evaluator will not disclose to any third party: any information
+        about the Services, including its existence, design, performance characteristics, feedback, and test results. Evaluator will use
+        reasonable efforts to prevent any access to the Services by anyone other than its employees who are obligated to comply with
+        the terms hereof.
+        
+        7. **PRODUCT DIAGNOSTIC REPORTING.** Evaluator acknowledges that the Services will store certain diagnostic information
+        about the routine operations of the Services (including, without limitation, its performance, data reduction ratios,
+        configuration data, and any software faults) and will periodically transmit this diagnostic information to Quantum. Evaluator
+        agrees that Quantum has a perpetual, irrevocable, worldwide, sublicenseable, and royalty-free right to use this diagnostic
+        information in any manner and that Evaluator will not interfere with the collection or transmission of such information to
+        Quantum. For clarification, there is no actual user data of Evaluator that is transmitted or provided to Quantum.
+        
+        8. **TERM AND TERMINATION.** This Agreement commences upon the Effective Date and will continue in effect until the
+        end of the Term. Either party may terminate this Agreement upon written notice to the other party. Upon termination,
+        Evaluator shall immediately cease all use of Services, and delete or destroy all copies of the Documentation in the possession
+        or control of Evaluator.
+        
+        9. **GENERAL PROVISIONS.** This Agreement will be governed by the laws of the State of Colorado. Evaluator submits to
+        the exclusive jurisdiction and venue of the federal and state courts located in Denver County, Colorado for any disputes
+        arising out of or related to this Agreement. Evaluator may not assign or transfer, by operation of law, change of control or
+        otherwise, any of its rights under this Agreement to any third party without Quantum's prior written consent. Any attempted
+        assignment or transfer in violation of the foregoing will be void. All waivers must be in writing. Any waiver or failure to
+        enforce any provision of this Agreement on one occasion will not be deemed a waiver of any other provision or of such
+        provision on any other occasion. If any part of this Agreement is found void and unenforceable, it will not affect the validity
+        of the balance of this Agreement, which shall remain valid and enforceable according to its terms. If any provision of this
+        Agreement is, for any reason, held to be invalid or unenforceable, the other provisions of this Agreement will remain
+        enforceable and the invalid or unenforceable provision will be deemed modified so that it is valid and enforceable to the
+        maximum extent permitted by law.
+Project-URL: Homepage, https://www.quantumrings.com/docs
+Project-URL: Documentation, https://www.quantumrings.com/docs
+Project-URL: API Reference, https://quantumrings.com/doc/modules.html
+Keywords: quantum,quantum circuit,quantum computing,quantum programming language,quantum register,quantum tools,tools,sdk
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: ==3.10.*
+Description-Content-Type: text/x-rst
+License-File: LICENSE.rst
+
+
+.. _minimum-system-requirements:
+
+Minimum System Requirements
+---------------------------
+
+A system with a configuration better than the minimum requirements is advised. 
+Lower configurations may affect the number of qubits that can be supported and
+may perform poorly.
+
+-  Operating systems supported:
+
+   -  Windows 11 Pro
+   -  Debian GNU/Linux 12 (bookworm)
+   -  OpenSUSE Tumbleweed - Version 20240415
+   -  Oracle Linux 9.3
+   -  Ubuntu 22.04.4 LTS
+
+-  64-bit Intel i9 x86 CPU (14 cores 20 logical processors recommended)
+
+-  32 GB Installed physical memory
+
+-  18 GB Available physical memory
+
+-  64-bit Python version 3.11
+
+
+=========================
+Installation - Windows 11
+=========================
+
+The Quantum Rings SDK can be installed directly using pip. 
+Many users find Anaconda (https://www.anaconda.com/) a good way to install the Quantum Rings SDK and use the Python environment efficiently.
+From Anaconda, select a Python 3.11 channel and launch `CMD.exe Prompt` to go to the
+command prompt and execute the following command.
+
+.. code-block:: console
+
+    pip install QuantumRingsLib
+
+
+If you do not have a Python 3.11 channel, select `Environments` from the left panel, `+ Create` button from the menu bar
+at the bottom and select Python 3.11 from the `Create New Environment` dialog.
+
+Quantum Rings SDK requires a 64-bit version of Python 3.11.
+
+After installation of the SDK, launch Python 3.11 environment by selecting the installed channel, before running your code.
+
+====================
+Installation - Linux
+====================
+
+Checking whether your Linux platform is supported
+-------------------------------------------------
+
+There are several variants of the Linux OS, with varying levels of inbuilt libraries. At present, we are supporting `manylinux_2_34_x86_64` platforms 
+based on 64 bit x86 processors. 
+Older platforms and other CPUs are not supported at the moment. If you have a specific requirement, please contact our technical support.
+
+To check whether your platform is supported, execute the following command from Python command line:
+
+.. code-block:: console
+
+    import platform
+    platform.platform()
+
+Watch for the `glibc` signature at the end. glibc2.34 and above are only supported.
+
+Installing Python 3.11 and creating the virtual environment
+-----------------------------------------------------------
+    
+Update all packages in your system using the following commands. Note that, this may cause incompatibilities in some installations due to variances 
+in packages and their mutual dependencies. Besides, this step might break existing software packages and make your system unusable. 
+You may refer to your operating system's manual or seek help from your system adminstrator. Alternatively, you can also use the Software Updater GUI tool,
+if that was packaged along with your system distribution.
+
+.. code-block:: console
+
+    sudo apt update        # Fetches the list of available updates
+    sudo apt upgrade       # Installs some updates; does not remove packages
+
+Note that `apt` command is not available in some Linux variants. You may have to use `dnf` on Oracle Linux distributions and `zypper` on Open SUSE distributions.
+
+
+Check whether your system has Python 3.11 installed by executing `python` from the terminal. If not, you can install Python 3.11 using the following command.
+
+.. code-block:: console
+
+    sudo apt install python3.11
+
+Create a virtual Python 3.11 environment and activate the environment using the following steps.
+
+.. code-block:: console
+
+    virtualenv --python=/usr/bin/python3.11 myenv
+    source myenv/bin/activate
+
+You may have to install `virtualenv` package if it is not already installed. When not required, you can deactivate the environment using `deactivate` command.
+
+Note that, `virtualenv` package is not available on Oracle Linux and Open SUSE Linux. You can use the following command equivalently on these distributions:
+
+.. code-block:: console
+
+    python3.11 -m venv myenv
+    source myenv/bin/activate
+
+
+Installing Jupyter notebook
+---------------------------
+
+Now, launch the virtual environment, and execute the following command:
+
+.. code-block:: console
+
+    sudo su
+    source myenv/bin/activate
+    pip install notebook
+
+
+Ensuring that jupyter notebook launches the correct python version
+------------------------------------------------------------------
+
+Check whether your virtual environment launches the correct python version (3.11) my executing the command `python --version`. On some installations you may
+have to execute the following commands to ensure that the Jupyter notebook launches the correct python version. 
+
+.. code-block:: console
+
+    python -m pip install ipykernel
+    python -m ipykernel install --user
+
+Now, you can launch the Jupyter notebook using the command `jupyter-notebook` or `jupyter notebook`.  If you are logged in as `root`, then you may have to
+append `--allow-root`. Once the notebook server starts, you can click the local-host link to launch the notebook on the browser.
+
+
+Installing Curl
+---------------
+
+On some installations, we found that curl was not installed. You can check whether curl is installed on your system by executing the command `curl` from the terminal. 
+If `curl` is not installed, you may use the following command:
+
+.. code-block:: console
+
+    sudo apt install curl
+
+Installing gcc
+--------------
+
+On some installations, we got `libgomp.so` not found error and it required installation of gcc, as follows:
+
+.. code-block:: console
+
+    zypper install gcc
+
+
+Finally, installing the QuantumRingsLibrary
+-------------------------------------------
+
+Now, you can install the QuantumRingsLibrary as follows:
+
+.. code-block:: console
+
+    pip install QuantumRingsLib
+
+
+=====
+Usage
+=====
+
+Obtain your account name and token from the Quantum Rings team. You can then use them to create the backend for execution.
+You can follow the reference code below for further information:
+
+
+.. code-block:: python
+        
+    import QuantumRingsLib
+    from QuantumRingsLib import QuantumRegister, AncillaRegister, ClassicalRegister, QuantumCircuit
+    from QuantumRingsLib import QuantumRingsProvider
+    from QuantumRingsLib import job_monitor
+    from QuantumRingsLib import JobStatus
+    from matplotlib import pyplot as plt
+    import numpy as np
+
+    provider = QuantumRingsProvider(token =<YOUR_TOKEN_HERE>, name=<YOUR_ACCOUNT_NAME_HERE>)
+    backend = provider.get_backend("scarlet_quantum_rings")
+    shots = 100
+
+    provider.active_account()
+
+
+
+==================
+Executing the Code
+==================
+
+You can execute the code in the backend as illustrated below and setup a job monitor to watch for completion. The code is executed in a background thread so
+you can use your system normally.
+
+*Using job_monitor function*
+
+.. code-block:: python
+
+    job = backend.run(qc, shots)
+    job_monitor(job)
+    result = job.result()
+    counts = result.get_counts()
+    print (counts)
+
+
+*Using wait_for_final_state function*
+
+.. code-block:: python
+
+    def jobCallback(job_id, state, job):
+        #print("Job Status: ", state)
+        pass
+
+    # Execute the circuit
+    job = backend.run(qc, shots)
+    job.wait_for_final_state(0, 5, jobCallback)
+    counts = job.result().get_counts() 
+
+
+
```

