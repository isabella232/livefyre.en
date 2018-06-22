---
description: You can style your Livefyre Apps to behave in various ways or change them to look and feel like the rest of your brand campaign.
seo-description: You can style your Livefyre Apps to behave in various ways or change them to look and feel like the rest of your brand campaign.
seo-title: Styling Features
title: Styling Features
---

# Styling Features

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

* `uicontrol Styling the Stream:` Livefyre streams may be styled and customized to fit your brand, and the rest of your site. For more information, see CSS Customizations.
* `uicontrol Styling the Comment Editor:` The comment editor may be customized by changing the color, size and family for your font, or by changing the background color for the comment box. For more information, see Editor CSS.
* `uicontrol Moving the Livefyre Logo:` While the default location for the Livefyre logo is at the top of the stream, this image may be removed, and replaced with a smaller “Powered by Livefyre” logo at the bottom of the stream. For more information, see Moving the Livefyre Logo.
* `uicontrol Hiding elements of the stream:` Elements of the stream may be hidden if they are not relevant to your community. Elements which may be removed include the reply button, edit profile menu, logout menu, comment notifier, and user avatars. For more information on removing these elements, see Hiding App Elements.
* `uicontrol Customizing the Friend Tagging Logo:` By default, the Livefyre logo is displayed in the friend tagging dropdown list for all users who have commented in the stream on the page. To replace this image with your own logo, please see Branding in Studio.
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
