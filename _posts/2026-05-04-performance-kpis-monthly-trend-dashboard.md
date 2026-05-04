---
title: "Performance KPIs Monthly Trend Dashboard"
layout: post
date: 2026-05-04 12:00
image: /assets/images/markdown.jpg
headerImage: false
category: dashboards
tags:
- Tableau
- KPI_Monitoring
- Vendor_Performance
- Marketplace_Analytics
- Performance_Tracking
- Trend_Analysis
star: true
description: "Tableau dashboard for monitoring long-term vendor performance KPI trends across orders, cancellations, issues, and delay-related indicators."
permalink: /performance-kpis-monthly-trend-dashboard/
---

## Overview

This dashboard was designed to monitor long-term trends in vendor performance KPIs.

The main objective was to create a consistent performance tracking layer that helps business and operations teams understand how key operational indicators evolve over time. Instead of looking only at isolated monthly snapshots, the dashboard provides a trend-based view of performance behavior across multiple weeks.

It helps answer a simple but important question: are marketplace performance indicators improving, deteriorating, or moving because of changes in order volume, vendor behavior, operational flow, or external conditions?

---

## Business Context

Vendor performance in a marketplace cannot be evaluated through one KPI alone. A vendor may have high order volume but poor cancellation behavior, or a low issue rate but worsening delay indicators. For this reason, performance monitoring needs a structured view across several KPI families.

This dashboard was built to help teams track long-term movement in performance indicators such as:

- order volume;
- cancellation behavior;
- customer-reported issues;
- delay-related indicators;
- net order performance;
- performance differences across operational segments.

The dashboard supports recurring business reviews, performance governance, and operational follow-up by showing how KPIs change over time and whether performance programs are creating measurable improvement.

---

## Interactive Dashboard

The dashboard below is published on Tableau Public using a public-safe synthetic dataset. It preserves the analytical structure of the original dashboard without exposing confidential company data.

<div class="tableau-embed-wrapper">
<div class='tableauPlaceholder' id='viz1777920591807' style='position: relative'>
  <noscript>
    <a href='https://public.tableau.com/views/PerformanceKPIsMonthlyTrendLive_v4/PerformanceKPITrends70Weeks'>
      <img alt='Performance KPI Trends Dashboard'
           src='https://public.tableau.com/static/images/Pe/PerformanceKPIsMonthlyTrendLive_v4/PerformanceKPITrends70Weeks/1_rss.png'
           style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz' style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
    <param name='embed_code_version' value='3' />
    <param name='site_root' value='' />
    <param name='name' value='PerformanceKPIsMonthlyTrendLive_v4/PerformanceKPITrends70Weeks' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https://public.tableau.com/static/images/Pe/PerformanceKPIsMonthlyTrendLive_v4/PerformanceKPITrends70Weeks/1.png' />
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='display_count' value='yes' />
    <param name='language' value='en-US' />
  </object>
</div>
</div>

<script type='text/javascript'>
  var divElement = document.getElementById('viz1777920591807');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width = '100%';
  vizElement.style.height = (divElement.offsetWidth * 0.75) + 'px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

<p>
  <a href="https://public.tableau.com/views/PerformanceKPIsMonthlyTrendLive_v4/PerformanceKPITrends70Weeks" target="_blank">
    Open the dashboard on Tableau Public
  </a>
</p>

---

## My Role

I designed the analytical structure behind the dashboard and prepared the KPI logic needed for long-term performance monitoring.

My work included:

- defining the main vendor performance KPI families;
- preparing the data structure for weekly and monthly trend analysis;
- standardizing performance indicators for consistent monitoring;
- designing the dashboard flow for business and operations users;
- connecting order volume, cancellation, issue, and delay metrics into one view;
- creating a public-safe version of the data for portfolio presentation.

---

## Dashboard Logic

The dashboard organizes performance KPIs into trend-based views.

The main idea is to make performance movement visible over time, so teams can understand whether a KPI change is temporary, structural, or related to a broader operational shift.

The dashboard focuses on several KPI groups.

### Order Volume

Order volume provides the base context for interpreting all other KPIs.

- Total Gross Orders
- Net Orders
- Weekly order trend
- Monthly order trend

### Cancellation KPIs

Cancellation indicators help monitor vendor reliability and operational stability.

- Total cancellations
- Cancellation rate
- Cancellation components
- Cancellation trend by period

### Issue KPIs

Issue indicators help track customer-facing operational quality.

- Total order issues
- Issue rate
- Issue components
- Long-term issue trend

### Delay KPIs

Delay indicators help identify operational friction in preparation, acceptance, or delivery-related flow.

- Preparation delay
- Confirmation delay
- Delivery-related delay indicators
- Delay trend over time

---

## Dashboard Use Case

This dashboard is mainly used as a performance monitoring layer.

It helps teams compare performance across time and detect whether operational KPIs are improving or deteriorating. It can also support monthly business reviews, performance program evaluation, and vendor lifecycle analysis.

Typical questions this dashboard helps answer include:

- Are cancellations decreasing over time?
- Are order issues improving after performance interventions?
- Are delays concentrated in specific periods?
- Is KPI movement related to order volume changes?
- Are recent improvements stable or temporary?
- Which performance areas require deeper investigation?

---

## Key Features

- Long-term KPI trend monitoring
- Weekly and monthly performance views
- Order volume context for KPI interpretation
- Cancellation, issue, and delay tracking
- Performance comparison across time periods
- Public-safe dataset for portfolio demonstration
- Tableau Public interactive dashboard embed

---

## Data Privacy

The public version of this dashboard does not use real company data.

For portfolio purposes, the dataset was transformed into a public-safe synthetic version. Sensitive vendor identifiers, operational fields, city-level details, and real KPI values were removed, shifted, masked, or replaced.

The synthetic data preserves the dashboard structure and analytical logic while preventing exposure of confidential business information.

---

## Tools Used

- Tableau
- SQL
- Python
- Excel
- KPI design
- Dashboard design
- Marketplace performance analysis
- Trend analysis

---

## What This Dashboard Demonstrates

This dashboard demonstrates my ability to build business-facing analytics products, not just isolated reports.

It shows how operational data can be transformed into a structured monitoring layer that supports recurring decision-making. The dashboard connects KPI design, data preparation, performance tracking, and business interpretation in one workflow.

For a marketplace environment, this type of dashboard helps teams move from reactive reporting to continuous performance governance.
