# 🎬 Movie Rating Prediction using Machine Learning

## 📌 Prompt

**Develop a predictive model to estimate movie ratings based on genre, director, and actors.**

---

## 🎯 Project Goal

The aim of this project is to build a machine learning regression model that accurately predicts **IMDb ratings** based on various features of movies such as:
- Genre
- Director
- Actors
- Year of release
- Duration
- Number of votes

This project enables a deeper understanding of the **factors influencing movie ratings** and provides a predictive tool for estimating ratings of new or upcoming movies.

---

## 📚 Dataset

- **Name:** IMDb Movies India  
- **Format:** CSV  
- **Source:** Stored in Google Drive (`IMDb Movies India.csv`)  
- **Features Used:**
  - `Name`
  - `Year`
  - `Duration`
  - `Genre`
  - `Rating` (target)
  - `Votes`
  - `Director`
  - `Actor 1`, `Actor 2`, `Actor 3`

---

## 🎥 Project Demo

🔗 **Watch the video demonstration on LinkedIn:**  
[Click here to view the demo](https://www.linkedin.com/posts/kesana-mohana-mounika-548114344_internorbit-machinelearning-datascience-activity-7352229401691885569-ewKS?utm_source=share&utm_medium=member_android&rcm=ACoAAFYoewgBCwKr-tM3UK4tbA8AS98p6O7bcOE)


---

## 🧰 Libraries & Tools Used

- `pandas`, `numpy` – Data manipulation  
- `matplotlib`, `seaborn` – Visualization  
- `scikit-learn` – Machine learning & model evaluation  
- `RandomForestRegressor` – Used for regression  
- `Google Colab` – Execution environment

---

## 🔧 Project Steps

### 1. Data Cleaning & Preprocessing
- Removed duplicates and null values
- Converted string values (e.g., `"120 min"`) to integers
- Handled multiple genres per movie using `.explode()`
- Filtered top 10 directors; others marked as "Other"
- Applied one-hot encoding to categorical features

### 2. Feature Selection
- Removed non-contributing features like `Name`
- Used: `Year`, `Duration`, `Votes`, `Genre`, `Director`

### 3. Model Building
- Split the data into training and testing sets (80-20)
- Used **Random Forest Regressor** with 100 trees
- Trained on encoded and aligned features

### 4. Model Evaluation
- **Mean Absolute Error (MAE):** ~0.42  
- **Mean Squared Error (MSE):** ~0.43  
- **R² Score:** 0.771  
> A strong performance indicating the model captures key predictive signals.

---

## 🔮 Sample Prediction

A sample movie input with:
- Year: 2023
- Duration: 120 minutes
- Genre: Action
- Votes: 100000
- Director: "Other"

**Predicted IMDb Rating:** `6.88`

---

## 📊 Visualizations

- Histogram: Distribution of IMDb Ratings  
- Line Plot: Year-wise average IMDb Ratings  
- Scatter Plot: Duration vs IMDb Rating  
- Bar Chart: Average Rating by Genre  
- Scatter Plot: Votes vs IMDb Rating (Log scale)

---

## 🙌 Acknowledgments

Thanks to **IMDb**, **Google Colab**, and the **open-source community** for providing datasets and tools.

---

