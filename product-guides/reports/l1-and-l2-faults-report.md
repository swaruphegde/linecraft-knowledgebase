# L1 and L2 Faults Report

## Overview

The L1 (Level 1) and L2 (Level 2) Faults report provides a unified export of both critical machine stoppages and hidden operational disruptions in a single chronological Excel report.

This report helps manufacturing teams identify not only when machines stopped production, but also when machines remained operational while silently impacting throughput, cycle completion, and operator efficiency.

The report is available as an Excel export template under the `Excel export`  report type

> _This report is intended for production leaders, maintenance teams, and operational stakeholders operating in live manufacturing environments where rapid fault interpretation and operational clarity are critical._

## Operational purpose

The L1 and L2 Faults Report helps manufacturing teams:

* Identify critical machine stoppages and hidden operational disruptions
* Detect production-impacting conditions that do not trigger formal downtime
* Analyze fault occurrences across machines and time periods
* Understand when machines dropped out of Auto mode
* Investigate recurring operational instability
* Reduce hidden throughput loss caused by latent machine conditions
* Improve root cause investigation workflows

## Understanding L1 and L2 faults

{% tabs %}
{% tab title="L1 faults (hard faults)" %}
### L1 faults (hard faults)

_L1, or Level 1 faults are critical machine faults that force production interruption._

#### Operational behavior

The machine:

* drops from Auto mode
* switches to Manual mode
* stops production execution

#### Characteristics

L1 faults are:

* explicitly logged
* easy to detect
* already understood by operators

> _Examples:_
>
> 1. _Emergency stop triggered_
> 2. _Servo failure_
> 3. _Critical interlock failure_
> 4. _Safety condition violation_
{% endtab %}

{% tab title="L2 faults (soft or latent faults)" %}
### L2 faults (soft or latent faults)

_L2 faults are production-impacting conditions that do not formally stop the machine._

#### Operational behavior

The machine:

* remains in Auto mode
* continues appearing operational
* fails to complete production cycles correctly

#### Operational impact

These conditions:

* create bottlenecks
* reduce throughput
* generate hidden downtime
* cause operator confusion
* lead to repeated manual interventions

> _Examples_
>
> * _Timeout conditions_
> * _Material not present during cycle execution_
> * _Intermittent sensor instability_
> * _Non-blocking alerts_
> * _Machine waiting states_
{% endtab %}
{% endtabs %}

<details>

<summary>Why this report matters</summary>

Traditional fault reporting systems are designed to detect events that explicitly stop machines.

These events are typically:

* easy to classify
* logged as fault codes
* mapped in PLC logic
* visible to operators

{% hint style="danger" %}
However, many production losses occur without machines formally entering a stopped state which remain invisible in standard downtime analysis
{% endhint %}

The L1 and L2 Faults Report helps expose these hidden operational losses.

***

#### Why L2 faults are difficult to detect

Unlike traditional faults, L2 conditions often:

* do not trigger mode drops
* are not classified as failures
* are inconsistently logged
* remain invisible in existing downtime workflows

As a result:

* production appears active
* machines remain in Auto mode
* throughput degrades silently
* root cause analysis becomes manual and time-consuming

This creates operational blind spots where production inefficiencies exist without formal downtime visibility.

</details>

## Report walkthrough

### Accessing the report

The report is available as an Excel export template under the `Excel export`  report type

#### Access flow

{% stepper %}
{% step %}
### Open the reports module

Log in to Ikshana and select the reports module
{% endstep %}

{% step %}
### Access the L1/L2 faults report

Select the `Excel export`  option while creating a new report and select the `L1/L2 faults` option as the report type in the configuration page
{% endstep %}
{% endstepper %}

### Available report configurations

Users can configure the export by:

{% stepper %}
{% step %}
### Date range

Select the operational time window for analysis.
{% endstep %}

{% step %}
### Cells

Select one or more production cells.
{% endstep %}

{% step %}
### Machines

Select one or more machines within the chosen cells.

{% hint style="warning" %}
The machine selector becomes available only after cell selection.
{% endhint %}
{% endstep %}
{% endstepper %}

## Exported columns

The exported Excel file contains the following fields:

| Column                | Description                      |
| --------------------- | -------------------------------- |
| Machine name          | Asset or machine name            |
| Fault type            | Error or Availability            |
| Start time            | Fault start timestamp            |
| End time              | Fault end timestamp              |
| Fault code            | Fault identifier                 |
| Fault name            | Human-readable fault description |
| Fault count           | Number of occurrences            |
| Total duration (mins) | Fault duration in minutes        |

## Fault classification

The report currently categorizes events into two operational groups.

{% columns %}
{% column valign="middle" %}
Availability
{% endcolumn %}

{% column %}
Level 1 (L1) faults that affect availability by making the machines go down
{% endcolumn %}
{% endcolumns %}

{% columns %}
{% column valign="middle" %}
Error
{% endcolumn %}

{% column %}
Level 2 (L2) faults that keep the machine running and are left undected by traditional methods
{% endcolumn %}
{% endcolumns %}

## Key benefits

{% stepper %}
{% step %}
### Hidden downtime visibility

Makes previously invisible L2 operational disruptions visible and actionable.
{% endstep %}

{% step %}
### Reduced Manual Dependency

Eliminates dependency on Linecraft teams for backend fault extraction and analysis.
{% endstep %}

{% step %}
### Faster Investigation

Provides a unified machine event timeline for rapid operational analysis.
{% endstep %}

{% step %}
### Improved Operational Clarity

Helps teams understand both production stoppages and latent production disruption in a single view.
{% endstep %}

{% step %}
### Self-Service Fault Analysis

Allows teams to independently export and investigate machine instability without requiring custom scripts or backend support.
{% endstep %}
{% endstepper %}



