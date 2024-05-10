# Comparing `tmp/openterrace-0.1.2.tar.gz` & `tmp/openterrace-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openterrace-0.1.2.tar", max compression
+gzip compressed data, was "openterrace-0.1.3.tar", max compression
```

## Comparing `openterrace-0.1.2.tar` & `openterrace-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0    35146 2024-03-25 07:33:37.228525 openterrace-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1838 2024-03-25 07:33:37.228525 openterrace-0.1.2/README.md
--rw-r--r--   0        0        0      177 2024-03-25 07:33:47.824579 openterrace-0.1.2/openterrace/__init__.py
--rw-r--r--   0        0        0     2360 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/analytical_functions.py
--rw-r--r--   0        0        0     3021 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/bed_substances/ATS50.py
--rw-r--r--   0        0        0     3021 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/bed_substances/ATS58.py
--rw-r--r--   0        0        0      210 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/bed_substances/__init__.py
--rw-r--r--   0        0        0     1653 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/bed_substances/magnetite.py
--rw-r--r--   0        0        0     1661 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/bed_substances/swedish_diabase.py
--rw-r--r--   0        0        0      210 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/convection_schemes/__init__.py
--rw-r--r--   0        0        0      477 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/convection_schemes/upwind_1d.py
--rw-r--r--   0        0        0      210 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/diffusion_schemes/__init__.py
--rw-r--r--   0        0        0      498 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/diffusion_schemes/central_difference_1d.py
--rw-r--r--   0        0        0      210 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/domains/__init__.py
--rw-r--r--   0        0        0     1542 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/domains/block_1d.py
--rw-r--r--   0        0        0     1604 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/domains/cylinder_1d.py
--rw-r--r--   0        0        0     1923 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/domains/hollow_sphere_1d.py
--rw-r--r--   0        0        0     1242 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/domains/lumped.py
--rw-r--r--   0        0        0     1646 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/domains/sphere_1d.py
--rw-r--r--   0        0        0      210 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/fluid_substances/__init__.py
--rw-r--r--   0        0        0     3077 2024-03-25 07:33:37.240525 openterrace-0.1.2/openterrace/fluid_substances/air.py
--rw-r--r--   0        0        0     3250 2024-03-25 07:33:37.244525 openterrace-0.1.2/openterrace/fluid_substances/water.py
--rw-r--r--   0        0        0    16340 2024-03-25 07:33:37.244525 openterrace-0.1.2/openterrace/openterrace.py
--rw-r--r--   0        0        0      210 2024-03-25 07:33:37.244525 openterrace-0.1.2/openterrace/postprocessing/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 07:33:37.244525 openterrace-0.1.2/openterrace/postprocessing/animation.py
--rw-r--r--   0        0        0        6 2024-03-25 07:33:37.244525 openterrace-0.1.2/openterrace/postprocessing/panda_dataframe.py
--rw-r--r--   0        0        0     6737 2024-03-25 07:33:37.244525 openterrace-0.1.2/openterrace/tests/test_functions.py
--rw-r--r--   0        0        0     1227 2024-03-25 07:33:47.824579 openterrace-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2608 1970-01-01 00:00:00.000000 openterrace-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35146 2024-05-10 10:17:29.938021 openterrace-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1786 2024-05-10 10:17:29.938021 openterrace-0.1.3/README.md
+-rw-r--r--   0        0        0      177 2024-05-10 10:17:50.642204 openterrace-0.1.3/openterrace/__init__.py
+-rw-r--r--   0        0        0     2360 2024-05-10 10:17:29.946021 openterrace-0.1.3/openterrace/analytical_functions.py
+-rw-r--r--   0        0        0     3021 2024-05-10 10:17:29.946021 openterrace-0.1.3/openterrace/bed_substances/ATS50.py
+-rw-r--r--   0        0        0     3021 2024-05-10 10:17:29.946021 openterrace-0.1.3/openterrace/bed_substances/ATS58.py
+-rw-r--r--   0        0        0      210 2024-05-10 10:17:29.946021 openterrace-0.1.3/openterrace/bed_substances/__init__.py
+-rw-r--r--   0        0        0     1653 2024-05-10 10:17:29.946021 openterrace-0.1.3/openterrace/bed_substances/magnetite.py
+-rw-r--r--   0        0        0     1661 2024-05-10 10:17:29.946021 openterrace-0.1.3/openterrace/bed_substances/swedish_diabase.py
+-rw-r--r--   0        0        0      210 2024-05-10 10:17:29.946021 openterrace-0.1.3/openterrace/convection_schemes/__init__.py
+-rw-r--r--   0        0        0      477 2024-05-10 10:17:29.946021 openterrace-0.1.3/openterrace/convection_schemes/upwind_1d.py
+-rw-r--r--   0        0        0      210 2024-05-10 10:17:29.946021 openterrace-0.1.3/openterrace/diffusion_schemes/__init__.py
+-rw-r--r--   0        0        0      383 2024-05-10 10:17:29.946021 openterrace-0.1.3/openterrace/diffusion_schemes/central_difference_1d.py
+-rw-r--r--   0        0        0      210 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/domains/__init__.py
+-rw-r--r--   0        0        0     1542 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/domains/block_1d.py
+-rw-r--r--   0        0        0     1604 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/domains/cylinder_1d.py
+-rw-r--r--   0        0        0     1923 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/domains/hollow_sphere_1d.py
+-rw-r--r--   0        0        0     1242 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/domains/lumped.py
+-rw-r--r--   0        0        0     1646 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/domains/sphere_1d.py
+-rw-r--r--   0        0        0      210 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/fluid_substances/__init__.py
+-rw-r--r--   0        0        0     3077 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/fluid_substances/air.py
+-rw-r--r--   0        0        0     3250 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/fluid_substances/water.py
+-rw-r--r--   0        0        0    16563 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/openterrace.py
+-rw-r--r--   0        0        0      210 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/postprocessing/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/postprocessing/animation.py
+-rw-r--r--   0        0        0        6 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/postprocessing/panda_dataframe.py
+-rw-r--r--   0        0        0     1790 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/tests/test_advection_step_function.py
+-rw-r--r--   0        0        0     1313 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/tests/test_energy_conservation.py
+-rw-r--r--   0        0        0     1967 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/tests/test_heat_diffusion_sphere.py
+-rw-r--r--   0        0        0     2076 2024-05-10 10:17:29.950021 openterrace-0.1.3/openterrace/tests/test_heat_diffusion_wall.py
+-rw-r--r--   0        0        0     1564 2024-05-10 10:17:50.642204 openterrace-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 openterrace-0.1.3/PKG-INFO
```

### Comparing `openterrace-0.1.2/LICENSE.txt` & `openterrace-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/README.md` & `openterrace-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,53 @@
+Metadata-Version: 2.1
+Name: openterrace
+Version: 0.1.3
+Summary: OpenTerrace: A fast, flexible and extendable Python framework for thermal energy storage packed bed simulations
+Home-page: https://github.com/OpenTerrace/openterrace-python
+License: MIT
+Keywords: Thermal energy storage,Packed bed,Simulation,Heat transfer,Phase change material,PCM,Python
+Author: Jakob Hærvig
+Maintainer: Jakob Hærvig
+Maintainer-email: jakob.haervig@gmail.com
+Requires-Python: ==3.11.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: matplotlib (==3.8.3)
+Requires-Dist: numba (==0.59.0)
+Requires-Dist: numpy (==1.26.4)
+Requires-Dist: pytest-xdist (==3.5.0)
+Requires-Dist: scipy (==1.12.0)
+Requires-Dist: tqdm (==4.66.2)
+Project-URL: Bug Tracker, https://github.com/OpenTerrace/openterrace-python/issues
+Project-URL: Documentation, https://openterrace.github.io/openterrace-python/
+Project-URL: Repository, https://github.com/OpenTerrace/openterrace-python
+Description-Content-Type: text/markdown
+
 ![GitHub Release](https://img.shields.io/github/v/release/OpenTerrace/openterrace-python) ![PyPI - Version](https://img.shields.io/pypi/v/openterrace)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openterrace) ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/openterrace/openterrace-python/pytest.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openterrace) ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/openterrace/openterrace-python/pytest.yml) ![GitHub Issues](https://img.shields.io/github/issues/openterrace/openterrace-python
+)
 
 
-[![Logo](docs/_figures/logo-banner-paths-green.svg)](#)
+![Logo](https://raw.githubusercontent.com/OpenTerrace/openterrace-python/main/docs/_figures/logo-openterrace.svg)
 
-OpenTerrace is a pure Python framework for thermal energy storage packed bed simulations. It is built from the ground up to be flexible and extendable on modern Python 3.x with speed in mind. It utilises Nvidia CUDA cores to harness the power of modern GPUs and has automatic fallback to CPU cores.
+OpenTerrace is a pure Python framework for thermal energy storage packed bed simulations. It is built from the ground up to be flexible and extendable on modern Python 3.x with speed in mind.
 
 OpenTerrace uses awesome open-source software such as
 [Numba](https://numba.pydata.org), [NumPy](https://numpy.org/) and [SciPy](https://scipy.org/):grey_exclamation:
 
 ### [Read the documentation of OpenTerrace](https://openterrace.github.io/openterrace-python/)
 
 ## Why OpenTerrace?
 - **FAST**  
-By making use of modern compilers and optimised tri-diagonal matrix solvers, OpenTerrace approaches the speed of compiled C or FORTRAN code with the added convenience of easy-to-read Python language.
+By making use of modern compilers and optimised tri-diagonal matrix solvers, OpenTerrace is built to be fast.
 
 - **FLEXIBLE**  
 OpenTerrace is built from the ground up to be flexible for easy integration in system models or optimisation loops.
 
 - **EXTENDABLE**  
 Modules for new materials such as non-spherical rocks or exotic Phase Change Materials (PCM) can easily be plugged into the OpenTerrace framework.
 
 ## Want to contribute?
 Contributions are welcome :pray: Feel free to send pull requests or get in touch with me to discuss how to collaborate. More details in the [docs](https://openterrace.github.io/openterrace-python/).
 
 ## Code contributors
-* Jakob Hærvig, Associate Professor, AAU Energy, Aalborg University, Denmark
+* Jakob Hærvig, Associate Professor, AAU Energy, Aalborg University, Denmark
```

### Comparing `openterrace-0.1.2/openterrace/analytical_functions.py` & `openterrace-0.1.3/openterrace/analytical_functions.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/bed_substances/ATS50.py` & `openterrace-0.1.3/openterrace/bed_substances/ATS50.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/bed_substances/ATS58.py` & `openterrace-0.1.3/openterrace/bed_substances/ATS58.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/bed_substances/magnetite.py` & `openterrace-0.1.3/openterrace/bed_substances/magnetite.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/bed_substances/swedish_diabase.py` & `openterrace-0.1.3/openterrace/bed_substances/swedish_diabase.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/domains/block_1d.py` & `openterrace-0.1.3/openterrace/domains/block_1d.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/domains/cylinder_1d.py` & `openterrace-0.1.3/openterrace/domains/cylinder_1d.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/domains/hollow_sphere_1d.py` & `openterrace-0.1.3/openterrace/domains/hollow_sphere_1d.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/domains/lumped.py` & `openterrace-0.1.3/openterrace/domains/lumped.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/domains/sphere_1d.py` & `openterrace-0.1.3/openterrace/domains/sphere_1d.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/fluid_substances/air.py` & `openterrace-0.1.3/openterrace/fluid_substances/air.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/fluid_substances/water.py` & `openterrace-0.1.3/openterrace/fluid_substances/water.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.1.2/openterrace/openterrace.py` & `openterrace-0.1.3/openterrace/openterrace.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,38 +57,45 @@
         if h_exp not in valid_h_exp:
             raise Exception("h_exp \'"+h_exp+"\' specified. Valid options for h_exp are:", valid_h_exp)
         
         self.coupling.append({"fluid_phase":fluid_phase, "bed_phase":bed_phase, "h_exp":h_exp, "h_value":h_value})
         self.flag_coupling = True
 
     def _coupling(self):
+        """This is the function that couples the fluid and bed phase."""
         for couple in self.coupling:
-            Q = couple['h_value']*self.Phase.instances[couple['bed_phase']].domain.A[-1][-1]*(self.Phase.instances[couple['fluid_phase']].T[0]-self.Phase.instances[couple['bed_phase']].T[:,-1])*self.dt
-            self.Phase.instances[couple['bed_phase']].h[:,-1] = self.Phase.instances[couple['bed_phase']].h[:,-1] + Q/(self.Phase.instances[couple['bed_phase']].rho[:,-1] * self.Phase.instances[couple['bed_phase']].domain.V[-1])
-            self.Phase.instances[couple['fluid_phase']].h[0] = self.Phase.instances[couple['fluid_phase']].h[0] - (1-self.Phase.instances[couple['fluid_phase']].phi)/self.Phase.instances[couple['fluid_phase']].phi * self.Phase.instances[couple['fluid_phase']].domain.V/self.Phase.instances[couple['bed_phase']].domain.V0 * Q/(self.Phase.instances[couple['fluid_phase']].rho*self.Phase.instances[couple['fluid_phase']].domain.V)
+            n_bed = self.Phase.instances[couple['fluid_phase']].domain.V/self.Phase.instances[couple['fluid_phase']].phi*(1-self.Phase.instances[couple['fluid_phase']].phi)/self.Phase.instances[couple['bed_phase']].domain.V0 #ok
 
+            Q = couple['h_value']*self.Phase.instances[couple['bed_phase']].domain.A[-1][-1]*(self.Phase.instances[couple['fluid_phase']].T[0]-self.Phase.instances[couple['bed_phase']].T[:,-1])*self.dt #ok
+
+            self.Phase.instances[couple['bed_phase']].h[:,-1] = self.Phase.instances[couple['bed_phase']].h[:,-1] + Q/(self.Phase.instances[couple['bed_phase']].rho[:,-1] * self.Phase.instances[couple['bed_phase']].domain.V[-1]) #ok
+
+            self.Phase.instances[couple['fluid_phase']].h[0] = self.Phase.instances[couple['fluid_phase']].h[0] - n_bed * Q/(self.Phase.instances[couple['fluid_phase']].rho*self.Phase.instances[couple['fluid_phase']].domain.V) #ok
+            
     def run_simulation(self):
         """This is the function full of magic."""
 
         for t in tqdm.tqdm(np.arange(self.t_start, self.t_end+self.dt, self.dt)):
+            
             for phase_instance in self.Phase.instances:
                 phase_instance._save_data(t)
                 phase_instance._solve_equations(t, self.dt)
                 phase_instance._update_properties()
             if self.flag_coupling:
                 self._coupling()
     class Phase:
         instances = []
         """Main class to define either the fluid or bed phase."""
 
         def __init__(self, outer=None, n:int=None, n_other:int=None, type:str=None):
             """Initialise a phase with number of control points and type.
 
             Args:
-                n_self (int): Number of discretisations for the given phase
+                outer (object): Outer class
+                n (int): Number of discretisations for the given phase
                 n_other (int): Number of discretisations for the other phase
                 type (str): Type of phase
             """
 
             self.outer = outer
             self.__class__.instances.append(self)
             self.n = n
@@ -146,23 +153,23 @@
             self.fcns.h_correlation = getattr(globals()['heat_transfer_correlations'], correlation)
 
         def select_domain_shape(self, domain:str=None, **kwargs):
             """Select domain shape and initialise constants.
             
             Args:
                 domain (str): Domain type
-                additional arguments (float): Dimensions of domain
+                **kwargs (float): Dimensions of domain to be specified depnding on the domain type
             """
 
             if not domain:
                 raise Exception("Keyword 'domain' not specified.")
             if not domain in globals()['domains'].__all__:
                 raise Exception("domain \'"+domain+"\' specified. Valid options for domain are:", self.valid_domains)
 
-            kwargs['n'] = self.n
+            kwargs['n'] = self.n 
             self.domain = getattr(globals()['domains'], domain)
             self.domain.type = domain
             self.domain.validate_input(kwargs, domain)
             self.domain.shape = self.domain.shape(kwargs)
             self.domain.dx = self.domain.dx(kwargs)
             self.domain.A = self.domain.A(kwargs)
             self.domain.V = self.domain.V(kwargs)
@@ -339,27 +346,27 @@
             for bc in self.bcs:
                 if bc['type'] == 'fixed_value':
                     self.h[bc['position']] = self.fcns.h(bc['value'])
                 if bc['type'] == 'fixed_value_timevarying':
                     self.h[bc['position']] = self.fcns.h(np.interp(t,bc['value'][:,0],bc['value'][:,1]))
                 if bc['type'] == 'zero_gradient':
                     if bc['position'] == np.s_[:,0]:
-                        self.h[bc['position']] = self.h[bc['position']] + (self.T[:,1]*self.D[1,:,0] - self.T[:,0]*self.D[1,:,0] - self.F[0,:,1]*self.T[:,1] + self.F[1,:,0]*self.T[:,0]) / (self.rho[:,0]*self.domain.V[0])*dt
+                        self.h[bc['position']] = self.h[bc['position']] + (2*self.T[:,1]*self.D[1,:,0] - 2*self.T[:,0]*self.D[1,:,0] - self.F[0,:,1]*self.T[:,1] + self.F[1,:,0]*self.T[:,0]) / (self.rho[:,0]*self.domain.V[0])*dt
                     if bc['position'] == np.s_[:,-1]:
-                        self.h[bc['position']] = self.h[bc['position']] + (self.T[:,-2]*self.D[0,:,-1] - self.T[:,-1]*self.D[0,:,-1] + self.F[1,:,-2]*self.T[:,-2] - self.F[0,:,-1]*self.T[:,-1]) / (self.rho[:,-1]*self.domain.V[-1])*dt
+                        self.h[bc['position']] = self.h[bc['position']] + (2*self.T[:,-2]*self.D[0,:,-1] - 2*self.T[:,-1]*self.D[0,:,-1] + self.F[1,:,-2]*self.T[:,-2] - self.F[0,:,-1]*self.T[:,-1]) / (self.rho[:,-1]*self.domain.V[-1])*dt
 
         def _update_source(self, dt:float=None):
             """Update source term.
             
             Args:
                 dt (float): Time step size
             """
 
             for source in self.sources:
-                self.h = self.h + (source['T_inf']-self.T) / source['R'] * dt/(self.rho*self.domain.V)
+                self.h = self.h + (source['T_inf']-self.T)*2 / source['R'] * dt/(self.rho*self.domain.V)
 
         def _solve_equations(self, t:float=None, dt:float=None):
             """Solve equations at each time step.
 
             Args:
                 t (float): Current time
                 dt (float): Time step size
```

### Comparing `openterrace-0.1.2/pyproject.toml` & `openterrace-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 [tool.poetry]
 name = "openterrace"
-description = "OpenTerrace is a pure Python framework for thermal energy storage packed bed simulations"
-version = "v0.1.2" # This will be overwritten by the dynamic versioning by Poetry
+description = "OpenTerrace: A fast, flexible and extendable Python framework for thermal energy storage packed bed simulations"
+version = "v0.1.3" # This will be overwritten by the dynamic versioning by Poetry
 authors = [
     "Jakob Hærvig"
 ]
+maintainers = [
+    "Jakob Hærvig <jakob.haervig@gmail.com>"
+]
 readme = "README.md"
 license = "MIT"
 
 packages = [
     { include = "openterrace"}
 ]
+keywords = [
+    "Thermal energy storage",
+    "Packed bed",
+    "Simulation",
+    "Heat transfer",
+    "Phase change material",
+    "PCM",
+    "Python"
+]
 
 repository = "https://github.com/OpenTerrace/openterrace-python"
 documentation = "https://openterrace.github.io/openterrace-python/"
 
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/OpenTerrace/openterrace-python/issues"
+
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 format = "v{base}"
 latest-tag = true
 
 [tool.poetry.dependencies]
```

