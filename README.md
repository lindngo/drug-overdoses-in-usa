# Drug Overdoses in USA

## Overview
I utilized Google Sheets to do an initial cleaning of the data. I also used visualization techniques on Tableau to create graphs of the data, including bar charts, line graphs, and more.

## Tableau Public Dashboard
https://public.tableau.com/app/profile/lindadngo/viz/usa-drug-overdoses-2/AnalyzingDrugOverdoseDeathsinUSA?publish=yes

## Dataset
[https://raw.githubusercontent.com/zariable/data/master/titanic_train.csv](https://github.com/lindngo/us-drug-overdoses/blob/main/cleaned_drug_overdose_death_rates.xlsx)

## Dataset Factors
See Dataset link above for more details

## Data Cleaning
- 1,112 data rows had * in the Flag column, indicating that these rows had null values in the Estimate column. For a more accurate and insightful analysis, I decided to remove these null values.
- In the Stub Label column, race was always paired with another label, such as sex. In order to do analysis based solely on race, I created a calculated field using "IF ELSE" statements. When creating these statements, I took note that there were two separate Asian labels -- Asian and Asian or Pacific Islander. To make the analysis more cohesive, I combined these two labels under Asian or Pacific Islander.
- Lastly, I wanted to better understand how drugs affected specific demographic groups. The current dataset called for new metrics to be created in order to complete this analysis. As a result, I created two metrics: percent difference in death estimates by year and percent of total deaths by race. 
