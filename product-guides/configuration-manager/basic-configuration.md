---
description: >-
  Set up or update your production line in minutes - without navigating complex
  UI workflows
icon: briefcase
---

# Basic Configuration

<details>

<summary><strong>Why We Built Configuration Manager</strong></summary>

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

***

### What Changed

Instead of forcing every change through rigid UI workflows, Configuration Manager introduces an Excel-based approach that allows you to:

* Build line structures faster
* Make targeted updates without rebuilding everything
* Validate changes before anything goes live
* Work offline and upload when ready
* Keep existing production lines safe while making changes

***

### What We’re Trying to Improve

At its core, this module is designed to solve one thing:

> **Help configurators make changes with confidence - even in fast-changing production environments.**

Whether you're setting up a new line, updating PLC mappings, or making last-minute ramp-up changes, the goal is simple:

**Less manual effort. Fewer errors. Faster configuration.**

</details>

The Basic Configuration under Configuration Manager lets you build your line structure, map PLC tags, and apply updates using a simple Excel file

{% hint style="info" icon="user" %}
<mark style="color:$warning;">**Who can use this feature?**</mark>

All users at the below role levels:

* Application Super Admin
* Organization Admin
* Line Configurator
{% endhint %}

## On this page

#### Getting Started

* [Before You Start](https://app.gitbook.com/o/pDAf3FQPWhPdFwj4FuIf/s/y2Me4Kn6229fD3kXS68B/~/edit/~/changes/144/product-guides/configuration-manager/basic-configuration#before-you-start)
* [Choose Your Template](https://app.gitbook.com/o/pDAf3FQPWhPdFwj4FuIf/s/y2Me4Kn6229fD3kXS68B/~/edit/~/changes/144/product-guides/configuration-manager/basic-configuration#step-1-choose-your-template)

#### Creating a Configuration

* [Build Your Line Structure](https://app.gitbook.com/o/pDAf3FQPWhPdFwj4FuIf/s/y2Me4Kn6229fD3kXS68B/~/edit/~/changes/144/product-guides/configuration-manager/basic-configuration#tab-1-build-your-line-structure)
* [Validation Rules - Line Builder](basic-configuration.md#validation-rules-line-builder)
* [Configure PLC Mapping](https://app.gitbook.com/o/pDAf3FQPWhPdFwj4FuIf/s/y2Me4Kn6229fD3kXS68B/~/edit/~/changes/144/product-guides/configuration-manager/basic-configuration#tab-2-configure-plc-mapping)
* [Upload Your File](https://app.gitbook.com/o/pDAf3FQPWhPdFwj4FuIf/s/y2Me4Kn6229fD3kXS68B/~/edit/~/changes/144/product-guides/configuration-manager/basic-configuration#step-3-upload-your-file)

#### Troubleshooting

* [Fix Upload Errors](https://app.gitbook.com/o/pDAf3FQPWhPdFwj4FuIf/s/y2Me4Kn6229fD3kXS68B/~/edit/~/changes/144/product-guides/configuration-manager/basic-configuration#step-4-fix-errors-if-needed)
* [Common Upload Errors](https://app.gitbook.com/o/pDAf3FQPWhPdFwj4FuIf/s/y2Me4Kn6229fD3kXS68B/~/edit/~/changes/144/product-guides/configuration-manager/basic-configuration#common-upload-errors)

#### Reference

* [Best Practices](https://app.gitbook.com/o/pDAf3FQPWhPdFwj4FuIf/s/y2Me4Kn6229fD3kXS68B/~/edit/~/changes/144/product-guides/configuration-manager/basic-configuration#best-practices)
* [Current Limitations](https://app.gitbook.com/o/pDAf3FQPWhPdFwj4FuIf/s/y2Me4Kn6229fD3kXS68B/~/edit/~/changes/144/product-guides/configuration-manager/basic-configuration#current-limitations)

### ⏱ Before You Start

Estimated setup time: **3–5 minutes**

Make sure you have:

* [ ] Access to the production line
* [ ] PLC mapping details (if configuring tags)
* [ ] Microsoft Excel installed
* [ ] Existing configuration file (if updating a live line)

{% hint style="info" icon="lightbulb-exclamation-on" %}
Updating an existing line? Download the current configuration first. It’s faster and safer.
{% endhint %}

## Step 1: Choose Your Template

Start by downloading the correct Excel file.

| If you want to...       | Download                   |
| ----------------------- | -------------------------- |
| Create a new line       | **Mapping Template**       |
| Update an existing line | **Existing Configuration** |

{% hint style="info" icon="lightbulb-exclamation-on" %}
We recommend using the existing configuration when making changes to a live line.
{% endhint %}

## Step 2: Fill in Your Excel File

Your file contains **2 tabs**.

Complete both tabs before uploading.

## Tab 1 - Build Your Line Structure

This tab defines your physical production line.

You’ll configure:

* **Zone** → Optional grouping (for example: Assembly Zone)
* **Cell** → Optional sub-grouping (for example: Welding Cell)
* **Asset\_Name** → The machine or equipment name
* **Asset\_Type** → Type of equipment

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
If Asset Type is invalid, the upload will fail and your line structure will not be created.
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

👎Avoid these mistakes:

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
