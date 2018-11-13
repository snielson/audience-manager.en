---
description: In Audience Manager, a destination is any third-party system (ad server, DSP, ad network, etc.) that you want to share data with. Destination Builder is the tool you used to create and manage cookie, URL, or server-to-server destinations.
keywords: integration code
seo-description: In Audience Manager, a destination is any third-party system (ad server, DSP, ad network, etc.) that you want to share data with. Destination Builder is the tool you used to create and manage cookie, URL, or server-to-server destinations.
seo-title: Destinations
solution: Audience Manager
title: Destinations
uuid: e6476ac6-34a7-4bc9-89d3-6018076fc1ff
index: y
internal: n
snippet: y
---

# Destinations{#destinations}

In Audience Manager, a destination is any third-party system (ad server, DSP, ad network, etc.) that you want to share data with. Destination Builder is the tool you used to create and manage cookie, URL, or server-to-server destinations.

## Purpose and Advantages {#section_D26ED9B4C55F4FAF9406C518ED41C5E6}

<!-- 

c_destinations.xml

 -->

[!UICONTROL Destinations] and [!UICONTROL Destination Builder] let you create destinations and send information about segmented users to your data partner. This helps you:

* **Protect data value:** Rather than send all user data to a destination, [!UICONTROL Destination Builder] let you share specific information about qualified users only. 

* **Take action on your data:** Sending data to a destination partner helps them quickly develop and target qualified audience segments. 
* **Reduce technical overhead:** Business users can set up destinations safely in the [!UICONTROL Destination Builder] interface. This helps reduce the time required for pre-deployment testing. With [!UICONTROL Destination Builder], you create, manage, and delete destinations as your business needs change, all without working through a long development cycle.

## Technical Considerations {#section_62E0C3764C86476683D5F8F6CE2F6DC9}

<!-- 

destination-delivery-methods.xml

 -->

Data delivery depends on how your data partner wants to, or can, receive destination information. Technical or engineering constraints may prevent a destination from receiving data via URL, cookie, or server-to-server processes. Work with your third-party partner to determine which method they can use.

## Business Considerations {#section_F666F33012EA4EA883190102E295AF5F}

Business decisions for selecting one delivery method over another depend on the technical capabilities of your destination partner and what you want to do with qualified user information. For example, technical constraints can limit your options if a destination cannot receive data by a particular delivery method. However, if there are no technical issues, you can send information based on how you want to take action on that data. For example:

* URLs and cookie-based destinations work almost synchronously with user actions on a page. 
* Server-to-server methods are good for building deep audience segments over time.

## Destination Types and Typical Uses {#section_84C13A0A9BEC430AA16CB6E7A6438049}

The examples in the following table can help you understand when to use a particular destination and the differences between each type. 

<table id="table_1510DBC812BB4DABAB3E009583C6B423"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Destination Type </th> 
   <th colname="col2" class="entry"> Typically Used When </th> 
   <th colname="col3" class="entry"> Example </th> 
   <th colname="col4" class="entry"> Considerations </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <b>URL</b> </td> 
   <td colname="col2" morerows="1"> You need to transfer data immediately so a destination can take action on a qualified user right away. </td> 
   <td colname="col3" morerows="1"> Sending data from a ticket purchasing site. Use a URL or cookie destination to qualify user and immediately re-target. </td> 
   <td colname="col4" morerows="1"> 
    <ul id="ul_92FF3164AEA749D58938784BAA5CFA17"> 
     <li id="li_1857F829FD634F68BB6DCCE2FF7FBFA7">Transfers data about new visitors only. </li> 
     <li id="li_C0541B2ABB6F4DC49DF1373E62E8BD20">Visitors must be seen again to qualify for the segment. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <b>Cookie</b> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <b>Server-to-server</b> </td> 
   <td colname="col2"> 
    <ul id="ul_64F3938944EA4BD98F26BE60DB51D585"> 
     <li id="li_AF63E5AE8E0747FA8A8EAD84B26FE20A">Immediate data transfer is not required. </li> 
     <li id="li_90C7CEE7871844619462D19781A4E567">Collecting data to build a large audience pool of qualified users. </li> 
    </ul> </td> 
   <td colname="col3"> Collecting data over time (hours or days) to use it in a campaign set to run at a later date. </td> 
   <td colname="col4"> 
    <ul id="ul_0F15F2A88888466F8DBEFE3BCADDE28E"> 
     <li id="li_D16F682745124A71BF127D118077C99B">Transfers data about new and previous site visitors. </li> 
     <li id="li_E58366168184443DA69B430B7ABBCE9A">Visitors don't have to be seen again to qualify for other segments. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
