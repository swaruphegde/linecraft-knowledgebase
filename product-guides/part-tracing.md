---
description: >-
  Walkthrough of how the part moved from the start of the line and a tabulation
  of its process parameters throughout its journey
---

# 📦 Part tracing

## Overview

The part tracing feature allows you to track the journey of a specified part on the line. This includes the assets it passed through and it’s parameters at each step.

<figure><img src="../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

To view the journey of the part there are two ways:&#x20;

* Entering the serial number of the part.
* Selecting a part from the list of parts that passed through the line for the specified date range.

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

#### Serial number search

Once you click on the text box for searching serial number, you will see your last 5 searches. When you start entering the serial number, you will get matching suggestions. Selecting a suggestion, will take you to the Part Tracing Gannt Chart that shows the journey of the part.

#### Quality KPIs

Another way is to clicking, by the Quality KPI cards shown below the search box.\
The quality KPIs number are based on the date selected. Clicking on any of the card will take you the table that shows all the parts matching that criteria.\
For e.g.

* Total parts introduced will take you the table that lists all the parts that entered the line
* Part Rejects will take you to the list of parts that were rejected.

\
The KPI cards are available on the left side of the table to switch to different KPI table.

* The table has details of the part like
* First introduced on the line
* Serial number
* Part Type
* Number of reworks
* Part Acceptance: Part OK or Part Reject
* Non compliant percentage: tells you the number of failed process parameters out of total process parameters of all assets.

Clicking on the serial number of any part opens a button that takes you to Part Tracing Gannt Chart of that part.

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

The part tracing module has four main sections:

## Part summary

Displays the part details of the current part. It also has a button to check the process parameters of the part. It contains the following details:

* Serial number: If any child parts were added, this section becomes collapsible to show IDs of the child part
* Part type
* Time stamp when the part first entered the line
* Time spent by the part on the line
* Number of re-works: if more than 0, then this section becomes collapsible to show the asset which sent it for rework. In case of multiple reworks, this will have list of assets with rework number besides it.

<figure><img src="../.gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

## Gantt chart

Shows the journey of the part across various assets. The list of assets on the left also has the search box to filter and show specific assets. For each asset it shows graphical representation of time spent by the part in that asset, a cycle time bar which shows red color if it exceeded target cycle time and green if within target cycle time and the target cycle time dotted line. Hovering over the bar will show the numerical values for above data in a tooltip.

<figure><img src="../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>

Clicking on any bar of the Gannt chart will expand the row of that asset showing following information

* Cycle Duration Statistics: target cycle time. Here you also have the option to switch to different instances of these details of the same asset in case of rework
* Quality Statistics: number of reworks and retries
* Process Parameter: Total process parameters & failed process parameters
* Cycles drilldown : will take you to the cycles drilldown for this instance of the asset

<figure><img src="../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>

If there was any rework done on the part that means that part has to pass through some of the assets more than once. You can check other information of other instances by clicking the arrow below Cycle statistics information. If the asset didn’t pass more than once from this asset, the arrows will be replaced with text indicating that there are no other instances present for this asset for this part.

## Process parameter table

Clicking on “Process Parameter” button from the part summary section will open up the process parameter table. Process Parameters for all the assets will be listed here. For some parameters where there is no min max value, like recipe number. These will be displayed in grey color.

<figure><img src="../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

## Process parameters

You can click on the view process parameters to open the process parameters side panel for this particular instance.\
The side panel will have a table that shows:

* Process parameter name
* Min limit (NA in case of Boolean process parameter)
* Max limit (NA in case of Boolean process parameter)
* Actual Value recorded when part passed (in case of reworks, this column will be present multiple times for each instance). Its color will be red if it was out of range(NOK in case of Boolean) and green if within range (OK in case of Boolean)
* Aggregator used to calculate the actual value.
