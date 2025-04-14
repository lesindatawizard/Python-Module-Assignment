# Python-Module-Assignment

# Overview

This project analyzes NBA player statistics with a focus on salary distribution patterns. The dataset contains 458 players with attributes including team affiliation, position, age, height, weight, and salary information. The analysis provides insights into team compositions, salary expenditures, and demographic distributions across the league.

# Dataset Characteristics

1. Source: Synthetic NBA player dataset
2. Records: 458 players
3. Original Features:
   1. Name, Team, Number, Position
   2. Age, Height, Weight
   3. College, Salary
4. Missing Values: 11 salary entries

# Preprocessing Steps

1. Height Standardization:
   1. Replaced inconsistent height values with random integers between 150-180 cm
   2. Added derived height in feet for better interpretability

2. Salary Imputation:
   1. Identified 11 missing salary values
   2. Replaced nulls with median salary ($5,837,145)
   3. Preserved original distribution by using median (robust to outliers)

3. Data Cleaning:
   1. Removed irrelevant 'College' column
   2. Converted age to integer type
   3. Verified no remaining null values after processing

# Analysis Tasks

1. Team Distribution Analysis
   1. Calculated absolute counts and percentage shares per team
   2. Identified largest teams (Boston Celtics, Brooklyn Nets)
   3. Found several smaller-market teams with <5% representation

2. Position Analysis
   1. SG (Shooting Guard) most common position (23.8%)
   2. Center position shows highest salary expenditure despite fewer players
   3. Point Guards show strongest age-salary correlation

3. Age Demographics
   1. Predominant age group: 26-30 years (42.6%)
   2. Significant drop-off after age 35 (only 8.3%)
   3. Weak positive age-salary correlation (r=0.22)

4. Salary Expenditures
   1. Highest spending team: Cleveland Cavaliers ($149M)
   2. Most expensive position: Power Forward ($68M total)
   3. Notable outliers among top salaries influence distributions

5. Salary - Age Correlation Analysis
   1. Salaries generally increase with age but with high variability
   2. Peak earnings typically occur between ages 28-32

# Key Visualizations

1. Team Distribution Bar Chart
   1. Shows how many players are on each team
   2. Tallest bars = teams with most players

2. Position Breakdown Horizontal Bars
   1. Lists all player positions sideways
   2. Longer bars = more players in that position

3. Age Group Histogram
   1. Columns show how many players are in each age group
   2. Highest column = most common age range

4. Salary Spending Chart
   1. Compares total salaries by team and position
   2. Darker/brighter colors = higher spending

5. Age vs Salary Dots
   1. Each dot = one player
   2. Trend line shows if older players generally earn more
   3. Dots higher up = higher salaries

# Key Insights:

1. Team Distribution: The company has employees distributed across various teams, with some teams being significantly larger than others.
2. Position Segregation: The most common position is SG with 102 employees.
3. Age Group: The predominant age group is 18-25 with 200 employees.
4. Salary Expenditure: The team with highest salary expenditure is Cleveland Cavaliers ($109,824,875.00), and the position is C ($466,377,332.00).
5. Age-Salary Correlation: The correlation between age and salary is 0.21, indicating a positive relationship.
Technical Implementation
Environment: Jupyter Notebook (Python 3.8+)

# Libraries:

1. pandas (data manipulation)
2. numpy (numerical operations)
3. matplotlib/seaborn (visualization)
4. scipy (statistical analysis)
