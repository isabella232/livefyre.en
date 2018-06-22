---
description: You can create Stream rules that pull content from Tumblr.
seo-description: You can create Stream rules that pull content from Tumblr.
seo-title: Tumblr Rules
solution: Experience Manager
title: Tumblr Rules
---

# Tumblr Rules

Create Tumblr rules based on a Tumblr blog and filtered by tag. Tumblr streams update every 5 minutes, looking for content that does not already exist in Livefyre from the first 20 items in the feed. Livefyre ignores everything past the first 20 items in the feed.

To create Tumblr Rules to pull content from Tumblr into your App or Folder, you can filter by:

* `uicontrol Blog`
    * Enter the `uicontrol Blog Name` for the Tumblr blog. Enter the URL (*staff.tumblr.com*) or the name of the blog (*staff*).
    * Include up to one `uicontrol Tag` to filter results by posts including a given tag.
  
* `uicontrol Include recent items.` If this is set to:
    * `uicontrol Enabled`, Livefyre adds the first 20 content items in your feed to the stream, regardless of the publication date.
    * `uicontrol Disabled`, Livefyre adds the first 20 content items in your feed to the stream with a publication date that is the same as the stream rule creation date or later.
  
For additional Stream rule options for all Stream rules, see [Stream Rule Options for All Stream Rules](c_stream_rule_options_for_all_stream_rules.md#c_stream_rule_options_for_all_stream_rules).

