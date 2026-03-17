# Vehicle Price Analysis & Predictive Pricing Model
** Floriand Beshku | 2026 **

This project demonstrates a data-driven approach to vehicle valuation, replacing subjective judgment with an objective statistical model. It bridges the gap between general market intuition and precise, quantifiable business insights.

## Business Problem
Pricing vehicles correctly is critical for dealerships, resellers, and financial institutions. Underpricing reduces revenue, while overpricing slows sales. This project aims to:

* **Estimate market value** based on observable characteristics.
* **Quantify depreciation** to understand exactly how much value is lost per month or per mile.
* **Support decision-making** for lenders, insurers, and fleet managers.

## Technical Stack
* **Language:** Python
* **Environment:** Anaconda / Jupyter Notebook
* **Libraries:** Pandas, NumPy, Scikit-Learn, Statsmodels, Matplotlib, Seaborn
* **Modeling:** Multiple Linear Regression (Ordinary Least Squares)

## Methodology & Workflow
I followed a structured data science workflow to ensure reliability and interpretability:

1.  **Data Preparation:** Cleaned and structured a dataset of 1,000 vehicle records, including feature engineering for categorical variables.
2.  **EDA:** Performed exploratory analysis to visualize relationships between price, age, and mileage.
3.  **Model Development:** Built a Multiple Linear Regression model to measure the combined effect of multiple factors on price.
4.  **Validation:** Used a 50/30/20 (Train/Validation/Test) split to ensure the model generalizes to unseen data.
5.  **Optimization:** Applied statistical variable selection to simplify the model, retaining only the 5 most significant drivers of price.

## Key Results & Business Insights
The final optimized model explains approximately **88–89%** of price variation ($R^2$).

**Critical Drivers of Price:**
* **Age:** Each additional month of age reduces vehicle value by approximately **$128.84**.
* **Mileage:** Each additional mile driven reduces value by **$0.02**.
* **Performance:** Higher horsepower and vehicle weight contribute positively to market value.
* **Fuel Type:** Diesel vehicles command a premium of roughly **$1,644** over CNG models.



## Practical Application
I developed a simplified pricing formula that can be easily integrated into a dealership management system or a mobile appraisal tool:

$$Price = -7906.96 - 128.84(Age) - 0.02(Mileage) + 51.55(HP) - 2.39(CC) + 22.82(Weight)$$
