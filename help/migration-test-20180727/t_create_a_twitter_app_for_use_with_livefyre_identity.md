---
description: You can use Livefyre Identity with Twitter to allow users to use their Twitter logins to interact Apps on your site.
seo-description: You can use Livefyre Identity with Twitter to allow users to use their Twitter logins to interact Apps on your site.
seo-title: Create a Twitter App for Use with Livefyre Identity
solution: Experience Manager
title: Create a Twitter App for Use with Livefyre Identity
uuid: 6c10c5d9-bd4c-476e-8e21-75018b666d8d
index: y
internal: n
snippet: y
translate: y
---

# Create a Twitter App for Use with Livefyre Identity

To enable Twitter login, Livefyre requires the following Twitter app information:

* Consumer Key (API Key)
* Consumer Secret (API Secret)
To create a Twitter App for use with Livefyre Identity:

>1. Go to [https://apps.twitter.com/](https://apps.twitter.com/), and sign into your Twitter account to create a new or select an existing app for use with Livefyre Identity.
>1. From the Settings page for the app:
>    
>    * Enter ** `Callback URL:` ** https://identity.livefyre.com/{networkName}.fyre.co (where **{networkName}** is your Livefyre provided network name. For example: ** `labs` ** in ** `labs.fyre.co` **.)
>    * Deselect ** `Enable Callback Locking` **.
>    * Select ** `Allow this application to be used to Sign in with Twitter` **.
>    
>1. From the ** `Permissions` ** tab, select ** `Access: Read only` **.
