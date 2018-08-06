---
description: These options apply for any stream rules from all social networks or posting methods.
seo-description: These options apply for any stream rules from all social networks or posting methods.
seo-title: Stream Rule Options for All Stream Rules
solution: Experience Manager
title: Stream Rule Options for All Stream Rules
uuid: f9faa85b-9c61-4a62-b914-fc0b63dcfc8f
index: y
internal: n
snippet: y
translate: y
---

# Stream Rule Options for All Stream Rules

Search features for text and keyword fields:
* When you enter keywords, Livefyre automatically uses the Boolean operator **OR**when for individual words. For example, to search for posts with either the word *cake* or *recipe*, enter *cake*, then enter *recipe* in the ** `keyword` ** field.
* You can search for exact phrases by surrounding the exact phrase text in quotes. For example, to search for the exact phrase *cake recipe*, enter *"cake recipe"* in the ** `keyword` ** field.
* You can combine the Boolean and exact phrase searches in one stream rule. For example, you can search for *cake*, *recipe*, and *"cake recipe"* by entering each phrase one at a time.

** `Additional Filters` **:

* ** `Media` **. Select one of the following:
    * ** `All Content.` ** Allow any content.
    * ** `Media Required.` ** Allow only content with images and videos. (For Instagram and Facebook content, you can specify ** `Photos` ** or ** `Videos` ** only).

* ** `Language` **. Choose the language to search in. English is the default language.
* ** `Smart Tags` **. Choose the tags to use to identify content. Livefyre uses image recognition technology to identify photos with specific smart tags to make this search more precise. Use the ** `ANY` ** modifier to filter content into the stream using any tag or the ** `ALL` ** modifier to filter content into the stream that uses all tags. Use the ** `Image contains none of these smart tags` ** field to enter tags for photos containing content you do not want in the stream. This filter option only works for content with images. This option does not work for video or text content.
* ** `Products` **. Add product tags to match the stream rule with products from your product catalog.
* ** `Premoderate` **. Select one of the following:
    * ** `On` **. Premoderate all incoming rule content. You can view premoderated content from the Streams section of ModQ. ** `On` ** overrides the settings in App Settings.
    * ** `Off` **. Do not premoderate any incoming rule content. ** `Off` ** overrides the settings in App Settings.
    * ** `Inherited (Off)` **. Use the premoderate settings from the site (under ** `Site Settings` **).

* ** `SAFE Rules` **. Select one of the following:
    * ** `Apply SAFE Rules` **. Apply all SAFE Rules to this stream.
    * ** `Apply SAFE Rules for:` ** Select one or more of the options to apply SAFE Rules for this stream rule.
    * ** `Disable SAFE Rules` **. Do not apply any SAFE Rules to this stream.

For Stream rule options specific to a social network or content type, see the following documentation for the respective social network or content type:

* [Facebook](c_facebook_rules.md#c_facebook_rules)
* [Facebook Pages](c_facebook_page_rules.md#c_facebook_page_rules)
* [Email](c_email_rules.md#c_email_rules)
* [Instagram](c_instagram_rules.md#c_instagram_rules)
* [Tumblr](c_tumblr_rules.md#c_tumblr_rules)
* [Twitter](c_twitter_rules.md#c_twitter_rules)
* [YouTube](c_youtube_rules.md#c_youtube_rules)
* [RSS](c_rss_rules_streams.md#c_rss_rules_streams)
