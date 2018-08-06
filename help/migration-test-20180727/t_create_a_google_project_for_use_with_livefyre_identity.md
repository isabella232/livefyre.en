---
description: You can use Livefyre Identity with Google to allow users to use their Google logins to interact with Apps on your site.
seo-description: You can use Livefyre Identity with Google to allow users to use their Google logins to interact with Apps on your site.
seo-title: Create a Google Project for Use with Livefyre Identity
solution: Experience Manager
title: Create a Google Project for Use with Livefyre Identity
uuid: c41e6c94-c800-4d45-a361-729c0ac33fe5
index: y
internal: n
snippet: y
translate: y
---

# Create a Google Project for Use with Livefyre Identity

To allow your users to log in with their Google credentials, Livefyre requires the following Google Project information:

* Client ID
* Client Secret
To create a Google Project for use with Livefyre Identity:

>1. Go to [https://console.cloud.google.com/project](https://console.cloud.google.com/project) and log into your Google account to create a new or select an existing app for use with Livefyre Identity.
>1. From within the project Dashboard for the app, click ** `Enable and Manage APIs` **.
>1. From the API Overview page, under Social APIs, click to enable the Google+ API.
>1. From the API Credentials page, select ** `Credentials > New credentials > OAuth` ** client ID. In the ** `Create client ID` ** page that opens:
>    
>    * Select Application type: Web application.
>    * Enter a ** `Name` ** for the ** `Client ID` **.
>    * Leave ** `Authorized JavaScript origins` ** field blank.
>    * Enter ** `Authorized redirect URIs` **: https://identity.livefyre.com/{networkName}.fyre.co/api/v1.0/public/profile/social/complete/google_fyre (where ** `{networkName}` ** is your Livefyre provided network name. For example: ** `labs` ** in ** `labs.fyre.co` **.)
>    * Click ** `Create` ** to save your credentials.
>    
