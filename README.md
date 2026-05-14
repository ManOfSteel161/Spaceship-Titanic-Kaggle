# 🚀 Spaceship Titanic: Kaggle Competition

[![Kaggle](https://img.shields.io/badge/Kaggle-035a7d?style=for-the-badge&logo=kaggle&logoColor=white)](#)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](#)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-F37626.svg?style=for-the-badge&logo=Jupyter&logoColor=white)](#)
[![Machine Learning](https://img.shields.io/badge/Machine_Learning-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](#)

## 🌌 Project Overview
This repository contains my solution for the **[Spaceship Titanic](https://www.kaggle.com/competitions/spaceship-titanic)** competition on Kaggle. 

**The Challenge:** Welcome to the year 2912. The Spaceship Titanic collided with a spacetime anomaly, and almost half of the passengers were transported to an alternate dimension. The goal of this project is to build a predictive Machine Learning model to determine whether a passenger was transported or not, using passenger manifest data (e.g., cabin location, amenities spending, and destination).

## 📂 Repository Structure
*   `Spaceship_Titanic.ipynb` 📓: The core Jupyter Notebook containing the entire end-to-end data science pipeline, including Exploratory Data Analysis (EDA), data preprocessing, feature engineering, model training, and predictions.
*   `train.csv` 📊: The training dataset containing passenger details and the target variable (`Transported`).
*   `test.csv` 📉: The test dataset used to generate the final predictions.
*   `sample_submission.csv` 📄: The required submission format for Kaggle scoring.
*   `README.md` 📝: Project documentation.

## 🛠️ Tech Stack
*   **Language:** Python
*   **Data Manipulation:** Pandas, NumPy
*   **Data Visualization:** Matplotlib, Seaborn
*   **Machine Learning:** Scikit-Learn (Classification models)

## 🎯 Methodology & Approach
To achieve high accuracy in this classification task, the following pipeline was implemented:

1.  **Exploratory Data Analysis (EDA):** Analyzed the distribution of numerical features (like spending on Room Service, Food Court, SPA) and categorical features (HomePlanet, Destination) against the target variable.
2.  **Data Cleaning & Imputation:** Handled missing values strategically. For example, inferring missing categorical data based on passenger groups or filling numerical spending columns with medians/zeros.
3.  **Feature Engineering:** 
    *   Extracted `Deck`, `Number`, and `Side` from the `Cabin` feature.
    *   Calculated `Total Spending` across all luxury amenities.
    *   Engineered group sizes from the `PassengerId` to determine if passengers traveling in groups had different survival rates.
4.  **Modeling & Evaluation:** Trained and evaluated multiple classification algorithms (e.g., Logistic Regression, Random Forest, Gradient Boosting, SVM, Catboost) to find the optimal model.

## 🚀 How to Run the Project

To replicate this analysis on your local machine:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/ManOfSteel161/Spaceship-Titanic-Kaggle.git](https://github.com/ManOfSteel161/Spaceship-Titanic-Kaggle.git)
    cd Spaceship-Titanic-Kaggle

2. Install the necessary dependencies:
Ensure you have Python installed, then run:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn jupyter

3.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook

4. Open the `.ipynb` file in your browser and execute the cells to view the EDA and model training process.
