---
description: Allow users to click through Collections from a single page layout and URL.
seo-description: Allow users to click through Collections from a single page layout and URL.
seo-title: Change Collection
solution: Experience Manager
title: Change Collection
uuid: a90e6dd8-e9c2-4ffc-9c2b-2ea7b28e87db
index: y
internal: n
snippet: y
translate: y
---

# Change Collection

Use the Change Collection Delegate to change the Collection shown on a page, without changing the URL, while a Livefyre App is already loaded. Use this feature to display photo or video galleries, or other Apps where the displayed Collection should change after a user action.

For example, clicking a video or photo in a gallery will load a Collection specific to that selection, while the URL of the page will not change.

To load one of three Collections from a single [](t_display_comment_count.md#t_display_comment_count) page:

```
<html> 
<head> 
<script src='//cdn.livefyre.com/Livefyre.js'></script> 
</head> 
<body> 
<script type="text/javascript"> 
convConfig1 = {"collectionMeta": <COLLECTION META 1>, 
             "checksum": <CHECKSUM 1>, 
             "siteId": <SITE ID>, 
             "articleId":"1", 
             "el":"livefyre"}; 
convConfig2 = {"collectionMeta": <COLLECTION META 2>, 
             "checksum": <CHECKSUM 2>, 
             "siteId": <SITE ID>, 
             "articleId":"2", 
             "el":"livefyre"}; 
convConfig3 = {"collectionMeta": <COLLECTION META 3>, 
             "checksum": <CHECKSUM 3>, 
             "siteId": <SITE ID>, 
             "articleId":"3", 
             "el":"livefyre"}; 
  
Livefyre.require(['fyre.conv#prod'],function(Conv) { 
    new Conv({"network": "<NETWORK NAME>"}, 
    [convConfig1], 
    function(app) {  
        window.changeConv = app.changeCollection; 
    } 
    ); 
}); 
</script> 
  
<div id="livefyre"></div> 
<button onclick="window.changeConv(convConfig1);">Conv 1</button> 
<button onclick="window.changeConv(convConfig2);">Conv 2</button> 
<button onclick="window.changeConv(convConfig3);">Conv 3</button> 
</body> 
</html>
```
