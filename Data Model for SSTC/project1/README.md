# Project Overview
The goal is to streamline the datasets and develop an effective data model for a small brewing company. This model will help the company analyze which products are popular and profitable, enabling them to make informed decisions about product prioritization as they grow. The project showcases a solid understanding of fundamental data modeling principles, including data cleaning, organization, and structuring in Power Query, creating a date table, building a data model with the appropriate relationships and filters, and generating a straightforward report using common visualizations and DAX measures.

# Project Steps
1. Get Data:
The following files were utilized: CFO Metrics Tracker.xlsx, Customer List (as of FY2021).txt, SSBC Product Offerings.pdf, USD-CAD Exchange Rates.csv, and Monthly Sales Logs, all of which can be found in the Source Files folder of this repository.

2. ETL with Power Query:
We employed Power Query for data cleaning and preprocessing, which included:

   - Merging monthly sales files for enhanced analysis.
   - Combining Customer List (as of FY2021 ).txt and SSBC Product Offerings.pdf.
   - Promoting the first rows to headers.
   - Removing NULL values across all datasets.
   - Renaming queries and columns with descriptive titles.
   - Adjusting column data types to their appropriate formats.
   - Creating a dynamic date table, detailed in the next section.
   - Creating the Date Table:
A date table was generated using Power Query, designed to dynamically update based on the start and end dates of the fact table. This table includes standard fields such as:

Calendar month name and number
Month year
Fy period
Fiscal year
Fiscal period

Fiscal quarter formatted (e.g., Q1 - FY2021)
Note: Seven Sages' fiscal year starts on October 1st and ends on September 30th. For example, a transaction on September 20th, 2020, falls within FY 2020, while one on October 20th would be recorded in FY 2021.

Creating the Data Model (Building Relationships):
We established one fact table and four dimension tables linked to it, creating an active one-to-many relationship.
<img width="706" alt="All tables" src="https://github.com/user-attachments/assets/747aeaf9-3acb-4cf6-81fc-7b04b0402807">
