# ✈️ Flight-Delay-EDA
## Exploratory Data Analysis of U.S. flight delays using real-world data from the U.S. Department of Transportation (2023–2024). Includes data cleaning, visualizations, and insights on delay causes, airline performance, and seasonal patterns.

Read the full blog post on Medium:  
- [Behind the Delay: What the Data Says About U.S. Flights]([https://medium.com/your-article-link](https://medium.com/@paboda-ratnayake/patterns-in-the-sky-a-flight-delay-analysis-1444df5d82d1))
  
---

## Project Objectives

- Identify the **most common causes** of flight delays.
- Compare **airline and airport performance** (best vs. worst).
- Discover **seasonal patterns** in delays and cancellations.

---

## Dataset Overview

- **Source**: U.S. Department of Transportation, Bureau of Transportation Statistics  
- **Period**: January 2023 – March 2024  
- **Granularity**: Monthly, aggregated by airline and airport  
- **Key Fields**:
  - `arr_delay`, `arr_cancelled`, `arr_diverted`
  - Delay counts and durations by cause: carrier, weather, NAS, security, late aircraft
  - Airline and airport identifiers

---

## EDA Workflow

- Dropped rows with missing values for key delay/cancellation metrics
- Created a `year_month` column for time-based visualizations
- Aggregated and analysed delays and cancellations by month, airline, and airport

---

## Key Visual Insights

- **Top Delay Causes**: Late aircraft is the largest contributor (~40% of delay minutes)
- **Seasonal Trends**: 
  - December–January: Peak in late aircraft delays
  - July–August: Cancellation rates nearly double
- **Airport performance**:
  - St. Cloud, MN: St. Cloud Regional has the least average delay of 45.68 minutes
  - Owensboro, KY: Owensboro Daviess County Regional and Pago Pago, TT: Pago Pago      International has the least no. of cancelled flights

---

## Recommendations

-  Add de-icing crews and schedule buffers during winter
-  Optimize aircraft turnaround times for delay-prone airlines
-  Schedule reserve crews and aircraft during summer peak season

---

## Tools Used

- Python (Pandas, Matplotlib, Seaborn)
- Google Colab Notebook
