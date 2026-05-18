# Asset-wise Availability Losses Report

## Overview

The Asset-Wise Availability Losses Report provides a consolidated operational view of asset-level availability losses, downtime contribution and recurring fault behavior across the manufacturing line.&#x20;

It is designed to help production and maintenance teams quickly identify which assets are contributing most significantly to availability degradation and prioritize corrective actions with minimal interpretation overhead.

> _This report is intended for production managers, maintenance teams and operational leaders working under live manufacturing conditions, where rapid interpretation and operational clarity are critical._

## Operational purpose

The Asset-Wise Availability Losses Report helps teams:

* identify assets contributing most to availability loss
* understand recurring fault patterns across machines
* prioritize maintenance intervention using downtime impact
* analyze fault occurrence frequency across assets
* reduce hidden availability losses
* improve overall equipment effectiveness (OEE)

## Report walkthrough

### Report availability

The Asset-Wise Availability Losses Report is available under the Reports module. Users can generate the report in two ways:

{% stepper %}
{% step %}
### Schedule report generation

The report can be configured to generate automatically for recurring operational reviews and maintenance analysis workflows.
{% endstep %}

{% step %}
### On-demand report generation

Users can generate the report instantly whenever downtime investigation or availability analysis is required.
{% endstep %}
{% endstepper %}

## Report sections



<figure><img src="../../.gitbook/assets/image (208).png" alt=""><figcaption></figcaption></figure>

The report provides a detailed lists of all assets and their faults, which can be sorted by fault occurrence or fault duration. Each asset consists of

&#x20;the following fault-related information:

| Parameter                  | Definition                                                       |
| -------------------------- | ---------------------------------------------------------------- |
| Asset name                 | Contains name of the individual asset                            |
| Total uptime               | Displays the time (in hh:mm:ss format) an asset was cycling      |
| Total downtime             | Displays the time (in hh:mm:ss format) an asset was down         |
| Total downtime occurrences | Displays the total duration an asset was down due to faults      |
| Fault code                 | Represents a unique code for faults                              |
| Source entity              | Contains cell or asset on which a fault originated from          |
| Fault name                 | Contains human-readable description of faults                    |
| Duration                   | Displays the total duration of occurrence of a fault in an asset |
| Occurrence                 | Displays the total number of times a fault occurred in an asset  |

## Operational interpretation guidelines

When analyzing the Asset-Wise Availability Losses Report, focus on:

| Operational signal                             | What it may indicate                        |
| ---------------------------------------------- | ------------------------------------------- |
| High downtime concentration on specific assets | Major availability degradation source       |
| Repeated occurrence of the same fault          | Chronic operational instability             |
| High occurrence with low downtime              | Frequent micro-interruptions                |
| Low occurrence with high downtime              | Severe operational failure events           |
| Repeated faults from same source entity        | Systemic subsystem instability              |
| Rising downtime trends across assets           | Emerging production reliability degradation |

The Asset-Wise Availability Losses Report is most effective when reviewed alongside downtime, bottleneck, production analysis workflows to establish broader operational context.

