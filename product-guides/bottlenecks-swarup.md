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

### Introduction to Bottlenecks in PSS

Imagine you are managing a Cylinder Head Subassembly Line. You walk the factory floor, and everything seems to be running smoothly - the machines are moving, the lights are green and parts are rolling off the conveyor. But when you check the daily reports, your total throughput isn't hitting the expected target.

Where is the lost time going?

In Linecraft's Productivity Synthesis System (PSS), a bottleneck isn't just a broken machine with a blaring siren. It is often an invisible mismatch in timing - any asset or cycle that secretly limits your overall line throughput. To find it, PSS acts as a detective, analyzing the temporal behavior of your entire line to find hidden inefficiencies and opportunities to resolve them.&#x20;

#### What is a bottleneck?

In the context of PSS, a bottleneck is any asset that limits your overall throughput. While the physical line might seem to be running smoothly, microscopic delays, mismatched timings and wait states cascade through the system, ultimately dictating the maximum speed of your entire production.

#### Why managing bottlenecks matters

An unmanaged bottleneck does more than just slow down a single machine. It causes upstream machines to become blocked (unable to pass parts forward) and downstream machines to become starved (idling while waiting for parts).&#x20;

By identifying and resolving these hidden constraints, you can synchronize the entire line, unlocking hidden capacity without needing to add new hardware.

#### How PSS identifies bottlenecks

The PSS does not just look for broken machines; it analyzes the temporal behavior of your entire line to find inefficiencies. The module highlights bottlenecks using three primary indicators:

* Critical Cycles: The system analyzes the "minimum" time requirements for all cycles and identifies the "critical" cycles. These are the cycles with the highest minimum timing, meaning they are the baseline steps that fundamentally limit your total throughput.
* Outlier Nodes: The PSS flags nodes that consistently perform outside of defined conditions. A node is considered an outlier if it takes the most time to perform its states without interactions, or if it is constantly unavailable due to being dependent on another asset.
* Wait States and Synchronization Loss: Bottlenecks frequently occur when assets fall out of rhythm. The system actively identifies "wait states" (when an asset is delayed while waiting for another asset) and detects losses of synchronization between interlinked machines.

Once the PSS identifies these critical cycles and outlier nodes, it doesn't leave you guessing. The system provides opportunities designed to synchronize operations between assets.

### The bottleneck module

