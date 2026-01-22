# Pakistan Housing Price Prediction Model 🇵🇰🏠

This repository contains an end-to-end Machine Learning project to predict property prices in major Pakistani cities. The model leverages historical real estate data to provide price estimations based on location, property type, and physical dimensions.

## 📌 Project Overview
The real estate market in Pakistan is diverse and volatile. This project aims to simplify price estimation using regression analysis. The workflow includes:
* **Data Collection:** Utilizing a dataset of 168,000+ property listings.
* **Data Cleaning:** Handling missing values in agency/agent fields and dropping redundant columns like URLs and IDs.
* **Outlier Removal:** Using domain knowledge (e.g., price per square foot) to remove data points that would skew the model.
* **Feature Engineering:** Creating specific features like `price_per_sqft` to improve prediction accuracy.
* **Model Selection:** Comparing multiple algorithms to find the most robust predictor.

## 📊 Dataset Features
The model is trained on the following key features:
- **Location:** City (Islamabad, Lahore, Karachi, Rawalpindi, Faisalabad) and specific localities.
- **Property Type:** House, Flat, Upper Portion, Lower Portion, etc.
- **Size:** Total Area (converted into a uniform square foot metric).
- **Amenities:** Number of bedrooms and bathrooms.



## 🛠️ Tech Stack
* **Python** (Core Language)
* **Pandas/NumPy** (Data Manipulation)
* **Matplotlib/Seaborn** (Visualization)
* **Scikit-Learn** (Machine Learning Pipeline)
* **Joblib** (Model Exporting)

## 📈 Model Performance
We evaluated the dataset using a `GridSearchCV` approach with `ShuffleSplit` cross-validation across the following models:
1. **Linear Regression**
2. **Lasso Regression**
3. **Decision Tree Regressor**

**Result:** The **Decision Tree Regressor** achieved the highest accuracy, with an R² score of approximately **0.99**, making it the primary model for this project.



## 🚀 How to Use
1. **Clone the repo:**
   ```bash
   git clone [https://github.com/yourusername/Pakistan-Real-Estate-Price-Predictor.git](https://github.com/yourusername/Pakistan-Real-Estate-Price-Predictor.git)
