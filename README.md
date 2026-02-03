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

```

## Usage
### Clone the repository:

```Bash
git clone [https://github.com/](https://github.com/)[YourUsername]/DynaBiome-BMC.git
```
### Dataset: The dataset in data/ is zipped. The scripts are configured to read the .zip file directly.

## Using the Pre-Trained Model:

You can skip training (Notebook 01) and go directly to Notebook 02 or 03.
These notebooks are configured to automatically load the pre-trained model from models/DynaBiome_PatientSplit_Model.keras.

## Retraining (Optional):

If you wish to retrain the model from scratch, run 01_DynaBiome_Model_Training.ipynb. This will overwrite the file in the models/ directory.

## Citation
If you use this code or model in your research, please cite our paper:

@article{Qureshi2026DynaBiome,
  title={DynaBiome: Interpretable Unsupervised Learning of Gut Microbiome Dysbiosis via Temporal Deep Models},
  author={Qureshi, Awais and Wahid, Abdul and Qazi, Shams and Shahzad, Muhammad K. and Moheed, Hashir},
  journal={BMC Bioinformatics},
  year={2026},
  publisher={BioMed Central}
}
## License
This project is licensed under the MIT License - see the LICENSE file for details.
