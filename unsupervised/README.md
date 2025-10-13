# 🧩 Unsupervised Learning — Complete Model Collection

This directory presents the **complete suite of Unsupervised Learning algorithms**, implemented and documented by **Shubham Singh**.  
Unsupervised learning identifies hidden structures or patterns in unlabeled data — without any explicit target variable — enabling clustering, representation learning, anomaly detection, and association rule mining.

---

## 🧭 Structure Overview

| Category | Description | Folder Link |
|-----------|-------------|--------------|
| 🧠 **Clustering** | Groups data points based on similarity using algorithms such as K-Means, Hierarchical, DBSCAN, GMM, Spectral, BIRCH, Mean Shift, and SOM. | [Open CLUSTERING Folder](./CLUSTERING/) |
| 📉 **Dimensionality Reduction** | Reduces high-dimensional data into compact representations while preserving structure — includes PCA, t-SNE, UMAP, Autoencoder, and VAE. | [Open Dimensionality Reduction Folder](./Dimensionality%20Reduction/) |
| ⚠️ **Anomaly Detection** | Detects rare or abnormal patterns using Isolation Forest, One-Class SVM, Autoencoder, and statistical baselines. | [Open Anomaly Detection Folder](./Anomaly%20Detection/) |
| 🛒 **Association Rule Learning** | Mines co-occurrence relationships (e.g., Market Basket Analysis) using Apriori, FP-Growth, and Eclat. | [Open Association Rule Learning Folder](./Association%20Rule%20Learning/) |

---

## 📚 Detailed ReadMe Access

### 🧠 CLUSTERING  
Implements **8 algorithms** on the Iris dataset — K-Means, Hierarchical (Ward/Complete), DBSCAN, GMM, Spectral, BIRCH, Mean Shift, and SOM.  
Evaluates both internal and external metrics, with PCA/t-SNE plots, silhouettes, dendrograms, and confusion heatmaps.  

🔗 [View Full CLUSTERING README](./CLUSTERING/README.md)

---

### ⚠️ ANOMALY DETECTION  
Implements **5 anomaly detection methods** — Isolation Forest, One-Class SVM, Autoencoder, Mahalanobis Distance, and Z-Score Baseline.  
Evaluates AUC-ROC, AUC-PR, and F1, with complete visualization and comparative summaries.  

🔗 [View Full ANOMALY DETECTION README](./Anomaly%20Detection/README.md)

---

### 🛒 ASSOCIATION RULE LEARNING  
Implements **Apriori**, **FP-Growth**, and **Eclat** algorithms for Market Basket Analysis.  
Includes redundancy pruning, rule metrics (support, confidence, lift, leverage), generalization checks, and rich visualizations.  

🔗 [View Full ASSOCIATION RULE LEARNING README](./Association%20Rule%20Learning/README.md)

---

### 📉 DIMENSIONALITY REDUCTION  
Implements **13 linear, manifold, and neural** techniques — PCA, t-SNE, UMAP, LLE, Isomap, MDS, NMF, ICA, Autoencoder, and Variational Autoencoder (VAE).  
Evaluates reconstruction error, trustworthiness, and clustering quality using ARI/NMI/Silhouette metrics.  

🔗 [View Full DIMENSIONALITY REDUCTION README](./Dimensionality%20Reduction/README.md)

---

## 📊 Summary Table

| Task Type | Algorithms | Purpose | Example Metrics |
|------------|-------------|----------|----------------|
| **Clustering** | K-Means, DBSCAN, GMM, Spectral, BIRCH | Discover natural groups in data | Silhouette, ARI, NMI |
| **Dimensionality Reduction** | PCA, t-SNE, UMAP, AE, VAE | Compress data while preserving structure | Reconstruction Error, Trustworthiness |
| **Anomaly Detection** | Isolation Forest, One-Class SVM, AE | Identify rare or abnormal points | AUC, F1, Precision-Recall |
| **Association Rule Learning** | Apriori, FP-Growth, Eclat | Discover item relationships | Support, Confidence, Lift |

---

## 👨‍💻 Author
**Shubham Singh**

## 📜 License
MIT License
