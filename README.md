# 📱 Clustering Mobilephone Sales

**K-Means Clustering Analysis on Smartphone Product Attributes for Market Segmentation**

## 📌 Project Overview

This project aims to analyze and cluster a smartphone product dataset based on attributes such as:

- Brand
- Type
- Storage Capacity
- Warranty
- Price
- Incoming Stock
- Outgoing Stock
- Remaining Stock

By applying **K-Means clustering**, we identify natural groupings of mobile phone products and derive strategic insights for inventory and marketing decisions.

---

## 🗃️ Dataset Summary

- **Total Records**: 100 smartphones
- **Features**:
  - `Merk` (Brand)
  - `Type` (Model)
  - `Penyimpanan` (Storage)
  - `Garansi` (Warranty)
  - `Harga` (Price)
  - `Barang Masuk` (Incoming stock)
  - `Barang Keluar` (Sold stock)
  - `Stok Barang` (Remaining stock)

---

## 🔍 Exploratory Data Analysis

- **No missing or duplicate values**
- Brands include: Xiaomi, Samsung, Oppo, Realme, Vivo, Infinix, Nokia, Meizu
- Prices range from **Rp 205,000** to **Rp 4,800,000**
- Most products have storage between **32GB and 128GB**
- Stock distributions vary by brand and model

---

## ⚙️ Preprocessing & Modeling

- Categorical columns dropped (focus on numerical features)
- Features scaled using `StandardScaler`
- Clustering with `KMeans`
- **Optimal cluster count: 3**, determined using:
  - Elbow Method
  - Silhouette Score
  - Davies-Bouldin Index

---

## 📊 Cluster Evaluation (Sklearn)

| Metric               | Score      |
|----------------------|------------|
| Silhouette Score     | 0.41       |
| Davies-Bouldin Index | 0.91       |

---

## 🧩 Cluster Profiles

### 🔴 Cluster 0 (21 products)
- Moderate price
- Moderate storage (32–64GB)
- Mid-to-high stock levels
- Mass-market, budget-friendly models (Xiaomi, Realme, Infinix)

### 🟡 Cluster 1 (28 products)
- Higher prices (up to Rp 4.8M)
- High storage (mostly 128GB)
- Lower stock levels
- Premium models (Samsung A52, Oppo Reno 4, Vivo V20)

### 🔵 Cluster 2 (51 products)
- Affordable prices (under Rp 2.3M)
- Mixed storage (32–64GB)
- Balanced stock levels
- Popular and legacy models for price-sensitive buyers

---

## 📈 Alternative Models

Tested `pyclustering` with:
- **Euclidean** and **Manhattan** distance
- Best silhouette score (Manhattan): **0.50**
- Reinforces 3-cluster structure

---

## 💡 Business Insights & Recommendations

1. **Cluster 0**  
   Target mass-market customers via volume discounts and bundle offers.

2. **Cluster 1**  
   Highlight premium features and exclusive services. Push via flagship stores and influencer campaigns.

3. **Cluster 2**  
   Position for entry-level and budget-conscious customers. Use clearance sales or student promotions.

---

## 🧰 Tools & Libraries

- Python
- pandas, numpy
- sklearn
- matplotlib, seaborn
- yellowbrick
- pyclustering

---

## ✍️ Author

**Alexander Tiopan**  
📫 alexandertiopan1212@gmail.com  
🔗 GitHub: [alexandertiopan1212](https://github.com/alexandertiopan1212)

