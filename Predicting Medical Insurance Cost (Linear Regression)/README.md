# Insurance Cost Prediction Using Linear Regression

This project aims to predict individual medical insurance costs (`charges`) using a linear regression model. The dataset includes features like age, sex, BMI, number of children, smoking status, and region. This project highlights **data preprocessing, model training, evaluation metrics, and visualizations**.

---

## Dataset
The dataset contains the following columns:

| Column     | Description |
|-----------|-------------|
| `age`     | Age of primary beneficiary |
| `sex`     | Insurance contractor gender (male/female) |
| `bmi`     | Body mass index (kg/m²) |
| `children`| Number of children/dependents covered by insurance |
| `smoker`  | Smoking status (yes/no) |
| `region`  | Residential area in the US (northeast, southeast, southwest, northwest) |
| `charges` | Individual medical costs billed by insurance (target variable) |

---

## Libraries
This Project uses the listed libraries for this Linear Regression task:
- numpy
- pandas
- scikit-learn
- matplotlib

## Features
- **Data Preprocessing**:
  - Handle missing values
  - Remove outliers
  - Encode categorical variables (`sex`, `smoker`, `region`) using OneHotEncoder
  - Scale numeric variables (`age`, `bmi`, `children`) using StandardScaler
- **Model Training**:
  - Linear Regression implemented from scratch
  - Linear Regression using scikit-learn
- **Evaluation Metrics**:
  - Mean Squared Error (MSE)
  - R² Score
- **Visualization**:
  - Distribution of features
  - Model predictions vs actual values

---
