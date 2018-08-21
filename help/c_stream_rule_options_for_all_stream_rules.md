---
description: These options apply for any stream rules from all social networks or posting methods.
seo-description: These options apply for any stream rules from all social networks or posting methods.
seo-title: Stream Rule Options for All Stream Rules
solution: Experience Manager
title: Stream Rule Options for All Stream Rules
uuid: b49dcc9f-0075-4bdf-b895-112e4957309f
index: y
internal: n
snippet: y
translate: y
---

# Stream Rule Options for All Stream Rules

Search features for text and keyword fields:
* When you enter keywords, Livefyre automatically uses the Boolean operator **OR**when for individual words. For example, to search for posts with either the word *cake* or *recipe*, enter *cake*, then enter *recipe* in the **[!UICONTROL  keyword]** field.
* You can search for exact phrases by surrounding the exact phrase text in quotes. For example, to search for the exact phrase *cake recipe*, enter *"cake recipe"* in the **[!UICONTROL  keyword]** field.
* You can combine the Boolean and exact phrase searches in one stream rule. For example, you can search for *cake*, *recipe*, and *"cake recipe"* by entering each phrase one at a time.


**[!UICONTROL  Additional Filters]**:

* **[!UICONTROL  Media]**. Select one of the following:
    * **[!UICONTROL  All Content.]** Allow any content.
    * **[!UICONTROL  Media Required.]** Allow only content with images and videos. (For Instagram and Facebook content, you can specify **[!UICONTROL  Photos]** or **[!UICONTROL  Videos]** only).

* **[!UICONTROL  Language]**. Choose the language to search in. English is the default language.
* **[!UICONTROL  Smart Tags]**. Choose the tags to use to identify content. Livefyre uses image recognition technology to identify photos with specific smart tags to make this search more precise. Use the **[!UICONTROL  ANY]** modifier to filter content into the stream using any tag or the **[!UICONTROL  ALL]** modifier to filter content into the stream that uses all tags. Use the **[!UICONTROL  Image contains none of these smart tags]** field to enter tags for photos containing content you do not want in the stream. This filter option only works for content with images. This option does not work for video or text content.
* **[!UICONTROL  Products]**. Add product tags to match the stream rule with products from your product catalog.
* **[!UICONTROL  Premoderate]**. Select one of the following:
    * **[!UICONTROL  On]**. Premoderate all incoming rule content. You can view premoderated content from the Streams section of ModQ. **[!UICONTROL  On]** overrides the settings in App Settings.
    * **[!UICONTROL  Off]**. Do not premoderate any incoming rule content. **[!UICONTROL  Off]** overrides the settings in App Settings.
    * **[!UICONTROL  Inherited (Off)]**. Use the premoderate settings from the site (under **[!UICONTROL  Site Settings]**).

* **[!UICONTROL  SAFE Rules]**. Select one of the following:
    * **[!UICONTROL  Apply SAFE Rules]**. Apply all SAFE Rules to this stream.
    * **[!UICONTROL  Apply SAFE Rules for:]** Select one or more of the options to apply SAFE Rules for this stream rule.
    * **[!UICONTROL  Disable SAFE Rules]**. Do not apply any SAFE Rules to this stream.

For Stream rule options specific to a social network or content type, see the following documentation for the respective social network or content type:

* [ Facebook](c_facebook_rules.md#c_facebook_rules)
* [ Facebook Pages](c_facebook_page_rules.md#c_facebook_page_rules)
* [ Email](c_email_rules.md#c_email_rules)
* [ Instagram](c_instagram_rules.md#c_instagram_rules)
* [ Tumblr](c_tumblr_rules.md#c_tumblr_rules)
* [ Twitter](c_twitter_rules.md#c_twitter_rules)
* [ YouTube](c_youtube_rules.md#c_youtube_rules)
* [ RSS](c_rss_rules_streams.md#c_rss_rules_streams)
