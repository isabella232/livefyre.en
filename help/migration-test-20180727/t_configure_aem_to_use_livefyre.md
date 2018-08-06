---
description: Configure AEM to use your organization’s Livefyre license credentials.
seo-description: Configure AEM to use your organization’s Livefyre license credentials.
seo-title: Configure AEM to Use Livefyre
title: Configure AEM to Use Livefyre
uuid: c739a5a6-1b16-433f-8b19-dcd97d08b9ee
index: y
internal: n
snippet: y
translate: y
---

# Configure AEM to Use Livefyre


>1. Find your organization’s Livefyre credentials. Open Livefyre Studio, and go to ** `Settings > Integration Settings > Credentials` **, to access the following information:
>    
>    * ** `Network Domain` **
>    * ** `Network Key` **
>    * ** `Site ID` **
>    * ** `Site Key` **
>    
>1. Configure AEM to use this Livefyre Network and Site by creating one or more Livefyre Cloud Service Configurations.
>   >1. From the AEM Dashboard, go to ** `Tools > Deployment > Cloud Services` **.
>   >1. Scroll to the ** `Livefyre` ** section.
>   >1. Click ** `Configure now` **or ** `Show Configurations` **(depending on your AEM platform).
>   >1. Click the plus sign ( ** `+` **) next to ** `Available Configurations` ** to create a Livefyre Configuration.
>   >1. Complete the information. For more on how to complete the information for Livefyre in AEM Cloud Services, see the Cloud Services Documentation for AEM on docs.adobe.com.
>1. When the ** `Livefyre Network Configuration` ** form displays, enter the Network Domain, Network Key, Site ID, and Site Key you obtained from Studio, and click ** `OK` **.
>   If your AEM Publish and AEM Author do not share the same cryptographic key you may need to repeat this process on the publisher instances. This is because the Network Key and Site Key are encrypted. For more information, see Replicate the Crypto Key on docs.adobe.com.>
