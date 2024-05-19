# Drug Overdoses in USA

## Overview
I utilized Google Sheets to do an initial cleaning of the data. I also used visualization techniques through Tableau to create graphs of the data, including bar charts, line graphs, and more.

## Tableau Public Dashboard
https://public.tableau.com/app/profile/lindadngo/viz/usa-drug-overdoses-2/AnalyzingDrugOverdoseDeathsinUSA?publish=yes

## Dataset
[https://github.com/lindngo/us-drug-overdoses/blob/main/cleaned_drug_overdose_death_rates.xlsx](https://github.com/lindngo/us-drug-overdoses/blob/main/cleaned_drug_overdose_death_rates.xlsx)

## Dataset Factors
See this page for more details: https://data.cdc.gov/NCHS/Drug-overdose-death-rates-by-drug-type-sex-age-rac/95ax-ymtc/about_data

## Defining Objectives and Questions
My maine objectives for this dashboard was to learn at least one new Tableau feature, visualize the data trends in an engaging manner, and format the cards to allow for smooth data storytelling.

With the limited time for the Datathon, my vision was to focus on 2 major questions and center my dashboard around these. After reviewing the prompt and directions, I ended up selecting the following for my target questions.
Q1: What are the trends in drug overdose death rates over time? Highlight any significant changes or patterns in the death rates over the years. Break down the trends by Drug overdose type, Sex, Age, and Race.
Q2: What formula would you use for a metric to rank and label the concern the government should have for a specific demographic group? What would the resulting ranking be when you use this formula? 


## Data Cleaning
- 1,112 data rows had * in the Flag column, indicating that these rows had null values in the Estimate column. For a more accurate and insightful analysis, I decided to remove these null values.
- In the Stub Label column, race was always paired with another label, such as sex. In order to do analysis based solely on race, I created a calculated field using "IF ELSE" statements. When creating these statements, I took note that there were two separate Asian labels -- Asian and Asian or Pacific Islander. To make the analysis more cohesive, I combined these two labels under Asian or Pacific Islander.


## Data Analysis
After cleaning the dataset and pinpointing which questions would be the focus of my analysis, I explored which different metrics would be the best to answer Q2 in the Defining Objectives and Questions. After brainstorming, I concluded that percent difference in death estimates by year and percent of total deaths by race would work the best for this report.

## Data Interpretation and Visualization
Once all metrics were created, I explored the various types of visualization techniques to see which mappings would best portray my data findings in a clear and effective manner. As a lot of my data points were plotted over time, I went with line charts to depict findings of estimated deaths by drug type and age group. For categorical data, such as sex and race, I used bar charts to visualize the number of deaths per 100,000 resident population.

## Data Storytelling
After all cards were created and formatted on dashboard pages, I mapped out the order and format of these pages on to a Story. That way, I can guide the user on a journey through the data.
