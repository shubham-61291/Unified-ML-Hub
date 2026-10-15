# Support Vector Machine (SVM) Classification

> Implementation notes for the code and artifacts currently stored in this directory.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Overview

A support-vector classifier comparison for binary, multiclass and multilabel tasks. The binary pipeline uses an RBF-kernel SVC with probability estimates; LinearSVC/one-vs-rest variants support additional comparisons.

## Data and assumptions

Scikit-learn Breast Cancer and Iris datasets, plus a generated multilabel classification dataset.

## Implemented workflow

- RBF SVC and LinearSVC variants
- StandardScaler pipeline for SVM
- Stratified cross-validation
- ROC/PR, threshold tuning, calibration and confusion matrices

## Evaluation and artifacts

The outputs are intended to help compare margin-based classifiers and probability/threshold behavior under standard sample datasets.

The following result files are present in this directory (paths checked against the repository tree):

- [confusion_matrix_binary.png](./confusion_matrix_binary.png)
- [roc_pr_curve_binary.png](./roc_pr_curve_binary.png)
- [roc_pr_curve_binary_optima.png](./roc_pr_curve_binary_optima.png)
- [threshold_tuning_binary.png](./threshold_tuning_binary.png)
- [calibration_curve_binary.png](./calibration_curve_binary.png)
- [confusion_matrix_multiclass.png](./confusion_matrix_multiclass.png)
- [roc_curve_multiclass.png](./roc_curve_multiclass.png)
- [confusion_matrix_label0.png](./confusion_matrix_label0.png)

### Selected visualizations

![confusion_matrix_binary.png](./confusion_matrix_binary.png)

![roc_pr_curve_binary.png](./roc_pr_curve_binary.png)

![roc_pr_curve_binary_optima.png](./roc_pr_curve_binary_optima.png)

![threshold_tuning_binary.png](./threshold_tuning_binary.png)

## Run and dependencies

- Implementation: [SVM.py](./SVM.py)
- Dependencies: [requirements.txt](./requirements.txt)
```bash
pip install -r "requirements.txt"
python "SVM.py"
```

## Limitations and reproducibility notes

- RBF SVC probability estimation entails calibration internally and adds computational cost.
- Saved results are tied to the recorded environment and split seed; this package does not rerun the benchmark.

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
