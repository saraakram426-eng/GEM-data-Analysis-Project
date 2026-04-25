# GEM-data-Analysis-Project
This project analyzes global fitness trends using Google Trends data. The analysis focuses on data cleaning, time-series preparation, and geographic data processing to identify how workout interests evolve over time and vary across different regions.  Below is the project description and a professional README tailored to the specific tasks
💎 Global Fitness Trend Analysis
📊 Project Overview
This repository contains a Python-based data analysis project that cleans and prepares fitness search trend data. The project handles global time-series data and regional geographic data to provide a clean slate for trend visualization and insight generation.

📂 Data Sources
The analysis utilizes four primary datasets:

workout.csv: Global "workout" search interest by month (2018–2023).

workout_geo.csv: Workout interest distributed by country.

three_keywords.csv: Comparative search interest for three specific fitness keywords.

three_keywords_geo.csv: Geographic distribution of interest for the three keywords.

🛠️ Tech Stack
Language: Python

Libraries: pandas (Data Manipulation), numpy (Numerical Operations), matplotlib & seaborn (Visualization).

Environment: Jupyter Notebook / Google Colab.

🧼 Cleaning & Preprocessing Steps
The following operations were performed to ensure data integrity:

Type Conversion: The month column in the global dataset was converted from a string object to a datetime64 object to enable time-series sorting and filtering.

Missing Value Handling: In the geographic dataset (workout_geo.csv), 189 null values were identified in the workout_2018_2023 column. These were imputed with 0, representing regions with no significant recorded search activity.

Integrity Checks: Each file was audited for duplicate rows and inconsistent data types to prevent skewed results during the aggregation phase.

📈 Summary Statistics (Example: Global Workouts)
Based on the cleaned global data:

Average Interest Score: ~56.7

Peak Interest: 100.0 (representing the highest relative search volume)

Data Range: March 2018 to March 2023

🚀 How to Run
Clone the repository.

Ensure you have the datasets (.csv files) in the root directory or update the file paths in the notebook.

Install dependencies:

Bash
pip install pandas numpy matplotlib seaborn
Open Gem_Project.ipynb in your preferred Jupyter environment and run the cells.
