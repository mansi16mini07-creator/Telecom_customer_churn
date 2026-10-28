# 📊 Telecom Customer Churn Prediction

## 📌 Project Overview

Telecom Customer Churn Prediction is a data analysis and machine learning project that aims to identify customers who are likely to discontinue their telecom services. Customer churn is a significant challenge for telecommunications companies because losing existing customers can reduce revenue and increase customer acquisition costs.

This project uses a telecom customer churn dataset containing **7,043 rows and 38 columns** to analyze customer behavior, identify factors associated with churn, visualize important patterns, and develop machine learning models to support customer retention strategies.

The project combines Exploratory Data Analysis (EDA), data preprocessing, statistical hypothesis testing, data visualization, and machine learning to transform raw customer data into actionable business insights.

## 🎯 Objectives

- Understand customer demographics, account information, and service usage.
- Clean and preprocess the dataset for reliable analysis.
- Perform Exploratory Data Analysis (EDA) to identify patterns and trends.
- Visualize customer churn and its associated factors.
- Apply statistical tests to investigate relationships between customer attributes and churn.
- Build and evaluate machine learning models for churn prediction.
- Identify customers who may be at risk of leaving.
- Recommend strategies to improve customer retention.

## 📂 Dataset Description

The project uses a telecom customer churn dataset containing **7,043 records and 38 columns**.

The dataset includes information about customer services, account details, charges, and churn behavior.

### Important Features

| Feature | Description |
|---|---|
| Customer ID | Unique identifier for each customer |
| Gender | Customer's gender |
| Age | Customer's age |
| Tenure in Months | Duration of the customer's relationship with the company |
| Contract | Type of customer contract |
| Monthly Charge | Monthly amount charged to the customer |
| Total Revenue | Total revenue generated from the customer |
| Internet Type | Type of internet service used |
| Multiple Lines | Whether the customer has multiple phone lines |
| Online Security | Availability of online security services |
| Online Backup | Availability of online backup services |
| Device Protection Plan | Whether device protection is included |
| Premium Tech Support | Availability of premium technical support |
| Streaming TV | Whether the customer uses streaming TV |
| Streaming Movies | Whether the customer uses streaming movies |
| Churn Category | Category associated with customer churn |
| Churn Reason | Reported reason for customer churn |
| Customer Status | Whether the customer stayed, churned, or joined |

*Note: Confirm the exact feature names against your dataset, as column names can differ between telecom churn datasets.*

## 🛠️ Technologies Used

- **Python** — Data analysis and model development
- **Pandas** — Data manipulation and preprocessing
- **NumPy** — Numerical computations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **SciPy** — Statistical hypothesis testing
- **Scikit-learn** — Machine learning and model evaluation
- **Jupyter Notebook** — Interactive development and documentation
- **Git and GitHub** — Version control and project hosting

## 🔄 Project Workflow

### 1. Data Acquisition
- Load the telecom customer churn dataset.
- Examine its dimensions, columns, and data types.
- Understand the meaning of important variables.

### 2. Data Cleaning and Preprocessing
- Check for missing values and duplicate records.
- Correct inappropriate data types.
- Handle missing and inconsistent values.
- Standardize categorical values where necessary.
- Encode categorical features for machine learning.
- Prepare the target variable for model training.
- Separate features and target variables.

### 3. Exploratory Data Analysis (EDA)
- Analyze the distribution of customer status.
- Explore customer demographics and service usage.
- Examine contract types and customer tenure.
- Investigate monthly charges and total revenue.
- Identify patterns associated with customer churn.
- Use summary statistics and visualizations to understand the data.

### 4. Data Visualization
Visualizations help communicate the findings to both technical and non-technical audiences.

Examples include:
- Customer status distribution.
- Churn by contract type.
- Monthly charges by churn status.
- Churn category distribution.
- Customer tenure and churn patterns.
- Correlation heatmap for relevant numerical variables.

### 5. Statistical Hypothesis Testing
Statistical tests can help investigate whether customer characteristics differ across churn groups.

Possible techniques include:
- **Independent-samples t-test:** Compare mean monthly charges between churn groups.
- **Chi-square test:** Examine associations between categorical variables and churn.
- **ANOVA:** Compare mean values across multiple customer groups when its assumptions are satisfied.

The results are interpreted using appropriate significance levels and the assumptions of each test.

### 6. Machine Learning Model Development
Machine learning models can identify patterns in historical customer data and estimate the likelihood of churn.

Potential models include:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

The workflow includes:
1. Selecting relevant input features.
2. Splitting the dataset into training and testing sets.
3. Encoding categorical variables and scaling numerical features when required.
4. Training the selected models.
5. Generating predictions on unseen test data.
6. Comparing model performance.

### 7. Model Evaluation

Model performance can be evaluated using:

| Metric | Purpose |
|---|---|
| Accuracy | Measures the proportion of correct predictions |
| Precision | Measures how many predicted churn cases are actual churn cases |
| Recall | Measures how many actual churn cases are correctly identified |
| F1-score | Balances precision and recall |
| Confusion Matrix | Shows correct and incorrect predictions for each class |
| ROC-AUC | Measures the model's ability to distinguish between classes |

For churn prediction, precision and recall are particularly important because incorrectly identifying customers can affect retention costs and business decisions.

### 8. Business Recommendations

The analysis can help telecom companies:

- Identify customer groups with higher churn rates.
- Investigate the relationship between contract types and churn.
- Review pricing and service issues associated with customer dissatisfaction.
- Develop targeted customer retention campaigns.
- Improve customer support and service quality.
- Prioritize retention efforts using model predictions.

Recommendations should be based on the actual results obtained from the dataset.

## 📈 Key Insights

The analysis aims to answer the following questions:

- What proportion of customers have churned?
- Which customer groups show higher churn rates?
- How are contract types associated with customer churn?
- Does monthly spending differ between churned and retained customers?
- Which services are associated with customer retention?
- How accurately can machine learning models identify customers at risk of churn?

**Note:** Add your actual findings and model evaluation scores after completing the analysis. Avoid reporting unverified results.

## 📁 Project Structure

A suggested repository structure is:

```text
Telecom-Customer-Churn/
│
├── data/
│   └── telecom_customer_churn.csv
│
├── notebooks/
│   ├── 01_data_cleaning_and_eda.ipynb
│   ├── 02_data_visualization.ipynb
│   ├── 03_statistical_hypothesis_testing.ipynb
│   └── 04_machine_learning_model.ipynb
│
├── visualizations/
│   ├── customer_status_distribution.png
│   ├── churn_by_contract.png
│   └── confusion_matrix.png
│
├── README.md
├── requirements.txt
└── .gitignore
```

*Adjust the folder and file names to match your actual repository.*

## ⚙️ Installation and Setup

### Prerequisites
- Python 3.10 or a compatible version.
- Jupyter Notebook or Visual Studio Code.
- Git, if you want to clone the repository.

### Step 1: Clone the Repository

```bash
git clone <your-github-repository-url>
```

### Step 2: Navigate to the Project Directory

```bash
cd Telecom-Customer-Churn
```

### Step 3: Create a Virtual Environment (Optional)

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### Step 4: Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn jupyter
```

### Step 5: Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the relevant notebook and execute the cells in sequence.

## 📋 Requirements File

Create a `requirements.txt` file containing:

```text
pandas
numpy
matplotlib
seaborn
scipy
scikit-learn
jupyter
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```

## ⚠️ Limitations

- Model performance depends on the quality and representativeness of the dataset.
- Historical customer behavior may not fully reflect future behavior.
- Class imbalance can affect the detection of churned customers.
- Correlation and statistical association do not necessarily establish causation.
- Model predictions are estimates and should not be treated as certain outcomes.
- Actual performance must be evaluated on unseen data before practical deployment.

## 🚀 Future Enhancements

- Develop an interactive Streamlit dashboard for customer churn analysis.
- Add customer-level churn probability predictions.
- Compare additional machine learning algorithms.
- Apply cross-validation and hyperparameter tuning.
- Investigate feature importance and model explainability using SHAP.
- Deploy the trained model as a web application.
- Develop targeted retention strategies based on model predictions.

## 👩‍💻 Author

**Mansi Mishra**

B.Tech Student | Aspiring Data Analyst & Data Scientist

GitHub: [Visit My GitHub Profile](https://github.com/mansi16mini07-creator)

## 📄 License

This project is intended for educational and analytical purposes. If you redistribute the dataset, follow its original license and terms of use. Consider adding an MIT License or another appropriate license to your own code if you want others to reuse it.

## ⭐ Acknowledgements

Thanks to the providers of the publicly available telecom customer churn dataset and the open-source Python community for the tools used in this project.
