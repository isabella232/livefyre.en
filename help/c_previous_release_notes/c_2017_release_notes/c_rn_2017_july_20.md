---
description: Release Notes for the July 20, 2017 release.
seo-description: Release Notes for the July 20, 2017 release.
seo-title: July 20, 2017
title: July 20, 2017
uuid: b68b2857-ff0e-444b-9ed0-2720a2a3a1ac
index: y
internal: n
snippet: y
translate: y
---

# July 20, 2017

Release Notes for the July 20, 2017 release.

## New Feature {#section_swl_jsm_p1b}

UGC Commerce allows you to add a Call-to-action button directly from your Livefyre Apps. For more information on UGC Commerce, see [UGC Commerce](../../c_ugc_commerce.md#c_ugc_commerce).

## Release Notes {#section_bjq_3sm_p1b}

The following tables list the Production and UAT Release Notes for the July 20, 2017 release.

#### Production Release
<table id="table_ng5_vtz_p1b">  
 <thead> 
  <tr> 
   <th class="entry"><b>Issue Type</b></th> 
   <th class="entry"><b>Component</b></th> 
   <th class="entry"><b>Release Note</b></th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> Enhancement</td> 
   <td> All</td> 
   <td> <p>Introducing Livefyre's new UGC Commerce initiative. This includes the ability to: </p> 
    <ul id="ul_lkr_5hd_k1b"> 
     <li>Add a conversion button to Mosaic and Media Wall.</li> 
     <li>UI enhancements to Mosaic, Media Wall and the content modal for both apps.</li> 
     <li>Ability to upload products into Studio in Network Settings.</li> 
     <li>Ability to associate content with products in Studio Library, App Content and ModQ.</li> 
     <li>Ability to associate products with Stream Rules for auto-tagging.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Authentication</td> 
   <td> Fixed a bug with decoding JSON Web Tokens when authenticating into Livefyre Apps.</td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Comments</td> 
   <td> Added an enhancement so that Comments Sort Order tabs are ADA compliant.</td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Media Wall</td> 
   <td> Fixed a bug in Media Wall that was preventing the share button to work appropriately in Firefox. </td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Mosaic</td> 
   <td> Updated the look and feel to the Details modal on Mosaic cards.</td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Social Search</td> 
   <td> Added text clarifying why rights requests cannot be requested in a social search when multiple assets are selected, the social provider is not supported for rights requests, or there are no enabled rights request accounts for a social provider on the network.</td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Storify 2</td> 
   <td> Fixed an issue with not being able to add an ñ (n with a tilde over it) in Storify 2.</td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Studio</td> 
   <td> Fixed a bug to allow all Settings sections to load in Studio when scoped to a specific site.</td> 
  </tr> 
 </tbody> 
</table>

#### UAT Release
| **Issue Type** |**Component** |**Release Note** |
|---|---|---|
|  Bug | Carousel | Fixed a bug that caused Instagram Carousel posts without captions from getting pulled into Studio. |
|  Enhancement | Storify 2 | Removed the Facebook Comments by ID search option in Storify Search, due to Facebook's deprecation of the feature. |
|  Bug | Storify 2 | Improved the stability of fetching Facebook Comments by URL results in Storify 2. |
|  Bug | Streams | Fixed a bug that caused text pills in Stream Rule Configuration textboxes to be removed upon click. |
