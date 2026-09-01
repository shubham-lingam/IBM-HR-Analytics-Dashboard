IBM HR Analytics Dashboard
📌 Project Overview

The IBM HR Analytics Dashboard is an interactive, two-page HR analytics project built using Google Looker Studio. The dashboard analyzes employee attrition, workforce demographics, income, job satisfaction, and other key HR metrics to help identify patterns and support data-driven decision-making.

The project transforms raw HR data into an interactive and visually engaging dashboard designed to provide meaningful insights into employee attrition and workforce trends.

🎯 Project Objectives

The main objectives of this project are to:

Analyze employee attrition patterns.
Understand workforce demographics.
Identify departments and employee groups with higher attrition rates.
Analyze the relationship between attrition and age, income, job satisfaction, and business travel.
Build an interactive and professional HR dashboard using Google Looker Studio.
Apply data visualization and dashboard design best practices.
📊 Dashboard Overview

The dashboard consists of two interactive pages.

🏠 Page 1 — HR Overview

The HR Overview page provides a high-level view of the workforce.

Key Performance Indicators (KPIs)
Total Employee Count
Total Attrition Count
Attrition Rate
Average Monthly Income
Average Employee Age
Visualizations
Attrition Split
Attrition by Department
Employee Count by Job Role
Gender Distribution
Attrition by Business Travel
Interactive Filters
Department
Gender
OverTime

📈 Page 2 — Advanced HR Analysis

The Advanced HR Analysis page provides deeper insights into employee attrition.

Advanced Analysis Includes
Attrition Rate by Department
Attrition Rate by Age Group
Attrition Rate by Income Bracket
Attrition Rate by Job Satisfaction Level
Department × Gender Attrition Analysis
Advanced Visualization

A pivot table with conditional formatting and an IBM-inspired heatmap color scale was used to highlight high and low attrition patterns across departments and genders.

🧮 Calculated Fields

Several calculated fields were created in Google Looker Studio to perform advanced analysis.

Attrition Flag
CASE
  WHEN Attrition = "Yes" THEN 1
  ELSE 0
END
Attrition Rate
SUM(Attrition Flag) / COUNT(EmployeeNumber)

This calculates the percentage of employees who left the organization.

Age Group
CASE
  WHEN Age <= 25 THEN "25 and Below"
  WHEN Age <= 35 THEN "26-35"
  WHEN Age <= 45 THEN "36-45"
  WHEN Age <= 55 THEN "46-55"
  ELSE "56 and Above"
END
Income Bracket
CASE
  WHEN MonthlyIncome < 3000 THEN "Below 3K"
  WHEN MonthlyIncome < 6000 THEN "3K-6K"
  WHEN MonthlyIncome < 9000 THEN "6K-9K"
  WHEN MonthlyIncome < 12000 THEN "9K-12K"
  ELSE "Above 12K"
END
Satisfaction Label
CASE
  WHEN JobSatisfaction = 1 THEN "Low"
  WHEN JobSatisfaction = 2 THEN "Medium"
  WHEN JobSatisfaction = 3 THEN "High"
  WHEN JobSatisfaction = 4 THEN "Very High"
  ELSE "Unknown"
END

📊 Key Insights Explored

The dashboard helps explore questions such as:

Which department has the highest employee attrition?
Which age groups experience higher attrition rates?
Does income level influence employee attrition?
How does job satisfaction relate to employee attrition?
Does business travel impact attrition?
How does attrition vary across departments and genders?
Which job roles have the highest employee count?

🛠️ Tools & Technologies

Google Looker Studio — Dashboard development and visualization
Google Sheets — Data storage and preparation
Microsoft PowerPoint — Dashboard documentation and access link
GitHub — Project documentation and version control

🎨 Dashboard Design

The dashboard follows an IBM-inspired color palette to maintain a professional and consistent visual identity.

Primary Colors
IBM Blue: #0F62FE
Dark IBM Blue: #002D9C
IBM Red (Attrition): #DA1E28
Light IBM Blue: #D0E2FF
Page Background: #F4F4F4

Color Logic

🔴 Attrition = Yes
🔵 Attrition = No
🔵 IBM Blue shades are used for analytical charts
🟦 Blue gradient is used for the attrition heatmap

📁 Repository Structure

IBM-HR-Analytics-Dashboard
│
├── Dataset
│   └── HR Analytics Final Dataset
│
├── Dashboard
│   ├── IBM HR Analytics Dashboard.pdf
│   └── IBM HR Analytics Dashboard.pptx
│
└── README.md

🚀 How to View the Dashboard
Option 1 — View the Dashboard PDF

Open the PDF file available in the Dashboard folder.

Option 2 — Interactive Dashboard

The PowerPoint file contains access to the interactive Google Looker Studio Dashboard.

Open the PowerPoint file and use the provided dashboard link.

💡 Skills Demonstrated

This project demonstrates skills in:

Data Visualization
HR Analytics
Dashboard Development
Google Looker Studio
Data Analysis
Calculated Fields
Data Transformation
KPI Development
Interactive Filtering
Data Storytelling
Dashboard UI/UX Design

📈 Future Improvements

Potential future improvements include:

Adding employee tenure analysis
Adding employee performance analysis
Creating predictive attrition models
Adding drill-down functionality
Adding automated data refresh
Adding additional workforce diversity metrics

👤 Author
Shubham Lingam

Aspiring Data Analyst | Data Visualization | SQL | Python | Tableau | Google Looker Studio

⭐ If you found this project interesting, feel free to star the repository!
