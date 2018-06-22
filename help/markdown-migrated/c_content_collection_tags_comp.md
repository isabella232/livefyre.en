---
description: Use your bit.ly URL shortener to customize content permalinks.
seo-description: Use your bit.ly URL shortener to customize content permalinks.
seo-title: Permalinks
solution: Experience Manager
title: Permalinks
---

# Permalinks


>## Collection and Content Tags {#c_content_collection_tags}
>Add keyword tags to collections and content, to categorize and organize content for easy retrieval.

On this page:

* [](#c_content_collection_tags/section_uhd_frk_wy)
* [](#t_filter_search_by_tag)
* [](#t_filter_search_by_content_tag)
* [](#c_embedly_integration)
* [](#c_featured_content)
* [](#t_feature_content)
* [](#t_select_content_to_feature)
* [](#select_content_to_feature_from_studio)
* [](#t_enable_featuring_content_in_studio)
* [](#c_permalinks)
<!-- c_content_collection_tags.dita -->
Assigning tags allows you to filter searches by a specific tag, and to pull data for the Heat Index API.

Tags may be added through the `uicontrol Content` and `uicontrol Collections` panels in Studio, or directly to the Collection Metadata (using the collectionMeta object) when initializing or updating the Collection with Livefyre.

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
## Using Collection Tags with the Heat Index API {#section_uhd_frk_wy}

The Heat Index API accepts a Tag parameter, allowing you to retrieve relative hotness for any Collection with that Tag, across a site or entire network.

For implementation details, refer to the Heat Index API technical documentation.

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

>## Filter Search by Collection or Content tag {#t_filter_search_by_tag}
>Filter content searches in Studio by Collection tag.

<!-- c_content_collection_tags.dita -->
>1. Select `uicontrol Tag` in the search dropdown of the `uicontrol Collections` panel.
>   
>1. Entering the tag for your search or click on the `uicontrol Tag` listed under a Collection.
>       
>   
>   

>## Filter Search by Content Tag {#t_filter_search_by_content_tag}
>Filter content searches in Studio by Collection tag.

<!-- t_filter_search_by_content.dita -->
>1. Select `uicontrol Filter by: Contains` from the `uicontrol Content` panel.
>   
>1. Enter the tag.
>   
>   

>## Embedly Integration {#c_embedly_integration}
>Use embed.ly to display multiple media formats, directly in the App.

<!-- c_embedly_integration.dita -->
To better enable embedded media content from a variety of sources, including Google Maps, YouTube, Flickr, Facebook, Instagram, Spotify, and Tumblr, Livefyre Apps use Embedly as a third-party provider for URL expansion. If a user or moderator includes a supported link in a post, the media included in the link will expand when posted to the Collection.

This provides Livefyre Apps with access to the more than 250 different embedded media options that Embedly supports.

>[!NOTE]
>
>Livefyre expands only a subset of Embedly’s full provider list. Embedded images will expand on HTTPS pages only if the provider is Twitter, YouTube, Imgur, Vine, Wikipedia, or SoundCloud. Please contact your Technical Account Manager for any further questions about link expansion or sources.
This page lists examples of some popular embedded media types, and their acceptable URL patterns. Embed.ly is continually adding new sources. For a complete list of providers, please go to https://embed.ly/embed/features/providers.

>[!NOTE]
>
>The Embedly formatting requires a full permalink. Shortened links will not work.
Only publicly viewable content is embeddable. If you attempt to embed a piece of content that is not public, the link to the content will appear in the blog post, and a placeholder icon will accompany it. When clicked, the link will take the reader to an error message from the service where the content is hosted, such as a Facebook message for a friends-only photo. Please contact your Account Manager if you notice that media is not expanded as expected.

<table id="table_lth_m4x_vy"> 
 <title>Sample Embedly URLs</title> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <tbody> 
   <tr> 
    <td> <b>Maps</b> </td> 
    <td> <b>Google Maps</b> </td> 
    <td> 
     <ul id="ul_mth_m4x_vy"> 
      <li>https://maps.google.com/maps?*</li> 
      <li>https://maps.google.com/?*</li> 
      <li>https://maps.google.com/maps/ms?*</li> 
      <li> <b>Note: </b>URL must begin with “http” and not “https.”</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td> <b>Social Networking</b> </td> 
    <td> <b>Google Plus</b> </td> 
    <td> 
     <ul id="ul_nth_m4x_vy"> 
      <li>https://plus.google.com/*</li> 
      <li>https://www.google.com/profiles/*</li> 
      <li>https://plus.google.com/*</li> 
      <li>https://google.com/profiles/*</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> <b>YouTube</b> </td> 
    <td> 
     <ul id="ul_oth_m4x_vy"> 
      <li>https://*youtube.com/watch*</li> 
      <li>https://*.youtube.com/v/*</li> 
      <li>https://*youtube.com/watch*</li> 
      <li>https://*.youtube.com/v/*</li> 
      <li>https://youtu.be/*</li> 
      <li>https://*.youtube.com/user/*</li> 
      <li>https://*.youtube.com/*#*/*</li> 
      <li>https://m.youtube.com/watch*</li> 
      <li>https://m.youtube.com/index*</li> 
      <li>https://*.youtube.com/profile*</li> 
      <li>https://*.youtube.com/view_play_list*</li> 
      <li>https://*.youtube.com/playlist*</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td> <b>Photos</b> </td> 
    <td> <b>Flickr</b> </td> 
    <td> 
     <ul id="ul_pth_m4x_vy"> 
      <li>https://www.flickr.com/photos/*</li> 
      <li>https://flic.kr/*</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> <b>Instagram</b> </td> 
    <td> 
     <ul id="ul_qth_m4x_vy"> 
      <li>https://instagr.am/p/*</li> 
      <li>https://instagram.com/p/*</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> <b>TwitPic</b> </td> 
    <td> 
     <ul id="ul_rth_m4x_vy"> 
      <li>https://twitpic.com/*</li> 
      <li>https://www.twitpic.com/*</li> 
      <li>https://twitpic.com/photos/*</li> 
      <li>https://www.twitpic.com/photos/*</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> <b>Facebook</b> </td> 
    <td> 
     <ul id="ul_sth_m4x_vy"> 
      <li>https://www.facebook.com/photo.php*</li> 
      <li>https://www.facebook.com/photo.php*</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> <p> <b>Ow.ly </b> </p> <p>(Hootsuite’s Content Uploading Service)</p> </td> 
    <td> 
     <ul id="ul_tth_m4x_vy"> 
      <li>https://ow.ly/i/*</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td> <b>Polls</b> </td> 
    <td> <b>GoPollGo</b> </td> 
    <td> 
     <ul id="ul_uth_m4x_vy"> 
      <li>https://gopollgo.com/*</li> 
      <li>https://www.gopollgo.com/*</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> <b>Droplr</b> </td> 
    <td> 
     <ul id="ul_vth_m4x_vy"> 
      <li>https://d.pr/i/*</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td> <b>Audio</b> </td> 
    <td> <b>SoundCloud</b> </td> 
    <td> 
     <ul id="ul_wth_m4x_vy"> 
      <li>https://soundcloud.com/*</li> 
      <li>https://soundcloud.com/*/*</li> 
      <li>https://soundcloud.com/*/sets/*</li> 
      <li>https://soundcloud.com/groups/*</li> 
      <li>https://snd.sc/*</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> <b>Spotify</b> </td> 
    <td> 
     <ul id="ul_xth_m4x_vy"> 
      <li>https://open.spotify.com/*</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td> <b>Blogs</b> </td> 
    <td> <b>Tumblr</b> </td> 
    <td> 
     <ul id="ul_yth_m4x_vy"> 
      <li>https://tumblr.com/*</li> 
      <li>https://*.tumblr.com/post/*</li> 
     </ul> </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

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

>## Featured Content {#c_featured_content}
>Highlight important content to your users by using CSS to custom style Featured content.

<!-- c_featured_content.dita -->
Any piece of content in a Collection can be tagged as “featured” by your network site owners or moderators, in order to highlight important content and encourage high quality replies from other users. Once a piece of content has been featured, a `uicontrol Featured` tag will be displayed on the content in the app, so that users can easily identify content that owners and moderators have highlighted.

In Comments:

* The two most recent pieces of `uicontrol Featured` content will also be pulled above the stream.
* It may take up to seven minutes for Featured content to appear above the editor.
* A `uicontrol Featured` tag may be added to any comment within the stream, and used to style the comment, but only Livefyre-native user generated content will appear above the editor.
When content is unfeatured, the `uicontrol Featured` tag displayed will be removed in real-time.

Once a piece of content has been featured, a `uicontrol Featured` badge will be displayed on the content in the app, and you may use the fyre-featured CSS class to custom style the content.

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

>## Feature Content {#t_feature_content}
>Use custom styling to highlight featured content.

<!-- t_featured_content.dita -->
Featuring content allows you to call attention to selected user posts. Featured content may be styled differently than other content on the page, and featured Livefyre-native content appears above the editor. Once featured, content includes a Featured badge, and may be custom styled using the fyre-featured CSS class. The two most recently featured Livefyre-native content items will also be displayed above the editor in the stream.

>1. Enable the option in Studio.
>   
>1. Train your moderators to identify and select content to be featured.
>   
>1. Use CSS to style the way in which the content will be displayed in the App.
>   
>1. Use API calls to automate the process.
>* Feature
>* Unfeature
>   
>   
>1. Aggregate Featured Content.
>* Featured (Network)
>* Featured (Site)
>* Featured (Collection)
>* Featured (Head)
>   
>   
>   

>## Select Content to Feature from an App {#t_select_content_to_feature}
>Feature or unfeature content directly from an App/

<!-- t_select_content_to_feature.dita -->
>1. From within an App, hover over the content you wish to feature.
>   
>1. Click `uicontrol Feature` to feature the content or `uicontrol Unfeature` to stop featuring that piece of content.
>   
>   

>## Select Content to Feature From Studio {#select_content_to_feature_from_studio}
>You can select content to feature from Studio instead of an App.

<!-- t_select_content_to_feature_from_studio.dita -->
>1. From Studio, click the `uicontrol +` sign beside a piece of content.
>   
>1. Select the `uicontrol Featured` tag in the dropdown list.
>   
>1. Click `uicontrol Enter` to Feature the piece of content.
>       
>   
>1. To stop featuring a piece of content, click the `uicontrol x` on the `uicontrol Featured` tag displayed on the piece of content.
>   
>   

>## Enable Featuring Content in Studio {#t_enable_featuring_content_in_studio}
>To feature content, you must first enable the 
<uicontrol>
 Enable Featured Comments
</uicontrol> setting in Studio.

<!-- t_enable_featuring_content_in_studio.dita -->
>1. Go to `uicontrol Studio &gt; Settings &gt; Network Settings &gt; Default Settings`.
>   
>1. Toggle the `uicontrol Enable Featured Comments` setting to allow you to highlight recently featured comments above the editor.
>   
>   

>## Permalinks {#c_permalinks}
>Use your bit.ly URL shortener to customize content permalinks.

<!-- c_permalinks.dita -->
Permalinks allow you to link to archived comments or content within your streams. To enable this feature, Livefyre uses a default URL format: **fyre.it**. This format may be customized to match your standard bit.ly format.

## Permalink display {#section_mxd_wwg_wy}

If users click a permalink from a social network to a Livefyre content app, they will be taken to the Livefyre content stream. The content will be displayed in a breakout view of the stream, just below the editor, with full context displayed. A blue line will be shown below the avatar for the permalinked content. (This blue line will disappear after a few seconds.)

(If permalinked content is deleted, a message to that effect will be displayed in the breakout view.)

## Custom Permalinks {#section_uyn_5wg_wy}

If you wish to create custom permalinks for comments when sharing conversations, you may use your Bitly account, rather than the standard Livefyre shortened URL (fyre.it). Using your Bitly account will help remind users that they will be visiting content on your site when clicking on a permalink.

To implement this feature, go to `uicontrol Studio &gt; Settings &gt; Integration Settings &gt; Social Sharing`, and enter your Bitly API Key and username.

>[!NOTE]
>
>To avoid unnecessary URLs created on your behalf, Bitly permalinks are generated on an as-needed basis.
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
