# PSS 7.4.2

## Key Configuration Improvements

### Ensuring Accurate Part Type Assignment with Standard & Non-Standard Asset Classification

These enhancements give configurators better control over how part types are assigned, improving accuracy and preventing incorrect mappings.

1. **Standard Asset as Default**
   * All assets are treated as _Standard_ by default.
   * The system will continue to use existing mappings to assign part types wherever available.
   * This ensures consistency with current configurations and avoids unnecessary changes.
2. **Support for Non-Standard Assets**
   * Users can now mark specific assets as _Non-Standard_ directly in Excel.
   * For such assets, the system will always create a new part type instead of using existing mappings.
   * This helps handle special cases where standard logic does not apply.
3. **Avoidance of Incorrect Assignments**
   * The system ensures the correct part type is assigned based on whether an asset is standard or non-standard.
   * If no mapping exists for a standard asset, a new part type will be created automatically.
4. **Prevention of Duplicate Part Types**
   * The system intelligently avoids creating duplicate part types for the same configuration.
   * Existing part types are reused whenever applicable.
5. **Manual Override Capability**
   * Configurators can manually assign or override part types when needed.
   * These overrides are saved and reused in future configurations.
   * All such changes are tracked for transparency and audit purposes.
6. **Handling Special Machine Scenarios**
   * Specific machines that do not follow standard mapping can be marked accordingly.
   * The system will automatically apply the correct logic based on this selection.
7. **Notifications for New Part Types**
   * Whenever a new part type is created, configurators will receive a notification.
   * This ensures visibility and control over configuration changes.
8. **Excel Template Enhancements**
   * A new column “Is Standard Asset?” has been added.
   * Only valid inputs (Yes/No) are accepted to maintain data accuracy.
   * Invalid or missing entries will be flagged during upload.
9. **Backward Compatibility**
   * Existing configurations remain unaffected.
   * All current assets will continue to behave as standard unless explicitly updated.

### Configuration Manager – Excel Template Enhancements

These updates improve configuration accuracy, simplify usage, and support new business requirements:

1. **Improved Download Experience**
   * Fixed issues that previously blocked downloads in certain scenarios.
   * Users can now download configurations even when minimal data is present.
2. **Stronger Data Validation**
   * Ensures every asset is properly structured with required components.
   * Prevents incomplete or inconsistent configurations during upload.
3. **Excel-Driven Controls**
   * Key configuration controls (enable/disable) can now be managed directly through Excel for faster updates.
4. **Consistent Naming Across Configurations**
   * Standardized naming behavior across different configuration elements for better clarity and uniformity.
5. **Flexible Input Handling**
   * Reduced dependency on exact text formats (e.g., “Yes” vs “YES”).
   * System now automatically standardizes inputs to avoid errors.
6. **Enhanced Quality Configuration**
   * Added support for defining part-related settings directly within Excel.
7. **Simplified Template**
   * Removed unnecessary fields to make the Excel template cleaner and easier to use.
8. **Improved Zone Handling**
   * Zone-related configurations are now more stable and consistent during upload and download.
   * Automatic setup of zone-related structures reduces manual effort.
9. **Optimized Data Model**
   * Streamlined how zone information is stored and linked, improving system efficiency and scalability.
