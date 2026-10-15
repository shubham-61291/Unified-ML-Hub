# Dimensionality Reduction: Linear, Manifold and Neural Methods

> Implementation notes for the code and artifacts currently stored in this directory.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Overview

A consolidated embedding comparison using linear decompositions, manifold-learning methods and neural autoencoders, evaluated through embedding visualizations, reconstruction diagnostics and downstream clustering.

## Data and assumptions

Scikit-learn Iris dataset with ground-truth labels available for post-hoc external evaluation.

## Implemented workflow

- PCA, Kernel PCA, Sparse PCA, Truncated SVD, ICA, NMF and Factor Analysis
- t-SNE, UMAP, Isomap, Locally Linear Embedding and MDS
- Autoencoder and Variational Autoencoder
- Explained variance, trustworthiness, reconstruction MSE, silhouette, ARI and NMI

## Evaluation and artifacts

The stored plots support qualitative comparison; downstream cluster metrics depend on the embedding, clustering configuration and dataset.

The following result files are present in this directory (paths checked against the repository tree):

- [dimensionality_reduction_side_by_side.png](./dimensionality_reduction_side_by_side.png)
- [pca_2d_coloured_by_class.png](./pca_2d_coloured_by_class.png)
- [pca_screen_plot_cumulative_variance.png](./pca_screen_plot_cumulative_variance.png)
- [umap_2d_coloured_by_class.png](./umap_2d_coloured_by_class.png)
- [autoencoder_2d_coloured_by_class.png](./autoencoder_2d_coloured_by_class.png)
- [vae_2d_coloured_by_class.png](./vae_2d_coloured_by_class.png)
- [reconstruction_error_comparison.png](./reconstruction_error_comparison.png)
- [manifold_trustworthiness.png](./manifold_trustworthiness.png)

### Selected visualizations

![dimensionality_reduction_side_by_side.png](./dimensionality_reduction_side_by_side.png)

![pca_2d_coloured_by_class.png](./pca_2d_coloured_by_class.png)

![pca_screen_plot_cumulative_variance.png](./pca_screen_plot_cumulative_variance.png)

![umap_2d_coloured_by_class.png](./umap_2d_coloured_by_class.png)

## Run and dependencies

- Implementation: [DIMENSIONALITY_REDUCTION.py](./DIMENSIONALITY_REDUCTION.py)
- Dependencies: [requirements.txt](./requirements.txt)
```bash
pip install -r "requirements.txt"
python "DIMENSIONALITY_REDUCTION.py"
```

## Limitations and reproducibility notes

- The source implements 14 techniques when all listed methods are counted; the previous README stated 13 despite listing 14.
- The repo includes results and a requirements file but no trained model checkpoint. Autoencoder/VAE training occurs in the script.
- External clustering metrics use the Iris labels only for post-hoc evaluation; this is not supervised training of the embedding.

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
