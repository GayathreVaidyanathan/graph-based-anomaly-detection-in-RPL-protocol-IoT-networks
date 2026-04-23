# 🔐 IoT Intrusion Detection via Graph-Enriched Features

> **Graph-Based Anomaly Detection in RPL-Protocol IoT Networks**  
> Dataset: [UOS-IOTSH-2024](https://github.com/UOSIOTSH2024/UOS_IOTSH_2024-Dataset)

---

## 📌 Overview

This notebook presents a **graph-enriched machine learning pipeline** for detecting routing attacks in IoT networks that use the **RPL (Routing Protocol for Low-Power and Lossy Networks)** protocol.

Traditional intrusion detection systems rely solely on **raw traffic features** (packet length, rank, interval, etc.). This work augments those features with **topological features extracted from network communication graphs**, resulting in a significant improvement in detection accuracy.

### 🔑 Key Contributions
- Construction of **per-scenario communication graphs** from IoT packet traces
- Extraction of **graph-level topological features** (degree stats, clustering coefficient, diameter, betweenness, PageRank)
- A **node2vec embedding pipeline** to encode structural node roles
- Side-by-side comparison: **Baseline (raw features)** vs **Proposed (graph-enriched features)**
- Explainability via **SHAP values** and publication-quality visualizations

### 📊 Headline Results

| Model | Accuracy | ROC-AUC | Attack F1 |
|---|---|---|---|
| Baseline (Raw Traffic Features) | 77.71% | 0.9042 | 0.6303 |
| **Proposed (Graph-Enriched)** | **95.79%** | **0.9934** | **0.9108** |

---

## 🗂️ Table of Contents
1. [Dataset Setup](#1-dataset-setup)
2. [Data Loading & Preprocessing](#2-data-loading--preprocessing)
3. [Graph Construction & Feature Extraction](#3-graph-construction--feature-extraction)
4. [Feature Engineering & Embeddings](#4-feature-engineering--embeddings)
5. [Model Training & Evaluation](#5-model-training--evaluation)
6. [Explainability (SHAP)](#6-explainability-shap)
7. [Final Results & Comparison](#7-final-results--comparison)
8. [Conclusion](#8-conclusion)

---
