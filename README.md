# 🎮 Pre-launch Game Sales Prediction

This project predicts the **global sales of video games before launch** using only metadata such as genre, platform, publisher, and release year. By analyzing historical trends and applying machine learning, it helps game developers, publishers, and investors estimate commercial performance early in the development lifecycle.

---

## 📌 Problem Statement

Predicting a game's success before it hits the market is challenging. Most sales forecasts rely on post-launch performance data. This project aims to build a **regression model** that uses only **pre-launch attributes** (like Genre, Platform, Publisher, and Release Year) to forecast a game's **Global Sales**.

---

## 📊 Dataset

The dataset used comes from a historical video game sales record. Each entry includes:

- `Name`: Game title
- `Platform`: Console/platform (e.g., PS4, Xbox)
- `Year`: Release year
- `Genre`: Game genre (e.g., Action, Sports)
- `Publisher`: Publishing company
- `Global_Sales`: Total global sales (in millions)
- `NA_Sales`, `EU_Sales`, `JP_Sales`, `Other_Sales`: Regional sales

For pre-launch prediction, **only metadata features** were used: `Platform`, `Genre`, `Publisher`, `Year`.

---

## 🧪 Exploratory Data Analysis

- Visualized **sales distribution**, **regional trends**, and **sales over the years**
- Identified top publishers by total sales
- Explored feature correlations to understand predictive power

---

## ⚙️ Preprocessing

- Removed missing values
- Encoded categorical variables using `LabelEncoder`:
  - `Platform`, `Genre`, and `Publisher`
- Dropped columns not available pre-launch (e.g., regional sales)
- Split data into training and test sets

---

## 🧠 Model

- **Model Used**: `DecisionTreeRegressor` from Scikit-learn
- **Features Used**: Platform, Genre, Publisher, Year
- **Target**: Global Sales

### Evaluation Metrics:
- **R² Score**: `0.8411`
- **Mean Absolute Error (MAE)**: `0.0179`
- **Root Mean Squared Error (RMSE)**: `0.8244`

---

## 📈 Results

The model demonstrated that even basic pre-launch data holds strong predictive power. While Decision Trees were used here as a baseline, the approach can be extended to other models (e.g., Random Forest, XGBoost) for better accuracy.

---

## 📌 Future Work

- Try advanced regressors like **Random Forest** or **XGBoost**
- Implement **hyperparameter tuning** with GridSearchCV
- Build a **Streamlit app** for interactive sales prediction
- Include more metadata (developer, marketing budget, etc.)
- Experiment with **deep learning models** for complex feature interactions

---

## 🧰 Tech Stack

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn

---

## 🙌 Author

**Jaat Devrajsingh Bharat Singh**  
Data Science Enthusiast | [LinkedIn](https://www.linkedin.com/in/jaat-devrajsingh/)
