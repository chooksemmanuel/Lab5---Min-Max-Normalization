# 🏠 Min-Max Normalization & PCA Workshop

### 👤 Student Information
* **Group:** Group 6 
* **Team Members**
- Emmanuel Ihejiamaizu (9080005)
- Liggia Elena Taboada Cruz (9085905)
- Chao-Chung Liu (9067679)

---

## 📘 Project Overview
This workshop explores two essential data preprocessing techniques in Machine Learning: **Min-Max Normalization** and **Principal Component Analysis (PCA)**. We used a real-world housing dataset to understand how scaling affects data and how PCA helps find hidden structures in features.

## 🧠 Key Learning Topics

### 1. Min-Max Normalization
- **Manual Implementation:** We wrote the code from scratch without using libraries to understand the math: $\frac{x - x_{\min}}{x_{\max} - x_{\min}}$.
- **Why it matters:** Normalization ensures that features with large numbers (like Price) do not "bully" features with small numbers (like Bedrooms) during model training.

### 2. Principal Component Analysis (PCA)
- **Standardization:** We learned that **StandardScaler** is better than Min-Max for PCA because it gives every feature **equal weight** (Unit Variance).
- **Variance Analysis:** We found that 5 PCs are needed to explain 90% of the data. No single feature dominates this dataset.
- **Loadings & Geometry:** We used Heatmaps to see how features like `Area_sqft` and `Lot_Size` create a "tradeoff" in PC1.



## 🚀 Important Insights (Talking Points)
- **Variance ≠ Prediction:** Our most important finding was that high variance in PCA does not mean it can predict `Price`. The correlation was near zero (r ≈ 0.03).
- **Non-Linearity:** This suggests that house prices might have a **non-linear relationship** with the features, requiring models like **Random Forest** instead of simple linear PCA.



## 📂 Project Structure
```text
.
├── data/
│   └── housing_data.csv        # The housing dataset
├── .gitignore                  # Git ignore file
├── MinMax_Normalization_Workshop.ipynb  # Main analysis notebook
├── README.md                   # Project documentation
└── requirements.txt            # Project dependencies.

```

## 🛠️ How to Run
1. **1. Clone the project:**
    ```bash
    git clone [https://github.com/chooksemmanuel/Lab5---Min-Max-Normalization.git]
    ```
2. **Create a Virtual Environment:**
    ```bash
    python -m venv venv
    # On Windows:
    .\venv\Scripts\activate
    # On Mac/Linux:
    source venv/bin/activate
    ```
3. **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

---
