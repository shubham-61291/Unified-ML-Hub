# Unsupervised Learning

> Navigation and practical notes for this repository layer.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Scope

This layer groups experiments that discover structure without using target labels to fit the unsupervised model. Some demos use labels only for post-hoc external evaluation; those labels should not be confused with training supervision.

## Subdirectories

| Directory | Scope | README |
|---|---|---|
| **CLUSTERING** | Partition or organize examples using similarity, density, hierarchical and mixture-based methods. | [Open README](./CLUSTERING/README.md) |
| **Dimensionality Reduction** | Construct lower-dimensional representations for visualization or downstream analysis. | [Open README](./Dimensionality%20Reduction/README.md) |
| **Anomaly Detection** | Rank or flag unusual points using statistical, distance and reconstruction approaches. | [Open README](./Anomaly%20Detection/README.md) |
| **Association Rule Learning** | Discover item co-occurrence rules with support and interestingness statistics. | [Open README](./Association%20Rule%20Learning/README.md) |

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
