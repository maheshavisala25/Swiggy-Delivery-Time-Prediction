# Swiggy-Delivery-Time-Prediction
Machine Learning Project on Swiggy Delivery Time Prediction
# 🍔 Swiggy Delivery Time Prediction Using Machine Learning

## 📌 Project Overview

This project aims to predict food delivery time for Swiggy orders using Machine Learning techniques. The model analyzes different factors, such as distance, traffic conditions, weather, city type, and vehicle type, to estimate how long a food delivery may take.

Accurate delivery time prediction can help improve customer satisfaction, reduce uncertainty, and support better delivery planning.

## 🎯 Business Problem

Customers want to know when their food will arrive. However, delivery time can vary depending on traffic, weather, distance, and other factors.

The objective of this project is to build a Machine Learning regression model that predicts delivery time in minutes using historical delivery data.

## 🎯 Project Objectives

- Analyze the factors that affect food delivery time.
- Perform Exploratory Data Analysis (EDA).
- Clean and preprocess the dataset.
- Handle missing values and duplicate records.
- Encode categorical features and scale numerical features where required.
- Train and compare different regression models.
- Evaluate model performance using standard regression metrics.
- Develop a reusable prediction pipeline.

## 📂 Project Structure

```text
Swiggy-Delivery-Time-Prediction/
│
├── swiggy_delivery_prediction.ipynb
├── swiggy_demographic.csv
└── README.md
```

**Note:** The CSV dataset must be added separately to the repository if you have permission to share it. The notebook currently loads a file named `swiggy_demographic.csv`.

## 🛠️ Technologies Used

- **Python** — Programming language
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Scikit-learn** — Data preprocessing, model training, and evaluation
- **Jupyter Notebook** — Interactive development environment

## 📊 Dataset Description

The dataset contains information related to food delivery orders.

Some important features include:

| Feature | Description |
|---|---|
| `distance` | Distance associated with the delivery |
| `weather` | Weather conditions |
| `traffic` | Traffic conditions |
| `city_type` | Type of city |
| `type_of_vehicle` | Delivery vehicle category |
| `order_date` | Date of the order |
| `time_taken` | Actual delivery time in minutes; target variable |

The exact columns and their definitions depend on the dataset provided.

## 🔍 Project Workflow

### 1. Data Collection and Understanding
- Load the dataset using Pandas.
- Examine the dataset shape, column names, data types, and statistical summary.

### 2. Exploratory Data Analysis (EDA)
- Analyze the distribution of delivery times.
- Examine correlations between numerical features.
- Study the relationship between distance and delivery time.
- Compare delivery times across traffic and weather conditions.
- Explore categorical feature distributions.

### 3. Data Preprocessing
- Identify and remove duplicate records.
- Check for missing values.
- Separate independent variables (`X`) and the target variable (`y`).
- Remove unnecessary features such as rider identifiers.
- Extract useful date-related features.
- Handle numerical and categorical data using suitable preprocessing techniques.

### 4. Train-Test Split
Split the dataset into training and testing sets to evaluate the model on unseen data.

- Training data: 80%
- Testing data: 20%
- Random state: 42

### 5. Model Building

The notebook explores the following regression algorithms:

- Linear Regression
- Decision Tree Regression
- Random Forest Regression
- Stochastic Gradient Descent (SGD) Regression

### 6. Model Evaluation

The models are evaluated using the following metrics:

- **MAE (Mean Absolute Error):** Average absolute difference between actual and predicted delivery times.
- **MSE (Mean Squared Error):** Average squared prediction error.
- **RMSE (Root Mean Squared Error):** Square root of the mean squared error, expressed in the target's units.
- **R² Score:** Measures how well the model explains variation in delivery time.

### 7. Hyperparameter Tuning

GridSearchCV and cross-validation are used to explore model configurations and improve generalization.

### 8. Final Prediction Pipeline

A Scikit-learn pipeline combines data preprocessing and a Random Forest regression model, providing a reusable workflow for training and prediction.

## 📈 Expected Outcome

The project aims to predict food delivery time in minutes based on the available order and delivery features.

It also helps identify which factors are associated with longer delivery times and compare the performance of different regression algorithms.

*Actual model performance should be reported after running the notebook. No accuracy or R² value is claimed here.*

## ⚙️ Installation and Setup

### Prerequisites

Install Python and Jupyter Notebook, or use Anaconda.

### Step 1: Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

### Step 2: Navigate to the project folder

```bash
cd YOUR-REPOSITORY
```

### Step 3: Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Step 4: Add the dataset

Place `swiggy_demographic.csv` in the project directory, alongside the notebook.

### Step 5: Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `swiggy_delivery_prediction.ipynb` and execute the cells in order.

## 🚀 Future Improvements

- Build an interactive web application using Streamlit.
- Allow users to enter delivery-related details and obtain predictions.
- Improve model performance through additional feature engineering and tuning.
- Add prediction uncertainty estimates.
- Deploy the model as a web service.
- Evaluate performance on new and unseen delivery data.

## 👨‍💻 Author

**Your Name**

Machine Learning Project | Python | Data Analysis | Regression

## 📄 Disclaimer

This is an educational Machine Learning project. It is not an official Swiggy application and is not affiliated with or endorsed by Swiggy.
