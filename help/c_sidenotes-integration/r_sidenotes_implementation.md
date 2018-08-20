---
description: Implement Sidenotes using .js implementation.
seo-description: Implement Sidenotes using .js implementation.
seo-title: Sidenotes Implementation
solution: Experience Manager
title: Sidenotes Implementation
uuid: f6245f5c-ff6e-4f51-8792-09a86211b37e
index: y
internal: n
snippet: y
translate: y
---

# Sidenotes Implementation


<a id="section_xyg_51w_sy"></a>

To implement this feature, pass in a 1-1 object mapping of the strings you wish to override to the Javascript configuration object. If you don’t provide a field, then the default text will be used.

Example:

```
var customStrings = { postAsButton: "New Post As Text", postEditButton: "New Post Edit Text"};networkConfig["strings"] = customStrings; fyre.conv.load( networkConfig, [convConfig], function(){});
```
