# 🧠 Clustering — K-Means, Hierarchial (Ward/Complete), DBSCAN, GMM, Spectral, BIRCH, Mean Shift & SOM

The **Clustering** project implements and compares multiple unsupervised learning algorithms on the Iris dataset.  
It includes **K-Means, Hierarchial (Ward & Agglomerative-Complete), DBSCAN, Gaussian Mixture (GMM), Spectral Clustering, BIRCH, Mean Shift, and Self-Organizing Maps (SOM)** with complete evaluation (internal & external metrics) and rich visualizations (PCA, t-SNE, silhouettes, dendrograms, and confusion heatmaps).

---

## 🚀 Key Highlights
✅ 8 clustering algorithms with unified evaluation  
✅ Internal metrics: Silhouette, Davies–Bouldin, Calinski–Harabasz, Dunn  
✅ External metrics: ARI, NMI, V-Measure, Homogeneity, Completeness, FMI, Purity  
✅ Model selection aids: **K-Means Elbow & Gap**, **GMM BIC/AIC & Silhouette vs k**, **DBSCAN sweep (visualized via outputs)**  
✅ Visual suite per algorithm: **PCA/t-SNE**, **Silhouette**, **Confusion Heatmap**, **Cluster Size bars**

---

## 📊 K-Means

### Elbow & Gap
![K-Means Elbow](k_means_elbow.png)  
![K-Means Gap](k_means_gap.png)

### PCA & t-SNE
![PCA — K-Means](pca_2d_k_means.png)  
![t-SNE — K-Means](t_sne_2d_k_means.png)

### Silhouette & Confusion Heatmap
![Silhouette — K-Means](silhouette_k_means.png)  
![Confusion Heatmap — K-Means](confusion_heatmap_k_means.png)

### Cluster Sizes
![Cluster Sizes — K-Means](cluster_sizes_k_means.png)

---

## 🌲 Hierarchial (Ward) & Agglomerative (Complete)

### Dendrogram (Ward)
![Hierarchial Dendrogram — Ward](hierarchical_dendrogram_ward.png)

### PCA & t-SNE
![PCA — Hierarchial (Ward)](pca_2d_hierarchial_ward.png)  
![t-SNE — Hierarchial (Ward)](tsne_2d_hierarchial_ward.png)

### Silhouette & Confusion Heatmap (Ward)
![Silhouette — Hierarchial (Ward)](silhoutte_hierarchial_ward.png)  
![Confusion Heatmap — Hierarchial](confusion_heatmap_hierarchial.png)

### Agglomerative (Complete): PCA/t-SNE, Silhouette, Heatmap, Sizes
![PCA — Agglomerative Complete](pca_2d_agglomerative_complete.png)  
![t-SNE — Agglomerative Complete](tsne_2d_agglomerative_complete.png)  
![Silhouette — Agglomerative Complete](silhouette_agglomerative_complete.png)  
![Confusion Heatmap — Agglomerative Complete](confusion_heatmap_agglomerative_complete.png)  
![Cluster Sizes — Agglomerative Complete](cluster_sizes_agglomerative_complete.png)

---

## 💠 DBSCAN

### PCA & t-SNE
![PCA — DBSCAN](pca_2d_dbscan.png)  
![t-SNE — DBSCAN](tsne_2d_dbscan.png)

### Silhouette, Heatmap & Sizes
![Silhouette — DBSCAN](silhouette_bdscan.png)  
![Confusion Heatmap — DBSCAN](confusion_heatmap_dbscan.png)  
![Cluster Sizes — DBSCAN](cluster_sizes_dbscan.png)

---

## 🎯 Gaussian Mixture Model (GMM)

### Model Selection
![GMM — BIC/AIC vs k](gmm_bic_aic_vs_k.png)  
![GMM — Silhouette vs k](gmm_silhouette_vs_k.png)

### PCA & t-SNE
![PCA — GMM](pca_2d_gmm.png)  
![t-SNE — GMM](tsne_2d_gmm.png)

### Silhouette, Heatmap & Sizes
![Silhouette — GMM](silhouette_gmm.png)  
![Confusion Heatmap — GMM](confusion_heatmap_gmm.png)  
![Cluster Sizes — GMM](cluster_sizes_gmm.png)

---

## 🔷 Spectral Clustering

### PCA & t-SNE
![PCA — Spectral](pca_2d_spectral_clustering.png)  
![t-SNE — Spectral](tsne_2d_spectral_clustering.png)

### Silhouette, Heatmap & Sizes
![Silhouette — Spectral](silhouette_spectral_clustering.png)  
![Confusion Heatmap — Spectral](confusion_heatmap_spectral_clustering.png)  
![Cluster Sizes — Spectral](cluster_sizes_spectral_clustering.png)

---

## 🌐 BIRCH

### PCA & t-SNE
![PCA — BIRCH](pca_2d_birch.png)  
![t-SNE — BIRCH](tsne_2d_birch.png)

### Silhouette, Heatmap & Sizes
![Silhouette — BIRCH](silhouette_birch.png)  
![Confusion Heatmap — BIRCH](confusion_heatmap_birch.png)  
![Cluster Sizes — BIRCH](cluster_sizes_birch.png)

---

## 📡 Mean Shift

### PCA & t-SNE
![PCA — Mean Shift](pca_2d_mean_shift.png)  
![t-SNE — Mean Shift](tsne_2d_mean_shift.png)

### Silhouette, Heatmap & Sizes
![Silhouette — Mean Shift](silhouette_mean_shift.png)  
![Confusion Heatmap — Mean Shift](confusion_heatmap_mean_shift.png)  
![Cluster Sizes — Mean Shift](cluster_sizes_mean_shift.png)

---

## 🧩 Self-Organizing Maps (SOM)

### PCA & t-SNE
![PCA — SOM](pca_2d_som.png)  
![t-SNE — SOM](tsne_2d_som.png)

### Silhouette, Heatmap & Sizes
![Silhouette — SOM](silhouette_som.png)  
![Confusion Heatmap — SOM](confusion_heatmap_som.png)  
![Cluster Sizes — SOM](cluster_sizes_som.png)

---

## 🧮 Model Performance Summary

| Algorithm | Silhouette | ARI | NMI | Purity | FMI |
|----------|-----------:|----:|----:|------:|----:|
| K-Means | 0.460 | 0.620 | 0.659 | 0.833 | 0.745 |
| Hierarchial (Ward) | 0.447 | 0.615 | 0.675 | 0.827 | 0.750 |
| Agglomerative (Complete) | 0.450 | 0.573 | 0.653 | 0.787 | 0.728 |
| DBSCAN | 0.538 | 0.554 | 0.696 | 0.673 | 0.756 |
| GMM | 0.475 | 0.516 | 0.657 | 0.667 | 0.729 |
| Spectral | 0.459 | 0.646 | 0.684 | 0.853 | 0.767 |
| BIRCH | 0.454 | 0.661 | 0.733 | 0.860 | 0.780 |
| Mean Shift | 0.433 | 0.560 | 0.704 | 0.720 | 0.747 |
| SOM | 0.297 | 0.185 | 0.511 | 0.973 | 0.378 |

---

## 🔬 Insights
- **BIRCH** and **Spectral Clustering** show strong external agreement (high ARI/NMI) with excellent purity.  
- **DBSCAN** achieves the **best silhouette** under tuned parameters, capturing non-convex structures.  
- **K-Means** provides a solid baseline with competitive internal metrics.  
- **SOM** preserves topology and yields very high purity but lower ARI (fine-grained neuron mapping).

---

## 🔮 Future Enhancements
- Add **HDBSCAN** and **OPTICS** for advanced density-based clustering  
- Evaluate **ensemble clustering** and **stability indices**  
- Extend to high-dimensional data via **Autoencoder → K-Means** pipeline  
- Provide **interactive dashboards** (Plotly) for parameter exploration

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License




