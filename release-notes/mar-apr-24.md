---
description: 'Wipro Linecraft AI Product Updates: March-April 2024'
---

# Mar-Apr '24

{% hint style="info" %}
Last PSS Version: 4.22.8 \
Current PSS Version: 5.0.0
{% endhint %}

We are pleased to present the most recent updates to the Linecraft product, aimed at improving data accuracy, reliability, enhancing user experience, and boosting productivity. This release introduces a variety of new features, enhancements, and bug fixes to align with our customers' evolving needs.

#### Features and improvements

#### New reporting template - Asset Wise daily production summary

The Asset Wise daily production summary Report is a comprehensive Excel-based report designed to provide detailed insights into the cycles at each asset level.

This report is automatically generated and emailed to key stakeholders on a daily basis, ensuring that decision-makers have access to up-to-date information to optimize production efficiency.

By providing a comprehensive view of production metrics, the Daily Production Efficiency Report empowers manufacturers to optimize their processes, reduce waste, and increase overall productivity

{% embed url="https://www.loom.com/share/20578f5cc82a4f938bbafc56f3213ce5?sid=1a872e2f-e7ad-4bb6-87f4-cf23314ad0f6" %}

#### Improvement on Heatmaps

Facilitating users to conduct in-depth analysis by displaying self-performance through heatmaps, aiding users in comprehending performance at a granular cycle level. Additionally, offering users the capability to export heatmap data to Excel for extended utilization and analysis purposes.

{% embed url="https://www.loom.com/share/f8181df28a1a46238795d0b1215b8680?sid=a563eae3-45d6-47c2-8d23-7cdaf8da41fd" %}

#### Extend loss attribution to non real time setup

We have improved the product capability to record losses even in cases where there are issues with the data stream and data is captured in non-real-time mode.

This enhancement ensures that users can still retain crucial insights, like identified losses, from the data even when the real-time stream is inaccessible.

#### Key usability improvements and product enhancements

Improved Loss Attribution duration filter: The Loss Attribution module has been enhanced with a new filter that allows users to search for specific losses based on duration. This feature provides a more granular level of control, enabling users to filter losses by specifying a range of durations.

{% embed url="https://www.loom.com/share/1df50c1e84e0401cb82edb38e7d1827e?sid=e5608527-9da9-40e8-9005-b589a287c4f7]" %}

Shift and part variants Filters on Template dashboard: Enhancing user experience by introducing additional filtering options for each graph in maximized view, such as shifts and part types, to enable users to delve deeper into data analysis through graphical representations.

{% embed url="https://www.loom.com/share/3007c410011643d69897a2ba32bec32a?sid=6fc58eb2-acf4-44af-836f-1941e074055a" %}

Improving overall product filters and export pop-up: Streamline the product filtering process and enhance the export pop-up feature to provide a seamless user experience.

Time display format standardization: Improving the time display format throughout the product by enabling users to customize their preferred time

{% embed url="https://www.loom.com/share/3197dd029c0c4ae0b0490adde47db67a?sid=d0a97525-1d61-4dfa-a6ef-bed2a5be59dd" %}

Display most recent data processing timestamp within product: Displaying “Latest Data Available” on the product to assist users in identifying the latest information accessible for utilization. Display format in the settings->Preferences.

{% embed url="https://www.loom.com/share/b597f64bfb224a3dbd1420334e28199f?sid=5f66cfd4-d815-407f-adbc-250fca4ad495" %}

Improve Bottlenecks to display Impact in terms of JPH Loss: The Bottleneck page has been updated to show the bottleneck impact in terms of units lost per hour (JPH loss) instead of time lost. This change provides a more direct and actionable metric for understanding the impact of bottlenecks on production output

{% embed url="https://www.loom.com/share/fd9f0a9661a14f3eaf5a4d64f34a3266?sid=2de38906-330d-42e7-bc06-aa47160d19d5" %}

Delta not getting considered while plotting parameter in comparing cycles: The Delta factor specified in the process parameters table is being taken into account when plotting IoT parameters on cycles. However, this factor is not being applied when plotting a parameter on the cycle comparison page. To provide users with a consistent experience, a change has been made to address this discrepancy.

Improved logic for Critical Cell Ranking: In the Critical Assets view, we have introduced a new parameter to display Parts Loss, indicating the asset's unavailability. By default, the assets will be sorted based on their respective Parts Loss, providing a clear overview of the most critical assets.

Expand ability to plot quality parameters on cycle graph: In the cycle graph feature, users can now choose specific quality parameters for graph plotting and trend analysis. Previously, users were limited to selecting only IoT parameters

{% embed url="https://www.loom.com/share/b700b521d02e4350b028ab52ea854148?sid=7491a217-5e8f-4b8a-ae7c-bb5302abe945" %}

Notify about inaccurate Day-Level data in heatmaps: A new functionality has been developed to assist users in quickly identifying missing data within a selected time range. By indicating missing data for each hour out of the 24 in a day with an asterisk

{% embed url="https://www.loom.com/share/f75c3d1f1505418bac619d26e6f2dda9?sid=86a6e287-3e68-46f3-aacd-665c95966fbe" %}
