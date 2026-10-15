# Random Forest Classification

> Implementation notes for the code and artifacts currently stored in this directory.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Overview

A tree-ensemble classifier comparison across binary, multiclass and multilabel examples, including out-of-bag behavior and both impurity-based and permutation feature importance.

## Data and assumptions

Scikit-learn Breast Cancer and Iris datasets, plus a generated multilabel classification dataset.

## Implemented workflow

- RandomForestClassifier
- Stratified cross-validation
- OOB score vs. number of trees
- Threshold tuning, calibration, ROC/PR, confusion matrices, feature and permutation importance

## Evaluation and artifacts

The saved artifacts illustrate ensemble evaluation and model-inspection views across the included sample tasks.

The following result files are present in this directory (paths checked against the repository tree):

- [confusion_matrix_binary.png](./confusion_matrix_binary.png)
- [roc_pr_curve_binary.png](./roc_pr_curve_binary.png)
- [threshold_tuning_binary.png](./threshold_tuning_binary.png)
- [calibration_curve_binary.png](./calibration_curve_binary.png)
- [feature_importance_binary.png](./feature_importance_binary.png)
- [permutation_importance_binary.png](./permutation_importance_binary.png)
- [oob_score_vs_number_of_trees.png](./oob_score_vs_number_of_trees.png)
- [confusion_matrix_multiclass.png](./confusion_matrix_multiclass.png)

### Selected visualizations

![confusion_matrix_binary.png](./confusion_matrix_binary.png)

![roc_pr_curve_binary.png](./roc_pr_curve_binary.png)

![threshold_tuning_binary.png](./threshold_tuning_binary.png)

![calibration_curve_binary.png](./calibration_curve_binary.png)

## Run and dependencies

- Implementation: [random forest.py](./random%20forest.py)
- Dependencies: [requirements.txt](./requirements.txt)
```bash
pip install -r "requirements.txt"
python "random forest.py"
```

## Limitations and reproducibility notes

- The script filename includes a space; quote the path when executing it from a shell.
- Feature importance is diagnostic rather than causal evidence.

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
