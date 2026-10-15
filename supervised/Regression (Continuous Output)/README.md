# Regression (Continuous Output)

> Continuous-target regression experiments based primarily on California Housing.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Scope

The directories compare a transparent linear baseline with feature expansion, coefficient regularization, boosted trees and neural models. Most experiments fetch California Housing through scikit-learn; data retrieval may need network access on first run.

## Algorithm navigation

| Model | Focus | Project README |
|---|---|---|
| **Gradient Boosted Regression Trees** | LightGBM, hyperparameter search, residuals, PDP/ICE and SHAP. | [Open README](./Gradient%20Boosted%20Regression%20Trees/README.md) |
| **Linear Regression** | Ordinary least-squares baseline with holdout and cross-validation diagnostics. | [Open README](./Linear%20Regression/README.md) |
| **Neural Networks** | Neural regression with dropout/heteroscedastic uncertainty approaches. | [Open README](./Neural%20Networks%20%28for%20continuous%20outputs%29/README.md) |
| **Polynomial Regression** | Single-feature polynomial expansion and degree selection. | [Open README](./Polynomial%20Regression/README.md) |
| **Ridge / Lasso / ElasticNet** | Regularization, coefficient paths and validation sweeps. | [Open README](./Ridge_lasso/README.md) |

## Metrics

MSE and RMSE penalize larger errors, MAE summarizes absolute error, and R² compares prediction with a mean-target baseline. Adjusted R² tries to account for feature count but has assumptions and can be unstable on small samples. Compare validation and test splits separately; do not select models on the test set.

## Practical notes

- The model-specific README identifies the script, dependency file and available plots.
- A few scripts contain IPython package-install magic and require notebook-compatible execution unless converted.
- GPU acceleration is optional in principle but depends on compatible runtime libraries; it is not guaranteed by the existence of a GPU-oriented parameter.
- Historical metrics are not represented as newly reproduced benchmarks in this documentation refresh.

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
