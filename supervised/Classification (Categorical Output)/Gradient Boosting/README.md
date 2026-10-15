# Gradient Boosting Classification: XGBoost, LightGBM and CatBoost

> Implementation notes for the code and artifacts currently stored in this directory.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Overview

A comparative classification notebook/script for boosted-tree families across binary and multiclass tasks. The implementation includes ROC/precision–recall analysis, threshold diagnostics, calibration plots, confusion matrices, permutation importance and SHAP-related analysis where available.

## Data and assumptions

The code loads scikit-learn’s Breast Cancer and Iris datasets and generates a synthetic multilabel dataset. No project-specific CSV dataset is required for those examples; first-time dataset/model package downloads may require network access.

## Implemented workflow

- XGBoost classifier
- LightGBM classifier
- CatBoost classifier
- Binary and one-vs-rest multiclass/multilabel evaluation
- Cross-validation and threshold analysis

## Evaluation and artifacts

Model comparison artifacts cover classification quality and probability/threshold diagnostics; treat plotted results as saved experiment outputs, not as a fresh benchmark reproduced by this documentation pass.

The following result files are present in this directory (paths checked against the repository tree):

- [confusion_matrix_xgboost.png](./confusion_matrix_xgboost.png)
- [confusion_matrix_GBM.png](./confusion_matrix_GBM.png)
- [confusion_matrix_catboost.png](./confusion_matrix_catboost.png)
- [ROC_curve_xgboost.png](./ROC_curve_xgboost.png)
- [ROC_PR_Curve_GBM.png](./ROC_PR_Curve_GBM.png)
- [ROC_PR_curve_catboost.png](./ROC_PR_curve_catboost.png)
- [PR_curve_multiclass_catboost.png](./PR_curve_multiclass_catboost.png)
- [calibration_curve_binary.png](./calibration_curve_binary.png)
- [confusion_matrix_multiclass_catboost.png](./confusion_matrix_multiclass_catboost.png)

### Selected visualizations

![confusion_matrix_xgboost.png](./confusion_matrix_xgboost.png)

![confusion_matrix_GBM.png](./confusion_matrix_GBM.png)

![confusion_matrix_catboost.png](./confusion_matrix_catboost.png)

![ROC_curve_xgboost.png](./ROC_curve_xgboost.png)

## Run and dependencies

- Implementation: [gradient_boosting.py](./gradient_boosting.py)
- Dependencies: [requiremets.txt](./requiremets.txt)
```bash
pip install -r "requiremets.txt"
# Then run the script in a notebook-compatible environment as described above.
```

## Limitations and reproducibility notes

- The script is exported from Google Colab and contains an IPython `!pip` install line. It is not a plain `python file.py` script until that magic is removed or run in a notebook-compatible environment.
- XGBoost GPU parameters vary by package version and hardware; CPU/GPU compatibility is not guaranteed across environments.
- The file `requiremets.txt` is misspelled in the repository; the documentation preserves the existing filename rather than silently renaming it.

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
