---
description: Embedding the Comments App follows the process for embedding a Core App.
seo-description: Embedding the Comments App follows the process for embedding a Core App.
seo-title: Embed a Comments App
solution: Experience Manager
title: Embed a Comments App
---

# Embed a Comments App

Embedding the Comments App follows the process for embedding a Core App described in [](t_embed_an_app_on_your_site_using_livefyre.js.md#embed_an_app_on_your_site_using_livefyre.js)

**Example:**

```
&lt;html&gt; 
 &lt;head&gt; 
 &lt;script src="//cdn.livefyre.com/Livefyre.js"&gt; 
 &lt;/script&gt; 
 &lt;/head&gt; 
&lt;body&gt; 
 &lt;script type="text/javascript"&gt; 
 var networkConfig = { 
 network: 'domainName' 
 }; 
 var convConfig = { 
 siteId: 'siteId', 
 articleId: 'articleId', 
 el: 'livefyre', 
 collectionMeta: 'collectionMeta', 
 checksum: 'checksum' 
 }; 
 
 Livefyre.require(['fyre.conv#3', 'auth'], function(Conv, auth) { 
 new Conv(networkConfig, [convConfig], function(commentsWidget) {}); 
 auth.delegate({ 
 login: function (callback) { 
 callback(null,{livefyre:'&lt;userauthtoken&gt;'}); 
 }, 
 }); 
 }); 
 
 &lt;/script&gt; 
 &lt;div id="livefyre"&gt; 
 &lt;/div&gt; 
 &lt;/body&gt; 
&lt;/html&gt;
```
As noted in the Building CollectionMeta section, CollectionMeta is an encoded JSON object. In the above example, the JSON object takes the following format before it’s JWT encoded:

```
{ 
"url": "articleUrl", 
"articleId": "articleId", 
"type": "livecomments", 
"title": "articleTitle" 
}
```
