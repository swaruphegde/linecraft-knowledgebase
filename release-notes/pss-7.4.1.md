# PSS 7.4.1

{% hint style="info" %}
Last PSS Version: 7.4.0

New PSS Version: 7.4.1
{% endhint %}

Release 7.4.1 introduces improvements focused on operational visibility, fault analysis and insight interpretation. This release improves how cycle insights are communicated within the platform while also introducing a new export workflow for consolidated Level 1 (L1) and Level 2 (L2) fault analysis.

The goal of these updates is to reduce ambiguity during production investigations, improve visibility into hidden downtime conditions and enable advanced fault reporting.

## Cycle insights enhancements

<figure><img src="../.gitbook/assets/7.4.1 kb image 1.png" alt=""><figcaption></figcaption></figure>

Cycle insights are often used to investigate production instability, interrupted cycles and recurring throughput loss patterns. Previously, the distinction between self-cycle and total-cycle based insights was not always visually explicit, which could lead to interpretation inconsistencies during operational analysis.

This update improves clarity and context within the Cycle Insights experience

### What changed

{% stepper %}
{% step %}
### **Clear separation between self cycle and total cycle insights**

The screen now explicitly separates components related to:

* Self cycle based insights
* Total cycle based insights

This improves interpretability and reduces confusion while analyzing interrupted cycle behavior
{% endstep %}

{% step %}
### Informational context added for Top Problematic States

An informational tooltip has been added within the **Top Problematic States** section. This tooltip explains:

> _"The top problematic states displayed here are calculated only from interrupted cycles"_

This provides additional analytical context and helps users correctly interpret why certain states appear disproportionately during cycle analysis.
{% endstep %}

{% step %}
### Restricted Cycle Insights access for ignored assets

The **View Cycle Insights** action is now disabled for ignored assets within the **Dependent Machine State Delays** section.

This prevents non-actionable navigation paths and ensures cycle analysis workflows remain operationally relevant.
{% endstep %}
{% endstepper %}

## New excel export report - L1 and L2 faults

<details>

<summary>What are L1 and L2 faults?</summary>

Traditional fault analysis workflows primarily focus on hard-stop machine faults where assets transition from Auto mode to Manual mode. These events are highly visible, consistently logged and operationally understood.

However, many production losses originate from a different category of operational behavior:

* machines remaining in Auto mode
* cycles failing to complete
* intermittent waiting conditions
* hidden throughput restrictions
* operator interventions without formal fault states

These conditions are commonly referred to as **L2 faults**.

Unlike conventional machine stop conditions, L2 faults often:

* do not trigger mode drops
* are not logged as critical faults
* create hidden downtime
* reduce throughput without explicit failure visibility

This makes them significantly harder to investigate using standard fault workflows.

</details>

Release 7.4.1 introduces a new export report type - L1 and L2 Faults. This report is available under the new "Excel Export" report type while creating a new report

This new export allows users to generated a consolidated Excel report containing:

* hard faults (L1)
* latent operational issues (L2)
* alert occurrences
* auto mode drops
* manual mode switches
* event duration timelines

The objective is to provide a unified operational timeline that improves visibility into production-impacting conditions without requiring manual backend analysis.

### Export workflow

Users can now:

{% stepper %}
{% step %}
### Access export reports

Access the Export Report page by selecting the "Excel Export" option while creating a new report
{% endstep %}

{% step %}
### Download L1 and L2 faults

Select the L1 and L2 faults report type and choose:

* date range
* cells
* machines

Export an excel report containing chronological fault events
{% endstep %}
{% endstepper %}

This export improves investigation workflows by helping teams answer questions such as:

* What alerts occurred during production?
* When did Auto mode drop?
* Which faults remained active for extended durations?
* Which hidden conditions may have contributed to throughput loss?
* Where were repeated operator interventions occurring?

The report is designed to improve visibility into hidden downtime conditions while preserving compatibility with existing operational workflows.





