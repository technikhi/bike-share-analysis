# Cyclistic Bike-Share Usage Analysis

**Google Data Analytics Capstone Project**

An exploratory data analysis of Cyclistic bike-share usage in Chicago, comparing casual riders and annual members to identify behavioural differences and potential membership marketing opportunities.

**Reporting period:** October 2025 – September 2026  
**Prepared by:** technikhi

---

## 1. Project Overview

Cyclistic is a bike-share company operating in Chicago. It offers single-ride and full-day passes for casual riders, as well as annual memberships.

The marketing team aims to increase annual memberships. This project explores how casual riders and annual members use Cyclistic bikes differently, with the objective of identifying patterns that could inform targeted membership marketing strategies.

The analysis focuses on:
- Ride volume and seasonal trends
- Ride duration
- Weekday and weekend usage
- Starting-station preferences
- Bike-type preferences
- Hourly ride patterns

## 2. Tools and Technologies

- **Python** – Data analysis and processing
- **Pandas** – Data cleaning, manipulation and aggregation
- **Matplotlib and Seaborn** – Data visualisation
- **Jupyter Notebook** – Analysis environment

## 3. Data Source

The analysis uses 12 months of historical bike-share trip data published by Motivate International Inc.

**Source:** [Divvy Trip Data](https://divvy-tripdata.s3.amazonaws.com/index.html)

The dataset contains trip-level information, including rider category, bike type, trip start and end timestamps, and station details.

The data does not contain personally identifiable information and cannot be used to identify individual riders.

## 4. Data Cleaning and Preparation

The 12 monthly CSV files were imported and cleaned individually before being combined into a single master dataset.

Key preparation steps included:

- Converting trip timestamps into datetime formats.
- Calculating ride durations.
- Extracting day-of-week information.
- Removing invalid trip durations, including trips shorter than 60 seconds and longer than 24 hours.
- Removing records with missing station names.
- Standardising rider categories and bike-type labels.
- Checking for duplicate ride IDs.

Nineteen duplicate ride IDs were identified and retained because they did not materially affect the overall analysis.

## 5. Key Findings

The analysis identified several differences between casual riders and annual members:

**Ride volume and seasonality**
- Annual members accounted for approximately 65.5% of recorded rides.
- Both rider categories showed lower ride volumes during winter and increased activity during warmer months.

**Ride duration**
- Casual rides had a mean duration of 20.30 minutes, compared with 12.40 minutes for members.
- Casual rides were approximately 64% longer on average.

**Weekday and weekend usage**
- Weekend rides represented 37.26% of casual rides, compared with 22.57% of member rides.
- Casual rides were also longer on weekends.

**Starting-station patterns**
- Casual riders frequently started trips at stations near lakefront, recreational and visitor destinations.
- Members' most frequently used starting stations were primarily in central urban areas.

**Bike-type usage**
- Electric bikes accounted for 61.03% of casual rides and 53.47% of member rides.

**Hourly usage**
- Member rides showed morning and evening peaks, with the largest peak at 5 PM.
- Casual rides peaked at 5 PM without a comparable morning surge.

## 6. Marketing Recommendations

Based on the observed usage patterns, the project proposes four strategies for Cyclistic to test:

1. **Weekend-focused membership campaigns:** Highlight the value of annual membership for casual riders who frequently use the service on weekends.
2. **Location-based promotions:** Test membership promotions around stations with high casual-rider activity.
3. **Electric-bike marketing:** Emphasise electric-bike availability and convenience when communicating membership benefits.
4. **Campaign timing:** Use observed hourly and day-of-week patterns to inform campaign timing and test engagement.

These recommendations are potential strategies rather than proven conversion methods. Their effectiveness would need to be evaluated through campaign testing and membership conversion data.

## 7. Limitations

- The dataset describes individual trips, not unique riders.
- Missing station-name records were excluded from the analysis.
- Nineteen duplicate ride IDs were retained.
- Trip durations shorter than 60 seconds or longer than 24 hours were excluded.
- Trip patterns cannot definitively establish whether rides were for commuting, recreation or tourism.

## 8. Project Report

For the detailed methodology, analysis, visualisations, findings and recommendations, see the full project report.

---

*This project was completed as part of the Google Data Analytics Professional Certificate capstone project.*
