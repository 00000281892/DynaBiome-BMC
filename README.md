# DynaBiome-BMC

This repository contains the official source code and evaluation scripts for the manuscript:

**"DynaBiome: Interpretable Unsupervised Learning of Gut Microbiome Dysbiosis via Temporal Deep Models"**
*Accepted for publication in BMC Bioinformatics (2026).*

## 📂 Repository Structure

* **`data/`**: Directory containing the compressed microbiome tensors (`asv_interpretability_dataset_modified.zip`).
* **`models/`**: Contains the pre-trained LSTM Autoencoder model (`DynaBiome_PatientSplit_Model.keras`).
* **`01_DynaBiome_Model_Training.ipynb`**: The primary pipeline for training the LSTM Autoencoder architecture.
* **`02_Figure_Generation_Analysis.ipynb`**: Scripts to reproduce the figures and reconstruction error analysis presented in the paper.
* **`03_Baseline_Benchmarks.ipynb`**: Comparative analysis against baseline methods (PCA, Isolation Forest, Standard AE).

## 🚀 Getting Started

### Prerequisites
The code is implemented in Python 3.8+ using TensorFlow/Keras. Install dependencies via:

```bash
pip install tensorflow pandas numpy scikit-learn matplotlib seaborn shap

📄 Citation
If you use this code or model in your research, please cite our paper:
@article{Qureshi2026DynaBiome,
  title={DynaBiome: Interpretable Unsupervised Learning of Gut Microbiome Dysbiosis via Temporal Deep Models},
  author={Qureshi, Awais and Wahid, Abdul and Qazi, Shams and Shahzad, Muhammad K. and Moheed, Hashir},
  journal={BMC Bioinformatics},
  year={2026},
  publisher={BioMed Central}
}
