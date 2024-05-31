# Comparing `tmp/idinn-0.1.4.tar.gz` & `tmp/idinn-0.1.5.tar.gz`

## Comparing `idinn-0.1.4.tar` & `idinn-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 idinn-0.1.4/.readthedocs.yaml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 idinn-0.1.4/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/Makefile
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/conf.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/make.bat
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/requirements.txt
--rw-r--r--   0        0        0   453134 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/_static/optimization_schematic.png
--rw-r--r--   0        0        0   243113 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/_static/youtube.png
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/get_started/get_started.rst
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/get_started/installation.rst
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/joss/paper.bib
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/joss/paper.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/tutorials/api.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/tutorials/benchmark.rst
--rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/tutorials/dual.rst
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/tutorials/single.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/tutorials/transfer.rst
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/understand/dynamics.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/understand/optimization.rst
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/understand/order.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/understand/straight.rst
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 idinn-0.1.4/src/idinn/__init__.py
--rw-r--r--   0        0        0    23534 2020-02-02 00:00:00.000000 idinn-0.1.4/src/idinn/controller.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 idinn-0.1.4/src/idinn/demand.py
--rw-r--r--   0        0        0    10273 2020-02-02 00:00:00.000000 idinn-0.1.4/src/idinn/sourcing_model.py
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 idinn-0.1.4/tests/test_controller.py
--rw-r--r--   0        0        0     7757 2020-02-02 00:00:00.000000 idinn-0.1.4/tests/test_sourcing_model.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 idinn-0.1.4/.gitignore
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 idinn-0.1.4/LICENSE
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 idinn-0.1.4/README.md
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 idinn-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 idinn-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 idinn-0.1.5/.readthedocs.yaml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 idinn-0.1.5/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/Makefile
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/conf.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/make.bat
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/requirements.txt
+-rw-r--r--   0        0        0    45770 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/_static/dual_sourcing_output.png
+-rw-r--r--   0        0        0   453134 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/_static/optimization_schematic.png
+-rw-r--r--   0        0        0    31481 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/_static/single_sourcing_output.png
+-rw-r--r--   0        0        0   243113 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/_static/youtube.png
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/get_started/get_started.rst
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/get_started/installation.rst
+-rw-r--r--   0        0        0     8461 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/joss/paper.bib
+-rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/joss/paper.md
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/tutorials/api.rst
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/tutorials/benchmark.rst
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/tutorials/dual.rst
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/tutorials/single.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/tutorials/transfer.rst
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/understand/dynamics.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/understand/optimization.rst
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/understand/order.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 idinn-0.1.5/docs/understand/straight.rst
+-rw-r--r--   0        0        0   106539 2020-02-02 00:00:00.000000 idinn-0.1.5/notebooks/demo.ipynb
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 idinn-0.1.5/src/idinn/__init__.py
+-rw-r--r--   0        0        0    26037 2020-02-02 00:00:00.000000 idinn-0.1.5/src/idinn/controller.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 idinn-0.1.5/src/idinn/demand.py
+-rw-r--r--   0        0        0    10273 2020-02-02 00:00:00.000000 idinn-0.1.5/src/idinn/sourcing_model.py
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 idinn-0.1.5/tests/test_controller.py
+-rw-r--r--   0        0        0     7757 2020-02-02 00:00:00.000000 idinn-0.1.5/tests/test_sourcing_model.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 idinn-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 idinn-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 idinn-0.1.5/README.md
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 idinn-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 idinn-0.1.5/PKG-INFO
```

### Comparing `idinn-0.1.4/.readthedocs.yaml` & `idinn-0.1.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `idinn-0.1.4/docs/Makefile` & `idinn-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idinn-0.1.4/docs/conf.py` & `idinn-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idinn-0.1.4/docs/index.rst` & `idinn-0.1.5/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,37 +11,35 @@
 =============
 
 .. code-block:: python
 
    import torch
    from idinn.sourcing_model import SingleSourcingModel
    from idinn.controller import SingleSourcingNeuralController
+   from idinn.demand import UniformDemand
 
    # Initialize the sourcing model and the neural controller
    sourcing_model = SingleSourcingModel(
       lead_time=0,
       holding_cost=5,
       shortage_cost=495,
       batch_size=32,
       init_inventory=10,
-      demand_distribuion="uniform",
-      demand_low=1,
-      demand_high=4
+      demand_generator=UniformDemand(low=1, high=4),
    )
-   controller = SingleFullyConnectedNeuralController(
+   controller = SingleSourcingNeuralController(
       hidden_layers=[2],
       activation=torch.nn.CELU(alpha=1)
    )
    # Train the neural controller
-   controller.train(
+   controller.fit(
       sourcing_model=sourcing_model,
       sourcing_periods=50,
       validation_sourcing_periods=1000,
       epochs=5000,
-      tensorboard_writer=torch.utils.tensorboard.SummaryWriter(),
       seed=1,
    )
    # Simulate and plot the results
    controller.plot(sourcing_model=sourcing_model, sourcing_periods=100)
    # Calculate the optimal order quantity for applications
    controller.forward(current_inventory=10, past_orders=[1, 5])
```

### Comparing `idinn-0.1.4/docs/make.bat` & `idinn-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `idinn-0.1.4/docs/_static/optimization_schematic.png` & `idinn-0.1.5/docs/_static/optimization_schematic.png`

 * *Files identical despite different names*

### Comparing `idinn-0.1.4/docs/_static/youtube.png` & `idinn-0.1.5/docs/_static/youtube.png`

 * *Files identical despite different names*

### Comparing `idinn-0.1.4/docs/get_started/get_started.rst` & `idinn-0.1.5/docs/get_started/get_started.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Get Started
 ===========
 
 Initialization
 --------------
 
-The basic usage of `idinn` starts with a sourcing model and a controller. First, initialize a sourcing model, such as :class:`SingleSourcingModel`, with desired parameters according to users' needs.
+The basic usage of `idinn` starts with a sourcing model and a controller. First, initialize a sourcing model, such as :class:`SingleSourcingModel`, with your preferred parameters.
 
 .. code-block:: python
     
    import torch
    from idinn.sourcing_model import SingleSourcingModel
 
    # Initialize the sourcing model
@@ -35,15 +35,15 @@
 --------
 
 The selected controller needs to be trained to find the optimal neural-network parameters.
 
 .. code-block:: python
 
    # Train the neural controller
-   controller.train(
+   controller.fit(
       sourcing_model=sourcing_model,
       sourcing_periods=50,
       epochs=5000
    )
 
 Simulation, Plotting and Order Calculation
 ------------------------------------------
```

### Comparing `idinn-0.1.4/docs/get_started/installation.rst` & `idinn-0.1.5/docs/get_started/installation.rst`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ************
 
 Requirements
 ============
 
 The basic usage of `idinn` requires a working `Python`_ and `PyTorch`_ installation. If plotting simulation result of a controller is needed, `matplotlib`_ should also be installed. We recommend using the following versions for maximum compability:
 
-* Python_     ``>= 3.8``
+* Python_     ``>= 3.7``
 * PyTorch_    ``>= 2.0``
 * matplotlib_ ``>= 3.0``
 
 Install `idinn`
 ===============
 
 The package can be installed form PyPI. To do that, run
```

### Comparing `idinn-0.1.4/docs/tutorials/dual.rst` & `idinn-0.1.5/docs/tutorials/dual.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,111 +1,118 @@
 Solve Dual-Sourcing Problems Using Neural Networks
 ==================================================
 
-Dual-sourcing problems are similar to single-sourcing problems but are more intricate. In a dual-sourcing problem, a company has two potential suppliers for a product, each offering varying lead times (the duration for orders to arrive) and order costs (the expense of placing an order). The challenge lies in the company's decision-making process: determining which supplier to engage for each product to minimize costs given stochastic demand. We can solve dual-sourcing problems with `idinn` in a way similar to the approaches describes described in :doc:`/get_started/get_started` and :doc:`/tutorials/single`.
+Dual-sourcing problems are similar to single-sourcing problems but are more intricate. In a dual-sourcing problem, a company has two potential suppliers for a product, each offering varying lead times (the duration for orders to arrive) and order costs (the expense of placing an order). The challenge lies in the company's decision-making process: determining which supplier to engage for each product to minimize costs given stochastic demand. We can solve dual-sourcing problems with `idinn` in a way similar to the approaches described in :doc:`/get_started/get_started` and :doc:`/tutorials/dual`.
 
 Initialization
 --------------
 
-To address dual-sourcing problems, we employ two main classes: (i) `DualSourcingModel` and (ii) `DualSourcingNeuralController`, responsible for setting up the sourcing model and its corresponding controller. In this tutorial, we examine a dual-sourcing model characterized by the following parameters: the regular order lead time is 2; the expedited order lead time is 0; the regular order cost, :math:`c^r`, is 0; the expedited order cost, :math:`c^e`, is 20; and the initial inventory is 6. Additionally, the holding cost, :math:`h`, and the shortage cost, :math:`b`, are 5 and 495, respectively. Demand is generated from a discrete uniform distribution with interval :math:`[1, 4]`. Notice that both the `demand_low` and `demand_low` parameters are inclusive. In this example, we use a batch size of 256. 
-
-In `idinn`, the sourcing model is initialized as follows.
+To address dual-sourcing problems, we employ two main classes: (i) `DualSourcingModel` and (ii) `DualSourcingNeuralController`, responsible for setting up the sourcing model and its corresponding controller. In this tutorial, we examine a dual-sourcing model characterized by the following parameters: the regular order lead time is 2; the expedited order lead time is 0; the regular order cost, :math:`c^r`, is 0; the expedited order cost, :math:`c^e`, is 20; and the initial inventory is 6. Additionally, the holding cost, :math:`h`, and the shortage cost, :math:`b`, are 5 and 495, respectively. Demand is generated from a discrete uniform distribution with support :math:`[1, 4]`. In this example, we use a batch size of 256. 
 
 .. code-block:: python
     
    import torch
    from idinn.sourcing_model import DualSourcingModel
    from idinn.controller import DualSourcingNeuralController
+   from idinn.demand import UniformDemand
 
-    dual_sourcing_model = DualSourcingModel(
-        regular_lead_time=2,
-        expedited_lead_time=0,
-        regular_order_cost=0,
-        expedited_order_cost=20,
-        holding_cost=5,
-        shortage_cost=495,
-        batch_size=256,
-        init_inventory=6,
-        demand_distribution="uniform",
-        demand_low=1,
-        demand_high=4
-    )
+   dual_sourcing_model = DualSourcingModel(
+       regular_lead_time=2,
+       expedited_lead_time=0,
+       regular_order_cost=0,
+       expedited_order_cost=20,
+       holding_cost=5,
+       shortage_cost=495,
+       batch_size=256,
+       init_inventory=6,
+       demand_generator=UniformDemand(low=1, high=4),
+   )
 
 The cost at period :math:`t`, :math:`c_t`, is
 
 .. math::
 
    c_t = c^r q^r_t + c^e q^e_t + h \max(0, I_t) + b \max(0, - I_t)\,,
 
-where :math:`I_t` is the inventory level at the end of period :math:`t`, :math:`q^r_t` is the regular order placed at period :math:`t`, and :math:`q^e_t` is the expedited order placed at period :math:`t`. The higher the holding cost, the more costly it is to keep the inventory (when the inventory level is positive). The higher the shortage cost, the more costly it is to run out of stock (when the inventory level is negative). The higher the regular or expedited order costs, the more costly it is to place the respective orders. The cost can be calculated using the `get_total_cost` method of the sourcing model.
+where :math:`I_t` is the inventory level at the end of period :math:`t`, :math:`q^r_t` is the regular order placed at period :math:`t`, and :math:`q^e_t` is the expedited order placed at period :math:`t`. The higher the holding cost, the more costly it is to keep the inventory positive and high. The higher the shortage cost, the more costly it is to run out of stock when the inventory level is negative. The higher the regular and expedited order costs, the more costly it is to place the respective orders. The joint holding and stockout cost across all periods can be can be calculated using the `get_total_cost()` method of the sourcing model.
 
 .. code-block:: python
     
    dual_sourcing_model.get_total_cost(regular_q=0, expedited_q=0)
 
-In our example, this function should return 30 for each sample since the initial inventory is 6, the holding cost is 5, and there is neither a regular nor expedited order. We have 256 samples in this case, as we specified a batch size of 256.
+In this example, this function should return 30 for each sample since the initial inventory is 6, the holding cost is 5, and there is neither a regular nor expedited order. We have 256 samples in this case, as we specified a batch size of 256.
 
-For dual-sourcing problems, we initialize the neural network controller using the `DualSourcingNeuralController` class. In this tutorial, we use a simple neural network with 6 hidden layers. The numbers of neurons in each layer are 128, 64, 32, 16, 8, and 4, respectively. The activation function is `torch.nn.CELU(alpha=1)`. The neural network controller is initialized as follows.
+For dual-sourcing problems, we initialize the neural network controller using the `DualSourcingNeuralController` class. In this tutorial, we employ a simple neural network with 6 hidden layers. The numbers of neurons in each layer are 128, 64, 32, 16, 8, and 4, respectively. The activation function is `torch.nn.CELU(alpha=1)`.
 
 .. code-block:: python
 
     dual_controller = DualSourcingNeuralController(
-        hidden_layers=[128, 64, 32, 16, 8, 4], activation=torch.nn.CELU(alpha=1)
+        hidden_layers=[128, 64, 32, 16, 8, 4],
+        activation=torch.nn.CELU(alpha=1)
     )
 
 Training
 --------
 
 Although the neural network controller has not been trained yet, we can still compute the total cost associated with its order policy. To do so, we integrate it with our previously specified sourcing model and run simulations for 100 periods.
 
 .. code-block:: python
 
     dual_controller.get_total_cost(sourcing_model=dual_sourcing_model, sourcing_periods=100)
 
-Unsurprisingly, the performance is poor because we are only using the untrained neural network in which the weights are just (pseudo) random numbers. We can train the neural network controller using the `train` method, in which the training data is generated from the given sourcing model. To better monitor the training process, we specify the `tensorboard_writer` parameter to log both the training loss and validation loss. For reproducibility, we also specify the seed of the underlying random number generator using the  `seed` parameter.
+Unsurprisingly, the performance is poor because we are only using the untrained neural network in which the weights are just (pseudo) random numbers. We can train the neural network controller using the `train()` method, in which the training data is generated from the given sourcing model. To better monitor the training process, we specify the `tensorboard_writer` parameter to log both the training loss and validation loss. For reproducibility, we also specify the seed of the underlying random number generator using the  `seed` parameter.
 
 .. code-block:: python
 
     from torch.utils.tensorboard import SummaryWriter
 
-    dual_controller.train(
+    dual_controller.fit(
         sourcing_model=dual_sourcing_model,
         sourcing_periods=100,
         validation_sourcing_periods=1000,
         epochs=2000,
-        tensorboard_writer=SummaryWriter("runs/dual_sourcing_model"),
+        tensorboard_writer=SummaryWriter(comment="dual"),
         seed=4,
     )
 
 After training, we can use the trained neural network controller to calculate the total cost for 100 periods with our previously specified sourcing model. The total cost should be significantly lower than the cost associated with the untrained model.
 
 .. code-block:: python
     
     dual_controller.get_total_cost(sourcing_model=dual_sourcing_model, sourcing_periods=100)
 
-Simulation, Plotting, and Order Calculation
+Plotting and Order Calculation
 ------------------------------------------
 
-We can also inspect how the controller performs in the specified sourcing environment by (i) plotting the inventory and order histories, and (ii) calculating optimal orders.
+We can inspect how the controller performs in the specified sourcing environment by plotting the inventory and order histories.
 
 .. code-block:: python
 
     # Simulate and plot the results
     dual_controller.plot(sourcing_model=dual_sourcing_model, sourcing_periods=100)
+
+.. image:: ../_static/dual_sourcing_output.png
+   :alt: Output of the dual sourcing model and controller
+   :align: center
+
+Then we can use the trained network to calculate near-optimal orders.
+
+.. code-block:: python
+
     # Calculate the optimal order quantity for applications
     regular_q, expedited_q = dual_controller.forward(
         current_inventory=10,
         past_regular_orders=[1, 5],
         past_expedited_orders=[0, 0],
     )
 
 Save and Load the Model
 -----------------------
 
-It is also a good idea to save the trained neural network controller for future use. This can be done using the `save` method. The `load` method allows one to load a previously saved model.
+It is also a good idea to save the trained neural network controller for future use. This can be done using the `save()` method. The `load()` method allows one to load a previously saved model.
 
 .. code-block:: python
 
     # Save the model
     dual_controller.save("optimal_dual_sourcing_controller.pt")
     # Load the model
     dual_controller_loaded = DualSourcingNeuralController()
```

### Comparing `idinn-0.1.4/docs/tutorials/single.rst` & `idinn-0.1.5/docs/tutorials/single.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,97 +1,108 @@
 Solve Single-Sourcing Problems Using Neural Networks
 ====================================================
 
-Single-sourcing problems are inventory management problems where only one delivery option exists. The overall objective in single-sourcing and related inventory management problems is for companies to identify the optimal order quantities to minimize costs given stochastic demand. This problem can be addressed using `idinn`. As illustrated in the :doc:`/get_started/get_started` section, we first initialize the sourcing model and its associated neural network controller. Subsequently, we train the neural network controller using data generated from the sourcing model. Finally, we can use the trained neural network controller to compute optimal order quantities.
+The overall objective in single-sourcing and related inventory management problems is for companies to identify the optimal order quantities to minimize inventory-related costs, given stochastic demand. During periods when inventory remains after demand is met, each unit of excess inventory incurs a holding cost :math:`h`. If the demand exceeds the available inventory in a period, the surplus demand is considered satisfied in subsequent periods, incurring a shortage cost :math:`b`. This problem can be addressed using `idinn`. As illustrated in the :doc:`/get_started/get_started` section, we first initialize the sourcing model and its associated neural network controller. Subsequently, we train the neural network controller using data generated from the sourcing model. Finally, we use the trained neural network controller to compute optimal order quantities, which depend on the state of the system.
 
 Initialization
 --------------
 
-Since we deal with the single-sourcing problem, we use the `SingleSourcingModel` class to initialize the sourcing model. In this tutorial, let us pick a single sourcing model which has a lead time of 0 (i.e., the order arrives immediately after it is placed) and an initial inventory of 10. The holding cost, :math:`h`, and the shortage cost, :math:`b`, are 5 and 495, respectively. The demand is generated from a discrete uniform distribution with support :math:`[1, 4]`. Notice that both the `demand_low` and `demand_low` parameters are inclusive. In this example, we use a batch size of 32.
-
-In `idinn`, the sourcing model is initialized as follows.
+We use the `SingleSourcingModel` class to initialize a single-sourcing model. The single-sourcing model considered in this example has a lead time of 0, i.e., the order arrives immediately after it is placed, and initial inventory of 10. The holding cost, :math:`h`, and the shortage cost, :math:`b`, are 5 and 495, respectively. The demand is generated from a discrete uniform distribution with support :math:`[1, 4]`. We use a batch size of 32 for training the neural network, i.e. the sourcing model generate 32 samples simultaneously.
 
 .. code-block:: python
     
    import torch
    from idinn.sourcing_model import SingleSourcingModel
    from idinn.controller import SingleSourcingNeuralController
+   from idinn.demand import UniformDemand
 
    single_sourcing_model = SingleSourcingModel(
-      lead_time=0,
-      holding_cost=5,
-      shortage_cost=495,
-      batch_size=32,
-      init_inventory=10,
-      demand_distribution="uniform",
-      demand_low=1,
-      demand_high=4
-   )
+       lead_time=0,
+       holding_cost=5,
+       shortage_cost=495,
+       batch_size=32,
+       init_inventory=10,
+       demand_generator=UniformDemand(low=1, high=4),
+    )
 
 The cost at period :math:`t`, :math:`c_t`, is
 
 .. math::
 
    c_t = h \max(0, I_t) + b \max(0, - I_t)\,,
 
-where :math:`I_t` is the inventory level at the end of period :math:`t`. The higher the holding cost, the more costly it is to keep the inventory (when the inventory level is positive). The higher the shortage cost, the more costly it is to run out of stock (when the inventory level is negative). The cost can be calculated using the `get_total_cost` method of the sourcing model.
+where :math:`I_t` is the inventory level at the end of period :math:`t`. The higher the holding cost, the more costly it is to keep the inventory postive and high. The higher the shortage cost, the more costly it is to run out of stock when the inventory level is negative. The joint holding and stockout cost across all periods can be can be calculated using the `get_total_cost()` method of the sourcing model.
 
 .. code-block:: python
     
    single_sourcing_model.get_total_cost()
 
-In our example, this function should return 50 for each sample since the initial inventory is 10 and the holding cost is 5. We have 32 samples in this case, as we specified a batch size of 32.
+In this example, this function should return 50 for each sample since the initial inventory is 10 and the holding cost is 5. We have 32 samples in this case, as we specified the batch size to be 32.
 
-For single-sourcing problems, we initialize the neural network controller using the `SingleSourcingNeuralController` class. In this tutorial, we use a simple neural network with 1 hidden layer and 2 neurons. The activation function is `torch.nn.CELU(alpha=1)`. The neural network controller is initialized as follows.
+For single-sourcing problems, we use the neural network controller of the `SingleSourcingNeuralController` class. For illustration purposes, we employ a simple neural network with 1 hidden layer and 2 neurons. The activation function is `torch.nn.CELU(alpha=1)`.
 
 .. code-block:: python
 
     single_controller = SingleSourcingNeuralController(
         hidden_layers=[2], activation=torch.nn.CELU(alpha=1)
     )
 
 Training
 --------
 
 Although the neural network controller has not been trained yet, we can still compute the total cost associated with its order policy. To do so, we integrate it with our previously specified sourcing model and run simulations for 100 periods.
 
 .. code-block:: python
     
-    single_controller.get_total_cost(sourcing_model=single_sourcing_model, sourcing_periods=100)
+    single_controller.get_total_cost(
+        sourcing_model=single_sourcing_model,
+        sourcing_periods=100
+        )
 
-Unsurprisingly, the performance is poor because we are only using the untrained neural network in which the weights are just (pseudo) random numbers. We can train the neural network controller using the `train` method, in which the training data is generated from the given sourcing model. To better monitor the training process, we specify the `tensorboard_writer` parameter to log both the training loss and validation loss. For reproducibility, we also specify the seed of the underlying random number generator using the `seed` parameter.
+Unsurprisingly, the performance is poor because we are only using the untrained neural network in which the weights are just (pseudo) random numbers. We can train the neural network controller using the `train()` method, in which the training data is generated from the given sourcing model. To better monitor the training process, we specify the `tensorboard_writer` parameter to log both the training loss and validation loss. For reproducibility, we also specify the seed of the underlying random number generator using the `seed` parameter.
 
 .. code-block:: python
 
     from torch.utils.tensorboard import SummaryWriter
 
-    single_controller.train(
+    single_controller.fit(
         sourcing_model=single_sourcing_model,
         sourcing_periods=50,
         validation_sourcing_periods=1000,
         epochs=5000,
         seed=1,
-        tensorboard_writer=SummaryWriter()
+        tensorboard_writer=SummaryWriter(comment="single")
     )
 
 After training, we can use the trained neural network controller to calculate the total cost for 100 periods with our previously specified sourcing model. The total cost should be significantly lower than the cost associated with the untrained model.
 
 .. code-block:: python
 
-    single_controller.get_total_cost(sourcing_model=single_sourcing_model, sourcing_periods=100)
+    single_controller.get_total_cost(
+        sourcing_model=single_sourcing_model,
+        sourcing_periods=100
+        )
 
-Simulation, Plotting, and Order Calculation
+Plotting and Order Calculation
 ------------------------------------------
 
-We can also inspect how the controller performs in the specified sourcing environment by (i) plotting the inventory and order histories, and (ii) calculating optimal orders.
+We can inspect how the controller performs in the specified sourcing environment by plotting the inventory and order histories.
 
 .. code-block:: python
 
     # Simulate and plot the results
     single_controller.plot(sourcing_model=single_sourcing_model, sourcing_periods=100)
+
+.. image:: ../_static/single_sourcing_output.png
+   :alt: Output of the single sourcing model and controller
+   :align: center
+
+Then we can calculate optimal orders using the trained model.
+
+.. code-block:: python
     # Calculate the optimal order quantity for applications
     single_controller.forward(current_inventory=10, past_orders=[1, 5])
 
 Save and Load the Model
 -----------------------
 
 It is also a good idea to save the trained neural network controller for future use. This can be done using the `save` method. The `load` method allows one to load a previously saved controller.
```

### Comparing `idinn-0.1.4/src/idinn/controller.py` & `idinn-0.1.5/src/idinn/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 
 
-class NeuralControllerMixIn():
+class NeuralControllerMixIn:
     def save(self, checkpoint_path):
         torch.save(self.state_dict(), checkpoint_path)
 
     def load(self, checkpoint_path):
         self.load_state_dict(torch.load(checkpoint_path))
 
 
@@ -24,15 +24,15 @@
 
     Attributes
     ----------
     hidden_layers : list
         List of integers representing the number of units in each hidden layer.
     activation : torch.nn.Module
         Activation function used in the hidden layers.
-    stack : torch.nn.Sequential
+    architecture : torch.nn.Sequential
         Sequential stack of linear layers and activation functions.
 
     Methods
     -------
     init_layers(lead_time)
         Initialize the layers of the neural network based on the lead time.
     forward(current_inventory, past_orders)
@@ -48,15 +48,15 @@
     """
 
     def __init__(self, hidden_layers=[2], activation=torch.nn.CELU(alpha=1)):
         super().__init__()
         self.hidden_layers = hidden_layers
         self.activation = activation
         self.lead_time = None
-        self.stack = None
+        self.architecture = None
 
     def init_layers(self, lead_time):
         """
         Initialize the layers of the neural network based on the lead time.
 
         Parameters
         ----------
@@ -78,15 +78,15 @@
                     torch.nn.Linear(self.hidden_layers[i], self.hidden_layers[i + 1]),
                     self.activation,
                 ]
         architecture += [
             torch.nn.Linear(self.hidden_layers[-1], 1, bias=False),
             torch.nn.ReLU(),
         ]
-        self.stack = torch.nn.Sequential(*architecture)
+        self.architecture = torch.nn.Sequential(*architecture)
 
     def forward(
         self,
         current_inventory,
         past_orders,
     ):
         """
@@ -105,16 +105,20 @@
             Order quanty calculated by the neural network.
         """
         if not isinstance(current_inventory, torch.Tensor):
             current_inventory = torch.tensor([[current_inventory]], dtype=torch.float32)
         if not isinstance(past_orders, torch.Tensor):
             past_orders = torch.tensor([past_orders], dtype=torch.float32)
         if self.lead_time > 0:
-            h = torch.cat([current_inventory, past_orders[:, -self.lead_time :]], dim=1)
-        h = self.stack(h)
+            inputs = torch.cat(
+                [current_inventory, past_orders[:, -self.lead_time :]], dim=1
+            )
+        else:
+            inputs = current_inventory
+        h = self.architecture(inputs)
         q = h - torch.frac(h).clone().detach()
         return q
 
     def get_total_cost(self, sourcing_model, sourcing_periods, seed=None):
         """
         Calculate the total cost over a given number of sourcing periods.
 
@@ -131,79 +135,88 @@
         -------
         numpy.ndarray
             Total cost over the sourcing periods.
         """
         if seed is not None:
             torch.manual_seed(seed)
 
-        if self.lead_time is None:
+        if self.architecture is None:
             self.init_layers(sourcing_model.get_lead_time())
 
         total_cost = 0
         for i in range(sourcing_periods):
             current_inventory = sourcing_model.get_current_inventory()
             past_orders = sourcing_model.get_past_orders()
             q = self.forward(current_inventory, past_orders)
             sourcing_model.order(q)
             current_cost = sourcing_model.get_cost()
             total_cost += current_cost.mean()
         return total_cost
 
-    def train(
+    def fit(
         self,
         sourcing_model,
         sourcing_periods,
         epochs,
         validation_sourcing_periods=None,
-        lr_init_inventory=1e-1,
-        lr_parameters=3e-3,
-        seed=None,
+        validation_freq=10,
+        init_inventory_lr=1e-1,
+        init_inventory_freq=4,
+        parameters_lr=3e-3,
         tensorboard_writer=None,
+        seed=None,
     ):
         """
         Train the neural network controller using the sourcing model and specified parameters.
 
         Parameters
         ----------
         sourcing_model : SourcingModel
-            The sourcing model to be used for training.
+            The sourcing model for training.
         sourcing_periods : int
             The number of sourcing periods for training.
         epochs : int
             The number of training epochs.
         validation_sourcing_periods : int, optional
             The number of sourcing periods for validation.
-        lr_init_inventory : float, default is 1e-1
+        validation_freq : int, default is 10
+            Only relevant if `validation_sourcing_periods` is provided. Specifies how many training epochs to run before a new validation run is performed, e.g. `validation_freq=10` runs validation every 10 epochs.
+        init_inventory_freq : int, default is 4
+            Specifies how many parameter updating epochs to run before initial inventory is updated. e.g. `init_inventory_freq=4` updates initial inventory after updating parameters for 4 epochs.
+        init_inventory_lr : float, default is 1e-1
             Learning rate for initial inventory.
-        lr_parameters : float, default is 3e-3
-            Learning rate for updating neural network parameters. 
-        seed : int, optional
-            Random seed for reproducibility.
+        parameters_lr : float, default is 3e-3
+            Learning rate for updating neural network parameters.
         tensorboard_writer : tensorboard.SummaryWriter, optional
             Tensorboard writer for logging.
+        seed : int, optional
+            Random seed for reproducibility.
         """
         if seed is not None:
             torch.manual_seed(seed)
 
+        if self.architecture is None:
+            self.init_layers(sourcing_model.get_lead_time())
+
         optimizer_init_inventory = torch.optim.RMSprop(
-            [sourcing_model.init_inventory], lr=lr_init_inventory
+            [sourcing_model.init_inventory], lr=init_inventory_lr
         )
-        optimizer_parameters = torch.optim.RMSprop(self.parameters(), lr=lr_parameters)
+        optimizer_parameters = torch.optim.RMSprop(self.parameters(), lr=parameters_lr)
         min_cost = np.inf
 
         for epoch in range(epochs):
             # Clear grad cache
             optimizer_parameters.zero_grad()
             optimizer_init_inventory.zero_grad()
             # Reset the sourcing model with the learned init inventory
             sourcing_model.reset()
             total_cost = self.get_total_cost(sourcing_model, sourcing_periods)
             total_cost.backward()
             # Gradient descend
-            if epoch % 3 == 0:
+            if epoch % init_inventory_freq == 0:
                 optimizer_init_inventory.step()
             else:
                 optimizer_parameters.step()
             # Save the best model
             if validation_sourcing_periods is not None and epoch % 10 == 0:
                 eval_cost = self.get_total_cost(
                     sourcing_model, validation_sourcing_periods
@@ -216,21 +229,24 @@
                     min_cost = total_cost
                     best_state = self.state_dict()
             # Log train loss
             if tensorboard_writer is not None:
                 tensorboard_writer.add_scalar(
                     "Avg. cost per period/train", total_cost / sourcing_periods, epoch
                 )
-                # Log evaluation loss
-                if validation_sourcing_periods is not None and epoch % 10 == 0:
+                if (
+                    validation_sourcing_periods is not None
+                    and epoch % validation_freq == 0
+                ):
+                    # Log validation loss
                     eval_cost = self.get_total_cost(
                         sourcing_model, validation_sourcing_periods
                     )
                     tensorboard_writer.add_scalar(
-                        "Avg. cost per period/eval",
+                        "Avg. cost per period/val",
                         eval_cost / validation_sourcing_periods,
                         epoch,
                     )
                 tensorboard_writer.flush()
         # Load the best model
         self.load_state_dict(best_state)
 
@@ -260,37 +276,39 @@
             past_orders = sourcing_model.get_past_orders()
             q = self.forward(current_inventory, past_orders)
             sourcing_model.order(q)
         past_inventories = sourcing_model.get_past_inventories()[0, :].detach().numpy()
         past_orders = sourcing_model.get_past_orders()[0, :].detach().numpy()
         return past_inventories, past_orders
 
-    def plot(self, sourcing_model, sourcing_periods):
+    def plot(self, sourcing_model, sourcing_periods, linewidth=1):
         """
         Plot the inventory and order quantities over a given number of sourcing periods.
 
         Parameters
         ----------
         sourcing_model : SingleSourcingModel
             The sourcing model to be used for plotting.
         sourcing_periods : int
             The number of sourcing periods for plotting.
+        linewidth : int, default is 1
+            The width of the line in the step plots.
         """
         past_inventories, past_orders = self.simulate(
             sourcing_model=sourcing_model, sourcing_periods=sourcing_periods
         )
         fig, ax = plt.subplots(ncols=2, figsize=(10, 4))
 
-        ax[0].step(range(sourcing_periods), past_inventories[-sourcing_periods:])
+        ax[0].step(range(sourcing_periods), past_inventories[-sourcing_periods:], linewidth=linewidth, color='tab:blue')
         ax[0].yaxis.get_major_locator().set_params(integer=True)
         ax[0].set_title("Inventory")
         ax[0].set_xlabel("Period")
         ax[0].set_ylabel("Quantity")
 
-        ax[1].step(range(sourcing_periods), past_orders[-sourcing_periods:])
+        ax[1].step(range(sourcing_periods), past_orders[-sourcing_periods:], linewidth=linewidth, color='tab:orange')
         ax[1].yaxis.get_major_locator().set_params(integer=True)
         ax[1].set_title("Order")
         ax[1].set_xlabel("Period")
         ax[1].set_ylabel("Quantity")
 
 
 class DualSourcingNeuralController(torch.nn.Module, NeuralControllerMixIn):
@@ -314,15 +332,15 @@
         Activation function to be used in the hidden layers.
     compressed : bool
         Flag indicating whether the input is compressed.
     regular_lead_time : int
         Regular lead time.
     expedited_lead_time : int
         Expedited lead time.
-    stack : torch.nn.Sequential
+    architecture : torch.nn.Sequential
         Sequential stack of linear layers and activation functions.
 
     Methods
     -------
     init_layers(regular_lead_time, expedited_lead_time)
         Initialize the layers of the neural network.
     forward(current_inventory, past_orders)
@@ -336,23 +354,23 @@
     plot(sourcing_model, sourcing_periods)
         Plot the inventory and order quantities.
     """
 
     def __init__(
         self,
         hidden_layers=[128, 64, 32, 16, 8, 4],
-        activation=torch.nn.CELU(alpha=1),
+        activation=torch.nn.ReLU(),
         compressed=False,
     ):
         super().__init__()
         self.hidden_layers = hidden_layers
         self.activation = activation
         self.compressed = compressed
         self.lead_time = None
-        self.stack = None
+        self.architecture = None
 
     def init_layers(self, regular_lead_time, expedited_lead_time):
         """
         Initialize the layers of the neural network.
 
         Parameters
         ----------
@@ -378,15 +396,15 @@
                     torch.nn.Linear(self.hidden_layers[i], self.hidden_layers[i + 1]),
                     self.activation,
                 ]
         architecture += [
             torch.nn.Linear(self.hidden_layers[-1], 2),
             torch.nn.ReLU(),
         ]
-        self.stack = torch.nn.Sequential(*architecture)
+        self.architecture = torch.nn.Sequential(*architecture)
 
     def forward(self, current_inventory, past_regular_orders, past_expedited_orders):
         """
         Forward pass of the neural network.
 
         Parameters
         ----------
@@ -403,37 +421,43 @@
             Regular order quantity.
         expedited_q : torch.Tensor
             Expedited order quantity.
         """
         if not isinstance(current_inventory, torch.Tensor):
             current_inventory = torch.tensor([[current_inventory]], dtype=torch.float32)
         if not isinstance(past_regular_orders, torch.Tensor):
-            past_regular_orders = torch.tensor([past_regular_orders], dtype=torch.float32)
+            past_regular_orders = torch.tensor(
+                [past_regular_orders], dtype=torch.float32
+            )
         if not isinstance(past_expedited_orders, torch.Tensor):
-            past_expedited_orders = torch.tensor([past_expedited_orders], dtype=torch.float32)
+            past_expedited_orders = torch.tensor(
+                [past_expedited_orders], dtype=torch.float32
+            )
 
         if self.regular_lead_time > 0:
             if self.compressed:
                 inputs = past_regular_orders[:, -self.regular_lead_time :]
                 inputs[:, 0] += current_inventory
             else:
                 inputs = torch.cat(
                     [
                         current_inventory,
                         past_regular_orders[:, -self.regular_lead_time :],
                     ],
                     dim=1,
                 )
+        else:
+            inputs = current_inventory
 
         if self.expedited_lead_time > 0:
             inputs = torch.cat(
                 [inputs, past_expedited_orders[:, -self.expedited_lead_time :]], dim=1
             )
 
-        h = self.stack(inputs)
+        h = self.architecture(inputs)
         q = h - torch.frac(h).clone().detach()
         regular_q = q[:, [0]]
         expedited_q = q[:, [1]]
         return regular_q, expedited_q
 
     def get_total_cost(self, sourcing_model, sourcing_periods, seed=None):
         """
@@ -452,90 +476,102 @@
         -------
         total_cost : torch.Tensor
             Total cost.
         """
         if seed is not None:
             torch.manual_seed(seed)
 
-        if self.lead_time is None:
+        if self.architecture is None:
             self.init_layers(
                 regular_lead_time=sourcing_model.get_regular_lead_time(),
                 expedited_lead_time=sourcing_model.get_expedited_lead_time(),
             )
-        
+
         total_cost = 0
         for i in range(sourcing_periods):
             current_inventory = sourcing_model.get_current_inventory()
             past_regular_orders = sourcing_model.get_past_regular_orders()
             past_expedited_orders = sourcing_model.get_past_expedited_orders()
             regular_q, expedited_q = self.forward(
                 current_inventory, past_regular_orders, past_expedited_orders
             )
             sourcing_model.order(regular_q, expedited_q)
             current_cost = sourcing_model.get_cost(regular_q, expedited_q)
             total_cost += current_cost.mean()
         return total_cost
 
-    def train(
+    def fit(
         self,
         sourcing_model,
         sourcing_periods,
         epochs,
         validation_sourcing_periods=None,
-        lr_init_inventory=1e-1,
-        lr_parameters=3e-3,
-        seed=None,
+        validation_freq=50,
+        init_inventory_freq=4,
+        init_inventory_lr=1e-1,
+        parameters_lr=3e-3,
         tensorboard_writer=None,
+        seed=None,
     ):
         """
-        Train the neural network.
+        Train the neural network controller using the sourcing model and specified parameters.
 
         Parameters
         ----------
         sourcing_model : DualSourcingModel
-            The sourcing model.
+            The sourcing model for training.
         sourcing_periods : int
-            Number of sourcing periods.
+            Number of sourcing periods for training.
         epochs : int
             Number of training epochs.
         validation_sourcing_periods : int, optional
             Number of sourcing periods for validation.
-        lr_init_inventory : float, default is 1e-1
+        validation_freq : int, default is 10
+            Only relevant if `validation_sourcing_periods` is provided. Specifies how many training epochs to run before a new validation run is performed, e.g. `validation_freq=10` runs validation every 10 epochs.
+        init_inventory_freq : int, default is 4
+            Specifies how many parameter updating epochs to run before initial inventory is updated. e.g. `init_inventory_freq=4` updates initial inventory after updating parameters for 4 epochs.
+        init_inventory_lr : float, default is 1e-1
             Learning rate for initial inventory.
-        lr_parameters : float, default is 3e-3
+        parameters_lr : float, default is 3e-3
             Learning rate for updating neural network parameters.
+        tensorboard_writer : tensorboard.SummaryWriter, optional
         seed : int, optional
             Random seed for reproducibility.
-        tensorboard_writer : TensorBoard writer, optional
-            TensorBoard writer for logging.
+            Tensorboard writer for logging.
         """
         if seed is not None:
             torch.manual_seed(seed)
 
+        if self.architecture is None:
+            self.init_layers(
+                regular_lead_time=sourcing_model.get_regular_lead_time(),
+                expedited_lead_time=sourcing_model.get_expedited_lead_time(),
+            )
+
         optimizer_init_inventory = torch.optim.RMSprop(
-            [sourcing_model.init_inventory], lr=lr_init_inventory
+            [sourcing_model.init_inventory], lr=init_inventory_lr
         )
-        optimizer_parameters = torch.optim.RMSprop(self.parameters(), lr=lr_parameters)
+        optimizer_parameters = torch.optim.RMSprop(self.parameters(), lr=parameters_lr)
         min_cost = np.inf
 
         for epoch in range(epochs):
             # Clear grad cache
             optimizer_init_inventory.zero_grad()
             optimizer_parameters.zero_grad()
             # Reset the sourcing model with the learned init inventory
             sourcing_model.reset()
             total_cost = self.get_total_cost(sourcing_model, sourcing_periods)
             total_cost.backward()
             # Perform gradient descend
-            if epoch % 3 == 0:
+            if epoch % init_inventory_freq == 0:
                 optimizer_init_inventory.step()
             else:
                 optimizer_parameters.step()
             # Save the best model
-            if validation_sourcing_periods is not None and epoch % 10 == 0:
+            if validation_sourcing_periods is not None and epoch % validation_freq == 0:
                 eval_cost = self.get_total_cost(
                     sourcing_model, validation_sourcing_periods
                 )
                 if eval_cost < min_cost:
                     min_cost = eval_cost
                     best_state = self.state_dict()
             else:
@@ -543,20 +579,21 @@
                     min_cost = total_cost
                     best_state = self.state_dict()
             # Log train loss
             if tensorboard_writer is not None:
                 tensorboard_writer.add_scalar(
                     "Avg. cost per period/train", total_cost / sourcing_periods, epoch
                 )
-                # Log evaluation loss
-                tensorboard_writer.add_scalar(
-                    "Avg. cost per period/eval",
-                    eval_cost / validation_sourcing_periods,
-                    epoch,
-                )
+                if validation_sourcing_periods is not None and epoch % 10 == 0:
+                    # Log validation loss
+                    tensorboard_writer.add_scalar(
+                        "Avg. cost per period/val",
+                        eval_cost / validation_sourcing_periods,
+                        epoch,
+                    )
                 tensorboard_writer.flush()
 
         self.load_state_dict(best_state)
 
     def simulate(self, sourcing_model, sourcing_periods, seed=None):
         """
         Simulate the sourcing model using the neural network.
@@ -596,43 +633,51 @@
             sourcing_model.get_past_regular_orders()[0, :].detach().numpy()
         )
         past_expedited_orders = (
             sourcing_model.get_past_expedited_orders()[0, :].detach().numpy()
         )
         return past_inventories, past_regular_orders, past_expedited_orders
 
-    def plot(self, sourcing_model, sourcing_periods):
+    def plot(self, sourcing_model, sourcing_periods, linewidth=1):
         """
         Plot the inventory and order quantities.
 
         Parameters
         ----------
         sourcing_model : DualSourcingModel
             The sourcing model.
         sourcing_periods : int
             Number of sourcing periods.
+        linewidth : int, default is 1
+            Width of the line in the step plots.
         """
+        import matplotlib as mpl
+
         past_inventories, past_regular_orders, past_expedited_orders = self.simulate(
             sourcing_model=sourcing_model, sourcing_periods=sourcing_periods
         )
         fig, ax = plt.subplots(ncols=2, figsize=(10, 4))
-        ax[0].step(range(sourcing_periods), past_inventories[-sourcing_periods:])
+        ax[0].step(range(sourcing_periods), past_inventories[-sourcing_periods:], linewidth=linewidth, color='tab:blue')
         ax[0].yaxis.get_major_locator().set_params(integer=True)
         ax[0].set_title("Inventory")
         ax[0].set_xlabel("Period")
         ax[0].set_ylabel("Quantity")
 
         ax[1].step(
             range(sourcing_periods),
             past_expedited_orders[-sourcing_periods:],
             label="Expedited Order",
+            linewidth=linewidth,
+            color='tab:green'
         )
         ax[1].step(
             range(sourcing_periods),
             past_regular_orders[-sourcing_periods:],
             label="Regular Order",
+            linewidth=linewidth,
+            color='tab:orange'
         )
         ax[1].yaxis.get_major_locator().set_params(integer=True)
         ax[1].set_title("Order")
         ax[1].set_xlabel("Period")
         ax[1].set_ylabel("Quantity")
-        ax[1].legend()
+        ax[1].legend()
```

### Comparing `idinn-0.1.4/src/idinn/demand.py` & `idinn-0.1.5/src/idinn/demand.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 class UniformDemand(BaseDemand):
     def __init__(self, low, high):
         self.distribution = torch.distributions.Uniform(low=low, high=high + 1)
 
     def reset(self):
         pass
 
-    def sample(self, size) -> torch.Tensor:
-        return self.distribution.sample([size, 1]).int()
+    def sample(self, batch_size) -> torch.Tensor:
+        return self.distribution.sample([batch_size, 1]).int()
 
 
 class CustomDemand(BaseDemand):
     def __init__(self, demand_history):
         """
         Parameters
         ----------
```

### Comparing `idinn-0.1.4/src/idinn/sourcing_model.py` & `idinn-0.1.5/src/idinn/sourcing_model.py`

 * *Files identical despite different names*

### Comparing `idinn-0.1.4/tests/test_controller.py` & `idinn-0.1.5/tests/test_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         hidden_layers = [4, 2],
         activation = torch.nn.ReLU()
     )
     single_sourcing_controller.init_layers(lead_time=2)
     return single_sourcing_controller
 
 def test_single_controller_init_layers(single_sourcing_controller: SingleSourcingNeuralController):
-    assert len(single_sourcing_controller.stack) == 6
+    assert len(single_sourcing_controller.architecture) == 6
 
 def test_single_controller_forward(single_sourcing_controller: SingleSourcingNeuralController):
     current_inventory = 10
     past_orders = [0, 0]
     q = single_sourcing_controller.forward(current_inventory, past_orders)
     assert q.shape == torch.Size([1, 1])
 
@@ -36,16 +36,16 @@
     assert total_cost.item() == 14.0
 
 def test_single_controller_simulate(single_sourcing_model: SingleSourcingModel, single_sourcing_controller: SingleSourcingNeuralController):
     past_inventories, past_orders = single_sourcing_controller.simulate(single_sourcing_model, sourcing_periods=5, seed=42)
     assert past_inventories[0] == 10
     assert past_orders[0] == 0
 
-def test_single_controller_train(single_sourcing_model: SingleSourcingModel, single_sourcing_controller: SingleSourcingNeuralController):
-    single_sourcing_controller.train(single_sourcing_model, sourcing_periods=5, epochs=1)
+def test_single_controller_fit(single_sourcing_model: SingleSourcingModel, single_sourcing_controller: SingleSourcingNeuralController):
+    single_sourcing_controller.fit(single_sourcing_model, sourcing_periods=5, epochs=1)
 
 def test_single_controller_plot(single_sourcing_model: SingleSourcingModel, single_sourcing_controller: SingleSourcingNeuralController):
     single_sourcing_controller.plot(single_sourcing_model, sourcing_periods=5)
 
 @pytest.fixture
 def dual_sourcing_model():
     """
@@ -68,34 +68,34 @@
         hidden_layers = [4, 2],
         activation = torch.nn.ReLU()
     )
     dual_sourcing_controller.init_layers(regular_lead_time=2, expedited_lead_time=1)
     return dual_sourcing_controller
 
 def test_dual_controller_init_layers(dual_sourcing_controller: DualSourcingNeuralController):
-    assert len(dual_sourcing_controller.stack) == 6
-    assert dual_sourcing_controller.stack[-2].out_features == 2
+    assert len(dual_sourcing_controller.architecture) == 6
+    assert dual_sourcing_controller.architecture[-2].out_features == 2
 
 def test_dual_controller_forward(dual_sourcing_controller: DualSourcingNeuralController):
     current_inventory = 10
     past_regular_orders = [0, 0]
     past_expedited_orders = [0, 0]
     q = dual_sourcing_controller.forward(current_inventory, past_regular_orders, past_expedited_orders)
     assert len(q) == 2
     assert q[0].shape == torch.Size([1, 1])
     assert q[1].shape == torch.Size([1, 1])
 
 def test_dual_controller_get_total_cost(dual_sourcing_model: DualSourcingModel, dual_sourcing_controller: DualSourcingNeuralController):
     total_cost = dual_sourcing_controller.get_total_cost(dual_sourcing_model, sourcing_periods=5, seed=42)
-    assert total_cost.item() == 12.0
+    assert total_cost.item() == 14.0
 
 def test_dual_controller_simulate(dual_sourcing_model: DualSourcingModel, dual_sourcing_controller: DualSourcingNeuralController):
     past_inventories, past_regular_orders, past_expedited_orders = dual_sourcing_controller.simulate(dual_sourcing_model, sourcing_periods=5, seed=42)
     assert past_inventories[0] == 10
     assert past_regular_orders[0] == 0
     assert past_expedited_orders[0] == 0
 
-def test_dual_controller_train(dual_sourcing_model: DualSourcingModel, dual_sourcing_controller: DualSourcingNeuralController):
-    dual_sourcing_controller.train(dual_sourcing_model, sourcing_periods=5, epochs=1)
+def test_dual_controller_fit(dual_sourcing_model: DualSourcingModel, dual_sourcing_controller: DualSourcingNeuralController):
+    dual_sourcing_controller.fit(dual_sourcing_model, sourcing_periods=5, epochs=1)
 
 def test_dual_controller_plot(dual_sourcing_model: DualSourcingModel, dual_sourcing_controller: DualSourcingNeuralController):
     dual_sourcing_controller.plot(dual_sourcing_model, sourcing_periods=5)
```

### Comparing `idinn-0.1.4/tests/test_sourcing_model.py` & `idinn-0.1.5/tests/test_sourcing_model.py`

 * *Files identical despite different names*

### Comparing `idinn-0.1.4/.gitignore` & `idinn-0.1.5/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -160,11 +160,14 @@
 #.idea/
 
 # VS Code and macOS
 .vscode
 .DS_Store
 
 # Jupyter notebooks
-*.ipynb
+# *.ipynb
 
 # PyTorch checkpoints
-*.pt
+*.pt
+
+# Tensorboard runs
+runs/
```

### Comparing `idinn-0.1.4/LICENSE` & `idinn-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `idinn-0.1.4/README.md` & `idinn-0.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # idinn: Inventory-Dynamics Control with Neural Networks
 
+[![PyPI Latest Release](https://img.shields.io/pypi/v/idinn.svg)](https://pypi.org/project/idinn/)
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1BAMiveGXmErIp10MK3V_SUJlDAXHAyaI)
+
 [<img src="https://gitlab.com/ComputationalScience/idinn/-/raw/main/docs/_static/youtube.png" align="center" width="60%" size="auto" alt="youtube">](https://www.youtube.com/watch?v=hUBfTWV6tWQ)
 
 `idinn` implements **i**nventory **d**ynamics–**i**nformed **n**eural **n**etworks for solving single-sourcing and dual-sourcing problems. Neural network controllers and inventory dynamics are implemented into customizable objects with PyTorch backend to enable users to find the optimal neural controllers for the user-specified inventory systems.
 
 ## Installation
 
 The package can be installed form PyPI. To do that, run
@@ -22,37 +25,35 @@
 
 ## Example Usage
 
 ```python
 import torch
 from idinn.sourcing_model import SingleSourcingModel
 from idinn.controller import SingleSourcingNeuralController
+from idinn.demand import UniformDemand
 
 # Initialize the sourcing model and the neural controller
 sourcing_model = SingleSourcingModel(
     lead_time=0,
     holding_cost=5,
     shortage_cost=495,
     batch_size=32,
     init_inventory=10,
-    demand_distribution="uniform",
-    demand_low=1,
-    demand_high=4
+    demand_generator=UniformDemand(low=1, high=4),
 )
-controller = SingleFullyConnectedNeuralController(
+controller = SingleSourcingNeuralController(
     hidden_layers=[2],
     activation=torch.nn.CELU(alpha=1)
 )
 # Train the neural controller
-controller.train(
+controller.fit(
     sourcing_model=sourcing_model,
     sourcing_periods=50,
     validation_sourcing_periods=1000,
     epochs=5000,
-    tensorboard_writer=torch.utils.tensorboard.SummaryWriter(),
     seed=1,
 )
 # Simulate and plot the results
 controller.plot(sourcing_model=sourcing_model, sourcing_periods=100)
 # Calculate the optimal order quantity for applications
 controller.forward(current_inventory=10, past_orders=[1, 5])
 ```
```

### Comparing `idinn-0.1.4/pyproject.toml` & `idinn-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 keywords = ["neural networks", "dynamic control"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
-dependencies = ["numpy", "matplotlib", "torch>=2.0"]
+dependencies = ["numpy", "matplotlib", "tensorboard", "torch~=2.0"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://gitlab.com/ComputationalScience/idinn"
 Documentation = "https://inventory-optimization.readthedocs.io"
 Issues = "https://gitlab.com/ComputationalScience/idinn/-/issues"
```

### Comparing `idinn-0.1.4/PKG-INFO` & `idinn-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idinn
-Version: 0.1.4
+Version: 0.1.5
 Summary: Inventory dynamics–informed neural networks for solving single-sourcing and dual-sourcing problems.
 Project-URL: Homepage, https://gitlab.com/ComputationalScience/idinn
 Project-URL: Documentation, https://inventory-optimization.readthedocs.io
 Project-URL: Issues, https://gitlab.com/ComputationalScience/idinn/-/issues
 Author-email: Jiawei Li <sud.concept0x@icloud.com>, Thomas Asikis <thomas.asikis@uzh.ch>, Ioannis Fragkos <fragkos@rsm.nl>, Lucas Boettcher <l.boettcher@fs.de>
 License: MIT License
         
@@ -31,19 +31,23 @@
 Keywords: dynamic control,neural networks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: matplotlib
 Requires-Dist: numpy
-Requires-Dist: torch>=2.0
+Requires-Dist: tensorboard
+Requires-Dist: torch~=2.0
 Description-Content-Type: text/markdown
 
 # idinn: Inventory-Dynamics Control with Neural Networks
 
+[![PyPI Latest Release](https://img.shields.io/pypi/v/idinn.svg)](https://pypi.org/project/idinn/)
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1BAMiveGXmErIp10MK3V_SUJlDAXHAyaI)
+
 [<img src="https://gitlab.com/ComputationalScience/idinn/-/raw/main/docs/_static/youtube.png" align="center" width="60%" size="auto" alt="youtube">](https://www.youtube.com/watch?v=hUBfTWV6tWQ)
 
 `idinn` implements **i**nventory **d**ynamics–**i**nformed **n**eural **n**etworks for solving single-sourcing and dual-sourcing problems. Neural network controllers and inventory dynamics are implemented into customizable objects with PyTorch backend to enable users to find the optimal neural controllers for the user-specified inventory systems.
 
 ## Installation
 
 The package can be installed form PyPI. To do that, run
@@ -62,37 +66,35 @@
 
 ## Example Usage
 
 ```python
 import torch
 from idinn.sourcing_model import SingleSourcingModel
 from idinn.controller import SingleSourcingNeuralController
+from idinn.demand import UniformDemand
 
 # Initialize the sourcing model and the neural controller
 sourcing_model = SingleSourcingModel(
     lead_time=0,
     holding_cost=5,
     shortage_cost=495,
     batch_size=32,
     init_inventory=10,
-    demand_distribution="uniform",
-    demand_low=1,
-    demand_high=4
+    demand_generator=UniformDemand(low=1, high=4),
 )
-controller = SingleFullyConnectedNeuralController(
+controller = SingleSourcingNeuralController(
     hidden_layers=[2],
     activation=torch.nn.CELU(alpha=1)
 )
 # Train the neural controller
-controller.train(
+controller.fit(
     sourcing_model=sourcing_model,
     sourcing_periods=50,
     validation_sourcing_periods=1000,
     epochs=5000,
-    tensorboard_writer=torch.utils.tensorboard.SummaryWriter(),
     seed=1,
 )
 # Simulate and plot the results
 controller.plot(sourcing_model=sourcing_model, sourcing_periods=100)
 # Calculate the optimal order quantity for applications
 controller.forward(current_inventory=10, past_orders=[1, 5])
 ```
```

