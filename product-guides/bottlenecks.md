---
description: >-
  A deep dive into the various line level and asset level opportunities on your
  line
---

# ❗ Bottlenecks

## Overview

A cell or operation becomes a bottleneck when it throttles the line flow. This happens when both downstream and upstream cells wait for the cell in question.

<figure><img src="../.gitbook/assets/image (47) (1).png" alt=""><figcaption></figcaption></figure>

The Linecraft bottlenecks algorithm abstracts away internal asset efficiency and wait times and aggregates serial and parallel paths within a cell.

<figure><img src="../.gitbook/assets/image (48) (1).png" alt=""><figcaption></figcaption></figure>

You can access the bottlenecks module from the main menu by clicking on the “Bottlenecks” card

<figure><img src="../.gitbook/assets/image (49) (1).png" alt=""><figcaption></figcaption></figure>

The bottlenecks page consists of bottleneck cells’ summary, bottleneck visualization and bottleneck causes’ timeline.

#### Bottleneck cells' summary

The bottlenecks cell summary section shows you a list of all the cells that are bottlenecks on your line, ranked from most impact to least impact. Impact is the severity or magnitude of bottleneck in terms of the percentage of time it makes the adjacent cells wait. Bottleneck cells can be viewed at different intervals. To view the best results for bottlenecks, select 2 weeks interval from the calendar dropdown. This is the default date range as well.

Each cell in this list provides you the following information:

1. Name of the cell
2. JPH loss when the cell was a bottleneck
3. Bottleneck hours: Time (in hours) when the cell was a bottleneck
4. Bottleneck impact: Impact on availability, performance and quality during bottleneck hours of the cell

<figure><img src="../.gitbook/assets/image (50) (1).png" alt=""><figcaption></figcaption></figure>

Each bottleneck cell may have one or more bottleneck assets. To view these assets the their details, you can click on the “View bottleneck assets” button on the list of bottleneck cells. The number in parentheses highlights the number of bottleneck assets of the bottleneck cell.

<figure><img src="../.gitbook/assets/image (51) (1).png" alt=""><figcaption></figcaption></figure>

The view opportunities button will show you the opportunities to reduce the impact of the selected bottleneck cell or asset.&#x20;

#### Bottleneck visualization

Bottleneck visualization shows how long the bottleneck is making the other cells wait. The cells across the line show the direction of waits and their relative excess wait times. Cells that are bottlenecks will be highlighted red. There can be multiple bottlenecks in an interval.

<figure><img src="../.gitbook/assets/image (52) (1).png" alt=""><figcaption></figcaption></figure>

#### Bottleneck causes timeline

The timeline indicates all the intervals in which the selected cell is a bottleneck. The colors correspond to the cause of the cell being a bottleneck.

<figure><img src="../.gitbook/assets/image (53) (1).png" alt=""><figcaption></figcaption></figure>

The legend to understand the colors denoted in the timeline are as follows:

<figure><img src="../.gitbook/assets/image (54) (1).png" alt=""><figcaption></figcaption></figure>

#### Bottleneck verification

Clicking on verify from the timeline for a cell or an interval will show an asset diagram with the self-performance and availability of each asset as well as the adjacent waits for the selected cell and interval. This helps point out which asset or assets are the problem in that interval and why.

<figure><img src="../.gitbook/assets/image (55) (1).png" alt=""><figcaption></figcaption></figure>

Hover on an asset to view its availability, self performance and totals waits.

<figure><img src="../.gitbook/assets/image (56) (1).png" alt=""><figcaption></figcaption></figure>

If you select 1 asset from the total waits diagram, you will see drilldowns for cycles and downtime details. These will take you to the cycles and downtime details for the selected asset in the selected interval.

<figure><img src="../.gitbook/assets/image (57) (1).png" alt=""><figcaption></figcaption></figure>

If you select 2 or more assets from the total waits diagram, you will see a drilldown for interactions. This will take you to the interactions for the selected assets in the selected interval.

<figure><img src="../.gitbook/assets/image (58) (1).png" alt=""><figcaption></figcaption></figure>

## Bottleneck opportunities

Opportunities show the potential causes for bottlenecks on the line, and suggestions on how to fix them, with the objective of improving the efficiency of the line.

<figure><img src="../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

Opportunity cards describe the opportunities pertaining to the asset within the bottleneck cell, the type of opportunity as well as the potential impact of addressing the opportunity. By default when a cell is selected, opportunities for the first asset will be shown.

There are majorly three types of opportunity cards. These are:

#### Availability opportunities

Availability opportunities are down time opportunities that are caused by assets in a cell being down and unavailable to produce. These generally explain the root cause of bottlenecks but are not necessarily actionable.\


To drilldown into an availability opportunity, click on the card pertaining to availability opportunities for the selected asset. This will open a section that shows you all the hour intervals in which the selected asset faced a downtime along with the total number of downtimes in that hour and the total downtime duration.

\
From here, you can select an interval and move into downtime details from the button available below. This will take you to the downtime details page for the selected hour.

<figure><img src="../.gitbook/assets/image (60).png" alt=""><figcaption></figcaption></figure>

#### Stability opportunities

There are two major types of stability opportunities. These are stuck states and stoppages.\
Stuck states are events in which an asset is cycling but gets interlocked in a suboptimal state.&#x20;

To drilldown into a stuck state opportunity, click on the card pertaining to this opportunity for the selected asset. This will open a section that shows you all the hour intervals in which the selected asset faced a stuck state along with the total number of stuck states in that hour and the total stuck state duration.&#x20;

From here, you can select an interval and move into stuck states from the button available below.

<figure><img src="../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

This will open the cycles page for the selected hour, with the stuck state/s highlighted.

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

Stoppages are events where an asset is down for 15 minutes or less. To drilldown into a stoppage opportunity, click on the card pertaining to this opportunity for the selected asset.&#x20;

This will open a section that shows you all the hour intervals in which the selected asset faced a stoppage along with the total number of stoppages in that hour and the total stoppage duration. From here, you can select an interval and move into stoppages from the button available below.

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

This will open the downtimes page for the selected hour, with the stoppage/s highlighted.

<figure><img src="../.gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

#### Performance opportunities

**Static delays**

Conditions in which the asset is waiting between operations, usually a delay that is added by the PLC programmers that can be eliminated. To drilldown into a Static Delays opportunity, click on the card pertaining to this opportunity for the selected asset. This will open a section that shows you the state histogram for all the states in the cycles of the selected asset along with each states num instances, modes, means and standard deviations.

<figure><img src="../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

From here, you can select a state and click on A/B comparison to compare a fast and slow cycle for the selected state.

<figure><img src="../.gitbook/assets/image (51).png" alt=""><figcaption></figcaption></figure>

#### Variable cycle times

Cycles for the same asset are taking variable amounts of time. This indicates that the same operation can be performed more optimally (in the faster cycles). The fast and slow cycles can be compared to exploit this opportunity. To drilldown into a Static Delays opportunity, click on the card pertaining to this opportunity for the selected asset. This will open a section that shows you the state histogram for all the states in the cycles of the selected asset along with each states num instances, modes, means and standard deviations.

<figure><img src="../.gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure>

From here, you can select a state and click on A/B comparison to compare a fast and slow cycle for the selected state.

<figure><img src="../.gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure>

#### Interface delays

When assets are exchanging signals there are often delays and interlocks programmed into the system. These delays can be removed to improve the cycle time of both interfacing assets. To drilldown into an Interface delays opportunity, click on the card pertaining to this opportunity for the selected asset. This will open a section that shows you all the hour intervals in which the selected asset faced an Interface delay along with the start time and end time for the interval.

<figure><img src="../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

From here, you can select an interval and move into interactions from the button available below. This will show you the interaction graph between the selected asset and the asset it is facing interaction delays with.

<figure><img src="../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

#### Cyclical walls

It is sometimes observed that assets are simultaneously waiting on each other - either directly or through a chain of waits. This indicates that the assets are sub optimally programmed to work together. Typical root causes for this type of opportunity are :

* Sub-optimal priority logic for common zones
* Sub-optimal wait positions for automation

To drilldown into a Cyclical Waits opportunity, click on the card pertaining to this opportunity for the selected asset. This will open a section that shows you all the hour intervals in which the selected asset faced Cyclical Waits along with the start time and end time for the interval.

<figure><img src="../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

From here, you can select an interval and move into interactions from the button available below. This will show you the interaction graph between the selected asset and the asset it is facing cyclical waits with.

<figure><img src="../.gitbook/assets/image (57).png" alt=""><figcaption></figcaption></figure>

#### Interaction wait delays

There are sometimes delays programmed into the asset while interfacing with other assets. This means that even after the asset has been given the go-ahead to process a part / release a part, it still waits for a time before performing the action. These delays can be removed to improve the cycle time.
