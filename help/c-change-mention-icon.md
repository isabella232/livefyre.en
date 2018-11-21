---
description: Change the icon displayed for Livefyre users in the @mention pulldown menu.
seo-description: Change the icon displayed for Livefyre users in the @mention pulldown menu.
seo-title: Change @mention Icon
solution: Experience Manager
title: Change @mention Icon
uuid: 825fe655-775d-444d-aff5-27db07cb227d
index: y
internal: n
snippet: y
---

# Change @mention Icon{#change-mention-icon}

Change the icon displayed for Livefyre users in the @mention pulldown menu.

Change the Livefyre icon used in the @mention pulldown menu to an icon of your choosing, allowing you to indicate your community members with your own icon.

**Example**

To change this icon, add the following CSS to your stylesheet. Replace ***<your resource url>*** with the URL of the image selected to replace the default Livefyre badge.

```
.fyre-editor-container .fyre-editor-toolbar > .fyre-mention-menu .fyre-mention-item .fyre-mention-item-livefyre { 
    background: url(<your resource url>) no-repeat center; 
    background-position: 0px 0px; 
    background-size: 22px 22px; 
}
```

