# Student Performance Machine Learning

This repository contains a machine learning project designed to analyze and predict student performance based on demographic, social, and academic background data. The project uses the well-known UCI Student Performance dataset.

## Project Overview

The main objective of this project is to build and evaluate various machine learning models to predict a student's final grade (`G3`). The project tackles this problem from two distinct machine learning tracks:

1. **Regression Track**: Predicting the exact numerical value of the final grade (on a scale from 0 to 20).
2. **Classification Track**: Predicting whether a student will pass or fail (a score of 10 or higher is considered a Pass).

## Dataset

The dataset (`data/student_data.csv`) contains rich student information:
- **Demographics**: Age, sex, address type, family size, parent's education/jobs.
- **Social & Behavioral**: Study time, free time, frequency of going out, alcohol consumption (`Dalc`, `Walc`), health status.
- **Academic History**: Past class failures, school support, first period grade (`G1`), and second period grade (`G2`).
- **Target Variable**: Final grade (`G3`).

## Models Evaluated

The code tests a variety of algorithms to find the best performing model for both regression and classification:
- Linear / Logistic Regression
- Regularized Regression (Ridge, Lasso, ElasticNet)
- K-Nearest Neighbors (KNN)
- Decision Trees
- Ensemble Methods (Random Forest, AdaBoost, XGBoost)
- Support Vector Machines (SVM / SVR)

## Repository Structure

- `data/` : Contains the `student_data.csv` dataset.
- `notebooks/` : Contains the main `student_performance_ml.ipynb` Jupyter Notebook, featuring data exploration, preprocessing, and model training/evaluation pipelines.
- `requirements.txt` : Lists the required Python libraries.

## Getting Started

1. **Clone the repository**.
2. **Set up a virtual environment** (optional but recommended):
   ```bash
   python -m venv venv
   # On Windows: venv\Scripts\activate
   # On Mac/Linux: source venv/bin/activate
   ```
3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
4. **Run the Analysis**: Open your IDE or Jupyter Notebook and run the cells inside `notebooks/student_performance_ml.ipynb` to see the models in action!
