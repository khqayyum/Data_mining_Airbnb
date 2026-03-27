# 🏡 Airbnb Price Prediction using Machine Learning

This project builds a data-driven system to predict Airbnb listing prices using machine learning. Pricing short-term rentals is complex due to factors like location, room type, reviews, and demand patterns. This work focuses on designing a complete pipeline that transforms raw listing data into meaningful price predictions.

---

## 📊 Project Overview

- Dataset: ~232,000 Airbnb listings across 27 U.S. cities  
- Goal: Predict nightly listing price  
- Approach: End-to-end data mining pipeline with feature engineering and regression models  

The project emphasizes **practical modeling**, showing how structured data, text features, and location signals can be combined to improve prediction quality.

---

## ⚙️ Pipeline

The system follows a structured workflow:

1. Data cleaning and preprocessing  
2. Feature engineering  
3. Encoding and transformation  
4. Model training and comparison  
5. Model tuning and evaluation  

Key idea: The performance gain comes not just from the model, but from **how the data is represented**.

---

## 🧠 Feature Engineering Highlights

- 📍 **Geospatial Clustering**  
  Latitude and longitude are converted into neighborhood-like clusters using KMeans  

- 📝 **Text Features (TF-IDF)**  
  Listing titles are transformed into numerical features capturing signals like *luxury*, *view*, or *budget*  

- ⭐ **Review Signals**  
  Number of reviews, recency, and activity trends  

- 🏠 **Host & Listing Attributes**  
  Room type, availability, host activity  

- 🔄 **Log Transformation**  
  Stabilizes skewed price distribution for better learning  

---

## 🤖 Models Used

- Linear Regression  
- Random Forest  
- Gradient Boosting  
- **XGBoost (Best Performing Model)**  

---

## 📈 Results

| Metric | Value |
|------|------|
| R² Score | ~0.51 |
| MAE | ~$58 |
| RMSE | ~$89 |

The final model explains about half of the variance in listing prices and provides useful pricing guidance within a reasonable error range.

---

## 💡 Key Takeaways

- Feature engineering has a major impact on performance  
- Text and location features significantly improve predictions  
- Simpler models with strong features can compete with complex approaches  
- Real-world data requires careful handling of noise and outliers  

---

## 📂 Repository Contents

- 📄 `final_report.pdf` → Detailed project report  
- 💻 `notebook.ipynb` / `.py` → Implementation code  

---

## 🚀 How to Run

1. Install required libraries:

2. Run the notebook or Python script

---

## 🔗 Project Link

Colab Notebook:  
https://colab.research.google.com/drive/1mFbIX0X13UWfQo4TlA2ZNA1qqk7KZYXu?usp=sharing

---

## 📌 Future Improvements

- Incorporate external location data (distance to city center, attractions)  
- Model seasonal and time-based demand patterns  
- Build city-specific or hierarchical models  
- Deploy as a web-based pricing recommendation tool  

---

## 🙌 Final Note

This project demonstrates how machine learning can be applied to real-world pricing problems by combining structured data, text processing, and thoughtful feature design.
