---
description: Release Notes for the February 15, 2018 release.
seo-description: Release Notes for the February 15, 2018 release.
seo-title: February 15, 2018
solution: Experience Manager
title: February 15, 2018
---

# February 15, 2018

## New Features {#section_syx_mdt_wcb}

The following features are new in the production version of this release:

  *
  **Smart Tags.**
  
  Livefyre uses Adobe Sensei image-recognition technology to automatically tag images you save in the library.
  
  With Smart Tags you can save a significant amount of time searching and moderating content. With Smart Tags, you can:
  
    * Search saved images for precise content based on the image content, rather than only text
    * Collect content in streams based on precise search terms that analyze the image, rather than only text
  For more information about Smart Tags, see [Smart Tags](c_smart_tags.md#c_smart_tags).
  
  
* **In-product messages.** Now when you log in to Livefyre Studio, an announcements window pops up to display updates about new features.
* **UGC for Carousel.** You can now use all the functions of UGC Commerce in the Livefyre Carousel App. You can create a Call-to-Action Button and connect your product catalog to the App to create a shoppable experience from Carousel.
## Issues {#section_ehw_ndt_wcb}

The issues in the following tables were resolved in this release.

<table id="table_fbb_dxt_wcb"> 
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
    <td>Issue</td> 
    <td>ModQ</td> 
    <td>Fixed an issue where Instagram posts marked as approved or trashed were re-entering the queue.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Rights Management</td> 
    <td>Added an enhancement to display a warning when attempting to use expired Instagram accounts while making Rights Requests.</td> 
   </tr> 
   <tr> 
    <td>Issue</td> 
    <td>Trends</td> 
    <td>Fixed an issue with the Trends App still allowing HTTP at times, rather than HTTPS.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

<table id="table_ljk_5wt_wcb"> 
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
    <td>Enhancement</td> 
    <td>Apps</td> 
    <td>Added the ability to delete Apps from Livefyre.</td> 
   </tr> 
   <tr> 
    <td>Issue</td> 
    <td>Polls</td> 
    <td>Changed Polls to use HTTPS exclusively. Previously, Polls were still allowed to be used with HTTP.</td> 
   </tr> 
   <tr> 
    <td>Issue</td> 
    <td>UGC</td> 
    <td>Fixed an issue where UGC in a visualization App did not filter by Product ID as expected.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

