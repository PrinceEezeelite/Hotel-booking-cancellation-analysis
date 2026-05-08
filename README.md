## 🏨 Hotel Booking Cancellation Analysis

## Project Background

Hotels frequently experience booking cancellations, leading to:

Revenue loss
Inefficient room allocation
Poor operational forecasting

In this project, I analyzed hotel booking data to uncover the major drivers of booking cancellations and built a machine learning model capable of predicting high-risk cancellations.

## The project combines:

Data Cleaning
Exploratory Data Analysis (EDA)
Business Insight Generation
Predictive Modeling
## Business Problem

Hotel cancellations create uncertainty in:

Revenue management
Staffing
Customer planning
Inventory allocation

## The objective of this project was to:

Identify patterns behind booking cancellations
Understand customer behavior
Build a predictive model to detect high-risk bookings
Generate actionable business recommendations
## Dataset Information
### Dataset Used:

Hotel Booking Demand Dataset

## Dataset Includes:
Booking information
Customer demographics
Reservation channels
Deposit types
Lead time
Room allocation
Cancellation status
## Tools & Technologies
Tool	Purpose
Python	Data analysis & modeling
Pandas	Data cleaning
NumPy	Numerical operations
Matplotlib	Data visualization
Seaborn	Exploratory analysis
Scikit-learn	Machine learning
Jupyter Notebook	Development environment
GitHub	Version control & portfolio

---

## 📅 Week 1: Data Cleaning & Preparation

### 🔍 Objective
Prepare raw booking data for analysis by ensuring data quality, consistency, and usability.

---

## 🧹 Data Cleaning

### ✔️ Missing Values Handling
- `agent` and `company` → filled with **0** (no agent/company involved)
- `country` → filled with **"Unknown"**
- `children` → filled with **0** and converted to integer

### ✔️ Data Validation
- Removed records with **zero guests** (invalid bookings)
- Verified data types across all columns

### ✔️ Outlier Treatment
- Removed extreme values in `adr` (Average Daily Rate)
- Filtered negative and unrealistic pricing values

---

## ⚙️ Feature Engineering

The following features were created to enhance analysis:

- `total_nights` → total stay duration  
- `total_guests` → total number of guests  
- `is_family` → identifies family bookings  
- `has_changes` → indicates booking modifications  

---

## Outcome:

A structured and analysis-ready dataset suitable for EDA and machine learning.


## Week 2 — Exploratory Data Analysis (EDA)
The second phase focused on discovering patterns and business insights behind booking cancellations.
Analyses Performed:


Booking cancellation trends


Lead time analysis


Deposit type impact


Market segment behavior


Customer type analysis


Length of stay analysis


Special requests analysis


Correlation heatmap analysis



## 📊 Key Insights
🔹 Lead Time
Customers who booked far in advance showed significantly higher cancellation rates.

🔹 Special Requests
Customers with more special requests were far less likely to cancel, indicating stronger booking commitment and engagement.

🔹 Deposit Type
Bookings without deposits experienced the highest cancellation rates.

🔹 Online Travel Agents (OTA)
Bookings made through online travel agencies showed increased cancellation behavior compared to direct bookings.

🔹 Previous Cancellations
Customers with a history of cancellations were more likely to cancel future bookings.

## 💡 Business Insight

The analysis revealed that customer engagement, booking behavior, and reservation policies strongly influence cancellation risk.
## Hotels can reduce cancellations by:


Encouraging deposit-based bookings


Monitoring long lead-time reservations


Improving OTA booking retention strategies


Encouraging personalized booking experiences



## Week 3 — Machine Learning Modeling
The final phase focused on building a predictive model capable of identifying high-risk cancellations.

## 🤖 Model Development Process
## Steps Performed:


Feature selection


Categorical variable encoding


Train-test split


Feature scaling using StandardScaler


Logistic Regression model training


Performance evaluation



## 📈 Model Evaluation
Evaluation Techniques:


Confusion Matrix


Classification Report


ROC Curve


AUC Score


Feature Importance Analysis



## Model Performance
MetricScoreAccuracy76%Recall (Cancellation Detection)79%AUC Score0.85

## Model Interpretation
The model demonstrated strong ability to distinguish canceled bookings from non-canceled bookings.
Most Influential Features:


Lead Time


Previous Cancellations


Deposit Type


Online Travel Agents


ADR (Average Daily Rate)



## ROC Curve Analysis
The ROC Curve achieved an AUC score of 0.85, indicating strong classification performance and reliable separation between canceled and non-canceled bookings.

## Business Recommendations
## Based on the findings:
- Recommendation 1
Implement stricter policies for high lead-time bookings.
- Recommendation 2
Encourage non-refundable or partial deposit bookings.
- Recommendation 3
Improve customer engagement through personalized booking options.
- Recommendation 4
Develop retention strategies for OTA customers.
- Recommendation 5
Use predictive systems to proactively identify high-risk cancellations.

## Project Structure
Hotel-booking-cancellation-analysis/
│
├── data/
│
├── notebooks/
│  
└── Hotel_booking_analysis.ipynb
│
├── dashboard/
│
├── images/
│
└── README.md

## Project Visuals
## Exploratory Data Analysis
<img width="567" height="453" alt="Cancellation Rate by Lead Time Group" src="https://github.com/user-attachments/assets/e4238e0c-a459-4920-a0ae-9d594a76e0a7" />

<img width="846" height="620" alt="Cancellation Rate by Market Segment" src="https://github.com/user-attachments/assets/585d93a2-43fa-4ea6-9b93-e85a2346f89a" />

<img width="589" height="453" alt="Cancellation Distribution" src="https://github.com/user-attachments/assets/a3e563b6-de98-47c7-a807-65a98529a2ae" />

## ROC Curve
<img width="691" height="545" alt="roc_curve" src="https://github.com/user-attachments/assets/d17b62b9-75a7-4935-a8dd-ca42d342665a" />


## Feature Importance
<img width="304" height="204" alt="Features important" src="https://github.com/user-attachments/assets/1d3a33ca-106e-4400-8c38-46eade9187c4" />


## Future Improvements


Random Forest & XGBoost models


Hyperparameter tuning


Interactive dashboard development


Real-time prediction deployment


Streamlit web application



## Author
PrinceEezeelite
## Aspiring Data Analyst focused on:


Data Analytics


Machine Learning


Business Intelligence


Data-driven decision making



## Project Status
✅ Completed
✅ Portfolio Ready
✅ Open for collaboration and feedback

