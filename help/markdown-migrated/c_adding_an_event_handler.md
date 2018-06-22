---
description: To register event handlers, use the widget.on call within the App’s callback function.
seo-description: To register event handlers, use the widget.on call within the App’s callback function.
seo-title: Adding an Event Handler
solution: Experience Manager
title: Adding an Event Handler
---

# Adding an Event Handler

For example:

```javascript
Livefyre.require(['fyre.conv#3'], function(Conv) { 
 new Conv(networkConfig, [convConfig], function(widget) { 
 widget.on('&lt;strong&gt;&lt;eventName&gt;&lt;/strong&gt;', function (data) { 
 // Do something, perhaps using data 
 }); 
 }); 
}); 

```
For more information, and for a list of available events, see Reference &gt; Javascript Events.

