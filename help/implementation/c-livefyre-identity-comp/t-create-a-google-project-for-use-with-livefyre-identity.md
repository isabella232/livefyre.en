---
description: You can use Livefyre Identity with Google to allow users to use their Google logins to interact with Apps on your site.
seo-description: You can use Livefyre Identity with Google to allow users to use their Google logins to interact with Apps on your site.
seo-title: Create a Google Project for Use with Livefyre Identity
solution: Experience Manager
title: Create a Google Project for Use with Livefyre Identity
uuid: b0a6bb8a-abea-4f5c-92ed-026e60183e1d
index: y
internal: n
snippet: y
---

# Create a Google Project for Use with Livefyre Identity{#create-a-google-project-for-use-with-livefyre-identity}

You can use Livefyre Identity with Google to allow users to use their Google logins to interact with Apps on your site.

To allow your users to log in with their Google credentials, Livefyre requires the following Google Project information:

* Client ID
* Client Secret

To create a Google Project for use with Livefyre Identity:

1. Go to [https://console.cloud.google.com/project](https://console.cloud.google.com/project) and log into your Google account to create a new or select an existing app for use with Livefyre Identity.
1. From within the project Dashboard for the app, click **[!UICONTROL Enable and Manage APIs]**.
1. From the API Overview page, under Social APIs, click to enable the Google+ API.
1. From the API Credentials page, select **[!UICONTROL Credentials > New credentials > OAuth]** client ID. In the **[!UICONTROL Create client ID]** page that opens:

    * Select Application type: Web application.
    * Enter a **[!UICONTROL Name]** for the **[!UICONTROL Client ID]**.
    
    * Leave **[!UICONTROL Authorized JavaScript origins]** field blank.
    * Enter **[!UICONTROL Authorized redirect URIs]**: https://identity.livefyre.com/{networkName}.fyre.co/api/v1.0/public/profile/social/complete/google_fyre (where **[!UICONTROL {networkName}]** is your Livefyre provided network name. For example: **[!UICONTROL labs]** in **[!UICONTROL labs.fyre.co]**.)
    
    * Click **[!UICONTROL Create]** to save your credentials.

>When complete, Google’s API Manager > Credentials page will list the project’s Client ID and Client secret for use in Studio’s Integration Settings page.