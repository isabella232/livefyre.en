---
description: You can use Livefyre Identity with Facebook to allow users to use their Facebook logins to interact with Apps on your site.
seo-description: You can use Livefyre Identity with Facebook to allow users to use their Facebook logins to interact with Apps on your site.
seo-title: Create a Facebook App for Use with Livefyre Identity
solution: Experience Manager
title: Create a Facebook App for Use with Livefyre Identity
uuid: 0966cdb0-08fd-4a29-98d0-867ddef9457f
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

>1. Go to [https://developers.facebook.com/apps](https://developers.facebook.com/apps).
>1. Log into your Facebook developer account.
>1. Click ** `Add New App` ** or select an existing App for use with Livefyre Identity.
>1. Click ** `Settings` **, then ** `Basic` **. Enter a ** `Contact Email` ** address, ** `Display Name` **, ** `Privacy Policy URL` **, and ** `Terms of Service URL` **.
>1. Click the plus sign ( ** `+` **) next to ** `Products` **.
>1. Click on ** `Set Up` ** under ** `Facebook Login` **.
>1. Click ** `Settings` ** and set up the following:
>    
>    * Set ** `Client OAuth Login` ** to ** `Yes` **.
>    * Set ** `Web OAuth Login` ** to ** `Yes` **.
>    * Set ** `Use Strict Mode for Redirect URIs` ** to ** `Yes` **.
>    * Set ** `Enforce HTTPS for Web OAuth Login` ** to ** `Yes` **.
>    * Under ** `Valid OAuth redirect URLs` **, add the URL `https://identity.livefyre.com/{networkName}/api/v1.0/public/profile/social/complete/facebook_fyre` (where `{networkName}` is your Livefyre-provided network name).
>    
>1. Under ** `App Review` **:
>    
>    * Make the App public.
>    * Ensure that the ** `Approved Items` ** for ** `Login Permissions` ** include `email`, `public_profile`, and `user_friends`.
>    
