---
description: Use embed.ly to display multiple media formats, directly in the App.
seo-description: Use embed.ly to display multiple media formats, directly in the App.
seo-title: Embedly Integration
solution: Experience Manager
title: Embedly Integration
uuid: 1f27e32c-c2c3-4f7c-93de-c9c7bf783d6a
index: y
internal: n
snippet: y
---

# Embedly Integration{#embedly-integration}

Use `embed.ly` to display multiple media formats, directly in the App.

To better enable embedded media content from a variety of sources, including Google Maps, YouTube, Flickr, Facebook, Instagram, Spotify, and Tumblr, Livefyre Apps use Embedly as a third-party provider for URL expansion. If a user or moderator includes a supported link in a post, the media included in the link will expand when posted to the Collection.

This provides Livefyre Apps with access to the more than 250 different embedded media options that Embedly supports.

>[!NOTE]
>
>Livefyre expands only a subset of Embedly’s full provider list. Embedded images will expand on HTTPS pages only if the provider is Twitter, YouTube, Imgur, Vine, Wikipedia, or SoundCloud. Please contact your Technical Account Manager for any further questions about link expansion or sources.

This page lists examples of some popular embedded media types, and their acceptable URL patterns. `Embed.ly` is continually adding new sources. For a complete list of providers, please go to `http://embed.ly/embed/features/providers`.

>[!NOTE]
>
>The Embedly formatting requires a full permalink. Shortened links will not work.

Only publicly viewable content is embeddable. If you attempt to embed a piece of content that is not public, the link to the content will appear in the blog post, and a placeholder icon will accompany it. When clicked, the link will take the reader to an error message from the service where the content is hosted, such as a Facebook message for a friends-only photo. Please contact your Account Manager if you notice that media is not expanded as expected.

## Sample Embedly URLs

|Type|Provider|URLs|
|--- |--- |--- |
|Maps|Google Maps|`http://maps.google.com/maps?*` <br/><ul><li>`http://maps.google.com/?*`</li><li>`http://maps.google.com/maps/ms?*`</li></ul><br/>Note: URL must begin with `http` and not `https.`|
|Social Networking|Google Plus |`http://plus.google.com/*`<br/><ul><li>`http://www.google.com/profiles/*`</li><li> `https://plus.google.com/*`</li><li> `http://google.com/profiles/*`</li></ul> |
| Video | YouTube | `http://*youtube.com/watch*` <br/><ul><li> `http://*.youtube.com/v/*`</li><li>`https://*youtube.com/watch*` </li><li>`https://*.youtube.com/v/*`</li><li>`http://youtu.be/*`</li><li>`http://*.youtube.com/user/*` </li><li>`http://*.youtube.com/*#*/*`</li><li>`http://m.youtube.com/watch*`</li><li>`http://m.youtube.com/index*`</li><li>`http://*.youtube.com/profile*`</li><li>`http://*.youtube.com/view_play_list*`</li><li>`http://*.youtube.com/playlist*`</li></ul>|
|Photos|Flickr|`http://www.flickr.com/photos/*` <br/><ul><li>`http://flic.kr/*`</li></ul>|
||Instagram|`http://instagr.am/p/*` <br/><ul><li>`http://instagram.com/p/*`</li></ul>|
||TwitPic|`http://twitpic.com/*` <br/><ul><li>`http://www.twitpic.com/*`</li><li>`http://twitpic.com/photos/*`</li><li>`http://www.twitpic.com/photos/*`</li></ul>|
||Facebook|`http://www.facebook.com/photo.php*` <br/><ul><li> `https://www.facebook.com/photo.php*`</li></ul>|
||`Ow.ly` (Hootsuite’s Content Uploading Service)|`http://ow.ly/i/*`|
|Polls|GoPollGo|`http://gopollgo.com/*`<br/><ul><li> `http://www.gopollgo.com/*`</li></ul>|
||Droplr|`http://d.pr/i/*`</li></ul>|
|Audio|SoundCloud|`http://soundcloud.com/*` <br/><ul><li>`http://soundcloud.com/*/*` </li><li>`http://soundcloud.com/*/sets/*` </li><li>`http://soundcloud.com/groups/*` </li><li>`http://snd.sc/*`</li></ul>|
||Spotify|`http://open.spotify.com/*`|
|Blogs|Tumblr|`http://tumblr.com/*` `http://*.tumblr.com/post/*`</li></ul>|

Apps that use this feature:

* [Carousel](../../c-about-apps/c-carousel-app/c-carousel-app.md#c_carousel_app)
* [Chat](../../c-about-apps/c-chat-app/c-chat-app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Feature Card](../../c-about-apps/c-feature-card-app/c-feature-card-app.md#c_feature_card_app)
* [Map](../../c-about-apps/c-map-app/c-map-app.md#c_map_app)
* [Media Wall](../../c-about-apps/c-media-wall-app/c-media-wall-app.md#c_media_wall_app)
* [Mosaic](../../c-about-apps/c-mosaic-app/c-mosaic-app.md#c_mosaic_app)
* [Polls](../../c-about-apps/c-polls-app/c-polls-app.md#c_polls_app)
* [Reviews](../../c-about-apps/c-reviews-app/c-reviews-app.md#c_reviews_app)
* [Sidenotes](../../c-about-apps/c-sidenotes-app/c-sidenotes-app.md#c_sidenotes_app)
* [Storify 2](../../c-about-apps/c-storify2/c-storify2.md#c_storify2)
* [Trending](../../c-about-apps/c-trending-app/c-trending-app.md#c_trending_app)
* [Upload Button](../../c-about-apps/c-upload-button-app/c-upload-button-app.md#c_upload_button_app)

