---
description: Live Blog allows you to feature real-time updates and images from your site’s own editors when covering a live event.
seo-description: Live Blog allows you to feature real-time updates and images from your site’s own editors when covering a live event.
seo-title: Live Blog Integration
solution: Experience Manager
title: Live Blog Integration
---

# Live Blog Integration

## Integration {#section_dqx_dmk_d1b}

To embed a Live Blog App, follow the procedure for Integrating a Conversation App. See [](c_implement_a_conversation_app.md#concept_zvy_c3c_tbb). The following is an example of what an embedded Live Blog App looks like.

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
 new Conv(networkConfig, [convConfig], function(blogWidget) {}); 
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
CollectionMeta is an encoded JSON object. In the above example, the JSON object takes the following format before it’s JWT encoded:

```
{ 
"url": "http://dev.livefyre.com/articles/test.html", 
"articleId": "1", 
"type": "liveblog", 
"title": "Title 1" 
}
```
## Adding an Event Handler {#section_e2h_qb2_d1b}

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
For more information, and for a list of available events, see Reference &gt; [ Javascript Events ](https://answers.livefyre.com/developers/reference/app-customizations/javascript-events/).

