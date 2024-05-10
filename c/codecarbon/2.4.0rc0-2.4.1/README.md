# Comparing `tmp/codecarbon-2.4.0rc0.tar.gz` & `tmp/codecarbon-2.4.1.tar.gz`

## Comparing `codecarbon-2.4.0rc0.tar` & `codecarbon-2.4.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/_version.py
--rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/emissions_tracker.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/input.py
--rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/output.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/cli/__init__.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/cli/cli_utils.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/__init__.py
--rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/api_client.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/cloud.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/co2_signal.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/config.py
--rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/cpu.py
--rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/emissions.py
--rw-r--r--   0        0        0    10300 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/gpu.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/measure.py
--rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/powermetrics.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/rapl.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/schemas.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/units.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/util.py
--rw-r--r--   0        0        0   409749 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/canada_provinces.geojson
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/cloud/impact.csv
--rw-r--r--   0        0        0    49714 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/hardware/cpu_power.csv
--rw-r--r--   0        0        0    49131 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2023-07-07-22-40-48.png
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/carbon_intensity_per_source.json
--rw-r--r--   0        0        0    49591 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/global_energy_mix.json
--rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/our_world_in_data-2022_data.ipynb
--rw-r--r--   0        0        0   420635 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/world_energy_mix.csv
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2016/canada_energy_mix.json
--rw-r--r--   0        0        0    48072 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2016/global_energy_mix-old.json
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2016/usa_emissions.json
--rw-r--r--   0        0        0    42145 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/01_get_world_carbon_intensity.ipynb
--rw-r--r--   0        0        0    29597 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/02_convert_csv_to_json.ipynb
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/03_add_eu_data.ipynb
--rw-r--r--   0        0        0    13207 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/eu-carbon-intensity-electricity.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/__init__.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/geography.py
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/hardware.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/logger.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/scheduler.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/prometheus/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/prometheus/metric_definitions.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/prometheus/prometheus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/__init__.py
--rw-r--r--   0        0        0    11006 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/carbonboard.py
--rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/carbonboard_on_api.py
--rw-r--r--   0        0        0    28035 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/components.py
--rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/assets/__init__.py
--rw-r--r--   0        0        0    25442 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/assets/car_icon.png
--rw-r--r--   0        0        0    29734 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/assets/house_icon.png
--rw-r--r--   0        0        0    29874 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/assets/tv_icon.png
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/.gitignore
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/LICENSE
--rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/README.md
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/pyproject.toml
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/_version.py
+-rw-r--r--   0        0        0    47126 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/emissions_tracker.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/input.py
+-rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/output.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/cli/__init__.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/cli/cli_utils.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/__init__.py
+-rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/api_client.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/cloud.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/co2_signal.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/config.py
+-rw-r--r--   0        0        0    13483 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/cpu.py
+-rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/emissions.py
+-rw-r--r--   0        0        0    10300 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/gpu.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/measure.py
+-rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/powermetrics.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/rapl.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/schemas.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/units.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/util.py
+-rw-r--r--   0        0        0   409749 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/canada_provinces.geojson
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/cloud/impact.csv
+-rw-r--r--   0        0        0    92710 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/hardware/cpu_power.csv
+-rw-r--r--   0        0        0    49131 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2023-07-07-22-40-48.png
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/carbon_intensity_per_source.json
+-rw-r--r--   0        0        0    49591 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/global_energy_mix.json
+-rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/our_world_in_data-2022_data.ipynb
+-rw-r--r--   0        0        0   420635 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/world_energy_mix.csv
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2016/canada_energy_mix.json
+-rw-r--r--   0        0        0    48072 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2016/global_energy_mix-old.json
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2016/usa_emissions.json
+-rw-r--r--   0        0        0    42145 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2020/01_get_world_carbon_intensity.ipynb
+-rw-r--r--   0        0        0    29597 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2020/02_convert_csv_to_json.ipynb
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2020/03_add_eu_data.ipynb
+-rw-r--r--   0        0        0    13207 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2020/eu-carbon-intensity-electricity.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/__init__.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/geography.py
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/hardware.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/logger.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/scheduler.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/prometheus/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/prometheus/metric_definitions.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/prometheus/prometheus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/__init__.py
+-rw-r--r--   0        0        0    11006 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/carbonboard.py
+-rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/carbonboard_on_api.py
+-rw-r--r--   0        0        0    28035 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/components.py
+-rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/assets/__init__.py
+-rw-r--r--   0        0        0    25442 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/assets/car_icon.png
+-rw-r--r--   0        0        0    29734 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/assets/house_icon.png
+-rw-r--r--   0        0        0    29874 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/assets/tv_icon.png
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 codecarbon-2.4.1/.gitignore
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 codecarbon-2.4.1/LICENSE
+-rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 codecarbon-2.4.1/README.md
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 codecarbon-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 codecarbon-2.4.1/PKG-INFO
```

### Comparing `codecarbon-2.4.0rc0/codecarbon/emissions_tracker.py` & `codecarbon-2.4.1/codecarbon/emissions_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,17 @@
             isinstance(self._gpu_ids, list)
             and all(isinstance(gpu_id, int) for gpu_id in self._gpu_ids)
         ):
             self._gpu_ids: List[int] = parse_gpu_ids(self._gpu_ids)
             self._conf["gpu_ids"] = self._gpu_ids
             self._conf["gpu_count"] = len(self._gpu_ids)
         else:
-            logger.warn("Invalid gpu_ids format. Expected a string or a list of ints.")
+            logger.warning(
+                "Invalid gpu_ids format. Expected a string or a list of ints."
+            )
 
         logger.info("[setup] RAM Tracking...")
         ram = RAM(tracking_mode=self._tracking_mode)
         self._conf["ram_total_size"] = ram.machine_memory_GB
         self._hardware: List[Union[RAM, CPU, GPU, AppleSiliconChip]] = [ram]
 
         # Hardware detection
```

### Comparing `codecarbon-2.4.0rc0/codecarbon/input.py` & `codecarbon-2.4.1/codecarbon/input.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/output.py` & `codecarbon-2.4.1/codecarbon/output.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/cli/cli_utils.py` & `codecarbon-2.4.1/codecarbon/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/cli/main.py` & `codecarbon-2.4.1/codecarbon/cli/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/api_client.py` & `codecarbon-2.4.1/codecarbon/core/api_client.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/cloud.py` & `codecarbon-2.4.1/codecarbon/core/cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/co2_signal.py` & `codecarbon-2.4.1/codecarbon/core/co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/config.py` & `codecarbon-2.4.1/codecarbon/core/config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/cpu.py` & `codecarbon-2.4.1/codecarbon/core/cpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
 class TDP:
     def __init__(self):
         self.model, self.tdp = self._main()
 
     @staticmethod
     def _get_cpu_constant_power(match: str, cpu_power_df: pd.DataFrame) -> int:
         """Extract constant power from matched CPU"""
-        return cpu_power_df[cpu_power_df["Name"] == match]["TDP"].values[0]
+        return float(cpu_power_df[cpu_power_df["Name"] == match]["TDP"].values[0])
 
     def _get_cpu_power_from_registry(self, cpu_model_raw: str) -> Optional[int]:
         cpu_power_df = DataSource().get_cpu_power_data()
         cpu_matching = self._get_matching_cpu(cpu_model_raw, cpu_power_df)
         if cpu_matching:
             power = self._get_cpu_constant_power(cpu_matching, cpu_power_df)
             return power
```

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/emissions.py` & `codecarbon-2.4.1/codecarbon/core/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/gpu.py` & `codecarbon-2.4.1/codecarbon/core/gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/measure.py` & `codecarbon-2.4.1/codecarbon/core/measure.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/powermetrics.py` & `codecarbon-2.4.1/codecarbon/core/powermetrics.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/rapl.py` & `codecarbon-2.4.1/codecarbon/core/rapl.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/schemas.py` & `codecarbon-2.4.1/codecarbon/core/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/units.py` & `codecarbon-2.4.1/codecarbon/core/units.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/core/util.py` & `codecarbon-2.4.1/codecarbon/core/util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/canada_provinces.geojson` & `codecarbon-2.4.1/codecarbon/data/canada_provinces.geojson`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/cloud/impact.csv` & `codecarbon-2.4.1/codecarbon/data/cloud/impact.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/2023-07-07-22-40-48.png` & `codecarbon-2.4.1/codecarbon/data/private_infra/2023-07-07-22-40-48.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/carbon_intensity_per_source.json` & `codecarbon-2.4.1/codecarbon/data/private_infra/carbon_intensity_per_source.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/global_energy_mix.json` & `codecarbon-2.4.1/codecarbon/data/private_infra/global_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/our_world_in_data-2022_data.ipynb` & `codecarbon-2.4.1/codecarbon/data/private_infra/our_world_in_data-2022_data.ipynb`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/world_energy_mix.csv` & `codecarbon-2.4.1/codecarbon/data/private_infra/world_energy_mix.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/2016/canada_energy_mix.json` & `codecarbon-2.4.1/codecarbon/data/private_infra/2016/canada_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/2016/global_energy_mix-old.json` & `codecarbon-2.4.1/codecarbon/data/private_infra/2016/global_energy_mix-old.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/2016/usa_emissions.json` & `codecarbon-2.4.1/codecarbon/data/private_infra/2016/usa_emissions.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/01_get_world_carbon_intensity.ipynb` & `codecarbon-2.4.1/codecarbon/data/private_infra/2020/01_get_world_carbon_intensity.ipynb`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/02_convert_csv_to_json.ipynb` & `codecarbon-2.4.1/codecarbon/data/private_infra/2020/02_convert_csv_to_json.ipynb`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/03_add_eu_data.ipynb` & `codecarbon-2.4.1/codecarbon/data/private_infra/2020/03_add_eu_data.ipynb`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/eu-carbon-intensity-electricity.csv` & `codecarbon-2.4.1/codecarbon/data/private_infra/2020/eu-carbon-intensity-electricity.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/external/geography.py` & `codecarbon-2.4.1/codecarbon/external/geography.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/external/hardware.py` & `codecarbon-2.4.1/codecarbon/external/hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/external/logger.py` & `codecarbon-2.4.1/codecarbon/external/logger.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/external/scheduler.py` & `codecarbon-2.4.1/codecarbon/external/scheduler.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/external/task.py` & `codecarbon-2.4.1/codecarbon/external/task.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/prometheus/metric_definitions.py` & `codecarbon-2.4.1/codecarbon/prometheus/metric_definitions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/prometheus/prometheus.py` & `codecarbon-2.4.1/codecarbon/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/viz/carbonboard.py` & `codecarbon-2.4.1/codecarbon/viz/carbonboard.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/viz/carbonboard_on_api.py` & `codecarbon-2.4.1/codecarbon/viz/carbonboard_on_api.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/viz/components.py` & `codecarbon-2.4.1/codecarbon/viz/components.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/viz/data.py` & `codecarbon-2.4.1/codecarbon/viz/data.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/viz/assets/car_icon.png` & `codecarbon-2.4.1/codecarbon/viz/assets/car_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/viz/assets/house_icon.png` & `codecarbon-2.4.1/codecarbon/viz/assets/house_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/codecarbon/viz/assets/tv_icon.png` & `codecarbon-2.4.1/codecarbon/viz/assets/tv_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/.gitignore` & `codecarbon-2.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/LICENSE` & `codecarbon-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/README.md` & `codecarbon-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.0rc0/pyproject.toml` & `codecarbon-2.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "codecarbon"
 dynamic = ["version"]
 readme = "README.md"
-license = ""
 requires-python = ">=3.7"
 authors = [
     { name = "Mila" },
     { name = "DataForGood" },
     { name = "BCG GAMMA" },
     { name = "Comet.ml" },
     { name = "Haverford College" },
@@ -33,14 +32,22 @@
     "psutil",
     "py-cpuinfo",
     "pynvml",
     "rapidfuzz",
     "requests",
 ]
 
+[project.urls]
+Homepage = "https://codecarbon.io/"
+Repository = "https://github.com/mlco2/codecarbon"
+Dashboard = "http://dashboard.codecarbon.io/"
+Documentation = "https://mlco2.github.io/codecarbon/"
+Issues = "https://github.com/mlco2/codecarbon/issues"
+Changelog = "https://github.com/mlco2/codecarbon/releases"
+
 [project.optional-dependencies]
 
 viz = [
     "dash",
     "dash_bootstrap_components < 1.0.0",
     "fire",
 ]
@@ -81,15 +88,15 @@
     "mypy",
 ]
 
 [tool.hatch.envs.dev.scripts]
 precommit-install = "pre-commit install"
 precommit-update = "pre-commit autoupdate"
 precommit = "pre-commit run --show-diff-on-failure --color=always --all-files"
-mypy = "mypy -m codecarbon --ignore-missing-imports --no-strict-optional --disable-error-code attr-defined --disable-error-code assignment --disable-error-code misc"
+mypy-check = "mypy -m codecarbon --ignore-missing-imports --no-strict-optional --disable-error-code attr-defined --disable-error-code assignment --disable-error-code misc"
 lint = ["black --check --diff {args:.}", "ruff check {args:.}", "mypy {args:.}"]
 format = ["black {args:.}", "ruff --fix --exit-non-zero-on-fix {args:.}"]
 
 [tool.hatch.envs.test]
 features = ["viz"]
 dependencies = [
    "mock",
```

### Comparing `codecarbon-2.4.0rc0/PKG-INFO` & `codecarbon-2.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Metadata-Version: 2.3
 Name: codecarbon
-Version: 2.4.0rc0
+Version: 2.4.1
+Project-URL: Homepage, https://codecarbon.io/
+Project-URL: Repository, https://github.com/mlco2/codecarbon
+Project-URL: Dashboard, http://dashboard.codecarbon.io/
+Project-URL: Documentation, https://mlco2.github.io/codecarbon/
+Project-URL: Issues, https://github.com/mlco2/codecarbon/issues
+Project-URL: Changelog, https://github.com/mlco2/codecarbon/releases
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

