---
description: You can use Livefyre Identity with Twitter to allow users to use their Twitter logins to interact Apps on your site.
seo-description: You can use Livefyre Identity with Twitter to allow users to use their Twitter logins to interact Apps on your site.
seo-title: Create a Twitter App for Use with Livefyre Identity
solution: Experience Manager
title: Create a Twitter App for Use with Livefyre Identity
uuid: 12cf3159-dd64-47a7-a206-27cb9f92b900
index: y
internal: n
snippet: y
translate: y
---

# Create a Twitter App for Use with Livefyre Identity

You can use Livefyre Identity with Twitter to allow users to use their Twitter logins to interact Apps on your site.

To enable Twitter login, Livefyre requires the following Twitter app information:

* Consumer Key (API Key)
* Consumer Secret (API Secret)

To create a Twitter App for use with Livefyre Identity:

1. Go to [https://apps.twitter.com/](https://apps.twitter.com/), and sign into your Twitter account to create a new or select an existing app for use with Livefyre Identity.
1. From the Settings page for the app:

    * Enter **[!UICONTROL Callback URL:]** `https://identity.livefyre.com/{networkName}.fyre.co/api/v1.0/public/profile/social/complete/twitter_fyre` (where **{networkName}** is your Livefyre provided network name. For example: **[!UICONTROL labs]** in **[!UICONTROL labs.fyre.co]**.)
    
    * Deselect **[!UICONTROL Enable Callback Locking]**.
    * Select **[!UICONTROL Allow this application to be used to Sign in with Twitter]**.

1. From the **[!UICONTROL Permissions]** tab, select **[!UICONTROL Access: Read only]**.
>When complete, Twitter’s Application Management > Keys and Access Tokens page will list the app’s Consumer Key (API Key) and Consumer Secret (API Secret) for use in Studio’s Integration Settings page.
