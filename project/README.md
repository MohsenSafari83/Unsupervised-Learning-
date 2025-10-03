
# Customer Segmentation — Marketing Campaign

**Summary:**  
This repository contains the complete project for **Customer Segmentation** using a marketing campaign dataset. The goal is to identify distinct customer groups to enable targeted and more effective marketing strategies.

---

## Project Overview
- **Method:** K-Means Clustering  
- **Dataset:** 2,240 records, 29 attributes (demographics, purchasing behavior, channels, promotion engagement)  
- **Optimal Clusters:** **k = 4** (selected via Elbow Method)  
- **Visualization:** PCA reduced to 2 components (for visualization only)

---

## Dataset Summary (Features)
- **Customer Information:** `Income`, `Year_Birth`, `Education`, `Marital_Status`, `Kidhome`, `Teenhome`, `Dt_Customer`, `Recency`  
- **Product Spending (last 2 years):** `MntWines`, `MntMeatProducts`, `MntFruits`, `MntFishProducts`, `MntSweetProducts`, `MntGoldProds`  
- **Purchasing Channels:** `NumWebPurchases`, `NumCatalogPurchases`, `NumStorePurchases`, `NumWebVisitsMonth`  
- **Promotion Engagement:** `NumDealsPurchases`, `AcceptedCmp1` … `AcceptedCmp5`, `Response`  

---

## Methodology
1. **Data Cleaning & Preprocessing**
   - Missing `Income` values imputed with the median.  
   - Feature engineering: derived `Age` from `Year_Birth`, simplified `Marital_Status` → (Relationship / Single).  
   - Encoding: `LabelEncoder` for categorical variables.  
   - Scaling: `StandardScaler` applied to all features.  

2. **Clustering**
   - Cluster selection: Elbow Method → **k = 4**.  
   - Applied **K-Means (k=4)** to assign cluster labels.  

3. **Dimensionality Reduction**
   - **PCA** used after clustering to visualize data in 2D space (PC1, PC2).  

4. **Cluster Profiling**
   - Mean of standardized features computed per cluster.  
   - Profiles created to guide actionable marketing strategies.  

---

## Final Cluster Profiles (4 Segments)

| Cluster | Profile Summary | Marketing Strategy |
|--------:|----------------|---------------------|
| **0** | Low-income families with children (High Kidhome/Teenhome, low income, lowest spending). | Focus on discounts and budget-friendly product lines. |
| **1** | Medium-low income families with teens (slightly below-average income, higher Teenhome, overall low spending). | Use price-sensitive promotions and value offers. |
| **2** | High-income luxury buyers (very high income, heavy spenders on wines/gold, few/no children). | Target with premium product marketing and exclusive offers. |
| **3** | Medium-high income multi-channel shoppers (active in both web & store, moderate-to-high income, solid overall spending). | Implement cross-channel marketing, loyalty programs, and bundled promotions. |


---

### Elbow Method
![Elbow Method](https://github.com/MohsenSafari83/Unsupervised-Learning-/blob/main/project/images/elbow.png?raw=true)

### PCA Visualization
![PCA Clusters](https://github.com/MohsenSafari83/Unsupervised-Learning-/blob/main/project/images/pca_clusters.png?raw=true)

### Cluster Profiles Heatmap
![Cluster Profiles](https://github.com/MohsenSafari83/Unsupervised-Learning-/blob/main/project/images/cluster_profiles_heatmap.png?raw=true)

### Example Feature Barplots
![Income by Cluster](https://github.com/MohsenSafari83/Unsupervised-Learning-/blob/main/project/images/bar_income.png?raw=true)
![MntWines by Cluster](https://github.com/MohsenSafari83/Unsupervised-Learning-/blob/main/project/images/bar_mntwines.png?raw=true)
