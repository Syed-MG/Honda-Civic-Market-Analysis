

## Automotive Market Analysis & Predictive Pricing (Honda Civic)

###  1. Project Background & Objective
This project examines the secondary market for **Honda Civic models (2019–2024)** within the Birmingham, UK region. The primary goal was to identify the specific factors influencing resale value to assist in developing a data-driven pricing framework to optimize acquisition and resale margins for thirdparty showrooms.

### 2. Data Methodology
Data Sourcing:300 vehicle listings were manually scraped from autotraders.co.uk within a 200-mile radius of Birmingham (Postcode B160LP).
Sampling & Randomization: A purposive sampling method was first used to ensure all entries met the required criteria. From this cleaned dataset, 100 data points were randomly selected to serve as the representative sample for statistical analysis.
Preprocessing: Data cleaning included handling missing values for the "number of owners" variable by applying the mode of the dataset

### 3. Exploratory Data Analysis(EDA)
Bimodal Price Distribution: The market exhibits two primary price clusters: an entry-level segment (£13k–£15k) and a premium segment (£28k–£30k).
Key Visual Insights:  Mileage vs. Price:
A strong negative correlation (r = -0.71) confirms that high mileage is a primary driver of price reduction.

Fuel Type: Petrol Hybrid models command the highest average and median prices (£30,692 and £30,538 respectively).


Gearbox: Automatic vehicles initially carry higher resale value at low mileage but face faster depreciation compared to manual alternatives.

### 4. Statistical Validation
Regional Hypothesis Test:
A one-sample T-test was conducted comparing local prices against the London average of £20,584.

Confidence Intervals: We established a 95% Confidence Interval for the population mean price between £20,451 and £24,297, providing a reliable benchmark for evaluating supplier quotes.

### 5. Predictive Modeling (OLS Regression)
A parsimonious Ordinary Least Squares (OLS) model was developed, achieving an Adjusted $R^2$ of 0.926, explaining over 92% of price variance.

The Pricing Equation:Price = 3513.58 - 0.084(Mileage) + 1647.74(Reg) - 12480.45(Hybrid) + 2091.60(1.5L) + 19840.47(2.0L)

Model Diagnostics: The model passed all key regression assumptions (Linearity, Independence, Homoscedasticity, Normality, and No Multicollinearity) through comprehensive Residual Analysis

###  How to Use This Repository
1.  **View Data:** Navigate to the `/data` folder to view the Excel files containing both the raw scraped data (300 entries) and the randomized sample (100 entries).
2.  **Read Report:** Open the `Honda_Civic_Analysis_Report.docx` for the full professional report, including visualization charts and detailed business conclusions.

### Technologies Used
* **Data Collection:** Manual Web Scraping.
* **Data Management:** Microsoft Excel.
* **Statistical Analysis:** OLS Regression, T-Testing, Residual Analysis.

---

