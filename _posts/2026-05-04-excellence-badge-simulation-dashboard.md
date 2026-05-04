---
title: "Excellence Badge Simulation Dashboard"
layout: post
date: 2026-05-04 15:00
image: /assets/images/markdown.jpg
headerImage: false
category: dashboards
tags:
- Tableau
- Vendor_Performance
- Badge_Simulation
- Threshold_Analysis
- Marketplace_Analytics
- KPI_Design
- Decision_Support
star: true
description: "Tableau dashboard designed to simulate Excellence Badge eligibility by testing KPI thresholds and analyzing which vendors would qualify under different scenarios."
permalink: /excellence-badge-simulation-dashboard/
---

## Overview

This dashboard was designed to support decision-making for an Excellence Badge program.

The main purpose was to simulate how different KPI thresholds would affect vendor eligibility. By adjusting the thresholds, business and operations teams could understand how many vendors would qualify for the badge, what characteristics those vendors had, and exactly which vendors would be selected.

The dashboard helped transform badge design from a static rule-setting exercise into a more transparent and data-driven simulation process.

---

## Business Context

In marketplace performance programs, badge eligibility rules need to be carefully designed.

If the thresholds are too strict, only a very small number of vendors qualify and the badge may lose its motivational impact. If the thresholds are too loose, too many vendors qualify and the badge may lose credibility.

The team needed a way to test different scenarios before finalizing the badge logic.

This dashboard was created to answer questions such as:

1. How many vendors would receive the badge under each threshold scenario?
2. Which vendors would qualify?
3. What are the performance characteristics of eligible vendors?
4. How would eligibility change if thresholds became stricter or more flexible?
5. Would the selected vendors represent meaningful performance excellence?

---

## Interactive Dashboard

The dashboard below is published on Tableau Public using a public-safe synthetic dataset. It preserves the analytical structure of the original dashboard without exposing confidential company data.

<div class="tableau-embed-wrapper">
<div class='tableauPlaceholder' id='viz1777921167729' style='position: relative'>
  <noscript>
    <a href='https://public.tableau.com/views/Book1_17775836744800/Story1'>
      <img alt='Excellence Badge Simulation Dashboard'
           src='https://public.tableau.com/static/images/Bo/Book1_17775836744800/Story1/1_rss.png'
           style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz' style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
    <param name='embed_code_version' value='3' />
    <param name='site_root' value='' />
    <param name='name' value='Book1_17775836744800/Story1' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https://public.tableau.com/static/images/Bo/Book1_17775836744800/Story1/1.png' />
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
  var divElement = document.getElementById('viz1777921167729');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width = '100%';
  vizElement.style.height = (divElement.offsetWidth * 0.75) + 'px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

<p>
  <a href="https://public.tableau.com/views/Book1_17775836744800/Story1" target="_blank">
    Open the dashboard on Tableau Public
  </a>
</p>

---

## My Role

I designed the simulation logic and dashboard structure for analyzing badge eligibility scenarios.

My work included:

- defining the KPI dimensions used for badge eligibility;
- preparing multi-month vendor performance data for simulation;
- designing adjustable threshold logic in Tableau;
- creating views to show how many vendors qualify under each scenario;
- enabling vendor-level drill-down to identify exactly which vendors would receive the badge;
- comparing eligible vendors by performance characteristics;
- supporting business decision-making before finalizing the badge criteria;
- preparing a public-safe version of the dashboard for portfolio presentation.

---

## Dashboard Logic

The dashboard works as a threshold simulation tool.

Instead of applying one fixed rule, users can adjust selected KPI thresholds and immediately see how eligibility changes. This makes the badge design process more transparent and easier to discuss with stakeholders.

The dashboard connects three layers of analysis:

1. **Threshold selection**  
   Users can change the required performance levels.

2. **Eligibility calculation**  
   The dashboard recalculates which vendors qualify based on the selected rules.

3. **Vendor-level interpretation**  
   Users can inspect the number, profile, and identity of eligible vendors.

This structure helps teams understand the consequences of each badge scenario before applying it in practice.

---

## Main Analytical Areas

### Threshold Analysis

The dashboard allows users to test different eligibility thresholds and evaluate their business impact.

This helps answer:

- How many vendors qualify if the threshold is stricter?
- How many vendors qualify if the threshold is more flexible?
- Which KPI threshold has the strongest effect on eligibility?
- Does the final selection look too broad or too narrow?

### Vendor Eligibility Simulation

The dashboard identifies vendors that meet the selected criteria.

This supports operational and business teams in reviewing whether the selected vendors are aligned with the intended meaning of “excellence.”

### Multi-Month Performance Review

The dashboard covers several months of vendor performance data.

This is important because badge eligibility should not be based on a single short-term snapshot. Multi-month analysis helps identify vendors with more stable and consistent performance.

### Vendor Profile Analysis

The dashboard helps compare eligible and non-eligible vendors by their characteristics.

This makes it easier to understand whether badge recipients are concentrated in specific segments, areas, order-volume levels, or performance groups.

---

## Dashboard Use Case

This dashboard is mainly used for policy design and decision support.

Typical use cases include:

- testing badge eligibility rules before launch;
- comparing different KPI threshold scenarios;
- estimating the number of vendors who would receive the badge;
- reviewing the exact vendor list under each scenario;
- checking whether badge eligibility is too strict or too broad;
- supporting discussions between business, operations, product, and performance teams;
- making the final badge logic more transparent and defensible.

---

## Key Features

- Adjustable KPI threshold simulation
- Vendor eligibility calculation
- Multi-month performance coverage
- Vendor-level drill-down
- Scenario comparison
- Badge population size analysis
- Support for business rule design
- Public-safe Tableau Public version for portfolio demonstration

---

## Data Privacy

The public version of this dashboard does not use real company data.

For portfolio purposes, the dataset was transformed into a public-safe synthetic version. Sensitive vendor identifiers, internal business rules, real KPI values, city or area details, and confidential operational information were removed, masked, shifted, or replaced.

The public version preserves the simulation structure and analytical logic while preventing exposure of confidential business information.

---

## Tools Used

- Tableau
- SQL
- Excel
- KPI design
- Threshold analysis
- Scenario simulation
- Vendor performance analysis
- Marketplace analytics
- Decision-support dashboarding

---

## What This Dashboard Demonstrates

This dashboard demonstrates my ability to build analytical tools for business policy design.

The project was not only about visualizing data. It was about helping stakeholders test the consequences of different rule choices before applying them to vendors.

It combines KPI design, threshold simulation, vendor-level analysis, and decision-support logic. This type of dashboard helps teams make performance programs more transparent, measurable, and fair.
