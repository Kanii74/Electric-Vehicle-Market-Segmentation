# EV Segmentation Analysis

This repository contains a **data-driven market segmentation study of the Electric Vehicle (EV) market in India**, performed using **Python and machine learning techniques**.

The goal of the project is to analyze the **2-Wheeler Electric Vehicle market**, identify potential **customer segments**, and determine which segment would be the most **strategically promising for a new EV startup**.

The study applies **unsupervised machine learning techniques**, particularly **K-Means clustering**, to divide the EV market into meaningful customer segments. :contentReference[oaicite:1]{index=1}

---

# Project Overview

Electric vehicles are rapidly transforming the global transportation industry. In India, the **2-wheeler EV segment** has experienced the **highest adoption rates and market growth in recent years**.

For a startup entering the EV market, one of the most important strategic questions is:

**Which customer segment should the company target first?**

This project attempts to answer that question by performing **market segmentation analysis using machine learning**.

By analyzing available EV market datasets, this study identifies **distinct customer segments**, evaluates their characteristics, and determines the **most promising segment for an EV startup to target**.

---

# Objectives

The main objectives of this project are:

- Perform a **data-driven study of the Electric Vehicle market in India**
- Apply **machine learning segmentation techniques**
- Identify **distinct market segments**
- Determine the **optimal number of customer clusters**
- Identify the **most promising segment for a new EV startup**

---

# Dataset

The datasets used in this project were collected from **multiple publicly available online sources**. Significant effort was invested in **finding, extracting, and preparing these datasets for analysis**. :contentReference[oaicite:2]{index=2}

The dataset contains variables describing aspects of the EV market such as:

- customer demographics
- purchasing preferences
- vehicle usage patterns
- market demand indicators
- EV adoption trends

The focus of the analysis is specifically on the **2-Wheeler Electric Vehicle market**, which currently dominates EV adoption in India.

---

# Methodology

The segmentation process follows a standard **machine learning workflow**.

## 1 Data Preparation

The raw data is first cleaned and structured into a feature matrix:

$$
X =
\begin{bmatrix}
x_{11} & x_{12} & \dots & x_{1p} \\
x_{21} & x_{22} & \dots & x_{2p} \\
\vdots & \vdots & \ddots & \vdots \\
x_{n1} & x_{n2} & \dots & x_{np}
\end{bmatrix}
$$

where

- $n$ = number of observations  
- $p$ = number of variables describing each observation

This matrix becomes the input for clustering algorithms.

---

## 2 Market Segmentation using K-Means Clustering

To identify customer segments, the **K-Means clustering algorithm** is used.

K-Means partitions the dataset into $k$ clusters by minimizing the **within-cluster variance**:

$$
J = \sum_{i=1}^{k} \sum_{x \in C_i} ||x - \mu_i||^2
$$

where:

- $k$ = number of clusters  
- $C_i$ = cluster $i$  
- $\mu_i$ = centroid of cluster $i$

The algorithm iteratively:

1. Assigns each observation to the nearest cluster centroid  
2. Recomputes cluster centroids  
3. Repeats until convergence

---

## 3 Determining the Optimal Number of Segments

The segmentation analysis found that the **optimal number of clusters was 4**.

Thus, the market was divided into the following segments:

- Segment 0
- Segment 1
- Segment 2
- Segment 3

Each segment represents a **distinct group of EV customers with similar characteristics**.

---

# Key Findings

The segmentation analysis revealed several important insights:

- The **2-Wheeler EV segment is currently the most active part of the EV market**
- The EV market can be divided into **four meaningful customer segments**
- Among these clusters, **Segment 1 emerged as the most opportunistic market segment for the startup**. :contentReference[oaicite:3]{index=3}

This segment represents the **most favorable combination of demand, adoption potential, and market opportunity**.

---

# Visualization

Several plots were generated in the analysis to visualize the segmentation results.

These visualizations help in understanding:

- how clusters are distributed
- how different variables influence segment membership
- how the market structure is organized

Visualization techniques include:

- cluster scatter plots
- segmentation comparison plots
- cluster distribution graphs

These plots make it easier to interpret the **structure of the EV market segments**.

---

# Repository Structure

```
EV-Segmentation-Analysis
│
├── EV Code.ipynb
│   Jupyter notebook containing the Python implementation
│   of the segmentation analysis
│
├── Electric_Vehicle_Startup___Kanishka.pdf
│   Detailed report explaining the EV market study
│   and segmentation results
│
└── README.md
    Project documentation
```

---

# Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

# Applications

This analysis can help guide **strategic decisions for EV startups**, including:

- identifying **target customer groups**
- designing **market entry strategies**
- optimizing **product positioning**
- understanding **consumer adoption behavior**

Market segmentation is a critical tool for **building successful mobility startups in emerging EV markets**.

---

# Disclaimer

This project was carried out for **educational and analytical purposes** to demonstrate the use of **machine learning techniques for market segmentation in the EV industry**.
