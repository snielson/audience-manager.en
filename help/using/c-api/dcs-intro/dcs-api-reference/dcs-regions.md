---
description: The regional DCS server host name is required to make calls to the DCS. This is because the DCS stores information in data centers that are geographically close to site visitors. Your queries will work if you send them to the wrong DCS, but these calls are inefficient and can delay the response. To make a DCS request, match the region ID to its corresponding regional host name and form your query with the proper host name.
seo-description: The regional DCS server host name is required to make calls to the DCS. This is because the DCS stores information in data centers that are geographically close to site visitors. Your queries will work if you send them to the wrong DCS, but these calls are inefficient and can delay the response. To make a DCS request, match the region ID to its corresponding regional host name and form your query with the proper host name.
seo-title: DCS Region IDs, Locations, and Host Names
solution: Audience Manager
title: DCS Region IDs, Locations, and Host Names
uuid: 9709461d-4db8-4fcf-b624-5e277d087eaf
index: y
internal: n
snippet: y
---

# DCS Region IDs, Locations, and Host Names{#dcs-region-ids-locations-and-host-names}

The regional DCS server host name is required to make calls to the DCS. This is because the DCS stores information in data centers that are geographically close to site visitors. Your queries will work if you send them to the wrong DCS, but these calls are inefficient and can delay the response. To make a DCS request, match the region ID to its corresponding regional host name and form your query with the proper host name.

<table id="table_643212E4F9C64DFF9443904B01D89CB3"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> DCS Region ID (dcs_region) </th> 
   <th colname="col2" class="entry"> Region (and Location) </th> 
   <th colname="col3" class="entry"> Host Name </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>ID 3 </p> </td> 
   <td colname="col2"> <p>Southeast Asia (Singapore) </p> </td> 
   <td colname="col3"> <p> <span class="codeph"> apse.demdex.net</span> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>ID 4 </p> </td> 
   <td colname="col2"> <p>South America (São Paulo, Brazil) </p> </td> 
   <td colname="col3"> <p> <span class="codeph"> sae.demdex.net</span> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>ID 6 </p> </td> 
   <td colname="col2"> <p>Europe (Dublin, Ireland) </p> </td> 
   <td colname="col3"> <p> <span class="codeph"> irl1.demdex.net</span> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>ID 7 </p> </td> 
   <td colname="col2"> <p>US East (Virginia, USA) </p> </td> 
   <td colname="col3"> <p> <span class="codeph"> use.demdex.net</span> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>ID 8 </p> </td> 
   <td colname="col2"> <p>South Pacific / Oceania (Sydney, Australia) </p> </td> 
   <td colname="col3"> <p> <span class="codeph"> apse2.demdex.net</span> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>ID 9 </p> </td> 
   <td colname="col2"> <p>US West (Oregon, USA) </p> </td> 
   <td colname="col3"> <p> <span class="codeph"> usw2.demdex.net</span> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>ID 11 </p> </td> 
   <td colname="col2"> <p>Asia (Tokyo, Japan) </p> </td> 
   <td colname="col3"> <p> <span class="codeph"> tyo3.demdex.net</span> </p> </td> 
  </tr> 
 </tbody> 
</table>

You can also use API methods to get a list of the available [!UICONTROL DCS] regions. See [DCS Region API Methods](../../../c-api/c-rest-api-main/aam-api-dcs-regions.md#concept_C1EF1A07C73D489FAD2AECA39B113DC6). 