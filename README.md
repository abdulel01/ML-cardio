# ML-cardio — Cardiovascular Disease Risk Assessment

## Overview
This project builds a machine learning model to predict **cardiovascular disease risk** using patient clinical and lifestyle features.
The notebook trains baseline and tree-based models, evaluates performance, and outputs a **risk probability** and **risk band**
(Low / Medium / High) for each sample.

## Dataset
Source (Kaggle): https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset  (by sulianova)  
The dataset contains patient records with clinical measurements and a binary target `cardio` (0/1).  

**Important:** The dataset is provided via Kaggle and may be subject to Kaggle terms and the dataset’s license.  
If you plan to publish/redistribute the dataset (e.g., in Zenodo), confirm the dataset’s reuse/redistribution terms on Kaggle first.

## Files
- `Untitled4-2.ipynb` — main notebook (end-to-end workflow)
- `requirements.txt` — Python dependencies
- `DATA_DICTIONARY.md` — column descriptions and units
- `LICENSE` — code license (MIT)

## How to run (Google Colab)
1. Open the notebook in Colab.
2. Upload `cardio_train.csv` (from Kaggle) using the file sidebar, OR mount Google Drive.
3. Run the notebook top-to-bottom (**Runtime → Restart and run all**).

**Note:** The CSV is semicolon-separated, so it must be loaded with:
```python
pd.read_csv("cardio_train.csv", sep=";")
