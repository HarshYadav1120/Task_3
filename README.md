# 🏠 Linear Regression on Housing Dataset (Day 3)

## 📅 Date
**June 26, 2025**

## 📌 Task Summary

Today’s task focused on implementing a basic **machine learning regression pipeline** using a housing dataset. The objective was to:

- Preprocess the dataset (log transformation, encoding, scaling)
- Identify the most important numeric feature
- Train a simple linear regression model
- Plot the regression line
- Interpret the learned coefficients

---

## 📂 Steps Performed

1. **Data Cleaning and Transformation**
   - Dropped irrelevant or missing values
   - Applied `log1p()` transformation on the `price` column to handle skewness

2. **Feature Encoding and Scaling**
   - Categorical features encoded using `pd.get_dummies()` (One-Hot Encoding)
   - Concatenated with numerical features
   - Scaled the entire feature matrix using `StandardScaler`

3. **Feature Importance**
   - Computed Pearson correlation between all numeric features and `price_log`
   - Selected `area` as the most important predictor for visualization

4. **Simple Linear Regression**
   - Trained a model with `area` as input and `price_log` as target
   - Plotted the regression line using `matplotlib` and `seaborn`

5. **Coefficient Interpretation**
   - Extracted slope and intercept using `.coef_` and `.intercept_`
   - Explained the real-world meaning of the learned coefficient

---

## 📊 Output

- Regression line shows a positive correlation between `area` and `log(price)`
- Coefficient interpretation: _"For every 1 unit increase in area, log(price) increases by X units"_

---

## 📁 Files in this Folder

- `regression_plot.ipynb` – Jupyter notebook containing all code and plots
- `summary.md` – Short explanation of findings
- `data/` – (Optional) folder for sample data

---

## 🧠 Key Learnings

- Importance of preprocessing steps like encoding and scaling
- Why we visualize simple linear regression in 2D using one key feature
- How to interpret regression coefficients in terms of real-world impact

---

