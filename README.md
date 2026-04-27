# Honda-Civic-Market-Analysis
Statistical analysis and predictive pricing model for second-hand Honda Civics (2019-2024) using OLS regression
### Project Overview
This project investigates the second-hand car market for Honda Civics (2019–2024) in Birmingham, UK. The goal was to identify the most significant factors influencing resale value to assist "car4all" in creating an accurate pricing calculator
## Data Methodology

Data Sourcing: 300 vehicle entries were manually scraped from autotraders.co.uk within a 200-mile radius of Birmingham (Postcode B160LP).


Data Processing: The raw data was compiled into Excel, addressing missing values for "number of owners" by using the mode of the dataset.


Sampling: A purposive sampling method ensured all data met business criteria, followed by a randomization process to select 100 specific data points for final statistical analysis.

### Key FindingsMarket Distribution:
The price distribution is bimodal, with significant clusters at £13,000–£15,000 and £28,000–£30,000.Correlation: Engine size (2.0L) and registration year show the strongest positive correlation with price. Mileage shows a strong negative correlation ($r = -0.71$).
Regional Insights: A one-sample T-test revealed that local Birmingham prices differ significantly from London averages (£20,584), suggesting regional market premiums.

The final Parsimonious OLS Regression Model achieved an Adjusted R-squared of 0.926, explaining 92.6% of the price variance.Predictive Equation:$$Price = 3513.58 - 0.084(Mileage) + 1647.74(Reg) - 12480.45(Hybrid) + 2091.60(1.5L) + 19840.47(2.0L)

### How to Use This Repository
View Data: Navigate to /data to see the manually scraped dataset.
Read Report: Open /docs/Final_Market_Report.pdf for the full business analysis, including residual plots and hypothesis testing results.
### Technologies UsedData 
Collection: Manual Web Scraping.
Analysis: Descriptive Statistics, T-Testing, OLS Regression.Tools: Microsoft Excel, Python (Statsmodels, Seaborn).
