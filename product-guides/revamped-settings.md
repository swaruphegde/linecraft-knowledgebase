---
hidden: true
---

# Revamped Settings

{% hint style="info" %}
**Navigation Path:**\
\
Main Menu → Settings\
Top Nav Bar → Settings
{% endhint %}

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

### `Profile`

The **Profile** tab allows users to manage personal account information. The **Profile** tab is the default landing page when a user accesses the Settings module.

<figure><img src="../.gitbook/assets/Knowledgebase Settings (1).gif" alt=""><figcaption></figcaption></figure>

#### Capabilities

* View personal details
* Edit profile information
* Change account password

#### Edit Personal Information

Click **Edit** in the Personal Information section to open a popup.

**Editable fields:**

* Name
* Phone number

Changes are applied immediately after saving.

#### Password Management

Users can update their password from this tab.\
Password changes take effect immediately and apply across all sessions.

***

### `Preferences`

The **Preferences** tab allows users to customize system behavior for their account.

Preferences are **user‑specific** and do not affect other users.

#### Time Preferences

Users can configure how time values are displayed across the product.

**Available options:**

* Default
* Seconds
* HH:MM:SS

Clicking the field opens a dropdown with the available options.\
Changes are applied immediately.

***

### `Shifts`

The **Shifts** tab is used to define operational shift structures for production tracking and reporting.

#### Default Shift Group

* A default shift group exists when users first visit this page
* Created during initial system configuration
* If only one shift group exists:
  * It cannot be deleted
  * It cannot be unset as default

#### Shift Group Actions

Each shift group supports:

1. Mark as Default Shift Group
2. Edit Shift Group Name
3. Delete Shift Group\
   &#xNAN;_(Available only when more than one shift group exists)_

#### Creating a Shift Group

Click **Add Shift Group** to create a new shift group.

**Rules and behavior:**

* Shift Group Name is mandatory
* Breadcrumbs display the navigation path
* One shift is added by default
* Start Time and End Time default to `00:00`
* **Create Shift Group** button remains disabled until all required fields are filled

#### Adding Shifts

* Click **Add Shift** or **Add Another Shift**
* Multiple shifts can be added
* Delete icon appears once more than one shift exists

#### Adding Breaks

* Click **Add Break** within a shift
* Multiple breaks can be added per shift

#### Viewing and Editing Shifts

* Shifts are displayed in a table
* Hovering over a shift row shows **Edit** and **Delete** actions
* Clicking a shift row expands it to show breaks
* Shifts and breaks can be edited inline

***

### `Targets`

The **Targets** tab allows users to configure production targets for each part type.

#### Overview

* Targets are configured part‑type wise
* Unit of measurement: **JPH (Jobs Per Hour)**

#### Target List View

Each target row displays:

* Part Type
* Target value (JPH)
* Last Updated timestamp

#### Managing Targets

* Hover over a target row to edit or delete
* Click **Add Targets** to define a new target

#### Add / Edit Target

**Fields:**

1. Part Type
2. Target (JPH)

If a target already exists for a part type, the new value overwrites the existing one.

***

### `Fault Code Mapping`

The **Fault Code Mapping** tab standardizes fault codes at an asset level.

#### Asset List Behavior

* Assets are listed alphabetically
* **Non‑mapped assets**:
  * Always appear at the top
  * Display an information (`i`) icon
  * Show a tooltip indicating unmapped status
* Tooltip shows the number of remaining unmapped assets

#### Mapping Rules

* Fault code mapping is asset‑specific
* Each asset maintains its own mapping sheet

#### Download Mapping Template

Users can download a standardized fault code mapping template.

**Template Link:**\
https://docs.google.com/spreadsheets/d/1ZSAUnQZDNtR\_dwNjZ9q1uBJGnv6g9PF6vHZwVXqHtuI/edit

#### Mapped Assets

Once an asset is mapped:

* **Last Updated On** timestamp is displayed
* Asset moves below non‑mapped assets
* Available actions:
  * Download Existing Mapping
  * Upload New Mappings

Downloaded file name format:\
`<Asset_Name> Fault Codes`

#### Uploading New Mappings

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

***

### `Loss Types`

The **Loss Types** tab allows users to configure production loss classifications.

#### Default Loss Types

* The product includes **16 preconfigured loss types**
* Default loss types can be edited or deleted

#### Creating a Loss Type

Click **Create Loss Type** to open the creation popup.

**Required fields:**

* Loss Type Name
* Description

The **Create** button remains disabled until both fields are filled.

#### System Behavior

* Loss type changes are reflected across analytics and reports
* Used for loss attribution and OEE calculations

***

### `Process Parameters`

The **Process Parameters** tab allows users with the **Configurator role** to view and edit IoT and Quality parameters.

#### Parameter List View

Parameters are displayed in descending order of **Updated At** with:

* Parameter Name
* Associated Part Type
* Associated Asset
* Parameter Type (IoT / Quality)
* Min Value
* Max Value
* Target Value
* Unit

#### Editing Parameters

Click the **Edit** icon to modify parameter values.

**Editable fields:**

* Min Value
* Max Value
* Target Value
* Unit

#### Validation Rules

* Min, Max, and Target:
  * Mandatory
  * Must be floating‑point numeric
* Unit and Aggregator:
  * Cannot be set to `none`
* Errors are shown for invalid or missing data
* Valid updates are saved and reflected immediately
