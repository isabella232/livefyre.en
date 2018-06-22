---
description: The Livefyre for AEM package includes an out-of-the-box integration between AEM Identity Management’s User Profiles and Livefyre’s SSO service.
seo-description: The Livefyre for AEM package includes an out-of-the-box integration between AEM Identity Management’s User Profiles and Livefyre’s SSO service.
seo-title: Customize Single Sign-on Integration
title: Customize Single Sign-on Integration
---

# Customize Single Sign-on Integration

When users log into your AEM site, they are also logged into Livefyre social components, and when a logged-out user attempts to use a Livefyre component feature that requires authentication (like uploading a photo), the Livefyre component can initiate user authentication.

The default authentication integration may not be perfect for every site. To best match the authentication flow in your site templates, you may want to override the default Livefyre Authentication Delegate to meet your needs.

>1. Using CRXDE Lite, copy `codeph /libs/social/integrations/livefyre/components/authorizablecomponent/authclientlib` to `codeph /apps/social/integrations/livefyre/components/authorizablecomponent/authclientlib`
>   
>   
>1. Edit and save`codeph /apps/social/integrations/livefyre/components/authorizablecomponent/authclientlib/auth.js` to implement a Livefyre Auth Delegate that meets your needs.
>   For more information on customizing an Auth Delegate, see Identity Integration on answers.livefyre.com.
>   
>   For more on AEM Clientlibs, see Using Client-Side Libraries on docs.adobe.com.
>   
>   
>   
>   
