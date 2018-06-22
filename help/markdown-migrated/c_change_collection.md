---
description: Allow users to click through Collections from a single page layout and URL.
seo-description: Allow users to click through Collections from a single page layout and URL.
seo-title: Change Collection
solution: Experience Manager
title: Change Collection
---

# Change Collection

Use the Change Collection Delegate to change the Collection shown on a page, without changing the URL, while a Livefyre App is already loaded. Use this feature to display photo or video galleries, or other Apps where the displayed Collection should change after a user action.

For example, clicking a video or photo in a gallery will load a Collection specific to that selection, while the URL of the page will not change.

To load one of three Collections from a singl [](#t_display_comment_count)e page:

```
&lt;html&gt; 
&lt;head&gt; 
&lt;script src='//cdn.livefyre.com/Livefyre.js'&gt;&lt;/script&gt; 
&lt;/head&gt; 
&lt;body&gt; 
&lt;script type="text/javascript"&gt; 
convConfig1 = {"collectionMeta": &lt;COLLECTION META 1&gt;, 
 "checksum": &lt;CHECKSUM 1&gt;, 
 "siteId": &lt;SITE ID&gt;, 
 "articleId":"1", 
 "el":"livefyre"}; 
convConfig2 = {"collectionMeta": &lt;COLLECTION META 2&gt;, 
 "checksum": &lt;CHECKSUM 2&gt;, 
 "siteId": &lt;SITE ID&gt;, 
 "articleId":"2", 
 "el":"livefyre"}; 
convConfig3 = {"collectionMeta": &lt;COLLECTION META 3&gt;, 
 "checksum": &lt;CHECKSUM 3&gt;, 
 "siteId": &lt;SITE ID&gt;, 
 "articleId":"3", 
 "el":"livefyre"}; 
 
Livefyre.require(['fyre.conv#prod'],function(Conv) { 
 new Conv({"network": "&lt;NETWORK NAME&gt;"}, 
 [convConfig1], 
 function(app) { 
 window.changeConv = app.changeCollection; 
 } 
 ); 
}); 
&lt;/script&gt; 
 
&lt;div id="livefyre"&gt;&lt;/div&gt; 
&lt;button onclick="window.changeConv(convConfig1);"&gt;Conv 1&lt;/button&gt; 
&lt;button onclick="window.changeConv(convConfig2);"&gt;Conv 2&lt;/button&gt; 
&lt;button onclick="window.changeConv(convConfig3);"&gt;Conv 3&lt;/button&gt; 
&lt;/body&gt; 
&lt;/html&gt;
```
