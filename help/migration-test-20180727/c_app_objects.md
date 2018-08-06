---
description: Create authentication tokens to use to authenticate users for an App using App Objects.
seo-description: Create authentication tokens to use to authenticate users for an App using App Objects.
seo-title: App Objects
title: App Objects
uuid: f0141795-46c9-4e2a-b174-711b61b617de
index: y
internal: n
snippet: y
translate: y
---

# App Objects

Set up `authDelegate` to connect your existing authentication system to Livefyre to allow your site visitors to use your existing site authentication with Livefyre Apps. For example, if a user wants to comment on a post, they have to log in to comment. You can use Livefyre's built-in authentication system or connect your Livefyre Apps to your existing login and password for your site.
Pass your `authDelegate` through the `auth.Delegate` function.
Use `authDelegate` to generate a `userAuth` token to allow users to log into your authentication system. 
To customize Livefyre and Livefyre Apps with your existing identity and network system, you have to create a token, pass that token through two functions, then create an additional token to connect your system with Livefyre.
You must use the `CollectionMeta` function and `authDelegate` function to connect 
