---
description: Use Livefyre.js to add page-wide authentication for your Livefyre Apps.
seo-description: Use Livefyre.js to add page-wide authentication for your Livefyre Apps.
seo-title: Add Authetication to an App using Livefyre.js
title: Add Authetication to an App using Livefyre.js
---

# Add Authetication to an App using Livefyre.js

Livefyre.js Auth is a JavaScript package developed by Livefyre that enables all the Apps on your website to share a single authentication integration. Auth allows you to define how your users should register, log in, and log out by delegating these flows to an AuthDelegate object that you define.

## Step 1: Enable Authentication for a Page {#section_pgp_jtt_bbb}

Use Livefyre.js to enable authentication for a page in order to allow users to log in and interact with Apps using your existing authentication system.

   1.
   To enable authentication on a page, add Livefyre.js to the &lt;head&gt; element of your webpage or website template.
   
   ```
   &lt;script src="//cdn.livefyre.com/Livefyre.js"&gt;&lt;/script&gt;
   ```
   
   1.
   Use Livefyre.require to enable authentication. Using Livefyre.require is similar to using require to call other packages. The integration code to require auth looks like this:
   
   ```
   Livefyre.require(['auth'], function (auth) { // Do authy things...});
   ```
   
## Step 2: Register an AuthDelegate {#section_oqm_15t_bbb}

To enable authentication create an `codeph  AuthDelegate` and pass it to `codeph  Livefyre.js` Authentication.

An `codeph  AuthDelegate` is an object you define that determines how users will log in, log out, and view profiles.

1. Create an `codeph  AuthDelegate`. The way you construct an `codeph  AuthDelegate` depends on your identity provider. See Identity Integration for more detailed instructions.
1. Pass the `codeph  AuthDelegate` to `codeph  Livefyre.js` Authentication. The simplest `codeph  AuthDelegate` logs the same user in whenever a user triggered the delegated login method from an App:
   ```
   Livefyre.require(['auth'], function (auth) { 
    auth.delegate({ 
    login: function (errback) { 
    errback(null, { livefyre: '&lt;userAuthToken&gt;' }); 
    } 
    }); 
   });
   ```
   
## Step 3: Synchronize User Data {#section_u4m_j5t_bbb}

Synchronize the user profile information between Livefyre and your identity provider.

If you’re not using [ Livefyre Enterprise Profiles ](c_livefyre_enterprise_profiles.md#c_livefyre_enterprise_profiles), you must synchronize your user profile information between Livefyre and your Identity Provider. For more information, see:

* [ Your Identity Service ](c_your_identity_service.md#c_your_identity_service)
* [ Janrain Capture Integration ](c_janrain_capture_backplane.md#c_janrain_capture_backplane)
