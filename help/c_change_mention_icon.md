---
description: Change the icon displayed for Livefyre users in the @mention pulldown menu.
seo-description: Change the icon displayed for Livefyre users in the @mention pulldown menu.
seo-title: Change @mention Icon
solution: Experience Manager
title: Change @mention Icon
uuid: a6ba7700-7c8f-4cb4-b6e8-26b58ef74424
index: y
internal: n
snippet: y
translate: y
---

# Change @mention Icon

Change the Livefyre icon used in the @mention pulldown menu to an icon of your choosing, allowing you to indicate your community members with your own icon.

**Example**

To change this icon, add the following CSS to your stylesheet. Replace ***&amp;lt;your resource url&amp;gt;*** with the URL of the image selected to replace the default Livefyre badge.

```
.fyre-editor-container .fyre-editor-toolbar > .fyre-mention-menu .fyre-mention-item .fyre-mention-item-livefyre { 
    background: url(<your resource url>) no-repeat center; 
    background-position: 0px 0px; 
    background-size: 22px 22px; 
}
```
