# 💻 Laptop Price Prediction

A simple Machine Learning project to predict laptop prices based on their specifications.

## 📌 Project Overview

This project analyzes a laptop price dataset, cleans and preprocesses the data, selects important features, and uses a **linear regression model implemented with gradient descent** to estimate laptop prices.

## 📊 Dataset

The project uses the **Uncleaned Laptop Price Dataset** from Kaggle.

The dataset contains laptop information such as:

- Company
- Type
- Screen Resolution
- CPU
- RAM
- Memory
- GPU
- Operating System
- Weight
- Price

The original dataset contains **1303 rows and 12 columns**. After removing missing values and an unnecessary index column, the working dataset contains **1273 rows and 11 columns**.

## 🔧 Data Preprocessing

The following preprocessing steps are performed:

- Remove rows containing missing values
- Remove the unnecessary index column
- Encode categorical features based on their mean laptop price
- Convert RAM from text to numeric values
- Handle missing/unknown weight and screen-size values
- Convert weight from `kg` to numeric values
- Convert screen size to numeric values
- Remove duplicate records
- Analyze feature correlations
- Select features with a correlation greater than `0.5` with price
- Apply log transformation to the target price

## 🤖 Machine Learning Approach

Instead of using a ready-made regression library, the project implements the regression optimization manually.

### Model

**Linear Regression using Gradient Descent**

The model learns the parameters by minimizing the **Mean Squared Error (MSE)**.

The project includes:

- MSE calculation
- Gradient calculation
- Parameter initialization
- Iterative gradient descent
- Convergence based on a tolerance value

## 📈 Exploratory Data Analysis

The notebook also includes:

- Missing-value analysis
- Feature correlation analysis
- Correlation heatmap
- Price distribution
- Log-transformed price distribution

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook
- Kaggle Dataset

## 📁 Project Structure

```text
Laptop-price-prediction/
│
├── dataset/
│   └── laptopData.csv
│
├── laptop_src.ipynb
├── requirements.txt
├── lib_install.sh
└── README.md
```

## ▶️ How to Run

1. Clone this repository.

2. Install the required Python libraries:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```bash
jupyter notebook laptop_src.ipynb
```

4. Run the cells in order.

## 🎯 Objective

The main objective of this project is to understand the complete workflow of a regression problem:

**Data Collection → Data Cleaning → Feature Engineering → EDA → Feature Selection → Log Transformation → Linear Regression → Gradient Descent**

## 👨‍💻 Author

**Avdhesh02**
