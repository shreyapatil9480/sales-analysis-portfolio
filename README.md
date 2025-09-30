# Business Sales Analysis Portfolio Project

This repository contains a complete, ready‑to‑use data analysis project designed to showcase skills relevant to **business analyst**, **data analyst**, and **program manager** roles. The project walks through generating a realistic synthetic dataset, performing exploratory data analysis (EDA), and building a predictive model to estimate sales based on business and marketing features.

## Repository Contents

| File/Directory | Description |
|---------------|------------|
| `synthetic_sales_data.csv` | Generated dataset containing 800 sales records across multiple product categories, regions, and dates. |
| `analysis.ipynb` | Jupyter notebook that loads the dataset, explores the data through visualizations, and fits a linear regression model to predict sales. |
| `requirements.txt` | List of Python dependencies needed to run the notebook. |
| `README.md` | Project overview, dataset description, and setup instructions (this file). |

## Dataset Description

The synthetic dataset simulates daily product sales from **January 2023** to **June 2025**. Each row represents one product sale event and includes the following variables:

| Column | Type | Description |
|-------|------|-------------|
| `Date` | Date | Date of the sale (daily granularity). |
| `Region` | Categorical | Geographic region where the sale occurred (North America, Europe, Asia, South America, Africa). |
| `ProductCategory` | Categorical | Product line (Electronics, Furniture, Clothing, Accessories, Home Decor, Office Supplies). |
| `Price` | Numeric | Unit price of the product (USD). |
| `UnitsSold` | Numeric | Quantity sold in the transaction. |
| `MarketingSpend` | Numeric | Simulated marketing spend associated with the product/category on that day. |
| `CustomerSatisfaction` | Numeric | Customer satisfaction score on a 1–5 scale. |
| `Sales` | Numeric | Total revenue from the transaction (`UnitsSold` × `Price` plus a marketing effect and random noise). |
| `ProfitMargin` | Numeric | Assumed profit margin for the transaction (percentage). |
| `Profit` | Numeric | Actual profit earned (`Sales` × `ProfitMargin`). |

These features are designed to reflect real‑world factors that influence business performance, such as seasonality, product type, regional differences, and marketing investment.

## Exploratory Analysis

The notebook explores the dataset through:

* **Summary statistics** to understand the size and distribution of the data.
* **Visualizations** such as bar charts for sales by product category, time‑series plots for monthly sales trends, scatter plots showing the relationship between marketing spend and sales, histograms of profit margins, and a correlation heatmap.
* **Data cleaning and encoding** (one‑hot encoding) to prepare categorical variables for modeling.

These steps highlight typical tasks a business or data analyst performs to derive insights from raw data.

## Predictive Modeling

To illustrate the transition from analysis to actionable insights, the notebook builds a **linear regression model** using scikit‑learn. The model predicts the `Sales` variable based on product, pricing, marketing spend, customer satisfaction, and encoded categorical features. Model performance metrics such as **MAE**, **RMSE**, and **R‑squared** are reported. Suggestions for extending the analysis (e.g., non‑linear models, time‑series forecasting, and hyperparameter tuning) are provided in the conclusion.

## Setup Instructions

1. **Clone** or download this repository.
2. Ensure you have Python 3.8+ installed. We recommend using a virtual environment to avoid dependency conflicts:

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
3. Install dependencies from the `requirements.txt` file:

   ```bash
   pip install -r requirements.txt
   ```
4. Launch the Jupyter notebook:

   ```bash
   jupyter notebook analysis.ipynb
   ```
5. Run the notebook cells in sequence to reproduce the analysis, visualizations, and model.

## Why This Project?

This project is designed to illustrate a **progressive level of difficulty**:

1. **Data Generation**: Synthesize a realistic dataset with multiple business dimensions.
2. **EDA**: Perform descriptive analysis and visualization to uncover patterns.
3. **Feature Engineering**: Convert categorical variables into numeric format for modeling.
4. **Predictive Modeling**: Fit and evaluate a regression model, demonstrating how analytics can drive business decisions.
5. **Next Steps**: Outline potential extensions to further challenge yourself (e.g., advanced machine‑learning models, forecasting, interactive dashboards).

By completing and understanding this project, you will be able to demonstrate your proficiency in data handling, visualization, and modeling—skills that are vital for business analysis, data analysis, and program management roles.

## License

This project is provided for educational and portfolio purposes. Feel free to use, modify, or extend it for non‑commercial use. If you share your own version, please credit the original author.
