---
description: To create a new data source, go to Audience Data > Data Sources > Add New and complete the steps for each section described here. Administrator permissions are required to create a data source.
keywords: cdf;custom data feed
seo-description: To create a new data source, go to Audience Data > Data Sources > Add New and complete the steps for each section described here. Administrator permissions are required to create a data source.
seo-title: Create a Data Source
solution: Audience Manager
title: Create a Data Source
uuid: b1ac265a-99b1-448a-a6c9-ce0e50994c80
index: y
internal: n
snippet: y
---

# Create a Data Source{#create-a-data-source}

To create a new data source, go to Audience Data > Data Sources > Add New and complete the steps for each section described here. Administrator permissions are required to create a data source.

## Create a Data Source {#concept_3B7696B3EC77416492D3B99EBD79EA44}

To create a new data source, go to **[!UICONTROL Audience Data > Data Sources > Add New]** and complete the steps for each section described here. Administrator permissions are required to create a data source.

<!-- 

create-datasource.xml

 -->

>[!TIP]
>
>See [Data Source Settings and Menu Options](../c-features/datasources-list-and-settings.md#reference_A87B381067E04C26A426514AF3B64E64) for descriptions of these different controls.

## Data Source Details {#section_D359CAAE0BEA4527B3A04855486033DE}

To complete the [!UICONTROL Data Source Details] section:

1. Name the data source. 
1. *(Optional)* Describe the data source. A concise description helps you define the role or purpose of the data source. 
1. Provide an integration code. Generally, integration codes are optional. They are required when you want to:

    * [Create a cross-device data source](../c-features/profile-merge-rules/merge-rules-start.md#concept_3B7696B3EC77416492D3B99EBD79EA44). 
    * Use the [Experience Cloud ID service](https://marketing.adobe.com/resources/help/en_US/mcvid/). 
    * Work with [Profile Merge Rules](../c-features/profile-merge-rules/merge-rules-start.md#concept_34A9CEA00B24447EBF7EA8DA2928E1DD).

1. Choose an **[!UICONTROL ID Type]**. ID Type options include:

    * **[!UICONTROL Cookie]** 
    * **[!UICONTROL Device Advertising ID]** 
    * **[!UICONTROL Cross-device]** (Required to create a [!UICONTROL Profile Merge Rule]). Note, for some customers, this selection exposes the **[!UICONTROL ID Definition]** options.

1. Choose an **[!UICONTROL ID Definition]** option. Options include:

    * **[!UICONTROL Person]** 
    * **[!UICONTROL Household]**

<!-- 

<p> 
 <note>
  Selecting 
  <span class="uicontrol"> Device Advertising ID</span> or 
  <span class="uicontrol"> Cross Device</span> limits the inbound ID options in the Data Source Settings section to 
  <span class="uicontrol"> Customer ID</span> only. 
 </note> </p>

 -->

## Data Export Controls {#section_895821268F6F42E9A181B717DD6F1D04}

[Data Export Controls](../c-features/data-export-controls.md#concept_155AAFBA7D804467B6F8279D26C9D05C) are optional classification rules you can apply to a data source and destination. They prevent you from sending data to a destination when that action violates a data privacy or use agreement. Skip this section if you do not use [!UICONTROL Data Export Controls].

## Data Source Settings {#section_928E1EB8EE7149A88F46ABD3B6FE5BAF}

These settings determine how a data source is identified, used, and shared. You can also enable error reporting for inbound data files. To complete the [!UICONTROL Data Source Settings] section:

1. Select a [!UICONTROL Data Source Setting] check box to apply an option to your data source. 
1. Click **[!UICONTROL Save]**.

>[!MORE_LIKE_THIS]
>
>* [Data Source Settings and Menu Options](datasources-list-and-settings.md#reference_A87B381067E04C26A426514AF3B64E64)

## Delete a Data Source {#task_740BACDEAA184B489B92C386DE7211BE}

Delete a data source that you no longer need.

>[!NOTE]
>
><!-- 

t_datasource_delete.xml

 -->
>Please note the following restrictions: 
>
>* You cannot delete an [Active Audience or Data Source Synced Trait](../c-features/traits/client-activity-synced-audience-traits.md#concept_7D3F4AF1FAD440509956632B8A51E64D). 
>* For customers using Adobe Analytics: Audience Manager does not allow you to delete data sources created automatically from your Analytics report suites. Use the [Core Service](https://marketing.adobe.com/resources/help/en_US/mcloud/) to unmap these data sources. 
>

1. Click **[!UICONTROL Audience Data]** > **[!UICONTROL Data Sources]**.
1. Select the check box next to one or more data sources.

   You can use the [!UICONTROL Search] box to locate the desired data sources if you have a long list. 1. Click  ![](assets/icon_trash.png)

   , then confirm the deletion.