# bigDataAnalysis

A collection of big-data analysis lab assignments covering data exploration, cleaning, streaming, and pattern mining.

---

## LD1 — Uber NYC Trip Data Analysis
**Tech:** PySpark · Parquet · opendatasets (Kaggle)

Loads all 12 months of 2021 Uber NYC for-hire vehicle trip data (~Parquet files) into a single Spark DataFrame. Explores the dataset schema, finds the longest trip, counts rides where tips exceeded $100, and identifies suspiciously short trips with high fares.

---

## LD3 — IoT Energy Sensor Readings Analysis
**Tech:** PySpark · Parquet · CSV · JSON · Matplotlib

Reads energy-meter time-series readings from a Parquet file and enriches them with sensor metadata stored in CSV and JSON files. Computes daily and hourly average consumption, visualises trends, and profiles sensor attributes such as manufacturer counts and calibration date ranges.

---

## LD4 — Sales Data Cleaning Pipeline
**Tech:** PySpark · Parquet

Performs a full data-quality pass on a sales Parquet file. Counts and removes invalid numeric strings, null values, and duplicate rows; casts `Gross_Sales`/`Net_Sales` to proper types; normalises `Order_Date`/`Ship_Date`; profiles malformed `Order_ID` values; and fixes city–region geographic mismatches.

---

## LD6 — Comparative Sales Dataset Analysis
**Tech:** Pandas · Parquet · Matplotlib

Loads two versions of a cleaned sales dataset (`pirmas` and `antras`) and compares them across multiple dimensions: total gross/net sales and profit, per-segment (Consumer / Corporate / Home Office) order counts and average profit, shipping-mode profitability and average shipping duration.

---

## LD7 — Market Basket Analysis (FP-Growth)
**Tech:** Pandas · mlxtend (FP-Growth / Association Rules) · Kaggle

Applies the FP-Growth algorithm to an online-retail transaction dataset. Builds market baskets per invoice, mines frequent itemsets at several support thresholds, generates association rules at various confidence levels, and compares rule counts and top items across parameter combinations.

---

## LD8 — Weather Time-Series Analysis & Streaming Simulation
**Tech:** PySpark (Structured Streaming simulation) · Pandas · Matplotlib · Kaggle

Explores a long-term weather CSV dataset: determines the date range and measurement interval, computes overall temperature statistics, then simulates a PySpark micro-batch stream to calculate rolling averages with window functions. Finishes with a 2020-focused temperature trend visualisation.

---

## LD9 — Weather EDA — Temperature & Solar Radiation (2020)
**Tech:** Pandas · NumPy · Matplotlib · Kaggle API · Google Colab

Downloads the same weather dataset via the Kaggle API in a Colab environment. Filters to 2020, builds daily and monthly aggregates for temperature (`T`) and downward shortwave radiation (`SWDR`), assigns seasons, and analyses the correlation between temperature and solar radiation during daylight hours.
