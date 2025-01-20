# Bike Buyers Analysis

## Project Overview
This project involves analyzing a dataset of bike buyers to uncover trends and insights using Microsoft Excel. The analysis includes data cleaning, creating pivot tables, visualizations, and implementing interactive slicers for dynamic filtering.

## Dataset
The dataset contains information about individuals, including their marital status, gender, income, education, occupation, and whether they purchased a bike. The raw data is stored in a sheet named `bike_buyers`.

### Key Columns:
- **ID**: Unique identifier for each individual.
- **Marital Status**: Indicates whether the individual is Married or Single.
- **Gender**: Gender of the individual.
- **Income**: Annual income.
- **Children**: Number of children.
- **Education**: Education level.
- **Occupation**: Type of occupation.
- **Home Owner**: Indicates home ownership.
- **Cars**: Number of cars owned.
- **Commute Distance**: Distance traveled for commuting.
- **Region**: Geographic region.
- **Age**: Age of the individual.
- **Purchased Bike**: Indicates whether a bike was purchased.

## Steps Taken

### 1. Data Cleaning
- Removed duplicates, reducing the dataset to 26 rows.
- Standardized values in the `Marital Status` and `Gender` columns:
  - `M` replaced with `Married`, `S` replaced with `Single`.
  - `M` replaced with `Male`, `F` replaced with `Female`.
- Added a new column, **Age Brackets**, to categorize individuals:
  - `Old`: Age > 54
  - `Middle Age`: 31 <= Age <= 54
  - `Adolescent`: Age < 31

### 2. Pivot Tables and Visualizations

#### Pivot Table 1: Average Income by Gender and Purchase Status
- **Rows**: Gender (Female, Male)
- **Columns**: Purchased Bike (No, Yes, Grand Total)
- **Values**: Average of Income
- **Visualization**: Bar plot
![Description of Chart 1](images/Average_Income_by_Gender_and_Purchase_Status.png)

#### Pivot Table 2: Commute Distance by Purchase Status
- **Rows**: Commute Distance (e.g., 0-1 Miles, 1-2 Miles)
- **Columns**: Purchased Bike (No, Yes, Grand Total)
- **Values**: Count of Purchased Bike
- **Visualization**: Line plot
![Description of Chart 1](images/Commute_Distance_by_Purchase_Status.png)

#### Pivot Table 3: Age Brackets by Purchase Status
- **Rows**: Age Brackets (Adolescent, Middle Age, Old)
- **Columns**: Purchased Bike (No, Yes, Grand Total)
- **Values**: Count of Purchased Bike
- **Visualization**: Line plot
![Description of Chart 1](images/Age_Brackets_by_Purchase_Status.png)

#### Additional Pivot Table: Age by Purchase Status
- **Rows**: Individual ages (e.g., 25, 26, ...)
- **Columns**: Purchased Bike (No, Yes, Grand Total)
- **Values**: Count of Purchased Bike

### 3. Interactive Slicers
Added slicers to the dashboard for dynamic filtering:
- **Marital Status**
- **Education**
- **Region**

![Description of Chart 1](images/Dashboard.png)

## Key Insights
- Income trends vary by gender and purchase status, with males generally having higher average incomes.
- Commute distance influences bike purchase decisions, with shorter distances showing higher purchase counts.
- Middle-aged individuals are the most likely to purchase bikes compared to other age brackets.
- Purchase patterns vary significantly across different age groups.

## How to Use
1. Open the Excel file.
2. Navigate to the `Dashboard` sheet to view visualizations.
3. Use slicers to filter data dynamically by marital status, education, or region.
4. Refer to the `Pivot Table` sheet for detailed data summaries.

## Tools Used
- **Microsoft Excel**: Data cleaning, pivot tables, visualizations, and slicers.

## Future Enhancements
- Integrate more advanced visualizations using Power BI or Tableau.
- Perform statistical analysis to validate insights.
- Automate parts of the analysis using Python or VBA.

---
Feel free to reach out for any questions or collaboration opportunities!
