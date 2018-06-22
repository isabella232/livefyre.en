---
description: Configure AEM to use your organization’s Livefyre license credentials.
seo-description: Configure AEM to use your organization’s Livefyre license credentials.
seo-title: Configure AEM to Use Livefyre
title: Configure AEM to Use Livefyre
---

# Configure AEM to Use Livefyre

>1. Find your organization’s Livefyre credentials. Open Livefyre Studio, and go to `uicontrol Settings &gt; Integration Settings &gt; Credentials`, to access the following information:
>* `uicontrol Network Domain`
>* `uicontrol Network Key`
>* `uicontrol Site ID`
>* `uicontrol Site Key`
>   
>   
>1. Configure AEM to use this Livefyre Network and Site by creating one or more Livefyre Cloud Service Configurations.
>   >1. From the AEM Dashboard, go to `uicontrol Tools &gt; Deployment &gt; Cloud Services`.
>   >   
>   >1. Scroll to the `uicontrol Livefyre` section.
>   >   
>   >1. Click `uicontrol Configure now`or `uicontrol Show Configurations`(depending on your AEM platform).
>   >   
>   >1. Click the plus sign (`uicontrol +`) next to `uicontrol Available Configurations` to create a Livefyre Configuration.
>   >   
>   >1. Complete the information. For more on how to complete the information for Livefyre in AEM Cloud Services, see the Cloud Services Documentation for AEM on docs.adobe.com.
>   >   
>   >   
>   
>1. When the `uicontrol Livefyre Network Configuration` form displays, enter the Network Domain, Network Key, Site ID, and Site Key you obtained from Studio, and click `uicontrol OK`.
>   If your AEM Publish and AEM Author do not share the same cryptographic key you may need to repeat this process on the publisher instances. This is because the Network Key and Site Key are encrypted. For more information, see Replicate the Crypto Key on docs.adobe.com.
>   
>   
