# Alert Insights Report

## Overview

The Alert Insights Report provides a consolidated operational view of alert activity, asset-level alert concentration and parameter-driven alert behavior across the manufacturing environment.&#x20;

It is designed to help production, maintenance and operational teams quickly identify recurring operational abnormalities, understand alert generation patterns and prioritize high-impact issues with minimal interpretation overhead.

> _This report is intended for operational stakeholders working under live manufacturing conditions, where rapid interpretation and operational clarity are critical._

## Operational purpose

The Alert Insights Report helps teams:

* identify assets generating excessive alert activity
* understand which parameters contribute most to alert generation
* prioritize high-impact alerts requiring immediate attention
* monitor recurring operational instability patterns
* identify potential process degradation trends
* improve responsiveness to operational abnormalities

## Report walkthrough

### Report availability

The Alert Insights Report is available under the Reports module as a dedicated report template. Users can generate the report in two ways:

{% stepper %}
{% step %}
### Schedule report generation

The report can be configured to generate automatically at predefined intervals for recurring operational reviews and alert monitoring workflows.
{% endstep %}

{% step %}
### On-demand report generation

Users can generate the report instantly whenever operational validation or alert investigation is required.
{% endstep %}
{% endstepper %}

### Report KPIs

<figure><img src="../../.gitbook/assets/image (201).png" alt=""><figcaption></figcaption></figure>

The report surfaces operational and alert-critical KPIs that help teams evaluate alert concentration, operational instability and issue prioritization.

<details>

<summary>Understand report KPIs</summary>

#### Total alerts triggered

Represents the total number of alerts generated during the selected reporting duration.

This KPI helps teams evaluate the overall volume of operational abnormalities detected across the manufacturing environment.

Higher values may indicate:

* increasing process instability
* abnormal operating conditions
* recurring equipment issues
* elevated operational sensitivity
* widespread production disturbances

> _A sudden spike in total alerts triggered may indicate emerging operational degradation requiring immediate investigation._

***

#### Total unique alerts triggered

Displays the number of distinct alert conditions triggered during the reporting period.

This KPI helps teams understand:

* diversity of operational abnormalities
* spread of process instability across parameters
* breadth of operational exposure
* variability in production behavior

> _Higher unique alert counts may indicate that instability is affecting multiple operational areas rather than isolated equipment or parameters._

***

#### Priority alerts triggered

Represents the total number of high-priority alerts generated during the reporting duration.

This KPI helps teams identify:

* operational conditions with elevated production risk
* critical process deviations
* severe instability patterns
* escalation-worthy events

> _Increasing priority alert volume may indicate rising operational risk, quality exposure or potential throughput impact._

</details>

## Report sections

{% stepper %}
{% step %}
### Machines with most triggered alerts

<figure><img src="../../.gitbook/assets/image (202).png" alt=""><figcaption></figcaption></figure>

Provides a ranked view of machines generating the highest number of alerts during the reporting period.

This section includes:

* machine name
* total triggered alerts

This analysis helps teams:

* identify unstable assets
* prioritize maintenance intervention
* isolate recurring operational abnormalities
* focus corrective action efforts on high-impact machines

> _Machine-level alert visibility is essential for understanding where operational degradation originates rather than only observing downstream effects._
{% endstep %}

{% step %}
### Parameters with most triggered alerts

<figure><img src="../../.gitbook/assets/image (203).png" alt=""><figcaption></figcaption></figure>

Displays the parameters responsible for the highest alert frequency across the selected reporting duration.

This section includes:

* parameter name
* total triggered alerts

This helps teams identify:

* recurring process instability
* threshold sensitivity issues
* calibration drift
* parameter-specific operational degradation

> _Frequent alerts on the same parameter may indicate persistent process abnormalities requiring deeper investigation._
{% endstep %}

{% step %}
### Top triggered non-priority alerts

<figure><img src="../../.gitbook/assets/image (207).png" alt=""><figcaption></figcaption></figure>

Provides visibility into the most frequently triggered non-priority alerts across the manufacturing environment.

This section includes:

* group name (alert name)
* parameter
* entity
* condition
* check every
* trigger count

This analysis helps teams:

* monitor recurring low-severity operational abnormalities
* identify repetitive nuisance conditions
* improve alert tuning strategies
* reduce operational alert fatigue

> _Although categorized as non-priority, recurring alert patterns may still indicate emerging operational inefficiencies._
{% endstep %}

{% step %}
### Top triggered priority alerts

<figure><img src="../../.gitbook/assets/image (205).png" alt=""><figcaption></figcaption></figure>

Highlights the most frequently triggered priority alerts requiring elevated operational attention.

This section includes:

* group name (alert name)
* parameter
* entity
* condition
* check every
* trigger count

This helps teams:

* prioritize critical operational issues
* accelerate escalation workflows
* reduce production risk
* focus response efforts on severe operational abnormalities

> _Priority alert visibility is essential for minimizing operational disruption and preventing downstream quality or throughput impact._
{% endstep %}

{% step %}
### All triggered alerts

<figure><img src="../../.gitbook/assets/image (206).png" alt=""><figcaption></figcaption></figure>

Provides a consolidated operational view of all alerts triggered during the selected reporting duration.

This section includes:

* group name (alert name)
* parameter
* entity
* condition
* check every
* trigger count

This helps teams:

* perform detailed operational investigations
* understand overall alert distribution
* validate recurring abnormality patterns
* correlate alert activity with production behavior
* establish broader operational context

> _Comprehensive alert visibility is critical for identifying systemic operational instability and improving manufacturing responsiveness._
{% endstep %}
{% endstepper %}

## Operational interpretation guidelines

When analyzing the Alert Insights Report, focus on:

| Operational signal                                | What it may indicate                   |
| ------------------------------------------------- | -------------------------------------- |
| Repeated alerts on the same asset                 | Localized machine instability          |
| Frequent alerts on the same parameter             | Process drift or threshold instability |
| Sudden increase in total alerts triggered         | Emerging operational degradation       |
| High concentration of alerts from specific assets | Maintenance or calibration requirement |
| Recurring high-impact alerts                      | Elevated production or quality risk    |
| Consistent alert spikes across shifts             | Systemic operational inconsistency     |

The Alert Insights Report is most effective when reviewed alongside downtime, bottleneck and production analysis workflows to establish broader operational context.
