### Microbiome-Metabolome Integration with AnnData

This repository aims to contain a suite of comprehensive Jupyter Notebooks demonstrating advanced workflows for integrating, manipulating, and analyzing multi-omics datasets with an emphasis on Microbiome and Metabolome datasets using the **AnnData** ecosystem in Python. 

The pipeline utilizes real multi-omics clinical data investigating the impact of gastrectomy on microbial and metabolic compositions ([Gut Journal, 2020;10.1136/gutjnl-2019-319188](https://gut.bmj.com/content/69/11/1971)). 

### 💡 Why AnnData for Multi-Omics?

Managing high-dimensional data across disparate dataframes often leads to fragmented scripts and reproducibility challenges. AnnData provides a standard, unified architecture that simplifies this process: 

* **Unified Object Model:** Bind feature matrices (.X), sample metadata (.obs), feature annotations (.var), and multi-dimensional embeddings (.obsm/.uns) in a single, easily sliceable container.
* **Native Ecosystem Interoperability:** Anndata is natively implemented in gold-standard tools such as pylimma or pyDESeq2
* **Reproducibility & Workflow Tracking:** Keeps track of raw, normalized, and transformed states across the distinct phases of your workflow.  

### 🛠️ Main Features & Custom Wrappers

The core of this repository includes illustrations of Anndata covering: 

* **Dimensionality Reduction:** Automated Principal Component Analysis (PCA) and Principal Coordinate Analysis (PCoA) extraction.
* **Ecological Diversity:** Smooth calculations for **Alpha Diversity** (e.g., Shannon index) and **Beta Diversity** distance matrices.
* **Compositional Analysis:** Integrated differential abundance benchmarking for microbiome count data using ANCOM-BC equations.
* **Linear Modeling:** Direct processing pipelines for differential abundance profiling using pylimma.

Additional custom functions are provided to interact Anndata with the skbio ecosystem. 

### 📦 Required Stack

Make sure you have the following packages installed to execute the notebooks: 

```bash

pip install anndata pandas numpy scikit-bio scikit-learn plotnine seaborn pylimma statsmodels

```
