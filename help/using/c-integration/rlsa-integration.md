---
description: This procedure requires an AdWords remarketing list, pixel code, and an Audience Manager URL destination. It is also known as a remarketing list for search ads (RLSA) integration. Applies to paid search only.
seo-description: This procedure requires an AdWords remarketing list, pixel code, and an Audience Manager URL destination. It is also known as a remarketing list for search ads (RLSA) integration. Applies to paid search only.
seo-title: Send Segments to a Google AdWords Remarketing List
solution: Audience Manager
title: Send Segments to a Google AdWords Remarketing List
uuid: 0fcc6f0c-334b-4ef3-93ec-2a8af792fdbc
index: y
internal: n
snippet: y
---

# Send Segments to a Google AdWords Remarketing List{#send-segments-to-a-google-adwords-remarketing-list}

This procedure requires an AdWords remarketing list, pixel code, and an Audience Manager URL destination. It is also known as a remarketing list for search ads (RLSA) integration. Applies to paid search only.

To set up an AdWords remarketing list as an [!DNL Audience Manager] URL destination: 

1. In AdWords, [create a website re-marketing list](https://support.google.com/adwords/answer/2454064?hl=en).

1. Copy the pixel code from the [dynamic remarketing tag](https://support.google.com/adwords/answer/3103357). Do not copy the code this example.

   Your pixel code / image request will look similar to this:

   ```
      <img height="1" width="1" style="border-style:none;" alt="" 
   src="//googleads.g.doubleclick.net/pagead/viewthroughconversion/xxxxxxxx/? 
   value=0&guid=ON&script=0"/>
   ```

1. Remove all the image and source metadata from the pixel code.

   Your edited code snippet should look similar to this:

   ```
   //googleads.g.doubleclick.net/pagead/viewthroughconversion/xxxxxxxx/? 
   value=0&guid=ON&script=0
   ```

1. [Create a URL destination](../c-features/destinations/manage-destinations.md#concept_51842672DFA943EA982B363E74D42DF8) or edit an existing destination.
1. In the [!UICONTROL Segment Mappings] section of your URL destination, add the edited code to the **[!UICONTROL URL]** and **[!UICONTROL Secure URL]** boxes. Prefix the code with `https:` and `https:` in the URL and Secure URL boxes, respectively.

   >[!IMPORTANT]
   >
   >Replace encoded ampersands `&` with un-encoded ampersands `&`

   Unsecure URL code: 

   ```
   https://googleads.g.doubleclick.net/pagead/viewthroughconversion/xxxxxxxx/? 
   value=0&guid=ON&script=0
   ```

   Secure URL code: 

   ```
   https://googleads.g.doubleclick.net/pagead/viewthroughconversion/xxxxxxxx/? 
   value=0&guid=ON&script=0
   ```

1. Click **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >If you're working with multiple segments, get a new pixel for each segment you want to map to an AdWords destination. This ensures the data is applied to the appropriate remarketing list.

A completed mapping could look similar to this:

![](assets/rlsa_mapping.png)

>[!MORE_LIKE_THIS]
>
>* [Destinations](destinations.md#concept_5BDA346C376C4B719EA394108AB2735A)
>* [Create a URL Destination](manage-destinations.md#concept_51842672DFA943EA982B363E74D42DF8)
>* [About AdWords Remarketing Lists](https://support.google.com/adwords/answer/2472738)
>* [How AdWords Remarketing Works](https://support.google.com/adwords/answer/2454000)