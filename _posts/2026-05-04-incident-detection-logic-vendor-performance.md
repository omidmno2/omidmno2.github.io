---
title: "Performance-Impacting Incident Detection Logic"
layout: post
date: 2026-05-04 17:00
image: /assets/images/markdown.jpg
headerImage: false
category: projects
project_group: marketplace
tags:
- Incident_Detection
- Anomaly_Detection
- Vendor_Performance
- KPI_Design
- Marketplace_Analytics
- Python
- Decision_Support
- Performance_Governance
star: true
description: "An incident detection logic designed to identify platform-driven performance shocks and support fairer vendor performance evaluation."
permalink: /performance-impacting-incident-detection/
---

## Overview

This project focused on designing a repeatable logic for identifying time windows where vendor performance KPIs may have been affected by platform-side incidents.

In marketplace operations, performance deterioration is not always caused by vendor behavior. Technical disruptions, operational incidents, platform-side delays, or wider service interruptions can temporarily affect vendor-facing KPIs.

The goal of this project was to create an upstream analytical layer that helps teams detect suspicious performance-impacting windows and review them before they affect downstream vendor evaluation.

This public version intentionally describes the project at a high level. Exact KPI definitions, thresholds, scoring logic, model weights, SQL logic, operational rules, and internal workflows are not disclosed.

---

## Business Context

Vendor performance indicators are often used in scoring systems, reward programs, cost-related workflows, operational reporting, and vendor follow-up.

If platform-driven incidents are not identified, vendors may be evaluated unfairly. A vendor could appear to have poor performance during a period when the underlying issue was actually caused by a platform disruption or external operational shock.

This project was designed to support a fairer performance governance process by helping teams answer one key question:

> Did this performance deterioration likely happen because of a broader incident rather than normal vendor behavior?

The logic was built to support review and decision-making, not to replace human judgment.

---

## Problem

Before this type of logic, incident review could be fragmented or dependent on manual reporting.

Several challenges made the problem difficult:

- not every incident is reported consistently;
- some reported incidents may not materially affect performance KPIs;
- some KPI shocks may happen without a clearly logged incident;
- manual review can be slow and inconsistent;
- downstream scoring and performance programs need defensible treatment of affected periods;
- business teams need explainable evidence before making exclusion or adjustment decisions.

The project addressed this gap by creating a structured analytical process for identifying candidate incident windows from performance behavior.

---

## Solution

The solution was a repeatable detection workflow based on performance data.

At a high level, the logic compares current performance behavior with expected historical behavior, identifies unusual deterioration, groups related signals into broader operational patterns, and produces candidate windows for review.

The output is not a final automated decision. It is a decision-support artifact that helps analysts and stakeholders prioritize which periods should be reviewed.

The exact implementation details are intentionally excluded from this public version.

---

## My Role

I designed the analytical logic and documentation behind the detection process.

My work included:

- framing the business problem behind performance-impacting incidents;
- translating operational concerns into an analytical detection approach;
- defining the high-level structure of the detection workflow;
- designing an explainable review process rather than a black-box model;
- connecting detection outputs to potential downstream performance governance use cases;
- documenting the process so it could be reused and maintained by the team;
- linking the logic to a dashboard-based review workflow.

This project required both analytical modeling and business judgment, because the output could influence how vendor performance is interpreted.

---

## Detection Approach

The detection logic is based on a simple principle:

> If important performance signals deteriorate unusually during the same time window, and the pattern is not consistent with normal business variation, the window may have been affected by an incident.

The model was designed to focus on performance-impacting incidents only. It does not attempt to detect every technical incident, nor does it try to replace technical monitoring systems.

The goal is narrower: to find time windows where KPI behavior suggests that vendor performance may have been distorted by a broader disruption.

---

## Baseline-Based Thinking

Marketplace KPIs naturally vary by hour, day, and operating conditions.

For example, some hours are naturally busier than others, and some performance indicators may behave differently during peak periods. Because of this, a fixed threshold can create misleading alerts.

The project therefore used a baseline-based logic: current behavior was compared with relevant historical behavior rather than judged only by static limits.

This helped separate normal operational variation from unusual performance shocks.

The exact baseline construction method is not disclosed in this public version.

---

## Signal Grouping

A key design choice was to avoid judging each metric in isolation.

Real operational incidents usually affect several related indicators at the same time. For this reason, the logic grouped related performance signals into broader operational patterns.

This made the output easier to interpret and helped reviewers understand the likely nature of the disruption without exposing internal metric definitions.

In the public version, these groups can be described at a high level as:

- order-flow disruption signals;
- order failure or unsuccessful outcome signals;
- latency and processing slowdown signals;
- broader activity disruption signals.

The exact internal KPIs, weights, thresholds, and classification rules are intentionally not disclosed.

---

## Review Levels

The workflow produces different levels of detection confidence.

Instead of returning only a binary yes/no result, the logic distinguishes between weaker signals and stronger incident candidates.

At a high level, the levels represent:

- normal behavior;
- weak signals requiring context;
- stronger candidate windows requiring review;
- severe or multi-dimensional disruption patterns.

This structure makes the output more useful for operational review, because not every anomaly should trigger the same level of attention.

Exact level definitions and decision rules are not included in this public version.

---

## Incident Window Construction

Incidents often affect more than one isolated hour.

For this reason, suspicious time periods are consolidated into broader candidate windows. This makes the output easier to review and more useful for business decision-making.

The final artifact is a list of candidate time windows that can be reviewed by analysts and stakeholders.

The public version does not include the internal output schema, file structure, or downstream operational format.

---

## Explainability

Explainability was a core requirement.

The goal was not just to flag a suspicious period, but to provide enough context for a human reviewer to understand why the period was flagged.

The detection logic was designed to support questions such as:

- What kind of performance behavior changed?
- Was the signal isolated or multi-dimensional?
- Does the pattern look operationally plausible?
- Should the period be reviewed before being used in downstream performance evaluation?

This explainability layer was important because the project supported sensitive vendor performance governance decisions.

---

## Weekly Workflow

The intended workflow was designed as a recurring review process.

At a high level, the process includes:

1. preparing recent performance data;
2. running the detection workflow;
3. reviewing candidate incident windows;
4. comparing results with available operational context;
5. documenting confirmed, uncertain, or rejected cases;
6. deciding whether any period should move to downstream review.

The workflow was intentionally designed to be repeatable and maintainable, rather than dependent on one person’s manual judgment.

Operational execution details are not disclosed in this public version.

---

## Dashboard Connection

This project was connected to a Tableau dashboard that helps visualize suspected incident windows alongside performance KPI movement.

The dashboard supports review by showing whether performance changes align with suspected incident periods and by helping analysts inspect before, during, and after behavior.

The public portfolio includes a synthetic-data version of that dashboard.

Related dashboard:

[Incident Detection & KPI Shock Analysis Dashboard](/incident-detection-kpi-shock-dashboard/)

---

## Business Value

The project helped create a more structured way to review performance-impacting incidents.

It supported:

- fairer vendor performance evaluation;
- better separation between vendor-driven issues and platform-driven disruptions;
- more consistent weekly review;
- stronger explainability for sensitive performance decisions;
- reduced dependence on manual incident discovery;
- better connection between analytics, operations, and performance governance.

The project was designed as an analytical support layer, not as an automatic enforcement system.

---

## Limitations

This was intentionally designed as a first-version detection layer.

It does not:

- detect every possible incident;
- replace technical monitoring;
- determine exact root cause with certainty;
- automatically apply downstream exclusions;
- identify all affected vendor segments;
- replace human review.

Its purpose is to identify candidate windows where performance behavior suggests that additional review is needed.

---

## Future Improvements

Potential future improvements include:

- segment-level detection;
- better scope inference by geography, vendor group, or category;
- stronger validation against operational incident records;
- improved root-cause interpretation;
- better false-positive tracking;
- closer integration with downstream review workflows;
- more formal versioning of configuration and review outcomes.

These improvements would make the process more precise while preserving explainability and governance control.

---

## Data Privacy

This public project page intentionally excludes confidential operational and technical details.

The following are not disclosed:

- internal KPI definitions;
- metric weights;
- exact thresholds;
- SQL logic;
- notebook structure;
- internal links;
- stakeholder names;
- vendor identifiers;
- private file paths;
- incident logs;
- operational exclusion rules;
- internal review formats;
- downstream system details.

The purpose of this page is to explain the business problem, analytical thinking, and project value without exposing implementation details that could reveal confidential company logic.

---

## Tools Used

- Python
- SQL
- Jupyter Notebook
- Tableau
- KPI design
- Anomaly detection
- Time-series analysis
- Data validation
- Performance governance
- Process documentation

---

## What This Project Demonstrates

This project demonstrates my ability to design analytical systems for sensitive business decisions.

It combines marketplace understanding, KPI governance, anomaly detection thinking, explainable analytics, and operational review design.

The main value of the project was not only detecting unusual KPI behavior, but helping make vendor performance systems fairer, more explainable, and less dependent on manual incident discovery.
