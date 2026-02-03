This `README.md` is **almost perfect**, but because we made those changes to the folder structure (adding a `models` folder) and zipped the dataset, you need to make **two small updates** so the documentation matches the actual files.

Here are the specific lines to change:

1. **Add the `models/` directory:** You created this folder to hold the `.keras` file, so it should be listed.
2. **Update the Data filename:** Since you zipped the file to get past the 25MB limit, the file in the repo is now `.zip`, not `.csv`.

### **Corrected README Content (Copy & Paste this)**

```markdown
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

### Usage

1. Clone the repository:
```bash
git clone [https://github.com/](https://github.com/)[YourUsername]/DynaBiome-BMC.git

```


2. The dataset in `data/` is zipped. Pandas can read it directly, or you can unzip it manually if preferred.
3. Run the notebooks in sequential order (01 -> 02 -> 03).

## 📄 Citation

If you use this code or model in your research, please cite our paper:

```bibtex
@article{Qureshi2026DynaBiome,
  title={DynaBiome: Interpretable Unsupervised Learning of Gut Microbiome Dysbiosis via Temporal Deep Models},
  author={Qureshi, Awais and Wahid, Abdul and Qazi, Shams and Shahzad, Muhammad K. and Moheed, Hashir},
  journal={BMC Bioinformatics},
  year={2026},
  publisher={BioMed Central}
}

```

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

```

### **Next Step**
Once you update this `README.md` on GitHub, you are **officially done** with the code repository.

You can now confidently copy the link (`https://github.com/[YourUsername]/DynaBiome-BMC`) into your manuscript's "Availability of data and materials" section and submit the final revision to the Editor! Congratulations on reaching the finish line!

```
