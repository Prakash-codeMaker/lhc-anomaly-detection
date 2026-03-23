# 🔬 Anomaly Detection in LHC Collision Data using Machine Learning

## 📌 Overview

This project applies machine learning techniques to detect anomalies in particle collision data inspired by experiments at CERN's Large Hadron Collider (LHC).

The goal is to build a scalable and efficient anomaly detection system capable of identifying unusual patterns in high-energy physics data, which is critical for discovering rare events and monitoring system behavior.

---

## 🚀 Motivation

Experiments at CERN generate **petabytes of data** from particle collisions. Analyzing this data requires:

- High computational resources  
- Efficient data processing pipelines  
- Robust anomaly detection systems  

Traditional approaches such as Monte Carlo simulations are accurate but computationally expensive.

This project explores how **machine learning models can accelerate analysis and detect anomalies efficiently**, making them highly relevant for modern scientific computing.

---

## 🧠 Problem Statement

Detect anomalous events in particle collision datasets using unsupervised machine learning techniques.

---

## ⚙️ Methodology

### 1. Data Generation / Loading
- Simulated LHC-like dataset with features:
  - Transverse momentum (`pt`)
  - Pseudorapidity (`eta`)
  - Azimuthal angle (`phi`)
  - Energy
  - Mass

- Dataset size: **100,000+ samples**

---

### 2. Exploratory Data Analysis (EDA)

- Feature distribution plots  
- Correlation heatmap  
- Pairwise relationships  

---

### 3. Data Preprocessing

- Feature normalization using `StandardScaler`  
- Train-test split (80/20)  

---

### 4. Models Implemented

#### 🔹 Isolation Forest
- Tree-based anomaly detection  
- Identifies outliers based on feature distribution  

#### 🔹 Autoencoder (PyTorch)
- Neural network-based anomaly detection  
- Uses reconstruction error to identify anomalies  

Architecture:
Input → Dense → ReLU → Dense → Latent Space → Decoder → Output


---

### 5. Anomaly Detection

- Reconstruction error used as anomaly score  
- Threshold-based anomaly classification  

---

### 6. Evaluation

Since labels are not available:

- Distribution of anomaly scores  
- Separation of normal vs anomalous points  
- Visualization using PCA / scatter plots  

---

### 7. Performance Benchmark

To simulate real-world conditions:

- Compared ML inference with a computationally heavy function (Monte Carlo-like)

**Result:**
- Machine Learning model significantly faster than traditional computation  
- Demonstrates scalability for large datasets  

---

## 📊 Results

- Effective anomaly detection using unsupervised learning  
- Clear separation of anomalous patterns  
- High computational efficiency  

### Key Highlights:

- Scalable pipeline for large datasets  
- Fast inference compared to traditional simulation  
- Reproducible ML workflow  

---

## 📈 Visualizations

### Correlation Heatmap
![Heatmap](images/heatmap.png)

### Anomaly Detection
![Anomaly Plot](images/anomaly_plot.png)

### Feature Distribution
![Distribution](images/distribution.png)

---

## 🧪 Technologies Used

- Python  
- NumPy, Pandas  
- scikit-learn  
- PyTorch  
- Matplotlib, Seaborn  
- Uproot (for ROOT data support)  

---


---

## 🌍 Relevance to CERN

This project reflects key computing challenges at CERN:

- Large-scale data processing  
- anomaly detection in distributed systems  
- efficient analysis of particle collision data  

Machine learning-based approaches like this can:

- reduce computational cost  
- accelerate simulation workflows  
- improve detection of rare physics events  

---

## 🔮 Future Work

- Use real CERN Open Data (ROOT files)  
- Implement distributed processing using Dask or Spark  
- Apply advanced models (GANs, Variational Autoencoders)  
- Integrate real-time anomaly detection dashboards  

---

## 👨‍💻 Author

**Prakash Chand Jain**  
- 📍 Pune, India  
- 💼 Software Engineering | AI | Scientific Computing  
- 🔗 GitHub | LinkedIn | Portfolio  

---

## ⭐ Acknowledgment

Inspired by computing challenges in high-energy physics and large-scale data analysis at CERN.

