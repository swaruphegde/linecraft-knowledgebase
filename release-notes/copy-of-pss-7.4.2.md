---
hidden: true
---

# Copy of PSS 7.4.2

{% hint style="info" %}
Last PSS Version: 7.4.2

New PSS Version: 7.5.0
{% endhint %}

We are excited to announce the release of **PSS 7.5.0**, focused on modernizing user workflows, centralizing deployment orchestration, ensuring reporting consistency, and boosting data processing speed.

This release debuts a **revamped Settings module** with our updated design system and integrated IoT/quality parameter management. In configuration management, we introduced a **unified on-demand Data Processing pipeline** with enforced sanity validation, alongside an **all-in-one Deployment Setup interface** featuring native PLC backup parsing and one-click package exports.

We have also added **Configurable End of Line (EOL) asset marking** to guarantee accurate production counts across all platform views, while targeted optimizations accelerate cycle computation times across high-volume pipelines.

## Features and Improvements

### Revamped Settings module

The Settings module has been completey re-architected with our modern design system, improving everyday usability and visual clarity while retaining full backward compatibility with existing configurations.

#### Key highlights:

{% stepper %}
{% step %}
### Refreshed navigation and interface

A streamlined, responsive layout that unifies configuration administration under a cleaner visual hierarchy.
{% endstep %}

{% step %}
### Seamless functional migration

Centralized management for core operational parameters:

* **Shifts:** Manage shift schedules, operational windows, and planned breaks
* **Targets:** Configure and fine-tune line and asset-level production targets
* **Profile & Preferences:** Customize user profiles, viewing preferences, and notification defaults
* **Fault Code Mapping:** Map, inspect, and update PLC fault codes quickly.
{% endstep %}

{% step %}
### IoT and Quality Parameter management

A dedicated settings workspace to define and maintain IoT ingest parameters and quality thresholds directly within the platform.
{% endstep %}
{% endstepper %}

### Unified on-demand Data Processing and Sanity Checks

We have merged the legacy _Bulk Data Processing_ and _Model Configuration_ modules into a unified **Data Processing** workspace inside **Config Manager** module. This redesign enforces data integrity at every milestone while eliminating guesswork during processing runs.

#### Key highlights:

{% stepper %}
{% step %}
### Guided execution pipeline

* **Automated file pre-validation:** Data files uploaded for processing are instantly validated against file structure guidelines and baseline sanity rules prior to database loading.
* **Gated pre-processing checks:** Enforces resolution of critical "Error" level configuration sanity checks before data processing can begin, preventing broken runs downstream.
* **Extended processing windows:** Select and process up to 30 continuous days of historical operational data in a single run (with future dates safeguarded).
* **Targeted asset scope:** Run processing across all assets by default, or isolate specific machines for rapid iteration.
{% endstep %}

{% step %}
### Automated sanity verification

Runs data integrity sanity checks automatically and if a step fails, processing halts at the exact failure point. Intermediate database commits allow any authorized user to resume execution seamlessly from the failed step once configurations are corrected.
{% endstep %}

{% step %}
### Live progress tracking & thread logs


{% endstep %}
{% endstepper %}

