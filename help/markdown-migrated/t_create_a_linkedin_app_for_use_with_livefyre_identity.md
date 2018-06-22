---
description: You can use Livefyre Identity with LinkedIn to allow users to use their LinkedIn logins to interact Apps on your site.
seo-description: You can use Livefyre Identity with LinkedIn to allow users to use their LinkedIn logins to interact Apps on your site.
seo-title: Create a LinkedIn App for Use with Livefyre Identity
solution: Experience Manager
title: Create a LinkedIn App for Use with Livefyre Identity
---

# Create a LinkedIn App for Use with Livefyre Identity

To enable LinkedIn login, Livefyre requires the following LinkedIn app information:

* Consumer Key (API Key)
* Consumer Secret (API Secret)
To create a LinkedIn App for use with Livefyre Identity:

>1. Go to https://www.linkedin.com/secure/developer, and sign into your LinkedIn account to create a new or select an existing app for use with Livefyre Identity.
>   
>1. Click `uicontrol Create Application`.
>   
>1. Complete the form to create the Application.
>   
>1. In the `uicontrol Default Application Permissions`, enable the `uicontrol r_basicprofile` and `uicontrol r_emailaddress` app permissions.
>   
>1. Enter the `uicontrol OAuth 2.0 Authorized Redirect URL` as https://identity.livefyre.com/{network-name}.fyre.co/api/v1.0/public/profile/social/complete/linkedin_fyre.
>   
>1. Save the app.
>   
>1. In `uicontrol Livefyre &gt; Integration Settings &gt; Livefyre Identity &gt; LinkedIn`, switch the `uicontrol Enable LinkedIn Login` toggle to `uicontrol On`.
>   
>1. Enter the LinkedIn Client ID and LinkedIn Client Secret.
>   
>1. Click `uicontrol Save Settings`.
>   
>   
