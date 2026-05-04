---
title: "Cancellation & VMS Training Dashboard"
layout: post
date: 2026-05-04 14:00
image: /assets/images/markdown.jpg
headerImage: false
category: dashboards
tags:
- Tableau
- Operations_Analytics
- Vendor_Training
- Cancellation_Analysis
- Confirmation_Delay
- Vendor_Performance
- Marketplace_Analytics
star: true
description: "Tableau dashboard designed to support vendor training and operational follow-up for cancellation behavior and confirmation delay issues."
permalink: /cancellation-vms-training-dashboard/
---

## Overview

This dashboard was created to support vendor training and operational follow-up in two important performance areas:

- cancellation behavior;
- confirmation delay, previously referred to internally as VMS delay.

The dashboard was designed as a practical tool for the Operation team to identify vendors who may need training, consultation, or closer follow-up.

Its main purpose was not only to report performance problems, but to help the team act on them.

---

## Business Context

In a marketplace environment, vendor-side operational behavior directly affects customer experience, order reliability, and service quality.

Two recurring issues are especially important:

1. vendors cancelling orders after receiving them;
2. vendors delaying order confirmation.

Both issues can create friction for customers, increase operational workload, reduce trust in the platform, and negatively affect downstream vendor performance scores.

The Operation team needed a dashboard that could help them identify vendors with repeated cancellation or confirmation-delay problems and use that information for training and intervention planning.

This dashboard was built around that need.

---

## Interactive Dashboard

The dashboard below is published on Tableau Public using a public-safe synthetic dataset. It preserves the analytical structure of the original dashboard without exposing confidential company data.

<div class="tableau-embed-wrapper">
<div class='tableauPlaceholder' id='viz1777921028171' style='position: relative'>
  <noscript>
    <a href='https://public.tableau.com/views/CancelationVMSTrainingv1/Story1'>
      <img alt='Cancellation and VMS Training Dashboard'
           src='https://public.tableau.com/static/images/Ca/CancelationVMSTrainingv1/Story1/1_rss.png'
           style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz' style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
    <param name='embed_code_version' value='3' />
    <param name='site_root' value='' />
    <param name='name' value='CancelationVMSTrainingv1/Story1' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https://public.tableau.com/static/images/Ca/CancelationVMSTrainingv1/Story1/1.png' />
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
  var divElement = document.getElementById('viz1777921028171');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width = '100%';
  vizElement.style.height = (divElement.offsetWidth * 0.75) + 'px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

<p>
  <a href="https://public.tableau.com/views/CancelationVMSTrainingv1/Story1" target="_blank">
    Open the dashboard on Tableau Public
  </a>
</p>

---

## My Role

I designed this dashboard to support the Operation team’s vendor training workflow.

My work included:

- understanding the team’s training and follow-up needs;
- defining the cancellation and confirmation-delay indicators required for vendor diagnosis;
- structuring the dashboard around operational actionability;
- creating views to identify vendors with repeated or severe performance issues;
- supporting the team in using the dashboard for training and consultation;
- preparing a public-safe version of the dashboard for portfolio presentation.

---

## Dashboard Logic

The dashboard focuses on identifying vendors who require operational attention.

The logic is based on comparing vendor behavior across cancellation and confirmation-delay indicators. Vendors with high rates, repeated issues, or worsening behavior can be prioritized for training or follow-up.

The dashboard helps move the team from manual checking to a more structured intervention workflow.

---

## Main Analytical Areas

### Cancellation Analysis

Cancellation is one of the most important vendor performance problems because it directly affects customer experience and order reliability.

The dashboard helps identify:

- vendors with high cancellation behavior;
- vendors with repeated cancellation problems;
- cancellation patterns across time;
- vendors requiring training or intervention;
- segments or areas where cancellation behavior is more visible.

### Confirmation Delay Analysis

Confirmation delay, previously referred to as VMS delay, happens when vendors take too long to confirm incoming orders.

The dashboard helps investigate:

- vendors with high confirmation delay;
- delay patterns across selected periods;
- vendors that may need operational education;
- whether the issue is recurring or temporary;
- which vendors should be prioritized for follow-up.

### Vendor Training Prioritization

The main output of the dashboard is a practical training list.

Instead of only showing KPIs, the dashboard helps the Operation team decide which vendors should be contacted, trained, or monitored more closely.

---

## Dashboard Use Case

This dashboard is mainly used for vendor training and operational follow-up.

Typical use cases include:

- identifying vendors with high cancellation rates;
- finding vendors with repeated confirmation-delay issues;
- preparing vendor training lists;
- supporting operational consultation with data;
- tracking whether problematic vendors need repeated follow-up;
- helping the Operation team prioritize limited training capacity.

---

## Key Features

- Cancellation monitoring
- Confirmation-delay monitoring
- Vendor-level training prioritization
- Support for operational follow-up
- Practical views for the Operation team
- Public-safe Tableau Public version for portfolio demonstration

---

## Data Privacy

The public version of this dashboard does not use real company data.

For portfolio purposes, the dataset was transformed into a public-safe synthetic version. Sensitive vendor identifiers, internal operational details, real KPI values, user-related data, and confidential business fields were removed, masked, shifted, or replaced.

The public version preserves the dashboard structure and analytical logic while preventing exposure of confidential business information.

Internal team names, internal BI links, and private operational references are intentionally not included in this public portfolio page.

---

## Tools Used

- Tableau
- SQL
- Excel
- KPI design
- Vendor performance analysis
- Operations analytics
- Vendor training support
- Dashboard design

---

## What This Dashboard Demonstrates

This dashboard demonstrates my ability to build analytics tools that directly support operational action.

It was created for a specific business need: helping the Operation team identify vendors who require training for cancellation and confirmation-delay issues.

The project combines KPI design, operational diagnosis, dashboard development, and stakeholder-oriented analytics. It shows how a dashboard can move beyond reporting and become part of a practical vendor improvement workflow.
