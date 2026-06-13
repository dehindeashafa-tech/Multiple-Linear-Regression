# Multiple Linear Regression – Marketing ROI Analysis

## 📊 Project Overview

This project performs **Multiple Linear Regression** analysis on a marketing dataset to understand the combined impact of marketing channels (**TV**, **Radio**, **Social Media**) and **Social Media Influencer** tiers (**Nano**, **Micro**, **Mega**) on **Sales**.

The goal is to quantify the ROI of each channel and influencer category, handle categorical variables properly, and provide data-driven recommendations for optimal marketing budget allocation.

### Objectives:
- Load, clean, and preprocess the marketing dataset (including categorical encoding)
- Perform Exploratory Data Analysis (EDA)
- Build and evaluate a **Multiple Linear Regression** model using `statsmodels`
- Handle categorical variable (`Influencer`) with one-hot encoding
- Validate model assumptions (Linearity, Normality, Homoscedasticity, Multicollinearity)
- Interpret coefficients for each channel and influencer tier
- Provide clear ROI-based marketing budget recommendations

---

## 🛠 Technologies Used

- **Python** 3.x
- **pandas** – Data manipulation
- **numpy** – Numerical operations
- **matplotlib & seaborn** – Data visualization
- **statsmodels** – Statistical modeling (OLS regression)
- **scipy** – Statistical tests

---

## 📁 Dataset

The dataset contains marketing spend across different channels and corresponding Sales figures.

**Expected Columns:**
- `TV`, `Radio`, `Social Media`: Budget spent on each channel
- `Influencer`: Categorical variable (Nano, Micro, Mega)
- `Sales`: Revenue generated (target variable)

> **Note:** The code automatically detects and encodes the categorical `Influencer` column. Update column names in the script if yours differ.

---

## 🚀 How to Run the Project

### 1. Setup Environment

```bash
# Create virtual environment (optional)
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate

# Install dependencies
pip install pandas numpy matplotlib seaborn statsmodels scipy
```

### 2. Upload Dataset

- Place your dataset file (e.g., `marketing_data.csv`) in the project folder.
- Or upload it directly in Jupyter Notebook.

### 3. Run the Analysis

Open `marketing_regression_analysis.ipynb` (or the `.py` script) in Jupyter Notebook and run all cells step by step.

**Key Steps Covered:**
1. Load and explore data + handle missing values
2. Exploratory Data Analysis with visualizations
3. One-hot encoding of `Influencer` column (Nano/Micro/Mega)
4. Build Multiple Linear Regression (OLS) model
5. Model diagnostics (residual plots, VIF, statistical tests)
6. Business interpretation of coefficients & ROI recommendations

---

## 📈 Key Insights (Example)

After running the analysis, you will get:

- **Model Performance**: R-squared and Adjusted R-squared
- **Channel Impact**: Coefficients for TV, Radio, and Social Media
- **Influencer Lift**: Coefficients for Micro and Mega vs Nano (baseline)
- **Statistical Significance**: p-values for each predictor
- **Multicollinearity Check**: VIF scores
- **ROI Recommendations**: Prioritize highest-impact channels and influencer tiers

---

## 📋 Project Structure

```
marketing-roi-analysis/
├── README.md
├── marketing_regression_analysis.ipynb     # Main Jupyter Notebook
├── marketing_data.csv                      # Your dataset
├── requirements.txt
└── outputs/                                # Saved plots and results (optional)
```

---

## 🔍 Model Diagnostics

The project includes diagnostic plots to check:
- **Linearity**: Residuals vs Fitted plot
- **Normality**: Q-Q Plot
- **Homoscedasticity**: Scale-Location plot + Breusch-Pagan test

---

## 💼 Business Recommendations

The final section provides actionable insights such as:
- Which channel to prioritize
- Expected ROI
- Budget allocation suggestions
- Next steps (e.g., multiple regression, A/B testing)

---

## 📌 Future Improvements

- Interaction terms (e.g., TV × Mega Influencer)
- Polynomial regression or diminishing returns modeling
- Regularization techniques (Ridge / Lasso)
- Cross-validation and model comparison
- Predictive dashboard for budget simulation
- Advanced visualization of marginal ROI

---

## 👤 Author

Built as a step-by-step learning project for Marketing Analytics using Python.

---

**Feel free to customize this README with your actual results, plots, and findings!**

```

**File Created Successfully!** 🎉

You can now view or download the `README.md` file. 

Would you like me to:
- Generate a full Jupyter Notebook (.ipynb) file with all the code?
- Create a `requirements.txt` file?
- Add sample output images or results section? 

Just let me know!
