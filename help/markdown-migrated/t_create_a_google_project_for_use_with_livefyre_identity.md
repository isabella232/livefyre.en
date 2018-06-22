---
description: You can use Livefyre Identity with Google to allow users to use their Google logins to interact with Apps on your site.
seo-description: You can use Livefyre Identity with Google to allow users to use their Google logins to interact with Apps on your site.
seo-title: Create a Google Project for Use with Livefyre Identity
solution: Experience Manager
title: Create a Google Project for Use with Livefyre Identity
---

# Create a Google Project for Use with Livefyre Identity

To allow your users to log in with their Google credentials, Livefyre requires the following Google Project information:

* Client ID
* Client Secret
To create a Google Project for use with Livefyre Identity:

>1. Go to [https://console.cloud.google.com/project](https://console.cloud.google.com/project) and log into your Google account to create a new or select an existing app for use with Livefyre Identity.
>   
>1. From within the project Dashboard for the app, click `uicontrol Enable and Manage APIs`.
>   
>1. From the API Overview page, under Social APIs, click to enable the Google+ API.
>   
>1. From the API Credentials page, select `uicontrol Credentials &gt; New credentials &gt; OAuth` client ID. In the `uicontrol Create client ID` page that opens:
>* Select Application type: Web application.
>* Enter a `uicontrol Name` for the `uicontrol Client ID`.
>* Leave `uicontrol Authorized JavaScript origins` field blank.
>* Enter `uicontrol Authorized redirect URIs`: https://identity.livefyre.com/{networkName}.fyre.co/api/v1.0/public/profile/social/complete/google_fyre (where `uicontrol {networkName}` is your Livefyre provided network name. For example: `uicontrol labs` in `uicontrol labs.fyre.co`.)
>* Click `uicontrol Create` to save your credentials.
>   
>   
>   
