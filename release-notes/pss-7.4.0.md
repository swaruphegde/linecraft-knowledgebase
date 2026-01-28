# PSS 7.4.0

{% hint style="info" %}
Last PSS Version: 7.3.0&#x20;

New PSS Version: 7.4.0&#x20;
{% endhint %}

We’re excited to roll out powerful updates that elevate visibility, intelligence, and control across production operations. The new **Critical Machines Report** and **revamped Production Report** deliver sharper insights for smarter, data-driven performance tracking. As part of **Machine Monitoring** module, we are introducing **Cycle Insights** which provides state-level visibility, enabling proactive optimization through intelligent analytics. Plus, the **all-new Linecraft Administration Application** streamlines management with enhanced security and seamless control.

## Features and improvements

#### Critical Machines Report

Introducing a new report template, _Critical Machine Report_ to identify top critical machines based on self-performance. This helps optimize ramp-up lines for better design and output and address bottlenecks and quality issues on existing lines

<figure><img src="../.gitbook/assets/image (153).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (154).png" alt=""><figcaption></figcaption></figure>

#### Revamped Production Report

Launching a more interactive and insights-driven production report to support better decision-making and performance tracking.

**Key features include:**

1. **Production KPIs:** Overall production, EOL on-shift good and bad parts, total unplanned production (EOL), unplanned good and bad parts (EOL), total line-level rejections, on-shift line-level rejections, unplanned line-level rejections and on-shift JPH
2. **Production breakdown:** On-shift, by-shift and by part type
3. **Top 5 critical machines** based on part loss

<figure><img src="../.gitbook/assets/image (155).png" alt=""><figcaption></figcaption></figure>

#### **Machine monitoring: Cycle insights (Auto-analysis)**

We've introduced **Auto analysis**, a powerful machine learning driven feature within **Cycle insights** that automatically analyses production cycles to uncover key patterns and detect anomalies. With this new capability, users can:

1. **Understand typical machine behavior** over selected time ranges
2. **Identify deviations** and problematic states in production cycles
3. **Gain actionable insights** to improve efficiency and support better operational decisions

This enhancement empowers teams to move from reactive monitoring to proactive optimization through data-driven analysis.

<figure><img src="../.gitbook/assets/image (156).png" alt=""><figcaption></figcaption></figure>

#### Andon dashboard enhancements

Added capabilities to configure line visibility, update project status, adjust activation dates, customize landing page logos, modify full-line name display and rearrange project rankings for improved control and usability

<figure><img src="../.gitbook/assets/image (157).png" alt=""><figcaption></figcaption></figure>

#### Configurator visibility in reports

Now recipients can view the configurator who set up a report, ensuring better visibility into configurations and preventing duplicates or mismatches

<figure><img src="../.gitbook/assets/image (159).png" alt=""><figcaption></figcaption></figure>

#### Machine monitoring enhancements

Improved visibility into machine states (Running, idle, down) along with clear insights into individual machine utilization and performance metrics

<figure><img src="../.gitbook/assets/image (160).png" alt=""><figcaption></figcaption></figure>

#### Improved part type detection logic

Improved new part type detection logic to avoid creating duplicate part types

#### Auto addition of dummy quality nodes for lines where quality information is not required

Default addition of dummy quality nodes is provisioned for the projects where quality data is not available. This is to keep configuration consistent across projects and avoid data processing failure.&#x20;

#### Application administration

The **Linecraft Administration Application** provides a centralized platform for administrators to manage user access, create and control production lines and oversee user management with enhanced security and flexibility

<figure><img src="../.gitbook/assets/image (161).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (162).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (163).png" alt=""><figcaption></figcaption></figure>

#### Auto run DP from node states to update critical machines' data

The system now automatically reprocesses data from node states whenever production schedule shifts are modified. This enhacement ensures that any changes in shift configurations are accurately reflected across all critical machine data, maintaining consistency and reliability in production insights.

#### Display "No Mode" as downtime reason in specific transitions

Enhanced the fault mechanism to display "No Mode" as the downtime reason when Auto mode is off, manual mode is off and no error or fault code is received so that the system accurately reflects the machine's state for safety and traceability
