---
description: Release Notes for the April 26, 2018 release.
seo-description: Release Notes for the April 26, 2018 release.
seo-title: April 26, 2018
solution: Experience Manager
title: April 26, 2018
---

# April 26, 2018

## New Features {#section_syx_mdt_wcb}

The following features are new in the production version of this release:

* Added a new feature that enables customers to configure a specific number of columns for a Media Wall. The number of columns you choose will force the Media Wall into that number of columns, regardless of size. Otherwise, the number of Media Wall columns defaults to "auto" where the columns adjust to a number that optimizes Media Wall for the screen size.
* In the Media Wall Designer there is now a toggle that allows you to turn off the automatic Media Wall animation that occurs when a page with a Media Wall loads.
* You can now choose the confidence threshold for smart tags in streams. Setting the precision score (0-100) for tags allows you to control the accuracy of the assets we are retrieving.
* Added moderation recommendations. Livefyre now scans every post in commenting Apps and predicts whether you will trash it or not based on historical data and machine learning. These recommendations appear in ModQ.
    * Users can turn off moderation recommendations, which allow users to filter ModQ by the content Livefyre thinks you will trash.
    * Added the ability to filter ModQ by the moderation recommendation tag, Trash.
  
## Issues {#section_ehw_ndt_wcb}

The issues in the following tables were resolved in this release.

<table id="table_dv2_vt3_qdb"> 
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
    <td>Rights Management</td> 
    <td>Fixed an issue where rights requests weren't working for Assets after finding them in a Social Search.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Streams</td> 
    <td>Updated the streaming mechanism that allows content to stream from Facebook to comply with a back-end change created by Facebook.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>UGC Commerce</td> 
    <td>Fixed an issue where the CTA "Shop" button did not display in a Mosaic or Filmstrip App or a products modal when hovering over a card with a product when the CTA button is enabled.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>UGC Commerce</td> 
    <td>Fixed an issue where the UGC Commerce flag was set to "off" by default, instead of "on."</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

<a id="section_e4q_bkl_tdb"></a>

<table id="table_jdc_f53_qdb"> 
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
    <td>Library/Search</td> 
    <td>Fixed an issue with videos not uploading properly.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Studio</td> 
    <td>Added the ability to see suggested words when typing in tag names.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

