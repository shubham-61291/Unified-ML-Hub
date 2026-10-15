# Unified ML Hub

> A layered, code-first collection of supervised and unsupervised machine-learning experiments.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Overview

Unified ML Hub organizes individual algorithm experiments beneath two top-level learning paradigms. Each algorithm-level directory contains its implementation, a local dependency file where provided, existing result visualizations, and a focused README. The documentation is organized to follow the repository tree rather than treating it as a flat list.

## Repository map

| Layer | Purpose | Navigation |
|---|---|---|
| Supervised learning | Learn from labeled examples for classification, regression or ranking | [Open supervised overview](./supervised/README.md) |
| Unsupervised learning | Explore groups, low-dimensional representations, anomalies and item co-occurrence | [Open unsupervised overview](./unsupervised/README.md) |

## Supervised learning

| Collection | What it contains | README |
|---|---|---|
| **Classification (Categorical Output)** | Binary, multiclass and multilabel classifiers: boosted trees, KNN, Keras neural networks, Naïve Bayes, SVM, decision tree, logistic regression and random forest. | [Open overview](./supervised/Classification%20%28Categorical%20Output%29/README.md) |
| **Regression (Continuous Output)** | Linear and polynomial baselines, regularized regression, LightGBM regression and neural regression with uncertainty-oriented experiments. | [Open overview](./supervised/Regression%20%28Continuous%20Output%29/README.md) |
| **Learning-to-Rank** | Pointwise, pairwise, listwise, boosted and neural ranking experiments. | [Open overview](./supervised/RANKING/README.md) |

## Unsupervised learning

| Collection | What it contains | README |
|---|---|---|
| **Clustering** | Nine clustering methods/variants with internal and post-hoc external diagnostics. | [Open overview](./unsupervised/CLUSTERING/README.md) |
| **Dimensionality Reduction** | Linear, manifold and neural representations, with plots and downstream evaluation. | [Open overview](./unsupervised/Dimensionality%20Reduction/README.md) |
| **Anomaly Detection** | Classical, distance/statistical and autoencoder approaches on synthetic data. | [Open overview](./unsupervised/Anomaly%20Detection/README.md) |
| **Association Rule Learning** | Apriori, FP-Growth and Eclat on demonstration and synthetic transactions. | [Open overview](./unsupervised/Association%20Rule%20Learning/README.md) |

## How to use this repository

1. Open the overview for the learning paradigm or task you need.
2. Follow the link to the algorithm directory and read its local README before running code.
3. Install the dependencies from that directory’s `requirements.txt` where present. Some notebook exports contain IPython `!pip` magic and must be run in a notebook-compatible environment as committed, or have those magic lines removed after dependencies are installed.
4. Review the dataset and evaluation notes before interpreting a plot or a score.

## Reproducibility and interpretation

- Many classification examples use scikit-learn’s built-in Breast Cancer and Iris datasets; multilabel and several unsupervised demonstrations generate data in code. California Housing examples fetch data on first use. The association-rule example constructs synthetic transactions.
- Saved PNG files are retained experiment artifacts. This documentation refresh checks source, paths and claims; it does not claim every experiment was freshly rerun or that all historical metric tables were reproduced.
- Thresholds, scores and feature-importance plots are evidence about a particular experiment, dataset and split—not causal claims or guarantees of production performance.
- GPU support and dependency compatibility depend on the installed versions, operating system and hardware.

## Documentation and licensing

Each directory with a README also has a local `LICENSE` file. All package READMEs include the full MIT License text and link to their own `./LICENSE`. See [the repository license](./LICENSE).

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
