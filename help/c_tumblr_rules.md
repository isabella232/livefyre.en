---
description: You can create Stream rules that pull content from Tumblr.
seo-description: You can create Stream rules that pull content from Tumblr.
seo-title: Tumblr Rules
solution: Experience Manager
title: Tumblr Rules
uuid: cfd6db47-b081-4428-a0c2-c61647a86de2
index: y
internal: n
snippet: y
translate: y
---

# Tumblr Rules

You can create Stream rules that pull content from Tumblr.

Create Tumblr rules based on a Tumblr blog and filtered by tag. Tumblr streams update every 5 minutes, looking for content that does not already exist in Livefyre from the first 20 items in the feed. Livefyre ignores everything past the first 20 items in the feed.

To create Tumblr Rules to pull content from Tumblr into your App or Folder, you can filter by:

* **[!UICONTROL Blog]**

    * Enter the **[!UICONTROL Blog Name]** for the Tumblr blog. Enter the URL (*staff.tumblr.com*) or the name of the blog (*staff*).
    
    * Include up to one **[!UICONTROL Tag]** to filter results by posts including a given tag.

* **[!UICONTROL Include recent items.]** If this is set to:

    * **[!UICONTROL Enabled]**, Livefyre adds the first 20 content items in your feed to the stream, regardless of the publication date.
    * **[!UICONTROL Disabled]**, Livefyre adds the first 20 content items in your feed to the stream with a publication date that is the same as the stream rule creation date or later.

For additional Stream rule options for all Stream rules, see [Stream Rule Options for All Stream Rules](c_stream_rule_options_for_all_stream_rules.md#c_stream_rule_options_for_all_stream_rules). 
