---
description: You can create Stream rules that pull content from Facebook Pages.
seo-description: You can create Stream rules that pull content from Facebook Pages.
seo-title: Facebook Page Rules
solution: Experience Manager
title: Facebook Page Rules
---

# Facebook Page Rules

You can use Facebook Page Rules to stream publicly posted content from Facebook Pages. The content will be pulled into the App or Folder at the same frequency as SocialSync, which changes based on Facebook Page and post traffic patterns. Links within Facebook Pages are also supported, and will be displayed in the stream.

To create Facebook Page Rules to pull content from Facebook pages into your App or Folder, you can filter by:

* `uicontrol Facebook Page`
    * Enter the `uicontrol Name` for the Page. Enter only the trailing text for the URL. **For example: **To add content from https://facebook.com/KellysSuperFunFanPage, type *KellysSuperFunFanPage* in the `uicontrol Name` field.
    * Switch `uicontrol Include Facebook Comments for each post` on if you wish to include user comments to Page posts.
    * Switch `uicontrol Only Show Author Posts` on if you wish to exclude posts from other users.
  
For additional Stream rule options for all Stream rules, see [Stream Rule Options for All Stream Rules](c_stream_rule_options_for_all_stream_rules.md#c_stream_rule_options_for_all_stream_rules).

>[!NOTE]
>
>Livefyre is restricted to content received from Facebook, and is therefore unable to guarantee that every post on a Facebook Page will be included in your stream.
>[!NOTE]
>
>If Facebook SocialSync and a Facebook Page Rule are both enabled for a specific Facebook Page, and user comments are enabled for the Facebook Page Rule, the Stream Rule will override SocialSync. Content will be streamed into the App based on the Facebook Page Curate Rule only, and not using SocialSync.
The types of content supported by Facebook Page Curate include:

  *
  Page Owner or Admin
  
    * Status
    * Photos
    * Videos as links
  
  *
  Standard Facebook User
  
    * Status
    * Photos
    * Videos as links
  
  *
  Third Parties
  
    * Status
  
