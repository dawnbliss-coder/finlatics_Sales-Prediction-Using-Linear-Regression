# 📊 Data Analytics & Sales Prediction

Two data analysis projects demonstrating exploratory data analysis (EDA), statistical modeling, and machine learning techniques for business insights.

## Projects

1. **Facebook Live Sellers Analysis** - EDA and K-means clustering on Thailand marketplace data
2. **Advertising Sales Prediction** - Multiple linear regression model predicting sales from TV, radio, and newspaper spend

## Key Techniques

- Exploratory Data Analysis (EDA) with correlation analysis
- K-means clustering for customer segmentation
- Multiple linear regression for sales forecasting
- Feature engineering and data preprocessing
- Model evaluation and comparison

---

## 📌 Project 1: Facebook Live Sellers Dataset

### 📂 Dataset Overview
- **Rows:** 7050  
- **Columns:** 14 (after cleaning)  
- Includes reaction metrics, post types, timestamps, comments, and shares.

---

### ✔ Tasks Completed

#### **1️⃣ Effect of Upload Time on Reactions**
- Converted `status_published` to datetime.
- Extracted **month** and **hour**.
- Plotted average reactions by month and hour.

#### **2️⃣ Correlation Analysis**
Analyzed correlations between:
- `num_reactions`
- `num_comments`
- `num_shares`

**Findings:**
- Reactions ↔ Comments → Very weak correlation  
- Reactions ↔ Shares → Weak positive correlation  
- Comments ↔ Shares → Strong correlation  

#### **3️⃣ K-Means Clustering**
- Used numeric features such as reactions, emotions, shares.
- Applied Label Encoding for `status_type`.
- Scaled data and applied K-Means.
- Elbow method selected **8 clusters**.

#### **4️⃣ Post Type Counts**
| Post Type | Count |
|-----------|-------|
| link | 63 |
| photo | 4288 |
| status | 365 |
| video | 2334 |

#### **5️⃣ Average Engagement per Post Type**
Calculated mean reactions, comments, and shares for each post type.

---

## 📌 Project 2: Sales Prediction Using Advertising Data

### 📂 Dataset Overview
- Columns: TV, Radio, Newspaper, Sales  
- Filled missing Radio values using **median**.

---

### ✔ Tasks Completed

#### **1️⃣ Average TV Advertising Spend**
- **147.04**

#### **2️⃣ Correlation (Radio vs Sales)**
- Correlation = **0.349** (weak positive)

#### **3️⃣ Most Influential Advertising Medium**
- **TV shows the strongest influence** on Sales.

#### **4️⃣ Multiple Linear Regression Model**
- Trained model on TV, Radio, Newspaper.
- Visualized **Actual vs Predicted Sales**.

#### **5️⃣ Prediction for New Input**
Input:  
TV = 200, Radio = 40, Newspaper = 50  
**Predicted Sales ≈ 19.73**

#### **6️⃣ With and Without Data Normalization**
- Compared scaled vs unscaled models.
- Scaling improved stability but not major accuracy change.

#### **7️⃣ Model Using Only Radio & Newspaper**
- Built reduced model.
- Accuracy decreased → confirms **TV is the key predictor**.

---

## 🛠️ Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Jupyter Notebook  

---
