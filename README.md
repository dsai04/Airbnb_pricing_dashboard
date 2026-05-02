# Airbnb Pricing & Demand Analysis Dashboard

An interactive Tableau dashboard analyzing pricing dynamics, seasonal demand patterns, and geographic market distribution across 2,580+ Airbnb listings in Seattle (2016).

![Dashboard Preview](.png)

---

## Project Overview

This project explores what drives Airbnb pricing in Seattle — geography, property size, and time of year. The goal was to move beyond surface-level averages and identify the structural patterns that explain pricing behavior across the market.

**Dataset:** 2,580+ listings | 52 weeks of revenue data | 10 ZIP codes | 6 property size tiers

---

## Key Findings

### 1. Geography is the dominant pricing factor
Top ZIP codes (98134, 98119) exceeded the city-wide average price by ~37%, while ZIP codes like 98116 and 98104 fell below average despite being within Seattle city limits. Central ZIP codes — close to downtown, waterfront, and tourist zones — consistently command the premium.

### 2. Seasonal demand amplifies pricing in premium locations disproportionately
Revenue trends from January to late 2016 show a clear upward trajectory toward $2M in total revenue, with peak demand in June–August. Crucially, premium ZIP codes exhibited price swings of ~60% between off-peak and peak months — nearly double the volatility of below-average ZIP codes. Location and seasonality are not independent variables; they interact.

### 3. Property size shows a U-shaped pricing efficiency curve
Price per bedroom is highest for 1-bedroom ($96.25) and 6-bedroom ($97.47) listings, but dips significantly for mid-size properties (4BR = $78.86). This non-linear pattern suggests two distinct demand segments operating in the same market: solo/couple travelers targeting compact listings, and large groups targeting 5–6BR homes. Mid-size properties serve neither segment optimally and consequently show weaker pricing power.

---

## Dashboard Views

| View | What It Shows |
|---|---|
| **Price per ZIP Code (Choropleth)** | Geographic price distribution across Seattle ZIP codes; top ZIPs labeled with average prices |
| **Weekly Revenue Trend** | Total revenue trajectory across 52 weeks with moving average overlay, highlighting seasonal demand peaks |
| **Price per Bedroom by Property Size** | Average price-per-bedroom across 1–6BR tiers, revealing the U-shaped efficiency curve |
| **Total Price by Bedroom Count** | Absolute average price by property size ($96 → $585), showing the total price vs. efficiency trade-off |
| **Top ZIP Codes by Avg Price** | Bar chart ranking ZIPs against city average, with 98134 ($205.85) leading the market |
| **Seasonal Price Volatility (Premium ZIPs)** | Moving average price trends for top 5 ZIP codes across the calendar year |

---

## Tools Used

- **Tableau Desktop** — dashboard design, choropleth mapping, calculated fields, moving averages, dynamic filters
- **Excel / CSV** — data cleaning and preparation before import

---

## Skills Demonstrated

- Multi-dimensional dashboard design (time, geography, property attributes in a single view)
- Geographic data visualization using choropleth maps
- Moving average calculations for trend smoothing
- Segmentation analysis (ZIP performance relative to market average)
- Insight annotation directly within visualizations

---

## How to View

1. Download the `.twbx` file from this repository(uploading soon)
2. Open with Tableau Desktop or Tableau Public
3. Use the ZIP Group filter (Top ZIPs toggle) and Bedroom filter to explore segments

---

## Data Source

Public Airbnb listing and revenue dataset for Seattle, WA (2016). Originally sourced from Kaggle / Inside Airbnb.
