---
description: Livefyre.js is a small base library that provides authentication for Apps on your site.
seo-description: Livefyre.js is a small base library that provides authentication for Apps on your site.
seo-title: Add Livefyre.js to the Page
title: Add Livefyre.js to the Page
---

# Add Livefyre.js to the Page


>## App Objects {#c_app_objects}
>Create authentication tokens to use to authenticate users for an App using App Objects.

<!-- c_app_objects.dita -->
Set up `codeph authDelegate` to connect your existing authentication system to Livefyre to allow your site visitors to use your existing site authentication with Livefyre Apps. For example, if a user wants to comment on a post, they have to log in to comment. You can use Livefyre's built-in authentication system or connect your Livefyre Apps to your existing login and password for your site.

Pass your `codeph authDelegate` through the `codeph auth.Delegate` function.

Use `codeph authDelegate` to generate a `codeph userAuth` token to allow users to log into your authentication system.

To customize Livefyre and Livefyre Apps with your existing identity and network system, you have to create a token, pass that token through two functions, then create an additional token to connect your system with Livefyre.

You must use the `codeph CollectionMeta` function and `codeph authDelegate` function to connect


>## Add Livefyre.js to the Page {#t_add_livefyre.js_to_the_page}
>Livefyre.js is a small base library that provides authentication for Apps on your site.

<!-- t_add_livefyre.js_to_the_page.dita -->
To enable authentication:

>1. Add Livefyre.js to the `codeph &lt;head&gt;` element of your webpage or website template.
>   
>1. Add one of the following to your page:
>* `codeph globalwindow.Livefyre` variable
>* `codeph Livefyre.require` to load other Livefyre packages on demand
>   ```
>   &lt;script src="//cdn.livefyre.com/Livefyre.js"&gt;&lt;/script&gt;
>   ```
>   
>   
>   
