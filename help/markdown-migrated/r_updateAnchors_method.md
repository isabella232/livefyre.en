---
---

<a id="section_efb_tk4_sy"></a>

This method is useful for pagination, or in other cases where sidenote-able content is added to the page dynamically. This method defines new anchors for the matched elements, and takes a single argument: `codeph  newSelectors`.

`codeph  newSelectors`. The selectors to add to Sidenotes. This may be a selector string, a jQuery object, or an array of elements (any of the types accepted by the selectors argument passed during app construction).

Format:

```
app.updateAnchors(newSelectors);
```
Example:

```
var app = new Livefyre.Sidenotes(convConfig);// Load more contentapp.updateAnchors('#content');
```
