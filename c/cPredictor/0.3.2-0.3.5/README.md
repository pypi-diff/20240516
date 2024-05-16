# Comparing `tmp/cPredictor-0.3.2-py3-none-any.whl.zip` & `tmp/cPredictor-0.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20111 bytes, number of entries: 11
--rw-r--r--  2.0 unx    42101 b- defN 24-Apr-17 06:36 cPredictor/SVM_prediction.py
--rw-r--r--  2.0 unx      354 b- defN 24-Apr-17 06:36 cPredictor/__init__.py
--rw-r--r--  2.0 unx     6922 b- defN 24-Apr-17 06:36 cPredictor/tests/SVM_prediction_test.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 06:36 cPredictor/tests/__init__.py
--rw-r--r--  2.0 unx     2398 b- defN 24-Apr-17 06:36 cPredictor/tests/cPredictor_test_model.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3349 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      227 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      941 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/RECORD
-11 files, 67752 bytes uncompressed, 18503 bytes compressed:  72.7%
+Zip file size: 22411 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    43185 b- defN 24-May-16 08:09 cPredictor/SVM_prediction.py
+-rw-r--r--  2.0 unx      354 b- defN 24-May-16 08:09 cPredictor/__init__.py
+-rw-r--r--  2.0 unx     6922 b- defN 24-May-16 08:09 cPredictor/tests/SVM_prediction_test.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 08:09 cPredictor/tests/__init__.py
+-rw-r--r--  2.0 unx     8174 b- defN 24-May-16 08:09 cPredictor/tests/cPredictor_test_model.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3361 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      227 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      941 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/RECORD
+11 files, 74624 bytes uncompressed, 20803 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: cPredictor/tests/__init__.py
 Comment: 
 
 Filename: cPredictor/tests/cPredictor_test_model.py
 Comment: 
 
-Filename: cPredictor-0.3.2.dist-info/LICENSE
+Filename: cPredictor-0.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: cPredictor-0.3.2.dist-info/METADATA
+Filename: cPredictor-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: cPredictor-0.3.2.dist-info/WHEEL
+Filename: cPredictor-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: cPredictor-0.3.2.dist-info/entry_points.txt
+Filename: cPredictor-0.3.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: cPredictor-0.3.2.dist-info/top_level.txt
+Filename: cPredictor-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: cPredictor-0.3.2.dist-info/RECORD
+Filename: cPredictor-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cPredictor/SVM_prediction.py

```diff
@@ -21,24 +21,25 @@
 from sklearn.model_selection import StratifiedKFold
 from sklearn.model_selection import KFold
 from sklearn.preprocessing import LabelEncoder
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.metrics import f1_score
 from sklearn.metrics import accuracy_score
 from sklearn.metrics import precision_score
+from sklearn.metrics import classification_report
 from sklearn.svm import LinearSVC
 import logging
 import pickle
 import joblib
 import json
 
 class CpredictorClassifier():
     def __init__(self, Threshold_rej, rejected, OutputDir):
         self.scaler = MinMaxScaler()
-        self.Classifier = LinearSVC(dual = False, random_state = 42, class_weight = 'balanced', max_iter = 2500)
+        self.Classifier = LinearSVC(C = 0.01, dual = False, random_state = 42, class_weight = 'balanced', max_iter = 1000)
         self.threshold = Threshold_rej
         self.rejected = rejected
         self.output_dir = OutputDir
         self.expression_treshold = 162
         self.kf = StratifiedKFold(n_splits = 3, shuffle = True, random_state = 42)
 
     def expression_cutoff(self, Data, LabelsPath):
@@ -321,26 +322,27 @@
         cpredictor.save_results(rejected)
         
     else:
         cpredictor.fit_and_predict_svm(labels_train, OutputDir, data_train, data_test)
         cpredictor.save_results(rejected)
 
 
-def SVM_import(query_H5AD, OutputDir, SVM_type, replicates, colord=None, meta_atlas=False, show_bar=False):
+def SVM_import(query_H5AD, OutputDir, SVM_type, replicates, sub_rep=None, colord=None, meta_atlas=False, show_bar=False):
     '''
     Imports the output of the SVM_predictor and saves it to the query_H5AD.
 
     Parameters:
     query_H5AD: H5AD file of datasets of interest.
     OutputDir: Output directory defining the path of the exported SVM_predictions.
     SVM_type: Type of SVM prediction, SVM (default) or SVMrej.
     Replicates: A string value specifying a column in query_H5AD.obs.
     colord: A .tsv file with the order of the meta_atlas and corresponding colors.
     meta_atlas : If the flag is added the predictions will use meta_atlas data.
     show_bar: Shows bar plots depending on the SVM_type, split over replicates.
+    sub_rep:  A string value specifying an instance within the selected column in query_H5AD.obs.
 
     '''
     logging.basicConfig(level=logging.DEBUG, 
                         format='%(asctime)s - %(name)s - %(levelname)s - %(message)s', datefmt='%d/%m/%Y %H:%M:%S',
                         filename='cPredictor_import.log', filemode='w')
     logging.info('Reading query data')
 
@@ -469,14 +471,18 @@
     if SVM_key == "SVM_predicted":
         logging.info('Plotting label prediction certainty scores')
         category_colors = category_colors
 
         # Create a figure and axes
         fig, ax = plt.subplots(1,1)
 
+        # This allows for subsetting the density plot to individual instances of the replicates column
+        if sub_rep is not None:
+            adata = adata[adata.obs[replicates] == str(sub_rep)] # Add funcitonal test here later
+            
         # Iterate over each category and plot the density
         for category, color in category_colors.items():
             subset = adata.obs[adata.obs['SVM_predicted'] == category]
             sns.kdeplot(data=subset['SVMrej_predicted_prob'], fill=True, color=color, label=f"{category} (Median: {subset['SVMrej_predicted_prob'].median():.2f})", ax=ax)
 
         # Set labels and title
         plt.xlabel('SVM Certainty Scores')
@@ -518,15 +524,15 @@
     Data = read_h5ad(reference_H5AD)
 
     # Using the child class of the CpredictorClassifier to process the data
     cpredictorperf = CpredictorClassifierPerformance(Threshold_rej, rejected, OutputDir)
     
     Data = cpredictorperf.expression_cutoff(Data, LabelsPath)
 
-    data_train = pd.DataFrame.sparse.from_spmatrix(Data.X, index=list(Data.obs.index.values), columns=list(Data.var.index.values))
+    data_train = pd.DataFrame.sparse.from_spmatrix(Data.X, index=list(Data.obs.index.values), columns=list(Data.var.features.values))
     data_train = data_train.to_numpy(dtype="float16")
     
     data_train = cpredictorperf.preprocess_data_train(data_train)
     data_train_processed = data_train
     
     # Do label encoding
     labels = pd.read_csv(LabelsPath, header=0,index_col=None, sep=',') #, usecols = col
@@ -643,14 +649,27 @@
     cnf_matrix = cnf_matrix.sort_index(axis=1)
     cnf_matrix = cnf_matrix.sort_index()
 
     # Plot png
     sns.set_theme(font_scale=0.8)
     cm = sns.clustermap(cnf_matrix.T, cmap="Blues", annot=True,fmt='.2%', row_cluster=False,col_cluster=False)
     cm.savefig(f"{OutputDir}/figures/{SVM_type}_cnf_matrix.png")
+
+    # Save classification report
+    report =classification_report(true, pred, output_dict=True)
+    df_classification_report = pd.DataFrame(report).transpose()
+    df_classification_report = df_classification_report.sort_values(by=['f1-score'], ascending=False)
+    df_classification_report.to_csv(f"{OutputDir}report.tsv", index=True, sep="\t")
+
+    with open(f"{OutputDir}/metrics.txt", "w") as text_file:
+        text_file.write(str(F1score)+"\n")
+        text_file.write(str(acc_score)+"\n")
+        text_file.write(str(prec_score)+"\n")
+        text_file.close()
+    
     return F1score,acc_score,prec_score
 
 def SVM_pseudobulk(condition_1, condition_1_batch, condition_2, condition_2_batch, Labels_1, OutputDir="pseudobulk_output/", min_cells=50, SVM_type="SVM"):
     '''
     Produces pseudobulk RNA-seq count files and sample files of either technical or biological replicates.
     It produces pseudobulk of all labels from LabelsPath against predicted labels after SVMprediction.
     Moreover, it produces overall pseudobulk of condition_1 vs condition_2 split by indicated batches.
@@ -898,25 +917,27 @@
 def importpars():
 
     parser = argparse.ArgumentParser(description="Imports predicted results back to H5AD file")
     parser.add_argument("--query_H5AD", type=str, help="Path to query H5AD file")
     parser.add_argument("--OutputDir", type=str, help="Output directory path")
     parser.add_argument("--SVM_type", type=str, help="Type of SVM prediction (SVM or SVMrej)")
     parser.add_argument("--replicates", type=str, help="Replicates")
+    parser.add_argument("--sub_rep", type=str, help="Replicates")
     parser.add_argument("--colord", type=str, help=".tsv file with meta-atlas order and colors")
     parser.add_argument("--meta_atlas", dest="meta_atlas", action="store_true", help="Use meta-atlas data")
     parser.add_argument("--show_bar", dest="show_bar", action="store_true", help="Plot barplot with SVM labels over specified replicates")
 
     args = parser.parse_args()
 
     SVM_import(
         args.query_H5AD,
         args.OutputDir,
         args.SVM_type,
         args.replicates,
+        args.sub_rep,
         args.colord,
         args.meta_atlas,
         args.show_bar)
     
 
 def pseudopars():
```

## cPredictor/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.2"
+__version__ = "0.3.5"
 
 from .SVM_prediction import SVM_predict
 from .SVM_prediction import SVM_import
 from .SVM_prediction import SVM_performance
 from .SVM_prediction import SVM_pseudobulk
 from .SVM_prediction import predpars
 from .SVM_prediction import importpars
```

## cPredictor/tests/cPredictor_test_model.py

```diff
@@ -1,40 +1,186 @@
 # Import modules
 import argparse
+import gc
 import os
 import numpy as np
 import pandas as pd
-import scanpy as sc
+import pyarrow as pa
+import scanpy
 import time as tm
 import seaborn as sns
 import matplotlib
 import matplotlib.pyplot as plt
+import matplotlib.gridspec as gridspec
 from sklearn.svm import LinearSVC
-from sklearn.calibration import CalibratedClassifierCV
+from sklearn.calibration import (CalibratedClassifierCV, calibration_curve, CalibrationDisplay)
 from sklearn.metrics import confusion_matrix
-from sklearn.model_selection import KFold
-from sklearn.preprocessing import LabelEncoder
-from sklearn.preprocessing import MinMaxScaler
-from sklearn.metrics import f1_score
-from sklearn.metrics import accuracy_score
-from sklearn.metrics import precision_score
-from scanpy import read_h5ad
+from sklearn.model_selection import (train_test_split, StratifiedKFold, KFold)
+from sklearn.preprocessing import (LabelEncoder, MinMaxScaler)
+from sklearn.metrics import (confusion_matrix, f1_score, accuracy_score, precision_score)
+import logging
+import pickle
+import joblib
+import json
 from importlib.resources import files
+from scanpy import read_h5ad
+import subprocess
+
+# Importing custom functions/modules if any
+from cPredictor.SVM_prediction import (CpredictorClassifier,CpredictorClassifierPerformance)
+
+# Add module and check if it works, if it does work, move it to processing scripts
+class NaivelyCalibratedLinearSVC(LinearSVC):
+    """LinearSVC with `predict_proba` method that naively scales
+    `decision_function` output for binary classification."""
+
+    def fit(self, X, y):
+        super().fit(X, y)
+        df = self.decision_function(X)
+        self.df_min_ = df.min()
+        self.df_max_ = df.max()
+
+    def predict_proba(self, X):
+        """Min-max scale output of `decision_function` to [0, 1]."""
+        df = self.decision_function(X)
+        calibrated_df = (df - self.df_min_) / (self.df_max_ - self.df_min_)
+        proba_pos_class = np.clip(calibrated_df, 0, 1)
+        proba_neg_class = 1 - proba_pos_class
+        proba = np.c_[proba_neg_class, proba_pos_class]
+        return proba
+
+def SVM_calibration(reference_H5AD, LabelsPath, OutputDir, rejected=True, Threshold_rej=0.7):
+    '''
+    Tests performance of SVM model based on a reference H5AD dataset.
+
+    Parameters:
+    reference_H5AD : H5AD file of datasets of interest.
+    OutputDir : Output directory defining the path of the exported SVM_predictions.
+    SVM_type: Type of SVM prediction, SVM or SVMrej (default).
+    '''
+    logging.basicConfig(level=logging.DEBUG, 
+                        format='%(asctime)s - %(name)s - %(levelname)s - %(message)s', datefmt='%d/%m/%Y %H:%M:%S',
+                        filename='cPredictor_performance.log', filemode='w')
+
+    # Using the child class of the CpredictorClassifier to process the data
+    cpredictorperf = CpredictorClassifierPerformance(Threshold_rej, rejected, OutputDir)
+
+    svc = NaivelyCalibratedLinearSVC(max_iter=10_000, dual="auto")
+    svc_isotonic = CalibratedClassifierCV(svc, cv=3, method="isotonic")
+    svc_sigmoid = CalibratedClassifierCV(svc, cv=3, method="sigmoid")
+
+    # Setup cpredictors params from its class
+    kf = StratifiedKFold(n_splits = 3, shuffle = True, random_state = 42)
+    cpredictormodel = getattr(cpredictorperf,"Classifier")
+    svc_cpredictor = CalibratedClassifierCV(cpredictormodel, cv=kf)
+
+    clf_list = [
+        (svc, "SVC"),
+        (svc_isotonic, "SVC + Isotonic"),
+        (svc_sigmoid, "SVC + Sigmoid"),
+        (svc_cpredictor, "SVC + cPredictor"),
+    ]
+
+    logging.info('Reading in the data')
+    Data = read_h5ad(reference_H5AD)
+    
+    Data = cpredictorperf.expression_cutoff(Data, LabelsPath)
+
+    data_train = pd.DataFrame.sparse.from_spmatrix(Data.X, index=list(Data.obs.index.values), columns=list(Data.var.index.values))
+    data_train = data_train.to_numpy(dtype="float16")
+    
+    data_train = cpredictorperf.preprocess_data_train(data_train)
+    #data_train_processed = data_train
+    
+    # Do label encoding
+    labels = pd.read_csv(LabelsPath, header=0,index_col=None, sep=',') #, usecols = col
+    label_encoder = LabelEncoder()
+    
+    y = label_encoder.fit_transform(labels.iloc[:,0].tolist())
+
+    # Generate a dictionary to map values to strings
+    res = dict(zip(label_encoder.inverse_transform(y),y))
+    res['Unlabeled'] = 999999
+    res = {v: k for k, v in res.items()}
+    res
+
+    # CV 3
+    y_binaries = []
+    for cls in range(len(np.unique(y))):
+        y_binary = np.where(y == cls, 1, 0)
+        y_binaries.append(y_binary)
+    print(y_binaries)
+
+    for i, y_binary in enumerate(y_binaries):
+        name_cond=''.join(list(label_encoder.inverse_transform([i])))
+        print(name_cond)
+        X_train, X_test, y_train, y_test = train_test_split(data_train, y_binaries[i], test_size=0.2, random_state=42)
+        colors = plt.get_cmap("Dark2")
+        fig = plt.figure(figsize=(5, 8))
+        gs = gridspec.GridSpec(4, 2)
+
+        ax_calibration_curve = fig.add_subplot(gs[:2, :2])
+        calibration_displays = {}
+        for i, (clf, name) in enumerate(clf_list):
+            clf.fit(X_train, y_train)
+            display = CalibrationDisplay.from_estimator(
+                clf,
+                X_test,
+                y_test,
+                n_bins=10,
+                name=name,
+                ax=ax_calibration_curve,
+                color=colors(i),
+                pos_label=1
+            )
+            calibration_displays[name] = display
+
+        ax_calibration_curve.grid()
+        ax_calibration_curve.set_title(f"Calibration plots (SVC) {name_cond}")
+
+        # Add histogram
+        grid_positions = [(2, 0), (2, 1), (3, 0), (3, 1)]
+        for i, (_, name) in enumerate(clf_list):
+            row, col = grid_positions[i]
+            ax = fig.add_subplot(gs[row, col])
+
+            ax.hist(
+                calibration_displays[name].y_prob,
+                range=(0, 1),
+                bins=10,
+                label=name,
+                color=colors(i),
+            )
+            ax.set(title=name, xlabel="Mean predicted probability", ylabel="Count")
+
+        plt.tight_layout()
+        #plt.savefig(f"{name_cond}_calibrated.png")
+        mlflow.log_figure(fig,f"{name_cond}_calibrated.png")
+        #plt.show()
+    return
+
+# Setup the scripts
+svc = NaivelyCalibratedLinearSVC(max_iter=10_000, dual="auto")
+svc_isotonic = CalibratedClassifierCV(svc, cv=3, method="isotonic")
+svc_sigmoid = CalibratedClassifierCV(svc, cv=3, method="sigmoid")
+
+clf_list = [
+    (svc, "SVC"),
+    (svc_isotonic, "SVC + Isotonic"),
+    (svc_sigmoid, "SVC + Sigmoid"),
+]
 
-print("Import performance function")
-from cPredictor.SVM_prediction import SVM_performance
 os.environ["GIT_PYTHON_REFRESH"] = "quiet"
 import git
 
-reference = "data/cma_meta_atlas.h5ad"
+# Specify data types and output dirs
+reference = "test/cma_meta_atlas_rfe.h5ad"
 labels = "data/training_labels_meta.csv"
 outdir = "test_output/"
-cPredictor_version = "0.3.2"
-
-metrics = SVM_performance(reference_H5AD=reference,LabelsPath=labels,OutputDir=outdir)
+cPredictor_version = "0.3.5"
 
 print("Setup tokens")
 # Set environments and passwords
 DAGSHUB_USER_NAME = 'Arts-of-coding'
 DAGSHUB_TOKEN =  os.environ['DH_key']
 DAGSHUB_REPO_OWNER = 'Arts-of-coding'
 MLFLOW_EXPERIMENT_NAME = 'Cornea'
@@ -50,21 +196,31 @@
 os.environ['MLFLOW_TRACKING_PASSWORD'] = DAGSHUB_TOKEN
 os.environ['MLFLOW_TRACKING_URI'] = f'https://dagshub.com/{DAGSHUB_REPO_OWNER}/{DAGSHUB_REPO_NAME}.mlflow'
 mlflow.set_tracking_uri(os.environ['MLFLOW_TRACKING_URI'])
 os.environ['MLFLOW_EXPERIMENT_NAME'] = MLFLOW_EXPERIMENT_NAME
 
 print("Upload metrics to dagshub for model tracking")
 
+# Read in metrics from the produced file of the CLI command
+with open(f"{outdir}metrics.txt", "r") as file:
+    metrics = []
+    for line in file:
+        metric = float(line)
+        metrics.append(metric)
+
 # Create new experiment if it does not exist yet otherwise add to the current experiment
 try:
     expid = mlflow.create_experiment(MLFLOW_EXPERIMENT_NAME)
 except:
     print(f'Using existing run of {MLFLOW_EXPERIMENT_NAME}')
     mlflow.set_experiment(MLFLOW_EXPERIMENT_NAME)
 
 mlflow.start_run(run_name=str(f'{MLFLOW_EXPERIMENT_NAME}_full_{Upload_type}'),experiment_id=None,
                  tags={"version": str(cPredictor_version),"model": str(SVM_model)})
 mlflow.log_metric("weighted_F1_score", metrics[0])
 mlflow.log_metric("weighted_accuracy_score", metrics[1])
 mlflow.log_metric("weighted_precision_score", metrics[2])
 
+# Run calibration function
+SVM_calibration(reference_H5AD=reference,LabelsPath=labels,OutputDir=outdir, rejected=False)
+
 mlflow.end_run()
```

## Comparing `cPredictor-0.3.2.dist-info/LICENSE` & `cPredictor-0.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cPredictor-0.3.2.dist-info/METADATA` & `cPredictor-0.3.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cPredictor
-Version: 0.3.2
+Version: 0.3.5
 Summary: Cell command line predictor
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools ==68.2.2
 Requires-Dist: wheel
 Requires-Dist: python-build
 Requires-Dist: pytest-cov
 Requires-Dist: h5py
 Requires-Dist: numpy <1.24,>=1.23.3
 Requires-Dist: pandas >=1.4.4
 Requires-Dist: scikit-learn
 Requires-Dist: scanpy >=1.9.1
 Requires-Dist: importlib-resources
-Requires-Dist: pyarrow
+Requires-Dist: pyarrow <16,>=4.0.0
 Requires-Dist: scikit-learn-intelex
 
 # `cPredictor` package <img src='cPredictor/man/c_predictor_simple.png' align="right" height="80" />
 
 [![PyPI version](https://badge.fury.io/py/cPredictor.svg)](https://badge.fury.io/py/cPredictor)
 [![CI/CD](https://github.com/Arts-of-coding/cPredictor/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Arts-of-coding/cPredictor/actions/workflows/ci-cd.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/598ba117b586183c46a8/maintainability)](https://codeclimate.com/github/Arts-of-coding/cPredictor/maintainability)
```

## Comparing `cPredictor-0.3.2.dist-info/RECORD` & `cPredictor-0.3.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-cPredictor/SVM_prediction.py,sha256=Qkkntk72C_87wus0CqWNJgxWK1Mdvr2uqHj3EzmrTIU,42101
-cPredictor/__init__.py,sha256=GAkuTjv5ua-ClItkaKLoQft-LQ2ghF4O_ewpmu4i8cM,354
+cPredictor/SVM_prediction.py,sha256=8972cpamcVDflAcqAz3ocjNenIo13QRlpThMH34Zjm8,43185
+cPredictor/__init__.py,sha256=ye20bcsMXJLCNLdmqzTzjDgan2OaAgQ8wT00WD-cNDo,354
 cPredictor/tests/SVM_prediction_test.py,sha256=sKJF3SHRSY6Njt1XD6ty-D_CkHcE4n1O57J5IMJkKak,6922
 cPredictor/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cPredictor/tests/cPredictor_test_model.py,sha256=pem9bCWiMC7sCl0McLPddi1i7OkTxXLF2dZxdTCaTiU,2398
-cPredictor-0.3.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-cPredictor-0.3.2.dist-info/METADATA,sha256=7QVqk_4n56irw2KGxt4CG9TeFIV-lt6O96bDKUt0t3g,3349
-cPredictor-0.3.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cPredictor-0.3.2.dist-info/entry_points.txt,sha256=jWviDlyXk8UTuVRVDXW5ihbZ7xWbKSt3uKRwjx2pvJw,227
-cPredictor-0.3.2.dist-info/top_level.txt,sha256=NXWRMFJ_ywM9zoRGffXs1j38bnAtf-odfECMfsNtJV4,11
-cPredictor-0.3.2.dist-info/RECORD,,
+cPredictor/tests/cPredictor_test_model.py,sha256=NWA9XGx6_f78E3dMs3PVXUJKiAcGxFWAak-TIX0hVPM,8174
+cPredictor-0.3.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+cPredictor-0.3.5.dist-info/METADATA,sha256=O9B4NHihtm5UgymUp1AFS_Ci8O6K0HP8nhVxbbpH7cU,3361
+cPredictor-0.3.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cPredictor-0.3.5.dist-info/entry_points.txt,sha256=jWviDlyXk8UTuVRVDXW5ihbZ7xWbKSt3uKRwjx2pvJw,227
+cPredictor-0.3.5.dist-info/top_level.txt,sha256=NXWRMFJ_ywM9zoRGffXs1j38bnAtf-odfECMfsNtJV4,11
+cPredictor-0.3.5.dist-info/RECORD,,
```

