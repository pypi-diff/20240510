# Comparing `tmp/sklearn_viz-0.5.0.tar.gz` & `tmp/sklearn_viz-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_viz-0.5.0.tar", max compression
+gzip compressed data, was "sklearn_viz-0.6.0.tar", max compression
```

## Comparing `sklearn_viz-0.5.0.tar` & `sklearn_viz-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1069 2024-05-08 12:37:45.071231 sklearn_viz-0.5.0/LICENSE
--rw-r--r--   0        0        0      354 2024-05-08 12:37:45.071231 sklearn_viz-0.5.0/README.md
--rw-r--r--   0        0        0      165 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/components/__init__.py
--rw-r--r--   0        0        0     4385 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/components/estimators.py
--rw-r--r--   0        0        0      811 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/components/kfold.py
--rw-r--r--   0        0        0      329 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/__init__.py
--rw-r--r--   0        0        0     8306 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/importance.py
--rw-r--r--   0        0        0     4633 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/outlier_detection.py
--rw-r--r--   0        0        0     2403 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/parallel_coordinates.py
--rw-r--r--   0        0        0    16590 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/principal_components.py
--rw-r--r--   0        0        0      643 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/scatter_matrix.py
--rw-r--r--   0        0        0      129 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/__init__.py
--rw-r--r--   0        0        0     6079 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/learning_curve.py
--rw-r--r--   0        0        0     1572 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/metrics.py
--rw-r--r--   0        0        0    21547 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/model_selection.py
--rw-r--r--   0        0        0     2497 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/models.py
--rw-r--r--   0        0        0      508 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/scorers.py
--rw-r--r--   0        0        0       21 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/residuals/__init__.py
--rw-r--r--   0        0        0     2058 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/residuals/error.py
--rw-r--r--   0        0        0       28 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/utils/__init__.py
--rw-r--r--   0        0        0      544 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/utils/file.py
--rw-r--r--   0        0        0     3033 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/utils/plotly.py
--rw-r--r--   0        0        0     3111 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/utils/timer.py
--rw-r--r--   0        0        0      978 2024-05-08 12:37:45.079231 sklearn_viz-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-10 13:31:23.533871 sklearn_viz-0.6.0/LICENSE
+-rw-r--r--   0        0        0      354 2024-05-10 13:31:23.533871 sklearn_viz-0.6.0/README.md
+-rw-r--r--   0        0        0      165 2024-05-10 13:31:23.533871 sklearn_viz-0.6.0/elphick/sklearn_viz/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:31:23.533871 sklearn_viz-0.6.0/elphick/sklearn_viz/components/__init__.py
+-rw-r--r--   0        0        0     5912 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/components/estimators.py
+-rw-r--r--   0        0        0      811 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/components/kfold.py
+-rw-r--r--   0        0        0      329 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/__init__.py
+-rw-r--r--   0        0        0     8306 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/importance.py
+-rw-r--r--   0        0        0     4633 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/outlier_detection.py
+-rw-r--r--   0        0        0     2403 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/parallel_coordinates.py
+-rw-r--r--   0        0        0    16590 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/principal_components.py
+-rw-r--r--   0        0        0      643 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/scatter_matrix.py
+-rw-r--r--   0        0        0      129 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/__init__.py
+-rw-r--r--   0        0        0    11404 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/cross_validation.py
+-rw-r--r--   0        0        0     6079 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/learning_curve.py
+-rw-r--r--   0        0        0     1572 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/metrics.py
+-rw-r--r--   0        0        0    13278 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/model_selection.py
+-rw-r--r--   0        0        0     2497 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/models.py
+-rw-r--r--   0        0        0      508 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/scorers.py
+-rw-r--r--   0        0        0       21 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/residuals/__init__.py
+-rw-r--r--   0        0        0     2058 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/residuals/error.py
+-rw-r--r--   0        0        0       28 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/utils/__init__.py
+-rw-r--r--   0        0        0      544 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/utils/file.py
+-rw-r--r--   0        0        0     3033 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/utils/plotly.py
+-rw-r--r--   0        0        0     3111 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/utils/timer.py
+-rw-r--r--   0        0        0      977 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 sklearn_viz-0.6.0/PKG-INFO
```

### Comparing `sklearn_viz-0.5.0/LICENSE` & `sklearn_viz-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/components/estimators.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/components/estimators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,37 @@
+from abc import ABC
+
 import numpy as np
 import pandas as pd
-from sklearn.base import RegressorMixin, BaseEstimator
+from sklearn.base import RegressorMixin, BaseEstimator, ClassifierMixin
 from sklearn.exceptions import NotFittedError
 from sklearn.utils._estimator_html_repr import _VisualBlock
 from sklearn.utils.validation import check_is_fitted
+from typing import Union, Optional
 
 
-class PartitionRegressor(RegressorMixin, BaseEstimator):
-    """Prediction for partitioned subsets of records (estimation domains) defined by filter criteria.
-
-    A PartitionRegressor is designed to allow multiple models to be fitted on a subset of records defined by
-     a criteria applied to the input features.  So in essence the criteria definitions define estimation domains
-    (a.k.a. partitions) for individual model fitting.
-    """
-
+# noinspection PyAttributeOutsideInit
+class PartitionEstimatorBase(BaseEstimator, ABC):
     def __init__(self, estimator, *, partition_defs: dict[str, str], n_jobs=None, verbose=False):
-        super(RegressorMixin).__init__()
-        super(BaseEstimator).__init__()
+        super().__init__()
 
         self.n_jobs = n_jobs
         self.verbose = verbose
         self.estimator = estimator
 
         self.estimators: list[tuple] = [(k, estimator) for k in partition_defs.keys()]
         self.partition_defs = partition_defs
 
         # set post fitting
         self.x_train_: pd.DataFrame
         self.y_train_: pd.DataFrame
         self.domain_indexes_: dict
         self.feature_names_in_: list
 
-    def score(self, X, y, sample_weight=None):
-        pass
-
-    def fit(self, X: pd.DataFrame, y: [pd.DataFrame, None] = None) -> 'PartitionRegressor':
+    def fit(self, X: pd.DataFrame, y: Union[pd.DataFrame, None] = None):
         # fit the estimators only on the appropriate records
         self.x_train_ = X
         self.y_train_ = y if isinstance(y, pd.DataFrame) else y.to_frame()
         domain_indexes: dict = dict()
         domains: pd.Series = pd.Series(np.nan, index=X.index, name='domains')
         for domain, criteria in self.partition_defs.items():
             mdl = [est[1] for est in self.estimators if est[0] == domain][0]
@@ -68,17 +61,20 @@
             else:
                 # this model had no data to fit on, so return nans
                 chunks.append(pd.DataFrame(np.nan, index=xf.index, columns=self.y_train_.columns).assign(domain=domain))
         res: pd.DataFrame = pd.merge(left=pd.Series(X.index, index=X.index, name='dummy'),
                                      right=pd.concat(chunks, axis=0),
                                      left_index=True, right_index=True,
                                      how='left', ).drop(columns=['dummy', 'domain'])
-        # res['domain'] = res['domain'].astype('category')
         return res
 
+    def score(self, X, y, sample_weight=None):
+        # implementation goes here
+        pass
+
     @property
     def n_features_in_(self):
         """Number of features seen during :term:`fit`."""
         # For consistency with other estimators we raise a AttributeError so
         # that hasattr() fails if the estimator isn't fitted.
         try:
             check_is_fitted(self)
@@ -91,7 +87,49 @@
 
         return self.estimators_[0].n_features_in_
 
     def _sk_visual_block_(self):
         names, estimators = zip(*self.estimators)
         criteria = list(self.partition_defs.values())
         return _VisualBlock("parallel", estimators, names=names, name_details=criteria)
+
+
+class PartitionRegressor(PartitionEstimatorBase, RegressorMixin):
+    """Prediction for partitioned subsets of records (estimation domains) defined by filter criteria.
+
+    A PartitionRegressor is designed to allow multiple models to be fitted on a subset of records defined by
+     a criteria applied to the input features.  So in essence the criteria definitions define estimation domains
+    (a.k.a. partitions) for individual model fitting.
+    """
+
+    def __init__(self, estimator, *, partition_defs: dict[str, str], n_jobs=None, verbose=False):
+        super().__init__(estimator, partition_defs=partition_defs, n_jobs=n_jobs, verbose=verbose)
+        # set scorer for regression
+        self.scorer_ = 'r2'
+
+    def fit(self, X: pd.DataFrame, y: Optional[pd.DataFrame] = None) -> 'PartitionRegressor':
+        super().fit(X, y)
+        return self
+
+    def predict(self, X: pd.DataFrame) -> pd.DataFrame:
+        return super().predict(X)
+
+
+class PartitionClassifier(PartitionEstimatorBase, ClassifierMixin):
+    """Prediction for partitioned subsets of records (estimation domains) defined by filter criteria.
+
+    A PartitionClassifier is designed to allow multiple models to be fitted on a subset of records defined by
+     a criteria applied to the input features.  So in essence the criteria definitions define estimation domains
+    (a.k.a. partitions) for individual model fitting.
+    """
+
+    def __init__(self, estimator, *, partition_defs: dict[str, str], n_jobs=None, verbose=False):
+        super().__init__(estimator, partition_defs=partition_defs, n_jobs=n_jobs, verbose=verbose)
+        # set scorer for regression
+        self.scorer_ = 'accuracy'
+
+    def fit(self, X: pd.DataFrame, y: Optional[pd.DataFrame] = None) -> 'PartitionClassifier':
+        super().fit(X, y)
+        return self
+
+    def predict(self, X: pd.DataFrame) -> pd.DataFrame:
+        return super().predict(X)
```

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/components/kfold.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/components/kfold.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/features/importance.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/features/importance.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/features/outlier_detection.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/features/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/features/parallel_coordinates.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/features/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/features/principal_components.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/features/principal_components.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/features/scatter_matrix.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/features/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/learning_curve.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/learning_curve.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/metrics.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/metrics.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/model_selection.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/model_selection.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,154 +4,81 @@
 import matplotlib
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 import sklearn
 from plotly import colors
 from plotly.subplots import make_subplots
-from sklearn import model_selection
-from sklearn.base import is_classifier, is_regressor
-from sklearn.model_selection import cross_validate
+from sklearn.base import BaseEstimator
 from sklearn.pipeline import Pipeline
 
-from elphick.sklearn_viz.model_selection.metrics import regression_metrics, classification_metrics
-from elphick.sklearn_viz.model_selection.scorers import classification_scorers, regression_scorers
+from elphick.sklearn_viz.model_selection.cross_validation import CrossValidatorBase
 
 
 def subplot_index(idx: int, col_wrap: int) -> Tuple[int, int]:
     col: int = int(idx % col_wrap + 1)
     row: int = int(np.floor(idx / col_wrap) + 1)
     return row, col
 
 
-def plot_model_selection(algorithms: Union[sklearn.base.RegressorMixin, sklearn.base.ClassifierMixin, Dict],
+def plot_model_selection(estimators: Union[sklearn.base.RegressorMixin, sklearn.base.ClassifierMixin, Dict],
                          datasets: Union[pd.DataFrame, Dict],
                          target: str,
                          pre_processor: Optional[Pipeline] = None,
                          k_folds: int = 10,
                          title: Optional[str] = None) -> go.Figure:
     """
 
     Args:
-            algorithms: sklearn estimator or a Dict of algorithms to cross-validate, keyed by string name/code.
+            estimators: sklearn estimator or a Dict of algorithms to cross-validate, keyed by string name/code.
             datasets: pandas DataFrame or a dict of DataFrames, keyed by string name/code.
             target: target column
             pre_processor: Optional pipeline used to pre-process the datasets.
             k_folds: The number of cross validation folds.
             title: Optional plot title
 
     Returns:
         a plotly GraphObjects.Figure
 
     """
 
-    return ModelSelection(algorithms=algorithms, datasets=datasets, target=target, pre_processor=pre_processor,
+    return ModelSelection(estimators=estimators, datasets=datasets, target=target, pre_processor=pre_processor,
                           k_folds=k_folds).plot(title=title)
 
 
-class ModelSelection:
+class ModelSelection(CrossValidatorBase):
     def __init__(self,
-                 algorithms: Union[
-                     sklearn.base.RegressorMixin, sklearn.base.ClassifierMixin, Dict[str, sklearn.base.BaseEstimator]],
+                 estimators: Union[BaseEstimator, Dict[str, BaseEstimator]],
                  datasets: Union[pd.DataFrame, Dict[str, pd.DataFrame]],
                  target: str,
                  pre_processor: Optional[Pipeline] = None,
                  k_folds: int = 10,
                  scorer: Optional[Union[str, Callable]] = None,
                  metrics: Optional[Dict[str, Callable]] = None,
                  group: Optional[pd.Series] = None,
                  random_state: Optional[int] = None):
         """
 
         Args:
-            algorithms: sklearn estimator or a Dict of algorithms to cross-validate, keyed by string name/code.
+            estimators: sklearn estimator or a Dict of algorithms to cross-validate, keyed by string name/code.
             datasets: pandas DataFrame or a dict of DataFrames, keyed by string name/code.
             target: target column
             pre_processor: Optional pipeline used to pre-process the datasets.
             k_folds: The number of cross validation folds.
             scorer: Optional callable scorers which the model will be fitted using
             metrics: Optional Dict of callable metrics to calculate post-fitting
             group: Optional group variable by which to partition/group metrics.  The same group applies across all
              datasets, so is more useful when testing different algorithms.
             random_state: Optional random seed
         """
-        self._logger = logging.getLogger(name=__class__.__name__)
-        self.pre_processor: Pipeline = pre_processor
-        if isinstance(algorithms, sklearn.base.BaseEstimator):
-            self.algorithms = {algorithms.__class__.__name__: algorithms}
-        else:
-            self.algorithms = algorithms
-        if isinstance(datasets, pd.DataFrame):
-            self.datasets = {'Dataset': datasets}
-        else:
-            self.datasets = datasets
-        self.target = target
-        self.k_folds: int = k_folds
-
-        self.is_classifier: bool = is_classifier(list(self.algorithms.values())[0])
-        self.is_regressor: bool = is_regressor(list(self.algorithms.values())[0])
-        if scorer is not None:
-            self.scorer = scorer
-        else:
-            self.scorer = classification_scorers[list(classification_scorers.keys())[0]] if self.is_classifier else \
-                regression_scorers[list(regression_scorers.keys())[0]]
-
-        if metrics is not None:
-            self.metrics = metrics
-        else:
-            self.metrics = classification_metrics if self.is_classifier else regression_metrics
-
-        self.group: pd.Series = group
-        self.random_state: Optional[int] = random_state
-
-        self.features_in: List[str] = [col for col in self.datasets[list(self.datasets.keys())[0]] if
-                                       col != self.target]
 
-        self._data: Optional[Dict] = None
-        self._num_algorithms: int = len(list(self.algorithms.keys()))
-        self._num_datasets: int = len(list(self.datasets.keys()))
-
-        if self._num_algorithms > 1 and self._num_datasets > 1:
-            raise NotImplementedError("Cannot have multiple algorithms and multiple datasets.")
-
-    @property
-    def data(self) -> Optional[Dict]:
-        if self.metrics is None:
-            cv_kwargs: Dict = dict()
-        else:
-            cv_kwargs: Dict = dict(return_estimator=True, return_indices=True, error_score=np.nan)
-
-        if self._data is not None:
-            results = self._data
-        else:
-            results: Dict = {}
-            for data_key, data in self.datasets.items():
-                self._logger.info(f"Commencing Cross Validation for dataset {data_key}")
-                results[data_key] = {}
-                x: pd.DataFrame = data[self.features_in]
-                y: pd.DataFrame = data[self.target]
-                if self.pre_processor:
-                    x = self.pre_processor.set_output(transform="pandas").fit_transform(X=x)
-
-                for algo_key, algo in self.algorithms.items():
-                    kfold = model_selection.KFold(n_splits=self.k_folds, random_state=self.random_state, shuffle=True)
-                    res = cross_validate(algo, x, y, cv=kfold, scoring=self.scorer, **cv_kwargs)
-                    if self.metrics is not None:
-                        res['metrics'], res['metrics_group'] = self.calculate_metrics(x=x, y=y,
-                                                                                      estimators=res['estimator'],
-                                                                                      indices=res['indices'],
-                                                                                      group=self.group)
-                    results[data_key][algo_key] = res
-                    res_mean = res[f"test_score"].mean()
-                    res_std = res[f"test_score"].std()
-                    self._logger.info(f"CV Results for {algo_key}: Mean = {res_mean}, SD = {res_std}")
-
-            self._data = results
+        self._logger = logging.getLogger(name=__class__.__name__)
 
-        return results
+        super().__init__(estimators=estimators, datasets=datasets, target=target, pre_processor=pre_processor,
+                         cv=k_folds, scorer=scorer, metrics=metrics, group=group, random_state=random_state)
 
     def plot(self,
              metrics: Optional[Union[str, List[str]]] = None,
              show_group: bool = False,
              title: Optional[str] = None,
              col_wrap: Optional[int] = None) -> go.Figure:
         """Create the plot
@@ -172,14 +99,15 @@
              col-wrap columns, and multiple rows.
 
         Returns:
             a plotly GraphObjects.Figure
 
         """
 
+        # Access the attributes of the CrossValidationResult dataclass
         data: pd.DataFrame = self.get_cv_scores()
         data = data.droplevel(level=0, axis=1) if self._num_datasets == 1 else data.droplevel(level=1, axis=1)
 
         metric_data: pd.DataFrame = pd.DataFrame()
 
         if metrics is not None:
             if isinstance(metrics, str):
@@ -194,15 +122,15 @@
             x_index = 'data_key'
 
         # define the color map for the scorer
         vmin, vmax = data.min().min(), data.max().max()
         norm = matplotlib.colors.Normalize(vmin=vmin, vmax=vmax)
         cmap = matplotlib.cm.get_cmap('RdYlGn')
 
-        subtitle: str = f'Cross Validation folds={self.k_folds}'
+        subtitle: str = f'Cross Validation folds={str(self.cv)}'
         if title is None:
             title = subtitle
         else:
             title = title + '<br>' + subtitle
 
         # create the plot, managing the shape.
         num_plots: int = len(metrics) + 1 if len(metrics) > 0 else 1
@@ -267,15 +195,15 @@
             col_wrap: If plotting multiple metrics, col_wrap will wrap columns to new rows, resulting in
              col-wrap columns, and multiple rows.
 
         Returns:
             a plotly GraphObjects.Figure
 
         """
-        algorithms: list[str] = list(self.algorithms.keys())
+        algorithms: list[str] = list(self.estimators.keys())
         algorithm: str = algorithms[0] if algorithm is None else algorithm
         if algorithm not in algorithms:
             raise KeyError(f"Algorithm {algorithm} is not in the list of available algorithms: {algorithms}")
 
         datasets: list[str] = list(self.datasets.keys())
         dataset: str = datasets[0] if dataset is None else dataset
         if dataset not in datasets:
@@ -295,15 +223,15 @@
                                                  ignore_index=False).assign(model='by_group')
         metric_data: pd.DataFrame = pd.concat([baseline_metrics, by_group_metrics]).sort_values(['model', 'metric'])
         metric_data = metric_data.set_index(['metric', 'group'], append=True).pivot(columns='model',
                                                                                     values='value').reset_index(
             'metric')
 
         if title is None:
-            title = f'Model by Group Test on {algorithm} with {self.k_folds} folds'
+            title = f'Model by Group Test on {algorithm} with cv = {str(self.cv)}'
 
         num_plots: int = len(metrics) if len(metrics) > 0 else 1
         num_cols: int = num_plots if col_wrap is None else col_wrap
         num_rows, _ = subplot_index(len(metrics) - 1, col_wrap=num_cols)
         fig = make_subplots(rows=num_rows, cols=num_cols,
                             subplot_titles=metrics)
 
@@ -324,98 +252,18 @@
         fig.update_layout(title=title, showlegend=False)
         fig.update_layout(boxmode='group', showlegend=True, legend_title='model',
                           boxgroupgap=0.5, boxgap=0
                           )
 
         return fig
 
-    def get_model_by_group_data(self, algorithm, dataset):
-        results: dict = {}
-        by_group_score_chunks: list = []
-        by_group_metric_chunks: list = []
-        for grp in self.group.unique():
-            grp_index: pd.Index = self.group.loc[self.group == grp].index
-            x: pd.DataFrame = self.datasets[dataset][self.features_in].loc[grp_index]
-            y: pd.DataFrame = self.datasets[dataset][self.target].loc[grp_index]
-            if self.pre_processor:
-                x = self.pre_processor.set_output(transform="pandas").fit_transform(X=x)
-            kfold = model_selection.KFold(n_splits=self.k_folds, random_state=self.random_state, shuffle=True)
-            res = cross_validate(self.algorithms[algorithm], x, y, cv=kfold, scoring=self.scorer, return_estimator=True,
-                                 return_indices=True)
-            by_group_score_chunks.append(pd.Series(res['test_score'], name=grp))
-            if self.metrics is not None:
-                res['metrics'], _ = self.calculate_metrics(x=x, y=y,
-                                                           estimators=res['estimator'],
-                                                           indices=res['indices'],
-                                                           group=None)
-            results[grp] = res
-            by_group_metric_chunks.append(
-                pd.DataFrame(res['metrics']).assign(group=grp).rename_axis('fold', axis='index'))
-        by_group_metrics: pd.DataFrame = pd.concat(by_group_metric_chunks)
-        #                                   .reset_index().melt(id_vars=['fold', 'group'],
-        #                                                                                       value_vars=list(
-        #                                                                                           self.metrics.keys()),
-        #                                                                                       var_name='metric'))
-        # by_group_metrics = by_group_metrics.set_index(['fold', 'metric', 'group']).unstack(level=-1)
-        # by_group_metrics = by_group_metrics.droplevel(level=0, axis=1).reset_index(-1)
-        by_group_scores = pd.concat(by_group_score_chunks, axis=1)
-
-        return by_group_metrics, by_group_scores
+    def get_model_by_group_data(self, estimator, dataset) -> tuple[pd.DataFrame, pd.DataFrame]:
+        return super().get_model_by_group_data(estimator, dataset)
 
     def get_cv_scores(self) -> pd.DataFrame:
-        chunks: List = []
-        for data_key, data in self.datasets.items():
-            for algo_key, algo in self.algorithms.items():
-                chunks.append(pd.Series(self.data[data_key][algo_key][f"test_score"], name=(data_key, algo_key)))
-        return pd.concat(chunks, axis=1)
+        return super().get_cv_scores()
 
     def get_cv_metrics(self, metrics, by_group: bool = False) -> pd.DataFrame:
-        chunks: List = []
-        metric_key = "metrics_group" if by_group else "metrics"
-        for data_key, data in self.datasets.items():
-            for algo_key, algo in self.algorithms.items():
-                for metric in metrics:
-                    chunks.append(pd.DataFrame(self.data[data_key][algo_key][metric_key][metric]).assign(
-                        **dict(data_key=data_key, algo_key=algo_key, metric=metric)))
-        res: pd.DataFrame = pd.concat(chunks, axis=0).set_index(['data_key', 'algo_key'], append=True).rename(
-            columns={0: 'value'})
-        res.index.names = ['fold', 'data_key', 'algo_key']
-        return res
+        return super().get_cv_metrics(metrics, by_group)
 
     def calculate_metrics(self, x, y, estimators, indices, group) -> Tuple[Dict, Dict]:
-        metric_results: Dict = {}
-        metric_results_group: Dict = {}
-
-        for k, fn_metric in self.metrics.items():
-            metric_values: List = []
-            metric_groups: Dict = {}
-            for estimator, test_indexes in zip(estimators, indices['test']):
-                y_true = y[y.index[test_indexes]]
-                y_est = estimator.predict(x.loc[x.index[test_indexes], :])
-                if isinstance(y_est, pd.DataFrame) and y_est.shape[1] == 1:
-                    y_est = y_est.iloc[:, 0]
-                metric_values.append(fn_metric(y_true, y_est))
-                if group is not None:
-                    # calculate the metric by each group in the group series.
-                    y_est = pd.merge(left=pd.Series(y_est, name='y_est', index=x.index[test_indexes]),
-                                     right=group, left_index=True, right_index=True)
-                    y_est_grouped = y_est.groupby([group.name])
-                    grouped_results = [y_est_grouped.get_group(x) for x in y_est_grouped.groups]
-                    for grp_res in grouped_results:
-                        group_value = str(grp_res[group.name].iloc[0])
-                        group_metric_results = fn_metric(y_true[grp_res.index], grp_res['y_est'].values)
-                        if group_value not in metric_groups.keys():
-                            metric_groups[group_value] = [group_metric_results]
-                        else:
-                            metric_groups[group_value].append(group_metric_results)
-            metric_results[k] = metric_values
-            if group is not None:
-                metric_results_group[k] = metric_groups
-
-        return metric_results, metric_results_group
-
-# if __name__ == '__main__':
-#
-#     for i in range(0, 7):
-#         print(subplot_index(i, col_wrap=3))
-#
-#     print('done')
+        return super().calculate_metrics(x, y, estimators, indices, group)
```

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/models.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/models.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/residuals/error.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/residuals/error.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/utils/file.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/utils/file.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/utils/plotly.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/utils/plotly.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/elphick/sklearn_viz/utils/timer.py` & `sklearn_viz-0.6.0/elphick/sklearn_viz/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.5.0/pyproject.toml` & `sklearn_viz-0.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sklearn-viz"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Greg <11791585+elphick@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "elphick/sklearn_viz" }]
 
 [[tool.poetry.source]]
 name = "PyPI"
@@ -16,18 +16,18 @@
 [tool.towncrier]
 package = "elphick.sklearn_viz"
 package_dir = "elphick/sklearn_viz"
 filename = "HISTORY.rst"
 directory = "towncrier/newsfragments"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.12"
 scikit-learn = ">=1.2.0"
 pandas = ">=1.3.0"
-matplotlib = "^3.7.2"
+matplotlib = ">=3.3"
 plotly = "^5.15.0"
 statsmodels = "^0.14.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `sklearn_viz-0.5.0/PKG-INFO` & `sklearn_viz-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: sklearn-viz
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Greg
 Author-email: 11791585+elphick@users.noreply.github.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
+Requires-Dist: matplotlib (>=3.3)
 Requires-Dist: pandas (>=1.3.0)
 Requires-Dist: plotly (>=5.15.0,<6.0.0)
 Requires-Dist: scikit-learn (>=1.2.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # sklearn-viz
```

