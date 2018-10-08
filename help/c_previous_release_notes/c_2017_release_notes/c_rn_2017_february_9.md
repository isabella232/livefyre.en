---
description: Release Notes for the February 9, 2017 release.
seo-description: Release Notes for the February 9, 2017 release.
seo-title: February 9, 2017
title: February 9, 2017
uuid: 4b8ac7e5-d20a-4d7a-abe8-11e463c2266b
index: y
internal: n
snippet: y
translate: y
---

# February 9, 2017

Release Notes for the February 9, 2017 release.

## SocialSync for Twitter {#section_nv4_yry_wy}

SocialSync for Twitter has been a part of our core functionality for several years. However, as our product has developed and grown over time, SocialSync for Twitter has become a lower-value feature that is currently used by a very small portion of our customer base. To improve the overall experience of Livefyre for our customers and focus development resources in areas of greatest value, we will be discontinuing the SocialSync for Twitter feature on February 24. SocialSync for Facebook will be unaffected by this update. If you have any questions or concerns about this update, please reach out to your Livefyre CSM.

## Production Release {#section_r24_1m2_wy}

<table id="table_t4j_gxt_wy"> 
 <thead> 
  <tr> 
   <th class="entry"><b>Issue Type</b></th> 
   <th class="entry"><b>Component</b></th> 
   <th class="entry"><b>Release Note</b></th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> Bug</td> 
   <td> Media Wall</td> 
   <td> <p>Fixed a bug that allows Facebook videos to play appropriately.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> ModQ</td> 
   <td> <p>Fixed a bug that prevented Email Subjects from not displaying in Email Stream Content.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Mosaic</td> 
   <td> <p>Added additional accessibility support to Mosaic to allow users to shift tab between content cards.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Reviews</td> 
   <td> <p>Fixed a bug that was preventing rating edits to appear appropriately.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Social Search</td> 
   <td> <p>Fixed a bug that caused the Show More button to be cut off on Twitter List Search results.</p> </td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Storify 2</td> 
   <td> <p>Enhanced Storify 2 to support Copywrite Free content search. Copywrite Free searches across Flickr, Noun Project, Kuler, Pixabay and Unsplash for copywrite free images.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Streams</td> 
   <td> <p>Fixed a bug that prevented Tumblr stream rules from saving.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Streams</td> 
   <td> <p>Fixed a bug that produced incorrect Generator Ids in the Collection JSON for RSS Feeds.</p> </td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Streams</td> 
   <td> <p>Made an adjustment to the setting of "Verified accounts only" option to be disabled by default.</p> </td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Streams</td> 
   <td> <p>Added a new feature to allow categories of content (via a Stream Rule) to be whitelisted and bypass moderation.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Streams</td> 
   <td> <p>Fixed a bug that caused "Premoderate" and "Media Premoderate" settings to carry over to a newly created Stream rule.</p> </td> 
  </tr> 
 </tbody> 
</table>

## UAT Release {#section_dyx_yl2_wy}

<table id="table_u4j_gxt_wy"> 
 <thead> 
  <tr> 
   <th class="entry"><b>Issue Type</b></th> 
   <th class="entry"><b>Component</b></th> 
   <th class="entry"><b>Release Note</b></th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> Bug</td> 
   <td> Conversation Apps</td> 
   <td> <p>Enhanced Conversation Apps to always link out to user profiles, even without a full auth integration.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Mosaic</td> 
   <td> <p>Fixed a bug that now serves all Twitter images via HTTPS.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Social Search</td> 
   <td> <p>Fixed a bug that caused the green "saved" checkmark to not appear when saving assets in Social Search and viewing assets in Library.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Social Search</td> 
   <td> <p>Fixed a bug that prevented the "Conceal explicit images" option from functioning properly.</p> </td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Storify 2</td> 
   <td> <p>Enhanced Storify 2 to support permalinks opening a modal (previously the app would scroll to the post location on the page). In Storify 2's Designer, we have added a configuration to toggle between Scroll and Modal permalink behavior. Modal permalink behavior will be default behavior.</p> </td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Storify 2</td> 
   <td> <p>Enhanced the Storify 2 Google AMP integration to produce a smaller CSS file.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Streams</td> 
   <td> <p>Enhanced content (images and videos) from Email Stream Rules to be available via HTTPS.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Streams</td> 
   <td> <p>Added a label for the Mile Radius Value in maps in Twitter Stream Rules.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Streams</td> 
   <td> <p>Fixed a bug with Facebook and Facebook Page Steam Rules to pull in posts with multiple media attachments appropriately.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Studio</td> 
   <td> <p>Fixed a bug that caused multiple &amp;'s from getting appended to the URL when using filters in Studio.</p> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Studio</td> 
   <td> <p>Fixed a bug that prevented certain checkboxes in Studio filters from allowing to be unchecked.</p> </td> 
  </tr> 
 </tbody> 
</table>

