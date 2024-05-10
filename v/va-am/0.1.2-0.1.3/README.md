# Comparing `tmp/va_am-0.1.2.tar.gz` & `tmp/va_am-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "va_am-0.1.2.tar", last modified: Wed Apr 10 08:50:52 2024, max compression
+gzip compressed data, was "va_am-0.1.3.tar", last modified: Fri May 10 08:18:04 2024, max compression
```

## Comparing `va_am-0.1.2.tar` & `va_am-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-04-10 08:50:52.080531 va_am-0.1.2/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    35149 2023-09-29 09:45:51.000000 va_am-0.1.2/LICENSE
--rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-04-10 08:50:52.080531 va_am-0.1.2/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     5078 2024-02-12 18:26:04.000000 va_am-0.1.2/README.md
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      756 2024-04-10 08:48:41.000000 va_am-0.1.2/pyproject.toml
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       38 2024-04-10 08:50:52.080531 va_am-0.1.2/setup.cfg
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       68 2023-09-28 11:32:10.000000 va_am-0.1.2/setup.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-04-10 08:50:52.076531 va_am-0.1.2/src/
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-04-10 08:50:52.080531 va_am-0.1.2/src/va_am/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      222 2024-02-20 12:03:10.000000 va_am-0.1.2/src/va_am/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       66 2023-09-28 11:12:58.000000 va_am-0.1.2/src/va_am/__main__.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-04-10 08:50:52.080531 va_am-0.1.2/src/va_am/utils/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    61061 2024-02-16 14:28:14.000000 va_am-0.1.2/src/va_am/utils/AutoEncoders.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2023-06-29 15:33:10.000000 va_am-0.1.2/src/va_am/utils/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3123 2023-09-25 14:36:24.000000 va_am-0.1.2/src/va_am/utils/functions.py
--rw-r--r--   0 cosmin    (1000) cosmin    (1000)   102225 2024-04-05 12:17:06.000000 va_am-0.1.2/src/va_am/va_am.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-04-10 08:50:52.080531 va_am-0.1.2/src/va_am.egg-info/
--rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      393 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/SOURCES.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/dependency_links.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       46 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/entry_points.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       71 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/requires.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        6 2024-04-10 08:50:52.000000 va_am-0.1.2/src/va_am.egg-info/top_level.txt
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-10 08:18:04.457400 va_am-0.1.3/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    35149 2023-09-29 09:45:51.000000 va_am-0.1.3/LICENSE
+-rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-10 08:18:04.457400 va_am-0.1.3/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     5078 2024-02-12 18:26:04.000000 va_am-0.1.3/README.md
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      756 2024-05-10 08:07:35.000000 va_am-0.1.3/pyproject.toml
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       38 2024-05-10 08:18:04.457400 va_am-0.1.3/setup.cfg
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       68 2023-09-28 11:32:10.000000 va_am-0.1.3/setup.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-10 08:18:04.453400 va_am-0.1.3/src/
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-10 08:18:04.457400 va_am-0.1.3/src/va_am/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      222 2024-02-20 12:03:10.000000 va_am-0.1.3/src/va_am/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       66 2023-09-28 11:12:58.000000 va_am-0.1.3/src/va_am/__main__.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-10 08:18:04.457400 va_am-0.1.3/src/va_am/utils/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    61075 2024-05-10 08:06:35.000000 va_am-0.1.3/src/va_am/utils/AutoEncoders.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2023-06-29 15:33:10.000000 va_am-0.1.3/src/va_am/utils/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3123 2023-09-25 14:36:24.000000 va_am-0.1.3/src/va_am/utils/functions.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)   102749 2024-05-10 08:06:35.000000 va_am-0.1.3/src/va_am/va_am.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-10 08:18:04.457400 va_am-0.1.3/src/va_am.egg-info/
+-rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-10 08:18:04.000000 va_am-0.1.3/src/va_am.egg-info/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      393 2024-05-10 08:18:04.000000 va_am-0.1.3/src/va_am.egg-info/SOURCES.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2024-05-10 08:18:04.000000 va_am-0.1.3/src/va_am.egg-info/dependency_links.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       46 2024-05-10 08:18:04.000000 va_am-0.1.3/src/va_am.egg-info/entry_points.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       71 2024-05-10 08:18:04.000000 va_am-0.1.3/src/va_am.egg-info/requires.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        6 2024-05-10 08:18:04.000000 va_am-0.1.3/src/va_am.egg-info/top_level.txt
```

### Comparing `va_am-0.1.2/LICENSE` & `va_am-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `va_am-0.1.2/PKG-INFO` & `va_am-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: va_am
-Version: 0.1.2
+Version: 0.1.3
 Summary: VA-AM method implementation
 Author-email: cosminmarina <cosmin.marina@uah.es>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `va_am-0.1.2/README.md` & `va_am-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `va_am-0.1.2/pyproject.toml` & `va_am-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "va_am"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{name="cosminmarina", email="cosmin.marina@uah.es" }]
 description = "VA-AM method implementation"
 readme = "README.md"
 dependencies = ["requests","sympy","keras","tensorflow","xarray","netcdf4","matplotlib","pandas","numpy"]
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `va_am-0.1.2/src/va_am/utils/AutoEncoders.py` & `va_am-0.1.3/src/va_am/utils/AutoEncoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1279,77 +1279,81 @@
         )
 
         vae_loss = reconstruction_loss + kl_factor*kl_loss + class_factor*cross_entropy_loss
         self.autoencoder.add_loss(vae_loss)
 
         
         
-    def compile(self, optimizer='adam', loss='mse', metrics=['mae', 'mape']):
+    #def compile(self, optimizer='adam', loss='mse', metrics=['mae', 'mape'], **kwargs):
+    def compile(self, **kwargs):
         """
         Compilation of the AutoEncoder.
         Here we specify the method to optimize, the loss function and,
         if we want, some metrics to show together with the loss.
         
         Parameters
         ----------
-        optimizer: the method to use for optimization. It sould be one
-            of tensorflow.keras.optimizers.
-        loss: loss function to be optmized. It sould be one of 
-            tensorflow.keras.losses.
-        metrics: list of metrics to be evaluated by the model during 
-            training and testing. It sould be one of
-            tensorflow.keras.losses.
+        **kwargs: dict
+            all available parameters for fit method at the keras/tensorflow version. If not specified, the default paramaters are optimizer=Adam, loss=mse, metrics=[mae, mape].
+        
         Returns
         ----------
+        :
         No output, only compile the model.
         """
+        default_compile_params = {"optimizer":"adam", "loss":"mse", "metrics":["mae", "mape"]}
+        if kwargs:
+            default_compile_params.update(kwargs)
         if self.arch in [4, 14, 15]:
-            self.autoencoder.compile(optimizer=optimizer, metrics=metrics)
+            if "loss" in kwargs.keys():
+                kwargs.pop("loss")
+            self.autoencoder.compile(**default_compile_params)
         else:
-            self.autoencoder.compile(optimizer=optimizer, loss=loss, metrics=metrics)
+            self.autoencoder.compile(**default_compile_params)
 
-    def fit(self, x, y, epochs=100, batch_size=64, shuffle=True, validation_split=0.15, verbose=1, min_delta=3e-6, patience=10, restore_best_weights=True, mask=False):
+    def fit(self, x, y, epochs=100, verbose=1, min_delta=3e-6, patience=10, restore_best_weights=True, mask=None, **kwargs):
         """
         Training of the AutoEncoder.
         Here we specify the parameters for our training.
 
         Parameters
         ----------
-        x: input data.
-        y: output data (data to be compared and trained).
-        batch_size: int or None. Number of samples per epoch (gradient
-            update).
-        shuffle: boolean whether to shuddle the training data before
-            each epoch.
-        validation_split: float between 0 and 1. Fraction of the 
-            training data to be used as validation data.
-        verbose: 'auto', 0, 1 or 2. Differents modes of verbosity when
-            the model is trained.
-        min_delta: minimum change in the monitored quantity to qualify
-            as an improvement.
-        patience: number of epochs with no improvement adter wich
-            training will be stoped.
-        restore_best_weigths: boolean whether to restore model weights
-            from the epoch with the best value of the monitored
-            quantity
+        x:
+            input data.
+        y:
+            output data (data to be compared and trained).
+        epochs: int
+            number of epochs to train the model.
+        verbose: 'auto', 0, 1 or 2.
+            differents modes of verbosity when the model is trained.
+        min_delta: int or float
+            minimum change in the monitored quantity to qualify as an improvement.
+        patience: int
+            number of epochs with no improvement adter wich training will be stoped.
+        restore_best_weigths: bool
+            whether to restore model weights from the epoch with the best value of the monitoredquantity
+        **kwargs: dict
+            all available parameters for fit method at the keras/tensorflow version, except verbose and epochs
         
         Returns
         ----------
+        : History
         A History object. See History.history.
         """
+        default_fit_params = {"batch_size":64, "validation_split":0.15}
+        if kwargs:
+            default_fit_params.update(kwargs)
         callback = tf.keras.callbacks.EarlyStopping(monitor='val_loss', min_delta=min_delta, patience=patience,
                                     restore_best_weights=restore_best_weights)
         if mask is not None:
             x[:,mask,0] = 0
             if (x!=y).any():
                 y[:,mask,0] = 0
             else:
                 y = x
         history = self.autoencoder.fit(x, y,
                             epochs=epochs,
-                            shuffle=shuffle,
-                            validation_split=validation_split,
-                            batch_size=batch_size,
                             callbacks=callback,
-                            verbose=verbose
+                            verbose=verbose,
+                            **default_fit_params
                             )
         return history
```

### Comparing `va_am-0.1.2/src/va_am/utils/functions.py` & `va_am-0.1.3/src/va_am/utils/functions.py`

 * *Files identical despite different names*

### Comparing `va_am-0.1.2/src/va_am/va_am.py` & `va_am-0.1.3/src/va_am/va_am.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     divs = np.array(sympy.divisors(size))
     dist_to_root = np.abs(divs-np.sqrt(size)*ratio_w_h)
     i = np.argmin(dist_to_root)
     x_size = int(divs[i])
     y_size = size//x_size
     return (x_size, y_size) if x_size < y_size else (y_size, x_size)
 
-def runAE(input_dim: Union[int, list[int]], latent_dim: int, arch: int, use_VAE: bool, with_cpu: bool, n_epochs: int, data_prs: Union[np.ndarray, list, xr.DataArray], file_save: str, verbose: bool):
+def runAE(input_dim: Union[int, list[int]], latent_dim: int, arch: int, use_VAE: bool, with_cpu: bool, n_epochs: int, data_prs: Union[np.ndarray, list, xr.DataArray], file_save: str, verbose: bool, compile_params: dict = {}, fit_params : dict() = {}):
     """
       runAE
        
       Function that performs the AE traing.
         
       Parameters
       ----------
@@ -68,42 +68,46 @@
          Represent the shape of the latent (code) space.                            
       arch: int
          Value that determine which model architecture sould be used to build the model.  
       use_VAE : bool
          Value that determines if the model should be a Variational Autoencoder or not.
       with_cpu: bool
          Value that determines if the cpu should be used instead of (default) gpu.
-      verbose: bool
-         Value that determines if the execution information should be displayed.  
       n_epochs: int 
          The number of epochs for the keras.model.                     
       data_prs: np.ndarray
          Driver/predictor data (usually) to train the model.        
       file_save: str
-         Where to save the .h5 model.            
+         Where to save the .h5 model.
+      verbose: bool
+         Value that determines if the execution information should be displayed.  
+      compile_params: dict
+         Dictionary that contains all the parameters (avaible depending on tensorflow/keras version) to use for the .compile() function. 
+      fit_params: dict
+         Dictionary that contains all the parametes (avaible depending on tensorflow/keras version) to use for the .fit() function, except for epochs and verbose.
         
       Returns
       ----------                                            
       AE.encoder: keras.model.
          Keras object that correspond to the fitted encoder model.
     """
     verbose = 1 if verbose else 0
     if with_cpu:
         with tf.device("/cpu:0"):
             AE = AutoEncoders.AE_conv(input_dim=input_dim,latent_dim=latent_dim,arch=arch,in_channels=np.shape(data_prs)[-1],out_channels=np.shape(data_prs)[-1],VAE=use_VAE)
 
-            AE.compile(optimizer='adam', loss='mse')
+            AE.compile(**compile_params)
 
-            history = AE.fit(data_prs, data_prs, epochs=n_epochs, batch_size=128, min_delta=1e-6, patience=50, verbose=verbose)
+            history = AE.fit(data_prs, data_prs, epochs=n_epochs, min_delta=1e-6, patience=50, verbose=verbose, **fit_params)
     else:
         AE = AutoEncoders.AE_conv(input_dim=input_dim,latent_dim=latent_dim,arch=arch,in_channels=np.shape(data_prs)[-1],out_channels=np.shape(data_prs)[-1],VAE=use_VAE)
 
-        AE.compile(optimizer='adam', loss='mse')
+        AE.compile(**compile_params)
 
-        history = AE.fit(data_prs, data_prs, epochs=n_epochs, batch_size=128, min_delta=1e-6, patience=50, verbose=verbose)
+        history = AE.fit(data_prs, data_prs, epochs=n_epochs, min_delta=1e-6, patience=50, verbose=verbose, **fit_params)
 
     Path("./figures").mkdir(parents=True, exist_ok=True)
     plt.plot(history.history['loss'],label='loss')
     plt.plot(history.history['val_loss'],label='val_loss')
     plt.yscale('log')
     plt.legend()
     plt.savefig(f'./figures/history-{file_save[9:-3]}.png')
@@ -323,24 +327,24 @@
         if idx%2==0:
             if elem < value_list[idx]:
                 message = 'Your interest region is out of lat or lon minimum limits. I correct it, but be aware'
                 if is_teleg:
                     url = f"https://api.telegram.org/bot{token}/sendMessage?chat_id={chat_id}&text={'[WARN]: '+message}"
                     requests.get(url).json()
                 warnings.warn(message, stacklevel=2)
-            new_elem = max((elem - value_list[idx]) // resolution, 0)
+            new_elem = int(max((elem - value_list[idx]) // resolution, 0))
             new_interest_region.append(new_elem)
         else:
             if elem > value_list[idx]:
                 message = 'Your interest region is out of lat or lon maximum limits. I correct it, but be aware'
                 if is_teleg:
                     url = f"https://api.telegram.org/bot{token}/sendMessage?chat_id={chat_id}&text={'[WARN]: '+message}"
                     requests.get(url).json()
                 warnings.warn(message, stacklevel=2)
-            new_elem = min((elem - value_list[idx-1]) // resolution , (value_list[idx] - value_list[idx-1]) // resolution) + 1
+            new_elem = int(min((elem - value_list[idx-1]) // resolution , (value_list[idx] - value_list[idx-1]) // resolution) + 1)
             new_interest_region.append(new_elem)
     return new_interest_region
 
 def save_reconstruction(params: dict, reconstructions_Pre_Analog: list, reconstructions_Post_Analog: list, reconstructions_Pre_AE: list, reconstructions_Post_AE: list):
     """
       save_reconstruction
        
@@ -539,21 +543,14 @@
             requests.get(url).json()
         raise message
         
     data_of_interest_temp = indust_temp.sel(time=slice(params["data_of_interest_init"],params["data_of_interest_end"]))
     data_of_interest_prs = indust_prs.sel(time=slice(params["data_of_interest_init"],params["data_of_interest_end"]))
     
     if params["remove_year"]:
-        print(params["data_of_interest_init"])
-        print(type(params["data_of_interest_init"]))
-        t_i = str(params["data_of_interest_init"].year)
-        t_f = str(params["data_of_interest_end"].year)
-        print(t_i, t_f)
-        a = (indust_temp.sel(time=slice(t_i,t_f))).get_index('time')
-        print(a)
         indust_temp = indust_temp.drop_sel(time=(indust_temp.sel(time=slice(str(params["data_of_interest_init"].year),str(params["data_of_interest_end"].year)))).get_index('time'))
         indust_prs = indust_prs.drop_sel(time=(indust_prs.sel(time=slice(str(params["data_of_interest_init"].year),str(params["data_of_interest_end"].year)))).get_index('time'))
         if params["period"] == 'pre':
             if datetime.datetime.strptime(params["data_of_interest_init"], "%Y-%m-%d") < datetime.datetime.strptime(params["pre_end"], "%Y-%m-%d"):
                 pre_indust_temp = pre_indust_temp.drop_sel(time=(pre_indust_temp.sel(time=slice(str(params["data_of_interest_init"].year),str(params["data_of_interest_end"].year)))).get_index('time'))
                 pre_indust_prs = pre_indust_prs.drop_sel(time=(pre_indust_prs.sel(time=slice(str(params["data_of_interest_init"].year),str(params["data_of_interest_end"].year)))).get_index('time'))        
     else:
@@ -718,14 +715,18 @@
         if params["period"] in ['both', 'pre']:
             print(np.shape(pre_indust_prs))
             print(np.shape(pre_indust_temp[params["temp_var_name"]].data))
         print(np.shape(indust_prs))
         print(np.shape(indust_temp[params["temp_var_name"]].data))
 
     # AutoEncoder
+    if not "compile_params" in params.keys():
+        params["compile_params"] = {}
+    if not "fit_params" in params.keys():
+        params["fit_params"] = {}
     if params["load_AE"]:
         if params["period"] in ['both', 'pre']:
             AE_pre = keras.models.load_model(params["file_AE_pre"], custom_objects={'keras': keras,'AutoEncoders': AutoEncoders})
         if params["period"] in ['both', 'post']:
             AE_ind = keras.models.load_model(params["file_AE_post"], custom_objects={'keras': keras,'AutoEncoders': AutoEncoders})
         if params["verbose"]:
             print('AE loaded')
@@ -737,30 +738,30 @@
         elif "cvae_params" in params.keys():
             input_dim = [data_prs.dims.get('latitude'),data_prs.dims.get('longitude')] + params["cvae_params"]
         else:
             input_dim = [data_prs.dims.get('latitude'),data_prs.dims.get('longitude')]
         if params["period"] in ['both', 'pre']:
             AE_pre = keras.models.load_model(params["file_AE_pre"], custom_objects={'keras': keras,'AutoEncoders': AutoEncoders})
         if params["period"] in ['both', 'post']:
-            AE_ind = runAE(input_dim, params["latent_dim"], params["arch"], params["use_VAE"], params["with_cpu"], params["n_epochs"], x_train_ind_prs, params["file_AE_post"], params["verbose"])
+            AE_ind = runAE(input_dim, params["latent_dim"], params["arch"], params["use_VAE"], params["with_cpu"], params["n_epochs"], x_train_ind_prs, params["file_AE_post"], params["verbose"], params["compile_params"], params["fit_params"])
         if params["verbose"]:
             print('Fitting finished for post & AE loaded for pre')
     else:
         if params["verbose"]:
             print('Start fitting')
         if "kl_factor" in params.keys():
             input_dim = [data_prs.dims.get('latitude'),data_prs.dims.get('longitude'),params["kl_factor"]]
         elif "cvae_params" in params.keys():
             input_dim = [data_prs.dims.get('latitude'),data_prs.dims.get('longitude')] + params["cvae_params"]
         else:
             input_dim = [data_prs.dims.get('latitude'),data_prs.dims.get('longitude')]
         if params["period"] in ['both', 'pre']:
-            AE_pre = runAE(input_dim, params["latent_dim"], params["arch"], params["use_VAE"], params["with_cpu"], params["n_epochs"], x_train_pre_prs, params["file_AE_pre"], params["verbose"])
+            AE_pre = runAE(input_dim, params["latent_dim"], params["arch"], params["use_VAE"], params["with_cpu"], params["n_epochs"], x_train_pre_prs, params["file_AE_pre"], params["verbose"], params["compile_params"], params["fit_params"])
         if params["period"] in ['both', 'post']:
-            AE_ind = runAE(input_dim, params["latent_dim"], params["arch"], params["use_VAE"], params["with_cpu"], params["n_epochs"], x_train_ind_prs, params["file_AE_post"], params["verbose"])
+            AE_ind = runAE(input_dim, params["latent_dim"], params["arch"], params["use_VAE"], params["with_cpu"], params["n_epochs"], x_train_ind_prs, params["file_AE_post"], params["verbose"], params["compile_params"], params["fit_params"])
         if params["verbose"]:
             print('Fitting finished')
     
     # Analog comparison
     ## Stats analog
     if params["enhanced_distance"]:
         if params["period"] == 'both':
@@ -1121,14 +1122,15 @@
                 params_multiple["secret_file"] = args.secret
             if ident:
                 heatwave_period = identify_heatwave_days(params_multiple)
                 params_multiple["data_of_interest_init"] = heatwave_period
                 params_multiple["data_of_interest_end"] = heatwave_period
             else:
                 heatwave_period = np.arange(datetime.datetime.strptime(params_multiple["data_of_interest_init"], '%Y-%m-%d'), datetime.datetime.strptime(params_multiple["data_of_interest_end"], '%Y-%m-%d'), datetime.timedelta(days=1))
+                heatwave_period = np.array(list(map(pd.Timestamp, heatwave_period)))
                 params_multiple["data_of_interest_init"] = heatwave_period
                 params_multiple["data_of_interest_end"] = heatwave_period
             params = params_multiple.copy()
             file_params.close()
         if verb is not None:
             params["verbose"] = verb
         if "p" not in params.keys():
@@ -1423,14 +1425,15 @@
                 params_multiple["secret_file"] = args.secret
             if ident:
                 heatwave_period = identify_heatwave_days(params_multiple)
                 params_multiple["data_of_interest_init"] = heatwave_period
                 params_multiple["data_of_interest_end"] = heatwave_period
             else:
                 heatwave_period = np.arange(datetime.datetime.strptime(params_multiple["data_of_interest_init"], '%Y-%m-%d'), datetime.datetime.strptime(params_multiple["data_of_interest_end"], '%Y-%m-%d'), datetime.timedelta(days=1))
+                heatwave_period = np.array(list(map(pd.Timestamp, heatwave_period)))
                 params_multiple["data_of_interest_init"] = heatwave_period
                 params_multiple["data_of_interest_end"] = heatwave_period
             params = params_multiple.copy()
             file_params.close()
         if verb is not None:
             params["verbose"] = verb
         if "p" not in params.keys():
@@ -1683,15 +1686,15 @@
         "arch":                     5,
         "teleg":                    False,
         "verbose":                  False
     }
     params_multiple = None
     file_params_name = config_file
     n_execs = 5
-    verb = verbose
+    verb = None
     token = None
     chat_id = None
     user_name = None
     if teleg:
         with open(secret_file) as f:
             token = f.readline().strip()
             chat_id = f.readline().strip()
```

### Comparing `va_am-0.1.2/src/va_am.egg-info/PKG-INFO` & `va_am-0.1.3/src/va_am.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: va_am
-Version: 0.1.2
+Version: 0.1.3
 Summary: VA-AM method implementation
 Author-email: cosminmarina <cosmin.marina@uah.es>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

