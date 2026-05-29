# 🚲 Bike Sales Demographics Analysis

## 🎯 Project Overview
This project analyzes consumer demographics to identify the key driving factors behind bicycle purchases. By processing and analyzing a dataset of 1,000 potential customers, this project uncovers actionable insights into how income, commute distance, age, and education influence buying behavior. 

This repository serves as a showcase of end-to-end data processing, from raw data ingestion to executive dashboarding using the `Bike_Demonogrpahics_Analysis.xlsx` dataset.

## 🛠️ Skills & Competencies Demonstrated
* **Data Management (ETL):** Ingested raw datasets, established version control (Original vs. Working data), and maintained data integrity throughout the pipeline.
* **Data Cleaning & Feature Engineering:** Standardized categorical variables for consistency (e.g, ensured all data was formatted consistently) and engineered new features (e.g., segmenting raw ages into "Age Brackets") to improve analytical grouping.
* **Exploratory Data Analysis (EDA):** Utilized pivot tables and cross-tabulation to identify trends, correlations, and outliers across demographic segments.
* **Data Visualization & Storytelling:** Designed an interactive dashboard to translate complex data aggregations into intuitive, high-level business insights for non-technical stakeholders.

## 🗂️ Data Architecture & Pipeline
The project follows a structured data pipeline across four distinct stages:

1. **Original Data:** The raw, untouched dataset containing 1,000 records and 13 demographic variables (Marital Status, Gender, Income, Children, Education, Occupation, Home Owner, Cars, Commute Distance, Region, Age, Purchased Bike).
2. **Data Cleansing:** 
   * **Formatting:** Expanded abbreviated values (e.g., converting 'M'/'S' to 'Married'/'Single' and 'M'/'F' to 'Male'/'Female') to ensure clean visualization labels.
   * **Feature Engineering:** Created an `Age Brackets` column (Adolescent, Middle Age, Old) using nested logic to group continuous age data into discrete categorical bins for better demographic profiling.
3. **Exploratory Analysis:** Aggregated data to calculate key metrics, such as Average Income by Gender/Purchase Status and Total Purchase Counts mapped against Commute Distance.
4. **Executive Reporting:** A centralized, visual presentation layer built on top of the pivot tables, allowing for dynamic slicing and filtering of the data. 

## 📊 Key Insights & Business Value
Based on the demographic analysis, several key purchasing behaviors were identified:
* **Income Correlation:** There is a positive correlation between average income and bike purchases. For example, males who purchased bikes had an average income of ~$60,123, compared to ~$56,208 for those who did not.
* **Age Bracket:** The group most likely to purchase a bike was the middle aged section (31-54). Some reasons for the middle aged group has the largest amount of people purchsing bikes might be phyical and fincancial abilites. 
* **Commute Distance Impact:** Commute distance is a strong predictor of purchase likelihood. Consumers with a short commute (0-1 Miles) are highly likely to purchase a bike (200 Yes vs. 166 No), whereas likelihood drops significantly as commute distance increases (e.g., More than 10 miles: 33 Yes vs. 78 No).

## 🚀 Future Scope (Data Science Integration)
To further evolve this project from Data Analysis to Predictive Data Science, the following next steps could be implemented:
* **Predictive Modeling:** Train a classification algorithm (e.g., Logistic Regression or Random Forest) on the demographic features to predict the likelihood of a new customer purchasing a bike (Binary Classification: `Yes`/`No`).
* **Customer Clustering:** Apply K-Means clustering to segment customers into distinct marketing personas based on their income, age, and commute distance.

## 💻 How to Use
1. Download the `Bike_Demonogrpahics_Analysis.xlsx` file to view the complete pipeline.
2. Navigate to the **Working Data** tab to view the data cleaning logic.
3. Interact with the **Dashboard** tab using the provided slicers to filter the visualizations by specific demographic constraints.
