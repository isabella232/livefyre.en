---
description: Release Notes for the March 30, 2017 release.
seo-description: Release Notes for the March 30, 2017 release.
seo-title: March 30, 2017
title: March 30, 2017
---

# March 30, 2017

<table id="table_q3m_qxq_kz"> 
 <title>Production Release</title> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry">Issue Type</th> 
    <th class="entry">Component</th> 
    <th class="entry">Release Note</th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td>Bug</td> 
    <td>Social Search</td> 
    <td>Fixed a bug that prevented saved Youtube assets in Social Search from publishing.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Social Sync</td> 
    <td>Deprecated Twitter Social Sync.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Storify 2</td> 
    <td>Added an enhancement to display the message "No results found" on Facebook Topic search when no results are found.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Streams</td> 
    <td>Added Summary Rules for SAFE Rules to the bottom of a Twitter Stream page.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Streams</td> 
    <td>Added an enhancement to visibly disable the "verified user" checkbox on Twitter Stream Rules when excluded authors are provided.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Streams</td> 
    <td>Fixed a bug to allow the usage of ANDing keywords and a Location filter in a Twitter rule.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Studio</td> 
    <td>Fixed a bug that was preventing the "Feature Tag" to save correctly when applied.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

<table id="table_r3m_qxq_kz"> 
 <title>UAT Release</title> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry">Issue Type</th> 
    <th class="entry">Component</th> 
    <th class="entry">Release Note</th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td>Bug</td> 
    <td>App Content</td> 
    <td>Changed the behavior of "More Info" such that if there are multiple Anonymous flag events on a given piece of content, the earliest event is always shown.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Library</td> 
    <td>Fixed a bug that caused Library searches with hashtags to intermittently fail.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Maps</td> 
    <td>Fixed a bug in Maps to support a large number of content in clusters on iOS devices.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Mosaic</td> 
    <td>Added the ability to configure Mosaic apps to click anywhere on a content card to open the modal by animation type `none` in designer and `cardAnimation: 'off'`if instantiated through the SDK.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Mosaic</td> 
    <td>Fixed a bug to allow users to successfully make changes to Mosaic apps in Designer.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Rights Request</td> 
    <td>Added a new rights request status called "Request Failed" to highlight when rights request messages fail to send.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Settings</td> 
    <td>Added the ability for customers to create Spam Moderation Rules in Settings.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Social Search</td> 
    <td>Fixed a bug that prevented VK.com posts from displaying via URL Social Searches.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Social Search</td> 
    <td>When searching for Instagram content from Studio, if the search is due to an expired Instagram API Token, the error message will now indicate as such.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Streams</td> 
    <td>Fixed a bug that caused an "App is not accepting new content" banner to falsely display on top of Stream Rule pages.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Streams</td> 
    <td>Modified the default of newly created stream rules to Apply SAFE Rules when applicable.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Streams (formerly, Curate Rules)</td> 
    <td>Removed the "Vines" only option from Twitter Stream/Curate rules, as Vines are now displayed as Twitter videos.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Studio Shell</td> 
    <td>Fixed a bug so that Livefyre Studio will load if http:// was explicitly prepended to the url.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

