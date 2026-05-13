# Production Report

## Overview

The Production Report provides a consolidated operational view of line output, quality, rejection trends and throughput performances across shifts and part types. It is designed to help production managers quickly evaluate production health, identify instability patterns and prioritize corrective actions with minimal interpretation overhead.

The Production Report aligns operational metrics with real manufacturing decision-making by emphasizing:

* production quality alongside quantity
* visibility into planned vs unplanned production
* rejection impact at both EOL and line-level
* througput consistency through JPH monitoring
* machine-level contribution to part loss

> _This report is intended for production leaders operating under live manufacturing conditions, where rapid interpreation and operation clarity are critical_

## Operational purpose

The Production Report helps teams:

* evaluate whether production targets are being achieved sustainably
* identify hidden production losses during unplanned runs
* compare performance across shifts and part categories
* isolate quality degradation through rejection tracking
* understand which machines are contributing most to production loss
* monitor throughput consistency using JPH metrics

## Report walkthrough

### Report availability

The Production Report is available under the **Reports** module as a dedicated report template. Users can generate the report in two ways:

{% stepper %}
{% step %}
### Schedule report generation

The report can be configured to generate automatically at predefined intervals for recurring operational reviews and production monitoring workflows.
{% endstep %}

{% step %}
### On-demand report generation

Users can generate the report instantly whenever production validation or shift-level investigation is required.
{% endstep %}
{% endstepper %}

### Report KPIs

The report surfaces production-critical KPIs that help teams evaluate both throughput and quality performance.

<figure><img src="../../.gitbook/assets/Frame 37947.png" alt=""><figcaption></figcaption></figure>

<details>

<summary>Understand report KPIs</summary>

#### Overall production

Represents the total number of parts produced during the selected reporting duration.

> _This metric establishes the primary production baseline and helps validate whether the line is operating at expected capacity._

#### EOL on-shift good parts

Indicates the number of successfully completed parts at the End-of-Line stage during active shift production.

> _A stable value typically reflects healthy production continuity and acceptable process stability._

#### EOL on-shift bad parts

Represents the number of rejected or failed parts identified at the End-of-Line stage during planned shift production.

> _Higher values may indicate:_
>
> * _process instability_
> * _quality degradation_
> * _upstream machine inconsistencies_
> * _operator-related variation_
> * _calibration drift_

#### Total unplanned production (EOL)

Tracks all production occurring outside planned production schedules at the End-of-Line stage.

> _Frequent unplanned production may indicate persistent throughput instability or target recovery dependence._

#### Unplanned good parts (EOL)

Represents successfully produced parts during unplanned production periods.

> _This helps evaluate whether recovery production maintains acceptable quality standards._

#### Unplanned bad parts (EOL)

Represents rejected or failed parts generated during unplanned production periods.

> _Elevated values may suggest that reactive production conditions are introducing additional instability or quality risk._

#### Total line-level rejections

Displays the total rejected parts identified across the entire production line.

> _This metric helps quantify cumulative quality loss and production inefficiency._

#### On-shift line-level rejections

Represents rejection counts specifically during planned shift operations.

> _This helps teams correlate rejection behavior with:_
>
> * _operator shifts_
> * _production schedules_
> * _machine loading conditions_
> * _process transitions_

#### Unplanned line-level rejections

Tracks rejection counts occurring during unplanned production windows.

> _This metric is particularly useful for evaluating the operational effectiveness of recovery production activities._

#### On-shift JPH

Displays the line’s Jobs Per Hour performance during active shift production.

> _Unexpected throughput drops may indicate bottlenecks, micro-stoppages, or production imbalance conditions._

</details>

### Production data analysis

The report provides detailed production segmentation across multiple operational dimensions.

{% stepper %}
{% step %}
### Production by shift

<figure><img src="../../.gitbook/assets/Frame 37953.png" alt=""><figcaption></figcaption></figure>

Enables comparative analysis between shifts to identify:

* throughput variation
* quality inconsistencies
* operational inefficiencies
* recurring shift-specific instability

> _This view is particularly useful during escalation reviews and continuous improvement analysis._
{% endstep %}

{% step %}
### Production by part type

<figure><img src="../../.gitbook/assets/Frame 37954.png" alt=""><figcaption></figcaption></figure>

Breaks down production performance by manufactured part category.

> _This helps teams understand:_
>
> * _part-specific production behavior_
> * _quality sensitivity across SKUs_
> * _throughput impact of complex part variants_
> * _rejection concentration by product type_
{% endstep %}

{% step %}
### On-shift production trends

<figure><img src="../../.gitbook/assets/Frame 37952.png" alt=""><figcaption></figcaption></figure>

Provides visibility into production behavior during planned manufacturing windows.

> _This helps validate whether production targets are being achieved under standard operating conditions._
{% endstep %}
{% endstepper %}

### Critical machine analysis

<figure><img src="../../.gitbook/assets/Frame 37955.png" alt=""><figcaption></figcaption></figure>

The report identifies the five machines contributing most significantly to part loss.

This analysis helps production teams:

* prioritize maintenance intervention
* isolate recurring bottlenecks
* identify unstable assets
* reduce hidden throughput loss
* focus continuous improvement efforts

> _Machine-level visibility is essential for understanding where production degradation originates rather than only observing downstream effects._

<figure><img src="../../.gitbook/assets/Frame 37956 (1).png" alt=""><figcaption></figcaption></figure>

### Notifications

Users receive notifications whenever:

* a scheduled production report is generated
* an on-demand production report completes generation

This ensures production stakeholders can immediately review updated operational insights without manually monitoring report execution status.

### Operational interpretation guidelines

When analyzing the Production Report, focus on:

<table><thead><tr><th width="352">Operational signal</th><th>What it may indicate</th></tr></thead><tbody><tr><td>Rising bad parts with stable throughput</td><td>Hidden quality degradation</td></tr><tr><td>High unplanned production</td><td>Reactive target recovery behavior</td></tr><tr><td>Increasing line-level rejections</td><td>Process instability or machine drift</td></tr><tr><td>Declining JPH</td><td>Emerging bottlenecks or micro-stoppages</td></tr><tr><td>Machine concentration in part loss</td><td>Localized asset instability</td></tr><tr><td>Shift-to-shift production variance</td><td>Operational inconsistency</td></tr></tbody></table>

The Production Report is most effective when reviewed alongside downtime, bottleneck, and rejection analysis workflows to establish broader operational context.
