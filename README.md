# AIML-model-creation-Test
Creating an Artificial Intelligence (AI) / Machine Learning (ML) model is the process of developing a system that can learn patterns from data and make predictions or decisions without being explicitly programmed.
# AIML Group Project – Preprocessing Pipeline  
Project Title: The Dark Side of Social Media – Predicting Time-Wasting Habits Using AI  

---

# Overview of the Project
This project explores how social media usage habits contribute to time-wasting behavior and reduced productivity.  
Our goal is to preprocess the dataset, clean it, and prepare it for machine learning models that can predict user addiction levels and time-wasting patterns.  

The preprocessing pipeline includes:  
- Encoding categorical variables  
- Feature Creation 
- Outlier removal  
- Normalization / scaling  
- Feature selection  
- Dimensionality reduction (PCA)  

Each team member contributed to one preprocessing technique, and together, we created a combined pipeline that generates a final clean dataset ready for model training.  

---

# Dataset Details
- Dataset Name: Time-Wasters on Social Media  
- Format: CSV  
- Total Features: 31 (demographic, behavioral, and engagement features)  
- Target Variable: `Addiction Level`  
  - Numeric scale (0–7)  
  - Later discretized into categories: Low, Medium, High  

---

# Group Member Roles

- IT24100622 – Encoding Categorical Variables (Rathnayake S.S)  

- IT24100623 – Outlier Removal(Amarasinghe K.A.H.J)    

- IT24100564 – Normalization / Scaling ( Gunarathna G.A.M.A.D)    

- IT24100593 – Feature Selection (Abishanan S)    

- IT24100715 – Dimensionality Reduction (PCA) (Madhushan W.M.G)  

- IT24100636 – Feature Creation(Fernando T.M.I.U)   

---

# How to Run the Code
# 1. Requirements
- Python 3.x  
- Jupyter Notebook or Google Colab  
- Required libraries:
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# 2. Dataset
- Place the dataset file `Time-Wasters on Social Media.csv` inside the `data/raw/` folder.  
- Path structure:
  
2025-Y2-S1-MLB-B4G2-05/
├── data/raw/
│         └── Time-Wasters on Social Media.csv
├── notebooks/
├── results/

---
 3. Run Individual Preprocessing Notebooks
Each member has their own notebook with their IT number and preprocessing step.  
You can open and run them separately in Google Colab or Jupyter Notebook:

notebooks/
├── IT24100622-Encoding_categorical_variables.ipynb
├── IT24100623-OutlierRemoval.ipynb
├── IT24100564-NormalizationScaling.ipynb
├── IT24100593-FeatureSelection.ipynb
├── IT24100715-DimensionReduction.ipynb
└── IT24100636_Feature_Creation.ipynb

---

# 4. Run the Combined Pipeline
- Open `group_pipeline.ipynb`  
- Run all cells to execute the entire preprocessing pipeline in order:  
  1. Encoding categorical variables  
  2. Binning addiction levels  
  3. Outlier removal  
  4. Normalization/scaling  
  5. Feature selection  
  6. Dimensionality reduction (PCA)

---

# 5. Outputs
- The pipeline will generate the following outputs:  
  - Final Processed Dataset:  
    results/outputs/final_dataset.csv
    
  - EDA Visualizations:  
    results/eda_visualizations/*.png

---

6. Run on Google Colab (Optional)
using Google Colab:

from google.colab import files

# Save final dataset
df_final.to_csv("final_dataset.csv", index=False)

# Download the file
files.download("final_dataset.csv")
