---
title: "Incident Detection & KPI Shock Analysis Dashboard"
layout: post
date: 2026-05-04 11:00
image: /assets/images/markdown.jpg
headerImage: false
category: dashboards
dashboard_group: performance
tags:
- Tableau
- Incident_Detection
- KPI_Monitoring
- Vendor_Performance
- Marketplace_Analytics
- Anomaly_Detection
star: true
description: "Tableau dashboard for identifying platform-driven incidents and matching them with operational KPI shocks to support fairer vendor performance evaluation."
permalink: /incident-detection-kpi-shock-dashboard/
---

## Overview

This dashboard was designed to identify operational incidents and analyze their impact on vendor performance KPIs.

In marketplace operations, KPI deterioration is not always caused by vendor behavior. Sometimes performance drops are driven by platform-side issues, order-flow disruptions, technical incidents, logistics instability, or external shocks. This dashboard helps detect those windows and compare them against hourly KPI movements.

The goal is to support fairer performance evaluation by separating vendor-driven issues from platform-driven disruptions.

---

## Business Context

Vendor performance systems often rely on operational KPIs such as cancellation rate, issue rate, confirmation delay, no-ack rate, and delivery-related delays.

However, these KPIs can be affected by incidents outside the vendor’s control. For example, a backend disruption, vendor panel issue, order confirmation flow problem, or logistics-side instability may create a temporary KPI shock across many vendors.

Without identifying these windows, downstream scoring systems may unfairly penalize vendors for platform-driven failures.

This dashboard was built to help business, operations, and performance teams answer three questions:

1. When did a potential incident happen?
2. Which KPIs moved abnormally during that time window?
3. Should the affected period be reviewed or excluded from vendor performance calculations?

---

## Interactive Dashboard

<div style="background:#fff8e1; border-left:4px solid #f4b400; padding:12px 16px; margin:20px 0; border-radius:6px; font-size:1.25rem; line-height:1.5;">
  <strong>Viewing tip:</strong> For the best experience, open this dashboard in fullscreen mode or view it directly on Tableau Public.
</div>

The dashboard below is published on Tableau Public using a public-safe synthetic dataset. It preserves the analytical structure of the original work without exposing confidential company data.

<div class="tableau-embed-wrapper">
<div class='tableauPlaceholder' id='viz1777899870859' style='position: relative'>
  <noscript>
    <a href='https://public.tableau.com/views/Incident_17659600637510/Story2'>
      <img alt='Incident Detection and KPI Shock Analysis Dashboard'
           src='https://public.tableau.com/static/images/In/Incident_17659600637510/Story2/1_rss.png'
           style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz' style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
    <param name='embed_code_version' value='3' />
    <param name='site_root' value='' />
    <param name='name' value='Incident_17659600637510/Story2' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https://public.tableau.com/static/images/In/Incident_17659600637510/Story2/1.png' />
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
  var divElement = document.getElementById('viz1777899870859');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width = '100%';
  vizElement.style.height = (divElement.offsetWidth * 0.75) + 'px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

<p>
  <a href="https://public.tableau.com/views/Incident_17659600637510/Story2" target="_blank">
    Open the dashboard on Tableau Public
  </a>
</p>

---

## My Role

I designed the analytical logic behind the dashboard and prepared the data structure required to compare incident windows with hourly KPI behavior.

My work included:

- defining the KPI families used for incident monitoring;
- preparing hourly performance data for dashboard analysis;
- structuring incident windows for comparison with KPI trends;
- designing the logic for matching incidents with affected time periods;
- creating a public-safe version of the dataset for portfolio presentation;
- documenting how incident windows can support fairer downstream treatment in Vendor Performance Scoring and Reward & Cost workflows.

---

## Dashboard Logic

The dashboard compares incident records with hourly operational KPIs.

The main idea is simple: if several related KPIs move abnormally during the same time window, the dashboard highlights that period as a potential incident impact window.

The KPI families include:

### Flow KPIs

These indicators show whether the normal order flow was disrupted.

- Pending action rate
- Confirmation delay rate
- No-ack rate

### Cancellation and NFC KPIs

These indicators help detect whether order failures increased during the suspected incident period.

- Cancellation rate
- Vendor-related cancellation components
- Rider or logistics-related NFC components

### Latency KPIs

These indicators help identify operational slowdowns.

- Average estimated preparation time
- Average actual preparation time
- Average delivery time
- Average end-to-end delivery time

### Volume KPIs

These indicators help detect sudden drops or unusual movements in order volume.

- Total gross orders
- Net orders
- Hourly order trend

---

## Dashboard Use Case

The dashboard is mainly used as a diagnostic layer.

It helps teams inspect whether a KPI shock was isolated, vendor-specific, or part of a wider platform-side incident. When a suspicious time window is detected, analysts can compare KPI behavior before, during, and after the incident.

This can support decisions such as:

- reviewing affected KPI windows;
- excluding incident periods from vendor scoring;
- preventing unfair vendor penalties;
- documenting incident impact for business and operations teams;
- improving trust in performance governance systems.

---

## Key Features

- Hourly KPI trend monitoring
- Incident window overlay
- Before / during / after incident comparison
- KPI-family-based interpretation
- Support for performance-score exclusion logic
- Public-safe data structure for portfolio demonstration

---

## Data Privacy

The public version of this dashboard does not use real company data.

For portfolio purposes, the dataset was transformed into a public-safe synthetic version. Real incident IDs, operational comments, ticket references, vendor identifiers, and sensitive KPI values were removed or replaced.

The synthetic data preserves the analytical structure of the dashboard, including hourly KPI movements and incident-window matching, without exposing confidential business information.

---

## Tools Used

- Tableau
- SQL
- Python
- Excel
- KPI design
- Anomaly detection logic
- Marketplace performance analysis

---

## What This Dashboard Demonstrates

This dashboard demonstrates my ability to connect analytics with operational decision-making.

It is not only a reporting dashboard. It is a decision-support layer designed to help teams understand whether performance deterioration reflects vendor behavior or broader platform-side disruptions.

The project combines KPI design, incident analysis, data preparation, dashboarding, and performance governance.
