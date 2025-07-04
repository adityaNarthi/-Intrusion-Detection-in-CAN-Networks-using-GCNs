# 🚗 Intrusion Detection in CAN Networks using Graph Convolutional Networks (GCNs)


This project proposes a graph-based approach for detecting cyber-attacks on Controller Area Networks (CAN), the core communication protocol in modern vehicles. We benchmark a customized Graph Convolutional Network (GCN) model against temporal and classical machine learning baselines, demonstrating the superiority of spatial graph learning in structured vehicular data.

---

## 🔍 Project Overview

CAN networks, despite being widely adopted in automotive systems, are inherently vulnerable to various attacks like DoS, Fuzzy, and Impersonation due to their lack of built-in security. This project addresses the problem by:

- Converting raw CAN messages into structured temporal graphs
- Using **Graph Convolutional Networks (GCNs)** for multi-class intrusion detection
- Comparing GCN performance with **TGAT**, **Random Forest**, and **MLP** models
- Achieving a **99.99% accuracy** using GCN, far outperforming other approaches

---

## 🧠 Key Contributions

- ⚙️ **29-dimensional feature engineering** from raw CAN frames (temporal, statistical, and byte-level features)
- 🧱 **Graph construction** from temporal message windows with nearest-neighbor edge creation
- 🕸️ **GCN architecture** built with PyTorch Geometric for graph-level classification
- 📊 Comprehensive benchmarking of:
  - **GCN**: 99.99% Accuracy
  - **TGAT**: 84.10%
  - **Random Forest**: 92.30%
  - **MLP**: 88.60%
- 📈 Detailed evaluation via classification reports, confusion matrices, and ablation studies

---

## 📦 System Pipeline

1. **Raw CAN Data** (from OTIDS dataset)
2. ➡️ **Feature Engineering** (timestamp deltas, entropy, ID encoding, etc.)
3. ➡️ **Graph Generation** (based on message proximity and structure)
4. ➡️ **Model Training** (GCN, TGAT, RF, MLP)
5. ➡️ **Intrusion Classification** (Normal, DoS, Fuzzy, Impersonation)
6. ➡️ **Evaluation & Visualization**

---

## 🧪 Dataset Used

- **OTIDS CAN Dataset**
  - 4 attack types: Normal, Denial-of-Service, Fuzzy, Impersonation
  - Total of 4.6M labeled messages
  - Balanced subset of **20,000 messages** used for model training and evaluation

---

## 🛠️ Technology Stack

- 📦 **Frameworks**: PyTorch, PyTorch Geometric, Scikit-learn
- 🧮 **Models**: GCN, TGAT, Random Forest, MLP
- 📊 **Evaluation**: Accuracy, Precision, Recall, F1-score, Confusion Matrix
- 🖥️ **Environment**: Google Colab with Tesla T4 GPU

---

## 📊 Results Snapshot

| Model          | Accuracy | Precision | Recall | F1-Score |
|----------------|----------|-----------|--------|----------|
| **GCN**        | **99.99%** | 1.00      | 1.00   | 1.00     |
| Random Forest  | 92.30%   | 0.92      | 0.92   | 0.92     |
| MLP            | 88.60%   | 0.89      | 0.89   | 0.88     |
| TGAT           | 84.10%   | 0.83      | 0.84   | 0.83     |

---



## 📬 Contact

For questions, collaborations, or citations:

- 📧 Email: [anarthi2004@gmail.com]
- 🔗 LinkedIn: [linkedin.com/in/yourprofile](linkedin.com/in/aditya-narthi-2523a42a2/)

---

⭐ **If you found this work insightful, feel free to star the repo or cite our paper!**
