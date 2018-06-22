---
---

<a id="section_xyg_51w_sy"></a>

To implement this feature, pass in a 1-1 object mapping of the strings you wish to override to the Javascript configuration object. If you don’t provide a field, then the default text will be used.

Example:

```
var customStrings = { postAsButton: "New Post As Text", postEditButton: "New Post Edit Text"};networkConfig["strings"] = customStrings; fyre.conv.load( networkConfig, [convConfig], function(){});
```
