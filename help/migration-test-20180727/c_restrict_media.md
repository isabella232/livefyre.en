---
description: Limit the type of media that gets into the App stream.
seo-description: Limit the type of media that gets into the App stream.
seo-title: Restrict Media
solution: Experience Manager
title: Restrict Media
uuid: eafc9f95-4db6-434c-b77a-c1c6aac38c9d
index: y
internal: n
snippet: y
translate: y
---

# Restrict Media

By default, all media attachments can be embedded into Apps. Livefyre allows you to change this option to prevent users from posting selected attachment types to your Apps.

>[!NOTE]
>
>Livefyre partners with Embedly for media integration. For more information, see Content Integration &gt; Embedly Integration. Please contact your Technical Account Manager for questions about link expansion or sources.

This example blocks YouTube and Vimeo embeds from your comment stream:

```
var attachmentDelegate = function(embedObj) { 
   var providersToBlock = ['youtube', 'vimeo']; 
   for (var i=0, len=providersToBlock.length; i<len; i++) { 
      if (embedObj.provider_url.indexOf(providersToBlock[i]) > -1) { 
         return false; 
      } 
   } 
   return true; 
};
```
When loading the conversation:

```
networkConfig["attachmentDelegate"] = attachmentDelegate; 
fyre.conv.load(networkConfig, [convConfig]);
```
