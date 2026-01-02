---
description: >-
  Drilldown into which machines you need to monitor for criticality based on
  various parameters
---

# ✴️ Critical machines

## Overview

The critical assets feature ranks assets and the cells it belongs to by various parameters in terms of the worst performing cell first. You can access the critical assets module by clicking on the "Critical assets" card from the main menu.

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

Once inside, you will be displayed the following sections in the critical assets module:

1. List of critical cells and their assets and opportunities&#x20;
2. Self performance, Total performance, Downtime Frequencies, Downtime durations and Bad parts at a cell and asset level&#x20;

You can view critical cells and assets over a duration of time. To get the best results, a 2-week time range is recommended. This is also the default time range.&#x20;

<figure><img src="../.gitbook/assets/Critical Assets.png" alt=""><figcaption></figcaption></figure>

You can view critical assets by:

1. Parts lost (Default view)
2. Self performance
3. Total performance
4. Downtime frequency
5. Downtime duration
6. Bad parts

Each cell in the list of critical cells also displays the following information:

1. Name of the cell
2. Parts lost
3. Availability of the cell
4. Quality of the cell
5. Self performance of the cell

You can view the critical assets of a cell by clicking on the "View critical assets" button. The number in parenthesis represents the number of critical assets of the critical cell.

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

You can view the same information against a critical asset as well. You can click on the "View opportunities" button to view improvement opportunities for critical assets.

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

To the right of the page, you can see graphs that correspond to the selected options on the left hand side. When a particular sort by is selected, the corresponding graph will open up on the right side. However, you can toggle between the various graphs available.

Currently, we provide the following graphs:

#### Self performance

The self performance graph will show you a self cycle histogram for the selected cell across the selected time range. This graph also provides an insight into how many cycles were over cycling and how much time was lost due to it. This graph will open by default when APQ or self performance is used to sort the left side list.

<figure><img src="../.gitbook/assets/Critical Assets (1).png" alt=""><figcaption></figcaption></figure>

#### Total performance

The total performance graph will show you a total cycle histogram for the selected cell across the selected time range. This graph also provides an insight into how many cycles were over cycling and how much time was lost due to it. This graph will open by default when Total Performance is used to sort the left side list.

<figure><img src="../.gitbook/assets/Critical Assets-1.png" alt=""><figcaption></figcaption></figure>

#### Downtime frequency

The downtime frequency graph will show you a count of downtimes by causes for the selected cell across the selected time range. Selecting a bar on the graph will show you the corresponding cause description and you can move into aggregate downtime details from here. This graph will open by default when Downtime Frequency is used to sort the left side list.

<figure><img src="../.gitbook/assets/Critical Assets-2.png" alt=""><figcaption></figcaption></figure>

#### Downtime duration

The downtime duration graph will show you the duration of downtimes by causes for the selected cell across the selected time range. Selecting a bar on the graph will show you the corresponding cause description and you can move into aggregate downtime details from here. This graph will open by default when Downtime Duration is used to sort the left side list.

<figure><img src="../.gitbook/assets/Critical Assets-3.png" alt=""><figcaption></figcaption></figure>

#### Bad parts

The bad parts graph will show you a count of bad parts produced by day for the selected cell across the selected time range. This graph will open by default when Bad Parts is used to sort the left side list.

<figure><img src="../.gitbook/assets/Critical Assets-4.png" alt=""><figcaption></figcaption></figure>

## Critical machines' opportunities

Opportunities show the potential causes for critical assets on the line, and suggestions on how to fix them, with the objective of improving the efficiency of the line.

Opportunity cards describe the opportunities pertaining to the asset within the critical cell, the type of opportunity as well as the potential impact of addressing the opportunity. By default when a cell is selected, opportunities for the first asset will be shown.

<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

There are majorly three types of opportunity cards. These are:

#### Availability opportunities

Availability opportunities are down time opportunities that are caused by assets in a cell being down and unavailable to produce. These generally explain the root cause of critical cells but are not necessarily actionable.\
To drilldown into an availability opportunity, click on the card pertaining to availability opportunities for the selected asset. This will open a section that shows you all the hour intervals in which the selected asset faced a downtime along with the total number of downtimes in that hour and the total downtime duration.\
From here, you can select an interval and move into downtime details from the button available below. This will take you to the downtime details page for the selected hour.

<figure><img src="../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

#### Stability opportunities

There are two major types of stability opportunities. These are stuck states and stoppages.\
Stuck states are events in which an asset is cycling but gets interlocked in a suboptimal state. To drilldown into a stuck state opportunity, click on the card pertaining to this opportunity for the selected asset.&#x20;

This will open a section that shows you all the hour intervals in which the selected asset faced a stuck state along with the total number of stuck states in that hour and the total stuck state duration. From here, you can select an interval and move into stuck states from the button available below.

<figure><img src="../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

This will open the cycles page for the selected hour, with the stuck state/s highlighted.

<figure><img src="../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

Stoppages are events where an asset is down for 15 minutes or less. To drilldown into a stoppage opportunity, click on the card pertaining to this opportunity for the selected asset. This will open a section that shows you all the hour intervals in which the selected asset faced a stoppage along with the total number of stoppages in that hour and the total stoppage duration. From here, you can select an interval and move into stoppages from the button available below.

<figure><img src="../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

This will open the downtimes page for the selected hour, with the stoppage/s highlighted.

<figure><img src="../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

#### Performance opportunities

**Static delays**

Conditions in which the asset is waiting between operations, usually a delay that is added by the PLC programmers that can be eliminated. To drilldown into a Static Delays opportunity, click on the card pertaining to this opportunity for the selected asset. This will open a section that shows you the state histogram for all the states in the cycles of the selected asset along with each states num instances, modes, means and standard deviations.

<figure><img src="../.gitbook/assets/image (77).png" alt=""><figcaption></figcaption></figure>

From here, you can select a state and click on A/B comparison to compare a fast and slow cycle for the selected state.

<figure><img src="../.gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>

#### Variable cycle times

Cycles for the same asset are taking variable amounts of time. This indicates that the same operation can be performed more optimally (in the faster cycles). The fast and slow cycles can be compared to exploit this opportunity. To drilldown into a Static Delays opportunity, click on the card pertaining to this opportunity for the selected asset. This will open a section that shows you the state histogram for all the states in the cycles of the selected asset along with each states num instances, modes, means and standard deviations.

<figure><img src="../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>

From here, you can select a state and click on A/B comparison to compare a fast and slow cycle for the selected state.

<figure><img src="../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>

#### Interface delays

When assets are exchanging signals there are often delays and interlocks programmed into the system. These delays can be removed to improve the cycle time of both interfacing assets. To drilldown into an Interface delays opportunity, click on the card pertaining to this opportunity for the selected asset. This will open a section that shows you all the hour intervals in which the selected asset faced an Interface delay along with the start time and end time for the interval.

<figure><img src="../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>

From here, you can select an interval and move into interactions from the button available below. This will show you the interaction graph between the selected asset and the asset it is facing interaction delays with.

<figure><img src="../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>

#### Cyclical walls

It is sometimes observed that assets are simultaneously waiting on each other - either directly or through a chain of waits. This indicates that the assets are sub optimally programmed to work together. Typical root causes for this type of opportunity are :

* Sub-optimal priority logic for common zones
* Sub-optimal wait positions for automation

To drilldown into a Cyclical Waits opportunity, click on the card pertaining to this opportunity for the selected asset. This will open a section that shows you all the hour intervals in which the selected asset faced Cyclical Waits along with the start time and end time for the interval.

<figure><img src="../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure>

From here, you can select an interval and move into interactions from the button available below. This will show you the interaction graph between the selected asset and the asset it is facing cyclical waits with.

<figure><img src="../.gitbook/assets/image (75).png" alt=""><figcaption></figcaption></figure>

#### Interaction wait delays

There are sometimes delays programmed into the asset while interfacing with other assets. This means that even after the asset has been given the go-ahead to process a part / release a part, it still waits for a time before performing the action. These delays can be removed to improve the cycle time.
