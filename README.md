# DynaBiome-BMC

This repository contains the official source code and evaluation scripts for the manuscript:

**"DynaBiome: Interpretable Unsupervised Learning of Gut Microbiome Dysbiosis via Temporal Deep Models"**
*Accepted for publication in BMC Bioinformatics (2026).*

## 📂 Repository Structure

* **`data/`**: Directory containing the preprocessed microbiome tensors (e.g., `asv_interpretability_dataset_modified.csv`).
* **`01_DynaBiome_Model_Training.ipynb`**: The primary pipeline for training the LSTM Autoencoder architecture.
* **`02_Figure_Generation_Analysis.ipynb`**: Scripts to reproduce the figures and reconstruction error analysis presented in the paper.
* **`03_Baseline_Benchmarks.ipynb`**: Comparative analysis against baseline methods (PCA, Isolation Forest, Standard AE).

## 🚀 Getting Started

### Prerequisites
The code is implemented in Python 3.8+ using TensorFlow/Keras. Install dependencies via:

```bash
pip install tensorflow pandas numpy scikit-learn matplotlib seaborn shap
