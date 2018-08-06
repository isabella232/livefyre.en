---
description: Use Livefyre.js to enable authentication for a page in order to allow users to log in and interact with Apps using your existing authentication system.
seo-description: Use Livefyre.js to enable authentication for a page in order to allow users to log in and interact with Apps using your existing authentication system.
seo-title: Enable Authentication for a Page
title: Enable Authentication for a Page
uuid: 2852e181-4371-48f4-8856-4924dea16c64
index: y
internal: n
snippet: y
translate: y
---

# Enable Authentication for a Page


>1. To enable authentication on a page, add Livefyre.js to the &lt;head&gt; element of your webpage or website template.
>
>   ```
>   <script src="//cdn.livefyre.com/Livefyre.js"></script>
>   ```
>
>1. Use Livefyre.require to enable authentication. Using Livefyre.require is similar to using require to call other packages. The integration code to require auth looks like this:
>
>   ```
>   Livefyre.require(['auth'], function (auth) { // Do authy things...});
>   ```
>
