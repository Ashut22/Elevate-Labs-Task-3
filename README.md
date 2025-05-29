# Elevate-Labs-Task-3
# Housing Price Prediction Using Linear Regression

This project implements a linear regression model to predict housing prices based on various features in the Housing dataset.

## Dataset
The dataset `Housing.csv` contains features like area, bedrooms, bathrooms, stories, parking, and categorical variables such as mainroad, guestroom, basement, etc.
- Target variable: `price`
- Dataset source: [Housing Dataset on Kaggle](https://www.kaggle.com/datasets/harishkumardatalab/housing-price-prediction)

## Steps Performed

1. **Data Loading and Exploration**  
   Loaded data, inspected basic info, and visualized distributions of numerical attributes and target variable.

2. **Categorical Variable Analysis**  
   Identified categorical features and counted unique classes in each.

3. **Data Preprocessing**  
   Applied one-hot encoding on categorical columns to convert them into numerical features.

4. **Feature-Target Split**  
   Split dataset into features (`X`) and target (`y`).

5. **Train-Test Split**  
   Divided data into training (80%) and testing (20%) sets.

6. **Model Training and Evaluation**  
   Trained a Linear Regression model and evaluated performance using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² Score.

7. **Feature Scaling**  
   Standardized numerical features and repeated model training and evaluation to check impact on performance.

## Results

| Metric         | Before Scaling     | After Scaling      |
|----------------|--------------------|--------------------|
| MAE            | 970,043.40         | 970,043.40         |
| MSE            | 1.75e+12           | 1.75e+12           |
| R² Score       | 0.6529             | 0.6529             |

*Note:* Standardization did not affect model accuracy because Linear Regression in scikit-learn is scale-invariant.

## Conclusion

Linear Regression explains about 65% of the variance in housing prices, with moderate prediction errors. One-hot encoding effectively handled categorical variables, and feature scaling had no impact on model performance.

---

**Tools & Libraries:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
