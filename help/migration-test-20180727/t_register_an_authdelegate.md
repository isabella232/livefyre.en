---
description: To enable authentication create an AuthDelegate and pass it to Livefyre.js Authentication.
seo-description: To enable authentication create an AuthDelegate and pass it to Livefyre.js Authentication.
seo-title: Register an AuthDelegate
title: Register an AuthDelegate
uuid: f4865a7b-cfb0-4ed8-8aa5-be9e0ef16b26
index: y
internal: n
snippet: y
translate: y
---

# Register an AuthDelegate

An ` AuthDelegate` is an object you define that determines how users will log in, log out, and view profiles. 
>1. Create an ` AuthDelegate`. The way you construct an ` AuthDelegate` depends on your identity provider. See Identity Integration for more detailed instructions.
>1. Pass the ` AuthDelegate` to ` Livefyre.js` Authentication. The simplest ` AuthDelegate` logs the same user in whenever a user triggered the delegated login method from an App:
>
>   ```
>   Livefyre.require(['auth'], function (auth) { 
>      auth.delegate({ 
>         login: function (errback) { 
>            errback(null, { livefyre: '<userAuthToken>' }); 
>         }    
>      });  
>   });
>   ```
>
