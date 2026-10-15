# K-Nearest Neighbors (KNN) Classification

> Implementation notes for the code and artifacts currently stored in this directory.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Overview

An end-to-end KNN comparison across binary, multiclass and multilabel classification, with scaling, cross-validation, probability-based diagnostics and selection of the neighborhood size.

## Data and assumptions

Scikit-learn Breast Cancer and Iris datasets, plus a generated multilabel classification dataset.

## Implemented workflow

- Distance-weighted KNN with a default neighborhood parameter in the script
- StandardScaler + estimator Pipeline
- Stratified cross-validation for binary classification
- Threshold, calibration, ROC/PR, confusion-matrix, k-vs-error and subset-accuracy diagnostics

## Evaluation and artifacts

Use this directory to study distance-based classification trade-offs and how scaling, neighbor count and threshold selection affect the displayed evaluation.

The following result files are present in this directory (paths checked against the repository tree):

- [confusion_matrix_binary.png](./confusion_matrix_binary.png)
- [ROC_PR_Curve_binary.png](./ROC_PR_Curve_binary.png)
- [threshold_tuning_binary.png](./threshold_tuning_binary.png)
- [Calibration_curve_binary.png](./Calibration_curve_binary.png)
- [Kvserror_binary.png](./Kvserror_binary.png)
- [Confusion_matrix_multiclass.png](./Confusion_matrix_multiclass.png)
- [ROC_curve_multiclass.png](./ROC_curve_multiclass.png)
- [PR_Curve_multilabel.png](./PR_Curve_multilabel.png)

### Selected visualizations

![confusion_matrix_binary.png](./confusion_matrix_binary.png)

![ROC_PR_Curve_binary.png](./ROC_PR_Curve_binary.png)

![threshold_tuning_binary.png](./threshold_tuning_binary.png)

![Calibration_curve_binary.png](./Calibration_curve_binary.png)

## Run and dependencies

- Implementation: [KNN.py](./KNN.py)
- Dependencies: [requirements.txt](./requirements.txt)
```bash
pip install -r "requirements.txt"
python "KNN.py"
```

## Limitations and reproducibility notes

- The datasets are loaded from scikit-learn; the multilabel data is generated in code.
- Saved figures represent existing recorded runs. Metrics may change with dependency versions and data-generation settings.

## Author

Shubham Kumar Singh

## License

Licensed under the MIT License. See [`./LICENSE`](./LICENSE). The complete license text is included below for portability.

```text
MIT License

Copyright (c) 2026 Shubham Kumar Singh

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
