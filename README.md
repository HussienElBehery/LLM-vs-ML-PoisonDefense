# A Comparative Study of Data Poisoning Detection in Wearable AI Systems using Machine Learning and Large Language Models

**Authors:** Hussien Ahmed, Abdelaziz Amr, Abdallah Emam, Mamdouh Korithem, Mohamed Youssef

*School of Information Technology and Computer Science, Nile University, Giza, Egypt*

---

## Abstract

Data poisoning poses a significant threat to wearable human activity recognition (HAR) systems by covertly flipping labels in sensor datasets. This work benchmarks the effectiveness of lightweight, traditional machine learning (ML) models against memory-efficient, quantized large language models (LLMs) for both detection and sanitization of poisoned data. 

Our findings indicate that ML classifiers, such as Random Forest and XGBoost, trained on a substantial dataset (100,000 samples), achieve high detection accuracies (93.5-94.0%) and recall rates (over 78%), with sanitization accuracies exceeding 87.8%, all achieved with CPU training times under 50 seconds.  In contrast, open-source LLMs (unsloth/gemma-2b, unsloth/llama-3.2-3B, unsloth/qwen2-1.5B), quantized and fine-tuned, demonstrated lower performance (up to 61% detection accuracy) on a smaller dataset, often defaulting to flagging all samples as poisoned to inflate recall.

The study concludes that, within typical resource constraints, traditional ML methods offer a more efficient, robust, and interpretable defense against label-flip attacks in wearable AI systems compared to the current quantized LLM approaches.

---

## 🎯 Key Focus & Contributions

* Comparative analysis of traditional ML and quantized LLMs for data poisoning detection and sanitization in Wearable AI for Human Activity Recognition (HAR).
* Evaluation of label-flipping attack scenarios.
* Performance metrics include detection accuracy, recall, F1-score, and sanitization accuracy.
* Highlights the efficiency and robustness of ML models (Random Forest, XGBoost) under resource constraints.
* Investigates the performance of 4-bit quantized LLMs (Gemma, Llama 3.2, Qwen2) using zero-shot, few-shot, and fine-tuning approaches.

---

## 📊 Dataset

The study utilizes the **MotionSense dataset**, which contains sensor data (accelerometer and gyroscope) from smartphones for various human activities.

---

## ⚙️ Models & Methods

### Machine Learning Models
* Logistic Regression
* Random Forest
* Support Vector Machine (SVM)
* k-Nearest Neighbors (KNN)
* Gaussian Naive Bayes (GNB)
* XGBoost

### Large Language Models (LLMs)
* unsloth/gemma-2b
* unsloth/llama-3.2-3B
* unsloth/qwen2-1.5B
    * All LLMs were quantized to 4-bit weights via BitsAndBytes and fine-tuned with PEFT. 

---
