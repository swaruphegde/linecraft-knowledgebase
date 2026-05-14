# EOD Part tracing report

## Overview

The EOD Part Tracing Report provides a consolidated operational view of parameter deviations, affected part serial numbers, non-compliant production and asset-level production impact across the manufacturing line.&#x20;

It is designed to help production and quality teams quickly isolate operational abnormalities, investigate deviation patterns and prioritize corrective actions with minimal interpretation overhead.

The report aligns operational traceability with real manufacturing decision-making by emphasizing:

* parameter deviation visibility against expected values
* actual recorded values for operational comparison
* serial number traceability for affected parts
* asset-level contribution to non-compliant production
* consolidated production visibility across all monitored assets

> _This report is intended for production, quality and manufacturing engineering teams operating under live manufacturing conditions, where rapid interpretation and operational clarity are critical._

## Operational purpose

The EOD Part Tracing Report helps teams:

* identify which parameters are operating outside expected thresholds
* isolate affected part serial numbers for containment and investigation
* understand which assets are contributing most to non-compliant production
* monitor recurring deviation patterns across shifts and assets
* validate production impact caused by operational instability
* accelerate root-cause analysis workflows using traceability visibility

## Report walkthrough

<figure><img src="../../.gitbook/assets/EOD Part Tracing Report.gif" alt=""><figcaption></figcaption></figure>

### Report availability

The EOD Part Tracing Report is available under the **Reports** module as a dedicated report template. Users can generate the report in two ways:

{% stepper %}
{% step %}
### Schedule report generation

The report can be configured to generate automatically at predefined intervals for recurring operational reviews, quality monitoring workflows and end-of-day traceability analysis.
{% endstep %}

{% step %}
### On-demand report generation

Users can generate the report instantly whenever parameter deviation validation, serial number tracing or operational investigation is required.
{% endstep %}
{% endstepper %}

### Report KPIs

<figure><img src="../../.gitbook/assets/image (189).png" alt=""><figcaption></figcaption></figure>

The report surfaces operational and traceability-critical KPIs that help teams evaluate production quality, parameter stability and non-compliant production impact.

<details>

<summary>Understand report KPIs</summary>

#### Quality

Represents the overall production quality performance based on compliant versus non-compliant parts produced during the reporting duration.

> _This KPI helps teams evaluate whether production is maintaining acceptable operational and quality standards under current manufacturing conditions._

Declining quality values may indicate:

* recurring parameter instability
* process drift
* machine inconsistency
* upstream operational degradation
* increasing rejection risk

***

#### Non-compliant parts

Indicates the total number of parts associated with parameter deviations outside expected operational thresholds.

Higher values may indicate:

* unstable process conditions
* calibration inconsistencies
* recurring operational abnormalities
* elevated downstream quality exposure

> _This KPI is critical for understanding the production impact of operational deviations._

***

#### Total parts on the line

Represents the total number of parts currently tracked within the production line during the reporting period.

> _This metric provides visibility into active production load and overall line utilization._

Unexpected spikes or drops may indicate:

* throughput imbalance
* production accumulation
* downstream congestion
* operational interruptions

***

#### Parts completed

Displays the total number of parts that successfully completed the manufacturing process during the selected reporting duration.

This KPI helps validate:

* production continuity
* operational throughput
* completion efficiency
* manufacturing stability

> _Consistently lower completion counts may indicate bottlenecks or process instability._

***

#### Parts-in-progress

Represents the number of parts actively moving through the manufacturing process but not yet completed.

This helps teams monitor:

* work-in-progress accumulation
* line congestion
* production flow consistency
* process delays

> _Elevated parts-in-progress values may indicate emerging operational bottlenecks._

***

### Average time in line in planned production

Displays the average time spent in the line specifically during planned production windows.

This helps teams evaluate:

* planned production efficiency
* operational consistency during standard manufacturing conditions
* line stability during scheduled runs
* deviation between planned and reactive production behavior

> _Unexpected increases may indicate underlying throughput degradation even during controlled production conditions._

</details>

### Report sections

{% stepper %}
{% step %}
### Bad parts pareto

<figure><img src="../../.gitbook/assets/image (190).png" alt=""><figcaption></figcaption></figure>

Provides a ranked breakdown of non-compliant parts contributing most significantly to production quality loss.

This analysis helps teams:

* identify dominant quality issues
* prioritize corrective actions
* isolate recurring defect patterns
* focus investigation efforts on high-impact abnormalities

> _Pareto visibility is essential for understanding where the largest quality losses originate rather than treating all non-compliant production equally._
{% endstep %}

{% step %}
### Average time on line by shift

<figure><img src="../../.gitbook/assets/image (191).png" alt=""><figcaption></figcaption></figure>

Displays the average time parts spend on the line across different production shifts.

This helps identify:

* shift-wise operational inefficiency
* throughput variation
* operator-dependent production behavior
* recurring delay patterns

> _This view is particularly useful during operational consistency and escalation reviews._
{% endstep %}

{% step %}
### Average time on line by part type

<figure><img src="../../.gitbook/assets/image (195).png" alt=""><figcaption></figcaption></figure>

Breaks down average manufacturing duration across different part categories.

This helps teams understand:

* part-specific throughput behavior
* complexity-driven production delays
* operational impact of different SKUs
* variation in production cycle efficiency

> _Part-type visibility is critical for identifying which product variants contribute most to line occupancy and throughput degradation._
{% endstep %}

{% step %}
### Non-compliant parts summary

<figure><img src="../../.gitbook/assets/image (196).png" alt=""><figcaption></figcaption></figure>

Provides a consolidated operational summary of all non-compliant production identified during the reporting duration.

This includes visibility into:

* total non-compliant parts
* affected assets
* deviation concentration
* operational quality impact
* production exposure

> _This section helps teams quickly assess the scale and severity of production abnormalities._
{% endstep %}

{% step %}
### Non-compliant part details

<figure><img src="../../.gitbook/assets/image (198).png" alt=""><figcaption></figcaption></figure>

Provides detailed traceability visibility for each non-compliant part identified in the report.

This section supports:

* root-cause investigation
* containment workflows
* downstream traceability
* quality validation
* corrective action analysis

> _Detailed part-level visibility is essential for isolating operational abnormalities and accelerating manufacturing investigations._
{% endstep %}
{% endstepper %}

## Operational interpretation guidelines

When analyzing the EOD Part Tracing Report, focus on:&#x20;

| Operational signal                             | What it may indicate                     |
| ---------------------------------------------- | ---------------------------------------- |
| Repeated deviation on the same parameter       | Emerging process instability             |
| High concentration of affected serial numbers  | Widespread quality exposure              |
| Asset-specific deviation spikes                | Localized machine instability            |
| Rising non-compliant production                | Process degradation or calibration drift |
| Shift-wise deviation inconsistency             | Operational variability between shifts   |
| Multiple deviations tied to similar SR numbers | Upstream production abnormality          |

The EOD Part Tracing Report is most effective when reviewed alongside production, downtime, bottleneck workflows to establish broader operational context.

