<div align="center">

# ☕ India Coffee Market ML

### Coffee Consumer Spending Prediction & Market Analysis

**Data Analysis • Machine Learning • Consumer Behaviour • Coffee Spending Prediction • Interactive Dashboard**

[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python\&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas\&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy\&logoColor=white)](https://numpy.org/)
[![Scikit--learn](https://img.shields.io/badge/Scikit--learn-Machine%20Learning-F7931E?logo=scikit-learn\&logoColor=white)](https://scikit-learn.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B?logo=streamlit\&logoColor=white)](https://streamlit.io/)

</div>

---

## 🚀 Project Overview

**India Coffee Market ML** is a machine learning project focused on analysing coffee consumer behaviour in India and predicting **monthly coffee spending** using survey-based consumer data.

The project follows an end-to-end machine learning workflow:

**Raw Survey Data → Data Cleaning → Exploratory Data Analysis → Feature Engineering → Encoding → Model Training → Model Evaluation → Spending Prediction → Dashboard**

The objective is to understand how factors such as **age, income, coffee consumption frequency, preferred coffee type, preferred brand, city and purchasing behaviour** are related to monthly coffee spending.

---

## 🎯 Project Objectives

* Analyse coffee consumption behaviour among Indian consumers.
* Explore demographic and purchasing patterns.
* Identify factors associated with monthly coffee expenditure.
* Build a machine learning model to predict monthly coffee spending.
* Compare model performance using standard regression metrics.
* Present analytical results through visualisations and an interactive dashboard.

---

## 📊 Dataset

The project uses survey data containing information about Indian coffee consumers.

### Main Features

| Feature               | Description                               |
| --------------------- | ----------------------------------------- |
| `age`                 | Consumer age                              |
| `gender`              | Consumer gender                           |
| `city`                | Consumer city                             |
| `occupation`          | Consumer occupation                       |
| `monthlyIncome`       | Monthly income                            |
| `coffeeFrequency`     | Coffee consumption frequency              |
| `preferredCoffeeType` | Preferred type of coffee                  |
| `preferredBrand`      | Preferred coffee brand                    |
| `purchaseLocation`    | Usual coffee purchase location            |
| `purchaseMode`        | Mode of purchase                          |
| `monthlyCoffeeSpend`  | Monthly coffee spending — target variable |

The dataset contains **11,072 records and 17 features** before modelling.

---

## 🧹 Data Preprocessing

The following preprocessing steps are performed:

* Dataset loading using Pandas
* Data inspection using `info()` and `describe()`
* Duplicate record detection and removal
* Missing-value checking
* Numerical and categorical feature identification
* Categorical feature encoding using One-Hot Encoding
* Feature/target separation
* Train-test splitting
* Machine learning pipeline creation

---

## 🔍 Exploratory Data Analysis

The analysis explores relationships between coffee spending and consumer characteristics, including:

* Age distribution
* Income distribution
* Coffee consumption frequency
* Preferred coffee types
* Preferred brands
* City-wise consumer behaviour
* Purchase locations
* Purchase modes
* Monthly coffee spending
* Relationship between income and coffee spending
* Relationship between coffee frequency and spending

Visualisations are created using Python data-analysis and plotting libraries.

---

## 🤖 Machine Learning

### Problem Type

This project treats **monthly coffee spending prediction as a regression problem**.

### Target Variable

```text
monthlyCoffeeSpend
```

### Input Features

The model uses consumer demographic, income, coffee preference and purchasing-behaviour features to predict monthly spending.

### Workflow

```text
Dataset
   ↓
Data Cleaning
   ↓
Feature Selection
   ↓
Categorical Encoding
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Prediction
   ↓
Model Evaluation
```

---

## 📈 Model Evaluation

Regression models are evaluated using standard metrics such as:

* **MAE — Mean Absolute Error**
* **MSE — Mean Squared Error**
* **RMSE — Root Mean Squared Error**
* **R² Score — Coefficient of Determination**

These metrics help measure how closely the predicted coffee spending values match the actual values.

---

## 🖥️ Interactive Dashboard

The project also includes an interactive dashboard for exploring the coffee market analysis and machine learning results.

The dashboard provides a visual interface for exploring:

* Consumer demographics
* Coffee consumption behaviour
* Spending patterns
* Market insights
* Model-related results
* Analytical visualisations

### Launch Dashboard

Install the required dependencies:

```bash
pip install -r requirements.txt
```

If the dashboard uses Streamlit:

```bash
streamlit run dashboard/app.py
```

> Run the command from the project root directory.

---

## 📂 Project Structure

```text
Coffee_Project/
│
├── README.md
├── requirements.txt
│
├── data/
│   └── coffee_dataset.csv
│
├── notebooks/
│   └── coffee_analysis.ipynb
│
├── src/
│   └── coffee_spending.py
│
├── dashboard/
│   └── app.py
│
├── models/
│   └── coffee_spending_model.pkl
│
├── outputs/
│   ├── figures/
│   └── results/
│
└── assets/
    └── figures/
```

> The structure above represents the intended organisation of the project. File and folder names can be adjusted according to the final repository contents.

---

## 🛠️ Technologies Used

| Technology       | Purpose                                  |
| ---------------- | ---------------------------------------- |
| Python           | Programming and ML development           |
| Pandas           | Data manipulation and analysis           |
| NumPy            | Numerical computation                    |
| Matplotlib       | Data visualisation                       |
| Scikit-learn     | Machine learning and preprocessing       |
| Streamlit        | Interactive dashboard                    |
| Joblib           | Model saving and loading                 |
| Jupyter Notebook | Exploratory analysis and experimentation |

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/Muskan2705/Coffee_Project.git
```

Move into the project directory:

```bash
cd Coffee_Project
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

### Run the Python Analysis

```bash
python src/coffee_spending.py
```

### Run the Notebook

Open:

```text
notebooks/coffee_analysis.ipynb
```

and execute the cells sequentially.

### Run the Dashboard

```bash
streamlit run dashboard/app.py
```

---

## 📌 Key Project Highlights

* End-to-end Python machine learning workflow.
* Analysis of **11K+ coffee consumer records**.
* Consumer behaviour analysis using survey data.
* Regression-based monthly coffee spending prediction.
* Numerical and categorical feature preprocessing.
* One-Hot Encoding for categorical variables.
* Model evaluation using MAE, RMSE and R².
* Interactive dashboard for visual analysis.
* Reusable machine learning workflow using Scikit-learn.

---

## ⚠️ Data & Analytical Limitation

The dataset is based on **survey responses rather than official historical coffee sales transactions**.

Therefore, the spending prediction model should be interpreted as a **survey-based consumer spending analysis**, not as an official forecast of India's total coffee market revenue or sales.

The model's results depend on the quality, representativeness and distribution of the survey responses.

---

## 🔐 Data Privacy

If the original survey dataset contains personally identifiable information, it should not be publicly published.

Only cleaned and privacy-safe data should be included in the public repository.

---

## 👤 Author

### Muskan

B.Tech — Computer Science & Engineering

GitHub: [@Muskan2705](https://github.com/Muskan2705)

---

<div align="center">

### ☕ India Coffee Market ML

**Turning coffee consumer data into meaningful machine learning insights.**

</div>
