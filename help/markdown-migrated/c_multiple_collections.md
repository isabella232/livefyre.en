---
description: Showcase multiple Collections on a single page.
seo-description: Showcase multiple Collections on a single page.
seo-title: Multiple Collections
solution: Experience Manager
title: Multiple Collections
---

# Multiple Collections

You may include multiple Collections on a single page on your site. For example, to publish an event, you may have a Live Blog or Chat discussion during the event, with a separate App on the side of your page, displaying related Curated Content from around the social web. Or, you could include a Comments App below an article, with a Chat to the side.

To get multiple conversations on a page, add one or more configurations in an array and pass the array to the load call. For example.

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
