
# Data Cleaning & Preprocessing

## Overview

This repository is a hands-on guide to **data cleaning and preprocessing** in Python. It is designed for beginners who want to understand how to transform raw data into a clean, structured, and ready-to-use format for machine learning tasks.

The project uses the **Titanic dataset** as an example and demonstrates step-by-step methods to handle missing values, remove duplicates, encode categorical features, scale numerical features, detect outliers, and visualize data for better understanding.

## Features

- Identify and handle **missing values** in numeric and categorical columns.
- Remove **duplicate rows** to ensure data integrity.
- Convert **categorical features** into numerical format using:
  - Label Encoding  
  - One-Hot Encoding
- **Standardize or normalize numerical features** for better comparability.
- Detect and remove **outliers interactively** using IQR.
- Visualize **feature distributions** and **normalized cardinality**.
- Compare datasets **before and after preprocessing**.

## Getting Started

### Requirements

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

You can install the required packages using:

```bash
pip install pandas numpy matplotlib scikit-learn
```

### Using the Jupyter Notebook

1. Open `DataCleaning_Preprocessing.ipynb` in Jupyter Notebook.
2. Follow the notebook step-by-step:
   - Import packages
   - Load the dataset
   - Explore missing values and duplicates
   - Handle categorical and numerical features
   - Encode categorical data
   - Scale numerical features
   - Detect and remove outliers interactively
   - Visualize and compare datasets
3. The notebook is **interactive** and will prompt you for decisions such as:
   - Dropping columns with too many missing values
   - Encoding categorical variables
   - Scaling or skipping numerical columns
   - Removing columns based on outlier percentage or cardinality

### Using the Python Script (Automated)

For a more **automated approach**, you can use the Python script version `data_cleaning.py`. Simply run:

```bash
python data_cleaning.py
```

This script applies the same preprocessing steps as the notebook but without interactive prompts, making it suitable for batch preprocessing or pipeline integration.

## Dataset

The notebook uses the **Titanic dataset** as an example. You can replace it with any dataset, but ensure that you adjust column names if needed.

Download the Titanic dataset [here](https://www.kaggle.com/c/titanic/data).

## Outputs

- Cleaned dataset ready for machine learning tasks.
- Visualizations showing:
  - Normalized cardinality of numeric features
  - Changes in numeric features before and after preprocessing

## Contributing

Feel free to submit issues, suggestions, or pull requests if you want to improve this repository.

