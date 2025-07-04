# 🩺 Medical Cost Prediction Using Linear Regression

This project predicts **medical insurance charges** based on patient attributes using a linear regression model. It walks through the full ML pipeline — from data analysis to model evaluation — all done inside a Kaggle notebook.

---

## 📘 Overview

In this notebook, we:
- Explored the dataset (shape, types, null values)
- Visualized relationships between features and target (`charges`)
- Encoded categorical variables using one-hot encoding
- Trained a linear regression model to predict medical costs
- Evaluated model performance using MSE and R² score

---

## 📂 Dataset

- **Source:** [Kaggle - Medical Cost Personal Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)
- **Rows:** 1338  
- **Columns:** 7

---

## 🧾 Features Used

| Feature | Description |
|--------|-------------|
| `age` | Age of the insured person |
| `sex` | Gender *(encoded)* |
| `bmi` | Body Mass Index |
| `children` | Number of children/dependents |
| `smoker` | Smoking status *(encoded)* |
| `region` | Residential region *(encoded)* |
| `charges` | **Target** — Medical insurance cost |

---

## 🔍 Exploratory Data Analysis

- No null values found
- Used `data.describe()`, `data.info()`, and `data.corr()` to explore
- Heatmap showed **age** and **smoking status** have the strongest correlation with charges

---

## 📊 Visualizations

- Histograms of numerical features
- Correlation heatmap using Seaborn
- Pairplot for spotting trends and outliers

---

## 🧠 Model Training

- **Algorithm:** Linear Regression (`sklearn.linear_model`)
- **Train-Test Split:** 80/20
- **Encoding:** One-hot encoding with `pd.get_dummies(drop_first=True)`

---

## 📈 Results

- **R² Score:** ~0.78
- **Mean Squared Error (MSE):** ~33.6 million  
- **Key Finding:** Smokers are charged significantly more — a major feature in cost prediction.

---

## ⚙️ Tools & Libraries

- Python
- Pandas
- Seaborn
- Matplotlib
- Scikit-learn

---

## 🚀 Potential Next Steps

- Try regularized models like Lasso or Ridge
- Use Polynomial Features for non-linear trends
- Add model explainability with SHAP or LIME
- Deploy with Streamlit or Flask

---

## 🤖 Author

Project by [@Shubham04-oss](https://github.com/Shubham04-oss)  
Another brick in the AI wall 🧱✨  
