# Telco Customer Churn Analysis
> Data preprocessing and customer churn analysis using Python and Pandas.

## 1. Introduction
Customer churn occurs when customers stop using a company's services. This project analyzes the Telco Customer Churn dataset to explore customer characteristics and service-related factors associated with churn.

## 2. Objectives
* Load and inspect the dataset structure.
* Identify and correct attribute data types.
* Convert `Churn` target values from Yes/No to binary 1/0.
* Identify, track, and systematically remove missing null values.
* Explore exploratory relationships between customer attributes and churn rates.

## 3. Tools and Technologies
* **Language:** Python
* **Library:** Pandas, NumPy, Seaborn, Matplotlib
* **Environment:** Kaggle Notebooks / Jupyter Notebooks

## 4. Data Preprocessing
The dataset was processed through a structured cleanup pipeline using Pandas:
1. Checked basic dataset dimensions and column data structures.
2. Formatted `TotalCharges` into a proper numeric decimal data type (`float64`) by trimming structural white spaces.
3. Isolated newly exposed unrecorded billing profiles and removed rows containing missing values (`NaN`).
4. Mapped the `Churn` attribute columns from categorical string descriptors (Yes/No) into standard numeric binary values (1/0).

## 5. Exploratory Data Analysis
The following attributes were systematically analyzed in direct relation to customer churn trends:
* **Demographics:** Gender, Senior citizen status, Partner status, and Dependents.
* **Service Configurations:** Phone service access.
* **Payments & Billing:** Contract terms, Paperless billing selections, and transactional Payment methods.

Churn rates were mathematically calculated for each distinct sub-category and interpreted to map actionable trends in consumer behavior.

## 6. Key Findings
* **Age Impact:** Senior citizens exhibit a significantly higher attrition risk, churning at nearly double the rate of younger customer segments.
* **Household Setup:** Customers living without partners or dependents are noticeably less loyal and maintain higher relative churn rates.
* **Commitment Windows:** Month-to-month service contracts represent the single highest churn risk across the entire enterprise portfolio. Customers on 1-year or 2-year contracts show excellent retention.
* **Billing Channels:** Customers utilizing manual Electronic Checks drop service plans at a drastically higher rate than any other payment demographic analyzed.
* **Neutral Factors:** Variations in customer gender profiles and basic phone service availability showed minor, negligible differences in final churn margins.

## 7. Dataset Information
* **Source Archive:** [Telco Customer Churn Dataset on Kaggle](https://kaggle.com)
* **File Structure:** Local CSV integration parsed via Pandas DataFrame engines.

## 8. Conclusion
The analysis successfully isolated several core customer characteristics tied closely to heightened attrition patterns, particularly highlighting contract binding type and payment methods. These operational findings can directly assist a company in building targeted retention strategies for high-risk customer pools. Note that while strong statistical associations were observed, these correlations do not explicitly prove direct baseline causation.
