---
description: Release Notes for the March 8, 2018 release.
seo-description: Release Notes for the March 8, 2018 release.
seo-title: March 8, 2018
solution: Experience Manager
title: March 8, 2018
uuid: 231aaee5-0f3f-4cc9-9bc9-72df50946950
index: y
internal: n
snippet: y
translate: y
---

# March 8, 2018

Release Notes for the March 8, 2018 release.

## New Features {#section_syx_mdt_wcb}

The following features are new in the production version of this release:

* **Deleting Apps. **Added the ability to delete Apps in Studio so users can better manage the App list. Deleting an App removes it from the table, but it does not remove the App from your site. The App will keep receiving content from a stream if it is configured to do so.

## Issues {#section_ehw_ndt_wcb}

The issues in the following tables were resolved in this release.

#### Production Release
|  **Issue Type** | **Component** | **Release Note** |
|---|---|---|
|  Bug | Polls | Changed Polls to use HTTPS exclusively. Previously, Polls were still allowed to be used with HTTP.  |
|  Bug | Studio | Fixed an issue that caused the modal window that displays announcements when you log into Studio to display too large on low resolution screens. |

#### UAT Release
<table id="table_hvf_nyp_cdb">  
 <thead> 
  <tr> 
   <th class="entry"> <b>Issue Type</b> </th> 
   <th class="entry"> <b>Component</b> </th> 
   <th class="entry"> <b>Release Note</b> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> Enhancement</td> 
   <td> Filmstrip</td> 
   <td>Updated the following accessibility features for Filmstrip: 
    <ul id="ul_z43_lzp_cdb"> 
     <li>Left/right arrows corrected from<span class="codeph"> &lt;div&gt; </span>to <span class="codeph"> &lt;button&gt;</span></li> 
     <li>Preview image element changed from a less-descriptive ARIA label of, "Open attached photo," to a label that reads the name of the platform and the post text.</li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Media Wall</td> 
   <td> Fixed an issue in Media Wall where tags were not clickable when an Instagram post was added from a stream rule.</td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Media Wall</td> 
   <td>Improved Media Wall accessibility in the following ways: 
    <ul id="ul_rzf_5zp_cdb"> 
     <li>Opening and closing modals via keyboard commands will no longer shift focus back to the top of the page. Focus instead remains on the element last focused before modal popup. </li> 
     <li>Load More button can be tabbed to and triggered using the keyboard Enter key.</li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Rights Management</td> 
   <td> Fixed an error where you couldn't see the rights request modal after rights for an Instagram asset were granted. </td> 
  </tr> 
 </tbody> 
</table>

