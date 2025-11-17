Retail Revenue Decomposition — ABV × Transactions Model

This project analyzes the core drivers of retail revenue by breaking it into its two fundamental components:

Transactions (customer traffic)

Average Basket Value (ABV)

Model 1 provides a clear, data-driven way to understand what really drives revenue, and how promotions or discounts influence customer behavior.

🧩 Model Components
1. ABV Regression (Promo + Discount + Transactions)

A linear regression model estimates how ABV is affected by:

promotional activity

discount rate

customer traffic

This identifies whether basket value changes because of price mechanics or customer flow.

Regression equation:

ABV = β0 + β1·Promo + β2·DiscountRate + β3·Transactions + ε

2. Discount Elasticity Estimation (α)

The model calculates:

“How much does ABV decrease when discounting increases?”

Formula:

α = – β_discount


This elasticity is directly used in pricing and promotion profitability analysis.

3. Revenue Decomposition (ΔTransactions vs ΔABV)

Revenue is defined as:

Revenue = Transactions × ABV


Change in revenue is decomposed into:

Volume effect

ΔT × ABV_prev


Value effect

ΔABV × T_curr


This structure is the basis of an FP&A Revenue Bridge.

📊 Core Formulas (Clean Markdown Version)
ABV Regression
ABV = β0 + β1·Promo + β2·DiscountRate + β3·Transactions

Revenue Change Decomposition
ΔRev = ΔT × ABV_prev  +  ΔABV × T_curr

Discount Elasticity
α = – β2


All formulas are now Markdown-safe and will not break in GitHub.

🧠 Why This Model Matters (FP&A + Retail Analytics)

Retailers like Aldi, Lidl, Tesco, Walmart, Carrefour use this methodology daily for:

Promo effectiveness

Margin protection

Discount impact analysis

Basket behavior insights

Customer traffic optimization

This model answers key business questions:

“Did sales increase because more customers came, or because basket value grew?”

“How much does discounting reduce ABV?”

“Which driver contributed more to revenue change?”

“What is the effective discount elasticity?”

📁 Project Structure
/notebooks
    model1_abv_transactions.ipynb

/data
    example_retail_data.csv   (optional)

/images
    revenue_decomposition.png (optional)

README.md

📎 LinkedIn & Portfolio

This repository is part of a larger retail analytics portfolio, including:

Revenue decomposition (Model 1)

Demand modeling

Supply capacity modeling

Operational Resilience Score (SRS)

Integrated supply–demand systems

If you'd like the extended model (Integrated Model: Revenue + Demand + Supply), feel free to reach out.
