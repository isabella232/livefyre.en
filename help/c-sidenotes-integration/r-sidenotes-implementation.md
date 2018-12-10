---
description: Implement Sidenotes using .js implementation.
seo-description: Implement Sidenotes using .js implementation.
seo-title: Sidenotes Implementation
solution: Experience Manager
title: Sidenotes Implementation
uuid: 4d6f87a9-93a1-4d22-9231-d60dfc96a620
index: y
internal: n
snippet: y
---

# Sidenotes Implementation{#sidenotes-implementation}

Implement Sidenotes using .js implementation.

<a id="section_xyg_51w_sy"></a>

To implement this feature, pass in a 1-1 object mapping of the strings you wish to override to the Javascript configuration object. If you don’t provide a field, then the default text will be used.

Example:

```
var customStrings = { postAsButton: "New Post As Text", postEditButton: "New Post Edit Text"};networkConfig["strings"] = customStrings; fyre.conv.load( networkConfig, [convConfig], function(){});
```

