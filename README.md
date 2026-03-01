# 🚀 Neuromorphic Anomaly Detection for KUCARS Rovers

### **Real-time Perception using Spiking Neural Networks (SNN) & Event-Based Vision**

## 📌 Project Overview

This repository contains a bio-inspired anomaly detection system designed for autonomous rovers operating in challenging environments (e.g., high-glare desert landscapes). Traditional frame-based cameras generate redundant data and suffer from motion blur; our approach utilizes **Event-Based Cameras** and **Spiking Neural Networks (SNNs)** to achieve low-latency, energy-efficient perception.

### **Key Features:**

* **Asynchronous Processing:** Only pixel-level changes (spikes) are processed, reducing data bandwidth.
* **Temporal Integration:** Uses Leaky Integrate-and-Fire (LIF) neurons to accumulate evidence of anomalies over time.
* **UAE Environment Ready:** High dynamic range (HDR) capabilities allow for reliable sensing in extreme sunlight and deep shadows.

---

## 📊 Live Visualizations

### **1. SNN Intelligence Dashboard**

The system monitors the "Spike Density" of the incoming event stream. When the density crosses a learned threshold, the SNN classifies the activity as an anomaly.

### **2. Prediction Confidence**

Real-time tracking of the model's confidence levels between "Normal" and "Anomalous" states.

---

## 🛠️ Technical Architecture

The pipeline translates raw events into actionable intelligence:

1. **Event Stream:** Raw `.h5` data from the neuromorphic sensor.
2. **SNN Layers:** A multi-layer architecture built with `snntorch` using LIF neurons.
3. **Thresholding:** Anomalies are detected when spike integration exceeds the membrane potential threshold.

---

## 📂 Repository Structure

* `animations/`: GIF exports of the model's real-time performance.
* `models/`: Trained weights (`neuromorphic_anomaly_detector.pth`).
* `scripts/`: Jupyter notebooks and Python scripts for data processing and visualization.
* `v2e/`: Integration scripts for video-to-events toolbox.

---

## 🚀 Getting Started

1. **Clone the repo:** `git clone https://github.com/Shehuadekunmi/neuromorphic-anomaly.git`
2. **Install dependencies:** `pip install snntorch tonic h5py matplotlib`
3. **Run the dashboard:** Open `scripts/Final_Dashboard.ipynb` in Jupyter.

---

## 🎓 Acknowledgments

This research is developed with the **Khalifa University Center for Autonomous Robotic Systems (KUCARS)** in mind, focusing on the next generation of neuromorphic rover perception.





**Would you like me to help you write the "Methodology" section for your formal 4-page paper next?**
