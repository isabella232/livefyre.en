---
description: Create authentication tokens to use to authenticate users for an App using App Objects.
seo-description: Create authentication tokens to use to authenticate users for an App using App Objects.
seo-title: App Objects
title: App Objects
---

# App Objects

Set up `codeph authDelegate` to connect your existing authentication system to Livefyre to allow your site visitors to use your existing site authentication with Livefyre Apps. For example, if a user wants to comment on a post, they have to log in to comment. You can use Livefyre's built-in authentication system or connect your Livefyre Apps to your existing login and password for your site.

Pass your `codeph authDelegate` through the `codeph auth.Delegate` function.

Use `codeph authDelegate` to generate a `codeph userAuth` token to allow users to log into your authentication system.

To customize Livefyre and Livefyre Apps with your existing identity and network system, you have to create a token, pass that token through two functions, then create an additional token to connect your system with Livefyre.

You must use the `codeph CollectionMeta` function and `codeph authDelegate` function to connect

