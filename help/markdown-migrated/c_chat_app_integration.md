---
description: Embedding the Chat App follows the process for embedding a Core App.
seo-description: Embedding the Chat App follows the process for embedding a Core App.
seo-title: Embed a Chat App
title: Embed a Chat App
---

# Embed a Chat App

Embedding the Chat App follows the process for embedding a Core App described in Getting Started &gt; Embedding an App.

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
"url": "http://dev.livefyre.com/articles/test.html", 
"articleId": "1", 
"type": "livechat", 
"title": "Title 1" 
}
```
