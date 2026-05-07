---
description: >-
  Identify and prioritize the assets that impact your production efficiency
  based on real-time performance metrics.
hidden: true
---

# Critical Machines

### What is the Critical Machines Module?

The Critical Machines module helps you identify the machines and production cells that are impacting production performance the most.

Assets are ranked based on production impact, allowing you to focus on the most critical issues first instead of manually reviewing every machine.

**Use this module to:**

* Identify production bottlenecks
* Analyze downtime patterns
* Investigate performance losses
* Track quality-related issues
* Discover optimization opportunities
* Prioritize operational improvements

To access this feature, select the **Critical Machines** card from the main menu.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-15 160402.png" alt=""><figcaption></figcaption></figure>

#### Understanding the Layout

<table><thead><tr><th width="230" valign="middle">Section</th><th>Purpose</th></tr></thead><tbody><tr><td valign="middle">Left Panel</td><td>Displays critical cells, assets, and opportunities</td></tr><tr><td valign="middle">Right Panel</td><td>Displays graphs related to the selected metric</td></tr></tbody></table>

The graph updates automatically based on:

* Selected asset or cell
* Selected sorting parameter
* Selected timeframe

**Recommended View:** The default 2-week timeframe is recommended because it typically captures meaningful production trends while reducing short-term noise.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-16 160831.png" alt=""><figcaption></figcaption></figure>

#### Sorting & Filtering

You can rank critical assets based on the following parameters to pinpoint specific issues:

<table><thead><tr><th width="231.59991455078125"></th><th></th></tr></thead><tbody><tr><td><strong>Parts Lost (Default)</strong></td><td>The total volume of missed production.</td></tr><tr><td><strong>Self Performance</strong></td><td>The efficiency of the asset in isolation.</td></tr><tr><td><strong>Total Performance</strong></td><td>The asset's performance within the context of the entire line.</td></tr><tr><td><strong>Downtime Frequency</strong></td><td>How often the asset stops.</td></tr><tr><td><strong>Downtime Duration</strong></td><td>Total time the asset remained inactive.</td></tr><tr><td><strong>Bad Parts</strong></td><td>The volume of non-conforming parts produced</td></tr></tbody></table>

#### Understanding Cell Insights

Each cell entry includes:

* Cell name
* Parts lost
* Availability
* Quality metrics
* Self performance

Available Actions

* **View Critical Assets** — Open machines within a selected cell

<figure><img src="../.gitbook/assets/Screenshot 2026-04-16 160831.png" alt=""><figcaption></figcaption></figure>

* **View Opportunities** — Investigate optimization opportunities for the selected asset

<figure><img src="../.gitbook/assets/Screenshot 2026-04-16 161519.png" alt=""><figcaption></figcaption></figure>

\
To the right of the page, you can see graphs that correspond to the selected options on the left hand side. When a particular sort by is selected, the corresponding graph will open up on the right side. However, you can toggle between the various graphs available.

#### Understanding the Graphs

#### Self performance

You can analyze cycle efficiency for the selected cell using the Self-Cycle Histogram. Identify over-cycling events, cycles exceeding targets, and the resulting production time loss.

_Default graph when sorting by APQ or Self Performance._

<figure><img src="../.gitbook/assets/Screenshot 2026-04-16 161519 (1).png" alt=""><figcaption></figcaption></figure>

#### Total performance

View line-wide cycle efficiency using the Total Cycle Histogram. Track over-cycling trends, production time loss, and performance impact across the entire production line.

_Default graph when sorting by Total Performance._

<figure><img src="../.gitbook/assets/Screenshot 2026-04-16 161737.png" alt=""><figcaption></figcaption></figure>

#### Downtime frequency

Track how often downtime events occur for the selected cell across the chosen timeframe. Select a bar to view the associated downtime cause and drill into Aggregate Downtime Details for deeper analysis.

_Default graph when sorting by Downtime Frequency._

<figure><img src="../.gitbook/assets/Screenshot 2026-04-16 161837.png" alt=""><figcaption></figcaption></figure>

#### Downtime duration

Analyze total downtime duration by cause for the selected cell. Select a bar to view the associated cause and navigate directly to Aggregate Downtime Details for further investigation.

_Default graph when sorting by Downtime Duration._

<figure><img src="../.gitbook/assets/Screenshot 2026-04-16 161915.png" alt=""><figcaption></figcaption></figure>

#### Bad parts

Monitor the daily count of non-conforming parts for the selected cell to identify quality trends and recurring production issues.

_Default graph when sorting by Bad Parts._

<figure><img src="../.gitbook/assets/Screenshot 2026-04-27 110109.png" alt=""><figcaption></figcaption></figure>



## Critical Machine Opportunities

Opportunities help identify the root causes behind underperforming assets and highlight areas for improving overall line efficiency. Each opportunity card provides insight into the issue, the affected asset, and its production impact.

By default, selecting a cell displays opportunities for the first asset within that cell.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-16 180013.png" alt=""><figcaption></figcaption></figure>

#### Availability opportunities

Represents periods where assets were completely unavailable for production.

**Best for:** Root-cause analysis and major production interruptions.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-27 155713.png" alt=""><figcaption></figcaption></figure>

* **Drilldown:** To investigate, click the **Availability Opportunity** card for the selected asset. This opens a section showing all hourly intervals where the asset was down, the frequency of those downtimes, and the total duration.
* **Action**: Select a specific interval and click the button below to navigate to the **Downtime Details** page for that specific hour.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-27 154834.png" alt=""><figcaption></figcaption></figure>

#### Stability opportunities

Highlights issues affecting production consistency.

**Best for:** Investigating recurring operational interruptions.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-27 154221.png" alt=""><figcaption></figcaption></figure>

These are divided into two types:

* **Stuck States:** These occur when an asset is cycling but becomes interlocked in a suboptimal state.
  * **Drilldown**: Click the Stuck State card to view an hourly breakdown of these instances and their total duration.
  * **Action**: Select an interval and click the button below to open the Cycles Page for that hour, where the specific stuck states will be highlighted.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-27 154030.png" alt=""><figcaption></figcaption></figure>

* **Stoppages**: These are short-duration downtime events lasting 15 minutes or less.
  * **Drilldown**: Click the Stoppage card to see the hourly intervals where these events occurred, including the total count and duration.
  * **Action**: Select an interval and click the button below to open the Downtime Page for that hour, with the relevant stoppages highlighted.

This will open the downtimes page for the selected hour, with the stoppage/s highlighted.

#### Performance opportunities

Focuses on hidden inefficiencies during active production.

**Best for:** Throughput optimization and cycle-time improvements.

Includes:

* **Static Delays**: These are conditions where an asset waits between operations, often due to programmed delays in the PLC that can be eliminated.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-27 112923.png" alt=""><figcaption></figcaption></figure>

* **Drilldown**: Click the Static Delays card to view a State Histogram for all states in the asset's cycles, including the number of instances, modes, means, and standard deviations.
* **Action**: Select a specific state and use the A/B Comparison tool to compare a fast and slow cycle to identify where the delay occurs.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-27 114639.png" alt=""><figcaption></figcaption></figure>

* **Variable Cycle Times**: This indicates that the same operation is taking inconsistent amounts of time, meaning the process could be optimized to match the "faster" cycles.
  * **Drilldown**: Click the Variable Cycle Times card to access the State Histogram and statistical data for that asset.
  * **Action**: Use the A/B Comparison tool to analyze the differences between fast and slow cycles to exploit optimization potential.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-27 114727.png" alt=""><figcaption></figcaption></figure>

#### Interface delays

Identify delays caused during signal exchange between connected assets. These programmed waits and interlocks can impact the cycle time of multiple assets across the line.

To investigate:

* Open the **Interface Delays** card
* Review affected hourly intervals
* Analyze the interval start and end times
* Investigate synchronization delays between interfacing assets

**Cyclical Waits (Walls)**:&#x20;

Analyze dependency-related waits where assets are blocked by one another directly or through chained dependencies. These waits are often caused by inefficient automation logic or priority sequencing.

To investigate:

* Open the **Cyclical Waits** card
* Review affected hourly intervals
* Select an interval
* Open the **Interaction Graph** to identify the blocking asset and dependency chain

<figure><img src="../.gitbook/assets/Screenshot 2026-04-27 153133.png" alt=""><figcaption></figcaption></figure>

#### Interaction wait delays

Identify programmed delays that occur between interfacing assets, even after a process or release signal is received. Reducing these waits can help improve overall cycle time and production flow.

Best used for:

* Identifying hidden interface delays
* Improving asset synchronization
* Optimizing overall throughput



> The Critical Machines module is designed to help teams move from identifying issues to understanding root causes and prioritizing operational improvements efficiently.





