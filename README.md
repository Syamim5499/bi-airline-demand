# Airline Demand Intelligence

Interactive, static BI case study using the public **AirPassengers / seaborn flights** teaching dataset.

## Business question
How did passenger volume change from 1949 to 1960, and which months show recurring seasonal peaks?

## Dashboard
[Open the live dashboard](https://syamim5499.github.io/bi-airline-demand/).

Open [index.html](index.html) in a browser. No install, server, account, or API key is needed. The Year filter updates four KPIs, annual trend, and monthly seasonality chart. Hover on chart marks to inspect values.

## Findings from the supplied sample
- Reported annual volume rises from **1,520 thousand in 1949** to **5,714 thousand in 1960**.
- **July** has the highest average monthly volume across the 12 years.
- These are descriptive observations of a historical teaching dataset; they do not establish causes or predict current demand.

## Model and metric definitions
Grain: one row per year and month, 144 rows. Passenger values are **thousands**, so the annual card sums monthly values in thousands. The seasonality chart averages each calendar month's values over selected years. With a single year selected, the annual point and monthly bars show that year's observations. No missing dates or duplicate year-month keys in the supplied snapshot.

## Source and reproducibility
[seaborn-data flights.csv](https://github.com/mwaskom/seaborn-data/blob/master/flights.csv), Git blob SHA `831265b40b19695dd9bd4f7c5bf4baa43c7b54b1`. The repository contains a derived `data.js` for immediate offline use. Run `python build_data.py` to refresh only if the upstream blob is still identical; the script stops on source drift. The seaborn copy is a teaching sample and may differ from canonical data. Attribution: AirPassengers time series distributed through seaborn-data.

## Portfolio skills
KPI design, time series aggregation, seasonality, filter context, data lineage, and cautious interpretation.
