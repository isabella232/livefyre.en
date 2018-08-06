---
description: Use the updateAnchors method to add sidenoted content to the page dynamically.
seo-description: Use the updateAnchors method to add sidenoted content to the page dynamically.
seo-title: updateAnchors Method
solution: Experience Manager
title: updateAnchors Method
uuid: 082be6b2-e625-4ad6-bdf7-6bbbb78bbd0a
index: y
internal: n
snippet: y
translate: y
---

# updateAnchors Method


<a id="section_efb_tk4_sy"></a>

This method is useful for pagination, or in other cases where sidenote-able content is added to the page dynamically. This method defines new anchors for the matched elements, and takes a single argument: ` newSelectors`.
` newSelectors`. The selectors to add to Sidenotes. This may be a selector string, a jQuery object, or an array of elements (any of the types accepted by the selectors argument passed during app construction).
Format:

```
app.updateAnchors(newSelectors);
```
Example:

```
var app = new Livefyre.Sidenotes(convConfig);// Load more contentapp.updateAnchors('#content');
```
