# Logistic Regression Classification

> Implementation notes for the code and artifacts currently stored in this directory.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Overview

A baseline statistical classifier implemented for binary, multiclass and multilabel examples, with standardized numeric input, cross-validation and decision-threshold analysis.

## Data and assumptions

Scikit-learn Breast Cancer and Iris datasets, plus a generated multilabel classification dataset.

## Implemented workflow

- LogisticRegression with an lbfgs solver in the binary example
- StandardScaler for binary inputs
- Stratified five-fold cross-validation
- F1/Youden’s-J/cost threshold sweeps, ROC/PR and confusion matrices

## Evaluation and artifacts

Provides a comparatively interpretable reference point for the other classification algorithms in this repository.

The following result files are present in this directory (paths checked against the repository tree):

- [ConfusionMatrix.png](./ConfusionMatrix.png)
- [ROC_PRcurve.png](./ROC_PRcurve.png)
- [ROC_PR_optimacurve.png](./ROC_PR_optimacurve.png)
- [thresholdtuning.png](./thresholdtuning.png)
- [confusion_matrixmulticlass.png](./confusion_matrixmulticlass.png)
- [roc_curve_multiclass.png](./roc_curve_multiclass.png)
- [confusionmatrix_multilabel.png](./confusionmatrix_multilabel.png)

### Selected visualizations

![ConfusionMatrix.png](./ConfusionMatrix.png)

![ROC_PRcurve.png](./ROC_PRcurve.png)

![ROC_PR_optimacurve.png](./ROC_PR_optimacurve.png)

![thresholdtuning.png](./thresholdtuning.png)

## Run and dependencies

- Implementation: [logistic_regression.py](./logistic_regression.py)
- Dependencies: [requirements.txt](./requirements.txt)
```bash
pip install -r "requirements.txt"
python "logistic_regression.py"
```

## Limitations and reproducibility notes

- Threshold selection is a decision-policy step; it does not change the underlying probability model.
- The cost-minimization threshold depends on the costs configured in the script.

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
