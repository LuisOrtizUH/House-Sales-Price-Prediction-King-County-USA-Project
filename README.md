# 🏠 House Sales Price Prediction - King County, USA

<p float="left">
    <img src="https://images.credly.com/size/680x680/images/d9ab365d-7897-4973-a764-8acf6c277570/Coursera_20IBM_20Data_20Analyst_20Prof_20Cert_20V3.png" width="300" />
    <img src="" width="300" />
</p>

![Data Analysis with Python](https://img.shields.io/badge/IBM-Data_Analysis_with_Python-0072CE?style=for-the-badge&logo=ibm)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine_Learning-01D277?style=for-the-badge&logo=tensorflow&logoColor=white)
![Real Estate Analytics](https://img.shields.io/badge/Real_Estate_Analytics-FF6B35?style=for-the-badge&logo=homeadvisor&logoColor=white)
![R² 0.798](https://img.shields.io/badge/R²_Score-0.798-brightgreen?style=for-the-badge)

![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit_learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-2596BE?style=flat-square&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

## 🎯 Project Overview

This project is the **Final Assignment** for the **IBM Data Analysis with Python** course, where I act as a Data Analyst for a Real Estate Investment Trust. The objective is to predict residential housing prices in King County (Seattle area) using machine learning techniques to inform investment decisions.

<p float="left">
    <img src="https://github.com/Willie-Conway/IBM-Data-Analyst-Portfolio/blob/9064d670d63f81972017fed3e6d9acc281129bde/Data%20Analysis%20with%20Python/Final%20Project/Screenshots/Question%204.png" width="300" />
    <img src="https://github.com/Willie-Conway/IBM-Data-Analyst-Portfolio/blob/9064d670d63f81972017fed3e6d9acc281129bde/Data%20Analysis%20with%20Python/Final%20Project/Screenshots/Question%205.png" width="300" />
    <img src="https://github.com/Willie-Conway/IBM-Data-Analyst-Portfolio/blob/9064d670d63f81972017fed3e6d9acc281129bde/Data%20Analysis%20with%20Python/Final%20Project/Screenshots/Question%208.png" width="300" />
</p>

<p float="left">
    <img src="https://github.com/Willie-Conway/IBM-Data-Analyst-Portfolio/blob/9064d670d63f81972017fed3e6d9acc281129bde/Data%20Analysis%20with%20Python/Final%20Project/Screenshots/Question%209.png" width="300" />
    <img src="https://github.com/Willie-Conway/IBM-Data-Analyst-Portfolio/blob/9064d670d63f81972017fed3e6d9acc281129bde/Data%20Analysis%20with%20Python/Final%20Project/Screenshots/Question%2010.png" width="300" />
    <img src="https://github.com/Willie-Conway/IBM-Data-Analyst-Portfolio/blob/9064d670d63f81972017fed3e6d9acc281129bde/Data%20Analysis%20with%20Python/Final%20Project/Screenshots/Question%207.png" width="300" />
</p>

## 📋 Business Context

### **Role**: Data Analyst at a Real Estate Investment Trust
### **Objective**: Start investing in residential real estate by accurately predicting housing prices
### **Dataset**: House sale prices for King County, Washington (May 2014 - May 2015)

## 📊 Dataset Information

### **Source**: [Kaggle - House Sales in King County, USA](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction)
### **Records**: 21,613 properties
### **Features**: 20+ attributes including:
- **Property Characteristics**: bedrooms, bathrooms, square footage, floors
- **Location Data**: latitude, longitude, zipcode
- **Quality Metrics**: grade, condition, view, waterfront
- **Temporal Data**: year built, year renovated

## 🛠️ Technical Implementation

### **Module 1: Importing Data Sets**
- Load and inspect the dataset
- Display data types and statistical summaries
- Initial data quality assessment

### **Module 2: Data Wrangling**
- Drop unnecessary columns (`id`, `Unnamed: 0`)
- Handle missing values in `bedrooms` and `bathrooms`
- Data cleaning and preparation for analysis

### **Module 3: Exploratory Data Analysis (EDA)**
- Analyze distribution of floor values
- Boxplot analysis: Waterfront vs Non-waterfront price outliers
- Correlation analysis using scatter plots
- Identify key features correlated with price

### **Module 4: Model Development**
- Simple Linear Regression with single features
- Multiple Linear Regression with feature combinations
- Pipeline creation for preprocessing and modeling
- Polynomial feature transformation

### **Module 5: Model Evaluation and Refinement**
- Train-test split (85-15 split)
- Ridge Regression with regularization (α=0.1)
- Second-order polynomial transformation
- Model performance evaluation using R² score

## 🔍 Key Analyses Performed

### **Question 1-3: Data Understanding & Wrangling**
- Displayed data types of each column
- Dropped irrelevant columns and handled missing values
- Analyzed unique floor value distributions

### **Question 4-5: Exploratory Analysis**
- Identified waterfront properties have higher prices and more outliers
- Determined `sqft_above` is positively correlated with price (0.605)
- Found top correlated features: `sqft_living` (0.702), `grade` (0.667)

### **Question 6-8: Model Development**
- Simple Linear Regression (sqft_living): R² = 0.493
- Multiple Linear Regression: R² = 0.657
- Pipeline implementation with polynomial features

### **Question 9-10: Model Refinement**
- Ridge Regression (α=0.1): R² = 0.701
- Polynomial Ridge Regression: R² = 0.798 (Best Model)

## 📈 Results & Performance

| Model | Features | R² Score | Description |
|-------|----------|----------|-------------|
| **Simple Linear** | `sqft_living` | 0.493 | Baseline model |
| **Multiple Linear** | 11 features | 0.657 | Improved with multiple predictors |
| **Ridge Regression** | All features | 0.701 | Regularization prevents overfitting |
| **Polynomial Ridge** | 2nd degree features | **0.798** | **Best performing model** |

### **Top 5 Price Predictors**:
1. **Square Footage (Living)**: 0.702 correlation
2. **House Grade**: 0.667 correlation  
3. **Square Footage (Above)**: 0.606 correlation
4. **Living Area (2015)**: 0.585 correlation
5. **Bathrooms**: 0.526 correlation

### **Key Business Insights**:
- 🏠 **Square footage** is the strongest price predictor
- 🌊 **Waterfront properties** command premium prices
- 📐 **House grade** (King County system) significantly impacts value
- 🛁 **Bathrooms** matter more than bedrooms for price
- 📍 **Location** (latitude) shows moderate correlation

## 🎯 Business Recommendations

### **Investment Strategy**:
1. **Prioritize Properties With**:
   - High square footage (especially living area)
   - Better grade ratings (7+ on King County scale)
   - Waterfront locations for premium returns
   - More bathrooms relative to bedrooms

2. **Consider**:
   - Properties with recent renovations
   - Higher floor counts (correlates with price)
   - Better views (view score impacts price)

3. **Caution Areas**:
   - Overly large lots without corresponding living space
   - Older properties without renovations
   - Properties far from Seattle center

### **Model Application**:
- Use polynomial ridge regression for price predictions
- Regularization helps prevent overfitting to training data
- Model can estimate prices within ~20% accuracy range
- Ideal for initial investment screening and due diligence

## 📁 Project Structure

```
📂 House-Sales-Price-Prediction/
│
├── 📜 House_Sales_in_King_Count_USA.ipynb      # Main Jupyter notebook
├── 📜 House_Sales_in_King_Count_USA.jupyterlite.ipynb  # JupyterLite version
├── 📜 housing.csv                               # Dataset (21,613 records)
│
├── 📂 Screenshots/                              # All question outputs
│   ├── Question 1.png
│   ├── Question 2.png
│   ├── Question 3.png
│   ├── Question 4.png
│   ├── Question 5.png
│   ├── Question 6.png
│   ├── Question 7.png
│   ├── Question 8.png
│   ├── Question 9.png
│   └── Question 10.png
│
└── 📜 README.md                                 # This file
```

## 🚀 How to Run This Project

### **Option 1: Cloud Environment (Recommended)**
1. Access the JupyterLab on Skills Network Labs
2. Upload the notebook and housing.csv file
3. Execute cells sequentially

### **Option 2: Local Machine**
```bash
# 1. Clone or download the project files
git clone https://github.com/yourusername/house-sales-prediction.git

# 2. Install required packages
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# 3. Launch Jupyter
jupyter notebook House_Sales_in_King_Count_USA.ipynb

# 4. Run all cells or execute step-by-step
```

### **Option 3: Google Colab**
1. Upload notebook to Google Colab
2. Upload housing.csv or use direct download link
3. Run all cells (adjust file paths as needed)

## 🛠️ Technical Skills Demonstrated

### **Data Analysis & Wrangling**
![Data Wrangling](https://img.shields.io/badge/Data_Wrangling-FF6B35?style=for-the-badge)
![Exploratory Data Analysis](https://img.shields.io/badge/EDA-3498DB?style=for-the-badge)
![Statistical Analysis](https://img.shields.io/badge/Statistical_Analysis-FF6B6B?style=for-the-badge)
![Data Cleaning](https://img.shields.io/badge/Data_Cleaning-27AE60?style=for-the-badge)

### **Machine Learning & Modeling**
![Predictive Modeling](https://img.shields.io/badge/Predictive_Modeling-9B59B6?style=for-the-badge)
![Linear Regression](https://img.shields.io/badge/Linear_Regression-8E44AD?style=for-the-badge)
![Ridge Regression](https://img.shields.io/badge/Ridge_Regression-2ECC71?style=for-the-badge)
![Feature Engineering](https://img.shields.io/badge/Feature_Engineering-E74C3C?style=for-the-badge)

### **Visualization & Communication**
![Data Visualization](https://img.shields.io/badge/Data_Visualization-FF6384?style=for-the-badge)
![Business Insights](https://img.shields.io/badge/Business_Insights-FF9E0F?style=for-the-badge)
![Data Storytelling](https://img.shields.io/badge/Data_Storytelling-27AE60?style=for-the-badge)

### **Tools & Technologies**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

## 🏆 Key Achievements

✅ **79.8% Prediction Accuracy** achieved with polynomial ridge regression  
✅ **Complete End-to-End Analysis** from data import to business recommendations  
✅ **10 Comprehensive Questions** addressing all aspects of data analysis workflow  
✅ **Multiple Modeling Techniques** compared and evaluated  
✅ **Business-Ready Insights** for real estate investment decisions  
✅ **Professional Documentation** with screenshots and clear explanations  

## 🔮 Future Enhancements

### **Technical Improvements**:
1. **Additional Algorithms**: Random Forest, XGBoost, Neural Networks
2. **Feature Engineering**: Price per sqft, property age, neighborhood clusters
3. **Advanced Validation**: K-fold cross-validation, hyperparameter tuning
4. **Geospatial Analysis**: Mapping property locations and price distributions

### **Business Applications**:
1. **Interactive Dashboard**: Real-time price prediction tool
2. **Investment Calculator**: ROI estimates based on predicted prices
3. **Market Trend Analysis**: Time-series forecasting
4. **Risk Assessment Module**: Confidence intervals for predictions

## 📄 Project Context

This project is part of the **IBM Data Analyst Professional Certificate** program, specifically the **Data Analysis with Python** course. It demonstrates practical application of data analysis techniques to solve real-world business problems in the real estate domain.

## 📝 License

This project is for educational and portfolio purposes. The dataset is publicly available on Kaggle under the [CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/) license.

## 🙏 Acknowledgments

- **IBM** for the comprehensive Data Analysis with Python course
- **Coursera** for the learning platform
- **Kaggle** for providing the House Sales in King County dataset
- The open-source community for amazing Python data science libraries

## 🫱🏿‍🫲🏿 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/yourprofile)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/yourusername)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF6B6B?style=for-the-badge&logo=about.me&logoColor=white)](https://yourportfolio.com)

---

⭐ **If you find this project helpful, please give it a star!** ⭐

*Last updated: December 2025*
