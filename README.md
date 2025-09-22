# 🧹 Data Cleaning and Preprocessing

This repository provides a comprehensive **Data Preprocessing Toolkit** using Python. It includes both an **interactive Jupyter Notebook** and a **Python script** to clean, encode, scale, and handle outliers in your dataset.

The pipeline is designed to handle **numerical and categorical data**, with options for automatic or user-guided preprocessing.

---

## 📁 Project Structure

```
.
├── datasets/
│   ├── Titanic-Dataset.csv       # Example dataset
│   └── ...                       # Your other datasets
├── data_preprocessing.ipynb      # Interactive notebook
├── data_preprocessing.py         # Python script for automated preprocessing
├── README.md                     # This file
└── requirements.txt              # Python dependencies
```

---

## 🛠 Features

### 1️⃣ Data Exploration

* View dataset info, missing values, duplicates, and unique value counts.
* Inspect numeric and non-numeric data summaries.

### 2️⃣ Missing Value Imputation

* **Numerical columns**: Fill missing values with the median.
* **Categorical columns**: Fill missing values with the mode.
* Optionally drop columns exceeding a **missing data threshold**.

### 3️⃣ Encoding Categorical Data

* Label Encoding for binary or high-cardinality columns.
* One-Hot Encoding for categorical columns with few unique values.
* Option to skip columns if desired.

### 4️⃣ Scaling Numerical Data

* Standardization (Z-score) or Normalization (Min-Max) for numeric features.
* Option to skip columns as required.

### 5️⃣ Outlier Detection & Handling

* Detect outliers in numeric columns using IQR.
* Drop columns exceeding outlier percentage or cardinality thresholds.

### 6️⃣ Visualization

* Bar plots for missing values.
* Line plots for normalized cardinality of numeric columns.
* Histograms comparing numeric columns before and after preprocessing.

### 7️⃣ Save Processed Data

* Save the cleaned dataset as a CSV file.

---

## ⚡ Usage

### Using the Jupyter Notebook

1. Open `data_preprocessing.ipynb` in Jupyter Notebook.
2. Update the dataset path if required (`datasets/Titanic-Dataset.csv`).
3. Run the cells step by step to explore and preprocess your data interactively.

### Using the Python Script (Automated)

1. Update the `load_path` and `save_path` in `data_preprocessing.py`.
2. Run the script:

```bash
python data_preprocessing.py
```

3. Follow the prompts to handle missing data, encoding, scaling, and outliers.
4. Optionally save the preprocessed dataset.

---

## 📦 Requirements

Install dependencies using pip:

```bash
pip install -r requirements.txt
```

**requirements.txt:**

```
pandas
numpy
matplotlib
scikit-learn
```

---

## 💡 Notes

* Paste your dataset in the `datasets/` folder and update the variables in the main() of the program
* Datasets will be stored in the `datasets/` folder by default.
* Thresholds for missing values, outliers, and cardinality can be adjusted in the script.
* This pipeline supports both interactive and automated preprocessing workflows.

---
