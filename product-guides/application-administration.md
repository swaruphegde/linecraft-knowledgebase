# 🛡️ Application administration

**Overview**&#x20;

The Application Administration Module introduces a centralized, secure way to administer Linecraft at scale. The primary objective is to enable controlled onboarding of new customers and expansion for existing customers by empowering a dedicated Application Super Admin role to create and manage Organizations, Plants, Production Lines, Users, and Roles.&#x20;

This module is designed as an independent application within the Linecraft ecosystem and serves as the single source of truth for entity structure, role definitions, and user access management.&#x20;

**Key Features**&#x20;

* Organization, Plant, and Line creation & management&#x20;
* Role definition and enforcement (OOTB roles)&#x20;
* User creation, role assignment, and role changes&#x20;
* Entity-specific user management&#x20;
* Static role reference documentation within product&#x20;

**Line Management – Features**&#x20;

* Unified view of all existing lines with Org/Plant context&#x20;
* Ability to:&#x20;
* Add new Organization / Plant / Line&#x20;
* Navigate to line-specific configuration and dashboards (based on role)&#x20;

<figure><img src="../.gitbook/assets/unknown.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/unknown (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/unknown (2).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/unknown (3).png" alt=""><figcaption></figcaption></figure>

**Role Management**  \
Role Mode&#x20;

* Roles are predefined (OOTB)
* Roles are mapped at Line level, enabling granular access&#x20;

<figure><img src="../.gitbook/assets/unknown (4).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/unknown (5).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/unknown (6).png" alt=""><figcaption></figcaption></figure>

**Out-of-the-Box Roles**&#x20;

1\. **Application Super Admin (Linecraft Internal)**&#x20;

* Ownership: Linecraft only&#x20;
* Responsibilities:&#x20;
  * Create and manage Organizations, Plants, and Lines&#x20;
  * Add users and assign roles&#x20;
  * Modify user roles&#x20;
  * Grant or revoke access across entities&#x20;
* Restrictions:&#x20;
  * Strictly limited to authorized Linecraft users&#x20;

2\. **Enterprise Executive**&#x20;

* Access Scope:&#x20;
  * All lines under assigned Plant(s)&#x20;
* Permissions:&#x20;
  * Read-only access to all enabled modules as per subscription plan&#x20;
* Key Module:&#x20;
  * Enterprise Dashboard&#x20;
* Navigation Behavior:&#x20;
  * When selection = All Lines / Plant → Only Enterprise Dashboard visible&#x20;
  * When selection = Individual Line → Can access all read-only modules&#x20;

3\. **Line Configurator**&#x20;

* Access Scope:&#x20;
  * Assigned Line(s)&#x20;
* Permissions:&#x20;
  * Full access to all modules&#x20;
  * Full access to Configuration Manager&#x20;
* Primary Responsibilities:&#x20;
  * Line modelling&#x20;
  * Line configuration&#x20;
  * System setup and optimization&#x20;

4\. **Line Manager (OOTB)**&#x20;

* Access Scope:&#x20;
  * Assigned Line(s)&#x20;
* Permissions:&#x20;
  * Write access to most operational modules&#x20;
  * No access to Configuration Manager&#x20;
  * Read-only access to limited settings:&#x20;

5\. **Operator**&#x20;

* Access Scope:&#x20;
  * Assigned Line(s)&#x20;
* Permissions:&#x20;
  * Read-only access to key product modules&#x20;
* Restrictions:&#x20;
  * No access to Application Administration&#x20;
  * No access to Configuration Manager&#x20;

**Summary**&#x20;

The Application Administration Module establishes a robust foundation for secure, scalable, and governed access control in Linecraft. By introducing a dedicated Super Admin role, predefined enterprise roles, and entity-aware user management, the platform is well-positioned to support enterprise growth while maintaining operational clarity and security.&#x20;



&#x20;

&#x20;

&#x20;

&#x20;
