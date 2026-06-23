# Network-Based Customer Segmentation

This repository contains the Python implementation for a customer segmentation study based on the Instacart Online Grocery Basket Analysis Dataset. The aim of the study is to compare three different customer segmentation approaches and examine how they differ in the customer segments and business insights they reveal.

The compared approaches are:

- RFM-based K-Means clustering
- Louvain-based community detection
- Autoencoder-based K-Means clustering

In addition, a cohort-based retention analysis is conducted to further examine customer activity.

## Dataset

This study uses the Instacart Online Grocery Basket Analysis Dataset, which contains anonymized transaction data from an online grocery platform. The dataset includes information on orders, products, aisles, departments, and customer purchase histories.

The dataset is publicly available on [Kaggle](https://www.kaggle.com/datasets/yasserh/instacart-online-grocery-basket-analysis-dataset/data).

The raw dataset files are not included in this repository and need to be downloaded separately from Kaggle.

## Repository Structure

```text
.
├── figures/
├── 01_data_understanding_preprocessing_cohort_analysis.ipynb
├── 02_rfm_kmeans_segmentation.ipynb
├── 03_louvain_segmentation.ipynb
├── 04_autoencoder_kmeans_segmentation.ipynb
├── 05_results_and_comparison.ipynb
└── README.md
```

## Notebook Overview

### 01_data_understanding_preprocessing_cohort_analysis.ipynb

In this notebook, the dataset is introduced, exploratory data analysis is performed, initial preprocessing steps are applied, and a cohort-based retention analysis is conducted.

### 02_rfm_kmeans_segmentation.ipynb

In this notebook, the RFM-based K-Means segmentation approach is implemented. 

### 03_louvain_segmentation.ipynb

In this notebook, the Louvain-based segmentation approach is implemented. 

### 04_autoencoder_kmeans_segmentation.ipynb

In this notebook, the autoencoder-based K-Means approach is implemented. 

### 05_results_and_comparison.ipynb

In this notebook, the generated cohort labels and segmentation results from the previous notebooks are combined, and the methods are compared.

## Results Summary

The results show that the three methods reveal different but complementary perspectives on the same customer base. RFM-based K-Means mainly captures differences in purchasing activity and average order size. Louvain-based community detection identifies more distinct aisle-level preference communities. The autoencoder-based K-Means approach, although based on aisle-level purchase behavior, separates customers mainly by overall purchasing activity.

Overall, the approaches should not be viewed as direct substitutes, but as complementary analytical perspectives for customer segmentation.
