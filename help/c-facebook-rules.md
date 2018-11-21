---
description: You can create Stream rules that pull public content from Facebook.
seo-description: You can create Stream rules that pull public content from Facebook.
seo-title: Facebook Rules
solution: Experience Manager
title: Facebook Rules
uuid: 262b5530-cc80-4793-b8f0-37a7f25bf760
index: y
internal: n
snippet: y
---

# Facebook Rules{#facebook-rules}

You can create Stream rules that pull public content from Facebook.

You can use Facebook Rules to stream publicly posted content from Facebook.

You can create Facebook Rules based on hashtags, keywords, or author.

>[!NOTE]
>
>All Facebook rules require at least one Keyword, Hashtag, or Author filter. Adding a Keyword and a Hashtag for your rule will return content which includes both entries.

To create Facebook Rules to pull public content from Facebook feeds into your App or Folder, you can filter by:

* **[!UICONTROL Contains]**

    * Enter **[!UICONTROL Keywords]** and/or **[!UICONTROL Hashtags]**to be included in, or excluded from your Facebook stream. Specifying values for both the **[!UICONTROL Any]** and **[!UICONTROL Does not contain]** fields will return posts which contain the first, and do not contain the second.
    
    * **[!UICONTROL For example:]** Entering **[!UICONTROL Contains]** keywords Giants, Posey, and **[!UICONTROL Does not contain]** keyword Dodger, will return all posts which include the word Giants or Posey, and do not include the word Dodger.

* **[!UICONTROL Author]**

    * Enter **[!UICONTROL Authors]** to pull into the stream, or exclude from the stream.     
    
      >[!NOTE]
      >
      >You may either include or exclude authors; you cannot combine these two fields into a single Facebook Rule.

* **[!UICONTROL Additional Filters]**

    * Select whether you would like to include **[!UICONTROL All Content]**, **[!UICONTROL Videos Only]**, or **[!UICONTROL Photos Only]** in your stream.

For additional Stream rule options for all Stream rules, see [Stream Rule Options for All Stream Rules](c-stream-rule-options-for-all-stream-rules.md#c_stream_rule_options_for_all_stream_rules). 
