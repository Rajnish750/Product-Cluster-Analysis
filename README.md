# Product Cluster Analysis

## Introduction

Welcome to the **Product Cluster Analysis** project.

This project aims to apply unsupervised machine learning techniques to identify **similar product groups based on historical sales patterns**. By clustering products, businesses can make data-driven decisions for inventory planning, promotions, and product bundling strategies.

The insights generated through clustering can help organizations:

- Optimize product stocking based on behavior-driven groupings  
- Tailor marketing strategies to specific product segments  
- Improve operational efficiency and forecasting

---

## Problem Statement

Retail and warehouse environments often handle a wide range of products with diverse sales patterns. Without meaningful segmentation, it becomes challenging to manage inventory and extract actionable insights.

Problems that arise due to lack of product clustering include:

- Overstocking or understocking specific products  
- Generalized marketing strategies that lack personalization  
- Difficulty in understanding product performance at scale

Unsupervised clustering methods provide a way to group products based on underlying sales trends, offering clarity and control over large product datasets.

---

## Objective

The goal of this project is to **cluster similar products** based on their sales behaviors (retail, warehouse, and transfers) using machine learning models. The ultimate aim is to enhance product-level decisions such as:

- Inventory control  
- Assortment planning  
- Category-based pricing and promotion

We will compare multiple clustering techniques to identify the best-performing model for segmenting products in a meaningful way.

---

## Dataset Description

The dataset used in this analysis includes **historical sales data for various product types**. It has been processed to extract statistical features such as mean, sum, and standard deviation for different sales channels.

| Attribute                  | Description                                                    |
|----------------------------|----------------------------------------------------------------|
| `ITEM TYPE`                | Category or name of the product                                |
| `RETAIL_SALES_*`           | Metrics related to sales from retail stores (mean, sum, std)   |
| `RETAIL_TRANSFERS_*`       | Metrics related to retail transfers (mean, sum, std)           |
| `WAREHOUSE_SALES_*`        | Metrics related to warehouse-level sales (mean, sum, std)      |
| `TOTAL_SALES`              | Total sales across all channels                                |
| `SALES_2017` to `SALES_2020`| Year-wise sales data                                          |

Additional columns such as `CLUSTER` and `CLUSTER_NAME` were added after clustering.

---

## Type of Machine Learning Task

This is an **Unsupervised Learning** task, specifically a **Clustering problem**, where the aim is to group products based on similarities in their sales statistics.

The following clustering algorithms are used and compared:

- K-Means  
- Agglomerative Clustering  
- DBSCAN  

Evaluation metrics used for comparison include:

- Silhouette Score  
- Calinski-Harabasz Index  
- Davies-Bouldin Index

Based on the performance metrics, the most appropriate model is selected for final segmentation.

---
