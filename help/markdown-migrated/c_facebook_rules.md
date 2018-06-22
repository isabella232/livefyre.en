---
description: You can create Stream rules that pull public content from Facebook.
seo-description: You can create Stream rules that pull public content from Facebook.
seo-title: Facebook Rules
solution: Experience Manager
title: Facebook Rules
---

# Facebook Rules

You can use Facebook Rules to stream publicly posted content from Facebook.

You can create Facebook Rules based on hashtags, keywords, or author.

>[!NOTE]
>
>All Facebook rules require at least one Keyword, Hashtag, or Author filter. Adding a Keyword and a Hashtag for your rule will return content which includes both entries.
To create Facebook Rules to pull public content from Facebook feeds into your App or Folder, you can filter by:

* `uicontrol  Contains`
    * Enter `uicontrol  Keywords` and/or `uicontrol  Hashtags`to be included in, or excluded from your Facebook stream. Specifying values for both the `uicontrol  Any` and `uicontrol  Does not contain` fields will return posts which contain the first, and do not contain the second.
    * `uicontrol  For example:` Entering `uicontrol  Contains` keywords Giants, Posey, and `uicontrol  Does not contain` keyword Dodger, will return all posts which include the word Giants or Posey, and do not include the word Dodger.
  
* `uicontrol  Author`
    * Enter `uicontrol  Authors` to pull into the stream, or exclude from the stream.
      >[!NOTE]
      >
      >You may either include or exclude authors; you cannot combine these two fields into a single Facebook Rule.
      
  
* `uicontrol  Additional Filters`
    * Select whether you would like to include `uicontrol  All Content`, `uicontrol  Videos Only`, or `uicontrol  Photos Only` in your stream.
  
For additional Stream rule options for all Stream rules, see [ Stream Rule Options for All Stream Rules ](c_stream_rule_options_for_all_stream_rules.md#c_stream_rule_options_for_all_stream_rules).

