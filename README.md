# 📊 Glassdoor Data Science Jobs — Exploratory Data Analysis

## 📌 Project Overview

This project performs an Exploratory Data Analysis (EDA) of Glassdoor Data Science job listings.

The analysis focuses on understanding job titles, job locations, industries, salary estimates, company ratings, and the relationship between company ratings and salaries.

The dataset was cleaned and analyzed using Python, NumPy, Pandas, and Matplotlib to identify meaningful patterns and business insights.

---

## 🎯 Objectives

- Identify the most common Data Science job titles.
- Find locations with the highest number of Data Science job listings.
- Identify industries with strong Data Science hiring demand.
- Analyze salary patterns.
- Understand company rating distribution.
- Examine the relationship between company ratings and salaries.

---

## 📂 Dataset

**Source:** Kaggle — Glassdoor Data Science Jobs

The dataset contains information about Data Science job listings, including:

- Job Title
- Salary Estimate
- Job Description
- Company Name
- Location
- Headquarters
- Company Size
- Founded Year
- Type of Ownership
- Industry
- Sector
- Revenue
- Company Rating
- Competitors

---

## 🛠️ Tools & Technologies

- Python
- NumPy
- Pandas
- Matplotlib
- Kaggle Notebook

---

## 🧹 Data Cleaning

The following preprocessing steps were performed:

- Checked dataset structure and data types.
- Identified missing values.
- Removed exact duplicate records.
- Converted `-1` values representing unavailable information into missing values where appropriate.
- Cleaned salary estimates.
- Separated annual and hourly salary estimates.
- Extracted minimum and maximum salaries.
- Calculated average salary.
- Created a company age feature.

---

## 📊 Business Questions

### Q1. What are the most common Data Science job titles?

The **Data Scientist** role dominates the job listings, indicating strong demand for core Data Science positions in the dataset.

### Q2. Which locations have the highest number of Data Science jobs?

**San Francisco, CA** has the highest number of listings with **60 jobs**, followed by **New York, NY with 55**.

### Q3. Which industries have the most Data Science jobs?

**Biotech & Pharmaceuticals** leads with **118 job listings**, followed by **IT Services with 99**.

### Q4. What are the salary patterns?

Among annual salary listings:

- Average salary: **$102.35K**
- Average minimum salary: **$82.76K**
- Average maximum salary: **$121.93K**
- Median average salary: **$97K**
- Salary range: **$56.5K–$184K**

### Q5. What is the distribution of company ratings?

The average company rating is **3.88/5**, based on **851 valid ratings**.

### Q6. Does company rating relate to salary?

The analysis does not show a consistent relationship between company ratings and average salaries. A higher company rating does not necessarily correspond to a higher salary.

---

## 🔎 Key Insights

1. **Data Scientist** is the dominant job title in the dataset.
2. **San Francisco** has the highest number of job listings with 60 opportunities.
3. **Biotech & Pharmaceuticals** is the leading industry with 118 listings.
4. Annual Data Science salaries average approximately **$102.35K**.
5. The average company rating is **3.88/5**.
6. Company ratings do not show a consistent relationship with salary.

---

## 💼 Business Recommendations

- Focus on developing strong core Data Science skills.
- Consider major employment hubs such as San Francisco and New York.
- Explore opportunities across technology, healthcare, pharmaceutical, insurance, and consulting industries.
- Compare salaries across roles, locations, and industries.
- Do not rely solely on company ratings when evaluating job opportunities.
- Develop transferable Data Science skills to increase career opportunities across industries.

---

## 📈 Project Workflow

```text
Raw Dataset
     ↓
Data Loading
     ↓
Data Exploration
     ↓
Data Cleaning
     ↓
Feature Engineering
     ↓
Exploratory Data Analysis
     ↓
Visualization
     ↓
Business Insights
     ↓
Recommendations
     ↓
Conclusion
