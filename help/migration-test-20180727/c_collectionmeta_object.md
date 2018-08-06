---
description: The CollectionMeta object is a JSON object that specifies metadata to store within the Collection.
seo-description: The CollectionMeta object is a JSON object that specifies metadata to store within the Collection.
seo-title: CollectionMeta Object
solution: Experience Manager
title: CollectionMeta Object
uuid: c45480cd-1bad-4adc-b4d7-8f1fffbfb8ba
index: y
internal: n
snippet: y
translate: y
---

# CollectionMeta Object

` CollectionMeta` is always encoded before being passed to Livefyre for security. The encoded value is passed into the ` ConvConfig` object shown above.

>[!NOTE]
>
>You must add server-side code to encode the ` CollectionMeta` JSON object. See Building Server-side Tokens for more information. 


<table frame="all" rowsep="1" colsep="1" id="table_ibg_xc5_nz"> 
 <thead> 
  <tr> 
   <th class="entry"> Parameter </th> 
   <th class="entry"> Type </th> 
   <th class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> <span class="varname"> articleId </span> </td> 
   <td> String (required) </td> 
   <td> A unique ID for the Collection. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> title </span> </td> 
   <td> String (required) </td> 
   <td> <p>The title you wish to apply to the Collection. This often corresponds to the title of the page that displays the App.</p> <p>For example: “Integration is So Much Fun!”</p> <p>Note:  The max character length for the title is 255 characters. The title field does not support HTML entities. Please encode special characters using UTF-8. </p> </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> url </span> </td> 
   <td> String (required) </td> 
   <td> <p>The canonical absolute URL you wish to attach to this Collection. This URL will be used to generate links back to the App from content shared on Facebook and Twitter, email notifications, and Livefyre Studio.</p> <p>Note:  Livefyre requires the use of a fully qualified domain name; the port number or a callback to resolve the local setup is not required. If testing locally, be certain to use a valid base URL domain. (For example: http://customer.com is valid, while http://localhost:5995 is not.) Once you have set up your local webserver to accept a fully qualified domain name, no callbacks or resolutions are needed, and local development can proceed as expected. </p> </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> type </span> </td> 
   <td> String (required) </td> 
   <td> The Collection type. Must be <span class="codeph"> livechat </span>. </td> 
  </tr> 
 </tbody> 
</table>

The ` CollectionMeta` object may also contain the following optional parameter:

|  Parameter  | Type  | Description  |
|---|---|---|
|  * ` tags` * | (optional) string  | A comma-separated list of single keywords or phrases. Search Collections by tags within Studio or with the search API. **Note:**While tags added through Studio may contain spaces, tags entered through the API cannot. Use underscores to define tags that will display spaces in the UI. (For example: use Monday_Quarterback to display Monday Quarterback in Studio.)  |

