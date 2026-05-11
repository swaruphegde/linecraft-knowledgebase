# PSS 7.4.2

{% hint style="info" %}
Last PSS Version: 7.4.1

New PSS Version: 7.4.2
{% endhint %}

Release 7.4.2 introduces enhancements to the Configuration Manager focused on improving accuracy, flexibility, and efficiency in configuration workflows. This includes updates to the Excel template with stronger validations, simplified structure, and improved handling of nodes and inputs to reduce errors and streamline setup.

Additionally, this release introduces Standard and Non-Standard asset classification to improve part type assignment. The system now ensures correct mappings, prevents duplicates, and provides flexibility through manual overrides and Excel-driven controls.

The goal of these updates is to reduce configuration errors, improve data consistency, and enable more reliable and scalable configuration management.

## Key Configuration Improvements

### Ensuring Accurate Part Type Assignment with Standard & Non-Standard Asset Classification

These enhancements give configurators better control over how part types are assigned, improving accuracy and preventing incorrect mappings.

{% stepper %}
{% step %}
### **Standard Asset as Default**

* All assets are treated as _Standard_ by default.
* The system will continue to use existing mappings to assign part types wherever available.
* This ensures consistency with current configurations and avoids unnecessary changes.
{% endstep %}

{% step %}
### **Support for Non-Standard Assets**

* Users can now mark specific assets as _Non-Standard_ directly in Excel.
* For such assets, the system will always create a new part type instead of using existing mappings.
* This helps handle special cases where standard logic does not apply.
{% endstep %}

{% step %}
### **Avoidance of Incorrect Assignments**

* The system ensures the correct part type is assigned based on whether an asset is standard or non-standard.
* If no mapping exists for a standard asset, a new part type will be created automatically.
{% endstep %}

{% step %}
### **Prevention of Duplicate Part Types**

* The system intelligently avoids creating duplicate part types for the same configuration.
* Existing part types are reused whenever applicable.
{% endstep %}

{% step %}
### **Manual Override Capability**

* Configurators can manually assign or override part types when needed.
* These overrides are saved and reused in future configurations.
* All such changes are tracked for transparency and audit purposes.
{% endstep %}

{% step %}
### **Handling Special Machine Scenarios**

* Specific machines that do not follow standard mapping can be marked accordingly.
* The system will automatically apply the correct logic based on this selection.
{% endstep %}

{% step %}
### **Notifications for New Part Types**

* Whenever a new part type is created, configurators will receive a notification.
* This ensures visibility and control over configuration changes.
{% endstep %}

{% step %}
### **Excel Template Enhancements**

* A new column “Is Standard Asset?” has been added.
* Only valid inputs (Yes/No) are accepted to maintain data accuracy.
* Invalid or missing entries will be flagged during upload.
{% endstep %}

{% step %}
### **Backward Compatibility**

* Existing configurations remain unaffected.
* All current assets will continue to behave as standard unless explicitly updated.
{% endstep %}
{% endstepper %}

### **Use case showcasing all standard machine configurations:**

<figure><img src="../.gitbook/assets/Standard Machine Case.png" alt=""><figcaption></figcaption></figure>

### **Use case showcasing both standard and non-standard machine configurations:**

<figure><img src="../.gitbook/assets/Combined Machine Case.png" alt=""><figcaption></figcaption></figure>

### Configuration Manager – Excel Template Enhancements

These updates improve configuration accuracy, simplify usage, and support new business requirements:

{% stepper %}
{% step %}
### **Download Fix**

* Resolved issue where downloads were skipped due to blank system nodes created by the old UI.
* Download button is now enabled even when only cell and asset nodes exist with empty system/quality nodes.
{% endstep %}

{% step %}
### **Validation Improvements**

* Each asset must have:
  * 1 System node
  * 1 Quality node
* System node IO must contain:
  * 1 Enabler
  * 1 Disabler
{% endstep %}

{% step %}
### **Excel-Based Enable/Disable Control**

* Added support to configure enabler/disabler directly through Excel.
{% endstep %}

{% step %}
### **Node Configuration Enhancements**

* Config IO node naming for **Quality, Process, and Fault nodes** is now aligned with System node behavior.
{% endstep %}

{% step %}
### **Case Sensitivity Handling**

* Improved leniency for inputs in **Decoupled** and **Flipped** columns.
* Accepted formats include: `Yes`, `YES`, etc.
* Inputs are standardized automatically during upload and download.
{% endstep %}

{% step %}
### **Quality Node Updates**

* Added support for **Part Type IO marking** via Excel.
{% endstep %}

{% step %}
### **Template Simplification**

* Removed **Driver column** from the Excel template.
{% endstep %}

{% step %}
### **Zone Fault Node Handling**

* Zone fault node is now preserved during upload/download (same as Interface node behavior).
* Automatically adds a Zone fault node based on **Line Builder Sheet Zone column**, with **Segment 1 as parent**.
{% endstep %}

{% step %}
### **Data Model Changes**

* Removed **Zone-to-Cell mapping** from database (`TCellMaster`).
* Introduced **Zone-to-Asset mapping** in the Assets table.
{% endstep %}
{% endstepper %}
