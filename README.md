# Analyzing Startup Ecosystem and Funding Trends in India

This project explores the Indian startup landscape using real-world funding data. It combines data cleaning, statistical analysis, visualization, SQL queries, and machine learning to uncover insights into industry trends, city-wise growth, investor behavior, and funding prediction.

---

##  Objective

To analyze startup funding trends in India and:
- Identify top industries, cities, and investors
- Discover yearly and sectoral funding patterns
- Detect funding outliers and variability
- Predict funding amounts using machine learning
- Provide data-driven insights to aspiring founders, investors, and analysts

---

##  Dataset

**Source:** [Startup Funding in India – Kaggle](https://www.kaggle.com/datasets/sudalairajkumar/indian-startup-funding)  
**Key Columns:**
- `Startup Name`, `Industry Vertical`, `SubVertical`, `City Location`
- `Investors Name`, `Investment Type`, `Amount in USD`, `Date`, `Remarks`

---

##  Project Structure

### 🧹 Section A: Python & Data Cleaning
- Load dataset, inspect structure & datatypes
- Clean and convert:
  - `Date` to datetime format
  - `Amount in USD` to numeric
- Standardize:
  - `City Location`, `Industry Vertical`, `Investment Type`
- Add new columns:
  - `Year`
  - `Funding Category` (Low, Medium, High)
  - `Number of Investors`

---

###  Section B: SQL Operations
Performed on cleaned data:
- Top 10 most funded startups
- Cities with highest total and average funding
- Yearly startup count by investment type
- Most frequent investor-city combinations
- Industries with highest median funding

---

###  Section C: EDA & Statistical Analysis

####  Visualizations
- Startup count per city and industry (bar plot)
- Total funding per year (line plot)
- Funding distribution across cities (box plot)
- Investment type distribution (pie chart)
- Word cloud of top investors
- Count plot by funding round
- Correlation heatmap

####  Descriptive Statistics
- Mean, median, standard deviation of funding
- Summary tables: average funding per industry per year
- Coefficient of Variation (CV) by city and industry
- Most stable vs most volatile funding regions
- IQR and outlier detection
- Top 3 sectors by median funding post-2018

---

###  Section D: Tableau Dashboard
**Source:** https://public.tableau.com/views/StartupTrendsAnalysis/StartupTrendsAnalysis?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

Interactive dashboard includes:
- Filters (industry, city, year, funding type)
- Time series of total funding
- Bar chart: average funding per industry
- Top 10 investors with sector view
- Scatter: funding vs number of investors
- Map: city-wise funding
- Investor click-tracker for startup visibility

---

###  Section E: Machine Learning

####  Regression Task
**Goal:** Predict `Amount in USD` using:
- `Industry Vertical`, `City`, `Investment Type`, `Year`, `Number of Investors`

**Models:**
- Linear Regression
- Random Forest Regressor
- XGBoost (optional)

####  Classification Task
**Goal:** Classify startups as `Low`, `Medium`, `High` funded

**Steps:**
- Label encode categorical columns
- Train using:
  - Decision Tree
  - Logistic Regression
  - Random Forest
- Evaluate with accuracy and feature importance

---


##  Contributors

- Anshul Rawat  
- Hitesh Kumar  
- Akul Khandelwal  
- Amit Raj  
- Tannu Rana  
- Nisha  
- Anjali  

---

## 📎 License

This project is for educational and academic purposes. Data is open-sourced under Kaggle's dataset license.

