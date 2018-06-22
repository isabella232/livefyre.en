---
description: Enable live commenting on your page.
seo-description: Enable live commenting on your page.
seo-title: Comments Integration
solution: Experience Manager
title: Comments Integration
---

# Comments Integration

Comments allows you to replace your default commenting system with real-time conversations on your page.

* Integration
* NetworkConfig Object
* ConvConfig Object
* CollectionMeta Object
* Adding an Event Handler
## Adding an Event Handler {#section_ktb_nv1_c1b}

To register event handlers, use the widget.on call within the App’s callback function.

For example:

```
Livefyre.require(['fyre.conv#3'], function(Conv) { 
 new Conv(networkConfig, [convConfig], function(widget) { 
 widget.on('&lt;strong&gt;&lt;eventName&gt;&lt;/strong&gt;', function (data) { 
 // Do something, perhaps using data 
 }); 
 }); 
}); 

```
* Ads in Comments
## Integration {#section_fmm_ppj_tbb}

To embed a Comments App, follow the procedure for Integrating a Conversation App. See [](c_implement_a_conversation_app.md#concept_zvy_c3c_tbb). The following is an example of an embedded Comments App.

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
As noted in the Building `codeph  CollectionMeta` section, `codeph  CollectionMeta` is an encoded JSON object. In the above example, the JSON object takes the following format before it’s JWT encoded:

```
{ 
"url": "articleUrl", 
"articleId": "articleId", 
"type": "livecomments", 
"title": "articleTitle" 
}
```
