---
description: Release Notes for the January 18, 2018 release.
seo-description: Release Notes for the January 18, 2018 release.
seo-title: January 18, 2018
solution: Experience Manager
title: January 18, 2018
---

# January 18, 2018

<table id="table_qty_nhy_4cb"> 
 <title>Production Release</title> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> <b>Issue Type</b> </th> 
    <th class="entry"> <b>Component</b> </th> 
    <th class="entry"> <b>Release Note</b> </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td>Bug</td> 
    <td>Apps</td> 
    <td>Fixed bug that prevented Avatars to be rendered correctly when a jpeg file was being used.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>ModQ</td> 
    <td>Fixed a bug for S1 customers to allow filtering by Collections in ModQ.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Streams</td> 
    <td>Fixed a bug that broke a stream rule when the language filter was set as "none."</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Streams</td> 
    <td>Fixed a bug that prevented Youtube stream rules from being saved.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Streams</td> 
    <td>Fixes a bug where users could create wrongfully formatted geo entries in stream rules and save them, which would make the stream fail. Now, users can no longer save badly formatted geo tags.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Studio</td> 
    <td>Fixed an issue that prevented some users from logging into Livefyre.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

<table id="table_cr1_42y_4cb"> 
 <title>UAT Release</title> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> <b>Issue Type</b> </th> 
    <th class="entry"> <b>Component</b> </th> 
    <th class="entry"> <b>Release Note</b> </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td>Bug</td> 
    <td>Library</td> 
    <td>Security bug fix. All authentication calls are now made using the HTTPS protocol instead of HTTP.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Smart Tags</td> 
    <td>Streamed content is now automatically smart tagged by Adobe Sensei as it is saved to a folder or published to an app.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Streams</td> 
    <td>Fixed an issue where Instagram stream rules did not recognize Japanese characters.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Streams</td> 
    <td>Customers can now use the logical operators ( ANY, ALL, NOT) to create detailed smart-tag filters in streams that curate much more accurate content. For example if I use the hashtag #himalyas I can select to show only images that include "snowy" "mountains".</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Studio</td> 
    <td>Fix to a bug which showed special characters in names as HTML.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

