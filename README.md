# Sports Equipment Price Prediction

## IADS Assignment 1 — Predictive Modeling Project

### Project Overview

This project uses **Linear Regression** to predict the production price of sports equipment from production-related features.

The project follows the requirements of the IADS Predictive Modeling assignment, which asks students to select a research problem, use a publicly available real-world dataset, perform data cleaning and preprocessing, train either Linear Regression or Logistic Regression, evaluate the model, and create at least one meaningful visualization. fileciteturn0file0L8-L19

---

## Research Problem

### Research Question

> **Can the production price of sports equipment be predicted using production-related features?**

Sports equipment can have different production prices depending on characteristics such as materials, manufacturing factors, dimensions, production quantity, and other measurable variables.

The goal of this project is to build a machine learning model that can learn relationships between these variables and the production price.

### Objective

Build and evaluate a **Linear Regression** model capable of predicting the continuous production price of sports equipment.

---

## Dataset

The assignment requires a **publicly available dataset**, such as a dataset from Kaggle, the UCI Machine Learning Repository, or Google Dataset Search. fileciteturn0file0L9-L11

### Dataset Information

| Item | Details |
|---|---|
| Dataset | Sports Equipment Production/Price Dataset |
| Target Variable | Production Price |
| Dataset Source | Add the exact public dataset URL |
| Number of Records | Add after dataset selection |
| Number of Features | Add after dataset selection |
| Problem Type | Regression |

> **Note:** The assignment PDF does not specify a particular sports-equipment dataset. The exact dataset source and statistics should be added once the dataset is selected.

---

## Methodology

The project follows these main steps:

1. Load the publicly available dataset.
2. Inspect the dataset structure and data types.
3. Identify missing values and duplicate records.
4. Clean and preprocess the data.
5. Encode categorical variables if required.
6. Select the input features and target variable.
7. Split the data into training and testing sets.
8. Train a Linear Regression model.
9. Generate predictions using the test data.
10. Evaluate the model using appropriate regression metrics.
11. Generate and save a meaningful visualization.
12. Interpret the results and discuss limitations.

The assignment specifically requires necessary data cleaning and preprocessing and allows the use of libraries such as scikit-learn. fileciteturn0file0L12-L16

---

## Machine Learning Model

### Linear Regression

Linear Regression is used because the project predicts a **continuous numerical value: production price**.

Example implementation:

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()

model.fit(X_train, y_train)

y_pred = model.predict(X_test)
```

---

## Model Evaluation

The model will be evaluated using:

### R² Score

R² measures how much of the variation in the target variable is explained by the regression model.

A value closer to **1.0** generally indicates that the model explains more of the variation in the target.

### RMSE

Root Mean Squared Error (RMSE) measures the typical prediction error.

A lower RMSE indicates that predicted prices are, on average, closer to the actual prices.

The assignment specifically identifies **R² score and RMSE** as appropriate evaluation metrics for Linear Regression. fileciteturn0file0L13-L16

---

## Results

Add the final results produced by the notebook here.

| Metric | Result |
|---|---:|
| R² Score | `Add result` |
| RMSE | `Add result` |
| Training Samples | `Add value` |
| Testing Samples | `Add value` |

### Interpretation

The final analysis should explain:

- How accurately the model predicts production prices.
- Which features appear to have the strongest relationship with price.
- Whether the R² score indicates a useful predictive relationship.
- Whether the RMSE is acceptable for the dataset.
- Any limitations of the model or dataset.

---

## Visualization

At least one meaningful graph is required by the assignment. fileciteturn0file0L17-L19

For this project, the recommended visualization is:

### Actual vs Predicted Production Price

The graph compares the actual production prices from the test dataset with the prices predicted by the Linear Regression model.

Recommended file:

```text
images/actual_vs_predicted.png
```

Other useful visualizations may include:

- Feature vs. production price scatter plots
- Residual/error plots
- Regression line plots

---

## Project Structure

```text
sports-equipment-price-prediction/
│
├── index.html
├── README.md
│
├── notebook/
│   └── sports_equipment_price_prediction.ipynb
│
├── src/
│   └── model.py
│
├── data/
│   └── README.md
│
├── images/
│   └── actual_vs_predicted.png
│
├── requirements.txt
└── .gitignore
```

The assignment requires the final GitHub repository to contain a README, the analysis code as either a Jupyter Notebook or Python script, and the generated visualization image(s). fileciteturn0file0L20-L27

---

## Technologies Used

- **Python**
- **Pandas** — data manipulation and preprocessing
- **NumPy** — numerical operations
- **Scikit-learn** — machine learning and evaluation
- **Matplotlib** — data visualization
- **Jupyter Notebook** — analysis and experimentation

---

## Installation

Install the required Python packages:

```bash
pip install pandas numpy scikit-learn matplotlib jupyter
```

Or use a `requirements.txt` file:

```text
pandas
numpy
scikit-learn
matplotlib
jupyter
```

---

## How to Run

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
notebook/sports_equipment_price_prediction.ipynb
```

Run the notebook cells in order to:

1. Load the dataset.
2. Clean and preprocess the data.
3. Train the Linear Regression model.
4. Generate predictions.
5. Calculate R² and RMSE.
6. Generate the visualization.

---

## Assignment Checklist

- [ ] Research problem selected and explained
- [ ] Publicly available dataset selected
- [ ] Dataset source documented
- [ ] Data cleaning completed
- [ ] Data preprocessing completed
- [ ] Linear Regression model trained
- [ ] R² Score calculated
- [ ] RMSE calculated
- [ ] At least one meaningful graph generated
- [ ] Visualization saved in the repository
- [ ] Jupyter Notebook or Python script included
- [ ] README.md included
- [ ] GitHub repository made publicly accessible

---

## Conclusion

This project demonstrates how **Linear Regression** can be applied to a real-world sports equipment pricing problem.

The completed analysis will show whether production-related characteristics can be used to estimate sports equipment production prices and will evaluate the quality of those predictions using R² and RMSE.

---

## Author

**Name:** Add your name  
**Course:** IADS  
**Assignment:** Assignment 1 — Predictive Modeling Project  
**GitHub:** Add your GitHub profile/repository link
