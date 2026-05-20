---
description: >-
  Set up or update your production line in minutes - without navigating complex
  UI workflows
icon: briefcase
---

# Basic Configuration

<details>

<summary>🧭 <strong>Why We Built Excel based Configuration Manager</strong></summary>

Every production line has its own story.

Some lines stay stable for years. Others evolve every week - especially during commissioning, pilot runs, ramp-ups, or customer-specific deployments.

For a long time, configuring these changes meant working through multiple UI screens, manually entering mappings, and carefully rebuilding structures one step at a time.

While this worked for stable environments, it created real challenges when lines changed frequently:

* Configuration took longer than expected
* Small manual mistakes could lead to rework
* Rebuilding existing structures for small changes felt unnecessary
* Engineers often preferred working offline before applying changes

We heard this feedback repeatedly from configurators, system integrators, and commissioning teams working on live shop floors.

That led to an important question:

> **What if configuring a production line felt as natural as editing a structured engineering file?**

That question became the foundation of Configuration Manager.

### What Changed

Instead of forcing every change through rigid UI workflows, Configuration Manager introduces an Excel-based approach that allows you to:

* Build line structures faster
* Make targeted updates without rebuilding everything
* Validate changes before anything goes live
* Work offline and upload when ready
* Keep existing production lines safe while making changes

### What We’re Trying to Improve

At its core, this module is designed to solve one thing:

> **Help configurators make changes with confidence - even in fast-changing production environments.**

Whether you're setting up a new line, updating PLC mappings, or making last-minute ramp-up changes, the goal is simple:

**Less manual effort. Fewer errors. Faster configuration.**

</details>

## Overview

Configuration Manager lets you define your line structure, map PLC tags, and apply targeted updates through a validated two-tab Excel template. The system handles all backend writes atomically — nothing is applied until every row passes validation.

{% hint style="info" icon="user" %}
<mark style="color:$warning;">**Who can use this feature?**</mark>

All users at the below role levels:

* Application Super Admin
* Organization Admin
* Line Configurator
{% endhint %}

### Before You Start

> _Estimated setup time:_ 3–10 minutes (depending on line complexity)

Make sure you have:

1. Zone and Cell names for your production line
2. Asset names and types for each cell
3. Data Logger, OPC, and PLC details - exactly as they exist in the system (names must match the database)
4. Tag and Tag Address values - must match what is registered in the PLC mapping
5. Microsoft Excel installed
6. The correct Excel template (download from the UI - do not create your own)
7. Existing configuration file (if updating a live line)

{% hint style="info" icon="lightbulb-exclamation-on" %}
Updating an existing line? Download the current configuration first. It’s faster and safer.
{% endhint %}

## How This Workflow Is Designed

Production lines in active manufacturing environments change frequently - during ramp-up, commissioning, and customer-specific deployments. Making those changes through multiple UI screens is slow, error-prone, and difficult to track.

Configuration Manager replaces that with a file-based approach. You define your line structure and PLC mappings in a structured Excel file. The system validates every field before applying anything - and if something is wrong, it tells you exactly which row and what to fix.

Nothing is written to the backend until all validations pass. This means you can never end up with a partial or inconsistent configuration.

The Excel file has two tabs, completed in this order:

```
Tab 1: Line Builder         → Define your physical line structure
        ↓
Tab 2: Basic Configuration  → Map PLC tags to your assets
        ↓
Upload → Validate → Apply
```

You can re-upload at any time to make incremental changes. Only the rows you modify are updated - the rest of your configuration stays intact.

## Step 1: Choose Your Template

Start from the Configuration Manager UI.

| If you want to...       | Download...                |
| ----------------------- | -------------------------- |
| Create a new line       | **Mapping Template**       |
| Update an existing line | **Existing Configuration** |

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-07 112312.jpg" alt="Update an existing line - Click Download Existing button"><figcaption><p>Update an existing line - Click Download Existing button</p></figcaption></figure>

{% hint style="info" icon="lightbulb-exclamation-on" %}
Using the existing configuration as your starting point is always faster and safer when making changes to a live line.
{% endhint %}

## Step 2: Fill in Your Excel File

Your file contains **2 tabs**.

Complete both tabs before uploading.

## Tab 1 - Build Your Line Structure

This tab defines the physical structure of your production line - how zones, cells, and assets relate to each other.

#### What to fill in

<table><thead><tr><th width="162.5999755859375">Column</th><th width="169.60003662109375">Required?</th><th>What to enter</th></tr></thead><tbody><tr><td>Zone</td><td>Optional</td><td>Name of the production zone</td></tr><tr><td>Cell</td><td>Optional</td><td>Name of the cell within the zone</td></tr><tr><td>Asset_Name</td><td>Required</td><td>Unique name for each asset on the line</td></tr><tr><td>Asset_Type</td><td>Required</td><td>Must match one of the supported asset types</td></tr></tbody></table>

### Example

| Zone     | Cell    | Asset\_Name | Asset\_Type |
| -------- | ------- | ----------- | ----------- |
| Assembly | Cell\_1 | Robot\_01   | MACHINE     |

### Validation Rules - Line Builder

Before upload, make sure:

* None of the two tabs is empty
* Column headers are precisely as per the downloaded template / configuration excel file
* **Zone & Cell**
  * Maximum 100 characters
  * Use only:
    * Letters
    * Numbers
    * `_`
    * `-`
* **Asset Name**
  * Cannot be blank
  * Must be unique
  * Maximum 100 characters
  * Use only:
    * Letters
      * Numbers
      * `_`
      * `-`
* **Asset Type**
  * Must match one of the supported system values:
    * MACHINE
    * TRANSFER\_CONVEYOR
    * BUFFER\_CONVEYOR
    * H\_GANTRY
    * I\_GANTRY
    * BUFFER\_TROLLEY
    * MARKING\_MACHINE
    * PICK\_UP\_CONVEYOR

{% hint style="danger" %}
Asset\_Type must exactly match one of the values above. Any variation - including lowercase, extra spaces, or unsupported values - will cause the upload to fail
{% endhint %}

## Tab 2 - Configure PLC Mapping

This tab connects your line structure to PLC data.

You’ll define:

* PLC details
* OPC details
* Tags
* Tag addresses
* Artifacts
* Data types

### Required System Fields

These values must already exist in the system:

* DataLogger\_Name
* OPC\_Name
* OPC\_IP\_Address
* PLC\_Name
* PLC\_IP\_Address

> These values are validated exactly as entered.

{% hint style="danger" %}
If even one value does not match, the upload will fail.
{% endhint %}

### Tag Validation

Each Tag is verified against your PLC mapping data.

The following must match:

* Tag
* Tag\_Address
* PLC\_Name

{% hint style="danger" %}
If the tag does not exist in your PLC mapping data, the system will reject the upload.
{% endhint %}

### Asset Validation

The Asset\_Name and Asset\_Type must match the values used in the Line Builder tab.

> This ensures your structure and PLC mappings stay aligned.

## Step 3: Upload Your File

Once your Excel file is ready:

1. Open Configuration Manager
2. Click **Upload File**
3. Select your Excel file

<div><figure><img src="../../.gitbook/assets/Screenshot 2026-05-07 113342.jpg" alt=""><figcaption><p>First click on Upload Structure button</p></figcaption></figure> <figure><img src="../../.gitbook/assets/Screenshot 2026-05-07 113449.jpg" alt=""><figcaption><p>On the pop up, scroll down to again click on Upload Structure button</p></figcaption></figure></div>

We automatically validate:

* File format
* Required tabs
* Column headers
* Missing values
* Duplicate rows
* PLC mappings

> No changes are applied until all validations pass.

## Step 4: Fix Errors (If Needed)

If validation fails:

You’ll see:

* Total number of errors
* **Download Error Log** button

### What’s in the Error Log?

You’ll get back:

📥 Your original Excel file\
➕ With an additional **Errors** column

Each row explains exactly what needs to be fixed.

Example:

| Asset\_Name | Error                |
| ----------- | -------------------- |
| Robot\_01   | Duplicate Asset Name |

> Fix only the highlighted rows and upload again.

## Step 5: Apply Configuration

When validation succeeds:

Your configuration is saved safely.

#### What happens behind the scenes?

* All changes are applied together
* No partial updates
* Existing live lines stay protected

> If validation fails, nothing is changed.

This prevents broken or incomplete configurations.

## Step 6: Review Your Line

After upload, your line structure appears as a visual tree.

You can review:

* Zones
* Cells
* Assets
* PLC mappings

## Making Changes Later

You don’t need to rebuild everything.

The Configuration Manager supports incremental updates.

### Smart Asset Handling

If your PLC mapping includes a new asset that does not exist in the line structure:

The system automatically creates it.

> This reduces manual rework during ramp-up.

## Common Upload Errors

⚠️Avoid these mistakes:

* Empty tabs
* Missing column headers
* Duplicate rows
* Unsupported Asset Types
* Invalid PLC or OPC values
* Tag mismatch with PLC mapping

## Best Practices

To avoid upload issues:

#### For New Lines

Start with a blank template.

#### For Existing Lines

Always download the current configuration first.

#### During Testing

Make smaller changes first.

Validate often.

#### Naming

Keep naming consistent across:

* Assets
* PLCs
* Tags

This reduces validation failures.

## Current Limitations

✅ The Configuration Manager currently supports:

* Excel uploads only
* Shallow line-level configuration

❌ Not supported:

* PLC code changes
* CSV uploads
* JSON uploads
* XML uploads
* Deep configuration flows

## Need Help?

If your upload keeps failing:

1. Download the error log
2. Fix highlighted rows
3. Re-upload

Still stuck? Contact your system administrator with the error file.

### What Happens Next?

Once your upload succeeds, your production line is ready for validation and deployment.
