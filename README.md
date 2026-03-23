# 🌍 Grouping Countries for Tourism Investment Using Unsupervised Learning

An unsupervised machine learning project that groups 229 countries into
distinct tourism investment categories based on socioeconomic, technological,
and environmental indicators.

---

## 👤 Author

**Takunda Manhongo** | Student ID: R2418440
BSc Data Science & Systems — University of Zimbabwe
📧 takundamanhongo16@gmail.com
🔗 Portfolio: https://takundamanhongo.github.io

---

## 🎯 Objectives

1. Clean and prepare country statistics using KNN Imputation
2. Select 14 meaningful features capturing economic, social, and tech profiles
3. Apply K-Means Clustering to partition countries into investment groups
4. Apply Hierarchical Clustering to independently validate the groupings
5. Compare both algorithms using internal evaluation metrics
6. Visualise cluster separation using PCA dimensionality reduction
7. Translate cluster findings into actionable tourism investment strategies

---

## 📁 Dataset

**File:** `country_stats.csv`
**Source:** UCI Machine Learning Repository
**Records:** 229 countries | **Features:** 22

| Feature | Description |
|---|---|
| Population & Density | Scale and urbanisation |
| GDP | Overall economic size |
| Economy: Agriculture / Industry / Services | Economic structure |
| International Trade: Exports / Imports | Global integration |
| Health & Education Expenditure | Social development |
| Mobile & Internet Usage | Technology adoption |
| CO2 Emissions & Energy Production | Environmental profile |

> Note: Missing values encoded as -99 and ... are replaced with NaN
> and filled using KNN Imputation before analysis.

---

## 🤖 Algorithms Used

| Algorithm | Role | Purpose |
|---|---|---|
| KNN Imputation | Supporting | Fill missing values using country similarity |
| K-Means Clustering | Main | Partition countries by minimising WCSS |
| Hierarchical Clustering | Main | Build dendrogram of country relationships |
| PCA | Supporting | Reduce 14 features to 2D for visualisation |

---

## 📊 Key Results

### K-Means (K=3) Evaluation
| Metric | Score | Interpretation |
|---|---|---|
| Silhouette Score | 0.1873 | Moderate separation |
| Davies-Bouldin Index | 1.4115 | Reasonable compactness |
| Calinski-Harabasz | 62.43 | Good cluster density ratio |

### Cluster Profiles

| Cluster | Label | Countries | Key Characteristics |
|---|---|---|---|
| 0 | Emerging Experience Seekers | 98 | Developing economies, higher agriculture, lower tech |
| 1 | Densely Developed Discoveries | 2 | High-density, service-oriented, moderate-high GDP |
| 2 | Global Tourist Magnets | 129 | Large economies, high trade, advanced technology |

### Tourism Investment Strategy

| Cluster | Investment Focus | Target Market |
|---|---|---|
| 0 | Eco-tourism, infrastructure, community-based | Budget, adventure, cultural explorers |
| 1 | Niche urban tourism, MICE, history | Business, short-stay, urban explorers |
| 2 | Mass & luxury tourism, digital marketing | All segments, high-value travellers |

---

## 📈 Visualisations Produced

| Plot | Description |
|---|---|
| Correlation Heatmap | Feature relationships before clustering |
| Feature Distributions | Histograms of all 14 features |
| Regional Overview | Countries and GDP by region |
| Elbow Method | Optimal K selection via WCSS |
| K-Means Metrics | Silhouette, Davies-Bouldin, Calinski-Harabasz across K values |
| Silhouette Plots | Per-country silhouette coefficients for both algorithms |
| Full Dendrogram | All 229 countries in Ward linkage tree |
| Truncated Dendrogram | Top 30 merges for clarity |
| Linkage Comparison | Ward vs Complete vs Average dendrograms |
| Algorithm Comparison | Side-by-side metric bar charts |
| PCA Scatter Plots | Both algorithms visualised in 2D |
| PCA Loadings | Feature contributions to PC1 and PC2 |

---

## 🚀 How to Run

1. Clone the repository:
   git clone https://github.com/takundamanhongo/tourism-clustering
   cd tourism-clustering

2. Install dependencies:
   pip install pandas numpy matplotlib seaborn scikit-learn scipy jupyter

3. Launch Jupyter Notebook:
   jupyter notebook tourism_clustering.ipynb

4. Run all cells:
   Kernel -> Restart & Run All

---

## 📌 Academic Context

Developed as part of the Machine Learning module
BSc Data Science & Systems — University of Zimbabwe | 2026
```

---

