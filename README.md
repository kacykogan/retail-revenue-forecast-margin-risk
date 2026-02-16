# Retail Revenue Forecast & Margin Risk Analysis
## Financial Modeling & Forecast Validation in Excel

### Overview
This project evaluates revenue sustainability, profitability drivers, and forecast reliability using historical sales data from the Superstore dataset (2014–2017).
The analysis was designed to answer three key business questions:
1.	How concentrated and volatile is revenue seasonally?
2.	Are category-level margins structurally healthy?
3.	Can we produce a reliable forward-looking revenue forecast for planning purposes?

### Data
* Source: Tableau Superstore Dataset, available [here](https://public.tableau.com/app/learn/sample-data).
* Timeframe: January 2014- December 2017
* Analysis was conducted in Excel using structured tables, pivot modeling, seasonality normalization, and forecast validation techniques.

### Methodology

1.	**Data Cleaning** 
    * Cleaned and structured raw transactional data
    * Integrated returns data to calculate Net Sales
    * Implemented validation checks to ensure data integrity
2.	**Revenue & Seasonality Analysis** 
    * Aggregated monthly net sales
    * Calculated normalized seasonality index across four historical years using a weighted seasonal average
    * Identified revenue concentration trends
3.	**Forecast Development** 
    Two models were tested:
    * Excel ETS model with automatic seasonality detection
    * Annual ETS trend model allocated monthly using a manually calculated seasonality index
    * A 2017 holdout year was used for validation.
      * Model Selection:
        * Manual seasonality model selected
        * 14% MAPE (vs 22% using ETS auto-seasonality)
        * Demonstrated improved monthly predictive accuracy
        * Projected 2018 revenue: $716,988 (9% growth)
        * Forecast range reflects ±14% historical accuracy.
4.	 **Profitability Diagnostics** 
     * Category-level revenue and margin comparison
     * Subcategory profit breakdown
     * Discount rate analysis
     * Return rate review to isolate margin drivers

### Key Insights 

**Revenue Risk Concentration**
* 51% of annual revenue occurs in the final four months (Sep–Dec).
*	A 10% underperformance during peak season would reduce full-year revenue by ~5%.
*	Revenue planning is highly dependent on Q4 execution.

**Growth Moderation**
  * Revenue grew 15% in 2017.
  * Growth projected to slow to 9% in 2018.
  * Forecast reliability is moderate (14% MAPE).
    
**Category Profitability Imbalance**
  * All three major categories contribute similar revenue share.
  * Margins vary significantly: Furniture (2%), Office Supplies (17%), Technology (22%).
  * Furniture materially dilutes blended profitability.
    
**Profit Leakage Drivers**
  * Subcategories generating negative profit in 2017:
    * Tables 
    * Bookcases
    * Machines
  * Observations:
    * Machines carried a 30% average discount.
    * Tables and Bookcases experienced elevated discounting with negative profitability despite comparable return rates.
    * Furnishings showed the strongest margin within Furniture, suggesting heavier items may be driving margin compression.

### Recommendations
  * Review pricing and discount strategy for high-discount items (particularly Machines).
  * Evaluate logistics and cost structure for heavier Furniture items.
  * Implement scenario planning for Q4 volatility given revenue concentration risk.
  * Monitor forecast accuracy quarterly and recalibrate seasonality annually.

### Tools & Skills Demonstrated
* Financial forecasting (trend + seasonality modeling)
* Holdout validation and MAPE evaluation
* Revenue concentration risk analysis
* Profitability diagnostics by category and SKU
* Executive dashboard design in Excel
