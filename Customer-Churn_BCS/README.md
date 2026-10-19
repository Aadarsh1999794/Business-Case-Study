# 📊 Telco Customer Churn Analysis — Exploratory Data Analysis (EDA)

## 📌 Project Overview

Customer churn is a major challenge for telecommunications companies because losing customers can reduce revenue and increase customer
acquisition costs.
This project performs **Exploratory Data Analysis (EDA)** on the IBM Telco Customer Churn dataset to understand customer churn patterns,
identify potentially high-risk customer segments, and develop data-driven business recommendations.
The analysis focuses on customer tenure, monthly charges, payment methods, and internet service types to identify patterns associated
with customer churn.

## 🎯 Business Objectives

- Calculate the overall customer churn rate.
- Identify customer segments with higher churn rates.
- Analyze the relationship between customer tenure and churn.
- Compare monthly charges for customers who churned and those who stayed.
- Investigate churn patterns across payment methods and internet services.
- Translate analytical findings into actionable business recommendations.

## 🛠️ Tools and Technologies

| Tool | Purpose |
|---|---|
| Python | Data analysis and programming |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook | Interactive analysis and documentation |

## 📂 Dataset

**Dataset:** IBM Telco Customer Churn

**Source:** [Kaggle — Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

The dataset contains customer information such as:

- Customer demographics
- Account information and tenure
- Monthly and total charges
- Contract and payment methods
- Internet and additional services
- Customer churn status

The target variable is `Churn`, which indicates whether a customer left the company (`Yes`) or stayed (`No`).

## 🔍 Project Workflow

### 1. Data Loading and Understanding

- Imported the dataset using Pandas.
- Inspected the dataset structure, dimensions, column names, and data types.
- Reviewed descriptive statistics to understand the distribution of numerical variables.

### 2. Data Quality Checks

- Checked for missing values.
- Checked for duplicate rows.
- Reviewed data types and considered potential data-quality issues.

**Results:**
- Missing values reported by `isnull()`: 0
- Exact duplicate rows: 0

*Note: These checks do not rule out blank strings or other data-quality issues.*

### 3. Exploratory Data Analysis

The following areas were investigated:

- Overall churn distribution
- Customer tenure and churn
- Monthly charges by churn status
- Payment method and churn
- Internet service type and churn

### 4. Data Visualization

Visualizations were used to communicate the findings and compare churn rates across customer segments.

Suggested key charts to include in the notebook or repository:

- Overall customer churn distribution
- Churn rate by tenure group
- Average monthly charges by churn status
- Churn rate by payment method
- Churn rate by internet service type

## 📈 Key Findings

### 1. Overall Customer Churn

- Total customers analyzed: **7,043**
- Customers who churned: **1,869**
- Customers who stayed: **5,174**
- Overall churn rate: **26.54%**

Approximately one in four customers in the dataset had churned.

**Business implication:** Customer retention should be monitored as an important business metric.

### 2. Customer Tenure and Churn

| Tenure Group | Churn Rate |
|---|---:|
| 0–12 months | 47.44% |
| 13–24 months | 28.71% |
| 25–48 months | 20.39% |
| 49–60 months | 14.42% |
| 60+ months | 6.61% |

Customers in their first 12 months had the highest observed churn rate, while customers with longer tenure had lower churn rates.

**Business implication:** The first year represents an important opportunity to investigate onboarding, service setup, early support, and the first billing experience.

### 3. Monthly Charges and Churn

| Customer Group | Average Monthly Charges |
|---|---:|
| Customers who stayed | 61.27 |
| Customers who churned | 74.44 |

Customers who churned had higher average monthly charges than customers who stayed.

**Business implication:** Investigate pricing, perceived value, service bundles, and customer expectations to understand whether affordability or value perception contributes to churn.

*The dataset's charge values are reported as provided; the difference alone does not establish that higher charges cause churn.*

### 4. Payment Method and Churn

| Payment Method | Churn Rate |
|---|---:|
| Electronic check | 45.29% |
| Mailed check | 19.11% |
| Bank transfer (automatic) | 16.71% |
| Credit card (automatic) | 15.24% |

Electronic-check customers had the highest observed churn rate among the payment methods analyzed.

**Business implication:** Investigate billing friction, payment failures, payment preferences, and differences in customer profiles. Test whether encouraging automatic payments improves retention before rolling out broad changes.

### 5. Internet Service and Churn

| Internet Service | Churn Rate |
|---|---:|
| Fiber optic | 41.89% |
| DSL | 18.96% |
| No internet service | 7.40% |

Fiber-optic customers had a higher observed churn rate than DSL customers and customers without internet service.

**Business implication:** Investigate service reliability, pricing, installation experience, technical support, and customer satisfaction for fiber-optic customers.

These results identify areas for further investigation; they do not establish the underlying causes of churn.

## 💡 Business Recommendations

Based on the analysis, the following actions are recommended:

1. **Strengthen early customer retention:** Review the onboarding journey and provide proactive support during the first 12 months.
2. **Investigate electronic-check churn:** Analyze billing complaints, payment experiences, and customer characteristics. Test automatic-payment adoption as one possible intervention.
3. **Review fiber-optic customer experience:** Investigate service quality, network issues, installation delays, support tickets, and pricing.
4. **Evaluate pricing and perceived value:** Review customer feedback, plan utilization, and service bundles, particularly among customers with higher monthly charges.
5. **Monitor churn regularly:** Track overall churn and segment-level churn rates over time to detect emerging problems.
6. **Validate recommendations through experiments:** Compare similar customer groups and run controlled retention campaigns to measure actual improvements.

## 📊 Business Impact

This project demonstrates how exploratory data analysis can help a business:

- Identify customer segments that warrant further investigation.
- Prioritize customer retention initiatives.
- Discover patterns related to tenure, billing, pricing, and service types.
- Convert analytical findings into testable business actions.
- Establish a foundation for future churn prediction and customer-retention modeling.

**Important:** The analysis is descriptive. Additional investigation, statistical validation, and controlled experiments are required to confirm causes and measure the effectiveness of retention strategies.

## 🚀 How to Run the Project

### Prerequisites

Install Python and the required libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Steps

1. Clone or download this repository.
2. Download the dataset from the Kaggle source linked above.
3. Place the CSV file in the appropriate project directory.
4. Open the Jupyter Notebook.
5. Update the dataset path in the notebook if required.
6. Run the notebook cells in sequence to reproduce the analysis and visualizations.

Example:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

df = pd.read_csv("WA_Fn-UseC_-Telco-Customer-Churn.csv")

print(df.head())
print(df.shape)
print(df.info())
```

*The CSV filename must match the file you downloaded.*

## 🔮 Future Improvements

Potential extensions to this project include:

- Statistical hypothesis testing to validate observed differences.
- Feature engineering and deeper analysis of customer characteristics.
- Customer churn prediction using Logistic Regression, Decision Trees, and Random Forest.
- Model evaluation using precision, recall, F1-score, ROC-AUC, and a confusion matrix.
- Explainability techniques to identify the strongest predictors of churn.
- A dashboard to monitor churn trends and customer segments.
- Retention campaign experiments to estimate business impact.

## 🏁 Conclusion

The analysis found an overall churn rate of **26.54%**, with notably higher churn among customers in their first 12 months, electronic-check users, and fiber-optic customers.

These findings provide a starting point for investigating customer experience and designing targeted retention initiatives. The next step is to validate the underlying drivers and measure whether specific interventions reduce churn.

This project strengthened my practical skills in Python, Pandas, exploratory data analysis, data visualization, and communicating data-driven business recommendations.


## ⭐ Feedback

Feedback, suggestions, and discussions about the analysis are welcome!

If you find this project useful, consider giving the repository a ⭐ on GitHub.
