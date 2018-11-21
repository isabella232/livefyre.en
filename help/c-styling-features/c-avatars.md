---
description: Allow users to customize the image that displays with their content.
seo-description: Allow users to customize the image that displays with their content.
seo-title: Avatars
title: Avatars
uuid: ae1dc34d-81db-4858-929b-5c68d82dcc4a
index: y
internal: n
snippet: y
---

# Avatars{#avatars}

Allow users to customize the image that displays with their content.

User avatars are displayed (by default) next to content in all Apps, and are pulled from the identity profile system used in your implementation. These avatars vary in size, according to the App in which they are displayed.

(Livefyre allows you to Disable Avatars if you do not wish to display them in your Apps.)

>[!NOTE]
>
>Avatars are displayed at 25p x 25p for Chat, and 50p x 50p within most other Apps.

## Avatar storage {#section_zbh_x1f_wy}

Avatars are loaded asynchronously in Livefyre. When a user first signs into the App, or changes their associated avatar image file, their profile image is added to a task queue. (A default avatar is displayed temporarily while your user’s is uploaded to the Livefyre avatar storage location.)

## Gravatars {#section_mqh_p1f_wy}

Livefyre supports the use of Gravatars. If a user does not have a custom avatar as part of their user profile, Livefyre will check for a Gravatar for that user. If no Gravatar exists, the default avatar will be used.

If Comments has been embedded using the Livefyre WordPress Plugin, the user’s Gravatar will be used if the following conditions are met:

* Gravatar has been activated in the WordPress admin panel, and
* the user has a Gravatar account, and
* a custom avatar is not provided.

For more information, see the WordPress Gravatar documentation.

<a id="section_blk_ccj_h1b"></a>

Apps that use this feature:

* [Carousel](../c-carousel-app/c-carousel-app.md#c_carousel_app)
* [Chat](../c-chat-app/c-chat-app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Feature Card](../c-feature-card-app/c-feature-card-app.md#c_feature_card_app)
* [Map](../c-map-app/c-map-app.md#c_map_app)
* [Media Wall](../c-media-wall-app/c-media-wall-app.md#c_media_wall_app)
* [Mosaic](../c-mosaic-app/c-mosaic-app.md#c_mosaic_app)
* [Reviews](../c-reviews-app/c-reviews-app.md#c_reviews_app)
* [Storify 2](../c-storify2/c-storify2.md#c_storify2)

