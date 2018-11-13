---
description: This article describes two features which provide advanced functionality for Audience Lab  Duplicate Allocation Template and Segment Holdout.
seo-description: This article describes two features which provide advanced functionality for Audience Lab  Duplicate Allocation Template and Segment Holdout.
seo-title: Audience Lab Advanced Functionality
solution: Audience Manager
title: Audience Lab Advanced Functionality
uuid: 7c438ca7-9595-4b00-a6b4-621efaad1718
index: y
internal: n
snippet: y
---

# Audience Lab Advanced Functionality{#audience-lab-advanced-functionality}

This article describes two features which provide advanced functionality for Audience Lab: Duplicate Allocation Template and Segment Holdout.

On this page:

<ul class="simplelist"> 
 <li> <a href="../../c-features/audience-lab/audience-lab-advanced.md#section_520626580ECB48C9A6EFEFC9A5D49D1B" format="dita" scope="local"> Duplicate Allocation Template </a> </li> 
 <li> <a href="../../c-features/audience-lab/audience-lab-advanced.md#section_1D72DBA56C2F44ADB38B1BF86A300098" format="dita" scope="local"> Test Segment Holdout </a> </li> 
</ul>

## Duplicate Allocation Template {#section_520626580ECB48C9A6EFEFC9A5D49D1B}

**Overview**

<!-- 

<p>The <b>Allocation Template</b> represents how you split a test group into test segments and the way the test segments are mapped to destinations. </p>

 -->

In Audience Lab, the **Allocation Template** represents the various selections you make when creating a test group:

* The distribution of devices between test segments; 
* The mapping of test segments to destinations; 
* The conversion trait(s) you use for a test group; 
* The date range in which the test group publishes to your selected destinations.

By duplicating an allocation template, you can reuse the same distribution of test segments and destinations for a different base segment, in a new test group. An example of an allocation template is illustrated below.

![](assets/allocation_template_3.png)

<!-- 

With the option to duplicate allocation templates, you can increase your productivity when running multivariate tests as part of multivariate campaigns.

 -->

Create an initial test group, then select **[!UICONTROL Duplicate Allocation Template]** to reuse the same settings across multiple test groups. For example, you can use this feature if you're running a test where you want to determine the efficacy of several destinations for multiple segments.

**How to Use**

1. In the Audience Lab main view, search for the test group whose allocation template you want to reproduce in a new test group. In the drop-down box, select **[!UICONTROL Duplicate Allocation Template]**.

   ![](assets/duplicate-allocation-template.png)

1. In the [Create Test Group](../../c-features/audience-lab/audience-lab-manage-test-groups.md#task_B62EF6D2992941FAAEA84BE2EA11A55E) wizard, you can specify a base segment and rename your test segments, if you wish. 
1. You *cannot* modify:

    * The distribution of devices between test segments; 
    * The conversion trait(s); 
    * The mapping of test segments to destinations. You can only fill in the mapping key, for the destinations that require one. 
    * The date range in which your test group will publish to your selected destinations.

1. Review the information you added in the previous steps and select **[!UICONTROL Finalize Group]**.

## Test Segment Holdout {#section_1D72DBA56C2F44ADB38B1BF86A300098}

>[!NOTE]
>
>Test Segment Holdout is an advanced functionality, activated on customer request. Please contact Customer Care or Adobe Consulting to activate this feature.

**Overview**

Use this feature to shave the audience you are testing by a certain percentage. The percentage you select is left out of the test. This way, you can measure and compare the number of conversions from targeted (activated on destinations) and untargeted (holdout group) audiences.

<!-- 

<p>Note that this option is different to the control segment because it subtracts the percentage ................. You can withhold an audience group and still use a control segment. </p>

 -->

**How to Use**

1. Create a new test group by using the [Create Test Group](../../c-features/audience-lab/audience-lab-manage-test-groups.md#task_B62EF6D2992941FAAEA84BE2EA11A55E) wizard. 
1. In the **[!UICONTROL Allocate Test Segment]** step, you can select a part of the audience to be withheld from testing.

   ![List Item](assets/test-segment-holdout.png)

1. Use the slider to adjust how many devices you want to hold out from testing. Notice how Test Segment 1 and Test Segment 2 now only make out 70% of the total devices.

   ![](assets/test-segment-holdout-selected.png)

1. Go through the rest of the steps in the **[!UICONTROL Create Test Group]** workflow and select **[!UICONTROL Finalize Group]** when you're satisfied with your selection.
