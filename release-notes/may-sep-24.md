---
description: 'Wipro Linecraft AI Product Updates: May-Sep 2024'
---

# May-Sep '24

{% hint style="info" %}
Last PSS Version: 6.0.0

New PSS Version: 7.1.0
{% endhint %}

We’re excited to announce the latest release packed with powerful enhancements designed to streamline your operations. This update elevates fault detection with new features such as fault code mapping, entity source display, and part type alerts, providing greater operational clarity and reducing reliance on manual workflows.

The release includes a new asset-wise availability losses report template, giving you deeper insights into availability issues. Combined with the ability to generate on-demand reports, these improvements will help you resolve issues faster, enhance performance tracking, and drive smoother, more efficient operations across the board.

## Features and improvements

#### New Report template: 'Asset-Wise Availability Losses Report': Faults, Downtime, and Occurrences

{% embed url="https://www.loom.com/share/7bfe956179fe444697df8abc4fcc3cf7?sid=344a11ae-bc79-4853-8b20-a486333dfe36" %}

A comprehensive report highlights the top assets or machines to prioritize, identifying areas for improving asset availability by focusing on the root causes of faults and downtime that affect overall equipment effectiveness (OEE). The report aims to deliver actionable insights and recommendations to enhance asset availability, minimize downtime, and boost production reliability.

#### On-demand reports

{% embed url="https://www.loom.com/share/db42f93bafb74c28aa8d04b3d5ca821c?sid=06b74652-5789-4d53-8f52-ace5b8fd4237" %}

Currently, in the reporting module, we offer the ability to schedule reports, allowing users to receive them at predefined intervals based on specified inputs. As a new enhancement, we are introducing a feature that enables users to generate reports instantly, addressing ad-hoc reporting needs without relying solely on scheduled reports.

#### Fault code mapping

We've introduced fault code mapping to accurately display downtime reasons associated with triggered fault codes. You can now upload and manage predefined fault codes and descriptions, allowing the system to automatically show the exact causes of downtime. This eliminates the need to rely on external spreadsheets for fault code mapping. We have enriched logic to support faults in both Integer and Boolean format.

{% embed url="https://www.loom.com/share/717fe6798293405d9a94f97890f9e679?sid=f4600500-b7da-48f0-8f79-e1235d134671" %}

#### Display entity source for faults

Given the varied configurations customers use to set up fault detection, we now help users understand the source of triggered faults by displaying the correct entity. This enhancement provides clearer insights into the origin of faults.

#### New part type detection alert

We've added support to detect and alert users when a new, unconfigured part type is detected. This alert helps users quickly configure new parts to ensure smooth operations.

#### AlertPulse - audio and visual alerts

We've introduced the capability to mark specific alerts as priority alerts. When these alerts are triggered, users will be notified with both audio and visual notification, ensuring they are immediately aware of potential issues that require prompt action.

#### IO State Plotting on Analysis Dashboards

You can now plot IO states (ON/OFF) on an instance-level graph, enabling detailed analysis of IO performance at the asset level.

{% embed url="https://www.loom.com/share/e37264f3a80442ce943c2004284c470d?sid=5ebae1a9-bf5c-4e26-be14-756520c52a4f" %}

#### Key Product Enhancements

Auto-fit asset names on UI: We've improved the representation of asset names for a better user experience.

EOD Part Tracing Report Enhancements:&#x20;We've enhanced the accuracy and reliability of the EOD Part Trace Report by excluding partial cycles and avoiding value rounding.

Copy state ID from cycles: Users can now copy the entire state name from a cycle, which can be used for plotting state duration as part of analysis.

{% embed url="https://www.loom.com/share/9479a05a59c34ded87b8526fe0522557?sid=31c9da30-51bc-471d-b0e0-1b8cae124be0" %}

Graph Analysis with Intuitive Window Zooming capability: We've added window zooming functionality, allowing users to zoom in on specific datasets for more detailed analysis and trend understanding.

{% embed url="https://www.loom.com/share/189c0bb8a181462dab547958e3261c7f?sid=a9d521d7-6b3a-4bd4-90b8-72812b340861" %}

Add Enabling Conditions on Graphs: Users now have the ability to add enabling conditions to graphs for more customized data visualization.

{% embed url="https://www.loom.com/share/5916904fa04243a187163fbcf39ce5c2?sid=9d90e189-9ca5-4209-92e3-7de9f755eec5" %}

Enhanced Visibility of Input/Output Transitions on UI:&#x20;We've added a dropdown menu to display multiple Input/Output transitions, improving the visibility of transitions that were previously trimmed.

Wipro Pari Andon Dashboard Improvements: We've enhanced the dashboard's KPIs to provide more accurate information during production off times and when no production is occurring.

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

Heatmap Export Improvements:&#x20;We've aligned heatmap exports with the data shown on the UI for more accurate reporting.

Show break icon for downtimes overlapping with breaks: In case when a downtime overlaps with a break, we are enriching logic to show a break icon to help users easily identify downtimes that coincide with breaks.

Enhance 'Asset Wise Production Summary' report to include Availability insights: Currently, the Asset-wise Production Summary report provides detailed insights into performance and quality. Introducing asset-level uptime and downtime data to enable users to perform more comprehensive analyses from an availability standpoint.

Display Plant and Line Name on Master header: The plant and line names should be prominently displayed on every screen of the product to eliminate the need for users to manually track which project and line they are analyzing.

Configure a new alert for Data Connectivity issues: Introducing a new alert option that notifies users when data collection has stopped for a specified duration. This will allow users to take timely action to resolve connectivity issues, preventing data loss and saving valuable time.

#### Internal Product Enhancements

Config tool reduction/update:\
We've refined our internal configuration application by eliminating unused features and introducing new functionalities to enhance usability and simplify future operations.

Enhanced Quality Node configuration: We've strengthened product support by upgrading the quality node configuration to manage multiple quality signals effectively, ensuring more accurate outcomes.

IoT/Quality Dashboard Enhancement: Improved the performance of the IoT/Quality dashboard by optimizing the data retrieval and display process for large data sets, resulting in more accurate trend visualization.

Restrict users from running DP for future dates from Config UI: Restrict users from running Data Processing (DP) for future dates from the Config UI to avoid data issues and product failures. This will ensure that DP is only executed for dates that have already occurred, preventing potential problems caused by processing incomplete or inaccurate data.

Key bug fixes:

* The Part Tracing module was frequently crashing due to some unhandled exceptions, which has now been stabilized.
* Alert names were inconsistent between Email notifications and product notifications, but they have been standardized.
* The Self-Performance Heatmap was showing zero values at the cell level, which has been corrected to display accurate data.
* The Done button was becoming disabled, preventing the configuration of Notification and SMS channels for alerts, but this has been resolved, and the button is now functional.
* The Target Production Count was displaying incorrect values on the Real-Time Dashboard, which has been adjusted to ensure accuracy.
* Some states in the IO Transition Sequence appeared as blocked or starved even after being force-marked; this has been addressed, and all states now display correctly.
* The Target Cycle Line was missing from the Part Trace Gantt chart, and it has been restored to visibility.
* The Unattributed Losses Pill was incorrectly shown as a loss type in the Filter Pop-Up within Loss Attribution; it has been removed from the loss type options.
* Unattributed Losses from the 2nd shift were appearing even after filtering for the 1st shift, and this has been fixed so that only relevant losses are displayed.
* The Asset Part Type Mapping page was failing to load in the Config UI, but it now opens properly.

\
\
