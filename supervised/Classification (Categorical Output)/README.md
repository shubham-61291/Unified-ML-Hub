# Classification (Categorical Output)

> An algorithm-level comparison of binary, multiclass and multilabel classification implementations.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Scope

This collection uses standard sample datasets and a generated multilabel dataset to demonstrate model-fitting and evaluation patterns. The directories are independent experiments rather than a single shared training pipeline.

## Algorithm navigation

| Algorithm | What to inspect | Project README |
|---|---|---|
| **Gradient Boosting** | XGBoost, LightGBM and CatBoost; binary and multiclass examples. | [Open README](./Gradient%20Boosting/README.md) |
| **KNN** | Distance-based binary, multiclass and multilabel classification. | [Open README](./KNN/README.md) |
| **Neural Networks (Keras)** | Dense networks and learning curves for three task formats. | [Open README](./NN/README.md) |
| **Naïve Bayes** | Probabilistic classification and feature-distribution diagnostics. | [Open README](./Na%C3%AFve%20Bayes/README.md) |
| **Support Vector Machines** | RBF and linear support-vector approaches. | [Open README](./Support%20Vector%20Machines%20%28SVM%29/README.md) |
| **Decision Tree** | Tree-based classification with feature and structure visualizations. | [Open README](./decission%20tree/README.md) |
| **Logistic Regression** | Linear decision boundaries, cross-validation and threshold analysis. | [Open README](./logistic%20regression/README.md) |
| **Random Forest** | Tree ensembles, OOB score and feature importance. | [Open README](./random%20forest/README.md) |

## Shared evaluation vocabulary

Accuracy, precision, recall and F1 measure label prediction under a selected decision rule. ROC-AUC and average precision evaluate ranked scores; calibration plots examine probability reliability; threshold curves show how the operating point changes. Confusion matrices should be read with the class balance and threshold in mind. Multilabel metrics (for example Hamming loss, Jaccard or subset accuracy) are not interchangeable with ordinary multiclass accuracy.

## Practical notes

- Most scripts load Breast Cancer and Iris datasets through scikit-learn and create the multilabel dataset in code.
- Some directories contain notebook-exported scripts. Follow the local README and requirements file, especially when IPython install magic is present.
- GPU-specific settings in boosted-model code depend on library version and hardware.
- Result figures are existing artifacts; no claim is made here that all historical metric tables were independently reproduced.

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
