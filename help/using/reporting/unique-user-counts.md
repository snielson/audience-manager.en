---
description: Describes the variation in unique user totals between reports for the same trait and time period.
seo-description: Describes the variation in unique user totals between reports for the same trait and time period.
seo-title: Counting Unique Users in Overlap and General Reports
solution: Audience Manager
title: Counting Unique Users in Overlap and General Reports
uuid: 6a085714-d4ee-41c7-b7d7-884a395c046d
index: y
internal: n
snippet: y
---

# Counting Unique Users in Overlap and General Reports{#counting-unique-users-in-overlap-and-general-reports}

Describes the variation in unique user totals between reports for the same trait and time period.

<!-- 

c_unique_user_counts.xml

 -->

**Overlap Report: Unique User Count**

The overlap reports count users as unique when they qualify for a trait:

* During the selected time interval for the report. 
* That has a [time-to-live](../c-features/traits/segment-ttl-explained.md#concept_2F85D4E738754EF387328A9754E125B3) value longer than the selected time interval for the report. 
* If they're seen as active in our system (i.e, qualified for any other trait, had an ID sync, etc.) within the past 60 days.

**General Report: Unique User Count**

The General report counts site visitors as unique if they qualified for the trait during the selected time period. 

>[!MORE_LIKE_THIS]
>
>* [Interactive Reports](dynamic-reports.md#concept_88ADC775F1E9458582A3285B29B76A46)
>* [General Reports](general-reports.md#concept_E4686B9B4BE54DFE9599E0868224E027)