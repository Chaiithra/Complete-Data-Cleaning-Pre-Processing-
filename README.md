---

# **Complete-Data-Cleaning-Pre-Processing**

🧠 **Titanic Dataset - End-to-End Exploratory Data Analysis & Preprocessing**

A structured, modular, and professional notebook demonstrating in-depth understanding of data analysis, feature engineering, categorical encoding, normalization, standardization, and outlier handling—crafted for industry-readiness and academic rigor.

---

## 🗂️ **Project Structure**

This notebook is divided into logical and independent sections for efficient workflow navigation, inspired by best practices in real-world data pipelines.

---

## 📌 **1. Importing Libraries**

All necessary libraries, including **NumPy**, **Pandas**, **Matplotlib**, **Seaborn**, **Scikit-learn**, and additional utility packages, are imported and explained where needed.

---

## 📂 **2. Loading the Dataset**

The Titanic dataset is loaded using **Pandas**, with insights into its size and type. Suggestions for subsampling are provided for large-scale datasets.

---

## 🧠 **3. Understanding Data**

### 3.1 **Surface-Level Dataset Check**
- **Shape and Size**: Quick overview of the dataset structure.
- **Columns Overview**: Column names and initial examination.
- **Data Types**: Analysis of feature data types.
- **High-Level Summary**: Brief overview of the dataset.
- **Descriptive Statistics**: Summary of means, medians, and distributions.

### 3.2 **Null and NaN Analysis**
- **Null Percentage per Column**: Inspection of missing data percentage.
  
### 3.3 **Check for Duplicates**
- Check for duplicate rows using `df.duplicated().sum()`.  
- In this dataset, duplicates are not present.

### 3.4 **Uniqueness & Cardinality**
- **Cardinality Check**: Analysis of categorical variables based on uniqueness levels.

---

## 🧼 **4. Handling Null Values**

### 4.1 **Visual Inspection of Missing Data**
- Heatmaps and bar plots are used to visually inspect missing values.

### 4.2 **Correlation with Missing Data**
- Check for relationships between missingness and other features.

### 4.3 **Feature Distribution vs Missingness**
- Understand how missing data might relate to feature distribution for numerical variables.

### 4.4 **Imputation Methods (Basic)**
- **Mean**, **Median**, and **Mode** imputation for missing values.

### 4.5 **Predictive Imputation (Advanced)**
- Use **KNN Imputer** and **Random Forest Regressor Imputer** for imputation.

---

## 🔢 **5. Converting Categorical Features into Numerical Features**

### Encoding Techniques Implemented:
- **Label Encoding**
- **One-Hot Encoding**
- **Binary Encoding**
- **Ordinal Encoding**
- **Frequency Encoding**
- **Target Encoding**
- **Hashing Encoding**
- **Count Encoding**

Each encoding technique is implemented with examples and use-case scenarios for model compatibility and data leakage prevention.

---

## ⚖️ **6. Normalization**

Normalization techniques to scale features between 0 and 1:
- **Min-Max Normalization**
- **MaxAbs Normalization**
- **Quantile Normalization (Uniform)**

---

## 🧮 **7. Standardization**

Standardization techniques (centering data to have a mean of 0 and a standard deviation of 1):
- **Z-score Standardization**
- **Robust Scaler (Median & IQR)**
- **Power Transformation (Yeo-Johnson)**

---

## 🧹 **8. Outlier Handling**

### 8.1 **Detecting Outliers**

#### 8.1.1 **Statistical Methods**:
- **Box Plot (IQR Method)**
- **Z-score**
- **Modified Z-score**

#### 8.1.2 **Visualization Methods**:
- **Boxplot**
- **Violin Plot**
- **Scatter Plot**

#### 8.1.3 **Machine Learning-Based Methods**:
- **Isolation Forest** (for large datasets)
- **Local Outlier Factor (LOF)**
- **DBSCAN Clustering** (Density-Based)

---

### 8.2 **Handling Outliers**

#### 8.2.1 **Capping (Winsorization)**
- **Percentile-based capping**
- **IQR-based capping**
- **Standard deviation capping**

#### 8.2.2 **Transformation Techniques**
- **Log Transformation**
- **Square Root Transformation**
- **Box-Cox Transformation**
- **Yeo-Johnson Transformation**

#### 8.2.3 **Robust Statistical Methods**
- Replace with robust metrics.
- **Robust Scaling** (Median & IQR)
- **Quantile-Based Analysis**

#### 8.2.4 **Model-Based Approaches**
- **Isolation Forest**
- **Local Outlier Factor**
- **One-class SVM**
- **DBSCAN Clustering**

#### 8.2.5 **Binning/Discretization**
- **Equal-width binning**
- **Equal-frequency binning**
- **Custom binning**

#### 8.2.6 **Custom Imputation for Outliers**
- **Regression-based Imputation**
- **KNN Imputation for outliers**

#### 8.2.7 **Separate Modeling**
- **Create outlier indicators**
- **Stratified Modeling**
- **Weighted Modeling**

#### 8.2.8 **Robust Loss Functions**
- Use **Huber Loss** or **Quantile Regression** when training models. These loss functions are less sensitive to outliers.

#### 8.2.9 **Ensemble Methods**
- Many tree-based methods (**Random Forest**, **XGBoost**) are naturally robust to outliers.
- Consider using these algorithms if outliers cannot be reliably removed.

---

## 📊 **Applied to Titanic Dataset**

Outliers were removed using the **Z-score method** with a threshold of 3 for continuous numerical columns (**Age**, **Fare**), ensuring that model assumptions are respected.

---

## ✅ **Key Takeaways**

- Hands-on with all standard data transformation techniques.
- Clean, modular code with reusable functions.
- Statistical and ML-based outlier detection methods.
- Insightful visualizations at every step.

---

## 🚀 **Future Work**

- **Feature Importance Analysis** using machine learning models.
- **Dimensionality Reduction** using **PCA** or **UMAP**.
- **Model Training Pipelines** with hyperparameter tuning.

---

## 📁 **How to Use**

### Clone the Repo
```bash
git clone https://github.com/your-username/titanic-eda.git
```

### Navigate to Project Directory
```bash
cd titanic-eda
```

### Open the Notebook
```bash
jupyter notebook Titanic_EDA_Preprocessing.ipynb
```

---

## 🙌 **Acknowledgements**

- **Dataset**: Kaggle Titanic Dataset
- **Libraries**: Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Category Encoders, etc.

---

## 📧 **Contact**

Made with ❤️ by **[Chaiithra Thota]**  
Connect on LinkedIn: (https://www.linkedin.com/in/chaiithrathota/)
Connect on Twitter: (https://x.com/DebugDiary_)

---
