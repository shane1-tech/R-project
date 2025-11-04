# 🏠 Boston Housing Price Prediction in R

This project applies **Multiple Linear Regression** in **R** to predict housing prices based on socioeconomic and structural features.

## 📊 Objective
Predict the **Median Value of Owner-Occupied Homes (MEDV)** using predictors such as:
- Average number of rooms per dwelling (`RM`)
- Percentage of lower status population (`LSTAT`)
- Pupil–teacher ratio (`PTRATIO`)

## 🧠 Techniques Used
- Linear Regression Modeling
- Correlation Analysis
- Data Visualization with `ggplot2`
- Model Evaluation (R², p-values, Residual Analysis)

## 🗂️ Dataset
The dataset (`Housing_Data.csv`) is based on the **Boston Housing Dataset** originally from UCI Machine Learning Repository.

## 🧮 R Markdown Report
All analysis steps are documented in the R Markdown file:
`scripts/housing_regression.Rmd`

To run it:
```r
rmarkdown::render("scripts/housing_regression.Rmd")
```

## 📈 Key Insights
- Houses with **more rooms (RM)** tend to have higher prices.
- Higher **LSTAT** (lower status population) significantly reduces prices.
- Higher **PTRATIO** (student–teacher ratio) lowers median home values.

## 📈 Results

- Model explains ~74% of the variance in housing prices
- `RM` (average number of rooms) has a strong positive correlation with `MEDV` (median home value)
- `LSTAT` (lower status population) is negatively correlated with `MEDV`
