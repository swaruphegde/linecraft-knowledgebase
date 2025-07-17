---
description: Configure alerts for conditions that you would like to track
---

# 🔔 Condition monitoring

## Overview

Condition monitoring allows the user to set up alerts for conditions that they would like to be alerted about.&#x20;You can access condition monitoring from the main menu by clicking the "Condition Monitoring" module.

<figure><img src="../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

The overview tab displays a summarized view of the following, pertaining to the alerts that have been set up:

1. List of recently triggered alerts
2. Trend of alerts triggered over time
3. Top parameters on which alerts were triggered
4. Top 5 assets that triggered the most alerts
5. Top 5 cells that triggered the most alerts

This tab will give a quick overview about configured alerts and help you understand which areas to focus on and if there is an overall improvement of their lines or not.&#x20;

{% hint style="info" %}
If no alerts have been set up, then the overview screen will be empty&#x20;
{% endhint %}

By default, you will be displayed the above information for the last 7 days. You can change the range of the data by selecting any one of the following options from the date range option:

1. Today - by hour
2. Last 7 days - by day
3. Last 14 days - by day
4. Last month - by day
5. Last quarter - by month

You will be able to create a new alert by clicking the "Create alert" button on the overview section.&#x20;

<figure><img src="../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

## Creating an alert

You will be displayed the alert creation screen when they click on the “Create alert” button on the overview screen. You can set up alerts by entering the following information: \


1. Group name for the alert being configured – this is used to classify various types of alerts
2. Trigger conditions for the alert – you can select the following conditions for triggering the alert
   1. Parameter on which the alert will be based&#x20;
   2. Level of the alert – Line, cell, asset or sub-assembly (You can select multiple or all entities)&#x20;
   3. Condition and frequency – Determines when to trigger the alert&#x20;
3. Once the alert conditions are set, you can select the channels/people to send the alerts to
4. Once an alert has been created, you can view alerts that you have created under the “My Alerts” tab

<figure><img src="../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

## My alerts

The “My alerts” tab lists the alerts created by you and serves as a dedicated space to manage your alerts. You will be displayed an empty state when there are no alerts set up with a button to create their first alert. Clicking on this button will redirect you to the create alert screen&#x20;

You can view the list of alerts either by group name or by level. By default, view by group name will be selected. &#x20;

**View by group name**&#x20;

Along with viewing the list of alerts, you can sort and filter the list. By default, the list will be sorted by ascending order of group name without any filters&#x20;

You can modify or delete existing alerts by clicking on the modify action from the list of alerts&#x20;

You can delete an alert group (all alerts that are part of the group) from the “delete group” button from the list of alerts.

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

**View by level**&#x20;

The “My alerts” tab lists down alerts created by you with the following information and options, grouped by the level of alerts&#x20;

Like group name view, you can sort and filter the list of alerts. By default, they will be sorted by ascending order of level without any filters&#x20;

Unlike the group name view, you can only modify an alert. You will, however, not be able to delete an alert or an alert group from the level view of the list&#x20;

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

## Team alerts

The team alerts tab displays the list of alerts that other users have set for you. If no alert has been set by others, then they will be displayed an empty screen. &#x20;

Alerts set by others will be displayed with the following information under the “Team alerts” section. &#x20;

You will have the option to sort and filter the list of team alerts. By default, the sorting will be on ascending order of group name and no filters will be applied. &#x20;

You can also enable/disable alerts from the list.

<figure><img src="../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

## Alert history

The alert history tab lists all received alerts for the specified date range.  If no alerts have been received for the specified date range, then you will be displayed an empty screen.&#x20;

If you received alerts for the specified date range, then you will be displayed the list of alerts with the following information.&#x20;

You can sort and filter the list of received alerts. By default, the alerts will be sorted on descending order of start time and no filters will be applied.&#x20;

Whenever there are new alerts, then a “Load new alerts” button will be available to you, through which they can sync alerts and update their alerts history to the latest.&#x20;

<figure><img src="../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

## Alert notifications

Whenever an alert is triggered, then all recipient you will get: &#x20;

1. An in-app notification (if configured)&#x20;
2. SMS (if configured)
3. Email (if configured)

<figure><img src="../.gitbook/assets/image (40).png" alt=""><figcaption><p>In-app notification</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (41).png" alt=""><figcaption><p>Email</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (42).png" alt="" width="188"><figcaption><p>SMS</p></figcaption></figure>
