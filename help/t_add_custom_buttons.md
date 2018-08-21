---
description: Add custom actions to your Livefyre Apps.
seo-description: Add custom actions to your Livefyre Apps.
seo-title: Add Custom Buttons
solution: Experience Manager
title: Add Custom Buttons
uuid: 14559296-fdd8-4e03-879c-c0533e519244
index: y
internal: n
snippet: y
translate: y
---

# Add Custom Buttons

Livefyre allows you add custom buttons next to the existing action buttons (like **[!UICONTROL  Share]**, and **[!UICONTROL  Flag]**) on a piece of content.

Use the mobile argument to define whether the button will be displayed on mobile devices.

For example, to add a custom action button for your mobile device interface:

```
var convConfig = {...}; // Should have siteId, articleId, etc. 
convConfig.actionButtons = [ 
   { 
      mobile: true,  
      // (optional) sets whether the button will appear on mobile devices 
      key: 'Do Something', 
      callback: function(contentInfo) { 
         console.log('Author of content is ' + contentInfo.authorId); 
         console.log('id of content is ' + contentInfo.contentId); 
      } 
   }, 
    ... 
]; 
  
fyre.conv.load(networkConfig, [convConfig]);
```

>1. Pass an additional argument in your ConvConfig object named actionButtons, containing an array of objects describing each button you would like to add.
>1. Define a key for the text to display for each button.
>1. Add a callback that will be invoked on a click event for each button.
>The callback is invoked with an object with two keys: ` authorId` and ` contentId`. 
