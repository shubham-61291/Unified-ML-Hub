# Supervised Learning

> Navigation and practical notes for this repository layer.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Scope

This layer groups implementations trained against labeled examples. Use the category README to select a task family, then the algorithm-level README for its script, dependencies, assets and caveats.

## Subdirectories

| Directory | Scope | README |
|---|---|---|
| **Classification (Categorical Output)** | Categorical prediction: binary, multiclass and multilabel classifiers. | [Open README](./Classification%20%28Categorical%20Output%29/README.md) |
| **Regression (Continuous Output)** | Continuous-target prediction and model regularization. | [Open README](./Regression%20%28Continuous%20Output%29/README.md) |
| **RANKING** | Learning-to-rank with classical, boosted and neural methods. | [Open README](./RANKING/README.md) |

## Working with a project

- Prefer the local `requirements.txt` rather than assuming a single environment will satisfy every algorithm.
- Several files originated as notebook exports; check each algorithm README before choosing `python script.py` versus a notebook-compatible execution path.
- Dataset downloads, optional GPU backends and version-specific estimator parameters may affect whether a script runs unchanged.
- Treat included plots as historical artifacts unless you rerun the experiment with the same configuration.

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
