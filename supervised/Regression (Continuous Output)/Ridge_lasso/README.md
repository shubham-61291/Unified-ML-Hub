# Ordinary Least Squares, Ridge, Lasso and ElasticNet

> Implementation notes for the code and artifacts currently stored in this directory.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Overview

A regularized-regression comparison focused on coefficient shrinkage, validation performance across regularization strength and model diagnostics.

## Data and assumptions

Scikit-learn California Housing dataset; first-time fetching may require network access.

## Implemented workflow

- Ordinary least squares baseline
- Ridge (L2), Lasso (L1) and ElasticNet regularization
- Validation sweeps over alpha values
- StandardScaler pipelines
- MSE, RMSE, MAE, R² and adjusted R²
- Coefficient paths and feature-coefficient comparison

## Evaluation and artifacts

The plots emphasize regularization effects, stability and diagnostics across four regression estimators.

The following result files are present in this directory (paths checked against the repository tree):

- [R2 comparison.png](./R2%20comparison.png)
- [RMSE comparison.png](./RMSE%20comparison.png)
- [MAE comparison.png](./MAE%20comparison.png)
- [RIDGE_metricsvsalpha.png](./RIDGE_metricsvsalpha.png)
- [LASSO_metricvsalpha.png](./LASSO_metricvsalpha.png)
- [Coefficientpaths_RIDGE.png](./Coefficientpaths_RIDGE.png)
- [Coefficientpaths_LASSO.png](./Coefficientpaths_LASSO.png)
- [ELASTICNET validation R2.png](./ELASTICNET%20validation%20R2.png)

### Selected visualizations

![R2 comparison.png](./R2%20comparison.png)

![RMSE comparison.png](./RMSE%20comparison.png)

![MAE comparison.png](./MAE%20comparison.png)

![RIDGE_metricsvsalpha.png](./RIDGE_metricsvsalpha.png)

## Run and dependencies

- Implementation: [ridge_lasso.py](./ridge_lasso.py)
- Dependencies: [requirements.txt](./requirements.txt)
```bash
pip install -r "requirements.txt"
python "ridge_lasso.py"
```

## Limitations and reproducibility notes

- Feature scaling is important when comparing penalty strengths.
- The validation-selected regularization level is not a guarantee of performance on future data.
- Coefficient magnitudes are not causal explanations.

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
