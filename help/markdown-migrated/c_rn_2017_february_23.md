---
description: Release Notes for the February 23, 2017 release.
seo-description: Release Notes for the February 23, 2017 release.
seo-title: February 23, 2017
title: February 23, 2017
---

# February 23, 2017

<table id="table_rcr_crx_1z"> 
 <title>Production Release</title> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead>
   <tr> 
    <th class="entry"><b>Issue Type</b></th> 
    <th class="entry"><b>Component</b></th> 
    <th class="entry"><b>Release Note</b></th> 
   </tr>
  </thead> 
  <tbody> 
   <tr> 
    <td>Enhancement</td> 
    <td>Android SDK</td> 
    <td>Re-organized the Android SDK to ensure that example and reference implementation directories are more clearly identifiable by their location.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Android SDK</td> 
    <td>Android SDK modified to now support a minimum SDK version of 14 (down from 16).</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Conversation Apps</td> 
    <td>Enhanced Conversation Apps to always link out to user profiles, even without a full auth integration.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Mosaic</td> 
    <td>Fixed a bug that now serves all Twitter images via HTTPS.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Search and Streams</td> 
    <td>Added the ability to search by Instagram Places (check-in’s) in Library Instagram Search and Instagram Stream Rules.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Settings</td> 
    <td>Fixed a bug that prevented Twitter Social Accounts from saving.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Social Search</td> 
    <td>Fixed a bug that prevented the “Conceal explicit images” option from functioning properly.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Storify 2</td> 
    <td>Enhanced Storify 2 to support permalinks opening a modal (previously the app would scroll to the post location on the page). In Storify 2’s Designer, we have added a configuration to toggle between Scroll and Modal permalink behavior. Modal permalink behavior will be default behavior.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Storify 2</td> 
    <td>Enhanced the Storify 2 Google AMP integration to produce a smaller CSS file.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Streams</td> 
    <td>Fixed a bug with Facebook rules that was causing content to be pulled in with incomplete metadata.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Streams</td> 
    <td>Enhanced content (images and videos) from Email Stream Rules to be available via HTTPS.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Streams</td> 
    <td>Added a label for the Mile Radius Value in maps in Twitter Stream Rules.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Streams</td> 
    <td>Fixed a bug with Facebook and Facebook Page Steam Rules to pull in posts with multiple media attachments appropriately.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Streams</td> 
    <td>Added a new feature to allow users to choose to apply or disable SAFE rules per stream rule.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Studio</td> 
    <td>Fixed a bug that was causing content to not publish or save correctly if it already existed.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Studio</td> 
    <td>Fixed a bug that caused multiple &amp;’s from getting appended to the url when using filters in Studio.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Studio</td> 
    <td>Fixed a bug that prevented certain checkboxes in Studio filters from allowing to be unchecked.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

<table id="table_scr_crx_1z"> 
 <title>UAT Release</title> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead>
   <tr> 
    <th class="entry"><b>Issue Type</b></th> 
    <th class="entry"><b>Component</b></th> 
    <th class="entry"><b>Release Note</b></th> 
   </tr>
  </thead> 
  <tbody> 
   <tr> 
    <td>Bug</td> 
    <td>Apps</td> 
    <td>Fixed a bug to show content in media modals with the correct aspect ratios.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Media Wall</td> 
    <td>Fixed a bug that was caused Media Walls to not render if specific foreign characters were included.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Search</td> 
    <td>Fixed a bug that was causing pages to load incorrectly when paging through search results with “Conceal explicit images” enabled.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Studio</td> 
    <td>Increased session time before expiring Studio User login sessions . Once a Studio session expires the user will be redirected to log in again.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Studio</td> 
    <td>Fixed a bug that was sometimes preventing users from saving Instagram credentials.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Studio</td> 
    <td>Fixed a bug that was preventing the “Feature Tag” to save correctly when applied.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

