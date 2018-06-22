---
description: Reposition the Livefyre logo on your page.
seo-description: Reposition the Livefyre logo on your page.
seo-title: Move the Livefyre Logo
solution: Experience Manager
title: Move the Livefyre Logo
---

# Move the Livefyre Logo

If your agreement with Livefyre allows, you may move the Livefyre logo from the top of the content stream to the bottom.

For example, add the following HTML to your page immediately following the element that contains the Livefyre App:

```
&lt;div id="powered_by_livefyre_new"&gt;&lt;a href="http://livefyre.com" target="_blank"&gt;Powered by Livefyre&lt;/a&gt;&lt;/div&gt;
```
Then, add the following to your page’s stylesheet:

```
/* Hide the top logo */ 
.fyre-widget .fyre-logo-drop, .fyre-widget .fyre-logo-help, .fyre-widget .fyre-help { 
 display:none !important; 
} 
 
/* Style the bottom logo */ 
#powered_by_livefyre_new a { background: url(https://cdn.livefyre.com/libs/fyre.conv/v3.0.0/images/poweredbylivefyre.png) no-repeat left top; 
 display: block; 
 height: 24px; 
 font: 13px "Helvetica Neue", Helvetica, Arial, Geneva, sans-serif; 
 text-decoration: none; 
 color: #404040; 
 padding-left: 28px; 
 padding-top: 4px; 
} 
#powered_by_livefyre_new a:hover { 
 text-decoration: underline; 
}
```
