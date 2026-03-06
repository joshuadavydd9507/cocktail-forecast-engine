# Cocktail Forecast Engine
Data Analytics Portfolio Project

## Project Summary

This project builds a forecasting and financial analysis engine for a luxury hotel cocktail bar.

Using historical cocktail sales data, the model estimates baseline demand and applies seasonal demand drivers to forecast future performance. The system then converts projected demand into revenue, cost of goods, and gross profit to evaluate menu strategy and supplier product utilisation.

The analysis also explores how a new cocktail launch (*Peach & Circumstance*) and a later ingredient switch influence usage of **KI NO BI Kyoto Dry Gin**.

---

## Project Structure

### 01_data_engine.ipynb

Builds the analytical data model used throughout the project.

Key tables include:

- Cocktail dimension table
- Ingredient dimension table
- Recipe bridge table
- Cocktail pricing table
- Monthly sales fact table

These tables allow calculation of:

- Revenue
- Cost of goods
- Gross profit

---

### 02_forecast_strategy.ipynb

Implements the forecasting logic.

Baseline demand is calculated using a **3-month moving average (MA3)** and adjusted using seasonal drivers.

Forecast model:
forecast = baseline × (1 + uplift) × growth_factor


Seasonal drivers include:

- Dry January demand decline
- Summer tourism uplift
- Major event demand spikes
- Christmas seasonal peak

The model produces a cocktail demand forecast extending into **2026**.

---

### 03_executive_portfolio.ipynb

Presents the forecasting results as commercial analysis.

Key outputs include:

- Monthly gross profit projections
- Seasonal demand visualisation
- Top cocktails by gross profit
- Event impact analysis
- Supplier product usage tracking

---

## Example Outputs

## Example Outputs

### Monthly Gross Profit Trend

![Monthly Gross Profit Trend](./exports/13H_monthly_gross_profit_trend.png)

### Top Cocktails by Gross Profit

![Top Cocktails by Gross Profit](./exports/13I_top_cocktails_by_gp.png)

### KI NO BI Bottle Usage Forecast

![KI NO BI Bottle Usage Forecast](./exports/13K_kino_bottle_progress.png

---

## Tools Used

- Python
- Pandas
- SQLite
- Matplotlib
- Jupyter Notebook

---

## Key Skills Demonstrated

- SQL data modelling
- Forecasting methodology
- Financial modelling
- Data visualisation
- Business analytics storytelling

---

## Author

Joshua Garthwaite  
Data Analytics Portfolio Project
