---
description: Collect data sent from FLA files to Analytics and work with that information in Audience Manager.
seo-description: Collect data sent from FLA files to Analytics and work with that information in Audience Manager.
seo-title: Flash DIL
solution: Audience Manager
title: Flash DIL
uuid: 65833cfd-768e-4b16-95c5-debd8411df38
---

# Flash DIL{#flash-dil}

Collect data sent from FLA files to Analytics and work with that information in Audience Manager.

## <wintitle> Flash DIL </wintitle> {#concept_4DEAEE702A344431960F4CD5549E64A5}

Collect data sent from FLA files to Analytics and work with that information in Audience Manager.

<!-- 

c_flash_dil_toc.xml

 -->

[!UICONTROL Flash DIL] is an [!DNL ActionScript] code library that lets you work with video playback data in Audience Manager. [!DNL Flash DIL] works by capturing SWF content the Adobe [!UICONTROL AppMeasurement] library passes in to Analytics. [!DNL Flash DIL] sends that data to the separate [!UICONTROL DIL] JavaScript data collection module, which passes that information to Audience Manager. Analytics data ( [!UICONTROL Props], [!UICONTROL eVars], events, etc.) captured from the [!DNL FLA] file is available in Audience Manager as traits or unused signals. 

## Requirements for <wintitle> Flash DIL </wintitle> Data Collection {#concept_4ABD8B608CCE4920B65DDD7C8319D2A3}

General implementation and code-related requirements.

<!-- 

c_flash_dil_intro.xml

 -->

**Implementation Requirements**

[!UICONTROL Flash] data collection requires:

* The [!UICONTROL DIL] class library ( `dil.swc`). Obtain the [!UICONTROL DIL] class library from your Partner Solutions contact. 

* JavaScript [!UICONTROL DIL] data collection code on the page. 
* [DIL ActionScript library](../dil/dil-flash.md#reference_601A61BDC2A946048AD308ECFDF7F1F5) loaded in the Flash object you want to collect data from. 
* Adobe [!DNL AppMeasurement] [!DNL AS] library (version 3.5.2, or later) loaded the [!DNL Flash] object you want to collect data from.

**Set AllowScriptAccess to `Always` or `sameDomain`**

The `AllowScriptAccess` in HTML code that loads a SWF file controls the ability to perform outbound URL access from within the SWF file. When you configure a [!UICONTROL Flash DIL] data integration, make sure the Flash `AllowScriptAccess` parameter is set to `always` or `sameDomain`. [!UICONTROL Flash DIL] data collection will not work if `AllowScriptAccess` is set to `never`. See [Control Access to Scripts or Host Web Page](https://helpx.adobe.com/flash/kb/control-access-scripts-host-web.html).

**JS [!UICONTROL DIL] Code Placement**

Try to place the JS [!UICONTROL DIL] data collection module on the page so it loads before the [!DNL FLA] file. When the [!DNL FLA] file loads first, before [!UICONTROL DIL] data collection is ready, you can miss the initial data signals that [!UICONTROL Flash DIL] sends to that module. However, once instantiated, the [!UICONTROL DIL] data collection module will capture all subsequent SWF file data passed in by [!UICONTROL Flash DIL]. 

## Data Collected by <wintitle> Flash DIL </wintitle> {#reference_C04E633B1E5A4674A808C4CD8A35B48A}

[!UICONTROL Flash DIL] captures page view, link tracking, media tracking, and other media view events from the Adobe [!UICONTROL AppMeasurement] library.

<!-- 

r_flash_dil_data_collected.xml

 -->

**Page View Events**

Unless specified otherwise by `s.trackVars`, [!UICONTROL Flash DIL] collects the following data from Adobe AppMeasurement:

* `pageName` 
* `channel` 
* `campaign` 
* `products` 
* `events` 
* `prop1 - prop75` 
* `eVar1 - eVar75`

**Link Tracking Events**

Unless specified otherwise by `s.linkTrackVars`, [!UICONTROL Flash DIL] collects the following data from Adobe [!UICONTROL AppMeasurement]:

* `pe` (Type of track link called) 
* `pev1` (Link URL) 
* `pev2`(Link text)

**Media Tracking Events**

Unless specified otherwise by `s.Media.trackVars`, [!UICONTROL Flash DIL] collects all the data enumerated in the Page View Events section.

**Other Data Points**

Data from these parameters is collected by default:

* `mediaName` (Media/video element name) 
* `mediaAdName` (Ad name) 
* `mediaAdParentName` (Name of the primary media content the ad is nested under) 
* `mediaAdParentPod` (The pod or ad break within the primary content where the ad plays) 
* `mediaAdParentPodPos` (The numeric position within the pod where the ad plays. More than one ad can play within a pod.

>[!MORE_LIKE_THIS]
>
>* [AppMeasurement Flash, Flex, and OSMF Implementation Guide](https://marketing.adobe.com/resources/help/en_US/sc/appmeasurement/flash/)

## <wintitle> Flash DIL </wintitle> Data in Audience Manager {#concept_6CB7727B74A5432DA2FE3B8386441F12}

The [!UICONTROL Flash DIL] module turns Adobe AppMeasurement data into Audience Management traits and unused signals.

<!-- 

c_flash_dil_in_aam.xml

 -->

Analytics [!UICONTROL Props], [!UICONTROL eVars], and events work like traits in Audience Management. Traits are key-value pairs and are used to build segments. For example, in an Analytics prop like `prop35=foo`, `prop35` is the key (a constant) and `foo` is the value (a variable).

**Match Audience Manager Traits to Analytics Variables**

To use the Analytics data passed by [!UICONTROL Flash DIL], you should create Audience Manager traits that have:

* The same names as their Analytics equivalents. 
* A key value prefixed with `c_`.

See the table for examples:  

|  Analytics Data Element  | Analytics Example  | As Audience Manager Trait  |
|---|---|---|
|  **prop** | `c30=foo`  | `c_prop35=foo`  |
|  **evar** | `v35=bar`  | `c_evar=bar`  |
|  **events** | `events=event10`  | `c_events=event10`  |

** [!UICONTROL Flash DIL]/Analytics Data as Unused Signals**

Audience Manager accepts Analytics [!UICONTROL Props], [!UICONTROL eVars], and events even without a corresponding trait. In this case, the data is unavailable for trait creation and appears in the [Unused Signals report](../reporting/dynamic-reports/unused-signals.md#concept_D3A6A3AD84AE47589699A13A8F971BE0) instead. To make the most of this information, create Audience Manager traits that match the Analytics data passed in by the [!UICONTROL Flash DIL] library. 

>[!MORE_LIKE_THIS]
>
>* [Traits](../features/traits/trait-details-page.md)
>* [Signals, Traits, and Segments](../reference/signal-trait-segment.md#concept_7550A48FE3F1415FACF0E077CFAB155F)
>* [Key-Value Pairs Explained](../reference/key-value-pairs-explained.md#concept_E4236E003076483AA939791FE2492B49)
>* [Prefix Requirements for Key Variables](../features/traits/trait-variable-prefixes.md#reference_E6F1E4257F664FC2A797C406BF147ABC)

## <wintitle> Flash DIL </wintitle> <keyword> ActionScript </keyword> Library {#reference_601A61BDC2A946048AD308ECFDF7F1F5}

Code for your [!DNL Flash] object to send Analytics data to Audience Management.

<!-- 

r_flash_dil_actionscript.xml

 -->

>[!NOTE]
>
>* For each [!DNL Flash] object, the code supports one partner instance ( `d.partner`) only. 
>
>* Requires the Adobe [!UICONTROL AppMeasurement] [!DNL AS] library version 3.5.2 or higher. 
>

```js
import com.omniture.AppMeasurement; // Omit this line if it already exists in the code 
import com.adobe.am.DIL; 
  
var s:AppMeasurement = new AppMeasurement(); // Omit this line if it already exists in the code 
var d:DIL = new DIL(); 
d.partner = "<partner>";// Partner name 
d.containerNSID = <container NSID>; // Optional, defaults to 0 
s.loadModule(d);
```
