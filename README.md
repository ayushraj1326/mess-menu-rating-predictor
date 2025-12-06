# Mess Menu Rating Predictor 🍽️

A machine learning project that predicts the rating of a mess meal (lunch/dinner) based on its features.  
The model learns from manually created ratings using regression, then converts the predicted value into a final decision:

**Eat in mess 👍 or Eat outside 👎**

---

## 📌 Project Overview

This project applies **supervised learning** to predict how good a meal will be using:

- Meal type (lunch/dinner)
- Day of the week
- Paneer/Chicken presence
- Number of items in the meal
- Dessert availability
- Spicy level
- Variety score

The output is a **predicted rating (1–5)** and a **binary decision**.

---

## 🔧 Techniques Used

- **Data collection & feature engineering**
- **OneHotEncoding** for categorical features
- **RandomForestRegressor**
- **Pipeline + ColumnTransformer**
- **Train-Test Split**
- **Evaluation Metrics**  
  - MAE  
  - RMSE  
  - R² Score
- **Learning Curve Visualization**
- **Feature Importance Plot**

---

## 📂 Files in This Repo

- `model.ipynb` — Main ML notebook  
- `rating-dataset.csv` — Custom dataset with 14 meal samples  
- `README.md` — Project documentation  
- `.gitignore`  

---

## 🚀 How to Run

### 1. Clone the repo

```bash
git clone https://github.com/ayushraj1326/mess-menu-rating-predictor.git
cd mess-menu-rating-predictor
```
## 2. Install dependencies
```
pip install scikit-learn pandas matplotlib
```
## 🧠 Model Decision Logic
```python
if predicted_rating > 3:
  decision = “Eat in mess 👍”
else:
  decision = “Eat outside 👎”
```
## ✨ Future Improvements
- Add more weekly menus for better accuracy
- Build a Streamlit web interface
- Add nutritional features (protein, calories, etc.)
- Predict separate ratings for taste, healthiness, and variety
- Add classification mode (good meal / bad meal)