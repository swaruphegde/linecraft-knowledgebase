# 🔥 Critical Machines

## Overview

In complex production environments, not all machines contribute equally to operational losses. Some assets consistently experience downtime, performance degradation, quality issues, or process instability that disproportionately affect line performance.

The Critical Machines module continuously evaluates production behavior and ranks cells and assets based on their operational impact, enabling teams to focus improvement efforts where they will deliver the greatest value.

Typical use cases include:

* Identifying high-impact production assets
* Prioritizing continuous improvement initiatives
* Investigating recurring operational losses
* Understanding equipment performance degradation
* Evaluating downtime patterns
* Monitoring quality-related losses
* Discovering performance improvement opportunities

## Why Critical Machines matter

Without a structured prioritization framework, teams may spend significant effort addressing visible issues while overlooking assets that contribute more substantially to production losses.

The Critical Machines module helps answer questions such as:

* Which machines are causing the greatest production losses?
* Which assets should improvement efforts focus on first?
* Are losses primarily caused by downtime, performance, or quality issues?
* Which machines exhibit the greatest operational instability?
* Where can throughput improvements be achieved most efficiently?

> _By ranking assets according to operational impact, the module helps teams focus on improvements that produce measurable business outcomes._

<details>

<summary>How We Identify Critical Machines</summary>

Rather than focusing on a single KPI, Ikshana evaluates machine behavior across multiple performance dimensions to determine which assets have the greatest influence on production efficiency. Assets can be ranked using:

#### Parts lost

Measures the production output lost as a result of operational inefficiencies.&#x20;

> _This the default prioritization method because it directly reflects the impact on manufacturing throughput._

#### Self-performance

Measures how efficiently an asset performs its own operations independent of external influences.

> _This view helps identify opportunities to improve cycle execution and machine-level efficiency._

#### Total performance

Measures overall production performance including interactions with surrounding assets.

> _This provides visibility into how machine behavior influences broader production flow._

#### Downtime frequency

Measures how often production interruptions occur.

> _High downtime frequency often indicates recurring operational issues that require investigation._

#### Downtime duration

Measures the total time lost to downtime events.

> _This helps identify assets responsible for significant availability losses._

#### Bad parts

Measures quality-related losses caused by rejected production.

> _This view helps prioritize quality improvement initiatives._

</details>

## Understanding Critical Cell Rankings

The module ranks production cells according to their contribution to operational losses. Each critical cell provides visibility into:

* Parts lost
* Availability
* Quality
* Self-performance

The ranking allows teams to quickly identify which production areas deserve more attention than others.

> _Provides a data-driven prioritization framework that helps focus improvement efforts on the cells with greatest business impact._

## Understanding Critical Asset Rankings

Each critical cell may contain one or more critical assets. Assets are ranked using the same performance dimensions as cells, allowing teams to identify specific machines responsible for operational losses.

> _Transforms cell-level performance issues into actionable machine-level investigations._

## Critical Machines Analysis

The Critical Machine module provides multiple analytical views that help teams understand the nature of operational losses

{% stepper %}
{% step %}
### Self-performance analysis

<figure><img src="../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

Self-performance evaluates how efficiently an asset executes its own production cycles and highlights cycle distribution, over-cycling events, lost production time and cycle variability

> _Helps identify machine-level inefficiencies that directly impact production output._
{% endstep %}

{% step %}
### Total performance analysis

<figure><img src="../.gitbook/assets/image (249).png" alt=""><figcaption></figcaption></figure>

Total performance evaluates production behavior while considering interactions with adjacent assets and provides visibility into end-to-end cycle behavior, interaction-driven delays and system-level performance losses

> _Helps distinguish machine inefficiencies from losses caused by broader production system interactions._
{% endstep %}

{% step %}
### Downtime analysis

<figure><img src="../.gitbook/assets/image (252).png" alt=""><figcaption></figcaption></figure>

Downtime analysis provides visibility into both the frequency and duration of downtime events. Users can investigate:

* Recurring fault conditions
* Availability losses
* Downtime causes
* Production interruptions

<figure><img src="../.gitbook/assets/image (255).png" alt=""><figcaption></figcaption></figure>

> _Supports_ _analysis of availability-related production losses._
{% endstep %}

{% step %}
### Quality analysis

<figure><img src="../.gitbook/assets/image (254).png" alt=""><figcaption></figcaption></figure>

Quality analysis evaluates rejected production and bad part generation over time and helps teams identify:

* Quality degradation trends
* High-loss production periods
* Assets contributing to rejection events

> _Supports targeted quality improvement initiatives and defect reduction efforts._
{% endstep %}
{% endstepper %}

## Best Practices

### Prioritize Parts Lost First

Parts Lost provides the clearest indication of business impact and is typically the most effective starting point for improvement initiatives.

### Investigate Trends Over Extended Periods

Operational behavior often varies significantly from day to day.

> _A two-week analysis period generally provides a more reliable representation of machine performance._

### Separate Symptoms from Causes

A critical machine is not always the root cause of a production issue. Use opportunity analysis and drilldowns to understand the underlying factors contributing to poor performance.

### Focus on High-Impact Opportunities

Improvement efforts should be prioritized based on expected operational impact rather than ease of implementation.

## Operational Outcome

The Critical Machines module transforms machine-level production data into a structured improvement roadmap.

By identifying the assets responsible for the greatest operational losses, ranking them according to business impact, and surfacing targeted improvement opportunities, the module helps manufacturing teams prioritize resources effectively, improve equipment performance, reduce production losses, and maximize overall line efficiency.
