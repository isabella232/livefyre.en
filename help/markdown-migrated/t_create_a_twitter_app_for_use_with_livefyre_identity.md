---
description: You can use Livefyre Identity with Twitter to allow users to use their Twitter logins to interact Apps on your site.
seo-description: You can use Livefyre Identity with Twitter to allow users to use their Twitter logins to interact Apps on your site.
seo-title: Create a Twitter App for Use with Livefyre Identity
solution: Experience Manager
title: Create a Twitter App for Use with Livefyre Identity
---

# Create a Twitter App for Use with Livefyre Identity

To enable Twitter login, Livefyre requires the following Twitter app information:

* Consumer Key (API Key)
* Consumer Secret (API Secret)
To create a Twitter App for use with Livefyre Identity:

>1. Go to [https://apps.twitter.com/](https://apps.twitter.com/), and sign into your Twitter account to create a new or select an existing app for use with Livefyre Identity.
>   
>1. From the Settings page for the app:
>* Enter `uicontrol Callback URL:` https://identity.livefyre.com/{networkName}.fyre.co (where **{networkName}** is your Livefyre provided network name. For example: `uicontrol labs` in `uicontrol labs.fyre.co`.)
>* Deselect `uicontrol Enable Callback Locking`.
>* Select `uicontrol Allow this application to be used to Sign in with Twitter`.
>   
>   
>1. From the `uicontrol Permissions` tab, select `uicontrol Access: Read only`.
>   
>   
