---
description: 'Wipro Linecraft AI Product Updates: April-May 2025'
---

# Apr-May '25

{% hint style="info" %}
Last PSS Version: 7.2.0&#x20;

New PSS Version: 7.3.0&#x20;
{% endhint %}

We’re excited to announce the launch of the Machine Monitoring module, providing real-time visibility into machine-level performance and enabling state-based prioritization. A new Parameters View has been introduced to offer KPI-driven insights across availability, performance, and quality. State Analysis now supports drill-down from cycles to state-level statistics for deeper root-cause investigation. Additional enhancements include redesigned heatmaps for improved readability, contextual subject lines in scheduled report emails, and in-app notifications for on-demand report availability.

## Features and improvements

#### New Module: Machine Monitoring

Introducing a new module within the product that provides users with a comprehensive view of all machines of a line along with their real-time status. It also includes a detailed machine-level view to help users understand individual machine performance and decide which machine to prioritize based on its state.

<figure><img src="../.gitbook/assets/image (93).png" alt=""><figcaption></figcaption></figure>

Launching a new ‘Parameters View’ as an alternative to the ‘Graph View’, enabling users to gain machine-level insights based on various KPIs related to availability, performance, and quality.&#x20;

<figure><img src="../.gitbook/assets/image (94).png" alt=""><figcaption></figcaption></figure>

The existing heatmap view will be retained. OEE monitoring functionalities will continue to be accessible from the existing heatmap.

<figure><img src="../.gitbook/assets/image (95).png" alt=""><figcaption></figcaption></figure>

#### State Analysis: Cycle Drill Down to State Statistics

Users can select a specific state as input for state analysis from various views and will be redirected to this view for deeper insights and drill-down at the state level.

<figure><img src="../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>

#### Improved subject line for scheduled report emails

The plant name will now be included in the email subject line, providing immediate context about which plant and line the report pertains to. This change addresses the confusion faced by users managing multiple lines, who previously had to open each email to identify the relevant line.

#### Notifications for On-Demand Report Completion

Users will now receive system notifications when on-demand reports are ready for download. Since these reports can span large time ranges and take longer to generate, this asynchronous approach allows users to continue working within the product and get notified once the report is available.

<figure><img src="../.gitbook/assets/image (97).png" alt=""><figcaption></figcaption></figure>

#### Redesign heatmaps to address data overlapping and improve usability

We’ve redesigned the heatmap to resolve issues where long asset names overlapped with the data, improving overall clarity and usability.

<figure><img src="../.gitbook/assets/image (98).png" alt=""><figcaption></figcaption></figure>

#### Optimized Loss Analysis Filter

The filter logic in the Loss Analysis module has been improved to minimize redundant API calls by streamlining how selections are made.

<figure><img src="../.gitbook/assets/image (99).png" alt=""><figcaption></figcaption></figure>

#### Asset-wise Production Summary Report – Improvements

Graph Update: Added hourly/daily data in a table alongside the line graph to allow users to view data in different resolutions.

Cycle Metrics: Minimum, maximum, and average self-cycle time now exclude partial cycles for accuracy.

<figure><img src="../.gitbook/assets/image (100).png" alt=""><figcaption></figcaption></figure>

#### Editable IOT & Quality Parameters via Settings

Ability to directly view and edit IOT and Quality parameters under Settings and Preferences, enabling faster updates without dependency on development teams.

<figure><img src="../.gitbook/assets/image (101).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (102).png" alt=""><figcaption></figcaption></figure>

#### Improved Logic for Identifying Critical Parallel Cells in the Critical Assets Module&#xD; The updated logic enhances the identification of parallel cells by analyzing bad part counts. By evaluating the contribution of each cell to overall part-level losses, the logic accurately ranks critical cells, even within parallel configurations.

This enhancement will ensure accurate identification of critical cells, including those in parallel arrangements, allowing for precise ranking in the Critical Assets module.

#### Improved Logic to Compute Cell-Level Quality

Refined the cell-level quality calculation by accurately identifying all unique serial numbers and corresponding reject signals. This approach ensures quality is computed based on the true count of inspected parts and actual rejections, eliminating data duplication or miscounts. The enhanced logic provides a more reliable and precise measure of quality performance at the cell level.
