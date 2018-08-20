---
description: You can use Livefyre Identity with Facebook to allow users to use their Facebook logins to interact with Apps on your site.
seo-description: You can use Livefyre Identity with Facebook to allow users to use their Facebook logins to interact with Apps on your site.
seo-title: Create a Facebook App for Use with Livefyre Identity
solution: Experience Manager
title: Create a Facebook App for Use with Livefyre Identity
uuid: a96a3707-fdaa-4e40-9467-c8fc1d926094
index: y
internal: n
snippet: y
translate: y
---

# Create a Facebook App for Use with Livefyre Identity

To allow your users to log in with their Facebook credentials, Livefyre requires the following Facebook app information:

* App ID
* App Secret
To create a Facebook app for use with Livefyre Identity:

>1. Go to [ https://developers.facebook.com/apps](https://developers.facebook.com/apps).
>1. Log into your Facebook developer account.
>1. Click **[!UICONTROL  Add New App]** or select an existing App for use with Livefyre Identity.
>1. Click **[!UICONTROL  Settings]**, then **[!UICONTROL  Basic]**. Enter a **[!UICONTROL  Contact Email]** address, **[!UICONTROL  Display Name]**, **[!UICONTROL  Privacy Policy URL]**, and **[!UICONTROL  Terms of Service URL]**.
>1. Click the plus sign ( **[!UICONTROL  +]**) next to **[!UICONTROL  Products]**.
>1. Click on **[!UICONTROL  Set Up]** under **[!UICONTROL  Facebook Login]**.
>1. Click **[!UICONTROL  Settings]** and set up the following:
>    
>    * Set **[!UICONTROL  Client OAuth Login]** to **[!UICONTROL  Yes]**.
>    * Set **[!UICONTROL  Web OAuth Login]** to **[!UICONTROL  Yes]**.
>    * Set **[!UICONTROL  Use Strict Mode for Redirect URIs]** to **[!UICONTROL  Yes]**.
>    * Set **[!UICONTROL  Enforce HTTPS for Web OAuth Login]** to **[!UICONTROL  Yes]**.
>    * Under **[!UICONTROL  Valid OAuth redirect URLs]**, add the URL ` https://identity.livefyre.com/{networkName}/api/v1.0/public/profile/social/complete/facebook_fyre` (where ` {networkName}` is your Livefyre-provided network name).
>    
>1. Under **[!UICONTROL  App Review]**:
>    
>    * Make the App public.
>    * Ensure that the **[!UICONTROL  Approved Items]** for **[!UICONTROL  Login Permissions]** include ` email`, ` public_profile`, and ` user_friends`.
>    
