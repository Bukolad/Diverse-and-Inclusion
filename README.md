# Diverse-and-Inclusion

## Table of Contents
 - [Project Overview](#project-overview)
 - [Objectives](#objectives)
 - [Type of Analysis used](#type-of-analysis-used)
 - [Data Cleaning & Preparation](#data-cleaning-&-preparation)
 - [Snapshot of KPIs](#snapshot-of-kpis)
 - [Snapshot of Visual Filter](#snapshot-of-visual-filter)
 - [Snapshot of Multi-Row Card](#snapshot-of-multi-row-card)
 - [Insights](#insights)
 - [Recommendation](#recommendation)
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
     ## Snapshot of KPIs
  ![image](https://github.com/user-attachments/assets/72b9ef11-1b30-485f-b772-a3362ae1fbaa)

  
- Step 5: Visual filters were added to the report for the fields (Department,Region Group,Age Group,Job Level)
  ## Snapshot of Visual filters
  ![image](https://github.com/user-attachments/assets/a75034ed-79da-483c-ab3a-8c446605c90f)

  
- Step 6: Line and stacked column chart were included in Report design
  - Both chart represent the Promotion for Female and Male after FY20
- Step 7:Line Chart was created to visualize Female and Male Turnover Rate for FY20
- Step 8: Multi-rows card was added to display - % of female and male hires
                                               - Average performance rating of female and male
                                                - Turnover Rate
  ## Snapshot of Multi-rows card
  ![image](https://github.com/user-attachments/assets/7c2eba68-a6ad-45aa-bdfa-1d322afdd2f4)

  # Insights
  - Female representation declines significantly at senior levels (Director and Executive positions).
  - Male employees have a higher turnover rate compared to female employees for FY20.
  - Turnover rates are higher at junior levels, indicating career advancement challenges.
  - Fewer women are promoted compared to men, especially at senior levels, despite similar performance ratings.
  - Hiring is nearly balanced between male and female employees, but more attention is needed at senior roles to improve gender diversity.

   # Recommendation
  - Implement targeted leadership development programs for women.
  - Focus on internal promotions and mentorship opportunities for female employees.
  - Conduct exit interviews to understand and address reasons for employee turnover.
  - Regularly review promotion criteria to eliminate potential biases.
   - Introduce transparent promotion policies and provide equal growth opportunities for all employees.
   - Set diversity hiring targets, especially for leadership roles.
   - Report findings regularly to stakeholders to promote accountability.

  
