# 🛡Network Intrusion Detection System (NIDS) using IBM AutoAI

This project implements an intelligent **Network Intrusion Detection System (NIDS)** using the **NSL-KDD dataset** and **IBM AutoAI**. The goal is to accurately classify network traffic as either normal or a type of cyber-attack (DoS, Probe, R2L, U2R), enabling early detection and improving cybersecurity.

---

## Problem Statement

Cyberattacks can severely compromise network systems. Manual monitoring is inefficient and prone to errors. This project aims to build a robust ML model that automates the detection and classification of intrusions, providing real-time insights for network security.

---

## Solution Overview

- **Dataset:** NSL-KDD (labeled network traffic with attack types)
- **Tool:** IBM AutoAI (free on IBM Cloud Lite)
- **Model Used:** Batched Tree Ensemble Classifier (Snap Random Forest)
- **Approach:**
  - Preprocess and encode 41 traffic features
  - Group attack types into 5 classes: DoS, Probe, R2L, U2R, Normal
  - Train and optimize using AutoAI
  - Deploy model via IBM Watson Machine Learning for predictions

---

## System Requirements

- IBM Cloud Lite account (Watson Studio + AutoAI access)
- Python (for local exploration, optional)
- Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

---

## Results

| Metric               | Value     |
|----------------------|-----------|
| Accuracy (Overall)   | XX.XX %   |
| Precision (Macro Avg)| XX.XX %   |
| Recall (Macro Avg)   | XX.XX %   |
| F1-Score (Macro Avg) | XX.XX %   |
| F1-Score (Weighted)  | XX.XX %   |

*Note: Replace XX.XX with actual AutoAI leaderboard results.*

---

## Future Scope

- Integrate with live monitoring tools (e.g., Wireshark)
- Add alert system and threat visualization
- Expand to detect zero-day attacks with DL models
- Continuous learning from live network streams

---

## References

- [NSL-KDD Dataset](https://www.unb.ca/cic/datasets/nsl.html)
- [IBM AutoAI Docs](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.6.x?topic=projects-autoai)
- Tavallaee et al., *A detailed analysis of the KDD Cup 99 data set*, 2009
- [Scikit-learn](https://scikit-learn.org/)

---

## File Structure
📂 intrusion-detection/
├── train.csv
├── test.csv
├── README.md
└── Nootbook.ipynb

