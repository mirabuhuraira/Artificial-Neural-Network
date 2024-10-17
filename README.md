# Artificial-Neural-Netwrok
This repository demonstrates data preprocessing and exploratory data analysis (EDA) for neural networks. Key steps include handling missing values, encoding categorical data, splitting data, and feature scaling to improve model performance.

# Data Preprocessing and Exploratory Data Analysis (EDA) for Neural Networks

## Project Overview
This project focuses on preparing data for training neural networks by performing **Exploratory Data Analysis (EDA)** and key preprocessing steps. It includes splitting the data, encoding categorical variables, scaling the features, and preparing the dataset for machine learning models.

## Files in the Repository
1. **1) Preprocessing for NN.ipynb**: This notebook covers all steps from EDA to data preprocessing and feature scaling.
2. **hcvdat0.csv**: The dataset used in the analysis (replace with your actual dataset file).

## Key Steps

### 1. Exploratory Data Analysis (EDA)
Before jumping into preprocessing, **EDA** is performed to understand the structure of the data. Key steps include:
- **Checking for Missing Values**: We identify any missing values that may need to be imputed or removed.
- **Descriptive Statistics**: Summarizing the dataset to understand the distribution of numerical and categorical variables.
- **Distribution of Features**: Plotting histograms, pie charts or using other visualization techniques to see how different features are distributed.

### 2. Label Encoding
Categorical variables (such as gender or target classes) are converted into numerical form using `LabelEncoder`:
- **Why?** Neural networks and most machine learning algorithms work better with numerical data.
- **How?** Each unique category is mapped to an integer value.
- 
### 3. Train-Test Split
The dataset is split into **training** and **test sets** to ensure that model performance is evaluated on unseen data. We use `train_test_split` to create an 80-20 split.

### 4. Feature Scaling
We use **StandardScaler** to standardize the features:
- **Why?** Neural networks perform better when input features have a mean of 0 and a standard deviation of 1. This ensures faster convergence during training and prevents features with large ranges from dominating the learning process.
- **How?** The scaler is fit on the training data, and the same transformation is applied to both the training and test sets.

### 5. Neural Network Ready Data
Finally, both the features (`X_train`, `X_test`) and targets (`Y_train`, `Y_test`) are converted into numpy arrays to ensure compatibility with neural network frameworks.

## Requirements
The project requires the following Python libraries:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

Install the libraries with:
```
pip install pandas numpy scikit-learn matplotlib seaborn

