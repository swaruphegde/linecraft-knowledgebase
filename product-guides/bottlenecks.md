---
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
---

# 🛑 Bottlenecks

## Overview

<figure><img src="../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

The Bottlenecks module helps manufacturing teams identify the assets, cells, processes, and operational conditions that restrict overall line throughput.

Production lines rarely lose performance because of a single catastrophic failure. More often, throughput is constrained by subtle inefficiencies that are difficult to detect through traditional manufacturing methods.

The Bottlenecks module analyzes production behavior to uncover these hidden constraints, helping teams understand not only where throughput is being lost, but also why the loss is occurring and how it impacts the rest of the line.

Typical use cases include:

* Identifying throughput constraints
* Understanding production instability
* Investigating recurring wait conditions
* Analyzing synchronization losses
* Prioritizing improvement opportunities
* Validating the impact of bottleneck assets
* Recovering hidden production capacity



<details>

<summary>What are bottlenecks?</summary>

### Introduction to Bottlenecks in PSS

Imagine you are managing a Cylinder Head Subassembly Line. You walk the factory floor, and everything seems to be running smoothly - the machines are moving, the lights are green and parts are rolling off the conveyor. But when you check the daily reports, your total throughput isn't hitting the expected target.

Where is the lost time going?

In Linecraft's Productivity Synthesis System (PSS), a bottleneck isn't just a broken machine with a blaring siren. It is often an invisible mismatch in timing - any asset or cycle that secretly limits your overall line throughput. To find it, PSS acts as a detective, analyzing the temporal behavior of your entire line to find hidden inefficiencies and opportunities to resolve them.&#x20;

***

#### What is a bottleneck?

<figure><img src="../.gitbook/assets/image (167).png" alt=""><figcaption></figcaption></figure>

In the context of PSS, a bottleneck is any asset, cell, process, cycle or state that limits your overall throughput. While the physical line might seem to be running smoothly, microscopic delays, mismatched timings and wait states cascade through the system, ultimately dictating the maximum speed of your entire production.

_Example of a bottleneck: An asset becomes a bottleneck when it makes both its upstream and downstream assets wait for it_

***

#### Why managing bottlenecks matters

An unmanaged bottleneck does more than just slow down a single machine. It causes upstream machines to become blocked (unable to pass parts forward) and downstream machines to become starved (idling while waiting for parts).&#x20;

By identifying and resolving these hidden constraints, you can synchronize the entire line, unlocking hidden capacity without needing to add new hardware.

***

#### How PSS identifies bottlenecks

The PSS does not just look for broken machines; it analyzes the temporal behavior of your entire line to find inefficiencies. The module highlights bottlenecks using three primary indicators:

* Critical Cycles: The system analyzes the "minimum" time requirements for all cycles and identifies the "critical" cycles. These are the cycles with the highest minimum timing, meaning they are the baseline steps that fundamentally limit your total throughput.
* Outlier Nodes: The PSS flags nodes that consistently perform outside of defined conditions. A node is considered an outlier if it takes the most time to perform its states without interactions, or if it is constantly unavailable due to being dependent on another asset.
* Wait States and Synchronization Loss: Bottlenecks frequently occur when assets fall out of rhythm. The system actively identifies "wait states" (when an asset is delayed while waiting for another asset) and detects losses of synchronization between interlinked machines.

Our bottlenecks algorithm abstracts away internal asset efficiency and wait times and aggregates serial and parallel paths within a cell

Once the PSS identifies these critical cycles and outlier nodes, it doesn't leave you guessing. The system provides opportunities designed to synchronize operations between assets.

</details>

## Why Bottleneck Management Matters

An unmanaged bottleneck affects more than the constrained machine itself. As bottlenecks develop, they exponentially introduce losses throughout the production system:

{% stepper %}
{% step %}
### Upstream blocking

Machines are unable to transfer completed work and accumulate unnecessary waiting time
{% endstep %}

{% step %}
### Downstream starvation

Machines remain idle while waiting for material from constrained processes or machines
{% endstep %}

{% step %}
### JPH reduction

The maximum production capacity of the line becomes limited by the bottleneck entity.
{% endstep %}

{% step %}
### Production instability

Variability increases as machines repeatedly transition between operating and waiting conditions.
{% endstep %}
{% endstepper %}

> _By identifying and resolving bottlenecks, organizations can improve throughput, stabalize production and unlock hidden capacities without additional capital investment._

## Understanding Bottleneck Impact

Every bottleneck identified by PSS is ranked according to its operational impact on availability, performance and stability of your line. Impact represents the severity of the bottleneck and quantifies how significantly it influences production performance.

Impact is further categorized into:

{% stepper %}
{% step %}
### Availability impact

Losses caused by machine unavailability and production interruptions
{% endstep %}

{% step %}
### Performance impact

Losses caused by reduced operating speed or extened cycle execution
{% endstep %}

{% step %}
### Stability impact

Losses caused by operational variability, synchronization issues, and inconsistent production behavior.
{% endstep %}
{% endstepper %}

> _This classification helps teams understand not only where throughput is being lost, but also the primary mechanism responsible for the loss._

## Bottleneck Summary

<figure><img src="../.gitbook/assets/image (243).png" alt=""><figcaption></figcaption></figure>

The Bottlenecks module provides a ranked view of the cells and machines that most significantly constrain production.

For each bottleneck entity, users can review:

* Bottleneck severity
* JPH loss
* Bottleneck hours
* Impact on availability, performance and stability

> _This serves as the starting point for identifying the highest-value improvement opportunities within the production system._

## Bottleneck Visualization

<figure><img src="../.gitbook/assets/image (244).png" alt=""><figcaption></figcaption></figure>

Understanding a bottleneck requires more than identifying the constrained asset.

The Bottleneck Visualization illustrates how bottlenecks affect the surrounding production system by displaying:

* Wait directions
* Relative wait durations
* Asset dependencies
* Bottleneck propagation across the line

> _Entities identified as bottlenecks are visually highlighted, allowing users to quickly understand how a localized constraint influences broader production behavior._

## Bottleneck Timeline

<figure><img src="../.gitbook/assets/image (245).png" alt=""><figcaption></figcaption></figure>

Assets are not permanently constrained. A machine may operate normally during one period and become a bottleneck during another.

The Bottleneck Timeline highlights the specific intervals during which an asset impacts line performance.

Users can investigate:

* Availability-related bottlenecks
* Performance-related bottlenecks
* Stability-related bottlenecks

> _Timeline visualization helps teams understand when bottlenecks occur and how frequently they affect production._

## Bottleneck Verification

<figure><img src="../.gitbook/assets/image (246).png" alt=""><figcaption></figcaption></figure>

Identifying a bottleneck is only the first step.

Verification enables users to understand the underlying reasons an asset became a bottleneck during a specific production interval.

For a selected bottleneck and timeframe, users can analyze:

* Asset availability
* Self-performance
* Adjacent wait conditions
* Cycle behavior
* Downtime events
* Asset interactions

> _Verification provides a detailed operational view of the production environment at the moment the bottleneck occurred._

## Cycle and Downtime Analysis

<figure><img src="../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

Users can drill into cycle and downtime information to identify:

* Fault conditions
* Performance degradation
* Extended cycle execution
* Operational interruptions

## Best Practices

### Prioritize impact before frequency

The most frequently occurring issue is not always the most important. Focus first on bottlenecks with the highest throughput impact.

### Investigate wait conditions

Bottlenecks often reveal themselves through excessive waiting behavior in adjacent assets. Review blocking and starvation patterns alongside asset performance.

### Verify before acting

A bottleneck asset is often a symptom rather than the root cause. Use verification and interaction analysis to understand the full operational context before implementing corrective actions.

### Track improvement over time

After implementing changes, continue monitoring bottleneck behavior to validate whether throughput constraints have been successfully reduced.

## Operational Outcome

The Bottlenecks module transforms hidden production constraints into actionable operational intelligence.

By identifying throughput-limiting assets, quantifying their impact, visualizing their influence across the production system, and enabling detailed root-cause investigation, the module helps manufacturing teams improve synchronization, recover hidden capacity, and maximize overall line performance.
