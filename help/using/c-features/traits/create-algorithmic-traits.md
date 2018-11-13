---
description: Describes set up steps and features unique to the algorithmic trait creation process.
seo-description: Describes set up steps and features unique to the algorithmic trait creation process.
seo-title: Create Algorithmic Traits
solution: Audience Manager
title: Create Algorithmic Traits
uuid: c5942e6d-91cc-4d91-aa98-909a77125378
index: y
internal: n
snippet: y
---

# Create Algorithmic Traits{#create-algorithmic-traits}

Describes set up steps and features unique to the algorithmic trait creation process.

## Create Algorithmic Traits {#concept_3FB1946A58AC489E822161B2EE4EB95A}

Describes set up steps and features unique to the algorithmic trait creation process.

<!-- 

c_tb_algo_traits.xml

 -->

## Create an Algorithmic Trait {#task_E9A3F46A50C14450AE263775EECA0353}

Describes the required and optional steps that let you create an algorithmic trait.

<!-- 

t_algo_trait_build.xml

 -->

To create an algorithmic trait, go to [!UICONTROL Traits] and follow the steps below: 

1. Click **[!UICONTROL Create New Trait]** and select **[!UICONTROL Algorithmic]** from the drop down menu.
1. In the [Basic Information](../../c-features/traits/create-onboarded-rule-based-traits.md#concept_D80233EF56764376B0F4C4FF882BAD2E) section

    * Name the trait. 
    * Select a data source. 
    * Choose a storage folder.

1. Expand the [!UICONTROL Configuration] pane and click **[!UICONTROL Browse All Models]**.

   This opens a new window that lets you select the model you want to use with the trait. 1. Select a model and click **[!UICONTROL Add Selected Model to Trait]**.

   Adding the model exposes the reach and accuracy settings. 1. Select reach or accuracy as your goal and choose a value from the respective drop down menus. Click **[!UICONTROL Save]** when done.

>[!MORE_LIKE_THIS]
>
>* [Accuracy and Reach](trait-accuracy-reach.md#concept_60F696940483424CA4E8EEDD63F46358)

## Configuration Settings for Algorithmic Traits {#reference_3A245B6E0888405E986B6C06FB5C9188}

In [!UICONTROL Trait Builder], the [!UICONTROL Configuration] section lets you associate an algorithmic model to a trait. To complete the algorithmic trait creation process, select a model and choose a reach or accuracy goal. 

**Prerequisites:** 

<!-- 

r_algo_trait_config_section.xml

 -->

* [Create an algorithmic model](../../c-features/create-model.md#task_71541056B8384EEBB6A3A8B161C71B8A). 
* Wait for the notification email that lets you know the model data run has finished. 
* Complete the required fields in the [Basic Information](../../c-features/traits/create-onboarded-rule-based-traits.md#concept_D80233EF56764376B0F4C4FF882BAD2E) section.

**Configuration Fields and Settings**

|  Interface Element  | Explanation  |
|---|---|
|  ****[!UICONTROL Select Model for Algorithmic Trait]**** |Click the **[!UICONTROL Update]** button to open the models window. From the window, select the algorithmic model that you want to use to create the trait.  |
|  ****[!UICONTROL Select Goal Accuracy]**** | Select this option to create a trait based on accuracy. Accuracy is a scored value that indicates how close potential users are to your baseline. The accuracy scale ranges from 0 (least accurate) to 1 (most accurate).  |
|  ****[!UICONTROL Reach and Accuracy Data Columns]**** | Located on the right, this section displays up to 21 rows of numeric data that displays the accuracy and reach values for your model.  |
|  ****[!UICONTROL Reach and Accuracy Slider]**** | Located at the bottom of the graph, the slider lets you set a numeric value for your reach or accuracy goals. You can set the slider and then choose the reach or accuracy goal button to create a trait.  |

>[!MORE_LIKE_THIS]
>
>* [Accuracy and Reach](trait-accuracy-reach.md#concept_60F696940483424CA4E8EEDD63F46358)