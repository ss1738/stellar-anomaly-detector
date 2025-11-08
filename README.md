# 🌟 Multi-Modal Anomaly Detection for Extraterrestrial Data

## Overview
This PyTorch-based project demonstrates advanced unsupervised anomaly detection by solving two distinct scientific challenges: flagging unprecedented stellar events (Phase I) and detecting complex, non-radiant anomalies in planetary data (Phase II).

---

## 🛠️ Technical Stack
- **Framework:** PyTorch (Leveraging CUDA/GPU)
- **Data Sources:** NASA TESS Light Curves, Simulated Planetary Sensor Data
- **Architectures:** Recurrent Autoencoders (LSTM) for time-series, Multi-Modal Autoencoders (CNN + Dense) for data fusion.

---

## 🌌 Phase I: Galactic Anomaly Monitor (G-AM)

**Goal:** Detect statistical outliers in the flux of a stable star.
**Model:** LSTM Autoencoder trained on TIC 286923464.

### 1. Score Distribution & Threshold
The model established a strict **Discovery Threshold** at the 99.5th percentile.

![Stellar Anomaly Score Distribution](images/stellar_anomaly_score_distribution.png)

### 2. Key Finding: UNPRECEDENTED Stellar Event
The most anomalous sequence detected had a score of **384.9506**, confirming a significant deviation from normal stellar behavior.

![Stellar Flux Anomaly Reconstruction](images/stellar_max_anomaly_reconstruction.png)

---

## 🔬 Phase II: Non-Radiant Power Source Locator (NRPSL)

**Goal:** Identify anomalies where a visual/structural feature is present but the thermal signature is absent.
**Model:** Multi-Modal Autoencoder (MMAE) for fusing Image (CNN) and Tabular (Dense) data.

### Key Finding: 100% Detection Rate
The MMAE successfully segregated the anomaly class (red cluster on the right) from the normal data (left peak), achieving a **100.00% True Positive Detection Rate**.

![Multi-Modal Anomaly Detection Histogram](images/mmae_detection_histogram.png)

---

## 🚀 Usage and Reproducibility
1.  **Clone** this repository.
2.  **Install dependencies** using the provided file: `pip install -r requirements.txt`
3.  **Run** the main notebook: `Stellar_Anomaly_Detector (1).ipynb`

---

## ✅ Final Launch!

Once your `README.md` is updated, your project is professionally published and ready to be shared. Your final step is to **post the link on LinkedIn**! Good luck!
