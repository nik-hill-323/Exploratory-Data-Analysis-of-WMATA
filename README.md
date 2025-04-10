# Exploratory-Data-Analysis-of-WMATA
Tomato Smoothie
# WMATA Transit System Analysis

![WMATA Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/WMATA_Metro_Logo.svg/240px-WMATA_Metro_Logo.svg.png)

## 📊 Overview

This repository contains a comprehensive exploratory data analysis (EDA) of the Washington Metropolitan Area Transit Authority (WMATA) system. The analysis examines multiple aspects of ridership patterns across the Metrorail system to provide actionable insights for transit planners and policymakers.

## 🚇 Dataset Description

The analysis uses the following WMATA ridership datasets:

- **Total_Entries_and_Exits_Processed.csv**: Daily system-wide entries and exits
- **Entries_Over_Time_Processed.csv**: Historical ridership trends
- **Entries_by_Tap_and_noTap_Processed.csv**: Station-level entries broken down by fare technology
- **Boardings_by_Day_of_Week_Processed.csv**: Ridership patterns by day of week
- **Boardings_by_Month_Processed.csv**: Monthly ridership trends
- **Boardings_by_Route_Table_Processed.csv**: Station-level boardings by time period
- **Entries_by_Year_Processed.csv**: Yearly ridership totals
- **Boardings_Weekends_Processed.csv**: Weekend-specific ridership data
- **Boardings_by_Time_Period_Processed.csv**: Time-of-day ridership analysis

## 🔧 Dependencies

This analysis requires the following R packages:

```r
library(ggplot2)      # For data visualization
library(dplyr)        # For data manipulation
library(readr)        # For reading all CSV files
library(tidyr)        # For data cleaning
library(lubridate)    # For date handling
library(gridExtra)    # For arranging multiple plots
library(reshape2)     # For data reshaping
library(forcats)      # For factor manipulation
library(stringr)      # For string manipulation
```

## 📋 Features

The analysis includes:

- **Temporal Analysis**: Examination of ridership patterns by time of day, day of week, and month
- **Station-Level Insights**: Identification of high and low-traffic stations and their characteristics
- **Peak Period Analysis**: Detailed breakdown of AM and PM peak ridership patterns
- **Fare Technology Adoption**: Analysis of tap vs. non-tap entry patterns
- **Statistical Testing**: ANOVA analysis of day-of-week ridership variations
- **Data Quality Assessment**: Identification of missing values and outliers
- **Actionable Recommendations**: Targeted suggestions for service improvements

## 🚀 Key Findings

1. **Peak Usage**: PM Peak (3pm-7pm) accounts for 35.6% of total ridership, followed by AM Peak (28.7%)
2. **Busiest Stations**: Gallery Place, Union Station, and Metro Center are the system's busiest stations
3. **Day of Week Patterns**: Wednesday shows the highest ridership; Sunday the lowest
4. **Fare Technology**: 92.2% of entries use tap technology
5. **Weekday/Weekend Ratio**: Weekday ridership is 1.66 times higher than weekend ridership

## 💡 Research Questions Addressed

The analysis addresses these SMART research questions:

1. **Specific**: How does ridership vary across different time periods and days of the week?
2. **Measurable**: What are the average daily ridership figures at each station?
3. **Achievable**: Which stations consistently show the highest and lowest ridership?
4. **Relevant**: How do entry and exit patterns compare across high-traffic stations?
5. **Time-bound**: What are the yearly ridership trends and post-pandemic recovery patterns?

## 📊 Usage

To run the analysis:

1. Clone this repository
2. Ensure all required packages are installed
3. Place the CSV datasets in the project directory
4. Open and run the RMarkdown file `wmata_transit_analysis.Rmd`
5. View the generated HTML output for the complete analysis

## 📂 Repository Structure

```
WMATA-Transit-Analysis/
├── README.md                              # Project overview (this file)
├── wmata_transit_analysis.Rmd             # R Markdown analysis file
├── wmata_transit_analysis.html            # Compiled HTML report
├── data/                                  # Data directory
│   ├── Total_Entries_and_Exits_Processed.csv
│   ├── Entries_Over_Time_Processed.csv
│   ├── Entries_by_Tap_and_noTap_Processed.csv
│   ├── Boardings_by_Day_of_Week_Processed.csv
│   └── [Additional CSV files]
└── figures/                               # Generated visualizations
    ├── ridership_by_day.png
    ├── top_stations.png
    └── [Additional visualization files]
```

## 📈 Sample Visualizations

![Day of Week Ridership](https://example.com/day_of_week_sample.png)
*Ridership by day of week showing weekday vs. weekend patterns*

![Top Stations](https://example.com/top_stations_sample.png)
*Top 10 stations by average daily ridership*

## 🔗 References

- [WMATA Open Data](https://developer.wmata.com/)
- [DC Metro Ridership Statistics](https://www.wmata.com/initiatives/ridership-portal/)
- [US Census Transportation Statistics](https://www.census.gov/topics/employment/commuting.html)

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👤 Author

Tomato Smoothie🍅

---

*Note: This analysis is intended for educational and planning purposes. For official WMATA statistics, please refer to their [official website](https://www.wmata.com/).*
