# 🏨 Hotel Booking Cancellation & Pricing Analysis

## 📌 Project Overview
This project analyzes hotel booking data to uncover the key drivers behind customer cancellations and pricing behavior. The goal is to provide actionable insights that can help revenue managers reduce cancellations and optimize pricing strategies.

---

## 🎯 Business Problem
In the hospitality industry, high cancellation rates lead to significant revenue loss. Hotels need to understand:
- Why customers cancel bookings
- Which customer segments are high-risk
- How pricing and seasonality affect demand

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

## 🛠️ Tools & Technologies
- Python (Pandas, NumPy)
- Jupyter Notebook
- GitHub (Version Control)

---

## 📊 Key Outcome
A clean, structured dataset ready for:
- Exploratory Data Analysis (EDA)
- Customer segmentation
- Predictive modeling (churn prediction)

---

## 📁 Project Structure
  project/
│
├── data/
├── notebooks/
├── images/
├── dashboard/
├── README.md
