---
description: Use Livefyre.js to enable authentication for a page in order to allow users to log in and interact with Apps using your existing authentication system.
seo-description: Use Livefyre.js to enable authentication for a page in order to allow users to log in and interact with Apps using your existing authentication system.
seo-title: Enable Authentication for a Page
title: Enable Authentication for a Page
---

# Enable Authentication for a Page

>1. To enable authentication on a page, add Livefyre.js to the &lt;head&gt; element of your webpage or website template.
>   ```
>   &lt;script src="//cdn.livefyre.com/Livefyre.js"&gt;&lt;/script&gt;
>   ```
>   
>   
>1. Use Livefyre.require to enable authentication. Using Livefyre.require is similar to using require to call other packages. The integration code to require auth looks like this:
>   ```
>   Livefyre.require(['auth'], function (auth) { // Do authy things...});
>   ```
>   
>   
>   
