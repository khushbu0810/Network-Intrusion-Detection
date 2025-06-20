# 🛡️ Network Intrusion Detection System using Machine Learning

Welcome to **Network Intrusion Detection System (NIDS)** — a machine learning-based project that identifies and classifies malicious network traffic using the **NSL-KDD** dataset. This system aims to strengthen cybersecurity by detecting various types of attacks like DoS, Probe, R2L, and U2R.

> 📁 GitHub Repository: https://github.com/khushbu0810/Network-Intrusion-Detection

---

## 📌 Project Overview

This project applies machine learning models to analyze network traffic and detect intrusions. The goal is to differentiate between normal and attack traffic with high accuracy using a clean and balanced dataset and well-engineered features.

### 🔍 Dataset: NSL-KDD

- NSL-KDD is a refined version of the KDD Cup 1999 dataset, created to remove redundant records and balance the classes.
- Contains 41 features and a target label (`attack_class`).
- Types of attacks:
  - **DoS (Denial of Service)**
  - **Probe**
  - **R2L (Remote to Local)**
  - **U2R (User to Root)**

---

## ⚙️ Workflow Summary

1. **Data Preprocessing**
   - Handle missing values (if any)
   - Encode categorical features: `proto`, `state`
   - Feature scaling for numerical data

2. **Balancing the Dataset**
   - Applied **SMOTE** from `imblearn` to handle class imbalance

3. **Model Training**
   - Trained multiple machine learning models:
     - Random Forest
     - Decision Tree
     - K-Nearest Neighbors
     - Logistic Regression

4. **Evaluation Metrics**
   - Accuracy
   - Precision
   - Recall
   - F1-Score
   - Confusion Matrix

## 💡 Key Takeaways

- Preprocessing steps (encoding + scaling) are essential for ML performance.
- Handling class imbalance improves recall and precision on minority attacks.
- Random Forest consistently outperforms simpler classifiers in detection accuracy.
- NIDS solutions should aim for low false positives to avoid alert fatigue in real-world systems.

---

## 🧪 Results

| Model               | Accuracy | Precision | Recall | F1-Score |
|--------------------|----------|-----------|--------|----------|
| Random Forest       | ✅ High  | ✅ High    | ✅ High| ✅ High   |
| Decision Tree       | Good     | Good      | Good   | Good     |
| K-Nearest Neighbors | Moderate | Moderate  | Moderate| Moderate|
| Logistic Regression | Lower    | Lower     | Lower  | Lower    |

> 📌 These are general observations. Exact metrics can be found in the notebook.

---

## 🚀 Future Enhancements

- 🧠 Use Deep Learning models like CNN, LSTM, or Autoencoders
- 🧪 Test on other datasets (e.g., UNSW-NB15, CICIDS2017)
- 🌐 Real-time packet inspection using Scapy
- 📊 Build a Streamlit or Flask-based UI for live predictions
- 🛡️ Integrate into a firewall or SIEM system for proactive security

---

## 🙋‍♀️ About the Author

**Khushbu Rani**  
B.Tech CSE Student @ VIT  
Machine Learning Enthusiast  
GitHub: [@khushbu0810](https://github.com/khushbu0810)  
