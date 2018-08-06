---
description: You can style your Livefyre Apps to behave in various ways or change them to look and feel like the rest of your brand campaign.
seo-description: You can style your Livefyre Apps to behave in various ways or change them to look and feel like the rest of your brand campaign.
seo-title: Styling Features
solution: Experience Manager
title: Styling Features
uuid: 7d95e189-823e-423d-a542-94b5eec16261
index: y
internal: n
snippet: y
translate: y
---

# Styling Features

## Styling Features {#c_styling_features}You can style your Livefyre Apps to behave in various ways or change them to look and feel like the rest of your brand campaign.On this page:

* [](#c_styling_features/section_yjl_rfs_d1b)
* [](#c_styling_features/section_kl2_n4s_d1b)
* [](#c_styling_features/section_yng_n4s_d1b)
* [](#c_styling_features/section_dnc_s4s_d1b)
* [](#c_styling_features/section_ldf_s4s_d1b)
* [](#c_avatars)
* [](#c_hovercards)
* [](#c_user_badges)
* [](#t_add_user_tags)
<!-- c_styling_features.dita --> 
## Default Styling {#section_yjl_rfs_d1b}

You can style an App in Studio in the App Designer without having to use livefyre.js to customize the App.
Apps that use this feature:

* [Carousel](c_carousel_app.md#c_carousel_app)
* [Chat](c_chat_app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Feature Card](c_feature_card_app.md#c_feature_card_app)
* [Map](c_map_app.md#c_map_app)
* [Media Wall](c_media_wall_app.md#c_media_wall_app)
* [Mosaic](c_mosaic_app.md#c_mosaic_app)
* [Polls](c_polls_app.md#c_polls_app)
* [Reviews](c_reviews_app.md#c_reviews_app)
* [Sidenotes](c_sidenotes_app.md#c_sidenotes_app)
* [Storify 2](c_storify2.md#c_storify2)
* [Trending](c_trending_app.md#c_trending_app)
* [Upload Button](c_upload_button_app.md#c_upload_button_app)

## Animation {#section_kl2_n4s_d1b}

You can animate an App using CSS.
Apps that use this feature:

* [Chat](c_chat_app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)

## CSS Styling and Branding {#section_yng_n4s_d1b}

Use CSS to style elements of a Livefyre App to fit your brand.
Livefyre apps offer an extensive CSS styling interface, allowing you to customize your user experience to meet your current design standards.
Styling options include:

* ** `Styling the Stream:` ** Livefyre streams may be styled and customized to fit your brand, and the rest of your site. For more information, see CSS Customizations.
* ** `Styling the Comment Editor:` ** The comment editor may be customized by changing the color, size and family for your font, or by changing the background color for the comment box. For more information, see Editor CSS.
* ** `Moving the Livefyre Logo:` ** While the default location for the Livefyre logo is at the top of the stream, this image may be removed, and replaced with a smaller “Powered by Livefyre” logo at the bottom of the stream. For more information, see Moving the Livefyre Logo.
* ** `Hiding elements of the stream:` ** Elements of the stream may be hidden if they are not relevant to your community. Elements which may be removed include the reply button, edit profile menu, logout menu, comment notifier, and user avatars. For more information on removing these elements, see Hiding App Elements.
* ** `Customizing the Friend Tagging Logo:` ** By default, the Livefyre logo is displayed in the friend tagging dropdown list for all users who have commented in the stream on the page. To replace this image with your own logo, please see Branding in Studio.
Apps that use this feature:

* [Carousel](c_carousel_app.md#c_carousel_app)
* [Chat](c_chat_app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Feature Card](c_feature_card_app.md#c_feature_card_app)
* [Map](c_map_app.md#c_map_app)
* [Media Wall](c_media_wall_app.md#c_media_wall_app)
* [Mosaic](c_mosaic_app.md#c_mosaic_app)
* [Polls](c_polls_app.md#c_polls_app)
* [Reviews](c_reviews_app.md#c_reviews_app)
* [Sidenotes](c_sidenotes_app.md#c_sidenotes_app)
* [Storify 2](c_storify2.md#c_storify2)
* [Trending](c_trending_app.md#c_trending_app)
* [Upload Button](c_upload_button_app.md#c_upload_button_app)

## Date and Timestamp {#section_dnc_s4s_d1b}

Change the date and timestamp format to meet your needs.
By default, Livefyre Apps display a relative timestamp for posts to the stream (4 minutes ago, 5 hours ago, 8 days ago, 2 months ago).
You may customize the timestamp displayed using the Date and Timestamp Customization, which allows you to select from a list of available formats.
Apps that use this feature:

* [Carousel](c_carousel_app.md#c_carousel_app)
* [Chat](c_chat_app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Feature Card](c_feature_card_app.md#c_feature_card_app)
* [Map](c_map_app.md#c_map_app)
* [Media Wall](c_media_wall_app.md#c_media_wall_app)
* [Mosaic](c_mosaic_app.md#c_mosaic_app)
* [Reviews](c_reviews_app.md#c_reviews_app)
* [Sidenotes](c_sidenotes_app.md#c_sidenotes_app)
* [Storify 2](c_storify2.md#c_storify2)

## Manage Embedded Media {#section_ldf_s4s_d1b}

Define the sources from which users may post media, and those from which media posts will be banned.
By default, all media attachments can be embedded into comments. For a comprehensive list of supported providers, see embed.ly/providers.
Livefyre uses Embed.ly, and standard oEmbed protocols, to embed media in App streams, and will pass through all media data provided by its source.
Embed.ly will pass through all available information, including the media’s title, description, thumbnail, and embed code for any provided URL. The availability of these items varies by provider. For example: Facebook does not return thumbnails for its videos, and passes only an embeddable video. Clicking Play will start the video (similar to YouTube’s display format). Twitter passes only static images, and does not send down videos. Therefore, Twitter native videos may not be played from within a Livefyre stream.
You may prevent certain attachments from being embedded into comments when embedding the comment stream. You may also choose to hide all Embed.ly expansions on the network, site and conversation level using Studio, displaying only links to the media, not fully embedded media.
Apps that use this feature:

* [Feature Card](c_feature_card_app.md#c_feature_card_app)
* [Map](c_map_app.md#c_map_app)
* [Media Wall](c_media_wall_app.md#c_media_wall_app)
>## Avatars {#c_avatars}Allow users to customize the image that displays with their content.<!-- c_avatars.dita --> User avatars are displayed (by default) next to content in all Apps, and are pulled from the identity profile system used in your implementation. These avatars vary in size, according to the App in which they are displayed.
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

* [Carousel](c_carousel_app.md#c_carousel_app)
* [Chat](c_chat_app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Feature Card](c_feature_card_app.md#c_feature_card_app)
* [Map](c_map_app.md#c_map_app)
* [Media Wall](c_media_wall_app.md#c_media_wall_app)
* [Mosaic](c_mosaic_app.md#c_mosaic_app)
* [Reviews](c_reviews_app.md#c_reviews_app)
* [Storify 2](c_storify2.md#c_storify2)
>## Hovercards {#c_hovercards}Enable or disable user hovercards across your site.<!-- c_hovercards.dita --> The Livefyre Hovercard is a popup that displays a quick snapshot of user information, including display name, bio, social networks, user likes, profile page URL and a link to view their full profile. Hovercards are available for all Livefyre streams, including Comments, Live Blog, and Chat.

>[!NOTE]
>
>Hovercards may be switched on or off at the network level only, and are implemented or disabled across all sites under your custom network. Please contact your Account Manager if you would like hovercards switched on for your network.


## Viewing Hovercards {#section_zjl_jtk_wy}

When you hover over a user’s avatar on Comments, Live Blog or Chat, their Hovercard will appear.
Clicking ** `View Full Profile` ** will take the user to the full profile page for that user.

>[!NOTE]
>
>Hovercards display information included with your User Profile system. Any fields not included in that system will not be displayed in the hovercards. If you do not have public profile pages, no page will be displayed. If you wish to disable Hovercards for your custom network, please contact your Technical Account Manager.


<a id="section_blk_ccj_h1b"></a>

Apps that use this feature:

* [Chat](c_chat_app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Reviews](c_reviews_app.md#c_reviews_app)
* [Sidenotes](c_sidenotes_app.md#c_sidenotes_app)
>## User Badges {#c_user_badges}Use CSS with User Tags to create User Badges for members of your community.<!-- c_user_badges.dita --> User Badges are custom styling features, which allow you to style Livefyre content posted by specific user types (such as moderators, editors, or any other User Group you wish to define) to Livefyre Chat, Comments, Reviews, or Live Blog Apps. This allows you to highlight this content to your users.
Apps that use this feature:

* [Chat](c_chat_app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Reviews](c_reviews_app.md#c_reviews_app)
* [Sidenotes](c_sidenotes_app.md#c_sidenotes_app)
>## Add User Tags to an Account {#t_add_user_tags}Add a User Tag to the account to apply User Badges.
>1. <!-- t_add_user_tags.dita -->
Create Owners and Moderators through Studio to assign the ** `Moderator` ** User Tag to the account.
>1. Create user groups, then add users to them through Studio to apply Tags with the group name to the selected users.
>1. Apply User Tags directly to Accounts using the Add User Tag HTTP call or Ping for Pull.
