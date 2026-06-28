# Global YouTube Ecosystem: A Macroeconomic & Demographic Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Wrangling-yellow.svg)
![Seaborn](https://img.shields.io/badge/Seaborn-Data%20Visualization-teal.svg)

## Project Overview
This project is a comprehensive, 20-question data analytics case study examining the **Top 1,000 YouTube Channels** globally. Moving beyond surface-level subscriber metrics, this analysis investigates the geographic distribution, content saturation, and macroeconomic factors (such as urbanization, education, and unemployment) that drive the creation of elite-tier digital creators.

The goal of this analysis is to provide rigorous, unbiased business insights into the creator economy, utilizing statistical methods such as log-transformations, Spearman rank correlations, and per-capita normalizations.

## The Dataset
The dataset utilized is the **Global YouTube Statistics** dataset, containing detailed metrics on the platform's top 1,000 channels, including:
* Channel Demographics (Subscribers, Video Views, Uploads)
* Content Categories
* Estimated Financial Earnings
* Geographic Data (Country, Latitude, Longitude)
* National Macroeconomics (Population, Urbanization %, Unemployment Rate, Tertiary Education Enrollment)

## Methodology & Tech Stack
* **Language:** Python
* **Data Wrangling:** `pandas`, `numpy` (Handled missing dates, fixed epoch timestamp bugs, created derived per-capita columns).
* **Data Visualization:** `matplotlib`, `seaborn` (Employed log-log scales, heatmaps, and custom plotting functions to handle heavy power-law distributions).
* **Statistics:** Avoided ecological fallacies and sample-size bias by using Medians for skewed financial data and Spearman Rank for non-linear correlations.

## Key Business Insights
Throughout the 20-question analysis, several major insights were uncovered:

1. **The "Matthew Effect" in Action:** Subscriber and view growth follows a strict power-law distribution. The YouTube algorithm heavily favors channels that are already winning, creating immense wealth inequality even among the Top 1000.
2. **True Engagement ROI:** While "Entertainment" generates massive absolute view counts, **"Comedy" and "Music"** yield the highest Return on Investment (ROI) per video (Total Views / Total Uploads). High-quality evergreen content passively out-scales brute-force daily vlogging.
3. **Macroeconomic Drivers:** A Spearman correlation heatmap reveals that **Urbanization** has the strongest positive correlation with a country's ability to produce top YouTubers, outweighing both National Unemployment and Tertiary Education. Access to internet infrastructure is the ultimate bottleneck.
4. **The "Golden Age" is Over:** Very few channels created after 2018 have managed to break into the global Top 1000, indicating that the platform has matured and the barrier-to-entry for new creators is at an all-time high.

## How to Run the Project
1. Clone this repository to your local machine.
2. Ensure you have the required libraries installed:
   ```bash
   pip install pandas numpy matplotlib seaborn tabulate
   ```
3. Open the `youtube_analytics_notebook.ipynb` notebook in Jupyter / Google Colab.
4. The script will automatically clean the data, calculate the necessary aggregations, and generate the 20 visualizations.

---
*This project was originally built during a DS with Python course with Finlatics but was completely dismantled, transformed, and rebuilt from the ground up to demonstrate professional, end-to-end data cleaning, EDA, and statistical storytelling.*
