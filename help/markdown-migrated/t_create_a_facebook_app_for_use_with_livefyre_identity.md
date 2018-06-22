---
description: You can use Livefyre Identity with Facebook to allow users to use their Facebook logins to interact with Apps on your site.
seo-description: You can use Livefyre Identity with Facebook to allow users to use their Facebook logins to interact with Apps on your site.
seo-title: Create a Facebook App for Use with Livefyre Identity
solution: Experience Manager
title: Create a Facebook App for Use with Livefyre Identity
---

# Create a Facebook App for Use with Livefyre Identity

To allow your users to log in with their Facebook credentials, Livefyre requires the following Facebook app information:

* App ID
* App Secret
To create a Facebook app for use with Livefyre Identity:

>1. Go to [https://developers.facebook.com/apps](https://developers.facebook.com/apps).
>   
>1. Log into your Facebook developer account.
>   
>1. Click `uicontrol Add New App` or select an existing App for use with Livefyre Identity.
>   
>1. Click `uicontrol Settings`, then `uicontrol Basic`. Enter a `uicontrol Contact Email` address, `uicontrol Display Name`, `uicontrol Privacy Policy URL`, and `uicontrol Terms of Service URL`.
>   
>1. Click the plus sign (`uicontrol +`) next to `uicontrol Products`.
>   
>1. Click on `uicontrol Set Up` under `uicontrol Facebook Login`.
>   
>1. Click `uicontrol Settings` and set up the following:
>* Set `uicontrol Client OAuth Login` to `uicontrol Yes`.
>* Set `uicontrol Web OAuth Login` to `uicontrol Yes`.
>* Set `uicontrol Use Strict Mode for Redirect URIs` to `uicontrol Yes`.
>* Set `uicontrol Enforce HTTPS for Web OAuth Login` to `uicontrol Yes`.
>* Under `uicontrol Valid OAuth redirect URLs`, add the URL`codeph https://identity.livefyre.com/{networkName}/api/v1.0/public/profile/social/complete/facebook_fyre` (where `codeph {networkName}` is your Livefyre-provided network name).
>   
>   
>1. Under `uicontrol App Review`:
>* Make the App public.
>* Ensure that the `uicontrol Approved Items` for `uicontrol Login Permissions` include `codeph email`, `codeph public_profile`, and `codeph user_friends`.
>   
>   
>   
