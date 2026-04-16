---
description: >-
  Identify and prioritize the assets that impact your production efficiency
  based on real-time performance metrics.
hidden: true
---

# Critical Machines

## Overview

The Critical Machines module ranks machines and production cells by performance, highlighting the most problematic areas first. This allows you to focus your attention where it matters most. You can access this feature by selecting the "Critical Machines" card from the main menu.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-15 160402.png" alt=""><figcaption></figcaption></figure>

#### Navigating the Module

Inside the module, the interface is divided into two primary areas:

1. A list of critical cells, their component assets, and identified improvement opportunities.&#x20;
2. Self performance, Total performance, Downtime Frequencies, Downtime durations and Bad parts at a cell and asset level&#x20;

**Recommended View:** While you can adjust the timeframe, a 2-week time range (the system default) is recommended to capture meaningful performance trends.

#### Sorting & Filtering

You can rank critical assets based on the following parameters to pinpoint specific issues:

* **Parts Lost (Default)**: The total volume of missed production.
* **Self Performance**: The efficiency of the asset in isolation.
* **Total Performance**: The asset's performance within the context of the entire line.
* **Downtime Frequency**: How often the asset stops.
* **Downtime Duration**: Total time the asset remained inactive.
* **Bad Parts**: The volume of non-conforming parts produced.

Cell Insights: Each cell entry displays its name, parts lost, availability, quality, and self-performance. Click "View Critical Assets" to see individual machines within a cell (the number in parentheses indicates how many assets require attention). Use the "View Opportunities" button to see specific recommendations for improvement.\
\
You can view the same information against a critical asset as well. You can click on the "View opportunities" button to view improvement opportunities for critical assets.\
\
To the right of the page, you can see graphs that correspond to the selected options on the left hand side. When a particular sort by is selected, the corresponding graph will open up on the right side. However, you can toggle between the various graphs available.

Currently, we provide the following graphs:

#### Self performance

This graph displays a **Self-Cycle Histogram** for the selected cell across your chosen timeframe. It provides critical insights into **"over-cycling"** events, specifically highlighting how many cycles exceeded their targets and the total production time lost as a result. This graph is the default view when sorting by **APQ or Self Performance.**

#### Total performance

This view provides a **Total Cycle Histogram** for the selected cell. Like the Self Performance graph, it tracks over-cycling trends and time loss, but within the context of the entire line's performance. This is the default view when sorting by **Total Performance**.

#### Downtime duration

This graph categorizes the duration of downtime by specific causes for the selected cell. By clicking on a bar within the graph, you can view the corresponding cause description and navigate directly into **Aggregate Downtime Details**. This is the default view when sorting by **Downtime Duration**.

#### Bad parts

This graph tracks the count of non-conforming parts produced per day for the selected cell. This is the default view when sorting by **Bad Parts.**



## Critical Machine Opportunities

**Opportunities** identify the root causes behind underperforming assets and provide targeted suggestions to improve overall line efficiency. These opportunity cards describe the specific issue, the asset involved, and the potential impact of addressing the problem. By default, when a cell is selected, the system displays opportunities for the first asset in that cell.

There are three primary categories of opportunity cards:

#### Availability opportunities

These represent significant downtime events where assets within a cell were completely unavailable for production. While these explain the primary reasons for a cell’s "critical" status, they are often used for root-cause analysis rather than immediate real-time adjustments.

* **Drilldown:** To investigate, click the **Availability Opportunity** card for the selected asset. This opens a section showing all hourly intervals where the asset was down, the frequency of those downtimes, and the total duration.
* **Action**: Select a specific interval and click the button below to navigate to the **Downtime Details** page for that specific hour.

#### Stability opportunities

**Stability issues** focus on events that disrupt the consistency of the production flow. These are divided into two types:

* **Stuck States:** These occur when an asset is cycling but becomes interlocked in a suboptimal state.
  * **Drilldown**: Click the Stuck State card to view an hourly breakdown of these instances and their total duration.
  * **Action**: Select an interval and click the button below to open the Cycles Page for that hour, where the specific stuck states will be highlighted.
* **Stoppages**: These are short-duration downtime events lasting 15 minutes or less.
  * **Drilldown**: Click the Stoppage card to see the hourly intervals where these events occurred, including the total count and duration.
  * **Action**: Select an interval and click the button below to open the Downtime Page for that hour, with the relevant stoppages highlighted.

This will open the downtimes page for the selected hour, with the stoppage/s highlighted.

#### Performance opportunities

These opportunities focus on optimizing active machine time and reducing hidden inefficiencies:

* **Static Delays**: These are conditions where an asset waits between operations, often due to programmed delays in the PLC that can be eliminated.
  * **Drilldown**: Click the Static Delays card to view a State Histogram for all states in the asset's cycles, including the number of instances, modes, means, and standard deviations.
  * **Action**: Select a specific state and use the A/B Comparison tool to compare a fast and slow cycle to identify where the delay occurs.
* **Variable Cycle Times**: This indicates that the same operation is taking inconsistent amounts of time, meaning the process could be optimized to match the "faster" cycles.
  * **Drilldown**: Click the Variable Cycle Times card to access the State Histogram and statistical data for that asset.
  * **Action**: Use the A/B Comparison tool to analyze the differences between fast and slow cycles to exploit optimization potential.
* **Cyclical Waits (Walls)**: This occurs when assets are waiting on one another, either directly or through a chain of dependencies, often due to suboptimal priority logic or automation wait positions.
  * **Drilldown**: Click the Cyclical Waits card to see the hourly intervals where these waits occurred, including start and end times.
  * **Action**: Select an interval and click the button below to view the Interaction Graph, which visualizes the relationship between the selected asset and the asset causing the wait.

#### Interaction wait delays

These are programmed delays that occur during the interface between assets. Even after an asset receives the **"go-ahead"** to process or release a part, it waits for a set duration. Removing these delays can significantly improve overall cycle time.





