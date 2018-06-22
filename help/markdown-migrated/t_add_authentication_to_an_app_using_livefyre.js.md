---
description: Implement authentication for Livefyre Apps using a front-end JavaScript implementation.
seo-description: Implement authentication for Livefyre Apps using a front-end JavaScript implementation.
seo-title: Add Authentication to an App using Livefyre.js
title: Add Authentication to an App using Livefyre.js
---

# Add Authentication to an App using Livefyre.js

Use Livefyre.js to add page-wide authentication for your Livefyre Apps.

Livefyre.js Auth is a JavaScript package developed by Livefyre that enables all the Apps on your website to share a single authentication integration. Auth allows you to define how your users should register, log in, and log out by delegating these flows to an AuthDelegate object that you define.

Use Livefyre.js to enable authentication for a page in order to allow users to log in and interact with Apps using your existing authentication system.

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
