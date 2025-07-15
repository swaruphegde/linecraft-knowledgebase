---
description: >-
  Walkthrough of the various types of dashboards that Linecraft provides and how
  they work
---

# 📊 Dashboards

## Overview

The dashboard provides you with a first glance of the most important data points on your line. These can either be standard KPIs that all lines will track or specific data points that you would like to be able to see at a glance.

The top section of the dashboard consists of cards that depict your top 5 bottlenecks over the last 2 weeks. This feature is only available as part of the analyze and optimize plan.

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
If your line is on the monitor plan, you will not be able to see bottleneck cards.
{% endhint %}

Below this, you will see a list of sub-tabs with 4 options. These are the 4 different types of dashboards that you can view:

<figure><img src="../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Template dashboard

Under template dashboard, you can create a dashboard to view important parameters of your line with the help of pre-defined templates provided by Linecraft AI.

#### Analysis dashboard

You can create custom graphs and configure them in the analysis dashboard. This allows for a more custom and tailored experience when analyzing your line.

#### IOT-Quality dashboard

The IoT-Quality dashboard enables you to plot custom, real-time graphs of your line's quality and process parameters that allow you to monitor your processes in real time.

#### KPI dashboard

The KPI dashboard allows you to monitor different KPIs of your line in real-time, by plotting custom graphs and configuring their layout.

## Template dashboard

Linecraft AI provides a wide range of pre-set templates that you can leverage to create your own template dashboard to monitor and analyze the following parameters:

* OEE
* JPH
* Good part production
* Overall production
* MTTR
* MTBF
* Downtimes and uptimes
* Bottlenecks
* Bad parts

#### OEE trend

The OEE trend graph highlights the OEE trend over a specified period of time along with the target OEE, in a line-chart view.

<figure><img src="../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### **JPH trend**

The JPH trend graph highlights the JPH trend over a specified period of time along with:

1. Average JPH
2. JPH availability, performance and quality losses

<figure><img src="../.gitbook/assets/image (3) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### **On-shift good part production**

The on-shift good part production graph highlights the number of good parts produced during defined shift timings along with the production target

<figure><img src="../.gitbook/assets/image (4) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### **Overall production**

The Overall production graph highlights the total number of parts (good and bad) produced during the defined shift timings and beyond that as well along with the target production

<figure><img src="../.gitbook/assets/image (5) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Downtime v/s uptime (cell and machine)

The downtime vs uptime graphs come in two variants: cell and machine.\
The cell downtime vs uptime graph highlights the duration when cells were down vs when they were up. The machine variant of it displays the same information, but for machines

<figure><img src="../.gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

#### JPH timeseries (cell and machine)

The JPH time series graphs come in two variants: cell and machine. The cell-wise JPH time series graph displays the following data for cells of a line, whereas the machine-wise JPH time series graph displays the same data, but for machines:

1. Average JPH
2. JPH availability loss
3. JPH performance loss
4. JPH quality loss

<figure><img src="../.gitbook/assets/image (7) (1).png" alt=""><figcaption></figcaption></figure>

#### OEE time series (cell and machine)

The OEE time series graphs come in two variants: cell and machine. The cell-wise OEE time series graph displays the following data for cells of a line, whereas the machine-wise OEE time series graph displays the same data, but for machines:

1. OEE
2. Availability
3. Performance
4. Quality
5. Target OEE

<figure><img src="../.gitbook/assets/image (8) (1).png" alt=""><figcaption></figcaption></figure>

#### MTBF time series

The MTBF time series represents the mean time taken between consecutive failures and the average MTBF, over a period of time

<figure><img src="../.gitbook/assets/image (9) (1).png" alt=""><figcaption></figcaption></figure>

#### MTTR time series

The MTTR time series represents the mean time taken to repair failures and the average MTTR , over a period of time

<figure><img src="../.gitbook/assets/image (10) (1).png" alt=""><figcaption></figcaption></figure>

#### Bad parts pareto

The bad parts pareto represents a pareto chart of bad parts produced by a machine and how much each machine is contributing to the total number of bad parts produced

<figure><img src="../.gitbook/assets/image (12) (1).png" alt=""><figcaption></figcaption></figure>

#### Bottleneck impact

The bottleneck impact represents the impact of bottleneck cells and machines on the entire line as a percentage value

<figure><img src="../.gitbook/assets/image (13) (1).png" alt=""><figcaption></figcaption></figure>

## Analysis dashboard

This subtab allows the user to add graphs for data points that are historic in nature. To create a graph, click on the create custom graph from the top right corner.

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

This will open a form where you will need to fill the following details:

1. Name of the graph
2. Parameter and Level Selection
3. Chart Parameter selection for Date range, Chart type, Resolution & Aggregator Selection
4. Entity/Machine selection for selecting the desired Machine/Cell/Process IO/ State

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

The analysis dashboard consists of a wide variety of parameters that you can select to plot a graph of your choice. You can also enter a custom formula of your own.

To create a custom formula, select custom formula from the parameter dropdown. This will then give you an option to either pick a pre created formula or create a new one. In the event that you have not yet created a custom formula, you will only see one option in the dropdown.

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

You can then use the custom formula creation screen to create the formula that you want. Simply choose the parameters that you would like to add and any mathematical operations required and click on Create.

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

Once a formula is created, it will show up in the list of custom formulas

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

Select variables and aggregators for your formula and you are good to go!

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

The selected parameters will be turned into a graph and will show up in the preview page

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

Here you have graph setting options like Graph Name, Selected Date Range, Filter Option, Resolution and Chart type.

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

The plotted graph is displayed in this section of the screen. The standard chart interactions like zooming on the selected area, moving forward and backwards in the range are available here. The plotted graph also has a target line plotted for it. Incase of a range target 2 lines i.e. min and max are plotted.

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

Once the graph is created and save, it will show up directly in your analysis dashboard. In the event that you would like to edit this graph, you can do so by clicking on the edit icon on the graph itself.

## IOT-Quality dashboard

This subtab allows the user to add graphs for data points that are real-time in nature, specifically for IoT and Quality parameters.

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

To create a graph, click on the create custom graph from the top right corner.

This will open a form where you will need to fill the following details:\
\- Name of the graph\
\- Parameter and Level Selection\
\- Chart Parameter selection for Date range and Chart type\
\- Entity/Machine selection for selecting the desired Machine/Cell/Process IO/ State

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

The IoT and Quality dashboard consists of a choice of the following parameters:

* Quality Parameters
* IoT Parameters
* Custom Formula

<figure><img src="../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

Once the graph is created and save, it will show up directly in your IoT and Quality dashboard. In the event that you would like to edit this graph, you can do so by clicking on the edit icon on the graph itself.

<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

## KPI dashboard

This subtab allows the user to add KPI trackers for data points that are real-time in nature, specifically for parameters other than IoT and Quality parameters.

<figure><img src="../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

To create a KPI tracker, click on the create custom graph from the top right corner.

<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

This will open a form where you will need to fill the following details:\
\- Name of the graph\
\- Parameter and Level Selection\
\- Chart Parameter selection for Date range and Chart type\
\- Entity/Machine selection for selecting the desired Machine/Cell/Process IO/ State

<figure><img src="../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

Once the graph is created and save, it will show up directly in your IoT and Quality dashboard. In the event that you would like to edit this graph, you can do so by clicking on the edit icon on the graph itself.
