# 🧠 Google Play Store App Success Prediction

A machine learning project aimed at predicting whether an app on the Google Play Store will be successful using real-world app metadata.

## 🔍 Objective

Help app developers, marketers, and Google itself identify what makes an app successful — defined as:
- **Rating ≥ 4.5**
- **Installs ≥ 100,000**

---

## 📊 Dataset
- Source: [Kaggle - Google Play Store Dataset](https://www.kaggle.com/datasets/lava18/google-play-store-apps)
- After cleaning: **7,729 apps** across **33 categories**
- Cleaned for corrupted rows, pricing and consistent formatting

---

## 🧪 Methodology

### 1. Data Cleaning
- Removed rows with `NaN`, `Free` in installs and broken prices
- Standardized columns like `Size`, `Price` and `Installs`
- Encoded categorical features (`Category`, `Content Rating`)

### 2. Feature Engineering
- Target column `Success` based on Rating + Installs
- Used features like `Reviews`, `Size`, `Installs`, `Category`

### 3. Modeling
- Random Forest Classifier
- 80/20 Train/Test split
- Scaled numeric features

---

## 📈 Results

- **Accuracy:** 87%
- **Precision for Success class:** 71%
- **Top Features:** `Reviews`, `Size`, and `Installs`

<img width="915" alt="Top 15 Most Important Features" src="https://github.com/user-attachments/assets/32dc1582-75df-45d3-8128-40ad7a8ecaff" />


---

## 💡 Key Insights

- ⭐ High number of **reviews** is the strongest indicator of success, suggesting user engagement is critical
- 📦 App **size** positively correlates with success, possibly due to richer features
- 📥 Higher **install counts** reinforce visibility with network effect
- 💰 0 paid apps remained after cleaning — confirming most Google Play apps are free

---

## 📎 Recommendation to Google

> Promote apps with high early engagement (reviews) and suggest creators optimize size & performance balance.
> Invest more in categories like **Education** and **Health & Fitness**, which show higher success rates.

---

## 🧠 Built With

- Python (Pandas, Scikit-learn, Seaborn, Matplotlib)
- Jupyter Notebook

---

## 📌 Author

**Saugat Pyakuryal**  
_M.S. Business Analytics | University of New Haven_  
GitHub: [@iamsaugaat](https://github.com/iamsaugaat)  
LinkedIn: [@iamsaugaat](https://linkedin.com/in/iamsaugaat)
