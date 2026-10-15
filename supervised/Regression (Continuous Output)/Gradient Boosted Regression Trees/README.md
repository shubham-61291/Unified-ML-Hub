# Gradient Boosted Regression Trees (LightGBM)

> Implementation notes for the code and artifacts currently stored in this directory.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Overview

A LightGBM regression experiment with data splitting, randomized and grid search, early stopping, residual diagnostics, feature attribution and partial-dependence views.

## Data and assumptions

California Housing data loaded through scikit-learn, with a remote CSV mirror fallback in the script. Initial access can require network connectivity.

## Implemented workflow

- LightGBM LGBMRegressor
- 70/15/15 train/validation/test split
- RandomizedSearchCV and a focused GridSearchCV pass
- MSE, RMSE, MAE, R² and adjusted R²
- Residual plots, PDP/ICE, SHAP global and local explanations

## Evaluation and artifacts

This directory emphasizes regression diagnostics and feature-level interpretation rather than only a single score.

The following result files are present in this directory (paths checked against the repository tree):

- [learningcurve.png](./learningcurve.png)
- [leaarningcurve_bestgridmodel.png](./leaarningcurve_bestgridmodel.png)
- [residual_validationbest.png](./residual_validationbest.png)
- [residual_testbest.png](./residual_testbest.png)
- [actualvspredicted_validationbest.png](./actualvspredicted_validationbest.png)
- [actualvspredicted_testbest.png](./actualvspredicted_testbest.png)
- [top2features.png](./top2features.png)
- [SHAPvalue.png](./SHAPvalue.png)

### Selected visualizations

![learningcurve.png](./learningcurve.png)

![leaarningcurve_bestgridmodel.png](./leaarningcurve_bestgridmodel.png)

![residual_validationbest.png](./residual_validationbest.png)

![residual_testbest.png](./residual_testbest.png)

## Run and dependencies

- Implementation: [GBRT.py](./GBRT.py)
- Dependencies: [requirements.txt](./requirements.txt)
```bash
pip install -r "requirements.txt"
# Then run the script in a notebook-compatible environment as described above.
```

## Limitations and reproducibility notes

- The script includes IPython package-install magic and notebook display calls. Run notebook-style or remove the magic after installing requirements.
- GPU support is platform- and build-dependent; `device="gpu"` is not guaranteed to work on every LightGBM install.
- The CSV fallback is external data, so its availability and content are outside this repository’s control.

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
