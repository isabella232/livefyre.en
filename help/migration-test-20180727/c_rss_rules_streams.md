---
description: You can create Stream rules that pull content from RSS feeds.
seo-description: You can create Stream rules that pull content from RSS feeds.
seo-title: RSS Rules
solution: Experience Manager
title: RSS Rules
uuid: 1b20c97f-7d5b-4edc-9a6f-0b08e4125418
index: y
internal: n
snippet: y
translate: y
---

# RSS Rules

RSS streams update every 5 minutes, looking for content that does not already exist in Livefyre from the first 50 items in the feed. Livefyre ignores everything past the first 50 items in the feed.
To create RSS Rules to pull content from RSS feeds into your App or Folder, you can filter by:

* ** `URL` ** of the RSS Feed.
* ** `Include recent items.` ** If this is set to:
    * ** `Enabled` **, Livefyre adds the first 50 content items in your feed to the stream, regardless of the publication date.
    * ** `Disabled` **, Livefyre adds the first 50 content items in your feed to the stream with a publication date that is the same as the stream rule creation date or later.

* ** `Extract post information from item link (when disabled, post information is extracted from XML).` ** Pull information from the item link or from the XML.
**RSS Rules**
Livefyre parses RSS feeds based on the following RSS specs:

* [RSS 2.0](https://en.wikipedia.org/wiki/RSS)
* [Media RSS](https://en.wikipedia.org/wiki/Media_RSS)
* [Atom feed](https://validator.w3.org/feed/docs/atom.html)
Livefyre does not read feeds that do not adhere to these specs, and their content will not be pulled into your stream. Use the WC3 Feed Validation Service to check the syntax of your RSS feed, and ensure that it is valid.
For additional Stream rule options for all Stream rules, see [Stream Rule Options for All Stream Rules](c_stream_rule_options_for_all_stream_rules.md#c_stream_rule_options_for_all_stream_rules). 
