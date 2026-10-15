# Learning-to-Rank (LTR) Model Comparison

> Implementation notes for the code and artifacts currently stored in this directory.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Overview

A consolidated ranking experiment covering pointwise, pairwise and listwise learning, boosted ranking models and PyTorch-based neural ranking approaches.

## Data and assumptions

Ranking examples and grouped relevance data are prepared within the script; verify the data-generation/splitting block before substituting production ranking data.

## Implemented workflow

- Pointwise Ridge baseline
- Pairwise logistic and listwise ranking approaches
- XGBoost and LightGBM with Optuna search
- Deep ListNet and neural LambdaRank-style training
- NDCG@k, Precision@k, MAP, MRR and per-query evaluation

## Evaluation and artifacts

Use the outputs to compare ranking quality at cutoffs and the variability of scores across queries, rather than treating one aggregate metric as sufficient.

The following result files are present in this directory (paths checked against the repository tree):

- [ndcg_vs_k_xgboost.png](./ndcg_vs_k_xgboost.png)
- [ndcg_vs_k_lightgbm_optuna.png](./ndcg_vs_k_lightgbm_optuna.png)
- [ndcg_vs_k_deep_listnet.png](./ndcg_vs_k_deep_listnet.png)
- [ndcg_vs_k_lambdarank_nn.png](./ndcg_vs_k_lambdarank_nn.png)
- [ndcg_distribution_xgboost_optuna.png](./ndcg_distribution_xgboost_optuna.png)
- [per_query_ndcg_boxplot.png](./per_query_ndcg_boxplot.png)
- [xgboost_top_20_feature_importance.png](./xgboost_top_20_feature_importance.png)
- [training_loss_deeplistnet.png](./training_loss_deeplistnet.png)

### Selected visualizations

![ndcg_vs_k_xgboost.png](./ndcg_vs_k_xgboost.png)

![ndcg_vs_k_lightgbm_optuna.png](./ndcg_vs_k_lightgbm_optuna.png)

![ndcg_vs_k_deep_listnet.png](./ndcg_vs_k_deep_listnet.png)

![ndcg_vs_k_lambdarank_nn.png](./ndcg_vs_k_lambdarank_nn.png)

## Run and dependencies

- Implementation: [RANKING.py](./RANKING.py)
- Dependencies: [requirements.txt](./requirements.txt)
```bash
pip install -r "requirements.txt"
# Then run the script in a notebook-compatible environment as described above.
```

## Limitations and reproducibility notes

- The script is a Colab notebook export containing `!pip` magic and should be run notebook-style as currently written or have those lines removed after dependency installation.
- Ranking scores depend on query grouping and relevance labels; do not compare aggregate metrics across incompatible grouping schemes.
- PyTorch wheels are requested from the CPU wheel index in the script; GPU behavior depends on the local install.

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
