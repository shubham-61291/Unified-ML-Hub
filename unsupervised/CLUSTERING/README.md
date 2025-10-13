# 🧠 Clustering — K-Means, Hierarchical, DBSCAN, GMM, Spectral & Advanced Models

The **Clustering** project implements and compares multiple unsupervised learning algorithms — both classical and advanced — to identify hidden patterns in unlabeled data.  
It covers **K-Means, Hierarchical Clustering, DBSCAN, GMM, Spectral, BIRCH, Mean Shift, and SOM**, with complete evaluation, visualization, and metric-based validation.

---

## 🚀 Key Highlights
✅ Implementation of 8 major clustering algorithms  
✅ Comprehensive evaluation using Silhouette, ARI, NMI, Purity, and FMI  
✅ Parameter tuning via Elbow, Gap Statistic, and DBSCAN sweep  
✅ Rich visualization suite — PCA, t-SNE, Dendrograms, Silhouette plots  
✅ Unified evaluation framework with internal & external metrics  
✅ Automatic comparison of all models across metrics  

---

## 📊 K-Means Clustering

### Elbow Method  
![K-Means Elbow](k_means_elbow.png)

### Cluster Visualization (PCA Projection)  
![K-Means PCA](tsne_2d_k_means.png)

### Silhouette Plot  
![K-Means Silhouette](silhouette_k_means.png)

---

## 🌲 Hierarchical Clustering

### Dendrogram (Ward Linkage)  
![Hierarchical Dendrogram Ward](hierarchial_dendrogram_ward.png)

### Silhouette Plot  
![Silhouette Ward](silhouette_hierarchial_ward.png)

### Cluster Visualization (PCA Projection)  
![Ward t-SNE](tsne_2d_hierarchial_ward.png)

---

## 💠 DBSCAN

### eps–min_samples Sweep  
![DBSCAN Sweep](dbscan_eps_sweep.png)

### Cluster Visualization (t-SNE)  
![DBSCAN t-SNE](tsne_2d_dbscan.png)

### Silhouette Plot  
![DBSCAN Silhouette](silhouette_dbscan.png)

---

## 🎯 Gaussian Mixture Model (GMM)

### BIC vs AIC Comparison  
![GMM BIC AIC](gmm_bic_aic.png)

### Cluster Visualization  
![GMM t-SNE](tsne_2d_gmm.png)

### Silhouette Plot  
![GMM Silhouette](silhouette_gmm.png)

---

## 🔷 Spectral Clustering

### Cluster Visualization (t-SNE)  
![Spectral t-SNE](tsne_2d_spectral_clustering.png)

### Silhouette Plot  
![Spectral Silhouette](silhouette_spectral_clustering.png)

---

## 🌐 BIRCH & Mean Shift

### Cluster Visualization (BIRCH)  
![BIRCH t-SNE](tsne_2d_birch.png)

### Cluster Visualization (Mean Shift)  
![Mean Shift t-SNE](tsne_2d_meanshift.png)

---

## 🧩 Self-Organizing Map (SOM)

### SOM t-SNE Visualization  
![SOM Visualization](tsne_2d_som.png)

### SOM Cluster Map  
![SOM Cluster Map](som_cluster_map.png)

---

## 🧮 Model Performance Summary

| Algorithm | Silhouette | ARI | NMI | Purity | FMI |
|------------|-------------|-----|-----|--------|------|
| K-Means | 0.460 | 0.620 | 0.659 | 0.833 | 0.690 |
| Hierarchical (Ward) | 0.447 | 0.615 | 0.675 | 0.827 | 0.681 |
| DBSCAN | 0.538 | 0.554 | 0.696 | 0.673 | 0.660 |
| GMM | 0.475 | 0.516 | 0.657 | 0.667 | 0.643 |
| Spectral | 0.459 | 0.646 | 0.684 | 0.853 | 0.700 |
| BIRCH | 0.454 | 0.661 | 0.733 | 0.860 | 0.708 |
| Mean Shift | 0.433 | 0.560 | 0.704 | 0.720 | 0.672 |
| SOM | 0.421 | 0.590 | 0.720 | 0.735 | 0.689 |

---

## 🔬 Insights

- **BIRCH** and **Spectral Clustering** deliver the best balance between accuracy and interpretability.  
- **DBSCAN** shows strong performance on complex, non-linear clusters due to density-based logic.  
- **K-Means** remains a reliable baseline with stable, circular boundaries.  
- **SOM** captures topology-preserving patterns and serves as a neural analog to traditional clustering.  

---

## 🔮 Future Enhancements

- Integrate **HDBSCAN** and **OPTICS** for density-based hierarchical clustering  
- Extend to **high-dimensional datasets** (e.g., MNIST via Autoencoders)  
- Add **ensemble clustering** and **meta-cluster stability** metrics  
- Deploy interactive visualization dashboards via **Plotly Dash**  

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License


