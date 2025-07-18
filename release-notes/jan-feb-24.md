---
description: 'Wipro Linecraft AI Product Updates: Jan-Feb 2024'
---

# Jan-Feb '24

{% hint style="info" %}
Last Version: 4.0.1\
New Version: 4.22.8
{% endhint %}

Ensuring exceptional experiences with every interaction is now essential, rather than optional. To achieve this objective, we are implementing a modularization concept in the revamp of our product. The aim is to streamline the product, enhance user experience, and optimize performance even further.

## Features and improvements

#### New reports module with out-of-the-box templates

The new report module offers pre-defined templates, allowing users to schedule reports using predefined Intervals/frequencies such as daily, shift-wise, weekly, etc. Users can preview reports before scheduling them. Furthermore, this module enhances users' ability to analyze additional insights from both received and scheduled reports

{% embed url="https://www.loom.com/share/b52a0aa6611e49179d6d119ff87a29a3?sid=b428ca1e-25c9-4c2e-a5e7-d9f6e52fedc6" %}

#### Enhanced EOD part tracing report

We have improved the EOD Part tracing report to help users get more visibility which will enable users to grasp the precise state of the part from its introduction on the line to its progress and completion. Such clarity is crucial for customers who prioritize quality assurance.&#x20;

Users will gain access to additional parameters regarding the part, including its status (In-progress/complete) and the total time it spent on the line.

{% embed url="https://www.loom.com/share/99e8622197704a24be21a7b4368fbb16?sid=afa991a8-a9ab-464b-855d-7962b7291d8e" %}

#### Default one week data load across the product

Throughout the product, we've implemented a default data loading setting for one week. Users can adjust the start and end times to view data over longer durations if desired.

#### Split IoT/Quality dashboard from KPIs

The current setup combines key performance indicators (KPIs) with graph plotting capabilities for IoT and quality parameters. To improve performance and user experience, we are dividing this into two separate categories.

Customers with a focus on quality will likely be drawn to the IoT and Quality graphs to grasp trends. Conversely, those prioritizing production efficiency will find KPIs more valuable for real-time production insights and JPH tracking.

{% embed url="https://www.loom.com/share/9e6dad9393dc43a487a0052621e0091d?sid=1a1912e7-134a-4ace-9c22-c3584a125d07" %}

#### Quality and performance losses overlapping

The objective here was to offer users a clear understanding of when losses occur due to over-cycling, ultimately resulting in the production of bad parts.

In this context, the duration of loss attributed to quality will equate to the cycle time, while the duration contributing to performance loss will specifically be the over cycling time.

#### Set alert to track unattributed losses count

In Alerts Configuration - We've introduced a new parameter called "Unattributed Losses" to our current list of parameters, enabling users to establish conditional alerts for any designated time frame.

This feature allows businesses to monitor unattributed losses and receive alerts via various modes such as email, SMS, or within the product interface when specified conditions are met.

This functionality will assist users in monitoring whether losses exceeding a certain threshold remain unattributed, potentially compromising the accuracy of loss analysis.

{% embed url="https://www.loom.com/share/4dd880e1000144fab47847843462203d?sid=a4ced02b-c83e-4920-a69a-c98e604a42c6" %}

#### Auto-run data processing on breaks/shift changes

Whenever users modify breaks or shifts in the production schedule, the product will execute data processing within the corresponding time range to reflect accurate data across products based on the user's defined changes.

When users make such changes, the auto-run process will occur accordingly. However, until the processing is complete, users will be restricted from making additional changes and will receive appropriate warnings.

#### Improved navigation for re-vamped user experience

Enhanced navigation lies at the heart of our revamped user experience, guiding users seamlessly through our platform.&#x20;

Upon logging into the product, users will experience a new main menu with module tiles providing detailed insights into each module's functionality. This empowers users to understand what each module has to offer and make informed decisions based on interest.

{% embed url="https://www.loom.com/share/70f0208a35db41e7b00e12a4541726fb?sid=cdc50ed0-3945-411f-a002-d6ce3ac023fa" %}
