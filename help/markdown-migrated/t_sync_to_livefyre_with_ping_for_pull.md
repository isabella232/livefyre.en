---
description: 
seo-description: 
seo-title: Sync to Livefyre with Ping for Pull
title: Sync to Livefyre with Ping for Pull
---

# Sync to Livefyre with Ping for Pull

**Step 4: Sync to Livefyre with Ping for Pull**

Keeping Livefyre Remote Profiles in sync with your Capture user management system involves a series of steps referred to as Ping for Pull. This process requires that you obtain a valid access token from Janrain, and then pass that token to an endpoint specified in step 3, below.

>1. Get an access code from Janrain.
>   To get the access code, supply the necessary credentials, specify the user_type as “user”, and the uuid as the current user’s uuid to update. For more information, see[http://developers.janrain.com/rest-api/methods/authentication/access-codes-and-tokens/getauthorizationcode/](http://developers.janrain.com/rest-api/methods/authentication/access-codes-and-tokens/getauthorizationcode/)
>   
>1. Trade the access code for an access token. Supply the necessary credentials, the access code received from step 1, and specify the grant_type as “authorization_code”.
>   For more information, see[http://developers.janrain.com/rest-api/methods/authentication/oauth/token/](http://developers.janrain.com/rest-api/methods/authentication/oauth/token/)
>   
>1. Hit the Livefyre “Ping to Pull Capture” endpoint.
>   Endpoint URL:`filepath http://{networkName}/api/v1.1/private/capture/profile_updated/?jrtoken={token}` where ***{networkName}*** is the network name provided to you by Livefyre, and the jrtoken is the token received from Janrain in step 2.
>       
>   
>   
