---
description: >-
  Set up or update your production line in minutes - without navigating complex
  UI workflows
icon: briefcase
---

# Basic Configuration

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

## Tab 2 - Configure PLC Mapping

This tab connects your line structure to PLC data.

You’ll define:

* PLC details
* OPC details
* Tags
* Tag addresses
* Artifacts
* Data types

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

## Step 5: Apply Configuration

When validation succeeds:

Your configuration is saved safely.

#### What happens behind the scenes?

* All changes are applied together
* No partial updates
* Existing live lines stay protected

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

***

#### For Existing Lines

Always download the current configuration first.

***

#### During Testing

Make smaller changes first.

Validate often.

***

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
