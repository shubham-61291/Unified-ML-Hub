# Decision Tree Classification

> Implementation notes for the code and artifacts currently stored in this directory.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Overview

An interpretable tree-classification pipeline spanning binary, multiclass and multilabel tasks with threshold selection, calibration and feature/tree visualizations.

## Data and assumptions

Scikit-learn Breast Cancer and Iris datasets, plus a generated multilabel classification dataset.

## Implemented workflow

- DecisionTreeClassifier with Gini criterion in the binary example
- Stratified cross-validation
- Binary threshold criteria including F1, Youden’s J and a configured cost objective
- Confusion matrices, ROC/PR, calibration and feature importance

## Evaluation and artifacts

The figures emphasize interpretability alongside task-specific classification evaluation.

The following result files are present in this directory (paths checked against the repository tree):

- [confusionmatrix_binary.png](./confusionmatrix_binary.png)
- [ROC_PRcurve_binary.png](./ROC_PRcurve_binary.png)
- [thresholdtuning_binary.png](./thresholdtuning_binary.png)
- [calibrationcurve_binary.png](./calibrationcurve_binary.png)
- [featureimportance_binary.png](./featureimportance_binary.png)
- [decissiontree_structure.png](./decissiontree_structure.png)
- [confusionmatrix_multiclass.png](./confusionmatrix_multiclass.png)
- [confusionmatrix_multilabel.png](./confusionmatrix_multilabel.png)

### Selected visualizations

![confusionmatrix_binary.png](./confusionmatrix_binary.png)

![ROC_PRcurve_binary.png](./ROC_PRcurve_binary.png)

![thresholdtuning_binary.png](./thresholdtuning_binary.png)

![calibrationcurve_binary.png](./calibrationcurve_binary.png)

## Run and dependencies

- Implementation: [decission_tree.py](./decission_tree.py)
- Dependencies: [requirements.txt](./requirements.txt)
```bash
pip install -r "requirements.txt"
python "decission_tree.py"
```

## Limitations and reproducibility notes

- The repository folder and script use the spelling `decission`; links retain those exact names.
- Decision trees can be sensitive to split/data variations; saved metrics should be interpreted with the recorded split and evaluation setup.

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
