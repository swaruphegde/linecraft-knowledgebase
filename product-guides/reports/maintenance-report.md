# Maintenance Report

## Overview

The Maintenance Report provides a consolidated operational view of production performance, equipment effectiveness, availability loss and recurring downtime behavior across the manufacturing line. It is designed to help production and maintenance teams quickly evaluate operational stability, identify reliability degradation patterns and prioritize maintenance interventions with minimal interpretation overhead.

> _This report is intended for production managers, maintenance teams and operational leaders working under live manufacturing conditions, where rapid interpretation and operational clarity are critical._

## Operational purpose

The Maintenance Report helps teams:

* evaluate overall production effectiveness and operational stability
* identify assets contributing most significantly to downtime
* understand recurring fault and downtime patterns
* monitor OEE degradation trends over time
* prioritize maintenance intervention based on operational impact
* improve equipment reliability and production continuity

## Report walkthrough

### Report availability

The Maintenance Report is available under the Reports module as a dedicated scheduled report template.

### Report generation

The report can be configured to generate automatically at predefined intervals for recurring maintenance reviews and operational monitoring workflows.

{% hint style="warning" %}
The Maintenance Report currently supports scheduled generation only and does not support on-demand report generation.
{% endhint %}

### Report KPIs

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

Provides a time-series operational view of equipment effectiveness and production efficiency trends.

> _Time-series visibility is essential for understanding how operational effectiveness evolves over time rather than relying only on static averages._
{% endstep %}

{% step %}
### Overall production

Provides consolidated production visibility comparing planned versus actual manufacturing behavior.

> _Production comparison visibility is essential for understanding whether output recovery behavior is masking deeper operational instability._
{% endstep %}

{% step %}
### Top 5 downtime assets

Provides a ranked operational view of the five assets contributing most significantly to downtime during the reporting duration.

> _Machine-level downtime visibility is essential for understanding where operational reliability degradation originates rather than only observing downstream production impact._
{% endstep %}

{% step %}
### Top 5 downtime causes

Provides a ranked operational view of the most significant downtime causes affecting production continuity.

> _Downtime cause visibility is essential for strengthening long-term operational stability._
{% endstep %}

{% step %}
### Downtime pareto analysis

Displays a Pareto visualization of downtime contribution using:

* downtime occurrence count
* downtime ranking
* ranked fault descriptions

along with a supporting operational table that represents faults, ranked by their occurrence

> _Pareto visibility is critical for prioritizing maintenance efforts using operational impact rather than treating all downtime conditions equally._
{% endstep %}
{% endstepper %}

## Operational interpretation guidelines

| Operational signal                             | What it may indicate                     |
| ---------------------------------------------- | ---------------------------------------- |
| Declining OEE trend                            | Emerging operational degradation         |
| High downtime concentration on specific assets | Localized equipment instability          |
| Rising off-shift bad parts                     | Reactive production quality degradation  |
| Repeated downtime causes                       | Chronic maintenance or reliability issue |
| Declining availability with stable performance | Frequent interruptions or stoppages      |
| High downtime count with short durations       | Persistent micro-stoppages               |
| Low downtime count with long durations         | Sever operational failure events         |

The Maintenance Report is most effective when reviewed alongside downtime, bottleneck, production and rejection analysis workflows to establish broader operational context.
