# 💼 Glassdoor Data Science Jobs — Exploratory Data Analysis

---

## 📌 Project Overview

The Data Science job market has grown across industries, locations, and company types, creating opportunities for professionals with analytical and technical skills.

This project performs an Exploratory Data Analysis (EDA) of Glassdoor Data Science job listings to understand hiring patterns, salary ranges, company ratings, locations, and industry demand.

The analysis was developed using **Python, Pandas, NumPy, and Matplotlib** in a Kaggle Notebook.

---

## 🎯 Business Objective

The objective of this project is to transform Data Science job listing data into meaningful business insights.

The analysis focuses on:

- Data Science job title demand
- Geographic distribution of job opportunities
- Industry-wise hiring demand
- Salary patterns
- Company rating distribution
- Relationship between company ratings and salaries

---

## ❓ Business Questions

This project answers six key business questions:

1. What are the most common Data Science job titles?
2. Which locations have the highest number of Data Science job listings?
3. Which industries have the highest number of Data Science jobs?
4. What are the salary patterns for Data Science jobs?
5. What is the distribution of company ratings?
6. Does company rating relate to salary?

---

## 📊 Dataset

The dataset contains **1,000 Data Science job listings** and 14 variables.

### Key Columns

| Column | Description |
|---|---|
| Job Title | Title of the job listing |
| Salary Estimate | Estimated salary provided by Glassdoor |
| Job Description | Description of the job |
| Rating | Company rating |
| Company Name | Name of the company |
| Location | Job location |
| Headquarters | Company headquarters |
| Size | Company employee size |
| Founded | Company founding year |
| Type of ownership | Company ownership type |
| Industry | Industry classification |
| Sector | Business sector |
| Revenue | Estimated company revenue |
| Competitors | Listed competitors |

Salary estimates include both **annual and hourly** compensation.

---

## 🧹 Data Cleaning

The dataset was inspected and cleaned before performing the analysis.

### Data Quality Findings

- **1,000 records**
- **14 columns**
- **101 duplicate records**
- **62 missing values** in `Rating` after treating `-1` as unavailable
- **167 missing values** in `Founded`
- Salary estimates contained both annual and hourly values

### Cleaning Approach

- Duplicate records were removed.
- `-1` values in `Rating` were treated as unavailable and converted to `NaN`.
- `-1` values in `Founded` were treated as unavailable and converted to `NaN`.
- Salary estimates were cleaned and separated into:
  - `Salary Type`
  - `Min Salary`
  - `Max Salary`
  - `Average Salary`
- Annual and hourly salaries were analyzed separately.
- A `Company Age` feature was created using the founding year.

---

# 📈 Key Findings

## 1️⃣ Most Common Job Titles

**Data Scientist** was by far the most common job title in the dataset.

Other frequently appearing roles included:

- Data Engineer
- Senior Data Scientist
- Data Analyst
- Senior Data Engineer

### 💡 Business Insight

The dominance of Data Scientist listings indicates strong demand for core Data Science positions in the dataset.

For aspiring Data Scientists, developing strong fundamental Data Science skills can provide access to a broad range of opportunities.

---

## 2️⃣ Leading Job Locations

**San Francisco, CA** had the highest number of Data Science job listings:

> **60 job listings**

The Top 10 locations were:

| Location | Job Listings |
|---|---:|
| San Francisco, CA | 60 |
| New York, NY | 55 |
| Cambridge, MA | 34 |
| Chicago, IL | 24 |
| Boston, MA | 23 |
| Washington, DC | 22 |
| Seattle, WA | 21 |
| Richmond, VA | 13 |
| Pittsburgh, PA | 13 |
| Remote | 12 |

### 💡 Business Insight

San Francisco and New York were the leading locations for Data Science opportunities in the dataset.

The concentration of opportunities in major business and technology hubs suggests that location can be an important factor when searching for Data Science jobs.

---

## 3️⃣ Leading Industries

**Biotech & Pharmaceuticals** had the highest number of Data Science job listings:

> **118 job listings**

The Top 10 industries were:

| Industry | Job Listings |
|---|---:|
| Biotech & Pharmaceuticals | 118 |
| IT Services | 99 |
| Unknown (`-1`) | 80 |
| Enterprise Software & Network Solutions | 76 |
| Computer Hardware & Software | 66 |
| Healthcare Services & Hospitals | 47 |
| Insurance Operators | 43 |
| Consulting | 40 |
| Staffing & Outsourcing | 40 |
| Internet | 39 |

> `-1` represents unavailable industry information and is not an actual industry.

### 💡 Business Insight

Data Science opportunities are distributed across several industries, particularly **Biotech & Pharmaceuticals, IT Services, Software, Healthcare, Insurance, and Consulting**.

This highlights the broad applicability of Data Science skills across different business sectors.

---

## 4️⃣ Salary Analysis

The salary analysis focused on **annual salary listings** to avoid mixing annual and hourly compensation.

### Salary Statistics

| Metric | Value |
|---|---:|
| Annual salary listings | **869** |
| Average Minimum Salary | **$82.76K** |
| Average Maximum Salary | **$121.93K** |
| Average Salary | **$102.35K** |
| Median Salary | **$97.00K** |
| Minimum Average Salary | **$56.50K** |
| Maximum Average Salary | **$184.00K** |

### 💡 Business Insight

The average estimated annual salary was approximately:

> **$102.35K**

The salary estimates varied considerably, indicating that compensation can differ based on factors such as job role, location, industry, and company characteristics.

---

## 5️⃣ Company Ratings

The company rating analysis produced the following results:

| Metric | Value |
|---|---:|
| Valid Ratings | **851** |
| Average Rating | **3.88 / 5** |
| Median Rating | **3.90 / 5** |
| Minimum Rating | **1.50 / 5** |
| Maximum Rating | **5.00 / 5** |

### 💡 Business Insight

Companies with available ratings had an average rating of approximately **3.88/5**, indicating generally positive ratings across the dataset.

However, ratings ranged from **1.5 to 5.0**, showing considerable variation between companies.

---

## 6️⃣ Company Rating vs Salary

The analysis compared company ratings with average salary estimates.

Some examples were:

| Company Rating | Average Salary |
|---:|---:|
| 2.6 | $114.67K |
| 4.3 | $111.27K |
| 4.7 | $108.63K |
| 5.0 | $102.65K |
| 4.8 | $92.34K |
| 1.5 | $56.50K |

### 💡 Business Insight

The analysis did **not show a consistent relationship between company rating and salary**.

For example, companies with a rating of **2.6** had a higher average salary than companies with ratings of **4.3, 4.7, and 5.0**.

Therefore, company rating alone should not be used as an indicator of salary level.

---

# 💡 Business Recommendations

Based on the analysis:

### 🎯 1. Focus on Core Data Science Roles

The strong presence of Data Scientist positions indicates that building strong fundamental Data Science skills can create broader career opportunities.

### 🌍 2. Consider Major Employment Hubs

San Francisco, New York, Cambridge, Chicago, and Boston showed strong demand in this dataset.

### 🏭 3. Explore Multiple Industries

Data Science opportunities exist across:

- Technology
- Biotechnology
- Healthcare
- Insurance
- Consulting
- Software

Candidates should avoid limiting their search to a single industry.

### 💰 4. Compare Salary Across Multiple Factors

Salary can vary significantly, so job seekers should compare compensation based on:

- Job title
- Location
- Industry
- Company
- Experience level

### ⭐ 5. Do Not Rely Only on Company Ratings

Company ratings do not show a consistent relationship with salary. Candidates should consider compensation, career growth, company culture, role responsibilities, and location together.

---

# 🛠️ Tools & Technologies

- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Kaggle Notebook**

---

# 📓 Notebook

The complete analysis is available in:

**`Glassdoor_Data_Science_Jobs_EDA.ipynb`**

The notebook contains:

- Data understanding
- Data cleaning
- Missing-value analysis
- Salary feature engineering
- Exploratory data analysis
- 6 business questions
- Data visualizations
- Business insights
- Recommendations
- Conclusion

---

# 📚 References

### Dataset

- Kaggle — **Glassdoor Data Science Jobs Dataset**
- https://www.kaggle.com/datasets/rkb0023/glassdoor-data-science-jobs

### Documentation

- NumPy Documentation — https://numpy.org/doc/
- Pandas Documentation — https://pandas.pydata.org/docs/
- Matplotlib Documentation — https://matplotlib.org/stable/

---

## 👤 Author

**L Shubham**

Aspiring Data Analyst | Python | SQL | Power BI | Excel | Tableau

📍 Pune, Maharashtra, India

### 🔗 Connect With Me

- **GitHub:** https://github.com/shubham-lingam
- **LinkedIn:** https://www.linkedin.com/in/shubham-lingam

---

⭐ **If you found this project useful, consider giving the repository a star!**

Your support motivates me to keep building and sharing Data Analytics projects.

---

<p align="center">
  Built with ❤️ using Python, Pandas, NumPy & Matplotlib
</p>

<p align="center">
  © 2026 L Shubham
</p>
