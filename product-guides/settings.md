# 🔩 Settings

<details>

<summary>About <strong>Settings Module</strong> </summary>

The **Settings** module allows users to configure system, operational, and personalization parameters required for effective use of the product.

From the Settings module, users can:

* Manage shifts and shift groups
* Configure production targets
* Update profile details and preferences
* Map fault codes to assets
* Configure loss types
* View and edit IoT and Quality parameters
* Sign out of the application

</details>

***

## `Profile`

The Profile section is where you keep your account information up to date. It opens by default whenever you land on Settings. Here, you can review your details, update your personal information, and change your password anytime.

### Edit Personal Information

<figure><img src="../.gitbook/assets/2026-04-15, 07_48_38 a.m.-Settings___Google_Chrome_Demo.gif" alt=""><figcaption></figcaption></figure>

Need to make a quick change? Just click Edit under Personal Information. You’ll be able to update your name and phone number, and your changes will reflect instantly once saved.

### Change Password

<figure><img src="../.gitbook/assets/image (174).png" alt=""><figcaption></figcaption></figure>

You can update your password directly from this tab. Once changed, it takes effect immediately across all your active sessions.

***

## `Preferences`

Preferences let you tailor how the system behaves for you. These settings are personal and  won’t affect anyone else.

### Time Preferences

Choose how time is displayed across the platform. You can switch between formats like standard view, seconds, or HH:MM:SS.\
\
Simply select your preferred option from the dropdown, and it will apply right away across the product.

<figure><img src="../.gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

***

## `Shifts`

The Shifts section helps you define how shift work hours are structured for production tracking and reporting.

### Default Shift Group

<figure><img src="../.gitbook/assets/image (177).png" alt=""><figcaption></figcaption></figure>

When you first visit, you’ll see a default shift group already set up during system configuration. If it’s the only one, it can’t be removed or changed as the default.

### Managing Shift Groups

<figure><img src="../.gitbook/assets/image (178).png" alt=""><figcaption></figcaption></figure>

You can:

* Rename a shift group
* Set a different one as default shift group
* Delete a shift group (only if more than one exists)

### Creating a Shift Group

Click **Add Shift Group** to create a new shift group.

<figure><img src="../.gitbook/assets/image (179).png" alt=""><figcaption></figcaption></figure>

You’ll be guided to:

* Enter a required name
* Add shifts (one is added by default)
* Define timings (starting and ending at 00:00 by default)

The Create button becomes active once all required details are filled.

### Adding Shifts and Breaks

You can easily build out your schedule by adding as many shifts as you need. Just click **Add Another Shift** to include more.

* While setting up shifts, make sure their timings don’t overlap. Once you have more than one shift, you’ll also see the option to remove any extra ones.
* Within each shift, you can add breaks to reflect downtime. Simply click **Add Break** inside a shift. Like shifts, break timings should not overlap, and you can add multiple breaks if needed.

### Viewing and Editing Shifts

<figure><img src="../.gitbook/assets/image (178).png" alt=""><figcaption></figcaption></figure>

Each shift is shown as an expandable section, so you can keep things organized.

Click on a shift to expand it and see more details. From there, you can:

* Update shift timings or details
* Delete the shift if needed
* Mark shift as off
* View and manage all associated breaks

This makes it easy to review and adjust your setup in one place without clutter.

***

## `Targets`

The **Targets** tab allows users to configure production targets for each part type.

<figure><img src="../.gitbook/assets/image (180).png" alt=""><figcaption></figcaption></figure>

#### Overview

* Targets are configured part‑type wise
* Unit of measurement: **JPH (Jobs Per Hour)**

#### Edit Target

<figure><img src="../.gitbook/assets/image (181).png" alt=""><figcaption></figcaption></figure>

**Fields:**

1. Part Type
2. Target (JPH)

If a target already exists for a part type, the new value overwrites the existing one.

***

## `Fault Code Mapping`

The **Fault Code Mapping** tab standardizes fault codes at an asset level.

<figure><img src="../.gitbook/assets/image (182).png" alt=""><figcaption></figcaption></figure>

#### Asset List Behavior

* Assets are listed alphabetically
* Tooltip at top shows the number of remaining unmapped assets
* Ignored assets will have “Ignored Asset” text below the asset name.
* **Non‑mapped assets**:
  * Always appear at the top
  * Display an information (`i`) icon which indicating unmapped status on hover

#### Mapping Rules

* Fault code mapping is asset‑specific
* Each asset maintains its own mapping sheet

#### Download Mapping Template

Users can download a standardized fault code mapping template.

#### Mapped Assets

Once an asset is mapped:

* **Last Updated On** timestamp is displayed
* Asset moves below non‑mapped assets
* Available actions:
  * Download Existing Mapping
  * Upload New Mappings

Downloaded file name format:\
`<Asset_Name> Fault Codes`

#### Uploading New Mappings and Bulk Uploads

**Upload options:**

* Single asset upload
* Bulk upload for multiple assets

**Rules:**

* At least one asset must be selected
* Upload without selection triggers an error
* Bulk upload is allowed even with one selected asset

#### Validation Checks

Uploaded sheets are validated for:

* Duplicate rows
* Numeric fault code values
* Empty or blank fields

Validation errors are displayed in an error popup.

<figure><img src="../.gitbook/assets/image (183).png" alt=""><figcaption></figcaption></figure>

Same applies for the Zone Mappings.&#x20;

***

## `Loss Types`

The **Loss Types** tab allows users to configure production loss classifications.

#### Default Loss Types

<figure><img src="../.gitbook/assets/image (184).png" alt=""><figcaption></figcaption></figure>

* The product includes **16 preconfigured loss types**
* Default loss types (loss type name and description) can be edited
* Each loss type name and description needs to be unique.

<figure><img src="../.gitbook/assets/image (187).png" alt=""><figcaption></figcaption></figure>

#### Creating a Loss Type

Click **Create Loss Type** to open the creation popup.

<figure><img src="../.gitbook/assets/image (186).png" alt=""><figcaption></figcaption></figure>

**Required fields:**

* Loss Type Name
* Description

The **Create** button remains disabled until both fields are filled.

#### System Behavior

* Loss type changes are reflected across analytics and reports
* Used for loss attribution

***

## `Process Parameters`

The **Process Parameters** tab allows users with the **Configurator role** to view and edit IoT and Quality parameters.

<figure><img src="../.gitbook/assets/No PLC Mapped.jpg" alt=""><figcaption></figcaption></figure>

#### Parameter List View

Parameters are displayed in descending order of **Updated At** with:

* Parameter Name
* Machine
* Part Type
* Min Value
* Max Value
* Target Value
* Unit
* Aggregator
* Parameter Type (IoT / Quality)

#### Editing Parameters

<figure><img src="../.gitbook/assets/No PLC Mapped (1).jpg" alt=""><figcaption></figcaption></figure>

Click the **Edit** icon to modify parameter values.

**Editable fields:**

* Min Value
* Max Value
* Target Value
* Unit
* Aggregator

#### Validation Rules

* Min, Max, and Target:
  * Mandatory
  * Must be floating‑point numeric
* Unit and Aggregator:
  * Cannot be set to none
* Errors are shown for invalid or missing data
* Valid updates are saved and reflected immediately
