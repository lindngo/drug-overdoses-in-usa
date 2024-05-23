# Drug Overdoses in USA

## Overview
I utilized Google Sheets to do an initial cleaning of the data. I also used visualization techniques through Tableau to create graphs and dashboards of the data, including bar charts, line graphs, and more.

## Tableau Public Dashboard
https://public.tableau.com/app/profile/lindadngo/viz/usa-drug-overdoses-2/AnalyzingDrugOverdoseDeathsinUSA?publish=yes

## Dataset
[https://github.com/lindngo/us-drug-overdoses/blob/main/cleaned_drug_overdose_death_rates.xlsx](https://github.com/lindngo/us-drug-overdoses/blob/main/cleaned_drug_overdose_death_rates.xlsx)

## Dataset Factors
- INDICATOR: Measure being estimated.
- PANEL: Submeasures of INDICATOR. Datasets may have multiple panels.
- PANEL_NUM: Numeric code for levels of PANEL that may be used for easier coding or formatting of the PANEL variable.
- UNIT:	Unit of measurement of the estimate.
- UNIT_NUM:	Numeric code for levels of UNIT that may be used for easier coding or formatting of the UNIT variable.
- STUB_NAME: Description of the population category pertaining to the estimate.
- STUB_NAME_NUM: Numeric code for levels of STUB_NAME that may be used for easier coding or formatting of the STUB_NAME variable.
- STUB_LABEL: Specific population subgroup pertaining to the estimate.
- STUB_LABEL_NUM: Numeric code for levels of STUB_LABEL that may be used for easier coding or formatting of the STUB_LABEL variable.
- YEAR: Data year or range of data years pertaining to the estimate.
- YEAR_NUM:	Numeric code for levels of YEAR that may be used for easier coding or formatting of the YEAR variable.
- AGE:	Age group pertaining to the estimate.
- AGE_NUM:	Numeric code for levels of AGE that may be used for easier coding or formatting of the AGE variable.
- ESTIMATE:	Calculated estimate of the measure.
- FLAG:	Additional information pertaining to the estimate. See the footnotes in the source table (Excel) for more information.

See this page for more details: https://data.cdc.gov/NCHS/Drug-overdose-death-rates-by-drug-type-sex-age-rac/95ax-ymtc/about_data

## Other Sources Used
https://www.cbo.gov/system/files/2022-09/58221-opioid-crisis.pdf

## Defining Objectives and Questions
My main objectives for this dashboard were to learn at least one new Tableau feature, visualize the data trends in an eye catching manner, and format the cards in a logical order to allow for smooth data storytelling.

With the limited time for the Datathon, my vision was to focus on 2 major questions and center my dashboard around these. After reviewing the prompt and directions, I ended up selecting the following for my target questions.

- Q1: What are the trends in drug overdose death rates over time? Highlight any significant changes or patterns in the death rates over the years. Break down the trends by Drug overdose type, Sex, Age, and Race.
- Q2: What formula would you use for a metric to rank and label the concern the government should have for a specific demographic group? What would the resulting ranking be when you use this formula? 


## Data Cleaning
- 1,112 data rows had * in the Flag column, indicating that these rows had null values in the Estimate column. For a more accurate and insightful analysis, I decided to remove these null values.
- In the Stub Label column, race was always paired with another label, such as sex. In order to do analysis based solely on race, I created a calculated field using "IF ELSE" statements. When creating these statements, I took note that there were two separate Asian labels -- Asian and Asian or Pacific Islander. To make the analysis more cohesive, I combined these two labels under Asian or Pacific Islander.


## Data Analysis
After cleaning the dataset and pinpointing which questions would be the focus of my analysis, I explored which metrics would be the best to answer Q2 in the Defining Objectives and Questions section. After brainstorming, I concluded that *percent difference in death estimates by year* and *percent of total deaths by race* would be insightful metrics for this report. The calculations for both metrics were as follows, respectively: 

## Data Interpretation and Visualization
Once all metrics were created, I explored the various types of visualization techniques to see which mappings would best portray my findings in a clear and effective manner. As a lot of my data points were plotted over time, I went with line charts to depict findings of estimated deaths by drug type and age group. For categorical data, such as sex and race, I used bar charts to visualize the number of deaths, which allowed to direct comparisons between populations.

## Conclusion
