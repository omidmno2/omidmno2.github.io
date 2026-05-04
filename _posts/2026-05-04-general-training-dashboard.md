---
title: "General Training Dashboard"
layout: post
date: 2026-05-04 13:00
image: /assets/images/markdown.jpg
headerImage: false
category: dashboards
tags:
- Tableau
- Operations_Analytics
- Vendor_Training
- Vendor_Performance
- Marketplace_Analytics
- KPI_Monitoring
- Dashboard_Design
star: true
description: "Tableau dashboard designed to support the Operation team with vendor training, consultation, follow-up, and performance diagnosis."
permalink: /general-training-dashboard/
---

## Overview

This dashboard was created to address the general and recurring analytical needs of the Operation team.

The main goal was to provide the team with a single practical tool for vendor training, operational follow-up, and consultation. Instead of relying on several limited or fragmented reports, the dashboard was designed as a broader operational layer where the team could investigate vendor behavior, performance problems, regional differences, product-level issues, and customer experience indicators.

The dashboard helped the Operation team answer frequent business questions more quickly and with more flexibility.

---

## Business Context

The Operation team needed a dashboard that could support day-to-day vendor consultation and training.

Before this dashboard, several existing reports had limitations. Some of them were too static, some did not include enough visual analysis, some did not support filtering properly, and some had originally been designed for Key Account users rather than the broader Operation team.

As a result, the team needed a more accessible and flexible dashboard that could help them investigate vendor performance, identify operational problems, and guide conversations with vendors.

This dashboard was created after multiple sessions with the Operation team, where their needs were collected, reviewed, prioritized, and translated into dashboard requirements.

---

## Interactive Dashboard

<div style="background:#fff8e1; border-left:4px solid #f4b400; padding:12px 16px; margin:20px 0; border-radius:6px; font-size:1.25rem; line-height:1.5;">
  <strong>Viewing tip:</strong> For the best experience, open this dashboard in fullscreen mode or view it directly on Tableau Public.
</div>

The dashboard below is published on Tableau Public using a public-safe synthetic dataset. It preserves the analytical structure of the original dashboard without exposing confidential company data.

<div class="tableau-embed-wrapper">
<div class='tableauPlaceholder' id='viz1777920776212' style='position: relative'>
  <noscript>
    <a href='https://public.tableau.com/views/GeneralTrainingDashboardLive_V7/ExcellenceStory'>
      <img alt='General Training Dashboard'
           src='https://public.tableau.com/static/images/Ge/GeneralTrainingDashboardLive_V7/ExcellenceStory/1_rss.png'
           style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz' style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
    <param name='embed_code_version' value='3' />
    <param name='site_root' value='' />
    <param name='name' value='GeneralTrainingDashboardLive_V7/ExcellenceStory' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https://public.tableau.com/static/images/Ge/GeneralTrainingDashboardLive_V7/ExcellenceStory/1.png' />
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
  var divElement = document.getElementById('viz1777920776212');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width = '100%';
  vizElement.style.height = (divElement.offsetWidth * 0.75) + 'px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

<p>
  <a href="https://public.tableau.com/views/GeneralTrainingDashboardLive_V7/ExcellenceStory" target="_blank">
    Open the dashboard on Tableau Public
  </a>
</p>

---

## My Role

I designed this dashboard based on the operational needs collected from the Operation team.

My work included:

- collecting and structuring the team’s recurring analytical questions;
- translating operational needs into dashboard requirements;
- defining the KPI and filter logic needed for vendor consultation;
- designing dashboard views for training, follow-up, and issue diagnosis;
- improving accessibility compared with previous static or limited reports;
- training the Operation team on how to use the dashboard;
- preparing a public-safe version of the dashboard for portfolio presentation.

---

## Dashboard Logic

The dashboard was designed around the questions that the Operation team repeatedly needed to answer during vendor training and follow-up.

Instead of focusing on a single KPI, it brings together multiple views related to vendor performance, basket behavior, product activity, delivery timing, regional comparison, and customer dissatisfaction.

The dashboard supports both high-level monitoring and detailed operational investigation.

---

## Operational Questions Covered

The dashboard helps answer questions such as:

- What is the average basket size?
- How many performance-related cases or issues are visible for a vendor?
- Which vendors or areas have higher delay indicators?
- Which products are more frequently sold?
- How long does basket preparation or order sending take?
- How does a vendor perform compared with nearby vendors or areas?
- How much month-over-month growth is visible?
- Which vendors are active in selected food categories?
- How many new and returning users are active in a selected area?
- What is the share of organic versus non-organic orders?
- Which areas show higher delayed orders?
- What are the main reasons for customer dissatisfaction?
- Which indicators contributed most to a negative performance score?
- How active are a vendor’s menu items?
- Which products or vendors should be treated as best sellers?
- Where does delay occur: preparation, confirmation, dispatch, or delivery flow?
- How do performance indicators compare with surrounding areas?

---

## Main Analytical Areas

### Vendor Training and Consultation

The dashboard supports operational conversations with vendors by showing where performance issues appear and which areas require follow-up.

It gives the Operation team a structured way to explain problems and recommend corrective actions.

### Basket and Product Analysis

The dashboard includes views related to basket size, product activity, best-selling items, and menu performance.

This helps the team identify whether performance issues are connected to product availability, product attractiveness, menu activity, or preparation complexity.

### Regional and Area-Level Comparison

The dashboard allows users to compare vendors or operational indicators across areas.

This helps distinguish whether an issue is vendor-specific or part of a broader local pattern.

### Delay and Service Quality

The dashboard helps investigate where delay-related problems occur, including preparation, confirmation, dispatch, and delivery-related stages.

This supports more precise vendor consultation because the team can focus on the actual source of the operational friction.

### Customer Dissatisfaction

The dashboard includes customer dissatisfaction signals and performance-related reasons, helping the Operation team connect internal KPIs with customer experience.

---

## Dashboard Use Case

This dashboard is mainly used as an operational enablement tool.

It helps the Operation team prepare for vendor conversations, identify training priorities, and follow up on recurring issues. Instead of manually checking multiple reports, users can access one dashboard to investigate performance from different angles.

Typical use cases include:

- preparing for vendor training sessions;
- diagnosing why a vendor’s performance is weak;
- identifying product or menu-related problems;
- comparing a vendor with surrounding areas;
- checking whether delay is concentrated in a specific operational stage;
- understanding customer dissatisfaction drivers;
- supporting consultation with data-backed evidence.

---

## Key Features

- Centralized operational dashboard for the Operation team
- Vendor-level and area-level performance diagnosis
- Product and basket behavior analysis
- Delay and service-quality tracking
- Customer dissatisfaction analysis
- Flexible filtering for operational follow-up
- Support for vendor training and consultation
- Public-safe Tableau Public version for portfolio demonstration

---

## Data Privacy

The public version of this dashboard does not use real company data.

For portfolio purposes, the dataset was transformed into a public-safe synthetic version. Sensitive vendor identifiers, internal operational details, area names, user-related data, and real KPI values were removed, masked, shifted, or replaced.

The public version preserves the dashboard structure and analytical logic while preventing exposure of confidential business information.

Internal Tableau and BI links are intentionally not included in this public portfolio page.

---

## Tools Used

- Tableau
- SQL
- Excel
- KPI design
- Dashboard design
- Operations analytics
- Vendor performance analysis
- Stakeholder requirement gathering

---

## What This Dashboard Demonstrates

This dashboard demonstrates my ability to turn stakeholder needs into a practical analytics product.

It was not built only as a reporting layer. It was designed as an operational tool that helps a business team diagnose problems, train vendors, and make follow-up conversations more data-driven.

The project combines requirement gathering, KPI design, dashboard development, operational thinking, and stakeholder training.
