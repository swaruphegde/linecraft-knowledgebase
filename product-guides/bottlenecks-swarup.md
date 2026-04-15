---
hidden: true
noIndex: true
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
---

# Bottlenecks - Swarup

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

## Overview

<figure><img src="../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

The bottlenecks module of Linecraft PSS enables you to understand the bottlenecks of your line, specifically, identify and analyze top bottleneck assets and why they are a bottleneck so that you can bring back your intended throughput without chasing invisible information.

<figure><img src="../.gitbook/assets/Bottleneck main menu (2) (1).gif" alt=""><figcaption></figcaption></figure>

It can be found from the main menu by choosing the 'Bottlenecks' option. Once you're inside the module, you can:

1. View top bottleneck cells and assets
2. View how these bottlenecks are impacting availability, performance and stability
3. Visualize how these bottlenecks are making other cells and assets wait
4. Verify the bottleneck - drilldown to view granular details of the bottleneck machine from the visualization
5. View opportunities to resolve the bottleneck's impact on availability, performance and stability

## Module walkthrough

### Bottleneck cells and assets

Bottleneck cells and their assets can be viewed in the summary section of the bottlenecks module. This section includes a list of all cells and their assets that are bottlenecks of your line, ranked based on their impact (most to least).

What is impact? It is the severity of the bottleneck entity in terms of availability, performance and stability. This is measured in %, taking into consideration the time the bottleneck makes adjacent cells or assets wait.

> _This view helps you identify which cells and machines are the top bottlenecks of your production line and what is their impact on availability, performance and stability. This acts as the first step in your journey to identify and resolve bottlenecks._

<figure><img src="../.gitbook/assets/Bottleneck list of critical cells.gif" alt=""><figcaption></figcaption></figure>

To view bottleneck cells:

{% stepper %}
{% step %}
#### Module selection

Select the 'Bottlenecks' module from the main menu
{% endstep %}

{% step %}
#### List of bottleneck cells

You will be displayed a list of top bottleneck cells, ranked by decreasing order of impact

Each bottleneck cells displays:

1. Name of the cell
2. JPH loss
3. Bottleneck hours
4. Total impact, which is further bifurcated in
   1. Availability impact
   2. Performance impact
   3. Stability impact
{% endstep %}
{% endstepper %}

Each bottleneck cell may have one or more bottleneck assets. To view bottleneck assets:

{% stepper %}
{% step %}
#### Click on 'View Bottleneck Assets'

View the bottleneck assets of a bottleneck cell by clicking the 'View bottleneck assets' button
{% endstep %}

{% step %}
#### List of bottleneck assets

You will then be displayed a list of top bottleneck assets of the cell, ranked by decreasing order of impact

Each bottleneck asset displays:

1. Name of the asset
2. JPH loss
3. Bottleneck hours
4. Total impact, which is further bifurcated in
   1. Availability impact
   2. Performance impact
   3. Stability impact
{% endstep %}
{% endstepper %}

### Bottleneck visualization

You can visualize how long bottlenecks are making cells or assets wait. The cells across the line show the direction of waits and their relative excess wait times. Cells that are bottlenecks will be highlighted red. There can be multiple bottlenecks in an interval.

> _By visualizing bottlenecks, you will be able to understand the exact wait times of a selected bottleneck. This step acts as the next step in drilling further into understanding your bottleneck entities._

### Bottleneck timeline

{% stepper %}
{% step %}
#### Causes timeline

The bottleneck causes timeline indicates all the intervals in which the selected cell is a bottleneck. The colors correspond to the cause of the cell being a bottleneck.
{% endstep %}

{% step %}
#### Timeline legend

View availability, performance and stability impacts on the timeline, differentiated by colors. You can always refer to the legend to identify which areas are being impacted on the bottleneck timeline
{% endstep %}
{% endstepper %}

### Bottleneck verification

Verifying a bottleneck helps in pointing out which assets are the problem in a specific interval and why

> _The bottleneck causes timeline helps you navigate different time zones during production and the bottlenecks that occurred during the timelines._
>
> _Verifying a bottleneck essentially allows you to view the cycles, interactions and downtime details of a machine while it was a bottleneck._

{% stepper %}
{% step %}
#### Click on the verify button

Clicking on verify from the timeline for a cell or an interval will show an asset diagram with the self-performance and availability of each asset as well as the adjacent waits for the selected cell and interval
{% endstep %}

{% step %}
#### View key KPIs and wait time of

Hover on an asset to view its availability, self performance and totals waits in the selected timeline
{% endstep %}

{% step %}
#### Drilldown to view further details

If you select 1 asset from the total waits diagram, you will see drilldowns for cycles and downtime details. This will take you to the cycles and downtime details for the selected asset in the selected interval.&#x20;

Analyzing the cycles and downtime details will help you identify which faults or cycle issues were the cause behind an entity becoming a bottleneck
{% endstep %}

{% step %}
#### Interaction drilldowns

If you select 2 or more assets from the total waits diagram, you will see a drilldown for interactions. This will take you to the interactions for the selected assets in the selected interval.
{% endstep %}
{% endstepper %}

## Bottleneck opportunities





