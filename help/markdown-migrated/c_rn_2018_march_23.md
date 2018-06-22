---
description: Release Notes for the March 23, 2018 release.
seo-description: Release Notes for the March 23, 2018 release.
seo-title: March 23, 2018
solution: Experience Manager
title: March 23, 2018
---

# March 23, 2018

## New Features {#section_syx_mdt_wcb}

The following features are new in the production version of this release:

  *
  **New in Production:** Facebook created a security update to Facebook Login that will cause a customer's Facebook Login to not work correctly. To fix this issue, you must:
  
       1.
       Add the following URL to `uicontrol Valid OAuth redirect URIs` field in Client OAuth Settings. Replace `codeph &lt;networkname&gt;` with your correct network name:
       
       `codeph https://identity.livefyre.com/&lt;networkname&gt;/api/v1.0/public/profile/social/complete/facebook_fyre`
    1. Switch `uicontrol Use Strict Mode for Redirect URI` to `uicontrol Yes`.
  
  *
  **New in UAT:** You can now choose the confidence threshold for smart tags in streams. Setting the precision score (0-100) for tags allows you to control the accuracy of the assets we are retrieving.
  
  
## Issues {#section_ehw_ndt_wcb}

The issues in the following tables were resolved in this release.

<table id="table_o5x_fbn_gdb"> 
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
    <td>Media Wall</td> 
    <td>Fixed an issue in Media Wall where tags were not clickable when an Instagram post was added from a stream rule.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>ModQ</td> 
    <td>Fixed an issue with ModQ not loading properly.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>ModQ</td> 
    <td>Fixed an issue where embedding audio caused ModQ to stop working.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

<a id="section_csm_hmk_mdb"></a>

<table id="table_lkw_gbn_gdb"> 
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
    <td>Filmstrip</td> 
    <td>Fixed some issues to make Filmstrip more accessible.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Studio</td> 
    <td>You can now log into Livefyre using an IMS login.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

