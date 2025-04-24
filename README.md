# Complete-Data-Cleaning-Pre-Processing

---

# 🧠 Titanic Dataset - End-to-End Exploratory Data Analysis & Preprocessing

> A structured, modular, and professional notebook to demonstrate in-depth understanding of data analysis, feature engineering, categorical encoding, normalization, standardization, and outlier handling—crafted for industry-readiness and academic rigor.

---

## 🗂️ Project Structure

This notebook is divided into logical and independent sections for efficient workflow navigation, inspired by best practices in real-world data pipelines.

---

## 📌 1. Importing Libraries
All necessary libraries including `numpy`, `pandas`, `matplotlib`, `seaborn`, `sklearn`, and additional utility packages are imported and explained where needed.

---

## 📂 2. Loading the Dataset
The Titanic dataset is loaded using `pandas`, with insights into its size and type. Suggestions for subsampling are given for large-scale datasets.

---

## 🧠 3. Understanding Data

### 3.1 Surface-Level Dataset Check
- Shape, column preview, memory usage, and basic schema inspection.

### 3.1.2 Renaming Columns (7 Methods)
- `re.sub()`, `.rename()`, `.set_axis()`, list comprehension, `map()`, `.add_prefix()`, `.add_suffix()` to maintain readable column names.

### 3.1.3-3.1.4 Data Types & Summary Stats
- Type-checking, null-counts, memory profiling, and identifying numeric columns for further transformations.

### 3.1.5 Descriptive Statistics
- Summary of means, medians, and distribution patterns.

### 3.2 Null and NaN Analysis  
- Column-wise null percentage.

### 3.3 Duplicate Check  
- Identification and removal of duplicate rows.

### 3.4 Uniqueness & Cardinality
- Categorical variable inspection based on uniqueness levels.

---

## 🧼 4. Handling Null Values

### 4.1 Visual Inspection  
- Heatmaps and bar plots to inspect missingness.

### 4.2 Correlation with Missing Data

### 4.3 Feature Distribution vs Missingness

### 4.4 Imputation (Basic Methods)  
- Mean, Median, Mode.

### 4.5 Predictive Imputation (Advanced)
- KNN Imputer & Random Forest Regressor Imputer.

---

## 🔢 5. Converting Categorical Features into Numerical

### Encoding Techniques Implemented:
- Label Encoding
- One-Hot Encoding
- Binary Encoding
- Ordinal Encoding
- Frequency Encoding
- Target Encoding
- Hashing Encoding
- Count Encoding

Each encoding technique is implemented with examples and use-case scenarios for model compatibility and data leakage prevention.

---

## ⚖️ 6. Normalization

### Techniques:
- Min-Max Normalization  
- MaxAbs Normalization  
- Quantile Normalization

---

## 🧮 7. Standardization

### Techniques:
- Z-score Standardization  
- Robust Scaler (Median & IQR)  
- Power Transformation (Yeo-Johnson)

---

## 🧹 8. Outlier Handling

### 8.1 Statistical Methods
- Box Plot  
- Z-score  
- Modified Z-score

### 8.2 Visualization
- Boxplot  
- Violin Plot  
- Multivariate Scatter Plot

### 8.3 Machine Learning-Based Methods
- Isolation Forest (for large datasets)  
- Local Outlier Factor (LOF)  
- DBSCAN Clustering (Density-Based)

### 8.4 Handling Techniques
- Winsorization  
- Replace with Median or Mean

---

## 📊 Applied to Titanic Dataset

Outliers were removed using **Z-score method** with a threshold of 3 for continuous numerical columns (`Age`, `Fare`) ensuring that model assumptions are respected.

---

## ✅ Key Takeaways

- 🔬 Hands-on with all standard data transformation techniques
- ⚙️ Clean, modular code with reusable functions
- 📉 Statistical and ML-based outlier detection
- 🧠 Insightful visualizations at every step

---

## 🚀 Future Work

- Feature importance analysis using ML models  
- Dimensionality reduction using PCA or UMAP  
- Model training pipelines with hyperparameter tuning

---

## 📁 How to Use

```bash
# Clone the repo
git clone https://github.com/your-username/titanic-eda.git

# Navigate to project directory
cd titanic-eda

# Open the notebook
jupyter notebook Titanic_EDA_Preprocessing.ipynb
```

---

## 🙌 Acknowledgements

- Dataset: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)
- Libraries: Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Category Encoders etc

---

## 📧 Contact

Made with ❤️ by [Chaiithra Thota]  
📫 Connect on LinkedIn: [linkedin.com/in/chaiithrathota](#)

---

