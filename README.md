# Diverse-and-Inclusion

## Table of Contents
# Project Overview
This projects focuses on analyzing Diversity and Inclusion data using power bi to gain insights into workforce compositions,hiring patterns,promotion and performance ratings. The key objective is to evaluate gender representation ,support strategic decision-making around workforce diversity.
# Objectives
- Monitor promotion and turnover trends to ensure career growth and promote fairness
- Provide data-driven insights to guide recruitment and improve gender diversity in hiring
- Track progress toward organizational diversity and inclusion goals
# Type of Analysis used
Descriptive Analysis : Provides an overview of the current state of diversity and inclusion ,focusing on gender distribution,performance ratings, and turnover rates.
# Data Cleaning & Preparation
- Step 1: load data into Power BI Desktop
- Step 2: Opened Power Query & in view tab under Data Preview section,check 'column distribution" , "column quality" options
- Step 3: Dataset is Cleaned and Error Free
- Step 4: New measures were created to find Total Customers, Total Female and Male, Leavers  and Promoted .
    Total Customers = Total Employee = COUNTA('Pharma Group AG'[Gender])
     Female = CALCULATE(COUNTROWS('Pharma Group AG'),'Pharma Group AG'[Gender]="FEMALE")
      Male = CALCULATE(COUNTROWS('Pharma Group AG'),'Pharma Group AG'[Gender]="MALE")
      Leavers =counta('Pharma Group AG'[Leaver FY])
      Promoted =  CALCULATE(COUNTROWS('Pharma Group AG'),'Pharma Group AG'[Promotion in FY21?]="yes")
- Step 5: Visual filters were added to the report for the fields (Department,Region Group,Age Group,Job Level)
- Step 6: Line and stacked column chart were included in Report design
  - Both chart represent the Promotion for Female and Male after FY20
- Step 7:Line Chart was created to visualize Female and Male Turnover Rate for FY20
- Step 8: Multi-rows card was added to display - % of female and male hires
                                               - Average performance rating of female and male
                                                - Turnover Rate
  
