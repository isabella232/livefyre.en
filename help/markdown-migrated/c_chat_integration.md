---
description: Adding live chat to your page.
seo-description: Adding live chat to your page.
seo-title: Chat Integration
solution: Experience Manager
title: Chat Integration
---

# Chat Integration

Chat allows your audience to engage in real-time conversation surrounding live events. Content is displayed as a continuous stream, encouraging rapid participation in the unfolding dialog.

* Integration
* NetworkConfig Object
* ConvConfig Object
* CollectionMeta Object
* Adding an Event Handler
To embed a Chat App, follow the procedure for Integrating a Conversation App. See [](c_implement_a_conversation_app.md#concept_zvy_c3c_tbb). The following is an example of an embedded Chat App.

```
&lt;html&gt; 
 &lt;head&gt; 
 &lt;script src="//cdn.livefyre.com/Livefyre.js"&gt; 
 &lt;/script&gt; 
 &lt;/head&gt; 
&lt;body&gt; 
 &lt;script type="text/javascript"&gt; 
 var networkConfig = { 
 network: "client-solutions.fyre.co" 
 }; 
 var convConfig = { 
 siteId: '347674', 
 articleId: '1', 
 el: 'livefyre', 
 collectionMeta: 'eyJ0eXAiOiJqd3QiLCJhbGciOiJIUzI1NiJ9.eyJ0aXRsZSI6IlRpdGxlIDEiLCJ1cmwiOiJodHRwOlwvXC9kZXYubGl2ZWZ5cmUuY29tIiwidGFncyI6InRhZzEsdGFnMiIsImNoZWNrc3VtIjoiY2Q0YTJjYWJkMTIxOTkyM2FjZGJhMjExOWY2NmYwNTUiLCJhcnRpY2xlSWQiOiIxIn0.Dq-ghi9KYmEPmagvCS1NPyYDRMGBujm735QaTRb7E7k', 
 checksum: '6e2e4faf7b95f896260fe695eafb34ba' 
 }; 
 
 Livefyre.require(['fyre.conv#3'], function(Conv) { 
 new Conv(networkConfig, [convConfig], function(chatWidget) {}); 
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
As noted in the CollectionMeta Token section, CollectionMeta is an encoded JSON object. In the above example, the JSON object takes the following format before it’s JWT encoded:

```
{ 
"url": "https://dev.livefyre.com/articles/test.html", 
"articleId": "1", 
"type": "livechat", 
"title": "Title 1" 
}
```
