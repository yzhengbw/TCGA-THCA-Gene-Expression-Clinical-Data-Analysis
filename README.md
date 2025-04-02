# 🧬 TCGA-THCA Clinical & Gene Expression Analysis Pipeline

This project provides a complete bioinformatics workflow based on the TCGA-THCA (Thyroid Carcinoma) dataset. It integrates clinical metadata and RNA-seq gene expression data to conduct exploratory data analysis (EDA), differential expression analysis (DEA), dimensionality reduction (PCA), clustering, and functional enrichment analysis (GO).

---

## 📁 Dataset

- **Source**: TCGA-THCA dataset(Gained from LinkedOmics)
- **Components**:
  - Clinical data: patient metadata (age, gender, etc.)
  - Gene expression data: RNA-seq (log2 normalized)

---

## 🔧 Tools & Libraries

- **R**: `ggplot2`, `pheatmap`, `dplyr`, `ggrepel`, `DESeq2`
- **Python**: `Pandas`, `NumPy`, `Scikit-learn`, `Matplotlib`, `Seaborn`, `GSEAPY`, `statsmodels`
- Platforms: Google Colab, Jupyter Notebook

---

## 🧪 Workflow Summary

### 1️⃣ Data Cleaning & Preprocessing
- Removed duplicated clinical entries
- Checked and handled missing values
- Aligned sample IDs between clinical and expression datasets

### 2️⃣ Exploratory Data Analysis (EDA)
- Visualized clinical parameters (age, gender distributions)
- Heatmap and distribution plots of gene expression data

### 3️⃣ Dimensionality Reduction
- Applied **PCA** on normalized gene expression data
- Plotted PC1 vs PC2 to reveal variance patterns

### 5️⃣ Clustering
- Used **KMeans clustering** on principal components
- Evaluated clustering performance via silhouette score

### 4️⃣ Differential Expression Analysis (DEA)
- Used **DESeq2** to identify differentially expressed genes (DEGs) between groups
- Volcano plot to visualize log2 fold change vs adjusted p-value
- Extracted top DEGs for downstream analysis

### 6️⃣ GO Enrichment Analysis
- Performed functional enrichment (Gene Ontology) on top DEGs
- Identified overrepresented biological processes and pathways using **GSEApy**

---

## 📊 Key Visualizations

- Barplots, histograms of clinical attributes
- Gene expression heatmaps
- PCA scatter plots
- KMeans clustering plots
- Volcano plot of DEGs
- GO term enrichment bar charts

---

## 💡 Future Improvements

- Integrate survival analysis with clinical data

---

## ✨ Outcome

This project demonstrates a full pipeline for analyzing cancer gene expression data using both R and Python. It showcases skills in bioinformatics preprocessing, statistical analysis, visualization, and biological interpretation — suitable for research and applied data analysis roles.
