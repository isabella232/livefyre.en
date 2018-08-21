---
description: You can use Livefyre Identity with Microsoft Live Identity to allow users to use their Facebook logins to interact Apps on your site.
seo-description: You can use Livefyre Identity with Microsoft Live Identity to allow users to use their Facebook logins to interact Apps on your site.
seo-title: Create a Microsoft Live Identity App for Use with Livefyre Identity
solution: Experience Manager
title: Create a Microsoft Live Identity App for Use with Livefyre Identity
uuid: 6d7b6e42-d8c2-4f0b-a7ba-c69f727cf3ed
index: y
internal: n
snippet: y
translate: y
---

# Create a Microsoft Live Identity App for Use with Livefyre Identity

To allow users to log in with their Microsoft Live Identity credentials, Livefyre requires the following Microsoft Live Identity Information:

* Client ID (Private Key)
* Client Secret (Password)
To create an Microsoft Live Identity app for use with Livefyre Identity:

>1. Create or sign in to a Microsoft Live account at [ https://apps.dev.microsoft.com](https://apps.dev.microsoft.com/)
>1. Create a new or select an existing app for use with Livefyre Identity.
>1. Click **[!UICONTROL  Add Platform]**, then select Web as the platform type.
>1. Make sure the **[!UICONTROL  Allow Implicit Flow]** option is checked and enter the Redirect URL, using your network name instead of {network-name}: https://identy.livefyre.com/{network-name}.fyre.co/api/v.1.0/public/profile/social/complete/mslive_fyre.
>1. Generate a new password/key pair to get the Private Key.
>1. In **[!UICONTROL  Livefyre Integration Settings Livefyre Identity Microsoft Live]**, switch the **[!UICONTROL  Enable Microsoft Live Login]** toggle to **[!UICONTROL  On]**.
>1. Enter the Microsoft Live Client ID and Microsoft Live Client Secret.
>1. Click **[!UICONTROL  Save Settings]**.
>When complete,Microsoft Live Identity’s app details page will list the app’s Client ID (Consumer Key) and Client Secret (Consumer Secret) for use in Studio’s Integration Settings page.
