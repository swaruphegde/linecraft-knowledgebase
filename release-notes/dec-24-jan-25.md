---
description: 'Wipro Linecraft AI Product Updates: Dec 2024 - Jan 2025'
---

# Dec '24-Jan '25

{% hint style="info" %}
Last PSS Version: 7.1.0&#x20;

New PSS Version: 7.2.0&#x20;
{% endhint %}

## Features and improvements

#### String Fault Support:

Linecraft will now support string-based fault descriptions from PLCs, extending beyond the existing integer and Boolean fault types. This enhancement allows for more accurate fault tracking, even when fault codes are not included in the fault code mapping, ensuring precise fault identification and resolution.

#### Condition Monitoring:

We are overhauling the existing alerts module to provide users with enhanced visualization and analysis capabilities. Key features include:

* Alert Trend Visualization: Users can easily track trends over time to spot recurring issues.
* Top Alerts Insights: Identifying the assets and parameters that generate the most alerts for targeted action.
* Condition Scheduling: Users can now schedule multiple conditions for the same parameter in one go, streamlining the alert configuration process.
* My alerts: A dedicated space to manage alerts set up by you. This section lists alerts that you have created and enables you to manage your alerts in one place.
* Duplicate Alert Prevention: Built-in safeguards to avoid the creation of redundant alerts.
* Alert History Analysis: A comprehensive view of past alerts for better decision-making.

These improvements empower users to detect issues early and respond more effectively delivering even more business value.

#### Enhanced Part Trace View and End of the day part trace report:

We’re adding new details to the Part Trace View, Excel export, and End-of-Day Part Trace Report. Users can now track the total time spent on the line and during Valid Production Time for each part or part type. This additional data enables more detailed analysis, helping customers understand production trends for specific part types and leverage insights to optimize efficiency and performance.

#### Critical Cells to include only VPI time for computation

Introducing an enhancement to critical cell logic that now considers only valid production time (excluding off-shift time and break cycles) for computations. This update ensures that availability and performance metrics provide a clear and accurate representation of production performance.

#### Production Overview:

We are revamping the current production scheduling capabilities and introducing a more robust module. Key features include:

* Shift & Day Visualization: A clear, at-a-glance view of production across shifts and days, along with critical production KPIs.
* Key Production Parameter Analysis: Users can easily analyze production data for essential parameters to ensure efficiency for selected time-range.

This upgrade aims to offer greater control and insight, helping users optimize production processes more effectively.

#### Bottleneck Analysis Report:

Introducing bottleneck report generation process to deliver vital insights more efficiently. This report provides a weekly analysis of bottlenecks, including key cycle-level and state-level data, helping users pinpoint critical areas for improvement. The goal is to offer actionable insights and recommendations to resolve bottlenecks, leading to production enhancements and value optimization.

#### Improved Heatmap Information:

Users will now receive clear notifications when no data is available in the selected date range on heatmaps, ensuring they have accurate information and eliminating confusion.

#### Config tool reduction/update:

We’re launching an updated, intuitive UI for the configuration tool, eliminating outdated screens to streamline navigation and improve efficiency.\
Users will experience a simplified workflow, making it easier to find relevant options and complete tasks faster.

#### Data Collection Monitoring and Remote Management:

We’re excited to introduce a Data Collection Monitoring and Remote Management platform in the latest Linecraft product update. This new feature empowers the engineering team to monitor data loggers’ connectivity, service status, storage, and synchronization seamlessly, enabling quick identification and resolution of service interruptions or data discrepancies.

#### Key Highlights:&#x20;

1. Logger Overview Section: Real-time visibility into connectivity and operational status of data loggers. Alerts for critical issues (e.g., service downtime, storage limits). Displays plant server details with time sync alerts.&#x20;
2. Data Sync Monitoring: Monitors synchronization status and triggers alerts for unsynced loggers.&#x20;
3. MQTT Monitoring Section: Ensures MQTT broker is running, with downtime alerts. Displays connection status and timestamps to identify delays.&#x20;
4. Real-Time Dashboard: Color-coded indicators for quick issue identification.&#x20;
5. Critical Alerts: Email/SMS notifications for service interruptions, storage issues, and time sync offsets.&#x20;
6. &#x20;New alert configuration to track mandatory states:&#x20;

To prevent production issues, we are introducing alerts that trigger when mandatory states in a cycle are skipped. This proactive measure helps the production team address missed steps early, preventing defective products, rework, and costly inefficiencies, while improving overall quality and performance.&#x20;

