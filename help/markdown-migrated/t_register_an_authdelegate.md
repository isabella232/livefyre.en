---
description: To enable authentication create an AuthDelegate and pass it to Livefyre.js Authentication.
seo-description: To enable authentication create an AuthDelegate and pass it to Livefyre.js Authentication.
seo-title: Register an AuthDelegate
title: Register an AuthDelegate
---

# Register an AuthDelegate

An`codeph  AuthDelegate` is an object you define that determines how users will log in, log out, and view profiles.
>1. Create an `codeph  AuthDelegate`. The way you construct an `codeph  AuthDelegate` depends on your identity provider. See Identity Integration for more detailed instructions.
>   
>1. Pass the `codeph  AuthDelegate` to `codeph  Livefyre.js` Authentication. The simplest `codeph  AuthDelegate` logs the same user in whenever a user triggered the delegated login method from an App:
>   ```
>   Livefyre.require(['auth'], function (auth) { 
>    auth.delegate({ 
>    login: function (errback) { 
>    errback(null, { livefyre: '&lt;userAuthToken&gt;' }); 
>    } 
>    }); 
>   });
>   ```
>   
>   
>   
