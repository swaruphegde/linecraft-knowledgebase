---
description: Monitor the OEE, Availability, Performance and Quality of all your assets
---

# 🚥 Machine monitoring

## Overview

The machine monitoring module provides real-time visibility into machine-level performance and enables state-based prioritization. It provides you with a comprehensive view of all machines on your line with their real-time status. &#x20;

You can also view machine-level details and understand individual machine performance. &#x20;

You can access the machine monitoring module from the main menu. &#x20;

<figure><img src="../.gitbook/assets/image (5) (1) (1).png" alt=""><figcaption></figcaption></figure>

You will be displayed all machines of your line in a real-time view on the landing page of the machine monitoring module. This view represents the real-time status of your machines if they are cycling, down or idle.&#x20;

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

You can view details of a machine for a specific period in the machine overview screen. For each machine, you will be displayed its:&#x20;

* Overall OEE and production&#x20;
* Availability, Performance and Quality KPIs&#x20;

On the same screen, you can change the time duration to view machine performance for a different period.&#x20;

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

You can view all parameters of a machine by navigating to the parameters section. You can either opt to view the parameters in a table form or a graph form.&#x20;

On this screen, you will also be able to drill down to view aggregate downtimes and aggregate cycles of a machine. &#x20;

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

You can also navigate to the heatmap view of cells and machines from the heatmap tab of the machine monitoring module. This will redirect you to the existing heatmap which will open in a new browser tab. &#x20;

## Heatmap

To access a heatmap view of your line's OEE and APQ parameters, navigate to the "Heatmap" tab of the machine monitoring module. This will open the heatmap in a new browser tab. By default, the heatmap displays all machines on your line along with their OEE values - including average, minimum, and maximum metrics. You can toggle between viewing data by machine(asset) or by cell.

Additionally, you can switch the heatmap to display various performance parameters and apply filters by part types or shifts.

<figure><img src="../.gitbook/assets/image (6) (1) (1).png" alt=""><figcaption></figcaption></figure>

You can filter the heatmap by various parameters to view their values during the selected date range:\
Available Parameters\


1. OEE
2. Availability
   1. Overall Availability
   2. JPH Availability Loss
   3. Availability Part Loss
   4. Downtime
3. Performance
   1. Total Performance
   2. Self-Performance
   3. Good Part JPH
   4. Total Part JPH
   5. Good Parts
   6. Total Parts
4. Quality
   1. Overall Quality
   2. Bad Part JPH
   3. Bad Parts\


You can either view the heatmap of all machines or cells of your line. By default, you will be displayed the heatmap of your machines. \
\
**Machine heatmap view**\
When viewing the machine-level heatmap, you’ll see a list of all machines on your line, each showing:

* The selected parameter’s values for the specified date range
* Machine-specific average, minimum, and maximum values for that parameter

<figure><img src="../.gitbook/assets/image (7) (1) (1).png" alt=""><figcaption></figcaption></figure>

Selecting a machine provides a detailed view of:

1. Production losses related to availability, performance, and quality
2. Key metrics: Availability, Performance, and Quality
3. Additional insights: Downtime details, Cycle details, and Opportunity analysis

<figure><img src="../.gitbook/assets/image (8) (1) (1).png" alt=""><figcaption></figcaption></figure>

**Cell heatmap view**\
When switching to cell-level heatmap view, you’ll see all cells on your line with:

* Selected parameter values for the chosen date range
* Cell-specific average, minimum, and maximum values

<figure><img src="../.gitbook/assets/image (9) (1) (1).png" alt=""><figcaption></figcaption></figure>

Upon selecting a cell, detailed insights include:

1. Production losses due to availability, performance, and quality issues
2. Metrics for Availability, Performance, and Quality
3. Further analysis: Gross downtimes, Interaction history, and Opportunities

<figure><img src="../.gitbook/assets/image (10) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Heatmap drilldowns

The heatmap of cells and machines provides you with a starting point to understand which machines or cells of your line are underperforming in what areas (such as availability, performance, quality, etc).

You can perform the following drilldowns from the heatmap to identify root causes and take appropriate preventive and corrective measures:

1. View gross downtimes and causes of all machines of a cell
2. View downtime details of a specific machine and sub-assemblies
3. View IO level transitions
4. View cell interactions
5. View cycle details of a machine and sub-assemblies
6. Compare two cycles of the same machine or sub-assembly

#### **Gross downtimes**&#x20;

You can view the downtimes of all machines of a cell from the cell-level heatmap by clicking on the "Gross downtimes" button after selecting a cell.

<figure><img src="../.gitbook/assets/image (11) (1) (1).png" alt=""><figcaption></figcaption></figure>

You will be redirected to the gross downtime screen that highlights:

1. The total wait diagram of the machines of a cell - this diagram represents the line flow of machines within the selected cell. You can select one or more machines from this diagram to view their individual and total downtimes.&#x20;
2. A non-production interval graph that highlights downtime instances by count and by duration of machines within the selected cell.&#x20;
3. List of selected machines (from the total wait diagram) of the selected cell in a tabular format. Each machine tab contains the following details:
   1. Name of the machine
   2. List of downtime causes, ranked by either duration or count
   3. Downtime causes trend of either count or duration

<figure><img src="../.gitbook/assets/image (12) (1) (1).png" alt=""><figcaption></figcaption></figure>

You can further focus on one particular machine's downtime details by clicking the "Downtime details" button from the gross downtimes screen. Additionally, you will be able to download PDFs, images and excel sheets of the non-production interval and downtime causes trend graphs by clicking on their respective download buttons.

#### **Downtime details**

You can view the downtime details of a machine and its sub-assemblies (if they exist) by clicking on the "Downtime details" button after selecting a machine in the machine heatmap.

<figure><img src="../.gitbook/assets/image (43) (1).png" alt=""><figcaption></figcaption></figure>

You will be redirected to the downtime details screen that highlights:

1. The downtime causes list - This lists down all downtimes of the selected machine and their causes.&#x20;
2. A downtimes graph that represents the downtime trends of the selected machine
3. The IO transition sequence of the selected machine - This represents each state transition of the machine with its machine status. Upon selecting a state either from the graph or from the transition sequence, following details the state will be displayed:
   1. Name of the state
   2. Option to perform analysis of the state
   3. Option to copy the state name for use in other modules of the product
   4. Start and end time of the state
   5. Duration of the state
   6. Category of the state
   7. Status of the state and duration of the state's status

<figure><img src="../.gitbook/assets/image (44) (1).png" alt=""><figcaption></figcaption></figure>

You will be able to roll up to gross downtimes by clicking on the "Gross downtimes" button on the downtime details screen. Additionally, you will also be able to download the downtimes graph as a PDF, image or an excel by clicking the download button.

#### Interactions drilldowns

In order to understand and view how machines within a cell are interacting with each other, you can click the "Interactions" button after selecting a cell in the heatmaps view.

<figure><img src="../.gitbook/assets/image (14) (1).png" alt=""><figcaption></figcaption></figure>

You will then be redirected to the interactions page that displays the following information:

1. An interaction diagram of all machines of the selected cell - this is similar to the total wait diagram of machines within a cell and highlights the machine status in the form of color coded machine units.&#x20;
2. Gantt chart of all machines of the selected cell - this highlights the status and duration of the status of all machines of the selected cell that helps in understanding how each machine was interacting and in which state within the cell.&#x20;
3. A tabular view of each selected machine (from the interaction diagram) within the cell highlighting the following information:
   1. Name of the machine
   2. Start time, end time and duration of the selected cycle/state of a machine
   3. Avg cycle time of the machine
   4. Target cycle time of the machine
   5. Dependent assets of the machine
   6. Part type that is being operated on by the machine and its related information
   7. Option to analyze the IO transition sequence of the machine

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

You will be able to drilldown further to view the cycle details of a particular machine by clicking the "Cycles" button on the interactions screen. Additionally, you will also be able to download the PDF, image and excel of the gantt chart of the cell's machines by clicking on the download button.

#### Cycles drilldown

In order to view the cycle details of a machine, you can click the "Cycles" button by selecting a machine's detail in the heatmap.

<figure><img src="../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption></figcaption></figure>

You will then be redirected to the cycles screen that includes the following details:

1. A list of all cycles of the machine along with their
   1. start time
   2. total duration (duration of the machine when it was cycling and interacting with other machines or operators)
   3. self duration (duration of the machine when it was cycling without any interactions)
   4. number of parts produced in each cycle.
2. Gantt chart of states of the machine highlighting their status and duration
3. Details of the machine and its sub-assemblies (if any):
   1. Machine name
   2. Sub-assemblies name (if any)
   3. Start time, end time and duration of the selected cycle/state
   4. Avg cycle time
   5. Target cycle time
   6. Part type the machine was working on along with its details
   7. Option to analyze the IO transition sequence of the machine

<figure><img src="../.gitbook/assets/image (3) (1) (1).png" alt=""><figcaption></figcaption></figure>

You can download the gantt chart of the machine in PDF, image or excel format by clicking on the download button. Additionally, you can roll back up to the interactions view by clicking the "Interactions" button.

#### IO level drilldown

You can drilldown to the IO transitions from the interactions or the cycles screen by clicking on the "I/O Level" button. This will redirect you to the IO analysis screen where you will be displayed the following information:

1. List of cycles of the selected machine with the following data:
   1. Start time
   2. Duration
   3. Self-duration
   4. Parts produced
2. A cycles graph that represents home to home state transition in all cycles of the machine
3. IO transition sequence of the selected cycle along with details of the selected state:
   1. Name of the state
   2. Option to perform state analysis
   3. Option to copy name of the state
   4. State ID - A unique number associated with every state
   5. Duration and status of the state

<figure><img src="../.gitbook/assets/image (4) (1) (1).png" alt=""><figcaption></figcaption></figure>

You can filter the graph by selecting up to 5 parameters to view as well as download it as a PDF, image or excel by clicking on the download button.

#### Cycles comparison

You can compare two different cycles of a machine on the IO level screen by setting one cycle as "cycle A" and another as "cycle B". In order to do this, simply hover over a state in the list of cycles. You will be displayed a button that allows you to set a cycle as the benchmark "A" cycle and another as the comparison "B" cycle.

Once these two are set for comparison, simply click on the compare button to view a comparative graph and IO transition view of the selected states.

<figure><img src="../.gitbook/assets/image (45) (1).png" alt=""><figcaption></figcaption></figure>

You can navigate back to the cycles graph or the interactions screen by clicking their respective buttons.
