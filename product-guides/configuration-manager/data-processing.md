---
description: >-
  Process production data safely - without worrying about missing steps, broken
  dependencies, or restarting from scratch.
---

# Data Processing

The Data Processing module helps you upload logger files, validate your configuration, process production data, and recover from failures - all from one place.

{% hint style="info" icon="user" %}
<mark style="color:$warning;">**Who can use this feature?**</mark>

All users at the below role levels:

* Application Super Admin
* Organization Admin
* Line Configurator
{% endhint %}

## ⏱ Before You Start

Estimated time: **5–10 minutes**

Make sure you have:

* Logger files ready (`.xml`) _if new raw data needs to be added_
* Configuration issues resolved
* Required production data available for the selected time range

{% hint style="info" icon="lightbulb-on" %}
If the required raw data already exists in the system, you can directly start Data Processing without uploading files
{% endhint %}

## Understanding the Workflow

The Data Processing module is split into **two connected tabs**, each with a specific purpose.

Together, they form one complete workflow.

***

### Tab 1 - Logger Files

Use this tab when you want to add new raw production data into the system.

#### What you can do here

* Upload one or more logger files (`.xml`)
* Validate file format and file quality
* Track upload status
* Review upload failures

***

### What happens after upload?

When a file upload succeeds:

1. The file is saved by the system
2. The raw data inside the file is automatically loaded into the database
3. That raw data becomes available for future processing runs

> 💡 Once raw data is loaded successfully, you do not need to upload the same files again unless the source data changes.

***

### Important to know

The **Logger Files** tab shows:

* Upload history
* Upload status
* File-level failures

It does **not** show downstream processing progress.

That status is shown in the **Data Processing** tab.

***

### Why is this separate?

This gives you flexibility.

You can:

* Upload all files upfront
* Start processing later
* Avoid re-uploading files if processing fails later

***

## Tab 2 - Data Processing

Use this tab to process raw data already available in the system.

This raw data may come from:

#### Previously uploaded files

Uploaded through the **Logger Files** tab.

***

#### Existing raw data

If data is already available in the database, you can start processing immediately.

***

### What happens when processing starts?

The system automatically runs:

1. Pre-processing sanity checks
2. All required processing steps
3. Step-level validations during processing

You do not need to manually select individual steps.

This ensures:

* Required dependencies are always processed
* Critical steps are never skipped
* Analytics always run on complete and validated data

***

> 💡 The system manages processing dependencies for you—so you can focus on fixing issues, not figuring out pipeline logic.

***

## Quick Start

To run Data Processing:

1. Upload logger files _(only if new raw data is needed)_
2. Open **Data Processing**
3. Select the date range
4. Select the machines
5. Review sanity check results
6. Start processing

***

## Step 1: Upload Logger Files _(Optional)_

Supported file format:

* `.xml` only

Maximum file size:

* **30 MB per file**

You can upload:

* A single file
* Multiple files at once

***

### Files are automatically validated for:

* File format
* File size
* Duplicate uploads
* Corrupted content
* Data consistency

If a file passes:

> Raw data is loaded into the system automatically.

If a file fails:

> The failed step and error details are shown.

***

## Step 2: Select Date Range

Choose the time period you want to process.

Available presets:

* Today
* Yesterday
* Last 7 Days
* Last 30 Days
* This Month
* Last Month
* Custom Range

***

### Rules

Your selected range must:

* Be within available raw data
* Not include future dates
* Be **30 days or less**

***

## Step 3: Select Machines

By default:

> All machines are selected automatically.

You can deselect machines if needed.

***

### Rules

At least:

✅ 1 machine must remain selected

***

## Step 4: Run Sanity Checks

Before processing begins, the system automatically validates your configuration.

These checks are mandatory.

***

### Error Levels

#### 🔴 Error Checks

These block processing until fixed.

Examples:

* Missing machine configuration
* Invalid mapping
* Missing dependencies

***

#### 🟡 Warning Checks

Shown to you, but processing continues.

***

#### ℹ️ Information Checks

Logged for visibility, but do not block processing.

***

## Step 5: Start Data Processing

Once blocking checks pass:

Processing starts automatically.

The system:

* Runs in the background
* Saves progress after each completed step
* Allows safe recovery if a failure happens

You can:

* Navigate to other modules
* Close the page
* Return later and continue monitoring

***

## If Processing Fails

If a step fails:

Click:

**Re-run Data Processing**

***

### Option 1: Resume from dependent step _(Recommended)_

The system automatically identifies:

* Where processing stopped
* What dependent steps need to run next

***

### Option 2: Restart from first step

Use this if:

* Major configuration changes were made
* You want to rerun the full workflow

***

## Tracking Progress

Every run shows:

* Trigger time
* Date range
* Selected machines
* Current status
* Number of reruns
* Total duration
* Initiator

***

## Common Mistakes

❌ Avoid these:

* &#x20;Uploading non-XML files
* Running overlapping processing for the same machines and dates
* Ignoring blocking sanity checks

***

## Pro Tips

#### Working with large factories?

Start with fewer machines first.

This makes troubleshooting easier.

***

#### Processing failed?

Always try:

**Resume from dependent step**

before running everything again.

***

#### Seeing repeated failures?

Check your historical runs.

Repeated failures often point to configuration issues.

***

## Current Limits

Current system limits:

* Maximum file size: **30 MB**
* Maximum date range: **30 days**
* Only `.xml` files supported

***

## Need Help?

If processing keeps failing:

1. Open the failed step
2. Review the error details
3. Fix the issue
4. Resume processing

Still stuck?

Contact your Linecraft administrator with the run ID.
