# Bottleneck Report

**Overview**

The Bottleneck Report provides a comprehensive week-over-week analysis of production bottlenecks, along with detailed cycle-level and state-level insights. It helps users understand the underlying causes of bottlenecks and delivers actionable recommendations to improve production performance by addressing identified issues.

The primary objective is to enable data-driven decision-making that enhances throughput and operational efficiency.\
<br>

<figure><img src="../../.gitbook/assets/Bottleneck Report (2).png" alt=""><figcaption></figcaption></figure>

**What the Report Delivers**

**1. Executive KPI Snapshot**

The report presents a consolidated summary of overall production performance, including:

* Overall Equipment Effectiveness (OEE)
* Availability
* Performance
* Quality
* Total Production

This snapshot provides leadership with a quick and clear view of operational health.

**2. Identification of Bottleneck Machines**

Machines are ranked using a Machine Importance Score, highlighting the most impactful bottlenecks in descending order.

This prioritization enables teams to focus improvement efforts where they will generate the greatest operational benefit.

**Structured Loss Analysis (A → P → Q Framework)**

For each identified bottleneck machine, opportunities are analyzed in a structured and standardized sequence:

Availability and/or Stability → Performance

This framework ensures clarity, logical prioritization, and effective root-cause analysis when multiple opportunity categories exist.

**Top Availability Opportunity**

When availability losses are detected, the report provides:

* The top Availability Opportunity
* Top 10 fault codes with corresponding source entities
* Fault descriptions
* Production impact (in parts)
* Total downtime duration
* Total downtime occurrences per fault

Faults are automatically ranked by total downtime duration, allowing maintenance teams to prioritize the most impactful issues quickly.

If no availability losses are recorded, this section remains blank to maintain a clean and focused report.

**Top Stability Opportunity**

When stability-related losses are identified, the report includes:

* The top Stability Opportunity
* Most problematic states ranked by occurrence
* Production impact (in parts)
* Fault descriptions

**Self-Cycle Histogram**

The report also includes a Self-Cycle Histogram showing:

* Identified problematic state instances
* State durations

This visualization helps teams identify:

* State time deviations
* Average state duration
* Comparison against target cycle time
* Process variability
* Throughput instability

By analyzing state behaviour, teams can address the most critical instability factors and eliminate hidden performance inefficiencies.

If no stability opportunity is detected, this section remains blank.

**Top Performance Opportunity**

When performance-related losses are identified, the report includes:

Shift-wise and Part-type-wise Self-Cycle Histograms

These histograms highlight cycles from assets with the most inefficient cycle behavior.

They help uncover:

* Cycle time deviations
* Cycles exceeding target cycle time
* JPH (Jobs Per Hour) loss due to over-cycling
* Comparison with average and target cycle durations
* Process variability
* Throughput instability

**Additional Shift-wise Insights**

* Total cycles per shift
* Over-cycling occurrences
* Average cycle time
* Minimum cycle time
* Maximum cycle time&#x20;

**Additional Part-type-wise Insights**

* Total cycles per part type
* Over-cycling occurrences
* Average cycle time
* Minimum cycle time
* Maximum cycle time

By analyzing cycle behaviour at both shift and part-type levels, teams can stabilize line speed, reduce variability, and eliminate hidden performance inefficiencies.

If no performance opportunities are detected, this section remains blank.\
<br>

