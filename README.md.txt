# Detection of Criminal Communication Networks in the Enron Accounting Fraud using BERTopic and Graph Neural Networks

## Overview

This project presents an intelligent graph-based framework for detecting criminal communication networks within the Enron Email Dataset. The proposed framework combines semantic topic modelling using **BERTopic**, graph feature engineering, **Graph Neural Networks (GCN, GraphSAGE, GAT, and TAGCN)**, and community detection techniques to identify criminal employees and suspicious communication communities.

Unlike traditional approaches that analyze either email content or communication structure independently, this framework integrates both semantic and structural information to improve the accuracy and interpretability of fraud detection.

---

## Problem Statement

Detecting criminal communication networks within large-scale organizational email datasets is challenging due to the massive volume of legitimate communications, complex employee interactions, and the highly imbalanced distribution of criminal and non-criminal instances.

This project addresses these challenges by integrating BERTopic, graph representation learning, Graph Neural Networks, and community detection techniques into a unified framework for criminal communication analysis.

---

## Objectives

* Preprocess and clean the Enron Email Dataset.
* Extract semantic communication topics using BERTopic.
* Generate employee-level graph features using communication statistics, centrality measures, Node2Vec embeddings, and topic-based information.
* Construct an employee communication graph.
* Compare multiple Graph Neural Network models (GCN, GraphSAGE, GAT, and TAGCN).
* Detect suspicious communication communities using Louvain Community Detection and Spectral Clustering.
* Interpret dominant communication topics within suspicious communities.

---

## Methodology

```text
Enron Email Dataset
        │
        ▼
Data Preprocessing
        │
        ▼
Feature Engineering
        │
        ▼
BERTopic-based Topic Modelling
        │
        ▼
Communication Graph Construction
        │
        ▼
Graph Neural Network Models
(GCN | GraphSAGE | GAT | TAGCN)
        │
        ▼
Model Performance Evaluation
        │
        ▼
Community Detection
(Louvain & Spectral Clustering)
        │
        ▼
Suspicious Community Analysis
```

---

## Technologies Used

* Python
* Pandas
* NumPy
* NetworkX
* BERTopic
* Sentence-BERT
* UMAP
* K-Means
* Node2Vec
* Scikit-learn
* PyTorch
* PyTorch Geometric
* GCN
* GraphSAGE
* GAT
* TAGCN

---

## Results

* Successfully generated semantic communication topics using BERTopic.
* Constructed an employee communication graph with engineered node features.
* Evaluated GCN, GraphSAGE, GAT, TAGCN, and KNN models for criminal node classification.
* TAGCN achieved the most balanced overall performance based on Accuracy, Precision, Recall, F1-score, Matthews Correlation Coefficient (MCC), and False Positive Rate.
* Identified suspicious communication communities using the Louvain Algorithm and Spectral Clustering.
* Integrated BERTopic with detected communities to interpret the dominant communication topics within suspicious groups.

---

## Repository Structure

```text
enron-criminal-communication-network-detection/
│
├── notebooks/
│   ├── 01_Data_Preprocessing.ipynb
│   └── 02_BERTopic_GNN_Framework.ipynb
│
├── report/
│   └── Enron_Criminal_Communication_Network_Detection_Report.pdf
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

## Future Scope

* Incorporate temporal graph neural networks for dynamic communication analysis.
* Explore explainable Graph Neural Networks for model interpretability.
* Extend the framework to other organizational communication datasets.
* Investigate heterogeneous graph neural networks for richer relationship modelling.

---

## Author

**Hanan Fathima K**

B.Tech Computer Science
