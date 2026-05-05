---
title: "NYC Bike Sharing Optimization & Demand Analysis"
layout: post
date: 2023-01-15 11:00
image: /assets/images/markdown.jpg
headerImage: false
category: projects
project_group: data_science
tags:
- Data_Analysis
- Feature_Engineering
- Mobility_Analytics
- Regression
- Optimization
- Python
- Business_Analytics
star: false
description: "A bootcamp data analytics project focused on bike-sharing utilization, short-trip demand, proactive maintenance, and weather-driven trip fluctuation analysis."
permalink: /nyc-bike-sharing-optimization-demand-analysis/
---

## Overview

This project analyzed bike-sharing trip data in New York City to support operational and business decisions around fleet utilization, short-distance demand, proactive maintenance, and regional trip distribution.

The project was completed as part of a Data Analyst bootcamp at Rahnema College. It was structured around several business questions related to profitability, bike redistribution, marketing opportunities, maintenance detection, and demand fluctuations.

The main objective was to move from raw trip data toward actionable recommendations for operations and marketing teams.

---

## Business Context

Bike-sharing systems face a recurring operational challenge: supply and demand are not evenly distributed across stations, regions, time periods, and user groups.

Adding more bikes or stations may seem like an obvious way to increase profit, but it is not always the best first decision. Before investing in fleet expansion, the existing system should be analyzed to understand whether current bikes and stations are being used efficiently.

This project explored whether better redistribution, targeted marketing, proactive maintenance, and regional demand analysis could improve system performance.

---

## Project Questions

The project focused on four main analytical questions.

### 1. Fleet Utilization and Redistribution

Should the company buy more bikes and build more stations, or can the existing fleet be used more efficiently?

This question focused on station-level imbalance, bike idle time, and the possibility of improving profitability through redistribution before expanding physical capacity.

### 2. Short-Trip Marketing

How should short-distance bike rides be promoted, and which user groups are most likely to respond?

This question focused on defining short trips, identifying user groups with higher short-trip demand, and evaluating whether demand changed meaningfully across months.

### 3. Proactive Bike Maintenance

Can potentially faulty or worn-out bikes be identified before users report them?

This question focused on building indicators that could flag bikes needing inspection based on usage patterns, abnormal trip behavior, and accumulated bike-level features.

### 4. Regional and Weather-Driven Demand Fluctuation

Are monthly trips distributed evenly across city regions, and which factors explain demand fluctuations?

This question focused on regional trip distribution, monthly variation, and the relationship between weather variables and trip volume.

---

## Data Preparation

The project required extensive preprocessing before analysis.

Monthly CSV files were combined into a single dataset for the selected time period. To make computation faster and reduce memory usage, data types were optimized and intermediate files were saved in a more efficient format.

Several features were engineered, including:

- trip duration;
- trip distance using the Haversine formula;
- bike speed;
- bike first appearance date;
- bike age;
- cumulative usage time per bike;
- cumulative distance per bike;
- bike idle time between consecutive trips;
- regional labels based on different city zoning methods;
- weather-related features.

The report notes that multiple geographic segmentation methods were considered, including neighborhood boundaries, city council districts, borough boundaries, and zoning-map-style fixed regions. :contentReference[oaicite:0]{index=0}

---

## Analysis 1: Fleet Utilization and Station Imbalance

The first analysis evaluated whether buying more bikes or expanding stations was necessarily the best path to profitability.

The project introduced the concept of station and bike idle time. If bikes remain unused for long periods at a station, this may indicate oversupply relative to demand. If bikes have very low idle time, the station may be unable to satisfy existing demand.

To make the analysis operationally useful, days were divided into several time windows, and weekend behavior was treated carefully because trip volume changed significantly compared with weekdays. The presentation also framed this part around whether investment should go toward more bikes, more stations, or a redistribution system. :contentReference[oaicite:1]{index=1}

This helped shift the decision from “buy more assets” to “first understand whether existing assets are being used efficiently.”

---

## Analysis 2: Short-Trip Demand and Target Users

The second analysis focused on short-distance trips.

A short trip was defined using the lower quartile of trip duration. In the dataset, the 25th percentile of trip duration was approximately 6.75 minutes, which was used as a practical threshold for identifying short trips. :contentReference[oaicite:2]{index=2}

The analysis then explored which user groups were most represented in short trips.

User segmentation considered:

- user type;
- age group;
- gender;
- region.

The strongest short-trip segment was the 26–36 age group, especially male users, based on the share of short trips reported in the analysis. :contentReference[oaicite:3]{index=3}

This part of the project translated trip behavior into a marketing recommendation: short-trip campaigns should focus on the user groups with the highest observed short-trip demand.

---

## Analysis 3: Proactive Maintenance Detection

The third analysis explored how to identify bikes that may need maintenance before users report a problem.

Because there was no direct maintenance label in the raw trip data, the project created proxy indicators. These included abnormal idle time, very short trips returning to the origin station, accumulated bike usage, bike age, total distance traveled, and other usage-based features.

The dataset was labeled using a binary approach:

- `1` indicated that a bike may need inspection;
- `0` indicated that no inspection signal was detected.

The project then used regression-based modeling and a scoring function to identify bikes that should be sent for maintenance review.

In the final estimate, around 205 bikes were identified as requiring service during the analyzed period. :contentReference[oaicite:4]{index=4}

The model performance was limited, and this should be interpreted as an exploratory maintenance-screening approach rather than a production-level predictive model.

---

## Analysis 4: Regional Demand and Weather Impact

The fourth analysis studied whether trips were distributed evenly across city regions and how weather factors affected monthly trip fluctuations.

The project compared trip distribution across regions and months. The analysis found that although trip counts changed over time, the share of trips across major regions remained relatively stable in several high-demand areas.

A statistical test was used to compare distributions across regions, and the result suggested that the distribution of trips across regions was not uniform.

The project also analyzed weather-related factors, including:

- average temperature;
- precipitation;
- snowfall;
- wind speed.

A regression model was used to estimate how these variables related to trip fluctuations. The model achieved an R-squared value of approximately 0.41, suggesting that weather explained part, but not all, of the variation in trip volume. :contentReference[oaicite:5]{index=5}

The analysis also noted that other external factors, such as tourism patterns or major weather events, could affect demand but were not fully available in the dataset.

---

## Key Outputs

The project produced several analytical outputs:

- cleaned and optimized trip dataset;
- engineered features for trip, bike, station, and weather analysis;
- station utilization and idle-time analysis;
- short-trip customer segmentation;
- maintenance candidate identification logic;
- regional demand distribution analysis;
- weather regression analysis;
- presentation and written report summarizing the business recommendations.

---

## Tools and Methods

- Python
- Pandas
- NumPy
- Feature engineering
- Haversine distance calculation
- Data cleaning and optimization
- Feather file format for faster processing
- Statistical testing
- Regression analysis
- Mobility analytics
- Business recommendation framing

---

## Limitations

This project was completed as a bootcamp analytics project and should be interpreted as an exploratory analysis rather than a production-ready optimization system.

Main limitations included:

- lack of direct ground-truth maintenance labels;
- reliance on proxy indicators for faulty bike detection;
- limited availability of external variables such as tourism or major city events;
- regression models with moderate explanatory power;
- need for stronger cost-benefit modeling before making investment decisions.

---

## What This Project Demonstrates

This project demonstrates my ability to connect data analysis with business decision-making.

It covered the full analytics flow: data preparation, feature engineering, exploratory analysis, statistical testing, modeling, and recommendation design.

The project also shows how operational datasets can be used to answer practical business questions around utilization, customer targeting, maintenance planning, and demand fluctuation.
