---
description: >-
  Upload logger files, validate your configuration, run data processing, and
  recover from failures - all from one place
---

# Data Processing

The Data Processing module helps you process production data safely while ensuring critical sanity checks are never skipped.

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

* Logger files ready (`.xml`)
* Configuration issues resolved
* Required production data available for the selected time range

## Understanding the two tabs - Logger Files & Data Processing

The Data Processing module is designed as **one connected workflow**, split into **two tabs**, each with a specific purpose.

This helps you work more efficiently while ensuring that the data processed in the system remains complete, consistent, and reliable.

***

### Tab 1 - Logger Files

This is where you prepare your raw data.

Use the **Logger Files** tab to:

✅ Upload one or more logger files (`.xml`)\
✅ Validate file format and file quality\
✅ Track uploaded files and upload status\
✅ Review file-level failures

***

### What happens after upload?

When a file upload succeeds:

1. The file is saved by the system
2. The raw data inside the file is automatically loaded into the database
3. That raw data becomes available for future data processing runs

> 💡 Once the raw data is loaded successfully, you do **not** need to upload the same files again unless the source data changes.

***

### Why is this a separate tab?

Separating file upload from processing gives you flexibility.

You can:

✅ Upload all required files upfront\
✅ Start processing later, whenever needed\
✅ Avoid re-uploading files if processing fails in later stages

### Important to know

The **Logger Files** table shows:

* File upload history
* File upload status
* File validation failures

It does **not** show the status of downstream data processing steps.

That status is shown in the **Data Processing** tab.

***

## Tab 2 - Data Processing

This is where you process already available raw data.

Use the **Data Processing** tab to:

✅ Select the date range\
✅ Select the machines\
✅ Run mandatory sanity checks\
✅ Start data processing\
✅ Monitor live progress\
✅ Resume failed runs

***

### Where does this data come from?

Data Processing always runs on raw data already available in the database.

That data may come from:

#### Option 1: Previously uploaded files

Files uploaded through the **Logger Files** tab.

***

#### Option 2: Existing historical data

If the required raw data is already present in the database, you can start processing immediately.

> 💡 This means uploading files is **not always required** before running Data Processing.

***

## How processing works

Once Data Processing starts:

The system automatically executes all required processing steps in the correct order.

You do not need to manually choose which internal steps to run.

This ensures:

✅ Required dependencies are always processed\
✅ No critical steps are accidentally skipped\
✅ Analytics always run on complete and validated data

***

## If processing fails

If a processing step fails:

Click:

**Re-run Data Processing**

You’ll see two options:

***

### Resume from dependent step _(Recommended)_

The system automatically identifies:

* Where processing stopped
* Which dependent steps need to run next

This helps you continue safely without reprocessing everything.

***

### Restart from first step

Use this when:

* Major configuration changes were made
* You want to run the full workflow again

***

> 💡 The system manages step dependencies for you, so you can focus on fixing the issue—not figuring out pipeline logic.

***

## Think of it this way

#### Logger Files = Prepare your data

```
Upload files → Raw data saved
```

***

#### Data Processing = Use your data

```
Select dates → Validate → Process → Review
```

***

Together, these two tabs give you:

✅ Flexibility in when you upload data\
✅ Confidence that all required processing steps are handled correctly\
✅ Faster recovery if processing fails

## Quick Start

To run data processing:

1. Upload your logger files
2. Select the date range
3. Select the machines
4. Configuration sanity checks run automatically
5. Data processing starts once configuration sanity checks pass
6. Monitor progress or resume if something fails

***

## Step 1: Upload Logger Files

Upload one or more logger files before processing begins.

Supported format:

* `.xml` only

Maximum file size:

* **30 MB per file**

You can upload:

* A single file
* Multiple files at once

***

### What happens after upload?

Each file is automatically checked for:

* File format
* File size
* Duplicate uploads
* Corrupted content
* Data consistency

If a file passes:

> It is uploaded and the data is loaded into the system.

If a file fails:

> You’ll see exactly where the validation failed.

***

### Example

Accepted:

```
machine_01.xmllogger_2026_05.xml
```

Rejected:

```
data.csvproduction.zip
```

***

## Step 2: Select Your Date Range

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

Date range must:

* Be within available raw data
* Not include future dates
* Be **30 days or less**

> ⚠️ If your selected range exceeds 30 days, processing will not start.

***

## Step 3: Select Machines

Choose which machines to process.

Default behavior:

> All machines are selected automatically.

You can deselect individual machines if needed.

***

### Rules

At least:

✅ 1 machine must remain selected

> ⚠️ If no machine is selected, processing cannot start.

***

## Step 4: Run Sanity Checks

Before data processing begins, the system automatically validates your configuration.

These checks are now **mandatory.**

No manual trigger required.

***

### Error Levels

#### 🔴 Error Checks

These block processing.

You must fix them before continuing.

Example:

* Missing machine configuration
* Invalid mapping
* Missing dependencies

***

#### 🟡 Warning Checks

These are shown to you, but do not block processing.

***

#### ℹ️ Information Checks

These are logged for visibility, but do not stop processing.

***

> 💡 This ensures critical issues are caught before expensive processing begins.

***

## Step 5: Start Data Processing

Once all blocking checks pass:

Processing starts automatically.

You’ll see:

* Live status updates
* Step-by-step progress
* Running subprocesses
* Failed steps (if any)

***

### Important

You can:

* Navigate to other screens
* Close the page and return later
* Continue monitoring from history

Your processing continues in the background.

***

## Tracking Progress

Each run shows:

* Trigger time
* Date range
* Selected machines
* Current status
* Number of reruns
* Total processing duration
* Initiator

***

### Status Types

#### 🟡 Running

Processing is active.

#### 🟢 Completed

Processing finished successfully.

#### 🔴 Failed

A step failed.

#### ⛔ Terminated

Processing was stopped manually or by the system.

***

## If Processing Fails

If a step fails:

The system stops automatically.

You’ll see:

* Which step failed
* Why it failed
* Troubleshooting guidance

This makes debugging faster and safer.

***

## Resume Processing

Once you fix the issue:

Click:

**Re-run Data Processing**

You’ll see 2 options:

#### Option 1: Resume from failed step _(recommended)_

Use this if you fixed a process issue.

***

#### Option 2: Start from first step

Use this only if:

You made configuration structure changes.

***

### Important

You cannot resume if:

❌ The process was manually terminated\
❌ More than 24 hours have passed since failure

***

## View Processing History

Every run is automatically logged.

You can see:

* When processing started
* Who started it
* How long it ran
* How many reruns happened
* Final status

***

### Why this matters

This helps you:

✅ Troubleshoot faster\
✅ Identify repeated failures\
✅ Audit past processing runs

***

## View Uploaded Files

The Logger Files tab shows:

* Upload date
* File name
* Logger details
* Time range
* Uploaded by
* Upload status

***

## Common Mistakes

Avoid these:

❌ Uploading non-XML files\
❌ Selecting future dates\
❌ Selecting more than 30 days\
❌ Starting overlapping processing for the same assets\
❌ Ignoring blocking sanity checks

***

## 💡 Pro Tips

#### For large factories

Start with fewer machines first.

This makes troubleshooting easier.

***

#### For failures

Always try:

**Resume from failed step**

before running everything again.

***

#### For recurring issues

Check your historical runs.

Repeated failures often point to configuration issues.

***

## Current Limits

Current limitations:

✅ Maximum file size: **30 MB**\
✅ Maximum date range: **30 days**\
✅ Only `.xml` files supported

***

## Need Help?

If processing keeps failing:

1. Open the failed step
2. Review the error details
3. Fix the configuration issue
4. Resume processing

Still stuck?

Contact your Linecraft administrator with the run ID.
