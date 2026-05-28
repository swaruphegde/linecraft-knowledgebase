# Quality Report

## Overview

The Quality Report provides a consolidated operational view of production quality, equipment effectiveness, rejection concentration and manufacturing consistency across the production line. It is designed to help production and quality teams quickly evaluate quality degradation patterns, identify operational instability and prioritize corrective actions with minimal interpretation overhead.

> _This report is intended for production managers, quality engineers and operational leaders working under live manufacturing conditions, where rapid interpretation and operational clarity are critical._

## Operational purpose

The Quality Report helps teams:

* evaluate overall production quality performance
* identify machines contributing most significantly to bad part generation
* monitor OEE degradation trends over time
* understand quality instability patterns across production
* prioritize corrective action using rejection concentration analysis
* improve production consistency and manufacturing reliability

## Report walkthrough

### Report availability

The Maintenance Report is available under the Reports module as a dedicated scheduled report template.

### Report generation

The report can be configured to generate automatically at predefined intervals for recurring maintenance reviews and operational monitoring workflows.

{% hint style="warning" %}
The Maintenance Report currently supports scheduled generation only and does not support on-demand report generation.
{% endhint %}

### Report KPIs

<figure><img src="../../.gitbook/assets/image (210).png" alt=""><figcaption></figcaption></figure>

The report surfaces operational and maintenance-critical KPIs that help teams evaluate equipment effectiveness, production reliability and operational continuity.

<details>

<summary>Understanding KPIs</summary>

#### Total target production

Represents the planned production target for the selected reporting duration.

> _This KPI helps teams evaluate whether operational output expectations are aligned with actual production performance_

Large deviations between target and actual production may indicate:

* downtime concentration
* throughput instability
* production interruptions
* equipment reliability degradation

#### Total actual production

Displays the total number of parts actually produced during the reporting duration.

This KPI helps validate:

* production continuity
* manufacturing stability
* operational throughput
* execution efficiency

> _Lower-than-expected actual production may indicate emerging operational bottlenecks or maintenance-related production loss._

#### Average OEE

Represents the average Overall Equipment Effectiveness across the reporting duration.

This KPI combines:

* availability
* performance
* quality

to provide a consolidated operational effectiveness indicator.

> _Declining OEE may indicate rising downtime, throughput degradation or operational inefficiency_

#### Average availability

Displays the average operational availability of the production line during the reporting duration

This KPI helps teams evaluate:

* uptime consistency
* downtime impact
* asset reliability
* maintenance effectiveness

> _Lower availability values may indicate recurring operational interruptions or unstable equipment behavior_

#### Average performance

Represents the average production performance efficiency during active manufacturing conditions.

This KPI helps identify:

* throughput degradation
* cycle-time instability
* production slowdowns
* operational imbalance

> _Declining performance values may indicate bottlenecks, micro-stoppages or equipment-related inefficiencies._

#### Average quality

Displays the average production quality performance during the reporting duration.

This KPI helps teams monitor:

* rejection exposure
* process stability
* production consistency
* operational quality degradation

> _Declining quality may indicate unstable operating conditions or recurring process abnormalities._



</details>

### Report sections

{% stepper %}
{% step %}
### OEE time series (End of line)

<figure><img src="../../.gitbook/assets/image (211).png" alt=""><figcaption></figcaption></figure>

Provides a time-series operational view of equipment effectiveness and production efficiency trends.

> _Time-series visibility is essential for understanding how operational effectiveness evolves over time rather than relying only on static averages._
{% endstep %}

{% step %}
### Overall production



<figure><img src="../../.gitbook/assets/image (212).png" alt=""><figcaption></figcaption></figure>

Provides consolidated production visibility comparing planned versus actual manufacturing behavior.

> _Production comparison visibility is essential for understanding whether output recovery behavior is masking deeper operational instability._
{% endstep %}

{% step %}
### Quality summary

<figure><img src="../../.gitbook/assets/image (215).png" alt=""><figcaption></figcaption></figure>

Provides a consolidated operational summary of production quality performance during the reporting duration.

> _Quality summary visibility is essential for understanding whether production output is being achieved sustainably without hidden quality degradation._
{% endstep %}

{% step %}
### On-shift bad parts pareto

<figure><img src="../../.gitbook/assets/image (216).png" alt=""><figcaption></figcaption></figure>

Provides a pareto-based operational analysis of machines contributing most significantly to bad part generation during planned production windows.

> _Machine-level rejection visibility is essential for understanding where quality degradation originates rather than only observing downstream rejection totals._
{% endstep %}
{% endstepper %}

## Operational interpretation guidelines

| Operational signal                            | What it may indicate                    |
| --------------------------------------------- | --------------------------------------- |
| Rising bad parts during stable throughput     | Hidden process instability              |
| Increasing rework dependency                  | Declining manufacturing consistency     |
| Declining OEE with stable availability        | Quality or performance degradation      |
| Concentrated bad parts on specific machines   | Localized equipment instability         |
| High off-shift bad parts                      | Reactive production quality degradation |
| Recurring machine presence in pareto analysis | Chronic operational abnormality         |
| Declining average quality trend               | Emerging process drift or instability   |

The Quality Report is most effective when reviewed alongside downtime, bottleneck, production analysis workflows to establish broader operational context.

