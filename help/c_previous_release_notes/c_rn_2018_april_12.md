---
description: Release Notes for the April 12, 2018 release.
seo-description: Release Notes for the April 12, 2018 release.
seo-title: April 12, 2018
solution: Experience Manager
title: April 12, 2018
uuid: 23d5d2c1-7507-4cee-bff6-1b09a348ad48
index: y
internal: n
snippet: y
translate: y
---

# April 12, 2018


## New Features {#section_syx_mdt_wcb}

The following features are new in the production version of this release:

You can now choose the confidence threshold for smart tags in streams. Setting the precision score (0-100) for tags allows you to control the accuracy of the assets we are retrieving.

## Issues {#section_ehw_ndt_wcb}

The issues in the following tables were resolved in this release.

#### Production Release
<table id="table_f5w_4xk_mdb">  
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
   <td> Apps</td> 
   <td> Enhanced the ability to navigate the preview modal in visualization Apps with a keyboard in Filmstrip, Mosaic, Carousel, and Media Wall.</td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Apps, Studio</td> 
   <td> Fixed an issue where users with Administrator permissions were not able to delete Apps.</td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Comments</td> 
   <td> Fixed an issue where three profile labels were pointing to one user profile, but were not identified as pointing to the same profile.</td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Feature Card</td> 
   <td> Fixed an issue where the Feature Card App did not display in the Microsoft Edge browser.</td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Filmstrip</td> 
   <td> Fixed an issue where Filmstrip fonts displayed an error.</td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Filmstrip</td> 
   <td> Fixed an issue in Filmstrip where the "Next" button was clickable, even though there was no more content to load.</td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Filmstrip</td> 
   <td> Fixed an issue where Tweets without images did not display in Filmstrip default view.</td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Filmstrip</td> 
   <td> Fixed some issues to make Filmstrip more accessible.</td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Library, Apps</td> 
   <td> Fixed an issue where videos from Instagram that were older than three months did not render correctly in the Library and Apps.</td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Media Wall</td> 
   <td> <p>Improved Media Wall accessibility in the following ways: </p> 
    <ul id="ul_tcq_r1l_mdb"> 
     <li>Opening and closing modals via keyboard commands will no longer shift focus back to the top of the page. Focus instead remains on the element last focused before modal popup. </li> 
     <li>Load More button can be tabbed to and triggered using the keyboard Enter key.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Media Wall</td> 
   <td> Fixed an issue where clicking on a Twitter, Instagram, or Facebook icon takes you to the homepage, but was incorrectly stating in screen readers that the icon takes you to the individual post. This has been fixed to identify that the icon takes you to the homepage, not the post.</td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Mosaic</td> 
   <td> Fixed an issue where a Mosaic App did not display the correct color from the App Designer.</td> 
  </tr> 
  <tr> 
   <td> Bug</td> 
   <td> Rights Management</td> 
   <td> Fixed an issue where rights requests weren't working for Assets after finding them in a Social Search.</td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Sidenotes</td> 
   <td> Fixed an issue with accessibility in the Sidenotes App where the role of the button was not clearly presented for screen reading software.</td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Studio</td> 
   <td> Fixed an issue where a modal window displayed the incorrect copy for large images.</td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> Studio</td> 
   <td> Fixed an accessibility issue to allow screen readers to read the body of modal windows.</td> 
  </tr> 
  <tr> 
   <td> Enhancement</td> 
   <td> UGC</td> 
   <td> Customers have now the ability to filter out certain products from a UGC that has multiple products associated with it. For example a UGC has 3 products associated with it, each in a different language. The customer has the ability to visualize that UGC with the specific product he /she desires in a specific page.</td> 
  </tr> 
 </tbody> 
</table>


<a id="section_crv_pq3_qdb"></a>


#### UAT Release
|  **Issue Type** | **Component** | **Release Note** |
|---|---|---|
|  Enhancement | UGC | Fixed an issue where the UGC Commerce flag was set to "off" by default, instead of "on." |
|  Enhancement | Streams | |

